# Comparing `tmp/perming-1.4.3-py3-none-any.whl.zip` & `tmp/perming-1.5.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 13756 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat      887 b- defN 23-Jul-24 13:50 perming/__init__.py
+Zip file size: 13801 bytes, number of entries: 10
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Aug-05 13:00 perming/__init__.py
 -rw-rw-rw-  2.0 fat      176 b- defN 23-May-29 15:03 perming/_typing.py
--rw-rw-rw-  2.0 fat    22971 b- defN 23-Jul-24 14:04 perming/_utils.py
+-rw-rw-rw-  2.0 fat    23104 b- defN 23-Aug-05 14:05 perming/_utils.py
 -rw-rw-rw-  2.0 fat      568 b- defN 23-May-29 16:53 perming/_version.py
 -rw-rw-rw-  2.0 fat    13949 b- defN 23-Jul-24 14:08 perming/common.py
 -rw-rw-rw-  2.0 fat     5605 b- defN 23-Jul-13 07:33 perming/general.py
--rw-rw-rw-  2.0 fat    10828 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat      747 b- defN 23-Jul-24 14:19 perming-1.4.3.dist-info/RECORD
-10 files, 55831 bytes uncompressed, 12502 bytes compressed:  77.6%
+-rw-rw-rw-  2.0 fat    10828 b- defN 23-Aug-05 14:29 perming-1.5.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 14:29 perming-1.5.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-05 14:29 perming-1.5.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 fat      747 b- defN 23-Aug-05 14:29 perming-1.5.0.dist-info/RECORD
+10 files, 55964 bytes uncompressed, 12547 bytes compressed:  77.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: perming/common.py
 Comment: 
 
 Filename: perming/general.py
 Comment: 
 
-Filename: perming-1.4.3.dist-info/METADATA
+Filename: perming-1.5.0.dist-info/METADATA
 Comment: 
 
-Filename: perming-1.4.3.dist-info/WHEEL
+Filename: perming-1.5.0.dist-info/WHEEL
 Comment: 
 
-Filename: perming-1.4.3.dist-info/top_level.txt
+Filename: perming-1.5.0.dist-info/top_level.txt
 Comment: 
 
-Filename: perming-1.4.3.dist-info/RECORD
+Filename: perming-1.5.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perming/__init__.py

```diff
@@ -23,8 +23,8 @@
 COMMON_MODELS = {
     'Regression': Regressier,
     'Binary-classification': Binarier,
     'Multi-classification': Mutipler,
     'Multi-outputs': Ranker
 }
 
-__version__ = '1.4.3'
+__version__ = '1.5.0'
```

## perming/_utils.py

