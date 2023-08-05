# Comparing `tmp/pyenphase-0.5.0.tar.gz` & `tmp/pyenphase-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.5.0.tar", max compression
+gzip compressed data, was "pyenphase-0.6.0.tar", max compression
```

## Comparing `pyenphase-0.5.0.tar` & `pyenphase-0.6.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-08-05 01:41:55.751094 pyenphase-0.5.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-05 01:41:55.751094 pyenphase-0.5.0/README.md
--rw-r--r--   0        0        0     2313 2023-08-05 01:41:56.575093 pyenphase-0.5.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-08-05 01:41:56.547093 pyenphase-0.5.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     6023 2023-08-05 01:41:55.751094 pyenphase-0.5.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      690 2023-08-05 01:41:55.751094 pyenphase-0.5.0/src/pyenphase/const.py
--rw-r--r--   0        0        0    10211 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1175 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1765 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     4170 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     2941 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0      833 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      825 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1388 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-05 17:45:17.385768 pyenphase-0.6.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-05 17:45:17.385768 pyenphase-0.6.0/README.md
+-rw-r--r--   0        0        0     2313 2023-08-05 17:45:18.349774 pyenphase-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      526 2023-08-05 17:45:18.313774 pyenphase-0.6.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     6023 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      690 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0    10211 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1175 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1765 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     4170 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     2941 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0      833 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      825 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1388 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.6.0/PKG-INFO
```

### Comparing `pyenphase-0.5.0/LICENSE` & `pyenphase-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/README.md` & `pyenphase-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/pyproject.toml` & `pyenphase-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.5.0"
+version = "0.6.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.5.0/src/pyenphase/auth.py` & `pyenphase-0.6.0/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/const.py` & `pyenphase-0.6.0/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/envoy.py` & `pyenphase-0.6.0/src/pyenphase/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/exceptions.py` & `pyenphase-0.6.0/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/firmware.py` & `pyenphase-0.6.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/dry_contacts.py` & `pyenphase-0.6.0/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/encharge.py` & `pyenphase-0.6.0/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/enpower.py` & `pyenphase-0.6.0/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/envoy.py` & `pyenphase-0.6.0/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/inverter.py` & `pyenphase-0.6.0/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/system_consumption.py` & `pyenphase-0.6.0/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/models/system_production.py` & `pyenphase-0.6.0/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/src/pyenphase/ssl.py` & `pyenphase-0.6.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.5.0/PKG-INFO` & `pyenphase-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.5.0
+Version: 0.6.0
 Summary: Library to control enphase envoy
 Home-page: https://github.com/pyenphase/pyenphase
 License: MIT
 Author: pyenphase
 Author-email: cgarwood@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyenphase Version: 0.5.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.6.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

