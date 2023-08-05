# Comparing `tmp/pyenphase-0.3.0.tar.gz` & `tmp/pyenphase-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.3.0.tar", max compression
+gzip compressed data, was "pyenphase-0.4.0.tar", max compression
```

## Comparing `pyenphase-0.3.0.tar` & `pyenphase-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,20 @@
--rw-r--r--   0        0        0     1067 2023-07-26 17:06:24.293280 pyenphase-0.3.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-07-26 17:06:24.293280 pyenphase-0.3.0/README.md
--rw-r--r--   0        0        0     2313 2023-07-26 17:06:25.277304 pyenphase-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-07-26 17:06:25.249303 pyenphase-0.3.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     6023 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      612 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/const.py
--rw-r--r--   0        0        0     5280 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0      896 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1765 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-07-26 17:06:24.297280 pyenphase-0.3.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-05 00:55:19.059681 pyenphase-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-05 00:55:19.059681 pyenphase-0.4.0/README.md
+-rw-r--r--   0        0        0     2313 2023-08-05 00:55:20.031686 pyenphase-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-05 00:55:19.999686 pyenphase-0.4.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     6023 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      690 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0     7865 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1175 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1765 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     4170 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     2941 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0      717 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      593 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      647 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.4.0/PKG-INFO
```

### Comparing `pyenphase-0.3.0/LICENSE` & `pyenphase-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.3.0/README.md` & `pyenphase-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.3.0/pyproject.toml` & `pyenphase-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.3.0"
+version = "0.4.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.3.0/src/pyenphase/auth.py` & `pyenphase-0.4.0/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.3.0/src/pyenphase/const.py` & `pyenphase-0.4.0/src/pyenphase/const.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # System Production
-URL_INVERTER_PRODUCTION = "/api/v1/production/inverters"
-URL_PRODUCTION = "/production.json"
+URL_PRODUCTION_INVERTERS = "/api/v1/production/inverters"
+URL_PRODUCTION_V1 = "/api/v1/production"
+URL_PRODUCTION_JSON = "/production.json"
+URL_PRODUCTION = "/production"
 
 # Battery and Enpower Status
 URL_DRY_CONTACT_STATUS = "/ivp/ensemble/dry_contacts"
 URL_DRY_CONTACT_SETTINGS = "/ivp/ensemble/dry_contact_settings"
 URL_ENSEMBLE_INVENTORY = "/ivp/ensemble/inventory"
 URL_ENCHARGE_BATTERY = "/ivp/ensemble/power"
 URL_GRID_RELAY = "/ivp/ensemble/relay"
```

### Comparing `pyenphase-0.3.0/src/pyenphase/exceptions.py` & `pyenphase-0.4.0/src/pyenphase/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
-class EnvoyFirmwareCheckError(Exception):
+class EnvoyError(Exception):
+    """Base class for Envoy exceptions."""
+
+
+class EnvoyFirmwareCheckError(EnvoyError):
     """Exception raised when unable to query the Envoy firmware version."""
 
     def __init__(self, status_code: int, status: str) -> None:
         self.status_code = status_code
         self.status = status
 
 
-class EnvoyFirmwareFatalCheckError(Exception):
+class EnvoyFirmwareFatalCheckError(EnvoyError):
     """Exception raised when we should not retry the Envoy firmware version."""
 
     def __init__(self, status_code: int, status: str) -> None:
         self.status_code = status_code
         self.status = status
 
 
-class EnvoyAuthenticationError(Exception):
+class EnvoyAuthenticationError(EnvoyError):
     """Exception raised when unable to query the Envoy firmware version."""
 
     def __init__(self, status: str) -> None:
         self.status = status
 
 
-class EnvoyAuthenticationRequired(Exception):
+class EnvoyAuthenticationRequired(EnvoyError):
     """Exception raised when authentication hasn't been setup."""
 
     def __init__(self, status: str) -> None:
         self.status = status
+
+
+class EnvoyProbeFailed(EnvoyError):
+    """Exception raised when the Envoy probe fails."""
+
+
+class EnvoyCommunicationError(EnvoyError):
+    """Exception raised when the Envoy communication fails."""
```

### Comparing `pyenphase-0.3.0/src/pyenphase/firmware.py` & `pyenphase-0.4.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.3.0/src/pyenphase/ssl.py` & `pyenphase-0.4.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.3.0/PKG-INFO` & `pyenphase-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.3.0
+Version: 0.4.0
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
-Metadata-Version: 2.1 Name: pyenphase Version: 0.3.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.4.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