```diff
@@ -162,14 +162,15 @@
         assert ratio_set['train'] + ratio_set['test'] + ratio_set['val'] == 10, 'The sum of 3 datasets ratio needs to be 10.'
         assert isinstance(features, TabularData) and features.ndim == 2, 'Please ensure features with dimension at (n_samples, n_features).'
         assert features.shape[1] == self.input, 'Please ensure `input_` is equal to `features.shape[1]`.'
         assert isinstance(target, TabularData), 'Please ensure target format at numpy.ndarray noted as TabularData.'
         target_dtype = str(target.dtype) # __str__
         is_int_type, is_float_type = 'int' in target_dtype, 'float' in target_dtype
         self.is_target_2d = isinstance(target[0], TabularData) # judge target is 2d matrix.
+        self.is_task_c1d = not self.is_target_2d and self.num_classes >= 2 # if task is 1d classification
         if self.is_target_2d: # (n_samples, n_outputs)
             assert target.shape[1] == self.num_classes, 'Please ensure target with (n_samples, n_outputs=num_classes).'
             assert is_int_type or is_float_type, 'Please ensure target.dtype in any int or float type of numpy.dtype.'
             roc: bool = not is_int_type and is_float_type
         else: # (n_samples,)
             if self.num_classes >= 2:
                 self.unique = numpy.unique(target) # int indexes -> any class with single value noted
@@ -257,36 +258,37 @@
                 print('Process stop at epoch [{}/{}] with patience {} within tolerance {}'.format(epoch+1, num_epochs, patience, tolerance))
                 break
 
     def test(self, 
              sort_by: str='accuracy',
              sort_state: bool=True):
         '''
-        Test with Initialized Configuration. `accuracy > 0`, 'correct_class != None'
         Configured keywords only work when `not self.is_target_2d and num_classes >= 2`.
+        Produce `self.aver_acc != 0` and 'correct_class != None' in the above condition.
         :param sort_by: str, 'accuracy', 'numbers', 'num-total'. default: 'accuracy'.
         :param sort_state: bool, whether to use descending order when sorting. default: True.
         '''
         with torch.no_grad():
             self.test_loss, test_loader_step, correct = 0, len(self.test_loader), 0
             test_total = test_loader_step * self.batch_size
-            self.correct_class = dict.fromkeys(self.unique, [0, 0]) if not self.is_target_2d and self.num_classes >= 2 else None
+            self.correct_class = dict.fromkeys(self.unique, [0, 0]) if self.is_task_c1d else None
             for features, target in self.test_loader:
                 features = features.to(self.device)
                 target = target.to(self.device)            
                 outputs = self.model(features)
-                if not self.is_target_2d and self.num_classes >= 2:
+                if self.is_task_c1d:
                     _, predicted = torch.max(outputs.data, 1)
                     for index, value in enumerate(predicted):
                         self.correct_class[self.unique[value]][1] += 1 # record total numbers of each class
                         self.correct_class[self.unique[value]][0] += (value == target[index]).item() # record total true numbers of each class
                     correct += (predicted == target).sum().item()
                 self.test_loss += self.criterion(outputs, target)
             self.test_loss /= test_loader_step
-            print('loss of {0} on the {1} test dataset: {2}. accuracy: {3:.4f} %'.format(self.__class__.__name__, test_total, self.test_loss.item(), 100 * correct / test_total))
+            self.aver_acc = 100 * correct / test_total if self.is_task_c1d else None
+            print('loss of {0} on the {1} test dataset: {2}.'.format(self.__class__.__name__, test_total, self.test_loss.item()))
         return OrderedDict(self._pack_info(sort_by, sort_state))
 
     def save(self, show: bool=True, dir: str='./model') -> None:
         '''
         Save Model Checkpoint with Box, Regressier, Binarier, Multipler, and Ranker.
         :param show: bool, whether to show `model.state_dict()`. default: True.
         :param dir: str, model save to dir. default: './model'.
@@ -313,14 +315,15 @@
         :param state: bool, choose the state when `correct_class` is sorting.
         '''
         loss_, classify, regress, outputs = {
             'loss': {'train': self.train_loss.item(), 
                      'val': self.val_loss.item(),
                      'test': self.test_loss.item()}
         }, {'problem': 'classification',
+            'accuracy': f'{self.aver_acc}%',
             'num_classes': self.num_classes,
             'column': ('label name', ('true numbers', 'total numbers')),
             'labels': self.correct_class}, {'problem': 'regression'}, {'problem': 'multi-outputs'}
         if not self.is_target_2d and self.num_classes >= 2:
             classify.update(loss_)
             if by == 'numbers':
                 classify.update({'sorted': sorted(self.correct_class.items(), key=lambda d: d[1][0], reverse=state)})
```

## Comparing `perming-1.4.3.dist-info/METADATA` & `perming-1.5.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perming
-Version: 1.4.3
+Version: 1.5.0
 Summary: The supervised learning framework based on perceptron for tabular data.
 Home-page: https://github.com/linjing-lab/easy-pytorch/tree/main/released_box
 Download-URL: https://github.com/linjing-lab/easy-pytorch/tags
 Author: 林景
 Author-email: linjing010729@163.com
 License: MPL 2.0
 Project-URL: Source, https://github.com/linjing-lab/easy-pytorch/tree/main/released_box/perming
```

## Comparing `perming-1.4.3.dist-info/RECORD` & `perming-1.5.0.dist-info/RECORD`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perming/__init__.py,sha256=iLONaHLqN3t0omi27mthtNVzohjSYYyFVGXgH_XWuCE,887
+perming/__init__.py,sha256=Rl8MisLDfEfUO36SE2fGZKljy450jNQuayrjzMYWvwI,887
 perming/_typing.py,sha256=SGQP3QKfMZr-ciHT6jIrv4NUDmgqkx-RhYxIQloBSC4,176
-perming/_utils.py,sha256=mOG_39IpZdBbuq4W9b7iS5_rqNKh7H8RzPLQ5T3bzks,22971
+perming/_utils.py,sha256=Jkp5GIVXNGKkkvl6RRMOQdobFUjN9dvvr0JQSg4DAsI,23104
 perming/_version.py,sha256=K3CPQxLgHmXPNpNWlhpnrp6Bt8v5rU9wZyVRBsRTI3E,568
 perming/common.py,sha256=X_n-3VxTkPbt8NJJWe1SeorolebHkK-UhsLhEi3viq8,13949
 perming/general.py,sha256=sUjieRqdWa3o6PXdici5ABarVHcBTCVuv1Wg2K1kggI,5605
-perming-1.4.3.dist-info/METADATA,sha256=IE8AFkdhJ0St1bMs0Q2xVCJuGgwOacNzuD9qtHP4HXc,10828
-perming-1.4.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-perming-1.4.3.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
-perming-1.4.3.dist-info/RECORD,,
+perming-1.5.0.dist-info/METADATA,sha256=qz5T2vSnxW12q9AjfubpuAowCaF-0owqc1gC-E5dxdY,10828
+perming-1.5.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+perming-1.5.0.dist-info/top_level.txt,sha256=mxFGHPJW81IzoNdyMqNWWZA7gUBzz0RtiAw5cQ0qzX8,8
+perming-1.5.0.dist-info/RECORD,,
```

