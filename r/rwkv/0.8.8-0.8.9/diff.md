# Comparing `tmp/rwkv-0.8.8.tar.gz` & `tmp/rwkv-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rwkv-0.8.8.tar", last modified: Fri Aug  4 03:30:22 2023, max compression
+gzip compressed data, was "rwkv-0.8.9.tar", last modified: Sat Aug  5 05:35:55 2023, max compression
```

## Comparing `rwkv-0.8.8.tar` & `rwkv-0.8.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.8/LICENSE
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.8/MANIFEST.in
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-08-04 03:30:22.000000 rwkv-0.8.8/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.8/README.md
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-08-04 03:29:43.000000 rwkv-0.8.8/pyproject.toml
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-08-04 03:30:22.000000 rwkv-0.8.8/setup.cfg
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.8/src/rwkv/__init__.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv/cuda/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3633 2023-08-04 03:28:50.000000 rwkv-0.8.8/src/rwkv/cuda/gemm_fp16_cublas.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.8/src/rwkv/cuda/operators.cu
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5002 2023-07-29 09:25:30.000000 rwkv-0.8.8/src/rwkv/cuda/wrapper.cpp
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    40726 2023-07-29 09:29:04.000000 rwkv-0.8.8/src/rwkv/model.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.8/src/rwkv/rwkv_tokenizer.py
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.8/src/rwkv/rwkv_vocab_v20230424.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.8/src/rwkv/utils.py
-drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/PKG-INFO
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/SOURCES.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/dependency_links.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/requires.txt
--rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-08-04 03:30:22.000000 rwkv-0.8.8/src/rwkv.egg-info/top_level.txt
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-05 05:35:55.000000 rwkv-0.8.9/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    11357 2023-03-01 07:25:16.000000 rwkv-0.8.9/LICENSE
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       47 2023-05-19 16:15:03.000000 rwkv-0.8.9/MANIFEST.in
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-08-05 05:35:55.000000 rwkv-0.8.9/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4372 2023-06-26 03:17:49.000000 rwkv-0.8.9/README.md
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      499 2023-08-05 05:32:51.000000 rwkv-0.8.9/pyproject.toml
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       38 2023-08-05 05:35:55.000000 rwkv-0.8.9/setup.cfg
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-02-28 12:56:58.000000 rwkv-0.8.9/src/rwkv/__init__.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv/cuda/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3633 2023-08-04 03:28:50.000000 rwkv-0.8.9/src/rwkv/cuda/gemm_fp16_cublas.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     8677 2023-04-27 19:18:02.000000 rwkv-0.8.9/src/rwkv/cuda/operators.cu
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5002 2023-07-29 09:25:30.000000 rwkv-0.8.9/src/rwkv/cuda/wrapper.cpp
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)    41203 2023-08-05 05:32:42.000000 rwkv-0.8.9/src/rwkv/model.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     3201 2023-06-10 18:48:52.000000 rwkv-0.8.9/src/rwkv/rwkv_tokenizer.py
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)  1093733 2023-05-18 04:00:58.000000 rwkv-0.8.9/src/rwkv/rwkv_vocab_v20230424.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     5356 2023-06-26 03:07:02.000000 rwkv-0.8.9/src/rwkv/utils.py
+drwxr-xr-x   0 blinkdl  (424401630) Domain Users (424400513)        0 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv.egg-info/
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)     4842 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv.egg-info/PKG-INFO
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)      409 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv.egg-info/SOURCES.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        1 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv.egg-info/dependency_links.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)       19 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv.egg-info/requires.txt
+-rw-r--r--   0 blinkdl  (424401630) Domain Users (424400513)        5 2023-08-05 05:35:55.000000 rwkv-0.8.9/src/rwkv.egg-info/top_level.txt
```

### Comparing `rwkv-0.8.8/LICENSE` & `rwkv-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/PKG-INFO` & `rwkv-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.8
+Version: 0.8.9
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `rwkv-0.8.8/README.md` & `rwkv-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv/cuda/gemm_fp16_cublas.cpp` & `rwkv-0.8.9/src/rwkv/cuda/gemm_fp16_cublas.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv/cuda/operators.cu` & `rwkv-0.8.9/src/rwkv/cuda/operators.cu`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv/cuda/wrapper.cpp` & `rwkv-0.8.9/src/rwkv/cuda/wrapper.cpp`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv/model.py` & `rwkv-0.8.9/src/rwkv/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,14 +245,22 @@
                     w['emb.weight'] = F.layer_norm(w['emb.weight'], (args.n_embd,), weight=w['blocks.0.ln0.weight'], bias=w['blocks.0.ln0.bias'])
                 except:
                     w['emb.weight'] = F.layer_norm(w['emb.weight'].float(), (args.n_embd,), weight=w['blocks.0.ln0.weight'].float(), bias=w['blocks.0.ln0.bias'].float())
                 del w['blocks.0.ln0.weight']
                 del w['blocks.0.ln0.bias']
 
             print_need_newline = False
+
+            REAL_TIME_FIRST = False
+            for x in list(w.keys()):
+                if '.time_faaaa' in x: REAL_TIME_FIRST = True
+            if REAL_TIME_FIRST:
+                w = {k.replace('.time_faaaa','.time_first') if '.time_faaaa' in k else k: v for k, v in w.items()}
+                self.w = w
+            
             keys = list(w.keys())
             for x in keys:
                 w[x].requires_grad = False
                 layer_id = int(x.split('.')[1]) if ('blocks.' in x) else 0
                 if ('ln_out.' in x) or ('head.' in x):
                     layer_id = args.n_layer
                 dd = strategy[layer_id]
@@ -277,15 +285,18 @@
                             w[x] = -torch.exp(w[x].float())
                         elif self.version == 5:
                             w[x] = torch.exp(-torch.exp(w[x].float())).reshape(-1,1,1)
                     elif '.time_first' in x: # need fp32 for this
                         if self.version == 4:
                             w[x] = w[x].float()
                         elif self.version == 5:
-                            w[x] = torch.exp(w[x].float()).reshape(-1,1,1)
+                            if REAL_TIME_FIRST:
+                                w[x] = w[x].float().reshape(-1,1,1)
+                            else:
+                                w[x] = torch.exp(w[x].float()).reshape(-1,1,1)
                     elif '.ln_x' in x: # need fp32 for group_norm
                         w[x] = w[x].float()
                     else:
                         if (len(w[x].shape) == 2) and ('emb' not in x):
                             if WTYPE != torch.uint8:
                                 w[x] = w[x].to(dtype=WTYPE)
                             else:
```

### Comparing `rwkv-0.8.8/src/rwkv/rwkv_tokenizer.py` & `rwkv-0.8.9/src/rwkv/rwkv_tokenizer.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv/rwkv_vocab_v20230424.txt` & `rwkv-0.8.9/src/rwkv/rwkv_vocab_v20230424.txt`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv/utils.py` & `rwkv-0.8.9/src/rwkv/utils.py`

 * *Files identical despite different names*

### Comparing `rwkv-0.8.8/src/rwkv.egg-info/PKG-INFO` & `rwkv-0.8.9/src/rwkv.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rwkv
-Version: 0.8.8
+Version: 0.8.9
 Summary: The RWKV Language Model
 Author: Bo PENG
 Project-URL: Homepage, https://github.com/BlinkDL/ChatRWKV
 Project-URL: Bug Tracker, https://github.com/BlinkDL/ChatRWKV/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

