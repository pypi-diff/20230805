# Comparing `tmp/dispersenn2-0.0.4.tar.gz` & `tmp/dispersenn2-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dispersenn2-0.0.4.tar", max compression
+gzip compressed data, was "dispersenn2-0.0.5.tar", max compression
```

## Comparing `dispersenn2-0.0.4.tar` & `dispersenn2-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      599 2023-07-28 19:39:37.121430 dispersenn2-0.0.4/README.md
--rw-r--r--   0        0        0        0 2023-07-27 20:51:57.445326 dispersenn2-0.0.4/disperseNN2/__init__.py
--rw-r--r--   0        0        0     2210 2023-07-27 22:45:44.334779 dispersenn2-0.0.4/disperseNN2/check_params.py
--rw-r--r--   0        0        0    13167 2023-07-29 23:32:56.018528 dispersenn2-0.0.4/disperseNN2/data_generation.py
--rw-r--r--   0        0        0    24859 2023-07-29 23:33:11.150694 dispersenn2-0.0.4/disperseNN2/disperseNN2.py
--rw-r--r--   0        0        0     7097 2023-07-29 23:33:24.482841 dispersenn2-0.0.4/disperseNN2/process_input.py
--rw-r--r--   0        0        0     3824 2023-07-27 20:51:57.445326 dispersenn2-0.0.4/disperseNN2/read_input.py
--rw-r--r--   0        0        0      620 2023-07-29 23:41:53.716020 dispersenn2-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1429 1970-01-01 00:00:00.000000 dispersenn2-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      655 2023-08-04 15:39:21.198344 dispersenn2-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-07-29 23:49:27.492759 dispersenn2-0.0.5/disperseNN2/__init__.py
+-rw-r--r--   0        0        0     2210 2023-07-29 23:49:27.492759 dispersenn2-0.0.5/disperseNN2/check_params.py
+-rw-r--r--   0        0        0    13331 2023-08-04 16:13:00.159428 dispersenn2-0.0.5/disperseNN2/data_generation.py
+-rw-r--r--   0        0        0    24859 2023-07-29 23:49:27.496759 dispersenn2-0.0.5/disperseNN2/disperseNN2.py
+-rw-r--r--   0        0        0     7097 2023-07-29 23:49:27.496759 dispersenn2-0.0.5/disperseNN2/process_input.py
+-rw-r--r--   0        0        0     3824 2023-07-29 23:49:27.496759 dispersenn2-0.0.5/disperseNN2/read_input.py
+-rw-r--r--   0        0        0      620 2023-08-04 15:57:47.190076 dispersenn2-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1485 1970-01-01 00:00:00.000000 dispersenn2-0.0.5/PKG-INFO
```

### Comparing `dispersenn2-0.0.4/README.md` & `dispersenn2-0.0.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # disperseNN2
 
 [![Documentation Status](https://readthedocs.org/projects/dispersenn2/badge/?version=latest)](https://dispersenn2.readthedocs.io/en/latest/?badge=latest)
 
 `disperseNN2` is a machine learning framework for predicting &#963;, the expected per generation displacement distance between offspring and their parent(s), from genetic variation data.
 `disperseNN2` replaces our previous method, `disperseNN`, by introducing
-a novel architecture. For details see our preprint (LINK).
+a novel architecture. For details see our [preprint](https://www.biorxiv.org/content/10.1101/2023.07.30.551115v1).
 
 For installation and usage instructions, see the [docs page](https://dispersenn2.readthedocs.io/en/latest/).
```

### Comparing `dispersenn2-0.0.4/disperseNN2/check_params.py` & `dispersenn2-0.0.5/disperseNN2/check_params.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.4/disperseNN2/data_generation.py` & `dispersenn2-0.0.5/disperseNN2/data_generation.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,20 +362,30 @@
 
     def __data_generation(self, list_IDs_temp):
         "Generates data containing batch_size samples"
         X1 = np.empty((self.batch_size, self.num_snps, self.n), dtype="int8")
         X2 = np.empty((self.batch_size, 2, self.n), dtype=float)
         y = np.empty((self.batch_size,), dtype=float)
         shuffled_indices = np.arange(self.n)
-        np.random.shuffle(shuffled_indices)
+        np.random.shuffle(shuffled_indices)  # augment training set
         for i, ID in enumerate(list_IDs_temp):
+            # load target
             y[i] = np.load(self.targets[ID])
+
+            # load and re-order genos
             genomat = np.load(self.genos[ID])
             genomat = genomat[
                 :, shuffled_indices
-            ]  # shuffe augments training set; especially pairs_encode<pairs
+            ]
             X1[i, :] = genomat
-            X2[i, :] = np.load(self.locs[ID])
+
+            # load and re-order locs
+            locs = np.load(self.locs[ID])
+            locs = locs[
+                :, shuffled_indices
+            ]
+            X2[i, :] = locs
+
         # (unindent)
         X = [X1, X2]
 
         return (X, y)
```

### Comparing `dispersenn2-0.0.4/disperseNN2/disperseNN2.py` & `dispersenn2-0.0.5/disperseNN2/disperseNN2.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.4/disperseNN2/process_input.py` & `dispersenn2-0.0.5/disperseNN2/process_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.4/disperseNN2/read_input.py` & `dispersenn2-0.0.5/disperseNN2/read_input.py`

 * *Files identical despite different names*

### Comparing `dispersenn2-0.0.4/pyproject.toml` & `dispersenn2-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "disperseNN2"
 packages = [
     {include = "disperseNN2"}
 ]
-version = "0.0.4"
+version = "0.0.5"
 description = "Neural net for estimating dispersal distance"
 authors = ["chriscrsmith <chriscs@uoregon.edu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.12"
 gpustat = "^1.1"
```

### Comparing `dispersenn2-0.0.4/PKG-INFO` & `dispersenn2-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dispersenn2
-Version: 0.0.4
+Version: 0.0.5
 Summary: Neural net for estimating dispersal distance
 Author: chriscrsmith
 Author-email: chriscs@uoregon.edu
 Requires-Python: >=3.9,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -23,11 +23,11 @@
 
 # disperseNN2
 
 [![Documentation Status](https://readthedocs.org/projects/dispersenn2/badge/?version=latest)](https://dispersenn2.readthedocs.io/en/latest/?badge=latest)
 
 `disperseNN2` is a machine learning framework for predicting &#963;, the expected per generation displacement distance between offspring and their parent(s), from genetic variation data.
 `disperseNN2` replaces our previous method, `disperseNN`, by introducing
-a novel architecture. For details see our preprint (LINK).
+a novel architecture. For details see our [preprint](https://www.biorxiv.org/content/10.1101/2023.07.30.551115v1).
 
 For installation and usage instructions, see the [docs page](https://dispersenn2.readthedocs.io/en/latest/).
```

