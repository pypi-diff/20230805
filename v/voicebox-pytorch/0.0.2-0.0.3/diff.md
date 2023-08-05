# Comparing `tmp/voicebox-pytorch-0.0.2.tar.gz` & `tmp/voicebox-pytorch-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.2.tar", last modified: Fri Aug  4 21:33:07 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.3.tar", last modified: Fri Aug  4 22:15:07 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.2.tar` & `voicebox-pytorch-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:33:07.461498 voicebox-pytorch-0.0.2/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:15:07.791079 voicebox-pytorch-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 22:15:07.791079 voicebox-pytorch-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:15:07.791079 voicebox-pytorch-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:15:07.787079 voicebox-pytorch-0.0.3/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:15:07.787079 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.2/LICENSE` & `voicebox-pytorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.2/PKG-INFO` & `voicebox-pytorch-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.2/README.md` & `voicebox-pytorch-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,15 @@
 
 - [x] read and internalize original flow matching paper
     - [x] basic loss
     - [ ] get neural ode working with torchdyn
 - [ ] consider switching to adaptive rmsnorm for time conditioning
 - [ ] integrate with either hifi-gan or soundstream / encodec
 - [ ] basic trainer
+- [ ] get basic mask generation logic with the p_drop of 0.2-0.3 for ICL
 
 ## Citations
 
 ```bibtex
 @article{Le2023VoiceboxTM,
     title   = {Voicebox: Text-Guided Multilingual Universal Speech Generation at Scale},
     author  = {Matt Le and Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari and Rashel Moritz and Mary Williamson and Vimal Manohar and Yossi Adi and Jay Mahadeokar and Wei-Ning Hsu},
```

#### html2text {}

```diff
@@ -14,15 +14,16 @@
 phonemes = torch.randint(0, 256, (1, 1024)) mask = torch.randint(0, 2, (1,
 1024)) loss = cfm_wrapper( x, phoneme_ids = phonemes, cond = x, mask = mask )
 loss.backward() # after much training above... sampled = cfm_wrapper.sample
 ( phoneme_ids = phonemes, cond = x, mask = mask ) ``` ## Todo - [x] read and
 internalize original flow matching paper - [x] basic loss - [ ] get neural ode
 working with torchdyn - [ ] consider switching to adaptive rmsnorm for time
 conditioning - [ ] integrate with either hifi-gan or soundstream / encodec -
-[ ] basic trainer ## Citations ```bibtex @article{Le2023VoiceboxTM, title =
+[ ] basic trainer - [ ] get basic mask generation logic with the p_drop of 0.2-
+0.3 for ICL ## Citations ```bibtex @article{Le2023VoiceboxTM, title =
 {Voicebox: Text-Guided Multilingual Universal Speech Generation at Scale},
 author = {Matt Le and Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari
 and Rashel Moritz and Mary Williamson and Vimal Manohar and Yossi Adi and Jay
 Mahadeokar and Wei-Ning Hsu}, journal = {ArXiv}, year = {2023}, volume = {abs/
 2306.15687}, url = {https://api.semanticscholar.org/CorpusID:259275061} } ```
 ```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
 and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
```

### Comparing `voicebox-pytorch-0.0.2/setup.py` & `voicebox-pytorch-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
```

### Comparing `voicebox-pytorch-0.0.2/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.3/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.2/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.3/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 2% similar despite different names*

```diff
@@ -455,14 +455,29 @@
 
             num = reduce(loss, 'b n -> b', 'sum')
             den = mask.sum(dim = -1).clamp(min = 1e-5)
             loss = num / den
 
         return loss.mean()
 
+# neural ode voicebox wrapper
+
+class NeuralODEVoiceboxWrapper(Module):
+    @beartype
+    def __init__(
+        self,
+        voicebox: VoiceBox
+    ):
+        super().__init__()
+        self.voicebox = voicebox
+        self.forward_kwargs = dict()
+
+    def forward(self, t, x):
+        return self.voicebox.forward_with_cond_scale(x, times = t, **self.forward_kwargs)
+
 # wrapper for the CNF
 
 class ConditionalFlowMatcherWrapper(Module):
     @beartype
     def __init__(
         self,
         voicebox: VoiceBox,
@@ -493,34 +508,35 @@
     @torch.inference_mode()
     def sample(
         self,
         *,
         phoneme_ids,
         cond,
         mask = None,
-        steps = 18,
+        steps = 2,
         cond_scale = 1.
     ):
         self.voicebox.eval()
 
-        def voicebox_forward_with_cond_scale(t, x):
-            return self.voicebox.forward_with_cond_scale(
-                x,
-                phoneme_ids = phoneme_ids,
-                times = t,
-                cond = cond,
-                mask = mask,
-                cond_scale = cond_scale
-            )
+        wrapped_voicebox = NeuralODEVoiceboxWrapper(self.voicebox)
+
+        wrapped_voicebox.forward_kwargs = dict(
+            phoneme_ids = phoneme_ids,
+            cond = cond,
+            mask = mask,
+            cond_scale = cond_scale
+        )
 
         node = NeuralODE(
-            voicebox_forward_with_cond_scale,
+            wrapped_voicebox,
             **self.node_kwargs
         )
 
+        print('sampling...')
+
         traj = node.trajectory(
             torch.randn_like(cond),
             t_span = torch.linspace(0, 1, steps, device = self.device)
         )
 
         return traj
```

### Comparing `voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

