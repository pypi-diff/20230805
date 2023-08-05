# Comparing `tmp/pyenphase-0.6.0.tar.gz` & `tmp/pyenphase-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.6.0.tar", max compression
+gzip compressed data, was "pyenphase-0.6.1.tar", max compression
```

## Comparing `pyenphase-0.6.0.tar` & `pyenphase-0.6.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-08-05 17:45:17.385768 pyenphase-0.6.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-05 17:45:17.385768 pyenphase-0.6.0/README.md
--rw-r--r--   0        0        0     2313 2023-08-05 17:45:18.349774 pyenphase-0.6.0/pyproject.toml
--rw-r--r--   0        0        0      526 2023-08-05 17:45:18.313774 pyenphase-0.6.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     6023 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      690 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/const.py
--rw-r--r--   0        0        0    10211 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1175 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1765 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     4170 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     2941 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0      833 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      694 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      825 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/system_consumption.py
--rw-r--r--   0        0        0     1388 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-08-05 17:45:17.389768 pyenphase-0.6.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-05 18:26:26.194192 pyenphase-0.6.1/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-05 18:26:26.194192 pyenphase-0.6.1/README.md
+-rw-r--r--   0        0        0     2313 2023-08-05 18:26:27.202276 pyenphase-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0      526 2023-08-05 18:26:27.166273 pyenphase-0.6.1/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     7305 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      690 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/const.py
+-rw-r--r--   0        0        0    10480 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1175 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1765 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     4170 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     2941 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0      833 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      825 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1388 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-08-05 18:26:26.194192 pyenphase-0.6.1/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.6.1/PKG-INFO
```

### Comparing `pyenphase-0.6.0/LICENSE` & `pyenphase-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/README.md` & `pyenphase-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/pyproject.toml` & `pyenphase-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.6.0"
+version = "0.6.1"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.6.0/src/pyenphase/__init__.py` & `pyenphase-0.6.1/src/pyenphase/__init__.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/auth.py` & `pyenphase-0.6.1/src/pyenphase/auth.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 """Envoy authentication methods."""
 
-import json
+import ssl
 from abc import abstractmethod, abstractproperty
+from typing import Any
 
 import httpx
+import orjson
+from tenacity import retry, retry_if_exception_type, wait_random_exponential
 
 from .exceptions import EnvoyAuthenticationError
 
 
+def create_default_ssl_context() -> ssl.SSLContext:
+    """Return an default SSL context."""
+    return ssl.create_default_context()
+
+
+_SSL_CONTEXT = create_default_ssl_context()
+
+
 class EnvoyAuth:
     """Base class for Envoy authentication."""
 
     def __init__(self, host: str) -> None:
         """Initialize the EnvoyAuth class."""
         pass
 
@@ -61,51 +72,18 @@
                     "Your firmware requires token authentication, but no cloud credentials were provided to obtain the token."
                 )
             # Raise if we are missing the envoy serial number
             if not self.envoy_serial:
                 raise EnvoyAuthenticationError(
                     "Your firmware requires token authentication, but no envoy serial number was provided to obtain the token."
                 )
-
-            # we require a new client that checks SSL certs
-            self.cloud_client = httpx.AsyncClient()
-
-            # Login to Enlighten to obtain a session ID
-            data = {
-                "user[email]": self.cloud_username,
-                "user[password]": self.cloud_password,
-            }
-            req = await self.cloud_client.post(
-                "https://enlighten.enphaseenergy.com/login/login.json?", data=data
-            )
-            if req.status_code != 200:
-                raise EnvoyAuthenticationError(
-                    "Unable to login to Enlighten to obtain session ID."
-                )
-            response = json.loads(req.text)
-            self._is_consumer = response["is_consumer"]
-            self._manager_token = response["manager_token"]
-
-            # Obtain the token
-            data = {
-                "session_id": response["session_id"],
-                "serial_num": self.envoy_serial,
-                "username": self.cloud_username,
-            }
-            req = await self.cloud_client.post(
-                "https://entrez.enphaseenergy.com/tokens", json=data
-            )
-            if req.status_code != 200:
-                raise EnvoyAuthenticationError(
-                    "Unable to obtain token for Envoy authentication."
-                )
-            self._token = req.text
+            self._token = await self._obtain_token()
 
         # Verify we have adequate credentials
