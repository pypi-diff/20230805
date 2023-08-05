# Comparing `tmp/tplink_omada_client-1.3.0.tar.gz` & `tmp/tplink_omada_client-1.3.2.tar.gz`

## Comparing `tplink_omada_client-1.3.0.tar` & `tplink_omada_client-1.3.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.pylintrc
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/Dockerfile.dev
--rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/requirements.txt
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/requirements_test.txt
--rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/sample_client.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.devcontainer/devcontainer.json
--rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.github/workflows/python-package.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.vscode/launch.json
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/__init__.py
--rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/clients.py
--rw-r--r--   0        0        0     3149 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/definitions.py
--rw-r--r--   0        0        0    19177 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/devices.py
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/exceptions.py
--rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/omadaapiconnection.py
--rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/omadaclient.py
--rw-r--r--   0        0        0    16156 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/omadasiteclient.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/py.typed
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/__init__.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/__main__.py
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_block_client.py
--rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_client.py
--rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_clients.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_default.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_devices.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_gateway.py
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_known_clients.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch.py
--rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch_ports.py
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switches.py
--rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_target.py
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_targets.py
--rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_unblock_client.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/config.py
--rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/src/tplink_omada_client/cli/util.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/tests/conftest.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/LICENSE
--rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/README.md
--rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.pylintrc
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/Dockerfile.dev
+-rw-r--r--   0        0        0      284 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/requirements.txt
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/requirements_test.txt
+-rwxr-xr-x   0        0        0     3375 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/sample_client.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.devcontainer/devcontainer.json
+-rw-r--r--   0        0        0     1304 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.vscode/launch.json
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/__init__.py
+-rw-r--r--   0        0        0     7531 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/clients.py
+-rw-r--r--   0        0        0     3172 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/definitions.py
+-rw-r--r--   0        0        0    19199 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/devices.py
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/exceptions.py
+-rw-r--r--   0        0        0     7907 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/omadaapiconnection.py
+-rw-r--r--   0        0        0     2903 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/omadaclient.py
+-rw-r--r--   0        0        0    16156 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/omadasiteclient.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/py.typed
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/__init__.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/__main__.py
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_block_client.py
+-rw-r--r--   0        0        0     2234 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_client.py
+-rw-r--r--   0        0        0     1771 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_clients.py
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_default.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_devices.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_gateway.py
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_known_clients.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_switch.py
+-rw-r--r--   0        0        0     4467 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_switch_ports.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_switches.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_target.py
+-rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_targets.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_unblock_client.py
+-rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/config.py
+-rw-r--r--   0        0        0     2300 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/src/tplink_omada_client/cli/util.py
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/tests/conftest.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/LICENSE
+-rw-r--r--   0        0        0     2332 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/README.md
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2992 2020-02-02 00:00:00.000000 tplink_omada_client-1.3.2/PKG-INFO
```

### Comparing `tplink_omada_client-1.3.0/Dockerfile.dev` & `tplink_omada_client-1.3.2/Dockerfile.dev`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/sample_client.py` & `tplink_omada_client-1.3.2/sample_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/.devcontainer/devcontainer.json` & `tplink_omada_client-1.3.2/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/.github/workflows/python-package.yml` & `tplink_omada_client-1.3.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/.github/workflows/python-publish.yml` & `tplink_omada_client-1.3.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/.vscode/launch.json` & `tplink_omada_client-1.3.2/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/clients.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/clients.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/definitions.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/definitions.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,16 @@
 class LinkSpeed(IntEnum):
     """Known link speeds."""
 
     SPEED_AUTO = 0
     SPEED_10_MBPS = 1
     SPEED_100_MBPS = 2
     SPEED_1_GBPS = 3
-    SPEED_10_GBPS = 4
+    SPEED_2_5_GBPS = 4
+    SPEED_10_GBPS = 5
 
 
 class LinkDuplex(IntEnum):
     """Known link duplex modes"""
 
     AUTO = 0
     HALF = 1
```

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/devices.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/devices.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,23 +101,23 @@
 class OmadaListDevice(OmadaDevice):
     """An Omada Device (router, switch, eap) as represented in the device list"""
 
     @property
     def need_upgrade(self) -> bool:
         """True, if a firmware upgrade is available for the device."""
         if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
-            return self._data["needUpgrade"]
+            return self._data.get("needUpgrade", False)
         else:
             return False
 
     @property
     def fw_download(self) -> bool:
         """True, if a firmware upgrade is being downloaded."""
         if self._data["statusCategory"] == DeviceStatusCategory.CONNECTED:
-            return self._data["fwDownload"]
+            return self._data.get("fwDownload", False)
         else:
             return False
 
 
 class OmadaLink(OmadaApiData):
     """Up/Downlink connection from a switch/ap device."""
```

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/exceptions.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/omadaapiconnection.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/omadaapiconnection.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/omadaclient.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/omadaclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/omadasiteclient.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/omadasiteclient.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/__init__.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_block_client.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_block_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_client.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_clients.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_clients.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_default.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_default.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_devices.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_devices.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_gateway.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_gateway.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_known_clients.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_known_clients.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_switch.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switch_ports.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_switch_ports.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_switches.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_switches.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_target.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_target.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_targets.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_targets.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/command_unblock_client.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/command_unblock_client.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/config.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/config.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/src/tplink_omada_client/cli/util.py` & `tplink_omada_client-1.3.2/src/tplink_omada_client/cli/util.py`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/LICENSE` & `tplink_omada_client-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/README.md` & `tplink_omada_client-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `tplink_omada_client-1.3.0/pyproject.toml` & `tplink_omada_client-1.3.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "tplink_omada_client"
-version = "1.3.0"
+version = "1.3.2"
 authors = [
   { name="Mark Godwin", email="author@example.com" },
 ]
 description = "Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `tplink_omada_client-1.3.0/PKG-INFO` & `tplink_omada_client-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplink_omada_client
-Version: 1.3.0
+Version: 1.3.2
 Summary: Python wrapper for TP-Link Omada SDN Controller API (OC200/OC300/Software Controller)
 Project-URL: Homepage, https://github.com/MarkGodwin/tplink-omada-api
 Project-URL: Bug Tracker, https://github.com/MarkGodwin/tplink-omada-api/issues
 Author-email: Mark Godwin <author@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

