# Comparing `tmp/nc_py_api-0.0.26.tar.gz` & `tmp/nc_py_api-0.0.27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nc_py_api-0.0.26.tar", last modified: Sat Jul 29 13:19:53 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `nc_py_api-0.0.26.tar` & `nc_py_api-0.0.27.tar`

### file list

```diff
@@ -1,38 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/
--rw-r--r--   0 runner    (1001) docker     (122)      475 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (122)     1551 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)      246 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2596 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 13:19:53.803912 nc_py_api-0.0.26/nc_py_api/
--rw-r--r--   0 runner    (1001) docker     (122)      560 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14068 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/_session.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     2419 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/appconfig_preferences_ex.py
--rw-r--r--   0 runner    (1001) docker     (122)     3768 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/apps.py
--rw-r--r--   0 runner    (1001) docker     (122)     2648 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)    26651 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/files.py
--rw-r--r--   0 runner    (1001) docker     (122)     4972 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/files_sharing.py
--rw-r--r--   0 runner    (1001) docker     (122)     1657 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/integration_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/misc.py
--rw-r--r--   0 runner    (1001) docker     (122)     6570 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/nextcloud.py
--rw-r--r--   0 runner    (1001) docker     (122)      523 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/options.py
--rw-r--r--   0 runner    (1001) docker     (122)      974 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (122)     1824 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/theming.py
--rw-r--r--   0 runner    (1001) docker     (122)     1788 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/ui_files_actions_menu.py
--rw-r--r--   0 runner    (1001) docker     (122)     5620 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/users.py
--rw-r--r--   0 runner    (1001) docker     (122)     4264 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/users_groups.py
--rw-r--r--   0 runner    (1001) docker     (122)     7900 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/users_status.py
--rw-r--r--   0 runner    (1001) docker     (122)     4288 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/nc_py_api/weather_status.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/nc_py_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4095 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      316 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-07-29 13:19:53.000000 nc_py_api-0.0.26/nc_py_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-29 13:19:43.000000 nc_py_api-0.0.26/nc_py_api.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)     1436 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1810 2023-07-29 13:19:53.807912 nc_py_api-0.0.26/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      344 2023-07-29 13:19:29.000000 nc_py_api-0.0.26/setup.py
+-rw-r--r--   0        0        0     2029 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/CHANGELOG.md
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/__init__.py
+-rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/_deffered_error.py
+-rw-r--r--   0        0        0    14975 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/_session.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/_version.py
+-rw-r--r--   0        0        0     3253 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/appcfg_prefs_ex.py
+-rw-r--r--   0        0        0     3777 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/apps.py
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/constants.py
+-rw-r--r--   0        0        0     1366 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/exceptions.py
+-rw-r--r--   0        0        0    22060 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/files.py
+-rw-r--r--   0        0        0     7226 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/files_defs.py
+-rw-r--r--   0        0        0     4012 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/files_sharing.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/gui.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/gui_defs.py
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/gui_files.py
+-rw-r--r--   0        0        0     1655 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/integration_fastapi.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/misc.py
+-rw-r--r--   0        0        0     5842 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/nextcloud.py
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/options.py
+-rw-r--r--   0        0        0     1302 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/preferences.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/theming.py
+-rw-r--r--   0        0        0     6286 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/users.py
+-rw-r--r--   0        0        0     6329 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/users_defs.py
+-rw-r--r--   0        0        0     3422 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/users_groups.py
+-rw-r--r--   0        0        0     3942 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/users_notifications.py
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/users_status.py
+-rw-r--r--   0        0        0     3319 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/nc_py_api/users_weather.py
+-rw-r--r--   0        0        0      990 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/.gitignore
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/AUTHORS
+-rw-r--r--   0        0        0     1551 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/LICENSE.txt
+-rw-r--r--   0        0        0     2582 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/README.md
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/pyproject.toml
+-rw-r--r--   0        0        0     5250 2020-02-02 00:00:00.000000 nc_py_api-0.0.27/PKG-INFO
```

### Comparing `nc_py_api-0.0.26/LICENSE.txt` & `nc_py_api-0.0.27/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nc_py_api-0.0.26/README.md` & `nc_py_api-0.0.27/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 ### Basic Features:
  * Operations with Files and Folders
  * ~~Operations with Trash bin and File versions~~
  * Operations with Users and User Groups
  * User status
  * Weather status
- * ~~Nextcloud notifications support~~
+ * Notifications support
  * Shares support
  * ~~Talk support~~
 
 ### Extended Features with AppEcosystemV2:
  * Defining callback routes with `FastAPI` for Nextcloud
  * Registering UI elements in Nextcloud
  * Storing logs to the `nextcloud.log` file