-        if not self.token:
+        if not self._token:
             raise EnvoyAuthenticationError(
                 "Unable to obtain token for Envoy authentication."
             )
 
         # Verify the token and obtain cookie with session ID necessary for some API calls
         req = await client.get(
             f"https://{self.host}/auth/check_jwt",
@@ -115,14 +93,69 @@
         if req.status_code != 200:
             raise EnvoyAuthenticationError(
                 "Unable to verify token for Envoy authentication."
             )
 
         self._cookies = req.cookies
 
+    async def _obtain_token(self) -> None:
+        """Obtain the token for Envoy authentication."""
+        # we require a new client that checks SSL certs
+        async with httpx.AsyncClient(verify=_SSL_CONTEXT, timeout=10) as cloud_client:
+            # Login to Enlighten to obtain a session ID
+            response = await self._post_json_with_cloud_client(
+                cloud_client,
+                "https://enlighten.enphaseenergy.com/login/login.json?",
+                data={
+                    "user[email]": self.cloud_username,
+                    "user[password]": self.cloud_password,
+                },
+            )
+            if response.status_code != 200:
+                raise EnvoyAuthenticationError(
+                    "Unable to login to Enlighten to obtain session ID: "
+                    f"{response.status_code}: {response.text}"
+                )
+            response = orjson.loads(response.text)
+            self._is_consumer = response["is_consumer"]
+            self._manager_token = response["manager_token"]
+
+            # Obtain the token
+            response = await self._post_json_with_cloud_client(
+                cloud_client,
+                "https://entrez.enphaseenergy.com/tokens",
+                json={
+                    "session_id": response["session_id"],
+                    "serial_num": self.envoy_serial,
+                    "username": self.cloud_username,
+                },
+            )
+            if response.status_code != 200:
+                raise EnvoyAuthenticationError(
+                    "Unable to obtain token for Envoy authentication: "
+                    f"{response.status_code}: {response.text}"
+                )
+            return response.text
+
+    @retry(
+        retry=retry_if_exception_type(
+            (httpx.NetworkError, httpx.TimeoutException, httpx.RemoteProtocolError)
+        ),
+        wait=wait_random_exponential(multiplier=2, max=3),
+    )
+    async def _post_json_with_cloud_client(
+        self,
+        client: httpx.AsyncClient,
+        url: str,
+        data: dict[str, Any] | None = None,
+        json: dict[str, Any] | None = None,
+    ) -> httpx.Response:
+        """Post to the Envoy API with the cloud client."""
+        return await client.post(url, json=json, data=data)
+
     @property
     def token(self) -> str:
         assert self._token is not None  # nosec
         return self._token
 
     @property
     def manager_token(self) -> str:
```

### Comparing `pyenphase-0.6.0/src/pyenphase/const.py` & `pyenphase-0.6.1/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/envoy.py` & `pyenphase-0.6.1/src/pyenphase/envoy.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,25 +66,32 @@
     ENCHARGE = 32
     ENPOWER = 64
 
 
 class Envoy:
     """Class for communicating with an envoy."""
 
-    def __init__(self, host: str) -> None:
+    def __init__(
+        self,
+        host: str,
+        client: httpx.AsyncClient | None = None,
+        timeout: float | None = None,
+    ) -> None:
         """Initialize the Envoy class."""
         # We use our own httpx client session so we can disable SSL verification (Envoys use self-signed SSL certs)
-        self._client = httpx.AsyncClient(
-            verify=_NO_VERIFY_SSL_CONTEXT, timeout=TIMEOUT
+        self._timeout = timeout or TIMEOUT
+        self._client = client or httpx.AsyncClient(
+            verify=_NO_VERIFY_SSL_CONTEXT
         )  # nosec
         self.auth: EnvoyAuth | None = None
         self._host = host
         self._firmware = EnvoyFirmware(self._client, self._host)
         self._supported_features: SupportedFeatures = SupportedFeatures(0)
         self._production_endpoint: str | None = None
+        self.data: EnvoyData | None = None
 
     @retry(
         retry=retry_if_exception_type(EnvoyFirmwareCheckError),
         wait=wait_random_exponential(multiplier=2, max=10),
     )
     async def setup(self) -> None:
         """Obtain the firmware version for later Envoy authentication."""
@@ -150,14 +157,15 @@
 
         response = await self._client.get(
             self.auth.get_endpoint_url(endpoint),
             headers={**DEFAULT_HEADERS, **self.auth.headers},
             cookies=self.auth.cookies,
             follow_redirects=True,
             auth=self.auth.auth,
+            timeout=self._timeout,
         )
         return orjson.loads(response.text)
 
     @property
     def host(self) -> str:
         """Return the Envoy host."""
         return self._host
@@ -252,16 +260,18 @@
             )
             inverters = {
                 inverter["serialNumber"]: EnvoyInverter.from_v1_api(inverter)
                 for inverter in inverters_data
             }
             raw["inverters"] = inverters_data
 
-        return EnvoyData(
+        data = EnvoyData(
             system_production=system_production,
             system_consumption=system_consumption,
             inverters=inverters,
             # Raw data is exposed so we can __eq__ the data to see if
             # anything has changed and consumers of the library can
             # avoid dispatching data if nothing has changed.
             raw=raw,
         )
+        self.data = data
+        return data
```

### Comparing `pyenphase-0.6.0/src/pyenphase/exceptions.py` & `pyenphase-0.6.1/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/firmware.py` & `pyenphase-0.6.1/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/dry_contacts.py` & `pyenphase-0.6.1/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/encharge.py` & `pyenphase-0.6.1/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/enpower.py` & `pyenphase-0.6.1/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/envoy.py` & `pyenphase-0.6.1/src/pyenphase/models/envoy.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/inverter.py` & `pyenphase-0.6.1/src/pyenphase/models/inverter.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/system_consumption.py` & `pyenphase-0.6.1/src/pyenphase/models/system_consumption.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/models/system_production.py` & `pyenphase-0.6.1/src/pyenphase/models/system_production.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/src/pyenphase/ssl.py` & `pyenphase-0.6.1/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.6.0/PKG-INFO` & `pyenphase-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.6.0
+Version: 0.6.1
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
-Metadata-Version: 2.1 Name: pyenphase Version: 0.6.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.6.1 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

