# Comparing `tmp/pymeten-0.0.4.tar.gz` & `tmp/pymeten-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeten-0.0.4.tar", last modified: Thu Aug  3 15:25:03 2023, max compression
+gzip compressed data, was "pymeten-0.0.5.tar", last modified: Sat Aug  5 02:00:59 2023, max compression
```

## Comparing `pymeten-0.0.4.tar` & `pymeten-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 15:25:03.595750 pymeten-0.0.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-08-03 15:25:03.595750 pymeten-0.0.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2023-08-03 15:25:03.000000 pymeten-0.0.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 15:25:03.595750 pymeten-0.0.4/pymeten/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten/itutils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6934 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten/triton_benchmark.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-03 15:25:03.595750 pymeten-0.0.4/pymeten.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-03 15:25:03.000000 pymeten-0.0.4/pymeten.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-03 15:25:03.595750 pymeten-0.0.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2023-08-03 15:25:03.000000 pymeten-0.0.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 02:00:59.622778 pymeten-0.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-08-05 02:00:59.622778 pymeten-0.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2640 2023-08-05 02:00:59.000000 pymeten-0.0.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 02:00:59.618778 pymeten-0.0.5/pymeten/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      131 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten/itutils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6983 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten/triton_benchmark.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 02:00:59.622778 pymeten-0.0.5/pymeten.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      448 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       83 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-05 02:00:59.000000 pymeten-0.0.5/pymeten.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-08-05 02:00:59.622778 pymeten-0.0.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2023-08-05 02:00:59.000000 pymeten-0.0.5/setup.py
```

### Comparing `pymeten-0.0.4/README.md` & `pymeten-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pymeten-0.0.4/pymeten/itutils.py` & `pymeten-0.0.5/pymeten/itutils.py`

 * *Files identical despite different names*

### Comparing `pymeten-0.0.4/pymeten/triton_benchmark.py` & `pymeten-0.0.5/pymeten/triton_benchmark.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
                         else math.prod(size)
             total_num_ops = self.num_ops * numel if self.num_ops is not None else 0
             total_num_bytes = self.num_bytes * numel if self.num_bytes is not None else 0
             num_ops_pms = total_num_bytes / ms
             num_bytes_pms = total_num_bytes / ms
 
         if self.unit == MetricUnit.MS:
-            return int(ms)
+            return ms
         elif self.unit == MetricUnit.GBPS:
             return num_bytes_pms * 1e-6
         elif self.unit == MetricUnit.TBPS:
             return num_bytes_pms * 1e-9
         elif self.unit == MetricUnit.GFLOPS:
             return num_ops_pms * 1e-6
         elif self.unit == MetricUnit.TFLOPS:
@@ -123,14 +123,15 @@
         }
 
         kernel_map = {
             'torch': lambda x, y: x + y,
             'triton': lambda x, y: add(x, y)
         }
     """
+    print(f'Using metric: {metric_config.unit.name}')
     providers = list(kernel_map.keys())
     assert len(providers) <= 10
     if colors is None:
         colors = list(mcolors.TABLEAU_COLORS.values())[:len(providers)]
     if line_styles is None:
         line_styles = ['-'] * len(providers)
     styles = list(zip(colors, line_styles))
```

### Comparing `pymeten-0.0.4/setup.py` & `pymeten-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'A tool for metrics of tensors'
 LONG_DESCRIPTION = 'Measure the different aspects of your tensor program efficiency'
 
 requirements = [
     'torch',
     'triton',
     'matplotlib',
```