```

### Comparing `nc_py_api-0.0.26/nc_py_api/_session.py` & `nc_py_api-0.0.27/nc_py_api/_session.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Session represents one connection to Nextcloud. All related stuff for these live here.
-"""
+"""Session represents one connection to Nextcloud. All related stuff for these live here."""
 
 import asyncio
 import hmac
 from abc import ABC, abstractmethod
 from collections.abc import Iterator
 from dataclasses import dataclass
 from datetime import datetime, timezone
@@ -12,91 +10,120 @@
 from json import dumps, loads
 from os import environ
 from typing import Optional, TypedDict, Union
 from urllib.parse import quote, urlencode
 
 from fastapi import Request
 from httpx import Client, Limits, ReadTimeout, Response
-from xxhash import xxh64
+
+try:
+    from xxhash import xxh64
+except ImportError as ex:
+    from ._deffered_error import DeferredError
+
+    xxh64 = DeferredError(ex)
+
 
 from . import options
 from .constants import OCSRespond
 from .exceptions import NextcloudException, NextcloudExceptionNotFound, check_error
 
 
 class ServerVersion(TypedDict):
-    """Nextcloud version information"""
+    """Nextcloud version information."""
 
     major: int
     """Major version"""
     minor: int
     """Minor version"""
     micro: int
     """Micro version"""
     string: str
     """Full version in string format"""
     extended_support: bool
     """Indicates if the subscription has extended support"""
 
 
 @dataclass
+class RuntimeOptions:
+    xdebug_session: str
+    timeout: Optional[int]
+    timeout_dav: Optional[int]
+    _nc_cert: Union[str, bool]
+
+    def __init__(self, **kwargs):
+        self.xdebug_session = kwargs.get("xdebug_session", options.XDEBUG_SESSION)
+        self.timeout = kwargs.get("npa_timeout", options.NPA_TIMEOUT)
+        self.timeout_dav = kwargs.get("npa_timeout_dav", options.NPA_TIMEOUT_DAV)
+        self._nc_cert = kwargs.get("npa_nc_cert", options.NPA_NC_CERT)
+
+    @property
+    def nc_cert(self) -> Union[str, bool]:
+        return self._nc_cert
+
+
+@dataclass
 class BasicConfig:
     endpoint: str
     dav_endpoint: str
     dav_url_suffix: str
+    options: RuntimeOptions
 
     def __init__(self, **kwargs):
-        full_nc_url = self._get_value("nextcloud_url", **kwargs)
+        full_nc_url = self._get_config_value("nextcloud_url", **kwargs)
         self.endpoint = full_nc_url.removesuffix("/index.php").removesuffix("/")
-        self.dav_url_suffix = self._get_value("dav_url_suffix", raise_not_found=False, **kwargs)
+        self.dav_url_suffix = self._get_config_value("dav_url_suffix", raise_not_found=False, **kwargs)
         if not self.dav_url_suffix:
             self.dav_url_suffix = "remote.php/dav"
         self.dav_url_suffix = "/" + self.dav_url_suffix.strip("/")
         self.dav_endpoint = self.endpoint + self.dav_url_suffix
+        self.options = RuntimeOptions(**kwargs)
 
     @staticmethod
-    def _get_value(value_name: str, raise_not_found=True, **kwargs):
-        value = kwargs.get(value_name, None)
-        if not value:
-            value = environ.get(value_name.upper(), None)
-        if not value and raise_not_found:
+    def _get_config_value(value_name: str, raise_not_found=True, **kwargs):
+        if value_name in kwargs:
+            return kwargs[value_name]
+        value_name_upper = value_name.upper()
+        if value_name_upper in environ:
+            return environ[value_name_upper]
+        if raise_not_found:
             raise ValueError(f"`{value_name}` is not found.")
-        return value
+        return None
 
 
 @dataclass
 class Config(BasicConfig):
     auth: tuple[str, str] = ("", "")
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.auth = (self._get_value("nc_auth_user", **kwargs), self._get_value("nc_auth_pass", **kwargs))
+        self.auth = (self._get_config_value("nc_auth_user", **kwargs), self._get_config_value("nc_auth_pass", **kwargs))
 
 
 @dataclass
 class AppConfig(BasicConfig):
-    """Application configuration"""
+    """Application configuration."""
 
     ae_version: str
     """AppEcosystem version"""
     app_name: str
     """Application name"""
     app_version: str
     """Application version"""
     app_secret: bytes
     """Application authentication secret"""
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
-        self.ae_version = self._get_value("ae_version", raise_not_found=False, **kwargs)
+        self.ae_version = self._get_config_value("ae_version", raise_not_found=False, **kwargs)
         if not self.ae_version:
             self.ae_version = "1.0.0"
-        self.app_name = self._get_value("app_id", **kwargs)
-        self.app_version = self._get_value("app_version", **kwargs)
-        self.app_secret = self._get_value("app_secret", **kwargs).encode("UTF-8")
+        self.app_name = self._get_config_value("app_id", **kwargs)
+        self.app_version = self._get_config_value("app_version", **kwargs)
+        self.app_secret = self._get_config_value("app_secret", **kwargs).encode("UTF-8")
 
 
 class NcSessionBasic(ABC):
     adapter: Client
     cfg: BasicConfig
     user: str
     custom_headers: dict
@@ -138,15 +165,15 @@
 
     def _ocs(self, method: str, path_params: str, headers: dict, data: Optional[bytes], **kwargs):
         self.init_adapter()
         url_params = f"{self.cfg.endpoint}{path_params}"
         info = f"request: method={method}, url={url_params}"
         nested_req = kwargs.pop("nested_req", False)
         try:
-            timeout = kwargs.pop("timeout", options.TIMEOUT)
+            timeout = kwargs.pop("timeout", self.cfg.options.timeout)
             if method == "GET":
                 response = self.adapter.get(url_params, headers=headers, timeout=timeout, **kwargs)
             else:
                 response = self.adapter.request(
                     method, url_params, headers=headers, content=data, timeout=timeout, **kwargs
                 )
         except ReadTimeout:
@@ -181,22 +208,23 @@
         data_bytes = None
         if data is not None:
             data_bytes = data.encode("UTF-8") if isinstance(data, str) else data
         return self._dav_stream(method, quote(self.cfg.dav_url_suffix + path), headers, data_bytes, **kwargs)
 
     def _dav(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Response:
         self.init_adapter()
-        timeout = kwargs.pop("timeout", options.TIMEOUT_DAV)
+        # self.cfg.
+        timeout = kwargs.pop("timeout", self.cfg.options.timeout_dav)
         return self.adapter.request(
             method, self.cfg.endpoint + path, headers=headers, content=data, timeout=timeout, **kwargs
         )
 
     def _dav_stream(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Iterator[Response]:
         self.init_adapter()
-        timeout = kwargs.pop("timeout", options.TIMEOUT_DAV)
+        timeout = kwargs.pop("timeout", self.cfg.options.timeout_dav)
         return self.adapter.stream(
             method, self.cfg.endpoint + path, headers=headers, content=data, timeout=timeout, **kwargs
         )
 
     def init_adapter(self, restart=False) -> None:
         if getattr(self, "adapter", None) is None or restart:
             if restart and hasattr(self, "adapter"):
@@ -240,17 +268,15 @@
     cfg: Config
 
     def __init__(self, **kwargs):
         self.cfg = Config(**kwargs)
         super().__init__(user=self.cfg.auth[0])
 
     def _create_adapter(self) -> Client:
-        return Client(
-            auth=self.cfg.auth, follow_redirects=True, limits=self.limits, verify=options.VERIFY_NC_CERTIFICATE
-        )
+        return Client(auth=self.cfg.auth, follow_redirects=True, limits=self.limits, verify=self.cfg.options.nc_cert)
 
 
 class NcSessionApp(NcSessionBasic):
     cfg: AppConfig
 
     def __init__(self, **kwargs):
         self.cfg = AppConfig(**kwargs)
@@ -265,15 +291,15 @@
         return super()._dav(method, path, headers, data, **kwargs)
 
     def _dav_stream(self, method: str, path: str, headers: dict, data: Optional[bytes], **kwargs) -> Iterator[Response]:
         self.sign_request(method, path, headers, data)
         return super()._dav_stream(method, path, headers, data, **kwargs)
 
     def _create_adapter(self) -> Client:
-        adapter = Client(follow_redirects=True, limits=self.limits, verify=options.VERIFY_NC_CERTIFICATE)
+        adapter = Client(follow_redirects=True, limits=self.limits, verify=self.cfg.options.nc_cert)
         adapter.headers.update(
             {
                 "AE-VERSION": self.cfg.ae_version,
                 "EX-APP-ID": self.cfg.app_name,
                 "EX-APP-VERSION": self.cfg.app_version,
             }
         )
```

### Comparing `nc_py_api-0.0.26/nc_py_api/appconfig_preferences_ex.py` & `nc_py_api-0.0.27/nc_py_api/appcfg_prefs_ex.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,68 +1,88 @@
-"""
-Nextcloud API for working with apps V2's storage w/wo user context(table oc_appconfig_ex/oc_preferences_ex).
-"""
-from typing import Optional, TypedDict, Union
+"""Nextcloud API for working with apps V2's storage w/wo user context(table oc_appconfig_ex/oc_preferences_ex)."""
+from dataclasses import dataclass
+from typing import Optional, Union
 
 from ._session import NcSessionBasic
 from .constants import APP_V2_BASIC_URL
 from .exceptions import NextcloudExceptionNotFound
 from .misc import require_capabilities
 
 
-class AppCfgPrefRecord(TypedDict):
-    configkey: str
-    configvalue: str
+@dataclass
+class CfgRecord:
+    """A representation of a single key-value pair returned from the `get_values` method."""
 
+    key: str
+    value: str
 
-class BasicAppCfgPref:
-    url_suffix: str
+    def __init__(self, raw_data: dict):
+        self.key = raw_data["configkey"]
+        self.value = raw_data["configvalue"]
+
+
+class _BasicAppCfgPref:
+    _url_suffix: str
 
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     def get_value(self, key: str, default=None) -> Optional[str]:
         if not key:
             raise ValueError("`key` parameter can not be empty")
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         r = self.get_values([key])
         if r:
-            return r[0]["configvalue"]
+            return r[0].value
         return default
 
-    def get_values(self, keys: list[str]) -> list[AppCfgPrefRecord]:
+    def get_values(self, keys: list[str]) -> list[CfgRecord]:
         if not keys:
             return []
         if not all(keys):
             raise ValueError("`key` parameter can not be empty")
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         data = {"configKeys": keys}
-        return self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self.url_suffix}/get-values", json=data)
-
-    def set(self, key: str, value: str) -> None:
-        if not key:
-            raise ValueError("`key` parameter can not be empty")
-        require_capabilities("app_ecosystem_v2", self._session.capabilities)
-        params = {"configKey": key, "configValue": value}
-        self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self.url_suffix}", json=params)
+        results = self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self._url_suffix}/get-values", json=data)
+        return [CfgRecord(i) for i in results]
 
     def delete(self, keys: Union[str, list[str]], not_fail=True) -> None:
         if isinstance(keys, str):
             keys = [keys]
         if not keys:
             return
         if not all(keys):
             raise ValueError("`key` parameter can not be empty")
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         try:
-            self._session.ocs(method="DELETE", path=f"{APP_V2_BASIC_URL}/{self.url_suffix}", json={"configKeys": keys})
+            self._session.ocs(method="DELETE", path=f"{APP_V2_BASIC_URL}/{self._url_suffix}", json={"configKeys": keys})
         except NextcloudExceptionNotFound as e:
             if not not_fail:
                 raise e from None
 
 
