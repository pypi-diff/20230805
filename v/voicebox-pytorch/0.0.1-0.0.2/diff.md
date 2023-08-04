# Comparing `tmp/voicebox-pytorch-0.0.1.tar.gz` & `tmp/voicebox-pytorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voicebox-pytorch-0.0.1.tar", last modified: Fri Aug  4 20:36:57 2023, max compression
+gzip compressed data, was "voicebox-pytorch-0.0.2.tar", last modified: Fri Aug  4 21:33:07 2023, max compression
```

## Comparing `voicebox-pytorch-0.0.1.tar` & `voicebox-pytorch-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:57.760784 voicebox-pytorch-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 20:36:47.000000 voicebox-pytorch-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 20:36:57.760784 voicebox-pytorch-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-08-04 20:36:47.000000 voicebox-pytorch-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 20:36:57.760784 voicebox-pytorch-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-04 20:36:47.000000 voicebox-pytorch-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:57.760784 voicebox-pytorch-0.0.1/voicebox_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 20:36:47.000000 voicebox-pytorch-0.0.1/voicebox_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 20:36:47.000000 voicebox-pytorch-0.0.1/voicebox_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    13493 2023-08-04 20:36:47.000000 voicebox-pytorch-0.0.1/voicebox_pytorch/voicebox_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:36:57.760784 voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 20:36:57.000000 voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 20:36:57.000000 voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 20:36:57.000000 voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 20:36:57.000000 voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 20:36:57.000000 voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:33:07.461498 voicebox-pytorch-0.0.2/voicebox_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/voicebox_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/voicebox_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-08-04 21:32:53.000000 voicebox-pytorch-0.0.2/voicebox_pytorch/voicebox_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:33:07.465498 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-04 21:33:07.000000 voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/top_level.txt
```

### Comparing `voicebox-pytorch-0.0.1/LICENSE` & `voicebox-pytorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.1/PKG-INFO` & `voicebox-pytorch-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

### Comparing `voicebox-pytorch-0.0.1/README.md` & `voicebox-pytorch-0.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 ## Voicebox - Pytorch (wip)
 
 Implementation of <a href="https://arxiv.org/abs/2306.15687">Voicebox</a>, new SOTA Text-to-Speech model from MetaAI, in Pytorch. <a href="https://about.fb.com/news/2023/06/introducing-voicebox-ai-for-speech-generation/">Press release</a>
 
 In this work, we will use rotary embeddings. The authors seem unaware that ALiBi cannot be straightforwardly used for bidirectional models.
 
+## Appreciation
+
+- <a href="https://stability.ai/">StabilityAI</a> for the generous sponsorship, as well as my other sponsors, for affording me the independence to open source artificial intelligence.
+
+- <a href="https://github.com/b-chiang">Bryan Chiang</a> for the ongoing code review, sharing his expertise on TTS, and pointing me to <a href="https://github.com/atong01/conditional-flow-matching">an open sourced implementation</a> of conditional flow matching
+
 ## Install
 
 ```bash
 $ pip install voicebox-pytorch
 ```
 
 ## Usage
@@ -41,14 +47,22 @@
     x,
     phoneme_ids = phonemes,
     cond = x,
     mask = mask
 )
 
 loss.backward()
+
+# after much training above...
+
+sampled = cfm_wrapper.sample(
+    phoneme_ids = phonemes,
+    cond = x,
+    mask = mask
+)
 ```
 
 ## Todo
 
 - [x] read and internalize original flow matching paper
     - [x] basic loss
     - [ ] get neural ode working with torchdyn
```

#### html2text {}

