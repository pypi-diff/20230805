# Comparing `tmp/pyenphase-0.4.0.tar.gz` & `tmp/pyenphase-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyenphase-0.4.0.tar", max compression
+gzip compressed data, was "pyenphase-0.5.0.tar", max compression
```

## Comparing `pyenphase-0.4.0.tar` & `pyenphase-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     1067 2023-08-05 00:55:19.059681 pyenphase-0.4.0/LICENSE
--rw-r--r--   0        0        0     3476 2023-08-05 00:55:19.059681 pyenphase-0.4.0/README.md
--rw-r--r--   0        0        0     2313 2023-08-05 00:55:20.031686 pyenphase-0.4.0/pyproject.toml
--rw-r--r--   0        0        0       44 2023-08-05 00:55:19.999686 pyenphase-0.4.0/src/pyenphase/__init__.py
--rw-r--r--   0        0        0     6023 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/auth.py
--rw-r--r--   0        0        0      690 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/const.py
--rw-r--r--   0        0        0     7865 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/envoy.py
--rw-r--r--   0        0        0     1175 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/exceptions.py
--rw-r--r--   0        0        0     1765 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/firmware.py
--rw-r--r--   0        0        0       53 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/main.py
--rw-r--r--   0        0        0        0 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/__init__.py
--rw-r--r--   0        0        0     2852 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/dry_contacts.py
--rw-r--r--   0        0        0     4170 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/encharge.py
--rw-r--r--   0        0        0     2941 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/enpower.py
--rw-r--r--   0        0        0      717 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/envoy.py
--rw-r--r--   0        0        0      593 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/inverter.py
--rw-r--r--   0        0        0      647 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/models/system_production.py
--rw-r--r--   0        0        0        0 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/py.typed
--rw-r--r--   0        0        0      915 2023-08-05 00:55:19.063681 pyenphase-0.4.0/src/pyenphase/ssl.py
--rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-08-05 01:41:55.751094 pyenphase-0.5.0/LICENSE
+-rw-r--r--   0        0        0     3476 2023-08-05 01:41:55.751094 pyenphase-0.5.0/README.md
+-rw-r--r--   0        0        0     2313 2023-08-05 01:41:56.575093 pyenphase-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0       44 2023-08-05 01:41:56.547093 pyenphase-0.5.0/src/pyenphase/__init__.py
+-rw-r--r--   0        0        0     6023 2023-08-05 01:41:55.751094 pyenphase-0.5.0/src/pyenphase/auth.py
+-rw-r--r--   0        0        0      690 2023-08-05 01:41:55.751094 pyenphase-0.5.0/src/pyenphase/const.py
+-rw-r--r--   0        0        0    10211 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/envoy.py
+-rw-r--r--   0        0        0     1175 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/exceptions.py
+-rw-r--r--   0        0        0     1765 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/firmware.py
+-rw-r--r--   0        0        0       53 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/main.py
+-rw-r--r--   0        0        0        0 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/__init__.py
+-rw-r--r--   0        0        0     2852 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/dry_contacts.py
+-rw-r--r--   0        0        0     4170 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/encharge.py
+-rw-r--r--   0        0        0     2941 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/enpower.py
+-rw-r--r--   0        0        0      833 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/envoy.py
+-rw-r--r--   0        0        0      694 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/inverter.py
+-rw-r--r--   0        0        0      825 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/system_consumption.py
+-rw-r--r--   0        0        0     1388 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/models/system_production.py
+-rw-r--r--   0        0        0        0 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/py.typed
+-rw-r--r--   0        0        0      915 2023-08-05 01:41:55.755094 pyenphase-0.5.0/src/pyenphase/ssl.py
+-rw-r--r--   0        0        0     4718 1970-01-01 00:00:00.000000 pyenphase-0.5.0/PKG-INFO
```

### Comparing `pyenphase-0.4.0/LICENSE` & `pyenphase-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/README.md` & `pyenphase-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/pyproject.toml` & `pyenphase-0.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyenphase"
-version = "0.4.0"
+version = "0.5.0"
 description = "Library to control enphase envoy"
 authors = ["pyenphase <cgarwood@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pyenphase/pyenphase"
 documentation = "https://pyenphase.readthedocs.io"
 classifiers = [
```

### Comparing `pyenphase-0.4.0/src/pyenphase/auth.py` & `pyenphase-0.5.0/src/pyenphase/auth.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/const.py` & `pyenphase-0.5.0/src/pyenphase/const.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/envoy.py` & `pyenphase-0.5.0/src/pyenphase/envoy.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,19 +18,20 @@
     URL_PRODUCTION_JSON,
     URL_PRODUCTION_V1,
 )
 from .exceptions import EnvoyAuthenticationRequired, EnvoyProbeFailed
 from .firmware import EnvoyFirmware, EnvoyFirmwareCheckError
 from .models.envoy import EnvoyData
 from .models.inverter import EnvoyInverter
+from .models.system_consumption import EnvoySystemConsumption
 from .models.system_production import EnvoySystemProduction
 
 _LOGGER = logging.getLogger(__name__)
 
-TIMEOUT = 15
+TIMEOUT = 20
 LEGACY_ENVOY_VERSION = AwesomeVersion("3.9.0")
 AUTH_TOKEN_MIN_VERSION = AwesomeVersion("7.0.0")
 DEFAULT_HEADERS = {
     "Accept": "application/json",
 }
 
 
@@ -54,17 +55,20 @@
 
 
 _NO_VERIFY_SSL_CONTEXT = create_no_verify_ssl_context()
 
 
 class SupportedFeatures(enum.IntFlag):
     INVERTERS = 1
-    DRY_CONTACTS = 2
-    ENCHARGE = 4
-    ENPOWER = 8
+    METERING = 2
+    TOTAL_CONSUMPTION = 4
+    NET_CONSUMPTION = 8
+    DRY_CONTACTS = 16
+    ENCHARGE = 32
+    ENPOWER = 64
 
 
 class Envoy:
     """Class for communicating with an envoy."""
 
     def __init__(self, host: str) -> None:
         """Initialize the Envoy class."""
@@ -128,16 +132,18 @@
                 "You must include username/password or token to authenticate to the Envoy."
             )
             raise EnvoyAuthenticationRequired("Could not setup authentication object.")
 
         await self.auth.setup(self._client)
 
     @retry(
-        retry=retry_if_exception_type((httpx.ReadError, httpx.RemoteProtocolError)),
-        wait=wait_random_exponential(multiplier=2, max=2),
+        retry=retry_if_exception_type(
+            (httpx.NetworkError, httpx.TimeoutException, httpx.RemoteProtocolError)
+        ),
+        wait=wait_random_exponential(multiplier=2, max=3),
     )
     async def request(self, endpoint: str) -> Any:
         """Make a request to the Envoy."""
         if self.auth is None:
             raise EnvoyAuthenticationRequired(
                 "You must authenticate to the Envoy before making requests."
             )