-class PreferencesExAPI(BasicAppCfgPref):
-    url_suffix = "ex-app/preference"
+class PreferencesExAPI(_BasicAppCfgPref):
+    """User specific preferences API."""
+
+    _url_suffix = "ex-app/preference"
+
+    def set_value(self, key: str, value: str) -> None:
+        if not key:
+            raise ValueError("`key` parameter can not be empty")
+        require_capabilities("app_ecosystem_v2", self._session.capabilities)
+        params = {"configKey": key, "configValue": value}
+        self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self._url_suffix}", json=params)
+
 
+class AppConfigExAPI(_BasicAppCfgPref):
+    """Non-user(App) specific preferences API."""
 
-class AppConfigExAPI(BasicAppCfgPref):
-    url_suffix = "ex-app/config"
+    _url_suffix = "ex-app/config"
+
+    def set_value(self, key: str, value: str, sensitive: bool = False) -> None:
+        if not key:
+            raise ValueError("`key` parameter can not be empty")
+        require_capabilities("app_ecosystem_v2", self._session.capabilities)
+        params: dict = {"configKey": key, "configValue": value}
+        if sensitive:
+            params["sensitive"] = True
+        self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{self._url_suffix}", json=params)
```

### Comparing `nc_py_api-0.0.26/nc_py_api/apps.py` & `nc_py_api-0.0.27/nc_py_api/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-"""
-Nextcloud API for working with applications.
-"""
+"""Nextcloud API for working with applications."""
 
 from typing import Optional, TypedDict
 
 from ._session import NcSessionBasic
 from .constants import APP_V2_BASIC_URL
 from .misc import require_capabilities
 
 ENDPOINT = "/ocs/v1.php/cloud/apps"
 
 
 class ExAppInfo(TypedDict):
-    """Information about the External Application"""
+    """Information about the External Application."""
 
     id: str
     """`id` of the application"""
     name: str
     """Display name"""
     version: str
     """Version of the application"""
@@ -35,77 +33,71 @@
         self._session = session
 
     def disable(self, app_name: str) -> None:
         """Disables the application.
 
         :param app_name: id of the application.
 
-        .. note:: Does not work in NextcloudApp mode, only for Nextcloud client mode."""
-
+        .. note:: Does not work in NextcloudApp mode, only for Nextcloud client mode.
+        """
         if not app_name:
             raise ValueError("`app_name` parameter can not be empty")
         self._session.ocs(method="DELETE", path=f"{ENDPOINT}/{app_name}")
 
     def enable(self, app_name: str) -> None:
         """Enables the application.
 
         :param app_name: id of the application.
 
-        .. note:: Does not work in NextcloudApp mode, only for Nextcloud client mode."""
-
+        .. note:: Does not work in NextcloudApp mode, only for Nextcloud client mode.
+        """
         if not app_name:
             raise ValueError("`app_name` parameter can not be empty")
         self._session.ocs(method="POST", path=f"{ENDPOINT}/{app_name}")
 
     def get_list(self, enabled: Optional[bool] = None) -> list[str]:
         """Get the list of installed applications.
 
         :param enabled: filter to list all/only enabled/only disabled applications.
         """
-
         params = None
         if enabled is not None:
             params = {"filter": "enabled" if enabled else "disabled"}
         result = self._session.ocs(method="GET", path=ENDPOINT, params=params)
         return list(result["apps"].values()) if isinstance(result["apps"], dict) else result["apps"]
 
     def is_installed(self, app_name: str) -> bool:
         """Checks if such application is installed.
 
         :param app_name: id of the application.
         """
-
         if not app_name:
             raise ValueError("`app_name` parameter can not be empty")
         return app_name in self.get_list()
 
     def is_enabled(self, app_name: str) -> bool:
         """Checks if such application is enabled.
 
         :param app_name: id of the application.
         """
-
         if not app_name:
             raise ValueError("`app_name` parameter can not be empty")
         return app_name in self.get_list(enabled=True)
 
     def is_disabled(self, app_name: str) -> bool:
         """Checks if such application is disabled.
 
         :param app_name: id of the application.
         """
-
         if not app_name:
             raise ValueError("`app_name` parameter can not be empty")
         return app_name in self.get_list(enabled=False)
 
     def ex_app_get_list(self) -> list[str]:
         """Gets the list of the external applications IDs installed on the server."""
-
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         return self._session.ocs(method="GET", path=f"{APP_V2_BASIC_URL}/ex-app/all", params={"extended": 0})
 
     def ex_app_get_info(self) -> list[ExAppInfo]:
         """Gets information of the external applications installed on the server."""
