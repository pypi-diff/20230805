# Comparing `tmp/openct-0.1.6.tar.gz` & `tmp/openct-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openct-0.1.6.tar", max compression
+gzip compressed data, was "openct-0.1.7.tar", max compression
```

## Comparing `openct-0.1.6.tar` & `openct-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    35149 2023-08-05 01:21:13.529826 openct-0.1.6/LICENSE
--rw-r--r--   0        0        0     1693 2023-08-05 01:21:13.529826 openct-0.1.6/README.md
--rw-r--r--   0        0        0      112 2023-08-05 01:21:28.061882 openct-0.1.6/openct/__init__.py
--rw-r--r--   0        0        0      649 2023-08-05 01:21:13.529826 openct-0.1.6/openct/__main__.py
--rw-r--r--   0        0        0       83 2023-08-05 01:21:13.529826 openct-0.1.6/openct/connections/__init__.py
--rw-r--r--   0        0        0     2723 2023-08-05 01:21:13.529826 openct-0.1.6/openct/connections/connections.py
--rw-r--r--   0        0        0       73 2023-08-05 01:21:13.529826 openct-0.1.6/openct/datastore/__init__.py
--rw-r--r--   0        0        0     1359 2023-08-05 01:21:13.529826 openct-0.1.6/openct/datastore/datastore.py
--rw-r--r--   0        0        0       65 2023-08-05 01:21:13.529826 openct-0.1.6/openct/devices/__init__.py
--rw-r--r--   0        0        0      743 2023-08-05 01:21:13.529826 openct-0.1.6/openct/devices/devices.py
--rw-r--r--   0        0        0      201 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/__init__.py
--rw-r--r--   0        0        0      888 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/__main__.py
--rw-r--r--   0        0        0     1440 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/config.py
--rw-r--r--   0        0        0      626 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/config_schema.py
--rw-r--r--   0        0        0     1696 2023-08-05 01:21:13.529826 openct-0.1.6/openct/setup/setup.py
--rw-r--r--   0        0        0      645 2023-08-05 01:21:28.057882 openct-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-08-05 18:16:21.398743 openct-0.1.7/LICENSE
+-rw-r--r--   0        0        0     1693 2023-08-05 18:16:21.398743 openct-0.1.7/README.md
+-rw-r--r--   0        0        0      112 2023-08-05 18:16:40.242814 openct-0.1.7/openct/__init__.py
+-rw-r--r--   0        0        0      649 2023-08-05 18:16:21.398743 openct-0.1.7/openct/__main__.py
+-rw-r--r--   0        0        0       83 2023-08-05 18:16:21.398743 openct-0.1.7/openct/connections/__init__.py
+-rw-r--r--   0        0        0     2723 2023-08-05 18:16:21.398743 openct-0.1.7/openct/connections/connections.py
+-rw-r--r--   0        0        0       73 2023-08-05 18:16:21.398743 openct-0.1.7/openct/datastore/__init__.py
+-rw-r--r--   0        0        0     1359 2023-08-05 18:16:21.398743 openct-0.1.7/openct/datastore/datastore.py
+-rw-r--r--   0        0        0       65 2023-08-05 18:16:21.398743 openct-0.1.7/openct/devices/__init__.py
+-rw-r--r--   0        0        0      743 2023-08-05 18:16:21.398743 openct-0.1.7/openct/devices/devices.py
+-rw-r--r--   0        0        0      201 2023-08-05 18:16:21.398743 openct-0.1.7/openct/setup/__init__.py
+-rw-r--r--   0        0        0     1052 2023-08-05 18:16:21.398743 openct-0.1.7/openct/setup/__main__.py
+-rw-r--r--   0        0        0     1844 2023-08-05 18:16:21.398743 openct-0.1.7/openct/setup/config.py
+-rw-r--r--   0        0        0      759 2023-08-05 18:16:21.398743 openct-0.1.7/openct/setup/config_schema.py
+-rw-r--r--   0        0        0     1696 2023-08-05 18:16:21.398743 openct-0.1.7/openct/setup/setup.py
+-rw-r--r--   0        0        0      645 2023-08-05 18:16:40.238813 openct-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2341 1970-01-01 00:00:00.000000 openct-0.1.7/PKG-INFO
```

### Comparing `openct-0.1.6/LICENSE` & `openct-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/README.md` & `openct-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/openct/__main__.py` & `openct-0.1.7/openct/__main__.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/openct/connections/connections.py` & `openct-0.1.7/openct/connections/connections.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/openct/datastore/datastore.py` & `openct-0.1.7/openct/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/openct/devices/devices.py` & `openct-0.1.7/openct/devices/devices.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/openct/setup/__main__.py` & `openct-0.1.7/openct/setup/__main__.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,16 +10,21 @@
 if os.path.exists(CONFIG_FILE):
     user_input = input(
         f"The config file '{CONFIG_FILE}' already exists. Do you want to overwrite it? (yes/no): "
     ).lower()
     if user_input not in {"yes", "y"}:
         print("Config file not overwritten. Exiting.")
         sys.exit()
