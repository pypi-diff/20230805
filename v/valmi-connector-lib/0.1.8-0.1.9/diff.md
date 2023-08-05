# Comparing `tmp/valmi_connector_lib-0.1.8.tar.gz` & `tmp/valmi_connector_lib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valmi_connector_lib-0.1.8.tar", last modified: Wed Apr 19 16:32:40 2023, max compression
+gzip compressed data, was "valmi_connector_lib-0.1.9.tar", last modified: Thu Apr 20 08:00:22 2023, max compression
```

## Comparing `valmi_connector_lib-0.1.8.tar` & `valmi_connector_lib-0.1.9.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.463301 valmi_connector_lib-0.1.8/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-19 16:32:40.463343 valmi_connector_lib-0.1.8/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.8/pyproject.toml
--rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-19 16:32:40.463564 valmi_connector_lib-0.1.8/setup.cfg
--rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-19 16:17:39.000000 valmi_connector_lib-0.1.8/setup.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.460399 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/
--rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/PKG-INFO
--rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/SOURCES.txt
--rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/dependency_links.txt
--rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/requires.txt
--rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-19 16:32:40.000000 valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/top_level.txt
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.460497 valmi_connector_lib-0.1.8/valmi_lib/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.8/valmi_lib/__init__.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.461655 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/destination_container_wrapper.py
--rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/engine.py
--rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
--rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_handler.py
--rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/read_handlers.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.461984 valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/
--rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/__init__.py
--rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/source_container_wrapper.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.462469 valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/
--rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)     8229 2023-04-19 16:29:23.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/valmi_destination.py
-drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-19 16:32:40.463114 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/
--rw-r--r--   0 raj        (501) staff       (20)      573 2023-04-17 12:17:20.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/__init__.py
--rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/valmi_event.py
--rw-r--r--   0 raj        (501) staff       (20)     4238 2023-04-19 16:17:21.000000 valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/valmi_protocol.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.546905 valmi_connector_lib-0.1.9/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-20 08:00:22.546954 valmi_connector_lib-0.1.9/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      501 2023-04-17 08:03:07.000000 valmi_connector_lib-0.1.9/pyproject.toml
+-rw-r--r--   0 raj        (501) staff       (20)      417 2023-04-20 08:00:22.547177 valmi_connector_lib-0.1.9/setup.cfg
+-rw-r--r--   0 raj        (501) staff       (20)      616 2023-04-20 08:00:10.000000 valmi_connector_lib-0.1.9/setup.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.544036 valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/
+-rw-r--r--   0 raj        (501) staff       (20)      244 2023-04-20 08:00:22.000000 valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/PKG-INFO
+-rw-r--r--   0 raj        (501) staff       (20)      873 2023-04-20 08:00:22.000000 valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 raj        (501) staff       (20)        1 2023-04-20 08:00:22.000000 valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 raj        (501) staff       (20)       57 2023-04-20 08:00:22.000000 valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/requires.txt
+-rw-r--r--   0 raj        (501) staff       (20)       10 2023-04-20 08:00:22.000000 valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/top_level.txt
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.544135 valmi_connector_lib-0.1.9/valmi_lib/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:13:32.000000 valmi_connector_lib-0.1.9/valmi_lib/__init__.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.545289 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 11:26:07.000000 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)     6010 2023-04-17 11:37:39.000000 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/destination_container_wrapper.py
+-rw-r--r--   0 raj        (501) staff       (20)     7156 2023-04-17 11:38:33.000000 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/engine.py
+-rw-r--r--   0 raj        (501) staff       (20)     5404 2023-04-17 11:38:11.000000 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py
+-rw-r--r--   0 raj        (501) staff       (20)     3557 2023-04-17 11:38:17.000000 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/proc_stdout_handler.py
+-rw-r--r--   0 raj        (501) staff       (20)     2449 2023-04-17 11:38:24.000000 valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/read_handlers.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.545601 valmi_connector_lib-0.1.9/valmi_lib/source_wrapper/
+-rw-r--r--   0 raj        (501) staff       (20)        0 2023-04-17 10:24:00.000000 valmi_connector_lib-0.1.9/valmi_lib/source_wrapper/__init__.py
+-rwxr-xr-x   0 raj        (501) staff       (20)    13616 2023-03-30 16:20:11.000000 valmi_connector_lib-0.1.9/valmi_lib/source_wrapper/source_container_wrapper.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.546045 valmi_connector_lib-0.1.9/valmi_lib/valmi_destination/
+-rw-r--r--   0 raj        (501) staff       (20)       80 2023-04-17 07:57:27.000000 valmi_connector_lib-0.1.9/valmi_lib/valmi_destination/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)     8229 2023-04-19 16:29:23.000000 valmi_connector_lib-0.1.9/valmi_lib/valmi_destination/valmi_destination.py
+drwxr-xr-x   0 raj        (501) staff       (20)        0 2023-04-20 08:00:22.546702 valmi_connector_lib-0.1.9/valmi_lib/valmi_protocol/
+-rw-r--r--   0 raj        (501) staff       (20)      573 2023-04-17 12:17:20.000000 valmi_connector_lib-0.1.9/valmi_lib/valmi_protocol/__init__.py
+-rw-r--r--   0 raj        (501) staff       (20)      138 2023-04-17 07:57:16.000000 valmi_connector_lib-0.1.9/valmi_lib/valmi_protocol/valmi_event.py
+-rw-r--r--   0 raj        (501) staff       (20)     4250 2023-04-20 07:58:56.000000 valmi_connector_lib-0.1.9/valmi_lib/valmi_protocol/valmi_protocol.py
```

### Comparing `valmi_connector_lib-0.1.8/setup.py` & `valmi_connector_lib-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 TEST_REQUIREMENTS = [
     "pytest~=6.2",
 ]
 
 setup(
     name="valmi_connector_lib",
-    version="0.1.8",
+    version="0.1.9",
     description="Connector library for valmi connectors.",
     long_description="Connector library for valmi connectors.",
     author="Rajashekar Varkala @ valmi.io",
     author_email="contact@valmi.io",
     packages=find_packages(),
     install_requires=MAIN_REQUIREMENTS,
     package_data={"": ["*.json", "*.yaml"]},
```

### Comparing `valmi_connector_lib-0.1.8/valmi_connector_lib.egg-info/SOURCES.txt` & `valmi_connector_lib-0.1.9/valmi_connector_lib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/destination_container_wrapper.py` & `valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/destination_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/engine.py` & `valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/engine.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py` & `valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/proc_stdout_event_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/proc_stdout_handler.py` & `valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/proc_stdout_handler.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/destination_wrapper/read_handlers.py` & `valmi_connector_lib-0.1.9/valmi_lib/destination_wrapper/read_handlers.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/source_wrapper/source_container_wrapper.py` & `valmi_connector_lib-0.1.9/valmi_lib/source_wrapper/source_container_wrapper.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/valmi_destination/valmi_destination.py` & `valmi_connector_lib-0.1.9/valmi_lib/valmi_destination/valmi_destination.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/__init__.py` & `valmi_connector_lib-0.1.9/valmi_lib/valmi_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `valmi_connector_lib-0.1.8/valmi_lib/valmi_protocol/valmi_protocol.py` & `valmi_connector_lib-0.1.9/valmi_lib/valmi_protocol/valmi_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     mirror = "mirror"
 
 
 class ValmiSink(BaseModel):
     class Config:
         extra = Extra.allow
 
-    supported_sync_modes: List[DestinationSyncMode] = Field(
+    supported_destination_sync_modes: List[DestinationSyncMode] = Field(
         ..., description="List of sync modes supported by this sink.", min_items=1
     )
 
     # SINK object -- Hubspot kind of destinations can populate this - Webhooks are empty
     name: str = Field(..., description="Sink's name.")
     json_schema: Optional[Dict[str, Any]] = Field(..., description="Sink schema using Json Schema specs.")
```