-
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         return self._session.ocs(method="GET", path=f"{APP_V2_BASIC_URL}/ex-app/all", params={"extended": 1})
```

### Comparing `nc_py_api-0.0.26/nc_py_api/exceptions.py` & `nc_py_api-0.0.27/nc_py_api/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Exceptions for the Nextcloud API.
-"""
+"""Exceptions for the Nextcloud API."""
 from httpx import codes
 
 
 class NextcloudException(Exception):
     """The base exception for all Nextcloud operation errors."""
 
     status_code: int
```

### Comparing `nc_py_api-0.0.26/nc_py_api/files.py` & `nc_py_api-0.0.27/nc_py_api/files.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,187 +1,27 @@
-"""
-Nextcloud API for working with the file system.
-"""
+"""Nextcloud API for working with the file system."""
 
 import builtins
 import os
-from dataclasses import dataclass
-from datetime import datetime
-from email.utils import parsedate_to_datetime
 from io import BytesIO
 from json import dumps, loads
 from pathlib import Path
 from random import choice
 from string import ascii_lowercase, digits
 from typing import Optional, Union
 from urllib.parse import unquote
 from xml.etree import ElementTree
 
 import xmltodict
 from httpx import Response
 
 from ._session import NcSessionBasic
 from .exceptions import NextcloudException, check_error
-
-
-@dataclass
-class FsNodeInfo:
-    """Extra FS object attributes from Nextcloud"""
-
-    size: int
-    """Length of file in bytes, zero for directories.."""
-    content_length: int
-    """For directories it is size of all content in it, for files it is equal to ``size``."""
-    permissions: str
-    """Permissions for the object."""
-    favorite: bool
-    """Flag indicating if the object is marked as favorite."""
-    fileid: int
-    """Clear file ID without Nextcloud instance ID."""
-    _last_modified: datetime
-
-    def __init__(self, **kwargs):
-        self.size = kwargs.get("size", 0)
-        self.content_length = kwargs.get("content_length", 0)
-        self.permissions = kwargs.get("permissions", "")
-        self.favorite = kwargs.get("favorite", False)
-        self.fileid = kwargs.get("fileid", 0)
-        try:
-            self.last_modified = kwargs.get("last_modified", datetime(1970, 1, 1))
-        except (ValueError, TypeError):
-            self.last_modified = datetime(1970, 1, 1)
-
-    @property
-    def last_modified(self) -> datetime:
-        """Time when the object was last modified.
-
-        .. note:: ETag if more preferable way to check if the object was changed."""
-
-        return self._last_modified
-
-    @last_modified.setter
-    def last_modified(self, value: Union[str, datetime]):
-        if isinstance(value, str):
-            self._last_modified = parsedate_to_datetime(value)
-        else:
-            self._last_modified = value
-
-
-@dataclass
-class FsNode:
-    """A class that represents a Nextcloud file object.
-
-    Acceptable itself as a ``path`` parameter for the most file APIs."""
-
-    full_path: str
-    """Path to the object, including the username. Does not include `dav` prefix"""
-
-    file_id: str
-    """File ID + NC instance ID"""
-
-    etag: str
-    """An entity tag (ETag) of the object"""
-
-    info: FsNodeInfo
-    """Additional extra information for the object"""
-
-    def __init__(self, full_path: str, **kwargs):
-        self.full_path = full_path
-        self.file_id = kwargs.get("file_id", "")
-        self.etag = kwargs.get("etag", "")
-        self.info = FsNodeInfo(**kwargs)
-
-    @property
-    def is_dir(self) -> bool:
-        """Returns ``True`` for the directories, ``False`` otherwise."""
-
-        return self.full_path.endswith("/")
-
-    def __str__(self):
-        return (
-            f"{'Dir' if self.is_dir else 'File'}: `{self.name}` with id={self.file_id}"
-            f" last modified at {str(self.info.last_modified)} and {self.info.permissions} permissions."
-        )
-
-    def __eq__(self, other):
-        if self.file_id and self.file_id == other.file_id:
-            return True
-        return False
-
-    @property
-    def has_extra(self) -> bool:
-        """Flag indicating whether this ``FsNode`` was obtained by the `mkdir` or `upload`
-        methods and does not contain extended information."""
-
-        return bool(self.info.permissions)
-
-    @property
-    def name(self) -> str:
-        """Returns last ``pathname`` component."""
-
-        return self.full_path.rstrip("/").rsplit("/", maxsplit=1)[-1]
-
-    @property
-    def user(self) -> str:
-        """Returns user ID extracted from the `full_path`."""
-
-        return self.full_path.lstrip("/").split("/", maxsplit=2)[1]
-
-    @property
-    def user_path(self) -> str:
-        """Returns path relative to the user's root directory."""
-
-        return self.full_path.lstrip("/").split("/", maxsplit=2)[-1]
-
-    @property
-    def is_shared(self) -> bool:
-        """Check if a file or folder is shared"""
-
-        return self.info.permissions.find("S") != -1
-
-    @property
-    def is_shareable(self) -> bool:
-        """Check if a file or folder can be shared"""
-
-        return self.info.permissions.find("R") != -1
-
-    @property
-    def is_mounted(self) -> bool:
-        """Check if a file or folder is mounted"""
-
-        return self.info.permissions.find("M") != -1
-
-    @property
-    def is_readable(self) -> bool:
-        """Check if the file or folder is readable"""
-
-        return self.info.permissions.find("G") != -1
-
-    @property
-    def is_deletable(self) -> bool:
-        """Check if a file or folder can be deleted"""
-
-        return self.info.permissions.find("D") != -1
-
-    @property
-    def is_updatable(self) -> bool:
-        """Check if file/directory is writable"""
-
-        if self.is_dir:
-            return self.info.permissions.find("NV") != -1
-        return self.info.permissions.find("W") != -1
-
-    @property
-    def is_creatable(self) -> bool:
-        """Check whether new files or folders can be created inside this folder"""
-
-        if not self.is_dir:
-            return False
-        return self.info.permissions.find("CK") != -1
-
+from .files_defs import FsNode
+from .files_sharing import FilesSharingAPI
 
 PROPFIND_PROPERTIES = [
     "d:resourcetype",
     "d:getlastmodified",
     "d:getcontentlength",
     "d:getetag",
     "oc:size",
@@ -210,58 +50,58 @@
     "size": "oc:size",  # gt, gte, eq, lt
     "favorite": "oc:favorite",  # eq
     "fileid": "oc:fileid",  # eq
 }
 
 
 class FilesAPI:
-    """This class provides all WebDAV functionality related to the files."""
+    """Class that encapsulates the file system and file sharing functionality."""
+
+    sharing: FilesSharingAPI
+    """API for managing Files Shares"""
 
     def __init__(self, session: NcSessionBasic):
         self._session = session
+        self.sharing = FilesSharingAPI(session)
 
     def listdir(self, path: Union[str, FsNode] = "", depth: int = 1, exclude_self=True) -> list[FsNode]:
         """Returns a list of all entries in the specified directory.
 
         :param path: path to the directory to get the list.
         :param depth: how many directory levels should be included in output. Default = **1** (only specified directory)
         :param exclude_self: boolean value indicating whether the `path` itself should be excluded from the list or not.
             Default = **True**.
         """
-
         if exclude_self and not depth:
             raise ValueError("Wrong input parameters, query will return nothing.")
         properties = PROPFIND_PROPERTIES
         path = path.user_path if isinstance(path, FsNode) else path
         return self._listdir(self._session.user, path, properties=properties, depth=depth, exclude_self=exclude_self)
 
     def by_id(self, file_id: Union[int, str, FsNode]) -> Optional[FsNode]:
-        """Returns :py:class:`FsNode` by file_id if any.
+        """Returns :py:class:`~nc_py_api.files_defs.FsNode` by file_id if any.
 
         :param file_id: can be full file ID with Nextcloud instance ID or only clear file ID.
         """
-
         file_id = file_id.file_id if isinstance(file_id, FsNode) else file_id
         result = self.find(req=["eq", "fileid", file_id])
         return result[0] if result else None
 
     def by_path(self, path: Union[str, FsNode]) -> Optional[FsNode]:
-        """Returns :py:class:`FsNode` by exact path if any."""
-
+        """Returns :py:class:`~nc_py_api.files_defs.FsNode` by exact path if any."""
         path = path.user_path if isinstance(path, FsNode) else path
         result = self.listdir(path, depth=0, exclude_self=False)
         return result[0] if result else None
 
     def find(self, req: list, path: Union[str, FsNode] = "") -> list[FsNode]:
         """Searches a directory for a file or subdirectory with a name.
 
         :param req: list of conditions to search for. Detailed description here...
         :param path: path where to search from. Default = **""**.
         """
-
         # `req` possible keys: "name", "mime", "last_modified", "size", "favorite", "fileid"
         path = path.user_path if isinstance(path, FsNode) else path
         root = ElementTree.Element(
             "d:searchrequest",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns", "xmlns:nc": "http://nextcloud.org/ns"},
         )
         xml_search = ElementTree.SubElement(root, "d:basicsearch")
@@ -281,29 +121,27 @@
         return self._lf_parse_webdav_records(webdav_response, request_info)
 
     def download(self, path: Union[str, FsNode]) -> bytes:
         """Downloads and returns the content of a file.
 
         :param path: path to download file.
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         response = self._session.dav("GET", self._dav_get_obj_path(self._session.user, path))
         check_error(response.status_code, f"download: user={self._session.user}, path={path}")
         return response.content
 
     def download2stream(self, path: Union[str, FsNode], fp, **kwargs) -> None:
         """Downloads file to the given `fp` object.
 
         :param path: path to download file.
         :param fp: filename (string), pathlib.Path object or a file object.
             The object must implement the ``file.write`` method and be able to write binary data.
         :param kwargs: **chunk_size** an int value specifying chunk size to write. Default = **4Mb**
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         if isinstance(fp, (str, Path)):
             with builtins.open(fp, "wb") as f:
                 self.__download2stream(path, f, **kwargs)
         elif hasattr(fp, "write"):
             self.__download2stream(path, fp, **kwargs)
         else:
@@ -311,60 +149,56 @@
 
     def upload(self, path: Union[str, FsNode], content: Union[bytes, str]) -> FsNode:
         """Creates a file with the specified content at the specified path.
 
         :param path: file's upload path.
         :param content: content to create the file. If it is a string, it will be encoded into bytes using UTF-8.
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         full_path = self._dav_get_obj_path(self._session.user, path)
         response = self._session.dav("PUT", full_path, data=content)
         check_error(response.status_code, f"upload: user={self._session.user}, path={path}, size={len(content)}")
         return FsNode(full_path.strip("/"), **self.__get_etag_fileid_from_response(response))
 
     def upload_stream(self, path: Union[str, FsNode], fp, **kwargs) -> FsNode:
         """Creates a file with content provided by `fp` object at the specified path.
 
         :param path: file's upload path.
         :param fp: filename (string), pathlib.Path object or a file object.
             The object must implement the ``file.read`` method providing data with str or bytes type.
         :param kwargs: **chunk_size** an int value specifying chunk size to read. Default = **4Mb**
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         if isinstance(fp, (str, Path)):
             with builtins.open(fp, "rb") as f:
                 return self.__upload_stream(path, f, **kwargs)
         elif hasattr(fp, "read"):
             return self.__upload_stream(path, fp, **kwargs)
         else:
             raise TypeError("`fp` must be a path to file or an object with `read` method.")
 
     def mkdir(self, path: Union[str, FsNode]) -> FsNode:
         """Creates a new directory.
 
         :param path: path of the directory to be created.
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         full_path = self._dav_get_obj_path(self._session.user, path)
         response = self._session.dav("MKCOL", full_path)
         check_error(response.status_code, f"mkdir: user={self._session.user}, path={path}")
         full_path += "/" if not full_path.endswith("/") else ""
         return FsNode(full_path.lstrip("/"), **self.__get_etag_fileid_from_response(response))
 
     def makedirs(self, path: Union[str, FsNode], exist_ok=False) -> Optional[FsNode]:
         """Creates a new directory and subdirectories.
 
         :param path: path of the directories to be created.
         :param exist_ok: ignore error if any of pathname components already exists.
         :returns: `FsNode` if directory was created or ``None`` if it was already created.
         """