```diff
@@ -1,26 +1,31 @@
 [./voicebox.png] ## Voicebox - Pytorch (wip) Implementation of Voicebox, new
 SOTA Text-to-Speech model from MetaAI, in Pytorch. Press_release In this work,
 we will use rotary embeddings. The authors seem unaware that ALiBi cannot be
-straightforwardly used for bidirectional models. ## Install ```bash $ pip
+straightforwardly used for bidirectional models. ## Appreciation - StabilityAI
+for the generous sponsorship, as well as my other sponsors, for affording me
+the independence to open source artificial intelligence. - Bryan_Chiang for the
+ongoing code review, sharing his expertise on TTS, and pointing me to an_open
+sourced_implementation of conditional flow matching ## Install ```bash $ pip
 install voicebox-pytorch ``` ## Usage ```python import torch from
 voicebox_pytorch.voicebox_pytorch import ( VoiceBox,
 ConditionalFlowMatcherWrapper ) model = VoiceBox( dim = 512, num_phoneme_tokens
 = 256, depth = 2, dim_head = 64, heads = 16 ) cfm_wrapper =
 ConditionalFlowMatcherWrapper( voicebox = model ) x = torch.randn(1, 1024, 512)
 phonemes = torch.randint(0, 256, (1, 1024)) mask = torch.randint(0, 2, (1,
 1024)) loss = cfm_wrapper( x, phoneme_ids = phonemes, cond = x, mask = mask )
