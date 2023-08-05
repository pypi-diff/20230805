# Comparing `tmp/mypyllant-0.4.3.tar.gz` & `tmp/mypyllant-0.4.4.tar.gz`

## Comparing `mypyllant-0.4.3.tar` & `mypyllant-0.4.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.dockerignore
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.3/Dockerfile
--rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.3/logo.png
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.3/requirements-dev.txt
--rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.3/run_pytest.sh
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.github/workflows/build-test.yaml
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.github/workflows/docker.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/__init__.py
--rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/api.py
--rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/const.py
--rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/export.py
--rw-r--r--   0        0        0     8965 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/py.typed
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/sample.py
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/__init__.py
--rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/conftest.py
--rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/find_countries.py
--rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/generate_test_data.py
--rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_api.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_countries.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_export.py
--rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_generate_test_data.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/test_sample.py
--rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/update_sample.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/utils.py
--rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
--rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
--rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
--rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
--rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.3/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.3/LICENSE
--rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 mypyllant-0.4.3/README.md
--rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.3/pyproject.toml
--rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 mypyllant-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.dockerignore
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 mypyllant-0.4.4/Dockerfile
+-rw-r--r--   0        0        0    45426 2020-02-02 00:00:00.000000 mypyllant-0.4.4/logo.png
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 mypyllant-0.4.4/requirements-dev.txt
+-rwxr-xr-x   0        0        0      195 2020-02-02 00:00:00.000000 mypyllant-0.4.4/run_pytest.sh
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.github/workflows/build-test.yaml
+-rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.github/workflows/docker.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/__init__.py
+-rw-r--r--   0        0        0    19536 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/api.py
+-rw-r--r--   0        0        0     2194 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/const.py
+-rwxr-xr-x   0        0        0     2379 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/export.py
+-rw-r--r--   0        0        0     8969 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/py.typed
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/sample.py
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/__init__.py
+-rw-r--r--   0        0        0      299 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/conftest.py
+-rwxr-xr-x   0        0        0     1035 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/find_countries.py
+-rw-r--r--   0        0        0     6579 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/generate_test_data.py
+-rw-r--r--   0        0        0     8668 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_api.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_countries.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_export.py
+-rw-r--r--   0        0        0     4861 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_generate_test_data.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/test_sample.py
+-rwxr-xr-x   0        0        0      655 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/update_sample.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/utils.py
+-rw-r--r--   0        0        0      364 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/control_identifier.json
+-rw-r--r--   0        0        0     2803 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/firmware_update_required.json
+-rw-r--r--   0        0        0     5540 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/time_zone.json
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/claims.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/connection_status.json
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/control_identifier.json
+-rw-r--r--   0        0        0     2818 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json
+-rw-r--r--   0        0        0     3072 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/firmware_update_required.json
+-rw-r--r--   0        0        0     5539 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/time_zone.json
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 mypyllant-0.4.4/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 mypyllant-0.4.4/LICENSE
+-rw-r--r--   0        0        0     6788 2020-02-02 00:00:00.000000 mypyllant-0.4.4/README.md
+-rw-r--r--   0        0        0     1542 2020-02-02 00:00:00.000000 mypyllant-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0     7394 2020-02-02 00:00:00.000000 mypyllant-0.4.4/PKG-INFO
```

### Comparing `mypyllant-0.4.3/.dockerignore` & `mypyllant-0.4.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/.pre-commit-config.yaml` & `mypyllant-0.4.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/logo.png` & `mypyllant-0.4.4/logo.png`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/.github/workflows/build-test.yaml` & `mypyllant-0.4.4/.github/workflows/build-test.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/.github/workflows/docker.yaml` & `mypyllant-0.4.4/.github/workflows/docker.yaml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/api.py` & `mypyllant-0.4.4/src/myPyllant/api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/const.py` & `mypyllant-0.4.4/src/myPyllant/const.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/export.py` & `mypyllant-0.4.4/src/myPyllant/export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/models.py` & `mypyllant-0.4.4/src/myPyllant/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,16 +237,16 @@
             logger.info("Could not get water pressure from system control state")
             return None
 
 
 class Device(BaseModel):
     system_id: str
     device_uuid: str
-    name: str = ""
-    product_name: str = ""
+    name: str | None
+    product_name: str | None
     diagnostic_trouble_codes: list = []
     properties: list = []
     ebus_id: str
     article_number: str
     device_serial_number: str
     type: str
     device_type: str
```

### Comparing `mypyllant-0.4.3/src/myPyllant/sample.py` & `mypyllant-0.4.4/src/myPyllant/sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/utils.py` & `mypyllant-0.4.4/src/myPyllant/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/find_countries.py` & `mypyllant-0.4.4/src/myPyllant/tests/find_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/generate_test_data.py` & `mypyllant-0.4.4/src/myPyllant/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/test_api.py` & `mypyllant-0.4.4/src/myPyllant/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/test_countries.py` & `mypyllant-0.4.4/src/myPyllant/tests/test_countries.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/test_export.py` & `mypyllant-0.4.4/src/myPyllant/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/test_generate_test_data.py` & `mypyllant-0.4.4/src/myPyllant/tests/test_generate_test_data.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/update_sample.py` & `mypyllant-0.4.4/src/myPyllant/tests/update_sample.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/utils.py` & `mypyllant-0.4.4/src/myPyllant/tests/utils.py`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json` & `mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/current_system.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9970238095238095%*

 * *Differences: {"'electric_backup_heater'": "{'product_name': None}"}*

```diff
@@ -21,15 +21,15 @@
         "device_serial_number": "4473c7336471b813876c29dd70bed74deb897e14",
         "device_type": "ELECTRIC_AUXILIARY_HEATER",
         "device_uuid": "b5b8533bd405f662cab27a89c0de1ea3507e1bb8",
         "ebus_id": "VWZ02",
         "emfValid": true,
         "first_data": "2022-10-11T16:16:40Z",
         "last_data": "2023-08-01T22:42:15Z",
-        "product_name": "hydraulic station",
+        "product_name": null,
         "spn": 351
     },
     "has_emf_capable_devices": true,
     "primary_heat_generator": {
         "article_number": "0010021118",
         "bus_coupler_address": 0,
         "data": [
```

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json` & `mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json` & `mypyllant-0.4.4/src/myPyllant/tests/json/56f4c513b87875849a089b83cafbe6fdd6020b55/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json` & `mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/current_system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json` & `mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/device_buckets.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json` & `mypyllant-0.4.4/src/myPyllant/tests/json/cf6a60bfab7c00bc4bd13cc80618315d9cec2129/system.json`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/.gitignore` & `mypyllant-0.4.4/.gitignore`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/LICENSE` & `mypyllant-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/README.md` & `mypyllant-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/pyproject.toml` & `mypyllant-0.4.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `mypyllant-0.4.3/PKG-INFO` & `mypyllant-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: myPyllant
-Version: 0.4.3
+Version: 0.4.4
 Summary: A Python library to interact with the API behind the myVAILLANT app
 Project-URL: Homepage, https://github.com/signalkraft/myPyllant
 Project-URL: Bug Tracker, https://github.com/signalkraft/myPyllant/issues
 Author-email: Philipp <pd@signalkraft.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

