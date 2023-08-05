# Comparing `tmp/pih-mio-1.48025.tar.gz` & `tmp/pih-mio-1.48026.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-mio-1.48025.tar", last modified: Fri Aug  4 01:22:14 2023, max compression
+gzip compressed data, was "pih-mio-1.48026.tar", last modified: Fri Aug  4 02:07:45 2023, max compression
```

## Comparing `pih-mio-1.48025.tar` & `pih-mio-1.48026.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 01:22:13.718815 pih-mio-1.48025/
-drwxrwxrwx   0        0        0        0 2023-08-04 01:22:14.172213 pih-mio-1.48025/MobileHelperCore/
--rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48025/MobileHelperCore/__init__.py
--rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48025/MobileHelperCore/__main__.py
--rw-rw-rw-   0        0        0   165341 2023-08-04 01:21:02.000000 pih-mio-1.48025/MobileHelperCore/api.py
--rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48025/MobileHelperCore/service.py
--rw-rw-rw-   0        0        0     9431 2023-08-04 01:20:17.000000 pih-mio-1.48025/MobileHelperCore/service_api.py
--rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48025/MobileHelperCore/tools.py
--rw-rw-rw-   0        0        0      279 2023-08-04 01:22:14.406583 pih-mio-1.48025/PKG-INFO
--rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48025/pih-mio_setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 01:22:14.312835 pih-mio-1.48025/pih_mio.egg-info/
--rw-rw-rw-   0        0        0      279 2023-08-04 01:22:12.000000 pih-mio-1.48025/pih_mio.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 01:22:12.000000 pih-mio-1.48025/pih_mio.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 01:22:13.000000 pih-mio-1.48025/pih_mio.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 01:22:14.422207 pih-mio-1.48025/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-04 02:07:45.622200 pih-mio-1.48026/
+drwxrwxrwx   0        0        0        0 2023-08-04 02:07:45.904269 pih-mio-1.48026/MobileHelperCore/
+-rw-rw-rw-   0        0        0        0 2023-03-23 02:22:16.000000 pih-mio-1.48026/MobileHelperCore/__init__.py
+-rw-rw-rw-   0        0        0      158 2023-07-28 13:41:38.000000 pih-mio-1.48026/MobileHelperCore/__main__.py
+-rw-rw-rw-   0        0        0   165341 2023-08-04 02:06:57.000000 pih-mio-1.48026/MobileHelperCore/api.py
+-rw-rw-rw-   0        0        0      718 2023-07-28 13:36:37.000000 pih-mio-1.48026/MobileHelperCore/service.py
+-rw-rw-rw-   0        0        0     9540 2023-08-04 02:06:12.000000 pih-mio-1.48026/MobileHelperCore/service_api.py
+-rw-rw-rw-   0        0        0      986 2023-06-21 05:38:40.000000 pih-mio-1.48026/MobileHelperCore/tools.py
+-rw-rw-rw-   0        0        0      279 2023-08-04 02:07:46.107386 pih-mio-1.48026/PKG-INFO
+-rw-rw-rw-   0        0        0     1651 2023-08-03 07:25:38.000000 pih-mio-1.48026/pih-mio_setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 02:07:46.076139 pih-mio-1.48026/pih_mio.egg-info/
+-rw-rw-rw-   0        0        0      279 2023-08-04 02:07:44.000000 pih-mio-1.48026/pih_mio.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2023-08-04 02:07:45.000000 pih-mio-1.48026/pih_mio.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 02:07:44.000000 pih-mio-1.48026/pih_mio.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-08-04 02:07:44.000000 pih-mio-1.48026/pih_mio.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2023-08-04 02:07:45.000000 pih-mio-1.48026/pih_mio.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-04 02:07:45.000000 pih-mio-1.48026/pih_mio.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 02:07:46.107386 pih-mio-1.48026/setup.cfg
```

### Comparing `pih-mio-1.48025/MobileHelperCore/api.py` & `pih-mio-1.48026/MobileHelperCore/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from MobileHelperContent.content import MEDIA_CONTENT
 import requests
 from io import BytesIO
 
 class MIO:
 
     NAME: str = "mio"       
-    VERSION: str = "1.48025"  
+    VERSION: str = "1.48026"  
 
 class InternalInterrupt(Exception):
 
     @property
     def type(self) -> int:
         return self.args[0]
```

### Comparing `pih-mio-1.48025/MobileHelperCore/service.py` & `pih-mio-1.48026/MobileHelperCore/service.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48025/MobileHelperCore/service_api.py` & `pih-mio-1.48026/MobileHelperCore/service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,16 @@
         self.checker = checker
         self.service_role: SR = SR.MOBILE_HELPER
         self.allow_send_to_next_service_in_chain: dict[str, bool] = defaultdict(bool)
         MobileHelperService.INSTANCE = self  
            
     def start(self) -> bool:
         if MobileHelperService.INIT:
+            A.SE.add_arg("--as_developer",
+                    nargs="?", const=1, type=str, default=None)
             service_role_desctiption: self.ServiceRoleDescription | None = A.SRV_A.create_support_service_or_master_service_description(A.CT_SR.description(self.service_role))
             if not A.D_C.empty(service_role_desctiption):
                 with A.ER.detect_interruption("Выход"):
                     A.SRV_A.serve(service_role_desctiption, self.service_call_handler,
                                 MobileHelperService.service_starts_handler)
                 return True
         return False
```

### Comparing `pih-mio-1.48025/MobileHelperCore/tools.py` & `pih-mio-1.48026/MobileHelperCore/tools.py`

 * *Files identical despite different names*

### Comparing `pih-mio-1.48025/pih-mio_setup.py` & `pih-mio-1.48026/pih-mio_setup.py`

 * *Files identical despite different names*

