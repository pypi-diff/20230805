# Comparing `tmp/numba-integrators-0.0.3.tar.gz` & `tmp/numba-integrators-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numba-integrators-0.0.3.tar", last modified: Sat May 13 21:19:01 2023, max compression
+gzip compressed data, was "numba-integrators-0.1.1.tar", last modified: Sat Aug  5 19:47:27 2023, max compression
```

## Comparing `numba-integrators-0.0.3.tar` & `numba-integrators-0.1.1.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:19:01.992125 numba-integrators-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-13 21:19:01.992125 numba-integrators-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:19:01.992125 numba-integrators-0.0.3/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/dependencies/build.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/dependencies/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/dependencies/main.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-13 21:18:54.000000 numba-integrators-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 21:19:01.992125 numba-integrators-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:19:01.988125 numba-integrators-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:19:01.992125 numba-integrators-0.0.3/src/numba_integrators/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/src/numba_integrators/_API.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-13 21:18:29.000000 numba-integrators-0.0.3/src/numba_integrators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 21:19:01.992125 numba-integrators-0.0.3/src/numba_integrators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-05-13 21:19:01.000000 numba-integrators-0.0.3/src/numba_integrators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-13 21:19:01.000000 numba-integrators-0.0.3/src/numba_integrators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 21:19:01.000000 numba-integrators-0.0.3/src/numba_integrators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-13 21:19:01.000000 numba-integrators-0.0.3/src/numba_integrators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-13 21:19:01.000000 numba-integrators-0.0.3/src/numba_integrators.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/dependencies/build.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/dependencies/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/dependencies/main.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-08-05 19:47:21.000000 numba-integrators-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/src/numba_integrators/
+-rw-r--r--   0 runner    (1001) docker     (123)    13723 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/src/numba_integrators/_API.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/src/numba_integrators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-08-05 19:46:53.000000 numba-integrators-0.1.1/src/numba_integrators/_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:47:27.741756 numba-integrators-0.1.1/src/numba_integrators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2811 2023-08-05 19:47:27.000000 numba-integrators-0.1.1/src/numba_integrators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-05 19:47:27.000000 numba-integrators-0.1.1/src/numba_integrators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:47:27.000000 numba-integrators-0.1.1/src/numba_integrators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-08-05 19:47:27.000000 numba-integrators-0.1.1/src/numba_integrators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 19:47:27.000000 numba-integrators-0.1.1/src/numba_integrators.egg-info/top_level.txt
```

### Comparing `numba-integrators-0.0.3/LICENSE` & `numba-integrators-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `numba-integrators-0.0.3/PKG-INFO` & `numba-integrators-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: numba-integrators
-Version: 0.0.3
+Version: 0.1.1
 Summary: Numerical integrators using Numba
 Author: Limespy
 Project-URL: Homepage, https://github.com/Limespy/numba-integrators
 Project-URL: Changelog, https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog
 Project-URL: Issue Tracker, https://github.com/Limespy/numba-integrators/issues
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -32,14 +32,15 @@
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Quick start guide](#quick-start-guide)
     - [The first steps](#the-first-steps)
         - [Installing](#installing)
         - [Importing](#importing)
+        - [Example](#example)
 
 # Quick start guide
 
 Here's how you can start numerically
 
 ## The first steps
 
@@ -55,16 +56,49 @@
 
 Import name is the same as install name, `numba_integrators`.
 
 ```python
 import numba_integrators
 ```
 
+### Example
+
+```python
+import numba as nb
+import numba_integrators as ni
+import numpy as np
+
+@nb.njit(nb.float64[:](nb.float64, nb.float64[:]))
+def f(t, y):
+    '''Differential equation for sine wave'''
+    return np.array((y[1], -y[0]))
+
+y0 = np.array((0., 1.))
+
+solver = ni.RK45(f, 0.0, y0,
+                 t_bound = 1, atol = 1e-8, rtol = 1e-8)
+
+t = []
+y = []
+
+while ni.step(solver):
+    t.append(solver.t)
+    y.append(solver.y)
+
+print(t)
+print(y)
+
+```
+
 # Changelog <!-- omit in toc -->
 
+## 0.1.1 2023-08-05 <!-- omit in toc -->
+
+- Initial working version
+
 ## 0.0.3 2023-05-14 <!-- omit in toc -->
 
-- Setup
+- Inital working state
 
 [1]: <https://pypi.org/project/numba_integrators> "Project PyPI page"
 [2]: <https://scipy.org/> "SciPy organisation homepage"
 [3]: <https://numba.pydata.org> "Numba organisation homepage"
```