-
         _path = ""
         path = path.user_path if isinstance(path, FsNode) else path
         result = None
         for i in Path(path).parts:
             _path = os.path.join(_path, i)
             if not exist_ok:
                 result = self.mkdir(_path)
@@ -378,30 +212,28 @@
 
     def delete(self, path: Union[str, FsNode], not_fail=False) -> None:
         """Deletes a file/directory (moves to trash if trash is enabled).
 
         :param path: path to delete.
         :param not_fail: if set to ``True`` and the object is not found, it does not raise an exception.
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         response = self._session.dav("DELETE", self._dav_get_obj_path(self._session.user, path))
         if response.status_code == 404 and not_fail:
             return
         check_error(response.status_code, f"delete: user={self._session.user}, path={path}")
 
     def move(self, path_src: Union[str, FsNode], path_dest: Union[str, FsNode], overwrite=False) -> FsNode:
         """Moves an existing file or a directory.
 
         :param path_src: path of an existing file/directory.
         :param path_dest: name of the new one.
         :param overwrite: if ``True`` and the destination object already exists, it gets overwritten.
             Default = **False**.
         """
-
         path_src = path_src.user_path if isinstance(path_src, FsNode) else path_src
         full_dest_path = self._dav_get_obj_path(
             self._session.user, path_dest.user_path if isinstance(path_dest, FsNode) else path_dest
         )
         dest = self._session.cfg.dav_endpoint + full_dest_path
         headers = {"Destination": dest, "Overwrite": "T" if overwrite else "F"}
         response = self._session.dav(
@@ -416,15 +248,14 @@
         """Copies an existing file/directory.
 
         :param path_src: path of an existing file/directory.
         :param path_dest: name of the new one.
         :param overwrite: if ``True`` and the destination object already exists, it gets overwritten.
             Default = **False**.
         """
-
         path_src = path_src.user_path if isinstance(path_src, FsNode) else path_src
         full_dest_path = self._dav_get_obj_path(
             self._session.user, path_dest.user_path if isinstance(path_dest, FsNode) else path_dest
         )
         dest = self._session.cfg.dav_endpoint + full_dest_path
         headers = {"Destination": dest, "Overwrite": "T" if overwrite else "F"}
         response = self._session.dav(
@@ -433,15 +264,14 @@
             headers=headers,
         )
         check_error(response.status_code, f"copy: user={self._session.user}, src={path_src}, dest={dest}, {overwrite}")
         return self.find(req=["eq", "fileid", response.headers["OC-FileId"]])[0]
 
     def listfav(self) -> list[FsNode]:
         """Returns a list of the current user's favorite files."""