+    os.rename(CONFIG_FILE, CONFIG_FILE + ".bak")
 
-mt_backup_config = {
+starting_config_values = {
+    "config_version": {
+        "version": "0.1.0",
+        "comments": "Inital config verion."
+    },
     "identity": {
         "username": "username",
         "key_file": "config/.ssh/id_rsa",
     },
     "dirs": {
         "backup_dir": "backups",
         "log_dir": "logs",
@@ -29,9 +34,9 @@
         "connection_timeout": 3,
         "backup_max_age": 60,
         "log_max_age": 30,
         "log_max_count": 10,
     },
 }
 
-with open(file="config.yml", mode="a", encoding="utf-8") as file:
-    yaml.dump(mt_backup_config, file, default_flow_style=False)
+with open(file="config.yml", mode="w", encoding="utf-8") as file:
+    yaml.dump(starting_config_values, file, default_flow_style=False)
```

### Comparing `openct-0.1.6/openct/setup/config.py` & `openct-0.1.7/openct/setup/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Config """
 
 import sys
 
 import yaml
 
-from .config_schema import Config, ConfigDirs, ConfigIdentity, ConfigSettings
+from .config_schema import Config, ConfigVersion, ConfigDirs, ConfigIdentity, ConfigSettings
 
 
 def load_config(config_file: str) -> Config:
     """Try loading config."""
     try:
         return load_config_from_file(config_file)
     except FileNotFoundError:
@@ -20,14 +20,25 @@
 
 
 def load_config_from_file(config_file: str) -> Config:
     """Load config from file."""
     with open(file=config_file, mode="r", encoding="utf-8") as conf_file:
         config_data = yaml.safe_load(conf_file)
 
+    if "config_version" in config_data:
+        config_version = ConfigVersion(
+            version=config_data["config_version"]["version"],
+            comments=config_data["config_version"]["comments"],
+        )
+    else:
+        config_version = ConfigVersion(
+            version="0.0.0",
+            comments="Pre-versioning configuration file.",
+        )
+
     identity = ConfigIdentity(
         username=config_data["identity"]["username"],
         key_file=config_data["identity"]["key_file"],
     )
 
     dirs = ConfigDirs(
         backup_dir=config_data["dirs"]["backup_dir"],
@@ -39,8 +50,8 @@
         datastore_type=config_data["settings"]["datastore_type"],
         connection_timeout=config_data["settings"]["connection_timeout"],
         backup_max_age=config_data["settings"]["backup_max_age"],
         log_max_age=config_data["settings"]["log_max_age"],
         log_max_count=config_data["settings"]["log_max_count"],
     )
 
-    return Config(identity=identity, dirs=dirs, settings=settings)
+    return Config(version=config_version, identity=identity, dirs=dirs, settings=settings)
```

### Comparing `openct-0.1.6/openct/setup/config_schema.py` & `openct-0.1.7/openct/setup/config_schema.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 """Config types schema."""
 
 from dataclasses import dataclass
 
 
 @dataclass
+class ConfigVersion:
+    """Config version dataclass."""
+
+    version: str
+    comments: str
+
+
+@dataclass
 class ConfigIdentity:
     """Config identity dataclass."""
 
     username: str
     key_file: str
 
 
@@ -31,10 +39,11 @@
     log_max_count: int
 
 
 @dataclass
 class Config:
     """Config dataclass."""
 
+    version: ConfigVersion
     identity: ConfigIdentity
     dirs: ConfigDirs
     settings: ConfigSettings
```

### Comparing `openct-0.1.6/openct/setup/setup.py` & `openct-0.1.7/openct/setup/setup.py`

 * *Files identical despite different names*

### Comparing `openct-0.1.6/pyproject.toml` & `openct-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openct"
-version = "0.1.6"
+version = "0.1.7"
 description = "Configuration backup and analysis tools for devices running pfSense and RouterOS"
 authors = ["Weehooey <info@weehooey.com>"]
 license = "GNU GPL v3.0"
 readme = "README.md"
 repository = "https://github.com/weehooey/openct"
 
 [tool.poetry.dependencies]
```

### Comparing `openct-0.1.6/PKG-INFO` & `openct-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openct
-Version: 0.1.6
+Version: 0.1.7
 Summary: Configuration backup and analysis tools for devices running pfSense and RouterOS
 Home-page: https://github.com/weehooey/openct
 License: GNU GPL v3.0
 Author: Weehooey
 Author-email: info@weehooey.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