### Comparing `numba-integrators-0.0.3/README.md` & `numba-integrators-0.1.1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Quick start guide](#quick-start-guide)
     - [The first steps](#the-first-steps)
         - [Installing](#installing)
         - [Importing](#importing)
+        - [Example](#example)
 
 # Quick start guide
 
 Here's how you can start numerically
 
 ## The first steps
 
@@ -32,16 +33,49 @@
 
 Import name is the same as install name, `numba_integrators`.
 
 ```python
 import numba_integrators
 ```
 
+### Example
+
+```python
+import numba as nb
+import numba_integrators as ni
+import numpy as np
+
+@nb.njit(nb.float64[:](nb.float64, nb.float64[:]))
+def f(t, y):
+    '''Differential equation for sine wave'''
+    return np.array((y[1], -y[0]))
+
+y0 = np.array((0., 1.))
+
+solver = ni.RK45(f, 0.0, y0,
+                 t_bound = 1, atol = 1e-8, rtol = 1e-8)
+
+t = []
+y = []
+
+while ni.step(solver):
+    t.append(solver.t)
+    y.append(solver.y)
+
+print(t)
+print(y)
+
+```
+
 # Changelog <!-- omit in toc -->
 
+## 0.1.1 2023-08-05 <!-- omit in toc -->
+
+- Initial working version
+
 ## 0.0.3 2023-05-14 <!-- omit in toc -->
 
-- Setup
+- Inital working state
 
 [1]: <https://pypi.org/project/numba_integrators> "Project PyPI page"
 [2]: <https://scipy.org/> "SciPy organisation homepage"
 [3]: <https://numba.pydata.org> "Numba organisation homepage"
```

### Comparing `numba-integrators-0.0.3/src/numba_integrators.egg-info/PKG-INFO` & `numba-integrators-0.1.1/src/numba_integrators.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: numba-integrators
-Version: 0.0.3
+Version: 0.1.1
 Summary: Numerical integrators using Numba
 Author: Limespy
 Project-URL: Homepage, https://github.com/Limespy/numba-integrators
 Project-URL: Changelog, https://github.com/Limespy/numba-integrators/blob/main/README.md#Changelog
 Project-URL: Issue Tracker, https://github.com/Limespy/numba-integrators/issues
-Classifier: Development Status :: 1 - Planning
+Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Unix
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.10
@@ -32,14 +32,15 @@
 
 ## Table of Contents <!-- omit in toc -->
 
 - [Quick start guide](#quick-start-guide)
     - [The first steps](#the-first-steps)
         - [Installing](#installing)
         - [Importing](#importing)
+        - [Example](#example)
 
 # Quick start guide
 
 Here's how you can start numerically
 
 ## The first steps
 
@@ -55,16 +56,49 @@
 
 Import name is the same as install name, `numba_integrators`.
 
 ```python
 import numba_integrators
 ```
 
+### Example
+
+```python
+import numba as nb
+import numba_integrators as ni
+import numpy as np
+
+@nb.njit(nb.float64[:](nb.float64, nb.float64[:]))
+def f(t, y):
+    '''Differential equation for sine wave'''
+    return np.array((y[1], -y[0]))
+
+y0 = np.array((0., 1.))
+
+solver = ni.RK45(f, 0.0, y0,
+                 t_bound = 1, atol = 1e-8, rtol = 1e-8)
+
+t = []
+y = []
+
+while ni.step(solver):
+    t.append(solver.t)
+    y.append(solver.y)
+
+print(t)
+print(y)
+
+```
+
 # Changelog <!-- omit in toc -->
 
+## 0.1.1 2023-08-05 <!-- omit in toc -->
+
+- Initial working version
+
 ## 0.0.3 2023-05-14 <!-- omit in toc -->
 
-- Setup
+- Inital working state
 
 [1]: <https://pypi.org/project/numba_integrators> "Project PyPI page"
 [2]: <https://scipy.org/> "SciPy organisation homepage"
 [3]: <https://numba.pydata.org> "Numba organisation homepage"
```