@@ -164,26 +170,50 @@
     @property
     def serial_number(self) -> str | None:
         """Return the Envoy serial number."""
         return self._firmware.serial
 
     async def probe(self) -> None:
         """Probe for model and supported features."""
-        for endpoint in (
-            URL_PRODUCTION_V1,
-            URL_PRODUCTION_JSON,
-            URL_PRODUCTION,
-        ):
-            try:
-                await self.request(endpoint)
-            except (json.JSONDecodeError, httpx.HTTPError) as e:
-                _LOGGER.debug("Production endpoint not found at %s: %s", endpoint, e)
-                continue
-            self._production_endpoint = endpoint
-            break
+        try:
+            production_json: dict[str, Any] = await self.request(URL_PRODUCTION)
+        except (json.JSONDecodeError, httpx.HTTPError) as e:
+            _LOGGER.debug("Production endpoint not found at %s: %s", URL_PRODUCTION, e)
+        else:
+            production: list[dict[str, str | float | int]] | None = production_json.get(
+                "production"
+            )
+            if production:
+                for type_ in production:
+                    if type_["type"] == "eim" and type_["activeCount"]:
+                        self._supported_features |= SupportedFeatures.METERING
+                        break
+            consumption: list[
+                dict[str, str | float | int]
+            ] | None = production_json.get("consumption")
+            if consumption:
+                for meter in consumption:
+                    meter_type = meter["measurementType"]
+                    if meter_type == "total-consumption" and meter["activeCount"]:
+                        self._supported_features |= SupportedFeatures.TOTAL_CONSUMPTION
+                    elif meter_type == "net-consumption" and meter["activeCount"]:
+                        self._supported_features |= SupportedFeatures.NET_CONSUMPTION
+            self._production_endpoint = URL_PRODUCTION
+
+        if not self._production_endpoint:
+            for endpoint in (URL_PRODUCTION_V1, URL_PRODUCTION_JSON):
+                try:
+                    await self.request(endpoint)
+                except (json.JSONDecodeError, httpx.HTTPError) as e:
+                    _LOGGER.debug(
+                        "Production endpoint not found at %s: %s", endpoint, e
+                    )
+                    continue
+                self._production_endpoint = endpoint
+                break
 
         try:
             await self.request(URL_PRODUCTION_INVERTERS)
         except (json.JSONDecodeError, httpx.HTTPError) as e:
             _LOGGER.debug("Inverters endpoint not found: %s", e)
         else:
             self._supported_features |= SupportedFeatures.INVERTERS