-
         root = ElementTree.Element(
             "oc:filter-files",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns", "xmlns:nc": "http://nextcloud.org/ns"},
         )
         xml_filter_rules = ElementTree.SubElement(root, "oc:filter-rules")
         ElementTree.SubElement(xml_filter_rules, "oc:favorite").text = "1"
         webdav_response = self._session.dav(
@@ -453,15 +283,14 @@
 
     def setfav(self, path: Union[str, FsNode], value: Union[int, bool]) -> None:
         """Sets or unsets favourite flag for specific file.
 
         :param path: path to the object to set the state.
         :param value: value to set for the ``favourite`` state.
         """
-
         path = path.user_path if isinstance(path, FsNode) else path
         root = ElementTree.Element(
             "d:propertyupdate",
             attrib={"xmlns:d": "DAV:", "xmlns:oc": "http://owncloud.org/ns"},
         )
         xml_set = ElementTree.SubElement(root, "d:set")
         xml_set_prop = ElementTree.SubElement(xml_set, "d:prop")
```

### Comparing `nc_py_api-0.0.26/nc_py_api/files_sharing.py` & `nc_py_api-0.0.27/nc_py_api/files_sharing.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,33 @@
-"""
-Nextcloud API for working with the files shares.
-"""
+"""Nextcloud API for working with the files shares."""
 
 from typing import Union
 
 from ._session import NcSessionBasic
-from .constants import SharePermissions, ShareType
-from .files import FsNode
+from .files_defs import FsNode, Share, SharePermissions, ShareType
 from .misc import check_capabilities, require_capabilities
 
 ENDPOINT_BASE = "/ocs/v1.php/apps/files_sharing/api/v1/"
 
 
-class Share:
-    """Class represents one Nextcloud Share."""
-
-    def __init__(self, raw_data: dict):
-        self.raw_data = raw_data
-
-    @property
-    def share_id(self) -> int:
-        return int(self.raw_data["id"])
-
-    @property
-    def type(self) -> ShareType:
-        return ShareType(int(self.raw_data["share_type"]))
-
-    @property
-    def permissions(self) -> SharePermissions:
-        """Recipient permissions"""
-
-        return SharePermissions(int(self.raw_data["permissions"]))
-
-    @property
-    def url(self) -> str:
-        return self.raw_data.get("url", "")
-
-    @property
-    def path(self) -> str:
-        return self.raw_data.get("path", "")
-
-    @property
-    def label(self) -> str:
-        return self.raw_data.get("label", "")
-
-    @property
-    def note(self) -> str:
-        return self.raw_data.get("note", "")
-
-    @property
-    def mimetype(self) -> str:
-        return self.raw_data.get("mimetype", "")
-
-
 class FilesSharingAPI:
-    """This class provides all File Sharing functionality."""
+    """Class provides all File Sharing functionality."""
 
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     @property
     def available(self) -> bool:
         """Returns True if the Nextcloud instance supports this feature, False otherwise."""
-
         return not check_capabilities("files_sharing", self._session.capabilities)
 
     def get_list(
         self, shared_with_me=False, reshares=False, subfiles=False, path: Union[str, FsNode] = ""
     ) -> list[Share]:
         """Returns lists of shares."""
-
         require_capabilities("files_sharing", self._session.capabilities)
         path = path.user_path if isinstance(path, FsNode) else path
         params = {
             "shared_with_me": "true" if shared_with_me else "false",
             "reshares": "true" if reshares else "false",
             "subfiles": "true" if subfiles else "false",
         }
@@ -105,15 +59,14 @@
             * ``send_password_by_talk`` - boolean indicating should password be automatically delivered using Talk.
               default = ``False``
             * ``expire_date`` - :py:class:`~datetime.datetime` time when share should expire.
               `hours, minutes, seconds` are ignored. default = ``None``
             * ``note`` - string with note, if any. default = ``""``
             * ``label`` - string with label, if any. default = ``""``
         """
-
         require_capabilities("files_sharing", self._session.capabilities)
         path = path.user_path if isinstance(path, FsNode) else path
         params = {
             "path": path,
             "permissions": int(permissions),
             "shareType": int(share_type),
         }
@@ -134,10 +87,9 @@
         return Share(self._session.ocs(method="POST", path=f"{ENDPOINT_BASE}/shares", params=params))
 
     def delete(self, share_id: Union[int, Share]) -> None:
         """Removes the given share.
 
         :param share_id: The Share object or an ID of the share.
         """
-
         share_id = share_id.share_id if isinstance(share_id, Share) else share_id
         self._session.ocs(method="DELETE", path=f"{ENDPOINT_BASE}/shares/{share_id}")
```

### Comparing `nc_py_api-0.0.26/nc_py_api/integration_fastapi.py` & `nc_py_api-0.0.27/nc_py_api/integration_fastapi.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-Directly related stuff to FastAPI.
-"""
+"""Directly related stuff to FastAPI."""
 
 from typing import Annotated, Callable, Optional
 
 from fastapi import Depends, FastAPI, HTTPException, Request, status
 from fastapi.responses import JSONResponse
 
 from .constants import ApiScopesStruct
```

### Comparing `nc_py_api-0.0.26/nc_py_api/nextcloud.py` & `nc_py_api-0.0.27/nc_py_api/nextcloud.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,192 +1,165 @@
-"""
-Nextcloud class providing access to all API endpoints.
-"""
+"""Nextcloud class providing access to all API endpoints."""
 from abc import ABC
 from typing import Optional, Union
 
 from fastapi import Request
 
 from ._session import AppConfig, NcSession, NcSessionApp, NcSessionBasic, ServerVersion
-from .appconfig_preferences_ex import AppConfigExAPI, PreferencesExAPI
+from .appcfg_prefs_ex import AppConfigExAPI, PreferencesExAPI
 from .apps import AppAPI
 from .constants import APP_V2_BASIC_URL, ApiScope, LogLvl
 from .files import FilesAPI
-from .files_sharing import FilesSharingAPI
+from .gui import GuiApi
 from .misc import check_capabilities
 from .preferences import PreferencesAPI
 from .theming import ThemingInfo, get_parsed_theme
-from .ui_files_actions_menu import UiFilesActionsAPI
 from .users import UsersAPI
-from .users_groups import UserGroupsAPI
-from .users_status import UserStatusAPI
-from .weather_status import WeatherStatusAPI
 
 
-class NextcloudBasic(ABC):
+class _NextcloudBasic(ABC):
     apps: AppAPI
     """Nextcloud API for App management"""
     files: FilesAPI
-    """Nextcloud FileSystem API"""
-    files_sharing: FilesSharingAPI
-    """Nextcloud File Sharing API"""
-    preferences_api: PreferencesAPI
+    """Nextcloud API for File System and Files Sharing"""
+    preferences: PreferencesAPI
     # """Nextcloud User Preferences API"""
     users: UsersAPI
-    """Nextcloud API for User management"""
-    users_groups: UserGroupsAPI
-    # """Nextcloud API for managing user groups"""
-    users_status: UserStatusAPI
-    """Nextcloud API for managing user statuses"""
-    weather_status: WeatherStatusAPI
-    """Nextcloud API for user's weather status"""
+    """Nextcloud API for managing users, user groups, user status, user weather status"""
     _session: NcSessionBasic
 
     def _init_api(self, session: NcSessionBasic):
         self.apps = AppAPI(session)
         self.files = FilesAPI(session)
-        self.files_sharing = FilesSharingAPI(session)
-        self.preferences_api = PreferencesAPI(session)
+        self.preferences = PreferencesAPI(session)
         self.users = UsersAPI(session)
-        self.users_groups = UserGroupsAPI(session)
-        self.users_status = UserStatusAPI(session)
-        self.weather_status = WeatherStatusAPI(session)
 
     @property
     def capabilities(self) -> dict:
         """Returns the capabilities of the Nextcloud instance."""
-
         return self._session.capabilities
 
     @property
     def srv_version(self) -> ServerVersion:
         """Returns dictionary with the server version."""
-
         return self._session.nc_version
 
     def check_capabilities(self, capabilities: Union[str, list[str]]) -> list[str]:
         """Returns the list with missing capabilities if any.
 
-        :param capabilities: one or more features to check for."""
-
+        :param capabilities: one or more features to check for.
+        """
         return check_capabilities(capabilities, self.capabilities)
 
     def update_server_info(self) -> None:
         """Updates the capabilities and the Nextcloud version.
 
         *In normal cases, it is called automatically and there is no need to call it manually.*
         """
-
         self._session.update_server_info()
 
     @property
     def theme(self) -> Optional[ThemingInfo]:
-        """Returns Theme information"""
-
+        """Returns Theme information."""
         return get_parsed_theme(self.capabilities["theming"]) if "theming" in self.capabilities else None
 
 
-class Nextcloud(NextcloudBasic):
+class Nextcloud(_NextcloudBasic):
     """Nextcloud client class.
 
-    Allows you to connect to Nextcloud and perform operations on files, shares, users, and everything else."""
+    Allows you to connect to Nextcloud and perform operations on files, shares, users, and everything else.
+    """
 
     _session: NcSession
 
     def __init__(self, **kwargs):
         """:param dsdada: ddsdsds"""
-
         self._session = NcSession(**kwargs)
         self._init_api(self._session)
 
     @property
     def user(self) -> str:
-        """Returns current user name"""
-
+        """Returns current user name."""
         return self._session.user
 
 
-class NextcloudApp(NextcloudBasic):
+class NextcloudApp(_NextcloudBasic):
     """Class for creating Nextcloud applications.
 
     Provides additional API required for applications such as user impersonation,
     endpoint registration, new authentication method, etc.
 
     .. note:: Instance of this class should not be created directly in ``normal`` applications,
-        it will be provided for each app endpoint call."""
+        it will be provided for each app endpoint call.
+    """
 
     _session: NcSessionApp
-    appconfig_ex_api: AppConfigExAPI
-    preferences_ex_api: PreferencesExAPI
-    ui_files_actions: UiFilesActionsAPI
+    appconfig_ex: AppConfigExAPI
+    gui: GuiApi
+    preferences_ex: PreferencesExAPI
 
     def __init__(self, **kwargs):
         self._session = NcSessionApp(**kwargs)
         self._init_api(self._session)
-        self.appconfig_ex_api = AppConfigExAPI(self._session)
-        self.preferences_ex_api = PreferencesExAPI(self._session)
-        self.ui_files_actions = UiFilesActionsAPI(self._session)
+        self.appconfig_ex = AppConfigExAPI(self._session)
+        self.preferences_ex = PreferencesExAPI(self._session)
+        self.gui = GuiApi(self._session)
 
     def log(self, log_lvl: LogLvl, content: str) -> None:
         """Writes log to the Nextcloud log file.
 
         :param log_lvl: level of the log, content belongs to.
         :param content: string to write into the log.
         """
-
         if self.check_capabilities("app_ecosystem_v2"):
             return
         if int(log_lvl) < self.capabilities["app_ecosystem_v2"].get("loglevel", 0):
             return
         self._session.ocs(
             method="POST", path=f"{APP_V2_BASIC_URL}/log", json={"level": int(log_lvl), "message": content}
         )
 
     def users_list(self) -> list[str]:
         """Returns list of users on the Nextcloud instance. **Available** only for ``System`` applications."""
-
         return self._session.ocs("GET", path=f"{APP_V2_BASIC_URL}/users", params={"format": "json"})
 
     def scope_allowed(self, scope: ApiScope) -> bool:
         """Check if API scope is avalaible for application.
 
-        Useful for applications which declare ``Optional`` scopes, to check if they are allowed for them."""
-
+        Useful for applications which declare ``Optional`` scopes, to check if they are allowed for them.
+        """
         if self.check_capabilities("app_ecosystem_v2"):
             return False
         return scope in self.capabilities["app_ecosystem_v2"]["scopes"]
 
     @property
     def user(self) -> str:
         """Property containing the current username.
 
         *System Applications* can set it and impersonate the user. For normal applications, it is set automatically.
         """
-
         return self._session.user
 
     @user.setter
     def user(self, value: str):
         if self._session.user != value:
             self._session.user = value
             self._session.update_server_info()
 
     @property
     def app_cfg(self) -> AppConfig:
         """Returns deploy config, with AppEcosystem version, Application version and name."""
-
         return self._session.cfg
 
     def request_sign_check(self, request: Request) -> bool:
         """Verifies the signature and validity of an incoming request from the Nextcloud.
 
         :param request: The `Starlette request <https://www.starlette.io/requests/>`_
 
         .. note:: In most cases ``nc: Annotated[NextcloudApp, Depends(nc_app)]`` should be used.
         """
-
         try:
             self._session.sign_check(request)
         except ValueError as e:
             print(e)
             return False
         return True
```

### Comparing `nc_py_api-0.0.26/nc_py_api/preferences.py` & `nc_py_api-0.0.27/nc_py_api/preferences.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-"""
-Nextcloud API for working with classics app's storage with user's context (table oc_preferences).
-"""
+"""Nextcloud API for working with classics app's storage with user's context (table oc_preferences)."""
 
 from ._session import NcSessionBasic
 from .misc import check_capabilities, require_capabilities
 
 ENDPOINT = "/ocs/v1.php/apps/provisioning_api/api/v1/config/users"
 
 
 class PreferencesAPI:
+    """API for setting/removing configuration values of applications that support it."""
+
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
     @property
     def available(self) -> bool:
+        """Returns True if the Nextcloud instance supports this feature, False otherwise."""
         return not check_capabilities("provisioning_api", self._session.capabilities)
 
-    def set(self, app_name: str, key: str, value: str) -> None:
+    def set_value(self, app_name: str, key: str, value: str) -> None:
+        """Sets the value for the key for the specific application."""
         require_capabilities("provisioning_api", self._session.capabilities)
         self._session.ocs(method="POST", path=f"{ENDPOINT}/{app_name}/{key}", params={"configValue": value})
 
     def delete(self, app_name: str, key: str) -> None:
+        """Removes a key and its value for a specific application."""
         require_capabilities("provisioning_api", self._session.capabilities)
         self._session.ocs(method="DELETE", path=f"{ENDPOINT}/{app_name}/{key}")
```

### Comparing `nc_py_api-0.0.26/nc_py_api/theming.py` & `nc_py_api-0.0.27/nc_py_api/theming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-"""
-Nextcloud stuff for work with Theming app.
-"""
+"""Nextcloud stuff for work with Theming app."""
 
 from typing import TypedDict
 
 
 class ThemingInfo(TypedDict):
-    """Nextcloud Theme information"""
+    """Nextcloud Theme information."""
 
     name: str
     """Name of the Nextcloud instance"""
     url: str
     """Url that set in Theme app"""
     slogan: str
     """Slogan, e.g. 'a safe home for all your data'"""
@@ -25,15 +23,14 @@
     """Either an URL of the background image or a hex color value"""
     background_plain: bool
     background_default: bool
 
 
 def convert_str_color(theming_capability: dict, key: str) -> tuple[int, int, int]:
     """Returns a tuple of integers representing the RGB color for the specified theme key."""
-
     if key not in theming_capability:
         return 0, 0, 0
     value = theming_capability[key]
     if not value or value == "#":
         return 0, 0, 0
     return int(value[1:3], 16), int(value[3:5], 16), int(value[5:7], 16)
```

### Comparing `nc_py_api-0.0.26/nc_py_api/ui_files_actions_menu.py` & `nc_py_api-0.0.27/nc_py_api/gui_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,24 @@
-"""
-Nextcloud API for working with drop down file's menu.
-"""
-
-from pydantic import BaseModel
-
+"""Nextcloud API for working with drop-down file's menu."""
 from ._session import NcSessionApp
 from .constants import APP_V2_BASIC_URL
 from .exceptions import NextcloudExceptionNotFound
 from .misc import require_capabilities
 
-
-class UiActionFileInfo(BaseModel):
-    fileId: int
-    name: str
-    dir: str
-
-
-class UiFileActionHandlerInfo(BaseModel):
-    actionName: str
-    actionHandler: str
-    actionFile: UiActionFileInfo
-
-
 ENDPOINT_SUFFIX = "files/actions/menu"
 
 
-class UiFilesActionsAPI:
+class GuiFilesActionsAPI:
+    """API for the drop-down menu in Nextcloud ``Files`` app."""
+
     def __init__(self, session: NcSessionApp):
         self._session = session
 
     def register(self, name: str, display_name: str, callback_url: str, **kwargs) -> None:
+        """Registers the files a dropdown menu element."""
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         params = {
             "fileActionMenuParams": {
                 "name": name,
                 "display_name": display_name,
                 "mime": kwargs.get("mime", "file"),
                 "permissions": kwargs.get("permissions", 31),
@@ -42,14 +27,15 @@
                 "icon_class": kwargs.get("icon_class", "icon-app-ecosystem-v2"),
                 "action_handler": callback_url,
             },
         }
         self._session.ocs(method="POST", path=f"{APP_V2_BASIC_URL}/{ENDPOINT_SUFFIX}", json=params)
 
     def unregister(self, name: str, not_fail=True) -> None:
+        """Removes files dropdown menu element."""
         require_capabilities("app_ecosystem_v2", self._session.capabilities)
         params = {"fileActionMenuName": name}
         try:
             self._session.ocs(method="DELETE", path=f"{APP_V2_BASIC_URL}/{ENDPOINT_SUFFIX}", json=params)
         except NextcloudExceptionNotFound as e:
             if not not_fail:
                 raise e from None
```

### Comparing `nc_py_api-0.0.26/nc_py_api/users.py` & `nc_py_api-0.0.27/nc_py_api/users.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,62 @@
-"""
-Nextcloud API for working with users.
-"""
+"""Nextcloud API for working with users."""
 
 from typing import Optional
 
 from ._session import NcSessionBasic
 from .misc import kwargs_to_dict
+from .users_groups import UserGroupsAPI
+from .users_notifications import NotificationsAPI
+from .users_status import UserStatusAPI
+from .users_weather import WeatherStatusAPI
 
 ENDPOINT_BASE = "/ocs/v1.php/cloud"
 ENDPOINT = f"{ENDPOINT_BASE}/users"
 
 
 class UsersAPI:
-    """The class provides the user management API on the Nextcloud server.
+    """The class provides the user, user groups, user status API on the Nextcloud server.
 
     .. note:: In NextcloudApp mode, only ``get_list`` and ``get_details`` methods are available.
     """
 
+    groups: UserGroupsAPI
+    # """API for managing user groups"""
+    status: UserStatusAPI
+    """API for managing user statuses"""
+    notifications: NotificationsAPI
+    # """API for managing user notifications"""
+    weather: WeatherStatusAPI
+    """API for managing user weather statuses"""
+
     def __init__(self, session: NcSessionBasic):
         self._session = session
+        self.groups = UserGroupsAPI(session)
+        self.status = UserStatusAPI(session)
+        self.notifications = NotificationsAPI(session)
+        self.weather = WeatherStatusAPI(session)
 
     def get_list(
         self, mask: Optional[str] = "", limit: Optional[int] = None, offset: Optional[int] = None
     ) -> list[str]:
         """Returns list of user IDs.
 
         :param mask: user ID mask to apply.
         :param limit: limits the number of results.
         :param offset: offset of results.
         """
-
         data = kwargs_to_dict(["search", "limit", "offset"], search=mask, limit=limit, offset=offset)
         response_data = self._session.ocs(method="GET", path=ENDPOINT, params=data)
         return response_data["users"] if response_data else {}
 
     def get_details(self, user_id: str = "") -> dict:
         """Returns detailed user information.
 
         :param user_id: the identifier of the user about which information is to be returned.
         """
-
         if not user_id:
             user_id = self._session.user
         if not user_id:
             raise ValueError("user_id can not be empty.")
         return self._session.ocs(method="GET", path=f"{ENDPOINT}/{user_id}")
 
     def create(self, user_id: str, **kwargs) -> None:
@@ -58,15 +71,14 @@
             * ``email`` - email of the new user. If ``password`` is not provided, then this field should be filled.
             * ``displayname`` - display name of the new user.
             * ``groups`` - groups IDs to which user belongs.
             * ``subadmin`` - boolean indicating is user should be the subadmin.
             * ``quota`` - quota for the user, if needed.
             * ``language`` - default language for the user.
         """
-
         password = kwargs.get("password", None)
         email = kwargs.get("email", None)
         if not password and not email:
             raise ValueError("Either password or email must be set")
         data = {"userid": user_id}
         for k in ("password", "displayname", "email", "groups", "subadmin", "quota", "language"):
             if k in kwargs:
@@ -74,84 +86,74 @@
         self._session.ocs(method="POST", path=ENDPOINT, params=data)
 
     def delete(self, user_id: str) -> None:
         """Deletes user from the Nextcloud server.
 
         :param user_id: id of the user.
         """
-
         self._session.ocs(method="DELETE", path=f"{ENDPOINT}/{user_id}")
 
     def enable(self, user_id: str) -> None:
         """Enables user on the Nextcloud server.
 
         :param user_id: id of the user.
         """
-
         self._session.ocs(method="PUT", path=f"{ENDPOINT}/{user_id}/enable")
 
     def disable(self, user_id: str) -> None:
         """Disables user on the Nextcloud server.
 
         :param user_id: id of the user.
         """
-
         self._session.ocs(method="PUT", path=f"{ENDPOINT}/{user_id}/disable")
 
     def resend_welcome_email(self, user_id: str) -> None:
         """Send welcome email for specified user again.
 
         :param user_id: id of the user.
         """
-
         self._session.ocs(method="POST", path=f"{ENDPOINT}/{user_id}/welcome")
 
     def editable_fields(self) -> list[str]:
         """Returns user fields that avalaible for edit."""
-
         return self._session.ocs(method="GET", path=f"{ENDPOINT_BASE}/user/fields")
 
     def edit(self, user_id: str, **kwargs) -> None:
         """Edits user metadata.
 
         :param user_id: id of the user.
         :param kwargs: dictionary where keys are values from ``editable_fields`` method, and values to set.
         """
-
         for k, v in kwargs.items():
             self._session.ocs(method="PUT", path=f"{ENDPOINT}/{user_id}", params={"key": k, "value": v})
 
     def add_to_group(self, user_id: str, group_id: str) -> None:
         """Adds user to the group.
 
         :param user_id: ID of the user.
         :param group_id: the destination group to which add user to.
         """
-
         self._session.ocs(method="POST", path=f"{ENDPOINT}/{user_id}/groups", params={"groupid": group_id})
 
     def remove_from_group(self, user_id: str, group_id: str) -> None:
         """Removes user from the group.
 
         :param user_id: ID of the user.
         :param group_id: group from which remove user.
         """
-
         self._session.ocs(method="DELETE", path=f"{ENDPOINT}/{user_id}/groups", params={"groupid": group_id})
 
     def promote_to_subadmin(self, user_id: str, group_id: str) -> None:
         """Makes user admin of the group.
 
         :param user_id: ID of the user.
         :param group_id: group where user should become administrator.
         """
-
         self._session.ocs(method="POST", path=f"{ENDPOINT}/{user_id}/subadmins", params={"groupid": group_id})
 
     def demote_from_subadmin(self, user_id: str, group_id: str) -> None:
         """Removes user from the admin role of the group.
 
         :param user_id: ID of the user.
         :param group_id: group where user should be removed from administrators.
         """
-
         self._session.ocs(method="DELETE", path=f"{ENDPOINT}/{user_id}/subadmins", params={"groupid": group_id})
```

### Comparing `nc_py_api-0.0.26/nc_py_api/users_groups.py` & `nc_py_api-0.0.27/nc_py_api/users_groups.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,48 +1,20 @@
-"""
-Nextcloud API for working with user groups.
-"""
+"""Nextcloud API for working with user groups."""
 
-from dataclasses import dataclass
 from typing import Optional
 
 from ._session import NcSessionBasic
 from .misc import kwargs_to_dict
+from .users_defs import GroupDetails
 
 ENDPOINT = "/ocs/v1.php/cloud/groups"
 
 
-@dataclass
-class GroupDetails:
-    """User Group information"""
-
-    group_id: str
-    """ID of the group"""
-    display_name: str
-    """Display name of the group"""
-    user_count: int
-    """Number of users in the group"""
-    disabled: bool
-    """Flag indicating is group disabled"""
-    can_add: bool
-    """Flag showing the caller has enough rights to add users to this group"""
-    can_remove: bool
-    """Flag showing the caller has enough rights to remove users from this group"""
-
-    def __init__(self, raw_group: dict):
-        self.group_id = raw_group["id"]
-        self.display_name = raw_group["displayname"]
-        self.user_count = raw_group["usercount"]
-        self.disabled = bool(raw_group["disabled"])
-        self.can_add = bool(raw_group["canAdd"])
-        self.can_remove = bool(raw_group["canRemove"])
-
-
 class UserGroupsAPI:
-    """The class provides an API for managing user groups on the Nextcloud server.
+    """Class providing an API for managing user groups on the Nextcloud server.
 
     .. note:: In NextcloudApp mode, only ``get_list`` and ``get_details`` methods are available.
     """
 
     def __init__(self, session: NcSessionBasic):
         self._session = session
 
@@ -51,72 +23,65 @@
     ) -> list[str]:
         """Returns a list of user groups IDs.
 
         :param mask: group ID mask to apply.
         :param limit: limits the number of results.
         :param offset: offset of results.
         """
-
         data = kwargs_to_dict(["search", "limit", "offset"], search=mask, limit=limit, offset=offset)
         response_data = self._session.ocs(method="GET", path=ENDPOINT, params=data)
         return response_data["groups"] if response_data else []
 
     def get_details(
         self, mask: Optional[str] = None, limit: Optional[int] = None, offset: Optional[int] = None
     ) -> list[GroupDetails]:
         """Returns a list of user groups with detailed information.
 
         :param mask: group ID mask to apply.
         :param limit: limits the number of results.
         :param offset: offset of results.
         """
-
         data = kwargs_to_dict(["search", "limit", "offset"], search=mask, limit=limit, offset=offset)
         response_data = self._session.ocs(method="GET", path=f"{ENDPOINT}/details", params=data)
         return [GroupDetails(i) for i in response_data["groups"]] if response_data else []
 
     def create(self, group_id: str, display_name: Optional[str] = None) -> None:
         """Creates the users group.
 
         :param group_id: the ID of group to be created.
         :param display_name: display name for a created group.
         """
-
         params = {"groupid": group_id}
         if display_name is not None:
             params["displayname"] = display_name
         self._session.ocs(method="POST", path=f"{ENDPOINT}", params=params)
 
     def edit(self, group_id: str, display_name: str) -> None:
         """Edits users group information.
 
         :param group_id: the ID of group to edit info.
         :param display_name: new group display name.
         """
-
         params = {"key": "displayname", "value": display_name}
         self._session.ocs(method="PUT", path=f"{ENDPOINT}/{group_id}", params=params)
 
     def delete(self, group_id: str) -> None:
         """Removes the users group.
 
         :param group_id: the ID of group to remove.
         """
-
         self._session.ocs(method="DELETE", path=f"{ENDPOINT}/{group_id}")
 
     def get_members(self, group_id: str) -> list[str]:
         """Returns a list of group users.
 
         :param group_id: Group ID to get the list of members.
         """
-
         response_data = self._session.ocs(method="GET", path=f"{ENDPOINT}/{group_id}")
         return response_data["users"] if response_data else {}
 
     def get_subadmins(self, group_id: str) -> list[str]:
         """Returns list of users who is subadmins of the group.
 
         :param group_id: group ID to get the list of subadmins.
         """
-
         return self._session.ocs(method="GET", path=f"{ENDPOINT}/{group_id}/subadmins")
```

