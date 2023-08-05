# Comparing `tmp/voicebox-pytorch-0.0.3.tar.gz` & `tmp/voicebox-pytorch-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.3.tar", last modified: Fri Aug  4 22:15:07 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.4.tar", last modified: Sat Aug  5 16:48:05 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.3.tar` & `voicebox-pytorch-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:15:07.791079 voicebox-pytorch-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 22:15:07.791079 voicebox-pytorch-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:15:07.791079 voicebox-pytorch-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:15:07.787079 voicebox-pytorch-0.0.3/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15082 2023-08-04 22:14:58.000000 voicebox-pytorch-0.0.3/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:15:07.787079 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 22:15:07.000000 voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16225 2023-08-05 16:47:49.000000 voicebox-pytorch-0.0.4/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:48:05.487434 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 16:48:05.000000 voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.3/LICENSE` & `voicebox-pytorch-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.3/PKG-INFO` & `voicebox-pytorch-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.3/README.md` & `voicebox-pytorch-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.3/setup.py` & `voicebox-pytorch-0.0.4/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.3',
+  version = '0.0.4',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
@@ -15,15 +15,16 @@
     'deep learning',
     'text to speech'
   ],
   install_requires=[
     'beartype',
     'einops>=0.6.1',
     'torch>=2.0',
-    'torchdyn==1.0.3'
+    'torchdyn==1.0.3',
+    'torchode'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
     'Programming Language :: Python :: 3.6',
```

### Comparing `voicebox-pytorch-0.0.3/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.4/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.3/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.4/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,14 +32,47 @@
     if prob == 1:
         return torch.ones(shape, device = device, dtype = torch.bool)
     elif prob == 0:
         return torch.zeros(shape, device = device, dtype = torch.bool)
     else:
         return torch.zeros(shape, device = device).float().uniform_(0, 1) < prob
 
+# mask construction helpers
+
+def mask_from_start_end_indices(
+    seq_len: int,
+    start: Tensor,
+    end: Tensor
+):
+    assert start.shape == end.shape
+    device = start.device
+
+    seq = torch.arange(seq_len, device = device, dtype = torch.long)
+    seq = seq.reshape(*((-1,) * start.ndim), seq_len)
+    seq = seq.expand(*start.shape, seq_len)
+
+    mask = seq >= start[..., None].long()
+    mask &= seq < end[..., None].long()
+    return mask
+
+def mask_from_frac_lengths(
+    seq_len: int,
+    frac_lengths: Tensor
+):
+    device = frac_lengths
+
+    lengths = (frac_lengths * seq_len).long()
+    max_start = seq_len - lengths
+
+    rand = torch.zeros_like(frac_lengths).float().uniform_(0, 1)
+    start = (max_start * rand).clamp(min = 0)
+    end = start + lengths
+
+    return mask_from_start_end_indices(seq_len, start, end)
+
 # sinusoidal positions
 
 class LearnedSinusoidalPosEmb(Module):
     """ used by @crowsonkb """
 
     def __init__(self, dim):
         super().__init__()
@@ -308,23 +341,22 @@
         x = self.transformer(x)
 
         if not exists(mask):
             return F.l1_loss(x, target)
 
         loss = F.l1_loss(x, target, reduction = 'none')
 
-        if exists(mask):
-            loss = reduce(loss, 'b n d -> b n', 'mean')
-            loss = loss.masked_fill(mask, 0.)
-
-            # masked mean
-
-            num = reduce(loss, 'b n -> b', 'sum')
-            den = mask.sum(dim = -1).clamp(min = 1e-5)
-            loss = num / den
+        loss = reduce(loss, 'b n d -> b n', 'mean')
+        loss = loss.masked_fill(mask, 0.)
+
+        # masked mean
+
+        num = reduce(loss, 'b n -> b', 'sum')
+        den = mask.sum(dim = -1).clamp(min = 1e-5)
+        loss = num / den
 
         return loss.mean()
 
 
 class VoiceBox(Module):
     def __init__(
         self,
@@ -443,23 +475,22 @@
             return x
 
         if not exists(mask):
             return F.mse_loss(x, target)
 
         loss = F.mse_loss(x, target, reduction = 'none')
 
-        if exists(mask):
-            loss = reduce(loss, 'b n d -> b n', 'mean')
-            loss = loss.masked_fill(mask, 0.)
-
-            # masked mean
-
-            num = reduce(loss, 'b n -> b', 'sum')
-            den = mask.sum(dim = -1).clamp(min = 1e-5)
-            loss = num / den
+        loss = reduce(loss, 'b n d -> b n', 'mean')
+        loss = loss.masked_fill(mask, 0.)
+
+        # masked mean
+
+        num = reduce(loss, 'b n -> b', 'sum')
+        den = mask.sum(dim = -1).clamp(min = 1e-5)
+        loss = num / den
 
         return loss.mean()
 
 # neural ode voicebox wrapper
 
 class NeuralODEVoiceboxWrapper(Module):
     @beartype
@@ -482,22 +513,25 @@
         self,
         voicebox: VoiceBox,
         sigma = 0.,
         node_solver = 'dopri5',
         node_sensitivity = 'adjoint',
         node_atol = 1e-5,
         node_rtol = 1e-5,
-        cond_drop_prob = 0.
+        cond_drop_prob = 0.,
+        prob_seq_drop = 0.3  # not entirely sure
     ):
         super().__init__()
         self.sigma = sigma
 
         self.voicebox = voicebox
         self.cond_drop_prob = cond_drop_prob
 
+        self.prob_seq_drop = prob_seq_drop
+
         self.node_kwargs = dict(
             solver = node_solver,
             sensitivity = node_sensitivity,
             atol = node_atol,
             rtol = node_rtol
         )
 
@@ -548,41 +582,51 @@
         cond,
         mask = None,
     ):
         """
         following the example put forth
         https://github.com/atong01/conditional-flow-matching/blob/main/torchcfm/conditional_flow_matching.py#L248
         """
-        batch, dtype = x1.shape[0], x1.dtype
+        batch, seq_len, dtype = *x1.shape[:2], x1.dtype
 
         x0 = torch.randn_like(x1)
 
         # random times
 
         times = torch.rand((batch,), dtype = dtype)
         padded_times = rearrange(times, 'b -> b 1 1')
 
         # sample xt
 
         mu_t = padded_times * x1
         sigma_t = 1 - (1 - self.sigma) * padded_times
 
         eps = torch.rand_like(x1)
-        xt = mu_t * sigma_t * eps
+        xt = mu_t + sigma_t * eps
+
+        flow = (x1 - (1 - self.sigma) * xt) / sigma_t
+
+        # construct mask if not given
 
-        conditional_flow = (x1 - (1 - self.sigma) * xt) / sigma_t
+        if (
+            not exists(mask) and
+            exists(self.prob_seq_drop) and
+            self.prob_seq_drop > 0.
+        ):
+            frac_lengths = torch.full((batch,), self.prob_seq_drop, device = self.device)
+            mask = mask_from_frac_lengths(seq_len, frac_lengths)
 
         # predict
 
         self.voicebox.train()
 
         loss = self.voicebox(
             xt,
             phoneme_ids = phoneme_ids,
             cond = cond,
             mask = mask,
             times = times,
-            target = conditional_flow,
+            target = flow,
             cond_drop_prob = self.cond_drop_prob
         )
 
         return loss
```

### Comparing `voicebox-pytorch-0.0.3/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.4/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.3
+Version: 0.0.4
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

