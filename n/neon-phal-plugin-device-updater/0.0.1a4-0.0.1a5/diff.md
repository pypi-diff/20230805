# Comparing `tmp/neon-phal-plugin-device-updater-0.0.1a4.tar.gz` & `tmp/neon-phal-plugin-device-updater-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a4.tar", last modified: Wed Aug  2 20:45:04 2023, max compression
+gzip compressed data, was "neon-phal-plugin-device-updater-0.0.1a5.tar", last modified: Sat Aug  5 01:32:00 2023, max compression
```

## Comparing `neon-phal-plugin-device-updater-0.0.1a4.tar` & `neon-phal-plugin-device-updater-0.0.1a5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/
--rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:45:04.148000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-02 20:45:04.000000 neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 20:45:04.152000 neon-phal-plugin-device-updater-0.0.1a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-02 20:45:00.000000 neon-phal-plugin-device-updater-0.0.1a4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1634 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater/
+-rw-r--r--   0 runner    (1001) docker     (123)    12876 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-05 01:32:00.000000 neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 01:32:00.315152 neon-phal-plugin-device-updater-0.0.1a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-08-05 01:31:56.000000 neon-phal-plugin-device-updater-0.0.1a5/setup.py
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a4/LICENSE.md` & `neon-phal-plugin-device-updater-0.0.1a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-phal-plugin-device-updater-0.0.1a4/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater/__init__.py` & `neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 # SOFTWARE,  EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 import hashlib
 import json
 import shutil
 import requests
 
+from datetime import datetime
 from typing import Optional, Tuple
 from os import remove
 from os.path import isfile, join, dirname
 from subprocess import Popen
 from ovos_bus_client.message import Message
 from ovos_utils.log import LOG
 from ovos_plugin_manager.phal import PHALPlugin
@@ -76,17 +77,18 @@
                 with open("/opt/neon/build_info.json") as f:
                     self._build_info = json.load(f)
             except Exception as e:
                 LOG.error(f"Failed to get build info: {e}")
                 self._build_info = dict()
         return self._build_info
 
-    def _check_initramfs_update_available(self):
+    def _check_initramfs_update_available(self) -> bool:
         """
         Check if there is a newer initramfs version available by comparing MD5
+        @return: True if a newer initramfs is available to download
         """
         if not self.initramfs_url:
             raise RuntimeError("No initramfs_url configured")
         md5_request = requests.get(f"{self.initramfs_url}.md5")
         if not md5_request.ok:
             LOG.warning("Unable to get md5; downloading latest initramfs")
             return self._get_initramfs_latest()
@@ -99,14 +101,15 @@
         LOG.info("initramfs update available")
         return True
 
     def _get_initramfs_latest(self) -> bool:
         """
         Get the latest initramfs image and check if it is different from the
         current installed initramfs
+        @return: True if the downloaded initramfs file is different from current
         """
         if not self.initramfs_url:
             raise RuntimeError("No initramfs_url configured")
         if isfile(self.initramfs_update_path):
             LOG.info("update already downloaded")
             with open(self.initramfs_update_path, 'rb') as f:
                 new_hash = hashlib.md5(f.read()).hexdigest()
@@ -121,39 +124,69 @@
         with open(self.initramfs_real_path, 'rb') as f:
             old_hash = hashlib.md5(f.read()).hexdigest()
         if new_hash == old_hash:
             LOG.debug("initramfs not changed")
             return False
         return True
 
+    @staticmethod
+    def check_version_is_newer(current: str, latest: str) -> bool:
+        """
+        Compare two image versions to check if an update is available
+        @param current: currently installed version string
+        @param latest: latest available version from remote
+        @return: True if latest is newer than current
+        """
+        try:
+            date_format = "%Y-%m-%d_%H_%M"
+            current_datetime = datetime.strptime(current, date_format)
+            latest_datetime = datetime.strptime(latest, date_format)
+            if latest_datetime > current_datetime:
+                return True
+            return False
+        except Exception as e:
+            LOG.exception(e)
+            # Parse failure, assume there's an update
+            return True
+
     def _check_squashfs_update_available(self) -> Optional[Tuple[str, str]]:
+        """
+        Check if a newer squashFS image is available and return the new version
+        and download link.
+        @return: new version and download link if available, else None
+        """
         # Get all available update files from the configured URL
         ext = '.squashfs'
         prefix = self.build_info.get("base_os", {}).get("name", "")
         links = scrape_page_for_links(self.squashfs_url)
         valid_links = [(name, uri) for name, uri in links.items()
                        if name.endswith(ext) and name.startswith(prefix)]
         valid_links.sort(key=lambda k: k[0], reverse=True)
         newest_version = valid_links[0][0]
         download_url = valid_links[0][1]
 
-        # Check if the latest version matches the installed version
+        # Parse time of latest and current OS Image
         installed_image_time = self.build_info.get("base_os", {}).get("time")
-        if installed_image_time and installed_image_time in newest_version:
-            LOG.info("Already updated")
-            return None
-        LOG.info(f"New squashFS: {newest_version}")
-        return newest_version, download_url
+        new_image_time = newest_version.split('_', 1)[1].rsplit('.', 1)[0]
+
+        # Compare latest version with current
+        if installed_image_time == new_image_time:
+            LOG.info(f"Already Updated ({new_image_time}")
+        elif self.check_version_is_newer(installed_image_time, new_image_time):
+            LOG.info(f"New squashFS: {newest_version}")
+            return newest_version, download_url
+        else:
+            LOG.info(f"Installed image ({installed_image_time}) is newer "
+                     f"than latest ({new_image_time})")
 
     def _get_squashfs_latest(self) -> Optional[str]:
         """
         Get the latest squashfs image if different from the installed version
-        @returns: path to downloaded update if present, else None
+        @return: path to downloaded update if present, else None
         """
-
         # Check for an available update
         update = self._check_squashfs_update_available()
         if not update:
             # Already updated
             return None
         newest_version, download_url = update
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a4/neon_phal_plugin_device_updater.egg-info/PKG-INFO` & `neon-phal-plugin-device-updater-0.0.1a5/neon_phal_plugin_device_updater.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-phal-plugin-device-updater
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Core Module Update Interface
 Home-page: https://github.com/NeonGeckoCom/neon-phal-plugin-device-updater
 Author: Neongecko
 Author-email: developers@neon.ai
 License: BSD-3
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

### Comparing `neon-phal-plugin-device-updater-0.0.1a4/setup.py` & `neon-phal-plugin-device-updater-0.0.1a5/setup.py`

 * *Files identical despite different names*