@@ -192,31 +222,46 @@
         """Update data."""
         if not self._production_endpoint:
             await self.probe()
 
         if not self._production_endpoint:
             raise EnvoyProbeFailed("Unable to determine production endpoint")
 
-        production_data = await self.request(self._production_endpoint)
+        production_endpoint = self._production_endpoint
+        supported_features = self._supported_features
+        system_consumption: EnvoySystemConsumption | None = None
+        production_data = await self.request(production_endpoint)
         inverters: dict[str, EnvoyInverter] = {}
-        raw = {
-            "production": production_data,
-        }
+        raw = {"production": production_data}
+
+        if production_endpoint == URL_PRODUCTION:
+            if (
+                supported_features & SupportedFeatures.TOTAL_CONSUMPTION
+                or supported_features & SupportedFeatures.NET_CONSUMPTION
+            ):
+                system_consumption = EnvoySystemConsumption.from_production(
+                    production_data
+                )
+            system_production = EnvoySystemProduction.from_production(production_data)
+        else:
+            # Production endpoint is either URL_PRODUCTION_V1 or URL_PRODUCTION_JSON
+            system_production = EnvoySystemProduction.from_v1_api(production_data)
 
-        if self._supported_features & SupportedFeatures.INVERTERS:
+        if supported_features & SupportedFeatures.INVERTERS:
             inverters_data: list[dict[str, Any]] = await self.request(
                 URL_PRODUCTION_INVERTERS
             )
             inverters = {
-                inverter["serialNumber"]: EnvoyInverter(inverter)
+                inverter["serialNumber"]: EnvoyInverter.from_v1_api(inverter)
                 for inverter in inverters_data
             }
             raw["inverters"] = inverters_data
 
         return EnvoyData(
-            system_production=EnvoySystemProduction(production_data),
+            system_production=system_production,
+            system_consumption=system_consumption,
             inverters=inverters,
             # Raw data is exposed so we can __eq__ the data to see if
             # anything has changed and consumers of the library can
             # avoid dispatching data if nothing has changed.
             raw=raw,
         )
```

### Comparing `pyenphase-0.4.0/src/pyenphase/exceptions.py` & `pyenphase-0.5.0/src/pyenphase/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/firmware.py` & `pyenphase-0.5.0/src/pyenphase/firmware.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/models/dry_contacts.py` & `pyenphase-0.5.0/src/pyenphase/models/dry_contacts.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/models/encharge.py` & `pyenphase-0.5.0/src/pyenphase/models/encharge.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/models/enpower.py` & `pyenphase-0.5.0/src/pyenphase/models/enpower.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/src/pyenphase/models/envoy.py` & `pyenphase-0.5.0/src/pyenphase/models/envoy.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from dataclasses import dataclass, field
 from typing import Any
 
 from .dry_contacts import EnvoyDryContact
 from .encharge import EnvoyEncharge
 from .enpower import EnvoyEnpower
 from .inverter import EnvoyInverter
+from .system_consumption import EnvoySystemConsumption
 from .system_production import EnvoySystemProduction
 
 
 @dataclass(slots=True)
 class EnvoyData:
     """Model for an envoy."""
 
     encharge: EnvoyEncharge | None = None
     enpower: EnvoyEnpower | None = None
+    system_consumption: EnvoySystemConsumption | None = None
     system_production: EnvoySystemProduction | None = None
     dry_contacts: dict[str, EnvoyDryContact] = field(default_factory=dict)
     inverters: dict[str, EnvoyInverter] = field(default_factory=dict)
     raw: dict[str, dict[str, Any]] = field(default_factory=dict)
```

### Comparing `pyenphase-0.4.0/src/pyenphase/ssl.py` & `pyenphase-0.5.0/src/pyenphase/ssl.py`

 * *Files identical despite different names*

### Comparing `pyenphase-0.4.0/PKG-INFO` & `pyenphase-0.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyenphase
-Version: 0.4.0
+Version: 0.5.0
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
-Metadata-Version: 2.1 Name: pyenphase Version: 0.4.0 Summary: Library to
+Metadata-Version: 2.1 Name: pyenphase Version: 0.5.0 Summary: Library to
 control enphase envoy Home-page: https://github.com/pyenphase/pyenphase
 License: MIT Author: pyenphase Author-email: cgarwood@gmail.com Requires-
 Python: >=3.10,<4.0 Classifier: Development Status :: 2 - Pre-Alpha Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