-loss.backward() ``` ## Todo - [x] read and internalize original flow matching
-paper - [x] basic loss - [ ] get neural ode working with torchdyn - [ ]
-consider switching to adaptive rmsnorm for time conditioning - [ ] integrate
-with either hifi-gan or soundstream / encodec - [ ] basic trainer ## Citations
-```bibtex @article{Le2023VoiceboxTM, title = {Voicebox: Text-Guided
-Multilingual Universal Speech Generation at Scale}, author = {Matt Le and
-Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari and Rashel Moritz and
-Mary Williamson and Vimal Manohar and Yossi Adi and Jay Mahadeokar and Wei-Ning
-Hsu}, journal = {ArXiv}, year = {2023}, volume = {abs/2306.15687}, url =
-{https://api.semanticscholar.org/CorpusID:259275061} } ``` ```bibtex
-@inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast and
-Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri and
-Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
+loss.backward() # after much training above... sampled = cfm_wrapper.sample
+( phoneme_ids = phonemes, cond = x, mask = mask ) ``` ## Todo - [x] read and
+internalize original flow matching paper - [x] basic loss - [ ] get neural ode
+working with torchdyn - [ ] consider switching to adaptive rmsnorm for time
+conditioning - [ ] integrate with either hifi-gan or soundstream / encodec -
+[ ] basic trainer ## Citations ```bibtex @article{Le2023VoiceboxTM, title =
+{Voicebox: Text-Guided Multilingual Universal Speech Generation at Scale},
+author = {Matt Le and Apoorv Vyas and Bowen Shi and Brian Karrer and Leda Sari
+and Rashel Moritz and Mary Williamson and Vimal Manohar and Yossi Adi and Jay
+Mahadeokar and Wei-Ning Hsu}, journal = {ArXiv}, year = {2023}, volume = {abs/
+2306.15687}, url = {https://api.semanticscholar.org/CorpusID:259275061} } ```
+```bibtex @inproceedings{dao2022flashattention, title = {Flash{A}ttention: Fast
+and Memory-Efficient Exact Attention with {IO}-Awareness}, author = {Dao, Tri
+and Fu, Daniel Y. and Ermon, Stefano and Rudra, Atri and R{\'e}, Christopher},
 booktitle = {Advances in Neural Information Processing Systems}, year = {2022}
 } ```
```

### Comparing `voicebox-pytorch-0.0.1/setup.py` & `voicebox-pytorch-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'voicebox-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.0.1',
+  version = '0.0.2',
   license='MIT',
   description = 'Voicebox - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/voicebox-pytorch',
   keywords = [
```

### Comparing `voicebox-pytorch-0.0.1/voicebox_pytorch/attend.py` & `voicebox-pytorch-0.0.2/voicebox_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `voicebox-pytorch-0.0.1/voicebox_pytorch/voicebox_pytorch.py` & `voicebox-pytorch-0.0.2/voicebox_pytorch/voicebox_pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -389,14 +389,22 @@
         times,
         cond_drop_prob = 0.1,
         target = None,
         mask = None,
     ):
         assert cond.shape[-1] == x.shape[-1]
 
+        # auto manage shape of times, for node.traj
+
+        if times.ndim == 0:
+            times = repeat(times, '-> b', b = cond.shape[0])
+
+        if times.ndim == 1 and times.shape[0] == 1:
+            times = repeat(times, '1 -> b', b = cond.shape[0])
+
         # classifier free guidance
 
         if cond_drop_prob > 0.:
             cond_drop_mask = prob_mask_like(cond.shape[:1], cond_drop_prob, cond.device)
 
             cond = torch.where(
                 rearrange(cond_drop_mask, '... -> ... 1 1'),
@@ -458,28 +466,68 @@
     def __init__(
         self,
         voicebox: VoiceBox,
         sigma = 0.,
         node_solver = 'dopri5',
         node_sensitivity = 'adjoint',
         node_atol = 1e-5,
-        node_rtol = 1e-5
+        node_rtol = 1e-5,
+        cond_drop_prob = 0.
     ):
         super().__init__()
         self.sigma = sigma
+
         self.voicebox = voicebox
+        self.cond_drop_prob = cond_drop_prob
 
-        self.node = NeuralODE(
-            voicebox,
+        self.node_kwargs = dict(
             solver = node_solver,
             sensitivity = node_sensitivity,
             atol = node_atol,
             rtol = node_rtol
         )
 
+    @property
+    def device(self):
+        return next(self.parameters()).device
+
+    @torch.inference_mode()
+    def sample(
+        self,
+        *,
+        phoneme_ids,
+        cond,
+        mask = None,
+        steps = 18,
+        cond_scale = 1.
+    ):
+        self.voicebox.eval()
+
+        def voicebox_forward_with_cond_scale(t, x):
+            return self.voicebox.forward_with_cond_scale(
+                x,
+                phoneme_ids = phoneme_ids,
+                times = t,
+                cond = cond,
+                mask = mask,
+                cond_scale = cond_scale
+            )
+
+        node = NeuralODE(
+            voicebox_forward_with_cond_scale,
+            **self.node_kwargs
+        )
+
+        traj = node.trajectory(
+            torch.randn_like(cond),
+            t_span = torch.linspace(0, 1, steps, device = self.device)
+        )
+
+        return traj
+
     def forward(
         self,
         x1,
         *,
         phoneme_ids,
         cond,
         mask = None,
@@ -491,20 +539,20 @@
         batch, dtype = x1.shape[0], x1.dtype
 
         x0 = torch.randn_like(x1)
 
         # random times
 
         times = torch.rand((batch,), dtype = dtype)
+        padded_times = rearrange(times, 'b -> b 1 1')
 
         # sample xt
 
-        mu_t = times * x1
-        sigma_t = 1 - (1 - self.sigma) * times
-        sigma_t = rearrange(sigma_t, 'b -> b 1 1')
+        mu_t = padded_times * x1
+        sigma_t = 1 - (1 - self.sigma) * padded_times
 
         eps = torch.rand_like(x1)
         xt = mu_t * sigma_t * eps
 
         conditional_flow = (x1 - (1 - self.sigma) * xt) / sigma_t
 
         # predict
@@ -513,11 +561,12 @@
 
         loss = self.voicebox(
             xt,
             phoneme_ids = phoneme_ids,
             cond = cond,
             mask = mask,
             times = times,
-            target = conditional_flow
+            target = conditional_flow,
+            cond_drop_prob = self.cond_drop_prob
         )
 
         return loss
```

### Comparing `voicebox-pytorch-0.0.1/voicebox_pytorch.egg-info/PKG-INFO` & `voicebox-pytorch-0.0.2/voicebox_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: voicebox-pytorch
-Version: 0.0.1
+Version: 0.0.2
 Summary: Voicebox - Pytorch
 Home-page: https://github.com/lucidrains/voicebox-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,text to speech
 Classifier: Development Status :: 4 - Beta
```

