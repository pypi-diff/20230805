# Comparing `tmp/aioruckus-0.24.tar.gz` & `tmp/aioruckus-0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioruckus-0.24.tar", last modified: Thu May  4 07:13:57 2023, max compression
+gzip compressed data, was "aioruckus-0.30.tar", last modified: Wed Jun  7 10:04:13 2023, max compression
```

## Comparing `aioruckus-0.24.tar` & `aioruckus-0.30.tar`

### file list

```diff
@@ -1,21 +1,24 @@
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/
--rw-r--r--   0 tony      (1000) tony      (1000)      681 2023-04-22 10:29:47.000000 aioruckus-0.24/LICENSE
--rw-r--r--   0 tony      (1000) tony      (1000)     3760 2023-05-04 07:13:57.161026 aioruckus-0.24/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)     3281 2023-05-04 04:16:11.000000 aioruckus-0.24/README.md
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/aioruckus/
--rw-r--r--   0 tony      (1000) tony      (1000)      166 2023-04-23 12:21:01.000000 aioruckus-0.24/aioruckus/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)     6400 2023-04-24 13:31:05.000000 aioruckus-0.24/aioruckus/ajaxsession.py
--rw-r--r--   0 tony      (1000) tony      (1000)     1598 2023-05-04 04:08:16.000000 aioruckus-0.24/aioruckus/const.py
--rw-r--r--   0 tony      (1000) tony      (1000)      110 2023-04-22 10:29:47.000000 aioruckus-0.24/aioruckus/exceptions.py
--rw-r--r--   0 tony      (1000) tony      (1000)    21469 2023-05-04 04:11:53.000000 aioruckus-0.24/aioruckus/ruckusapi.py
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/aioruckus.egg-info/
--rw-r--r--   0 tony      (1000) tony      (1000)     3760 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/PKG-INFO
--rw-r--r--   0 tony      (1000) tony      (1000)      349 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/SOURCES.txt
--rw-r--r--   0 tony      (1000) tony      (1000)        1 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/dependency_links.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       16 2023-05-04 07:13:57.000000 aioruckus-0.24/aioruckus.egg-info/top_level.txt
--rw-r--r--   0 tony      (1000) tony      (1000)       96 2023-05-04 07:12:00.000000 aioruckus-0.24/pyproject.toml
--rw-r--r--   0 tony      (1000) tony      (1000)      568 2023-05-04 07:13:57.161026 aioruckus-0.24/setup.cfg
-drwxr-xr-x   0 tony      (1000) tony      (1000)        0 2023-05-04 07:13:57.161026 aioruckus-0.24/tests/
--rw-r--r--   0 tony      (1000) tony      (1000)      373 2023-04-22 10:29:47.000000 aioruckus-0.24/tests/__init__.py
--rw-r--r--   0 tony      (1000) tony      (1000)      755 2023-04-22 10:29:47.000000 aioruckus-0.24/tests/test_connection.py
--rw-r--r--   0 tony      (1000) tony      (1000)     1399 2023-04-22 10:29:47.000000 aioruckus-0.24/tests/test_data.py
+drwxrwxrwx   0        0        0        0 2023-06-07 10:04:13.848106 aioruckus-0.30/
+-rw-rw-rw-   0        0        0      694 2023-06-07 09:46:52.000000 aioruckus-0.30/LICENSE
+-rw-rw-rw-   0        0        0     4558 2023-06-07 10:04:13.848106 aioruckus-0.30/PKG-INFO
+-rw-rw-rw-   0        0        0     4065 2023-06-07 09:46:52.000000 aioruckus-0.30/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 10:04:13.839104 aioruckus-0.30/aioruckus/
+-rw-rw-rw-   0        0        0      254 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/__init__.py
+-rw-rw-rw-   0        0        0     1160 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/abcsession.py
+-rw-rw-rw-   0        0        0     6966 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/ajaxsession.py
+-rw-rw-rw-   0        0        0     1906 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/backupsession.py
+-rw-rw-rw-   0        0        0     1627 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/const.py
+-rw-rw-rw-   0        0        0      116 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/exceptions.py
+-rw-rw-rw-   0        0        0    19446 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/ruckusajaxapi.py
+-rw-rw-rw-   0        0        0     5107 2023-06-07 09:46:52.000000 aioruckus-0.30/aioruckus/ruckusapi.py
+drwxrwxrwx   0        0        0        0 2023-06-07 10:04:13.844103 aioruckus-0.30/aioruckus.egg-info/
+-rw-rw-rw-   0        0        0     4558 2023-06-07 10:04:13.000000 aioruckus-0.30/aioruckus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      427 2023-06-07 10:04:13.000000 aioruckus-0.30/aioruckus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 10:04:13.000000 aioruckus-0.30/aioruckus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-07 10:04:13.000000 aioruckus-0.30/aioruckus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       99 2023-06-07 09:46:52.000000 aioruckus-0.30/pyproject.toml
+-rw-rw-rw-   0        0        0      592 2023-06-07 10:04:13.849103 aioruckus-0.30/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-07 10:04:13.847107 aioruckus-0.30/tests/
+-rw-rw-rw-   0        0        0      385 2023-06-07 10:00:23.000000 aioruckus-0.30/tests/__init__.py
+-rw-rw-rw-   0        0        0      781 2023-06-07 09:46:52.000000 aioruckus-0.30/tests/test_connection.py
+-rw-rw-rw-   0        0        0     1458 2023-06-07 09:46:52.000000 aioruckus-0.30/tests/test_data.py
```

### Comparing `aioruckus-0.24/LICENSE` & `aioruckus-0.30/LICENSE`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-BSD Zero Clause License
-
-Copyright Contributors to the aioruckus project.
-
-Permission to use, copy, modify, and/or distribute this software for any
-purpose with or without fee is hereby granted.
-
-THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
-REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
-AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
-INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
-LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
-OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
+BSD Zero Clause License
+
+Copyright Contributors to the aioruckus project.
+
+Permission to use, copy, modify, and/or distribute this software for any
+purpose with or without fee is hereby granted.
+
+THE SOFTWARE IS PROVIDED "AS IS" AND THE AUTHOR DISCLAIMS ALL WARRANTIES WITH
+REGARD TO THIS SOFTWARE INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY
+AND FITNESS. IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY SPECIAL, DIRECT,
+INDIRECT, OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES WHATSOEVER RESULTING FROM
+LOSS OF USE, DATA OR PROFITS, WHETHER IN AN ACTION OF CONTRACT, NEGLIGENCE OR
+OTHER TORTIOUS ACTION, ARISING OUT OF OR IN CONNECTION WITH THE USE OR
 PERFORMANCE OF THIS SOFTWARE.
```

### Comparing `aioruckus-0.24/PKG-INFO` & `aioruckus-0.30/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,105 @@
-Metadata-Version: 2.1
-Name: aioruckus
-Version: 0.24
-Summary: Python API to interact with Ruckus Unleashed and ZoneDirector devices.
-Home-page: https://github.com/ms264556/aioruckus
-Author: ms264556
-Author-email: bsd0@patterni.city
-License: BSD0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# aioruckus
-
-A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.
-
-Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
-
-## How to install
-
-```bash
-pip install aioruckus
-```
-
-## Usage
-
-Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
-
-```python
-from aioruckus import AjaxSession, SystemStat
-import asyncio
-
-async def test_aioruckus():
-    
-    async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
-        ruckus = session.api
-
-        wlans = await ruckus.get_wlans()
-        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
-        aps = await ruckus.get_aps()
-        ap_groups = await ruckus.get_ap_groups()
-        mesh = await ruckus.get_mesh_info()
-        default_system_info = await ruckus.get_system_info()
-        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
-        active_clients = await ruckus.get_active_clients()
-        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
-        blocked = await ruckus.get_blocked_client_macs()
-        syslog = await ruckus.get_syslog()
-
-        await ruckus.do_block_client("60:ab:de:ad:be:ef")
-        await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
-
-        await ruckus.do_disable_wlan("my ssid")
-        await ruckus.do_enable_wlan("my ssid")
-
-        await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
-
-        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
-        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
-
-        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
-        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
-
-        await ruckus.do_delete_wlan_group("Copy of Default")
-
-        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
-        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
-
-        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
-        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
-        await ruckus.do_delete_wlan("my newer sid")
-
-        await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
-        await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
-        
-        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
-
-asyncio.run(test_aioruckus())
-```
-
-### Other Python APIs for Ruckus Unleashed
-
-This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
-
-There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
-Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
+Metadata-Version: 2.1
+Name: aioruckus
+Version: 0.30
+Summary: Python API to interact with Ruckus Unleashed and ZoneDirector devices.
+Home-page: https://github.com/ms264556/aioruckus
+Author: ms264556
+Author-email: bsd0@patterni.city
+License: BSD0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aioruckus
+
+A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.  
+Configuration information can also be queried from Ruckus Unleashed and ZoneDirector backup files.
+
+Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
+
+## How to install
+
+```bash
+pip install aioruckus
+```
+
+## Usage
+
+Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
+
+```python
+from aioruckus import AjaxSession, BackupSession, SystemStat
+import asyncio
+
+async def test_aioruckus():
+    
+    with BackupSession.create("<ruckus backup filename>") as session:
+        ruckus = session.api
+
+        aps = await ruckus.get_aps()
+        ap_groups = await ruckus.get_ap_groups()
+        wlans = await ruckus.get_wlans()
+        wlan_groups = await ruckus.get_wlan_groups()
+        blocked = await ruckus.get_blocked_client_macs()
+        mesh = await ruckus.get_mesh_info()
+        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
+
+    async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
+        ruckus = session.api
+
+        aps = await ruckus.get_aps()
+        ap_groups = await ruckus.get_ap_groups()
+        wlans = await ruckus.get_wlans()
+        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
+        blocked = await ruckus.get_blocked_client_macs()
+        mesh = await ruckus.get_mesh_info()
+        default_system_info = await ruckus.get_system_info()
+        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
+
+        ap_group_stats = await ruckus.get_ap_group_stats()
+        wlan_group_stats = await ruckus.get_wlan_group_stats()
+
+        active_clients = await ruckus.get_active_clients()
+        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
+        syslog = await ruckus.get_syslog()
+
+        await ruckus.do_block_client("60:ab:de:ad:be:ef")
+        await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
+
+        await ruckus.do_disable_wlan("my ssid")
+        await ruckus.do_enable_wlan("my ssid")
+
+        await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
+
+        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
+        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
+
+        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
+        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
+
+        await ruckus.do_delete_wlan_group("Copy of Default")
+
+        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
+        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
+
+        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
+        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
+        await ruckus.do_delete_wlan("my newer sid")
+
+        await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
+        await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
+        
+        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
+
+asyncio.run(test_aioruckus())
+```
+
+### Other Python APIs for Ruckus Unleashed
+
+This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
+
+There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
+Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
```

### Comparing `aioruckus-0.24/README.md` & `aioruckus-0.30/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,74 +1,90 @@
-# aioruckus
-
-A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.
-
-Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
-
-## How to install
-
-```bash
-pip install aioruckus
-```
-
-## Usage
-
-Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
-
-```python
-from aioruckus import AjaxSession, SystemStat
-import asyncio
-
-async def test_aioruckus():
-    
-    async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
-        ruckus = session.api
-
-        wlans = await ruckus.get_wlans()
-        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
-        aps = await ruckus.get_aps()
-        ap_groups = await ruckus.get_ap_groups()
-        mesh = await ruckus.get_mesh_info()
-        default_system_info = await ruckus.get_system_info()
-        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
-        active_clients = await ruckus.get_active_clients()
-        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
-        blocked = await ruckus.get_blocked_client_macs()
-        syslog = await ruckus.get_syslog()
-
-        await ruckus.do_block_client("60:ab:de:ad:be:ef")
-        await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
-
-        await ruckus.do_disable_wlan("my ssid")
-        await ruckus.do_enable_wlan("my ssid")
-
-        await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
-
-        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
-        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
-
-        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
-        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
-
-        await ruckus.do_delete_wlan_group("Copy of Default")
-
-        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
-        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
-
-        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
-        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
-        await ruckus.do_delete_wlan("my newer sid")
-
-        await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
-        await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
-        
-        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
-
-asyncio.run(test_aioruckus())
-```
-
-### Other Python APIs for Ruckus Unleashed
-
-This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
-
-There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
-Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
+# aioruckus
+
+A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.  
+Configuration information can also be queried from Ruckus Unleashed and ZoneDirector backup files.
+
+Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
+
+## How to install
+
+```bash
+pip install aioruckus
+```
+
+## Usage
+
+Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
+
+```python
+from aioruckus import AjaxSession, BackupSession, SystemStat
+import asyncio
+
+async def test_aioruckus():
+    
+    with BackupSession.create("<ruckus backup filename>") as session:
+        ruckus = session.api
+
+        aps = await ruckus.get_aps()
+        ap_groups = await ruckus.get_ap_groups()
+        wlans = await ruckus.get_wlans()
+        wlan_groups = await ruckus.get_wlan_groups()
+        blocked = await ruckus.get_blocked_client_macs()
+        mesh = await ruckus.get_mesh_info()
+        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
+
+    async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
+        ruckus = session.api
+
+        aps = await ruckus.get_aps()
+        ap_groups = await ruckus.get_ap_groups()
+        wlans = await ruckus.get_wlans()
+        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
+        blocked = await ruckus.get_blocked_client_macs()
+        mesh = await ruckus.get_mesh_info()
+        default_system_info = await ruckus.get_system_info()
+        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
+
+        ap_group_stats = await ruckus.get_ap_group_stats()
+        wlan_group_stats = await ruckus.get_wlan_group_stats()
+
+        active_clients = await ruckus.get_active_clients()
+        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
+        syslog = await ruckus.get_syslog()
+
+        await ruckus.do_block_client("60:ab:de:ad:be:ef")
+        await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
+
+        await ruckus.do_disable_wlan("my ssid")
+        await ruckus.do_enable_wlan("my ssid")
+
+        await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
+
+        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
+        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
+
+        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
+        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
+
+        await ruckus.do_delete_wlan_group("Copy of Default")
+
+        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
+        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
+
+        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
+        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
+        await ruckus.do_delete_wlan("my newer sid")
+
+        await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
+        await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
+        
+        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
+
+asyncio.run(test_aioruckus())
+```
+
+### Other Python APIs for Ruckus Unleashed
+
+This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
+
+There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
+Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
```

### Comparing `aioruckus-0.24/aioruckus/ajaxsession.py` & `aioruckus-0.30/aioruckus/ajaxsession.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,145 +1,153 @@
-import asyncio
-import ssl
-from typing import Any
-
-import aiohttp
-import xmltodict
-from .exceptions import AuthenticationError
-
-from .const import (
-    AJAX_POST_NORESULT_ERROR,
-    AJAX_POST_REDIRECTED_ERROR,
-    CONNECT_ERROR_EOF,
-    CONNECT_ERROR_TEMPORARY,
-    CONNECT_ERROR_TIMEOUT,
-    LOGIN_ERROR_LOGIN_INCORRECT,
-)
-
-
-class AjaxSession:
-    """Connect to Ruckus Unleashed or ZoneDirector via HTTPS AJAX"""
-
-    def __init__(
-        self,
-        websession: aiohttp.ClientSession,
-        host: str,
-        username: str,
-        password: str,
-        auto_cleanup_websession=False,
-    ) -> None:
-        self.websession = websession
-        self.host = host
-        self.username = username
-        self.password = password
-        self.__auto_cleanup_websession = auto_cleanup_websession
-
-        self.__api = None
-
-        self.__login_url = None
-        self.base_url = None
-        self.cmdstat_url = None
-        self.conf_url = None
-
-    async def __aenter__(self) -> "AjaxSession":
-        await self.login()
-        return self
-
-    async def __aexit__(self, *exc: Any) -> None:
-        await self.close()
-
-    async def login(self) -> None:
-        """Create HTTPS AJAX session."""
-        # locate the admin pages: /admin/* for Unleashed and ZD 9.x, /admin10/* for ZD 10.x
-        try:
-            async with self.websession.head(f"https://{self.host}", timeout=3, allow_redirects=False) as head:
-                self.__login_url = head.headers["Location"]
-                self.base_url, login_page = self.__login_url.rsplit("/", 1)
-                if login_page == "index.html" or login_page == "wizard.jsp": # Unleashed Rebuilding or Setup Wizard
-                    raise ConnectionRefusedError(CONNECT_ERROR_TEMPORARY)
-                self.cmdstat_url = self.base_url + "/_cmdstat.jsp"
-                self.conf_url = self.base_url + "/_conf.jsp"
-        except aiohttp.client_exceptions.ClientConnectorError as cerr:
-            raise ConnectionError(CONNECT_ERROR_EOF) from cerr
-        except asyncio.exceptions.TimeoutError as terr:
-            raise ConnectionError(CONNECT_ERROR_TIMEOUT) from terr
-
-        # login and collect CSRF token
-        async with self.websession.head(
-            self.__login_url,
-            params={
-                "username": self.username,
-                "password": self.password,
-                "ok": "Log In",
-            },
-            timeout=3,
-            allow_redirects=False,
-        ) as head:
-            if head.status == 200:  # if username/password were valid we'd be redirected to the main admin page
-                raise AuthenticationError(LOGIN_ERROR_LOGIN_INCORRECT)
-            if "HTTP_X_CSRF_TOKEN" in head.headers:  # modern ZD and Unleashed return CSRF token in header
-                self.websession.headers["X-CSRF-Token"] = head.headers["HTTP_X_CSRF_TOKEN"]
-            else:  # older ZD and Unleashed require you to scrape the CSRF token from a page's javascript
-                async with self.websession.get(
-                    self.base_url + "/_csrfTokenVar.jsp",
-                    timeout=3,
-                    allow_redirects=False,
-                ) as response:
-                    if response.status == 200:
-                        csrf_token = (xmltodict.parse(await response.text())["script"].split("=").pop()[2:12])
-                        self.websession.headers["X-CSRF-Token"] = csrf_token
-                    elif response.status == 500:  # even older ZD don't use CSRF tokens at all
-                        pass
-                    else:  # token page is a redirect, maybe temporary Unleashed Rebuilding placeholder page is showing
-                        raise ConnectionRefusedError(CONNECT_ERROR_TEMPORARY)
-            return self
-
-    async def close(self) -> None:
-        """Logout of ZoneDirector/Unleashed and close websessiom"""
-        if self.websession:
-            async with self.websession.head(
-                self.__login_url,
-                params={"logout": "1"},
-                timeout=3,
-                allow_redirects=False,
-            ):
-                pass
-            if self.__auto_cleanup_websession:
-                await self.websession.close()
-
-    async def request(self, cmd: str, data: str, timeout: int | None = None, retrying: bool = False) -> str:
-        """Request data"""
-        async with self.websession.post(cmd, data=data, headers={"Content-Type": "text/xml"}, timeout=timeout, allow_redirects=False) as response:
-            if response.status == 302:  # if the session is dead then we're redirected to the login page
-                if retrying:  # we tried logging in again, but the redirect still happens - maybe password changed?
-                    raise PermissionError(AJAX_POST_REDIRECTED_ERROR)
-                await self.login()  # try logging in again, then retry post
-                return await self.request(cmd, data, timeout, retrying=True)
-            result_text = await response.text()
-            if not result_text or result_text == "\n":  # if the ajax request payload wasn't understood then we get an empty page back
-                raise RuntimeError(AJAX_POST_NORESULT_ERROR)
-            return result_text
-
-    @property
-    def api(self):
-        """Return a RuckusApi instance."""
-        if not self.__api:
-            # pylint: disable=import-outside-toplevel
-            from .ruckusapi import RuckusApi
-            self.__api = RuckusApi(self)
-        return self.__api
-
-    @classmethod
-    def async_create(cls, host: str, username: str, password: str) -> "AjaxSession":
-        """Create a default ClientSession & use this to create an AjaxSession instance"""
-        # create ssl context so we ignore cert errors
-        context = ssl.create_default_context()
-        context.set_ciphers("DEFAULT")
-        context.check_hostname = False
-        context.verify_mode = ssl.CERT_NONE
-        # make ClientSession using ssl the above SSLContext, allowing cookies on IP address URLs, and with short keepalive for compatibility with old Unleashed versions
-        websession = aiohttp.ClientSession(
-            timeout=aiohttp.ClientTimeout(total=10),
-            cookie_jar=aiohttp.CookieJar(unsafe=True),
-            connector=aiohttp.TCPConnector(keepalive_timeout=5, ssl_context=context),
-        )
-        return AjaxSession(websession, host, username, password, auto_cleanup_websession=True)
+import asyncio
+import ssl
+from typing import Any, TYPE_CHECKING
+
+if TYPE_CHECKING:
+    from .ruckusajaxapi import RuckusAjaxApi
+
+import aiohttp
+import xmltodict
+
+from .abcsession import AbcSession, ConfigItem
+from .exceptions import AuthenticationError
+
+from .const import (
+    AJAX_POST_NORESULT_ERROR,
+    AJAX_POST_REDIRECTED_ERROR,
+    CONNECT_ERROR_EOF,
+    CONNECT_ERROR_TEMPORARY,
+    CONNECT_ERROR_TIMEOUT,
+    LOGIN_ERROR_LOGIN_INCORRECT,
+)
+
+
+class AjaxSession(AbcSession):
+    """Connect to Ruckus Unleashed or ZoneDirector via HTTPS AJAX"""
+
+    def __init__(
+        self,
+        websession: aiohttp.ClientSession,
+        host: str,
+        username: str,
+        password: str,
+        auto_cleanup_websession=False,
+    ) -> None:
+        super().__init__()
+
+        self.websession = websession
+        self.host = host
+        self.username = username
+        self.password = password
+        self.__auto_cleanup_websession = auto_cleanup_websession
+
+        self.__login_url = None
+        self.base_url = None
+        self.cmdstat_url = None
+        self.conf_url = None
+
+    async def __aenter__(self) -> "AjaxSession":
+        await self.login()
+        return self
+
+    async def __aexit__(self, *exc: Any) -> None:
+        await self.close()
+
+    async def login(self) -> None:
+        """Create HTTPS AJAX session."""
+        # locate the admin pages: /admin/* for Unleashed and ZD 9.x, /admin10/* for ZD 10.x
+        try:
+            async with self.websession.head(f"https://{self.host}", timeout=3, allow_redirects=False) as head:
+                self.__login_url = head.headers["Location"]
+                self.base_url, login_page = self.__login_url.rsplit("/", 1)
+                if login_page == "index.html" or login_page == "wizard.jsp": # Unleashed Rebuilding or Setup Wizard
+                    raise ConnectionRefusedError(CONNECT_ERROR_TEMPORARY)
+                self.cmdstat_url = self.base_url + "/_cmdstat.jsp"
+                self.conf_url = self.base_url + "/_conf.jsp"
+        except aiohttp.client_exceptions.ClientConnectorError as cerr:
+            raise ConnectionError(CONNECT_ERROR_EOF) from cerr
+        except asyncio.exceptions.TimeoutError as terr:
+            raise ConnectionError(CONNECT_ERROR_TIMEOUT) from terr
+
+        # login and collect CSRF token
+        async with self.websession.head(
+            self.__login_url,
+            params={
+                "username": self.username,
+                "password": self.password,
+                "ok": "Log In",
+            },
+            timeout=3,
+            allow_redirects=False,
+        ) as head:
+            if head.status == 200:  # if username/password were valid we'd be redirected to the main admin page
+                raise AuthenticationError(LOGIN_ERROR_LOGIN_INCORRECT)
+            if "HTTP_X_CSRF_TOKEN" in head.headers:  # modern ZD and Unleashed return CSRF token in header
+                self.websession.headers["X-CSRF-Token"] = head.headers["HTTP_X_CSRF_TOKEN"]
+            else:  # older ZD and Unleashed require you to scrape the CSRF token from a page's javascript
+                async with self.websession.get(
+                    self.base_url + "/_csrfTokenVar.jsp",
+                    timeout=3,
+                    allow_redirects=False,
+                ) as response:
+                    if response.status == 200:
+                        csrf_token = (xmltodict.parse(await response.text())["script"].split("=").pop()[2:12])
+                        self.websession.headers["X-CSRF-Token"] = csrf_token
+                    elif response.status == 500:  # even older ZD don't use CSRF tokens at all
+                        pass
+                    else:  # token page is a redirect, maybe temporary Unleashed Rebuilding placeholder page is showing
+                        raise ConnectionRefusedError(CONNECT_ERROR_TEMPORARY)
+            return self
+
+    async def close(self) -> None:
+        """Logout of ZoneDirector/Unleashed and close websessiom"""
+        if self.websession:
+            async with self.websession.head(
+                self.__login_url,
+                params={"logout": "1"},
+                timeout=3,
+                allow_redirects=False,
+            ):
+                pass
+            if self.__auto_cleanup_websession:
+                await self.websession.close()
+
+    async def request(self, cmd: str, data: str, timeout: int | None = None, retrying: bool = False) -> str:
+        """Request data"""
+        async with self.websession.post(cmd, data=data, headers={"Content-Type": "text/xml"}, timeout=timeout, allow_redirects=False) as response:
+            if response.status == 302:  # if the session is dead then we're redirected to the login page
+                if retrying:  # we tried logging in again, but the redirect still happens - maybe password changed?
+                    raise PermissionError(AJAX_POST_REDIRECTED_ERROR)
+                await self.login()  # try logging in again, then retry post
+                return await self.request(cmd, data, timeout, retrying=True)
+            result_text = await response.text()
+            if not result_text or result_text == "\n":  # if the ajax request payload wasn't understood then we get an empty page back
+                raise RuntimeError(AJAX_POST_NORESULT_ERROR)
+            return result_text
+
+    @property
+    def api(self) -> "RuckusAjaxApi":
+        """Return a RuckusApi instance."""
+        if not self._api:
+            # pylint: disable=import-outside-toplevel
+            from .ruckusajaxapi import RuckusAjaxApi
+            self._api = RuckusAjaxApi(self)
+        return self._api
+
+    @classmethod
+    def async_create(cls, host: str, username: str, password: str) -> "AjaxSession":
+        """Create a default ClientSession & use this to create an AjaxSession instance"""
+        # create ssl context so we ignore cert errors
+        context = ssl.create_default_context()
+        context.set_ciphers("DEFAULT")
+        context.check_hostname = False
+        context.verify_mode = ssl.CERT_NONE
+        # make ClientSession using ssl the above SSLContext, allowing cookies on IP address URLs, and with short keepalive for compatibility with old Unleashed versions
+        websession = aiohttp.ClientSession(
+            timeout=aiohttp.ClientTimeout(total=10),
+            cookie_jar=aiohttp.CookieJar(unsafe=True),
+            connector=aiohttp.TCPConnector(keepalive_timeout=5, ssl_context=context),
+        )
+        return AjaxSession(websession, host, username, password, auto_cleanup_websession=True)
+
+    async def get_conf_str(self, item: ConfigItem, timeout: int | None = None) -> str:
+        return await self.request(self.conf_url, f"<ajax-request action='getconf' DECRYPT_X='true' updater='{item.value}.0.5' comp='{item.value}'/>", timeout)
```

### Comparing `aioruckus-0.24/aioruckus/const.py` & `aioruckus-0.30/aioruckus/const.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,39 +1,38 @@
-"""Constants used in aioruckus."""
-from enum import Enum
-
-# Error strings
-CONNECT_ERROR_EOF = "Could not establish connection to host"
-CONNECT_ERROR_TIMEOUT = "Timed out while waiting for client"
-CONNECT_ERROR_TEMPORARY = "Temporarily unable to handle the request"
-AJAX_POST_REDIRECTED_ERROR = "Insufficient permission to run this command"
-AJAX_POST_NORESULT_ERROR = "The command was not understood"
-LOGIN_ERROR_LOGIN_INCORRECT = "Login incorrect"
-VALUE_ERROR_INVALID_MAC = "Invalid MAC"
-VALUE_ERROR_INVALID_WLAN = "Invalid WLAN"
-VALUE_ERROR_INVALID_PASSPHRASE_LEN = "Passphrase can only contain between 8 and 63 characters or 64 HEX characters, space is not allowed"
-VALUE_ERROR_INVALID_PASSPHRASE_JS = "Embedding html or javascript code, e.g. < />, is not allowed"
-VALUE_ERROR_INVALID_PASSPHRASE_MISSING = "WPA2 and Mixed WPA2/3 WLANs require a passphrase"
-VALUE_ERROR_INVALID_SAEPASSPHRASE_MISSING = "WPA3 and Mixed WPA2/3 WLANs require an SAE passphrase"
-VALUE_ERROR_WLAN_SSID_SETTING_REQUIRES_NAME = "You must also provide a name if you wish to override the passphrase"
-
-class SystemStat(Enum):
-    ALL = ""
-    ADMIN = "<admin/>"
-    CLUSTER = "<cluster/>"
-    DEFAULT = "<identity/><sysinfo/><port/><unleashed-network/>"
-    IDENTITY = "<identity/>"
-    MESH_POLICY = "<mesh-policy/>"
-    MGMT_IP = "<mgmt-ip/>"
-    MGMT_VLAN = "<mgmt-vlan/>"
-    PORT = "<port/>"
-    SYSINFO = "<sysinfo/>"
-    TIME = "<time/>"
-    UNLEASHED_NETWORK = "<unleashed-network/>"
-
-
-class WlanEncryption(Enum):
-    NONE = "none"
-    OWE = "owe"
-    WPA2 = "wpa2"
-    WPA23_MIXED = "wpa23-mixed"
-    WPA3 = "wpa3"
+"""Constants used in aioruckus."""
+from enum import Enum
+
+# Error strings
+CONNECT_ERROR_EOF = "Could not establish connection to host"
+CONNECT_ERROR_TIMEOUT = "Timed out while waiting for client"
+CONNECT_ERROR_TEMPORARY = "Temporarily unable to handle the request"
+AJAX_POST_REDIRECTED_ERROR = "Insufficient permission to run this command"
+AJAX_POST_NORESULT_ERROR = "The command was not understood"
+LOGIN_ERROR_LOGIN_INCORRECT = "Login incorrect"
+VALUE_ERROR_INVALID_MAC = "Invalid MAC"
+VALUE_ERROR_INVALID_WLAN = "Invalid WLAN"
+VALUE_ERROR_INVALID_PASSPHRASE_LEN = "Passphrase can only contain between 8 and 63 characters or 64 HEX characters, space is not allowed"
+VALUE_ERROR_INVALID_PASSPHRASE_JS = "Embedding html or javascript code, e.g. < />, is not allowed"
+VALUE_ERROR_INVALID_PASSPHRASE_MISSING = "WPA2 and Mixed WPA2/3 WLANs require a passphrase"
+VALUE_ERROR_INVALID_SAEPASSPHRASE_MISSING = "WPA3 and Mixed WPA2/3 WLANs require an SAE passphrase"
+VALUE_ERROR_WLAN_SSID_SETTING_REQUIRES_NAME = "You must also provide a name if you wish to override the passphrase"
+
+class SystemStat(Enum):
+    ALL = []
+    ADMIN = ["admin"]
+    CLUSTER = ["cluster"]
+    DEFAULT = ["identity", "sysinfo", "port", "unleashed-network"]
+    IDENTITY = ["identity"]
+    MESH_POLICY = ["mesh-policy"]
+    MGMT_IP = ["mgmt-ip"]
+    MGMT_VLAN = ["mgmt-vlan"]
+    PORT = ["port"]
+    SYSINFO = ["sysinfo"]
+    TIME = ["time"]
+    UNLEASHED_NETWORK = ["unleashed-network"]
+
+class WlanEncryption(Enum):
+    NONE = "none"
+    OWE = "owe"
+    WPA2 = "wpa2"
+    WPA23_MIXED = "wpa23-mixed"
+    WPA3 = "wpa3"
```

### Comparing `aioruckus-0.24/aioruckus/ruckusapi.py` & `aioruckus-0.30/aioruckus/ruckusajaxapi.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,363 +1,328 @@
-from re import IGNORECASE, match
-from typing import Any, List, Literal
-from warnings import warn
-import xml.etree.ElementTree as ET
-import xml.sax.saxutils as saxutils
-
-import xmltodict
-
-from .const import (
-    VALUE_ERROR_INVALID_MAC,
-    VALUE_ERROR_INVALID_PASSPHRASE_LEN,
-    VALUE_ERROR_INVALID_PASSPHRASE_JS,
-    VALUE_ERROR_INVALID_PASSPHRASE_MISSING,
-    VALUE_ERROR_INVALID_SAEPASSPHRASE_MISSING,
-    VALUE_ERROR_INVALID_WLAN,
-    VALUE_ERROR_WLAN_SSID_SETTING_REQUIRES_NAME
-)
-from .const import SystemStat as SystemStat
-from .const import WlanEncryption as WlanEncryption
-from .ajaxsession import AjaxSession
-
-
-class RuckusApi:
-
-    def __init__(self, auth: AjaxSession):
-        self.auth = auth
-
-    async def get_mesh_info(self) -> dict:
-        meshinfo = await self.conf("<ajax-request action='getconf' comp='mesh-list' DECRYPT_X='true'/>")
-        return meshinfo["mesh-list"]["mesh"]
-
-    async def get_zerotouch_mesh_ap_serials(self) -> dict:
-        return await self.conf("<ajax-request action='getconf' updater='ztmeshSerial-list.0.5' comp='ztmeshSerial-list'/>", ["ztmeshSerial"])
-
-    async def get_blocked_client_macs(self) -> List:
-        blockedinfo = await self.conf("<ajax-request action='getconf' comp='acl-list' updater='page.0.5' />", ["accept", "deny", "acl"])
-        denylist = blockedinfo[0]["deny"] if "deny" in blockedinfo[0] else None
-        return [] if not denylist else [d for d in denylist if d]
-
-    async def get_system_info(self, *sections: SystemStat) -> dict:
-        section = ''.join(s.value for s in sections) if sections else SystemStat.DEFAULT.value
-        sysinfo = await self.cmdstat(f"<ajax-request action='getstat' comp='system'>{section}</ajax-request>")
-        return sysinfo["response"] if "response" in sysinfo else sysinfo["system"]
-
-    async def get_active_clients(self, interval_stats: bool = False) -> List:
-        if interval_stats:
-            endtime = await self._get_timestamp_at_controller()
-            starttime = endtime - 86400
-            clientrequest = f"<client INTERVAL-STATS='yes' INTERVAL-START='{starttime}' INTERVAL-STOP='{endtime}' />"
-        else:
-            clientrequest = "<client LEVEL='1' />"
-        return await self.cmdstat(f"<ajax-request action='getstat' comp='stamgr' enable-gzip='0'>{clientrequest}</ajax-request>", ["client"])
-
-    async def get_inactive_clients(self) -> List:
-        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0'><clientlist period='0' /></ajax-request>", ["client"])
-
-    async def get_aps(self) -> List:
-        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0'><ap LEVEL='1' /></ajax-request>", ["ap"])
-
-    async def get_ap_groups(self) -> List:
-        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0'><apgroup /></ajax-request>", ["group", "radio", "ap"])
-
-    async def get_vaps(self) -> List:
-        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0' caller='SCI'><vap INTERVAL-STATS='no' LEVEL='1' /></ajax-request>", ["vap"])
-
-    async def get_wlans(self) -> List:
-        return await self.conf("<ajax-request action='getconf' DECRYPT_X='true' updater='wlansvc-list.0.5' comp='wlansvc-list'/>", ["wlansvc"])
-
-    async def get_wlan_groups(self) -> List:
-        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0' caller='SCI'><wlangroup /></ajax-request>", ["wlangroup", "wlan"])
-
-    async def get_syslog(self) -> str:
-        syslog = await self.cmdstat("<ajax-request action='docmd' xcmd='get-syslog' updater='system.0.5' comp='system'><xcmd cmd='get-syslog' type='sys'/></ajax-request>")
-        return syslog["xmsg"]["res"]
-
-    async def do_block_client(self, mac: str) -> None:
-        mac = self._normalize_mac(mac)
-        await self.cmdstat(f"<ajax-request action='docmd' xcmd='block' checkAbility='10' comp='stamgr'><xcmd check-ability='10' tag='client' acl-id='1' client='{mac}' cmd='block'><client client='{mac}' acl-id='1' hostname=''></client></xcmd></ajax-request>")
-
-    async def do_unblock_client(self, mac: str) -> None:
-        mac = self._normalize_mac(mac)
-        blocked = await self.get_blocked_client_macs()
-        remaining = ''.join((f"<deny mac='{deny['mac']}' type='single'/>" for deny in blocked if deny["mac"] != mac))
-        await self._do_conf(f"<ajax-request action='updobj' comp='acl-list' updater='blocked-clients'><acl id='1' name='System' description='System' default-mode='allow' EDITABLE='false'>{remaining}</acl></ajax-request>")
-
-    async def do_disable_wlan(self, name: str, disable_wlan: bool = True) -> None:
-        wlan = await self._find_wlan_by_name(name)
-        if wlan:
-            await self._do_conf(f"<ajax-request action='updobj' updater='wlansvc-list.0.5' comp='wlansvc-list'><wlansvc id='{wlan['id']}' name='{wlan['name']}' enable-type='{1 if disable_wlan else 0}' IS_PARTIAL='true'/></ajax-request>")
-
-    async def do_enable_wlan(self, name: str) -> None:
-        await self.do_disable_wlan(name, False)
-
-    async def do_set_wlan_password(self, name: str, passphrase: str, sae_passphrase: str = None) -> None:
-        sae_passphrase = sae_passphrase or passphrase
-        await self.do_edit_wlan(name, {"wpa": {"passphrase": passphrase, "sae-passphrase": sae_passphrase}}, True)
-
-    async def do_add_wlan(self, name: str, encryption: WlanEncryption = WlanEncryption.WPA2, passphrase: str = None, sae_passphrase: str = None, ssid_override: str = None, ignore_unknown_attributes: bool = False) -> None:
-        patch = {"name": name, "ssid": ssid_override or name, "encryption": encryption.value}
-        if passphrase is not None or sae_passphrase is not None:
-            patch_wpa = {}
-            patch["wpa"] = patch_wpa
-            if passphrase is not None:
-                patch_wpa["passphrase"] = passphrase
-            if sae_passphrase is not None:
-                patch_wpa["sae-passphrase"] = sae_passphrase
-        await self.do_clone_wlan(patch)
-
-    async def do_clone_wlan(self, template: dict, new_name: str = None, new_ssid: str = None) -> None:
-        wlansvc = await self._get_default_wlan_template()
-        self._normalize_encryption(wlansvc, template)
-        self._patch_template(wlansvc, template, True)
-        if new_name is not None or new_ssid is not None:
-            if new_name is None:
-                raise ValueError(VALUE_ERROR_WLAN_SSID_SETTING_REQUIRES_NAME)
-            self._patch_template(wlansvc, {"name": new_name, "ssid": new_ssid or new_name })
-        await self._add_wlan_template(wlansvc)
-
-    async def do_edit_wlan(self, name: str, patch: dict, ignore_unknown_attributes: bool = False) -> None:
-        wlansvc = await self._get_wlan_template(name)
-        if wlansvc:
-            self._normalize_encryption(wlansvc, patch)
-            self._patch_template(wlansvc, patch, ignore_unknown_attributes)
-            await self._update_wlan_template(wlansvc)
-
-    async def do_delete_wlan(self, name: str) -> bool:
-        wlan = await self._find_wlan_by_name(name)
-        if wlan is None:
-            return False
-        else:
-            await self._do_conf(f"<ajax-request action='delobj' updater='wlansvc-list.0.5' comp='wlansvc-list'><wlansvc id='{wlan['id']}'/></ajax-request>", timeout=20)
-            return True
-
-    async def do_add_wlan_group(self, name: str, description: str = "", wlans: List = None) -> None:
-        wlangroup = ET.Element("wlangroup", {"name": name, "description": description or ""})
-        if wlans is not None:
-            wlan_map = {wlan["name"]:wlan["id"] for wlan in await self.get_wlans()}
-            for wlansvc in wlans:
-                wlan_name = None
-                if isinstance(wlansvc, str):
-                    if wlansvc in wlan_map:
-                        wlan_name = wlansvc
-                elif isinstance(wlansvc, dict):
-                    if "name" in wlansvc and wlansvc["name"] in wlan_map:
-                        wlan_name = wlansvc["name"]
-                if wlan_name is None:
-                    raise ValueError(VALUE_ERROR_INVALID_WLAN)
-                ET.SubElement(wlangroup, "wlansvc", {"id": wlan_map[wlan_name]})
-        await self._do_conf(f"<ajax-request action='addobj' comp='wlangroup-list' updater='wgroup'>{ET.tostring(wlangroup).decode('utf-8')}</ajax-request>")
-
-    async def do_clone_wlan_group(self, template: dict, name: str, description: str = None) -> None:
-        wlangroup = ET.Element("wlangroup", {"name": name, "description": description or (template["description"] if "description" in template else "")})
-        if "wlan" in template:
-            wlan_map = {wlan["name"]:wlan["id"] for wlan in await self.get_wlans()}
-            for wlansvc in template["wlan"]:
-                ET.SubElement(wlangroup, "wlansvc", {"id": wlan_map[wlansvc["name"]]})
-        await self._do_conf(f"<ajax-request action='addobj' comp='wlangroup-list' updater='wgroup'>{ET.tostring(wlangroup).decode('utf-8')}</ajax-request>")
-
-    async def do_delete_wlan_group(self, name: str) -> bool:
-        wlang = await self._find_wlan_group_by_name(name)
-        if wlang is None:
-            return False
-        else:
-            await self._do_conf(f"<ajax-request action='delobj' updater='wlangroup-list.0.5' comp='wlangroup-list'><wlangroup id='{wlang['id']}'/></ajax-request>")
-            return True
-
-    async def do_hide_ap_leds(self, mac: str, leds_off: bool = True) -> None:
-        mac = self._normalize_mac(mac)
-        ap = await self._find_ap_by_mac(mac)
-        if ap:
-            await self._do_conf(f"<ajax-request action='updobj' updater='ap-list.0.5' comp='ap-list'><ap id='{ap['id']}' IS_PARTIAL='true' led-off='{str(leds_off).lower()}' /></ajax-request>")
-
-    async def do_show_ap_leds(self, mac: str) -> None:
-        await self.do_hide_ap_leds(mac, False)
-
-    async def do_restart_ap(self, mac: str) -> None:
-        mac = self._normalize_mac(mac)
-        return await self._cmdstat_noparse(f"<ajax-request action='docmd' xcmd='reset' checkAbility='2' updater='stamgr.0.5' comp='stamgr'><xcmd cmd='reset' ap='{mac}' tag='ap' checkAbility='2'/></ajax-request>")
-
-    async def _get_default_wlan_template(self) -> ET.Element:
-        xml = await self._conf_noparse("<ajax-request action='getconf' DECRYPT_X='true' updater='wlansvc-standard-template.0.5' comp='wlansvc-standard-template'/>")
-        root = ET.fromstring(xml)
-        wlansvc = root.find(".//wlansvc")
-        if wlansvc is not None:
-            return wlansvc
-        else:
-            return self._get_default_cli_wlan_template()
-
-    @staticmethod
-    def _get_default_cli_wlan_template() -> ET.Element:
-        wlansvc = ET.Element("wlansvc", {"name": "default-standard-wlan", "ssid": "", "authentication": "open", "encryption": "none",
-                                         "is-guest": "false", "max-clients-per-radio": "100", "do-802-11d": "disabled", "sta-info-extraction": "1",
-                                         "force-dhcp": "0", "force-dhcp-timeout": "10", "usage": "user", "policy-id": "", "policy6-id": "",
-                                         "precedence-id": "1", "devicepolicy-id": "", "role-based-access-ctrl": "false", "acl-id": "1", "local-bridge": "1",
-                                         "client-isolation": "disabled", "ci-whitelist-id": "0", "bgscan": "1", "idle-timeout": "1", "max-idle-timeout": "300",
-                                         "dis-dgaf": "0", "authstats": "0", "https-redirection": "disabled"})
-        ET.SubElement(wlansvc, "qos", {"uplink-preset": "DISABLE", "downlink-preset": "DISABLE"})
-        ET.SubElement(wlansvc, "queue-priority", {"voice": "0", "video": "2", "data": "4", "background": "6"})
-        ET.SubElement(wlansvc, "wlan-schedule", {"value": "0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0: 0x0:0x0:0x0:0x0:0x0:0x0"})
-        return wlansvc
-
-    async def _get_wlan_template(self, name: str) -> ET.Element | None:
-        xml = await self._conf_noparse("<ajax-request action='getconf' DECRYPT_X='true' updater='wlansvc-list.0.5' comp='wlansvc-list'/>")
-        root = ET.fromstring(xml)
-        wlansvc = root.find(f".//wlansvc[@name='{saxutils.escape(name)}']")
-        return wlansvc
-
-    def _normalize_encryption(self, wlansvc: ET.Element, patch: dict):
-        patch_wpa = patch["wpa"] if "wpa" in patch else None
-        if patch_wpa is not None:
-            if "passphrase" in patch_wpa:
-                self._validate_passphrase(patch_wpa["passphrase"])
-            if "sae-passphrase" in patch_wpa:
-                self._validate_passphrase(patch_wpa["sae-passphrase"])
-
-        encryption = wlansvc.get("encryption")
-        if "encryption" in patch and patch["encryption"] != encryption:
-            new_encryption = patch["encryption"]
-            wlansvc.set("encryption", new_encryption)
-
-            wpa = wlansvc.find("wpa")
-            new_wpa = {"cipher": "aes", "dynamic-psk": "disabled"}
-
-            if new_encryption == WlanEncryption.WPA2.value or new_encryption == WlanEncryption.WPA23_MIXED.value:
-                passphrase = wpa.get("passphrase") if wpa is not None else None
-                if (patch_wpa is None or "passphrase" not in patch_wpa) and passphrase is None:
-                    raise ValueError(VALUE_ERROR_INVALID_PASSPHRASE_MISSING)
-                new_wpa["passphrase"] = passphrase or "<passphrase>"
-            if new_encryption == WlanEncryption.WPA3.value or new_encryption == WlanEncryption.WPA23_MIXED.value:
-                sae_passphrase = wpa.get("sae-passphrase") if wpa is not None else None
-                if (patch_wpa is None or "sae-passphrase" not in patch_wpa) and sae_passphrase is None:
-                    raise ValueError(VALUE_ERROR_INVALID_SAEPASSPHRASE_MISSING)
-                new_wpa["sae-passphrase"] = sae_passphrase or "<passphrase>"
-
-            if wpa is not None:
-                wlansvc.remove(wpa)
-            if new_encryption != WlanEncryption.NONE.value:
-                wpa = ET.SubElement(wlansvc, "wpa", new_wpa)
-
-    def _patch_template(self, element: ET.Element, patch: dict, ignore_unknown_attributes: bool = False, current_path: str = ""):
-        visited_children = set()
-        for child in element:
-            if child.tag in patch and isinstance(patch[child.tag], dict):
-                self._patch_template(child, patch[child.tag], ignore_unknown_attributes, f"{current_path}/{child.tag}")
-                visited_children.add(child.tag)
-        for name, value in patch.items():
-            if name in visited_children:
-                pass
-            else:
-                current_value = element.get(name)
-                if isinstance(value, List):
-                    raise ValueError(f"Applying lists is unsupported: {current_path}/{name}")
-                elif current_value is None:
-                    if not ignore_unknown_attributes:
-                        raise ValueError(f"Unknown attribute: {current_path}/{name}")
-                else:
-                    new_value = self._normalize_conf_value(current_value, value)
-                    element.set(name, new_value)
-                    x_name = f"x-{name}"
-                    if x_name not in patch and x_name in element.attrib:
-                        element.set(x_name, new_value)
-
-    async def _update_wlan_template(self, wlansvc: ET.Element):
-        xml_bytes = ET.tostring(wlansvc)
-        await self._do_conf(f"<ajax-request action='updobj' updater='wlan' comp='wlansvc-list'>{xml_bytes.decode('utf-8')}</ajax-request>", timeout=20)
-
-    async def _add_wlan_template(self, wlansvc: ET.Element):
-        xml_bytes = ET.tostring(wlansvc)
-        await self._do_conf(f"<ajax-request action='addobj' updater='wlansvc-list' comp='wlansvc-list'>{xml_bytes.decode('utf-8')}</ajax-request>", timeout=20)
-
-    async def _find_ap_by_mac(self, mac: str) -> dict:
-        return next((ap for ap in await self.get_aps() if ap["mac"] == mac), None)
-
-    async def _find_wlan_by_name(self, name: str) -> dict:
-        return next((wlan for wlan in await self.get_wlans() if wlan["name"] == name), None)
-
-    async def _find_wlan_group_by_name(self, name: str) -> dict:
-        return next((wlang for wlang in await self.get_wlan_groups() if wlang["name"] == name), None)
-
-    async def _get_timestamp_at_controller(self) -> int:
-        timeinfo = await self.cmdstat("<ajax-request action='getstat' updater='system.0.5' comp='system'><time/></ajax-request>")
-        return int(timeinfo["response"]["time"]["time"])
-
-    async def _cmdstat_noparse(self, data: str, timeout: int | None = None) -> str:
-        return await self.auth.request(self.auth.cmdstat_url, data, timeout)
-
-    async def cmdstat(self, data: str, collection_elements: List[str] = None, timeout: int | None = None) -> dict | List:
-        result_text = await self._cmdstat_noparse(data, timeout)
-        return self._ajaxunwrap(result_text, collection_elements)
-
-    async def _conf_noparse(self, data: str, timeout: int | None = None) -> str:
-        return await self.auth.request(self.auth.conf_url, data, timeout)
-
-    async def conf(self, data: str, collection_elements: List[str] = None, timeout: int | None = None) -> dict | List:
-        result_text = await self._conf_noparse(data, timeout)
-        return self._ajaxunwrap(result_text, collection_elements)
-
-    async def _do_conf(self, data: str, collection_elements: List[str] = None, timeout: int | None = None) -> None:
-        result = await self.conf(data, collection_elements, timeout)
-        if "xmsg" in result:
-            raise ValueError(result["xmsg"]["lmsg"])
-
-    @staticmethod
-    def _ajaxunwrap(xml: str, collection_elements: List[str] = None) -> dict | List:
-        # convert xml and unwrap collection
-        force_list = None if not collection_elements else {ce: True for ce in collection_elements}
-        result = xmltodict.parse(xml, encoding="utf-8", attr_prefix='', postprocessor=RuckusApi._process_ruckus_ajax_xml, force_list=force_list)
-        collection_list = [] if not collection_elements else [f"{ce}-list" for ce in collection_elements] + collection_elements
-        for key in ["ajax-response", "response", "apstamgr-stat"] + collection_list:
-            if result and key and key in result:
-                result = result[key]
-        return result or []
-
-    @staticmethod
-    def _process_ruckus_ajax_xml(path, key, value):
-        # passphrases are obfuscated and stored with an x- prefix; decrypt these
-        if key.startswith("x-"):
-            return key[2:], ''.join(chr(ord(letter) - 1) for letter in value) if value else value
-        elif key == "apstamgr-stat" and not value:  # return an empty array rather than None, for ease of use
-            return key, []
-        # client status is numeric code for active, and name for inactive. Show name for everything
-        elif key == "status" and value and value.isnumeric() and path and len(path) > 0 and path[-1][0] == "client":
-            description = "Authorized" if value == "1" else "Authenticating" if value == "2" else "PSK Expired" if value == "3" else "Authorized(Deny)" if value == "4" else "Authorized(Permit)" if value == "5" else "Unauthorized"
-            return key, description
-        else:
-            return key, value
-
-    @staticmethod
-    def _normalize_mac(mac: str) -> str:
-        if mac and match(r"(?:[0-9a-f]{2}[:-]){5}[0-9a-f]{2}", string=mac, flags=IGNORECASE):
-            return mac.replace('-', ':').lower()
-        raise ValueError(VALUE_ERROR_INVALID_MAC)
-
-    @staticmethod
-    def _validate_passphrase(passphrase: str) -> str:
-        if passphrase and match(r".*<.*>.*", string=passphrase):
-            raise ValueError(VALUE_ERROR_INVALID_PASSPHRASE_JS)
-        if passphrase and match(r"(^[!-~]([ -~]){6,61}[!-~]$)|(^([0-9a-fA-F]){64}$)", string=passphrase):
-            return passphrase
-        raise ValueError(VALUE_ERROR_INVALID_PASSPHRASE_LEN)
-
-    @staticmethod
-    def _normalize_conf_value(current_value: str, new_value: Any) -> str:
-        current_value_lowered = current_value.lower()
-        if current_value_lowered in ("enable", "disable", "enabled", "disabled", "true", "false", "yes", "no", "1", "0"):
-            if isinstance(new_value, str):
-                new_value_lowered = new_value.lower()
-                new_value = True if new_value_lowered in ("enable", "enabled", "true", "yes", "1") else False if new_value_lowered in ("disable", "disabled", "false", "no", "0") else new_value
-            elif isinstance(new_value, (int, float)) and not isinstance(new_value, bool):
-                new_value = True if new_value == 1 else False if new_value == 0 else new_value
-
-            if isinstance(new_value, bool):
-                if current_value_lowered in ("enable", "disable"):
-                    new_value = "ENABLE" if new_value else "DISABLE"
-                elif current_value_lowered in ("enabled", "disabled"):
-                    new_value = "enabled" if new_value else "disabled"
-                elif current_value_lowered in ("yes", "no"):
-                    new_value = "yes" if new_value else "no"
-                elif current_value_lowered in ("true", "false"):
-                    new_value = "true" if new_value else "false"
-                elif current_value_lowered in ("1", "0"):
-                    new_value = "1" if new_value else "0"
-        return new_value
+from re import IGNORECASE, match
+from typing import Any, List
+import xml.etree.ElementTree as ET
+import xml.sax.saxutils as saxutils
+
+from .abcsession import ConfigItem
+
+from .const import (
+    VALUE_ERROR_INVALID_MAC,
+    VALUE_ERROR_INVALID_PASSPHRASE_LEN,
+    VALUE_ERROR_INVALID_PASSPHRASE_JS,
+    VALUE_ERROR_INVALID_PASSPHRASE_MISSING,
+    VALUE_ERROR_INVALID_SAEPASSPHRASE_MISSING,
+    VALUE_ERROR_INVALID_WLAN,
+    VALUE_ERROR_WLAN_SSID_SETTING_REQUIRES_NAME
+)
+from .const import SystemStat as SystemStat
+from .const import WlanEncryption as WlanEncryption
+from .ajaxsession import AjaxSession
+from .ruckusapi import RuckusApi
+
+class RuckusAjaxApi(RuckusApi):
+
+    def __init__(self, session: AjaxSession):
+        self.session = session
+
+    async def get_system_info(self, *sections: SystemStat) -> dict:
+        sections = [s for section_list in sections for s in section_list.value] if sections else SystemStat.DEFAULT.value
+        section = ''.join(f"<{s}/>" for s in sections)
+        sysinfo = await self.cmdstat(f"<ajax-request action='getstat' comp='system'>{section}</ajax-request>")
+        return sysinfo["response"] if "response" in sysinfo else sysinfo["system"]
+
+    async def get_active_clients(self, interval_stats: bool = False) -> List:
+        if interval_stats:
+            endtime = await self._get_timestamp_at_controller()
+            starttime = endtime - 86400
+            clientrequest = f"<client INTERVAL-STATS='yes' INTERVAL-START='{starttime}' INTERVAL-STOP='{endtime}' />"
+        else:
+            clientrequest = "<client LEVEL='1' />"
+        return await self.cmdstat(f"<ajax-request action='getstat' comp='stamgr' enable-gzip='0'>{clientrequest}</ajax-request>", ["client"])
+
+    async def get_inactive_clients(self) -> List:
+        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0'><clientlist period='0' /></ajax-request>", ["client"])
+
+    async def get_ap_stats(self) -> List:
+        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0'><ap LEVEL='1' /></ajax-request>", ["ap"])
+
+    async def get_ap_group_stats(self) -> List:
+        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0'><apgroup /></ajax-request>", ["group", "radio", "ap"])
+
+    async def get_vap_stats(self) -> List:
+        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0' caller='SCI'><vap INTERVAL-STATS='no' LEVEL='1' /></ajax-request>", ["vap"])
+
+    async def get_wlan_group_stats(self) -> List:
+        return await self.cmdstat("<ajax-request action='getstat' comp='stamgr' enable-gzip='0' caller='SCI'><wlangroup /></ajax-request>", ["wlangroup", "wlan"])
+
+    async def get_syslog(self) -> str:
+        syslog = await self.cmdstat("<ajax-request action='docmd' xcmd='get-syslog' updater='system.0.5' comp='system'><xcmd cmd='get-syslog' type='sys'/></ajax-request>")
+        return syslog["xmsg"]["res"]
+
+    async def do_block_client(self, mac: str) -> None:
+        mac = self._normalize_mac(mac)
+        await self.cmdstat(f"<ajax-request action='docmd' xcmd='block' checkAbility='10' comp='stamgr'><xcmd check-ability='10' tag='client' acl-id='1' client='{mac}' cmd='block'><client client='{mac}' acl-id='1' hostname=''></client></xcmd></ajax-request>")
+
+    async def do_unblock_client(self, mac: str) -> None:
+        mac = self._normalize_mac(mac)
+        blocked = await self.get_blocked_client_macs()
+        remaining = ''.join((f"<deny mac='{deny['mac']}' type='single'/>" for deny in blocked if deny["mac"] != mac))
+        await self._do_conf(f"<ajax-request action='updobj' comp='acl-list' updater='blocked-clients'><acl id='1' name='System' description='System' default-mode='allow' EDITABLE='false'>{remaining}</acl></ajax-request>")
+
+    async def do_disable_wlan(self, name: str, disable_wlan: bool = True) -> None:
+        wlan = await self._find_wlan_by_name(name)
+        if wlan:
+            await self._do_conf(f"<ajax-request action='updobj' updater='wlansvc-list.0.5' comp='wlansvc-list'><wlansvc id='{wlan['id']}' name='{wlan['name']}' enable-type='{1 if disable_wlan else 0}' IS_PARTIAL='true'/></ajax-request>")
+
+    async def do_enable_wlan(self, name: str) -> None:
+        await self.do_disable_wlan(name, False)
+
+    async def do_set_wlan_password(self, name: str, passphrase: str, sae_passphrase: str = None) -> None:
+        sae_passphrase = sae_passphrase or passphrase
+        await self.do_edit_wlan(name, {"wpa": {"passphrase": passphrase, "sae-passphrase": sae_passphrase}}, True)
+
+    async def do_add_wlan(self, name: str, encryption: WlanEncryption = WlanEncryption.WPA2, passphrase: str = None, sae_passphrase: str = None, ssid_override: str = None, ignore_unknown_attributes: bool = False) -> None:
+        patch = {"name": name, "ssid": ssid_override or name, "encryption": encryption.value}
+        if passphrase is not None or sae_passphrase is not None:
+            patch_wpa = {}
+            patch["wpa"] = patch_wpa
+            if passphrase is not None:
+                patch_wpa["passphrase"] = passphrase
+            if sae_passphrase is not None:
+                patch_wpa["sae-passphrase"] = sae_passphrase
+        await self.do_clone_wlan(patch)
+
+    async def do_clone_wlan(self, template: dict, new_name: str = None, new_ssid: str = None) -> None:
+        wlansvc = await self._get_default_wlan_template()
+        self._normalize_encryption(wlansvc, template)
+        self._patch_template(wlansvc, template, True)
+        if new_name is not None or new_ssid is not None:
+            if new_name is None:
+                raise ValueError(VALUE_ERROR_WLAN_SSID_SETTING_REQUIRES_NAME)
+            self._patch_template(wlansvc, {"name": new_name, "ssid": new_ssid or new_name })
+        await self._add_wlan_template(wlansvc)
+
+    async def do_edit_wlan(self, name: str, patch: dict, ignore_unknown_attributes: bool = False) -> None:
+        wlansvc = await self._get_wlan_template(name)
+        if wlansvc:
+            self._normalize_encryption(wlansvc, patch)
+            self._patch_template(wlansvc, patch, ignore_unknown_attributes)
+            await self._update_wlan_template(wlansvc)
+
+    async def do_delete_wlan(self, name: str) -> bool:
+        wlan = await self._find_wlan_by_name(name)
+        if wlan is None:
+            return False
+        else:
+            await self._do_conf(f"<ajax-request action='delobj' updater='wlansvc-list.0.5' comp='wlansvc-list'><wlansvc id='{wlan['id']}'/></ajax-request>", timeout=20)
+            return True
+
+    async def do_add_wlan_group(self, name: str, description: str = "", wlans: List = None) -> None:
+        wlangroup = ET.Element("wlangroup", {"name": name, "description": description or ""})
+        if wlans is not None:
+            wlan_map = {wlan["name"]:wlan["id"] for wlan in await self.get_wlans()}
+            for wlansvc in wlans:
+                wlan_name = None
+                if isinstance(wlansvc, str):
+                    if wlansvc in wlan_map:
+                        wlan_name = wlansvc
+                elif isinstance(wlansvc, dict):
+                    if "name" in wlansvc and wlansvc["name"] in wlan_map:
+                        wlan_name = wlansvc["name"]
+                if wlan_name is None:
+                    raise ValueError(VALUE_ERROR_INVALID_WLAN)
+                ET.SubElement(wlangroup, "wlansvc", {"id": wlan_map[wlan_name]})
+        await self._do_conf(f"<ajax-request action='addobj' comp='wlangroup-list' updater='wgroup'>{ET.tostring(wlangroup).decode('utf-8')}</ajax-request>")
+
+    async def do_clone_wlan_group(self, template: dict, name: str, description: str = None) -> None:
+        wlangroup = ET.Element("wlangroup", {"name": name, "description": description or (template["description"] if "description" in template else "")})
+        if "wlan" in template:
+            wlan_map = {wlan["name"]:wlan["id"] for wlan in await self.get_wlans()}
+            for wlansvc in template["wlan"]:
+                ET.SubElement(wlangroup, "wlansvc", {"id": wlan_map[wlansvc["name"]]})
+        await self._do_conf(f"<ajax-request action='addobj' comp='wlangroup-list' updater='wgroup'>{ET.tostring(wlangroup).decode('utf-8')}</ajax-request>")
+
+    async def do_delete_wlan_group(self, name: str) -> bool:
+        wlang = await self._find_wlan_group_by_name(name)
+        if wlang is None:
+            return False
+        else:
+            await self._do_conf(f"<ajax-request action='delobj' updater='wlangroup-list.0.5' comp='wlangroup-list'><wlangroup id='{wlang['id']}'/></ajax-request>")
+            return True
+
+    async def do_hide_ap_leds(self, mac: str, leds_off: bool = True) -> None:
+        mac = self._normalize_mac(mac)
+        ap = await self._find_ap_by_mac(mac)
+        if ap:
+            await self._do_conf(f"<ajax-request action='updobj' updater='ap-list.0.5' comp='ap-list'><ap id='{ap['id']}' IS_PARTIAL='true' led-off='{str(leds_off).lower()}' /></ajax-request>")
+
+    async def do_show_ap_leds(self, mac: str) -> None:
+        await self.do_hide_ap_leds(mac, False)
+
+    async def do_restart_ap(self, mac: str) -> None:
+        mac = self._normalize_mac(mac)
+        return await self._cmdstat_noparse(f"<ajax-request action='docmd' xcmd='reset' checkAbility='2' updater='stamgr.0.5' comp='stamgr'><xcmd cmd='reset' ap='{mac}' tag='ap' checkAbility='2'/></ajax-request>")
+
+    async def _get_default_apgroup_template(self) -> ET.Element:
+        xml = await self.session.get_conf_str(ConfigItem.APGROUP_TEMPLATE)
+        root = ET.fromstring(xml)
+        return root.find(".//apgroup")
+
+    async def _get_default_wlan_template(self) -> ET.Element:
+        xml = await self.session.get_conf_str(ConfigItem.WLANSVC_STANDARD_TEMPLATE)
+        root = ET.fromstring(xml)
+        wlansvc = root.find(".//wlansvc")
+        if wlansvc is not None:
+            return wlansvc
+        else:
+            return self._get_default_cli_wlan_template()
+
+    @staticmethod
+    def _get_default_cli_wlan_template() -> ET.Element:
+        wlansvc = ET.Element("wlansvc", {"name": "default-standard-wlan", "ssid": "", "authentication": "open", "encryption": "none",
+                                         "is-guest": "false", "max-clients-per-radio": "100", "do-802-11d": "disabled", "sta-info-extraction": "1",
+                                         "force-dhcp": "0", "force-dhcp-timeout": "10", "usage": "user", "policy-id": "", "policy6-id": "",
+                                         "precedence-id": "1", "devicepolicy-id": "", "role-based-access-ctrl": "false", "acl-id": "1", "local-bridge": "1",
+                                         "client-isolation": "disabled", "ci-whitelist-id": "0", "bgscan": "1", "idle-timeout": "1", "max-idle-timeout": "300",
+                                         "dis-dgaf": "0", "authstats": "0", "https-redirection": "disabled"})
+        ET.SubElement(wlansvc, "qos", {"uplink-preset": "DISABLE", "downlink-preset": "DISABLE"})
+        ET.SubElement(wlansvc, "queue-priority", {"voice": "0", "video": "2", "data": "4", "background": "6"})
+        ET.SubElement(wlansvc, "wlan-schedule", {"value": "0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0:0x0: 0x0:0x0:0x0:0x0:0x0:0x0"})
+        return wlansvc
+
+    async def _get_wlan_template(self, name: str) -> ET.Element | None:
+        xml = await self.session.get_conf_str(ConfigItem.WLANSVC_LIST)
+        root = ET.fromstring(xml)
+        wlansvc = root.find(f".//wlansvc[@name='{saxutils.escape(name)}']")
+        return wlansvc
+
+    def _normalize_encryption(self, wlansvc: ET.Element, patch: dict):
+        patch_wpa = patch["wpa"] if "wpa" in patch else None
+        if patch_wpa is not None:
+            if "passphrase" in patch_wpa:
+                self._validate_passphrase(patch_wpa["passphrase"])
+            if "sae-passphrase" in patch_wpa:
+                self._validate_passphrase(patch_wpa["sae-passphrase"])
+
+        encryption = wlansvc.get("encryption")
+        if "encryption" in patch and patch["encryption"] != encryption:
+            new_encryption = patch["encryption"]
+            wlansvc.set("encryption", new_encryption)
+
+            wpa = wlansvc.find("wpa")
+            new_wpa = {"cipher": "aes", "dynamic-psk": "disabled"}
+
+            if new_encryption == WlanEncryption.WPA2.value or new_encryption == WlanEncryption.WPA23_MIXED.value:
+                passphrase = wpa.get("passphrase") if wpa is not None else None
+                if (patch_wpa is None or "passphrase" not in patch_wpa) and passphrase is None:
+                    raise ValueError(VALUE_ERROR_INVALID_PASSPHRASE_MISSING)
+                new_wpa["passphrase"] = passphrase or "<passphrase>"
+            if new_encryption == WlanEncryption.WPA3.value or new_encryption == WlanEncryption.WPA23_MIXED.value:
+                sae_passphrase = wpa.get("sae-passphrase") if wpa is not None else None
+                if (patch_wpa is None or "sae-passphrase" not in patch_wpa) and sae_passphrase is None:
+                    raise ValueError(VALUE_ERROR_INVALID_SAEPASSPHRASE_MISSING)
+                new_wpa["sae-passphrase"] = sae_passphrase or "<passphrase>"
+
+            if wpa is not None:
+                wlansvc.remove(wpa)
+            if new_encryption != WlanEncryption.NONE.value:
+                wpa = ET.SubElement(wlansvc, "wpa", new_wpa)
+
+    def _patch_template(self, element: ET.Element, patch: dict, ignore_unknown_attributes: bool = False, current_path: str = ""):
+        visited_children = set()
+        for child in element:
+            if child.tag in patch and isinstance(patch[child.tag], dict):
+                self._patch_template(child, patch[child.tag], ignore_unknown_attributes, f"{current_path}/{child.tag}")
+                visited_children.add(child.tag)
+        for name, value in patch.items():
+            if name in visited_children:
+                pass
+            else:
+                current_value = element.get(name)
+                if isinstance(value, List):
+                    raise ValueError(f"Applying lists is unsupported: {current_path}/{name}")
+                elif current_value is None:
+                    if not ignore_unknown_attributes:
+                        raise ValueError(f"Unknown attribute: {current_path}/{name}")
+                else:
+                    new_value = self._normalize_conf_value(current_value, value)
+                    element.set(name, new_value)
+                    x_name = f"x-{name}"
+                    if x_name not in patch and x_name in element.attrib:
+                        element.set(x_name, new_value)
+
+    async def _update_wlan_template(self, wlansvc: ET.Element):
+        xml_bytes = ET.tostring(wlansvc)
+        await self._do_conf(f"<ajax-request action='updobj' updater='wlan' comp='wlansvc-list'>{xml_bytes.decode('utf-8')}</ajax-request>", timeout=20)
+
+    async def _add_wlan_template(self, wlansvc: ET.Element):
+        xml_bytes = ET.tostring(wlansvc)
+        await self._do_conf(f"<ajax-request action='addobj' updater='wlansvc-list' comp='wlansvc-list'>{xml_bytes.decode('utf-8')}</ajax-request>", timeout=20)
+
+    async def _find_ap_by_mac(self, mac: str) -> dict:
+        return next((ap for ap in await self.get_aps() if ap["mac"] == mac), None)
+
+    async def _find_wlan_by_name(self, name: str) -> dict:
+        return next((wlan for wlan in await self.get_wlans() if wlan["name"] == name), None)
+
+    async def _find_wlan_group_by_name(self, name: str) -> dict:
+        return next((wlang for wlang in await self.get_wlan_groups() if wlang["name"] == name), None)
+
+    async def _get_timestamp_at_controller(self) -> int:
+        timeinfo = await self.cmdstat("<ajax-request action='getstat' updater='system.0.5' comp='system'><time/></ajax-request>")
+        return int(timeinfo["response"]["time"]["time"])
+
+    async def _cmdstat_noparse(self, data: str, timeout: int | None = None) -> str:
+        return await self.session.request(self.session.cmdstat_url, data, timeout)
+
+    async def cmdstat(self, data: str, collection_elements: List[str] = None, timeout: int | None = None) -> dict | List:
+        result_text = await self._cmdstat_noparse(data, timeout)
+        return self._ruckus_xml_unwrap(result_text, collection_elements)
+
+    async def _conf_noparse(self, data: str, timeout: int | None = None) -> str:
+        return await self.session.request(self.session.conf_url, data, timeout)
+
+    async def conf(self, data: str, collection_elements: List[str] = None, timeout: int | None = None) -> dict | List:
+        result_text = await self._conf_noparse(data, timeout)
+        return self._ruckus_xml_unwrap(result_text, collection_elements)
+
+    async def _do_conf(self, data: str, collection_elements: List[str] = None, timeout: int | None = None) -> None:
+        result = await self.conf(data, collection_elements, timeout)
+        if "xmsg" in result:
+            raise ValueError(result["xmsg"]["lmsg"])
+
+    @staticmethod
+    def _normalize_mac(mac: str) -> str:
+        if mac and match(r"(?:[0-9a-f]{2}[:-]){5}[0-9a-f]{2}", string=mac, flags=IGNORECASE):
+            return mac.replace('-', ':').lower()
+        raise ValueError(VALUE_ERROR_INVALID_MAC)
+
+    @staticmethod
+    def _validate_passphrase(passphrase: str) -> str:
+        if passphrase and match(r".*<.*>.*", string=passphrase):
+            raise ValueError(VALUE_ERROR_INVALID_PASSPHRASE_JS)
+        if passphrase and match(r"(^[!-~]([ -~]){6,61}[!-~]$)|(^([0-9a-fA-F]){64}$)", string=passphrase):
+            return passphrase
+        raise ValueError(VALUE_ERROR_INVALID_PASSPHRASE_LEN)
+
+    @staticmethod
+    def _normalize_conf_value(current_value: str, new_value: Any) -> str:
+        current_value_lowered = current_value.lower()
+        if current_value_lowered in ("enable", "disable", "enabled", "disabled", "true", "false", "yes", "no", "1", "0"):
+            if isinstance(new_value, str):
+                new_value_lowered = new_value.lower()
+                new_value = True if new_value_lowered in ("enable", "enabled", "true", "yes", "1") else False if new_value_lowered in ("disable", "disabled", "false", "no", "0") else new_value
+            elif isinstance(new_value, (int, float)) and not isinstance(new_value, bool):
+                new_value = True if new_value == 1 else False if new_value == 0 else new_value
+
+            if isinstance(new_value, bool):
+                if current_value_lowered in ("enable", "disable"):
+                    new_value = "ENABLE" if new_value else "DISABLE"
+                elif current_value_lowered in ("enabled", "disabled"):
+                    new_value = "enabled" if new_value else "disabled"
+                elif current_value_lowered in ("yes", "no"):
+                    new_value = "yes" if new_value else "no"
+                elif current_value_lowered in ("true", "false"):
+                    new_value = "true" if new_value else "false"
+                elif current_value_lowered in ("1", "0"):
+                    new_value = "1" if new_value else "0"
+        return new_value
```

### Comparing `aioruckus-0.24/aioruckus.egg-info/PKG-INFO` & `aioruckus-0.30/aioruckus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,89 +1,105 @@
-Metadata-Version: 2.1
-Name: aioruckus
-Version: 0.24
-Summary: Python API to interact with Ruckus Unleashed and ZoneDirector devices.
-Home-page: https://github.com/ms264556/aioruckus
-Author: ms264556
-Author-email: bsd0@patterni.city
-License: BSD0
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# aioruckus
-
-A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.
-
-Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
-
-## How to install
-
-```bash
-pip install aioruckus
-```
-
-## Usage
-
-Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
-
-```python
-from aioruckus import AjaxSession, SystemStat
-import asyncio
-
-async def test_aioruckus():
-    
-    async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
-        ruckus = session.api
-
-        wlans = await ruckus.get_wlans()
-        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
-        aps = await ruckus.get_aps()
-        ap_groups = await ruckus.get_ap_groups()
-        mesh = await ruckus.get_mesh_info()
-        default_system_info = await ruckus.get_system_info()
-        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
-        active_clients = await ruckus.get_active_clients()
-        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
-        blocked = await ruckus.get_blocked_client_macs()
-        syslog = await ruckus.get_syslog()
-
-        await ruckus.do_block_client("60:ab:de:ad:be:ef")
-        await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
-
-        await ruckus.do_disable_wlan("my ssid")
-        await ruckus.do_enable_wlan("my ssid")
-
-        await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
-
-        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
-        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
-
-        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
-        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
-
-        await ruckus.do_delete_wlan_group("Copy of Default")
-
-        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
-        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
-
-        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
-        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
-        await ruckus.do_delete_wlan("my newer sid")
-
-        await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
-        await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
-        
-        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
-
-asyncio.run(test_aioruckus())
-```
-
-### Other Python APIs for Ruckus Unleashed
-
-This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
-
-There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
-Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
+Metadata-Version: 2.1
+Name: aioruckus
+Version: 0.30
+Summary: Python API to interact with Ruckus Unleashed and ZoneDirector devices.
+Home-page: https://github.com/ms264556/aioruckus
+Author: ms264556
+Author-email: bsd0@patterni.city
+License: BSD0
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# aioruckus
+
+A Python API which interacts with Ruckus Unleashed and ZoneDirector devices via their AJAX Web Service interface.  
+Configuration information can also be queried from Ruckus Unleashed and ZoneDirector backup files.
+
+Compatible with all Ruckus Unleashed versions, and Ruckus ZoneDirector versions 9.10 onwards.
+
+## How to install
+
+```bash
+pip install aioruckus
+```
+
+## Usage
+
+Functions are defined within an [async](https://docs.python.org/3/library/asyncio.html) [context manager](https://docs.python.org/3/reference/datamodel.html#context-managers), so you will have to use [asyncio](https://docs.python.org/3/library/asyncio.html) rather than calling the functions directly in a shell.
+
+```python
+from aioruckus import AjaxSession, BackupSession, SystemStat
+import asyncio
+
+async def test_aioruckus():
+    
+    with BackupSession.create("<ruckus backup filename>") as session:
+        ruckus = session.api
+
+        aps = await ruckus.get_aps()
+        ap_groups = await ruckus.get_ap_groups()
+        wlans = await ruckus.get_wlans()
+        wlan_groups = await ruckus.get_wlan_groups()
+        blocked = await ruckus.get_blocked_client_macs()
+        mesh = await ruckus.get_mesh_info()
+        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
+
+    async with AjaxSession.async_create("<ruckus ip>", "<ruckus user>", "<ruckus password>") as session:
+        ruckus = session.api
+
+        aps = await ruckus.get_aps()
+        ap_groups = await ruckus.get_ap_groups()
+        wlans = await ruckus.get_wlans()
+        wlan_groups = await ruckus.get_wlan_groups() # WLAN Groups are CLI-only on Unleashed
+        blocked = await ruckus.get_blocked_client_macs()
+        mesh = await ruckus.get_mesh_info()
+        default_system_info = await ruckus.get_system_info()
+        all_system_info = await ruckus.get_system_info(SystemStat.ALL)
+
+        ap_group_stats = await ruckus.get_ap_group_stats()
+        wlan_group_stats = await ruckus.get_wlan_group_stats()
+
+        active_clients = await ruckus.get_active_clients()
+        inactive_clients = await ruckus.get_inactive_clients() # always empty on Unleashed
+        syslog = await ruckus.get_syslog()
+
+        await ruckus.do_block_client("60:ab:de:ad:be:ef")
+        await ruckus.do_unblock_client("60:ab:de:ad:be:ef")
+
+        await ruckus.do_disable_wlan("my ssid")
+        await ruckus.do_enable_wlan("my ssid")
+
+        await ruckus.do_set_wlan_password("my ssid", "blah>blah<")
+
+        await ruckus.do_add_wlan_group("new empty wlangroup", "empty group added by aioruckus")
+        await ruckus.do_add_wlan_group("new full wlangroup", "group added by aioruckus", wlans)
+
+        wlan_group_template = next((wlang for wlang in wlan_groups if wlang["name"] == "Default"), None)
+        await ruckus.do_clone_wlan_group(wlan_group_template, "Copy of Default")
+
+        await ruckus.do_delete_wlan_group("Copy of Default")
+
+        await ruckus.do_add_wlan("my new sid", passphrase="mypassphrase" )
+        await ruckus.do_edit_wlan("my new sid", {"ofdm-rate-only": True})
+
+        template_wlan = next((wlan for wlan in wlans if wlan["name"] == "my ssid"), None)
+        await ruckus.do_clone_wlan(template_wlan, "my newer sid")
+        await ruckus.do_delete_wlan("my newer sid")
+
+        await ruckus.do_hide_ap_leds("24:79:de:ad:be:ef")
+        await ruckus.do_show_ap_leds("24:79:de:ad:be:ef")
+        
+        await ruckus.do_restart_ap("24:79:de:ad:be:ef")
+
+asyncio.run(test_aioruckus())
+```
+
+### Other Python APIs for Ruckus Unleashed
+
+This project was originally a fork of [pyuckus](https://github.com/gabe565/pyruckus), which provides similar query functionality by controlling an SSH CLI session.
+
+There is also [scrapli](https://github.com/carlmontanari/scrapli) support for the Ruckus Unleashed SSH CLI via [scrapli community](https://github.com/scrapli/scrapli_community).  
+Authentication and privilege levels are implemented, but no templates are implemented as of April 2023.
```

### Comparing `aioruckus-0.24/tests/test_connection.py` & `aioruckus-0.30/tests/test_connection.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-"""Test connecting to a device and issuing commands."""
-import pytest
-
-from aioruckus.exceptions import AuthenticationError
-from tests import connect_ruckus
-
-
-@pytest.mark.asyncio
-async def test_connect_success():
-    """Normal connection / disconnection."""
-    async with connect_ruckus() as ruckus:
-        pass
-
-@pytest.mark.asyncio
-async def test_authentication_error():
-    """Invalid login."""
-    with pytest.raises(AuthenticationError):
-        async with connect_ruckus(password="bad-password") as ruckus:
-            pass
-
-@pytest.mark.asyncio
-async def test_connection_error():
-    """Non- Unleashed/ZoneDirector host."""
-    with pytest.raises(ConnectionError):
-        async with connect_ruckus(host="127.0.0.1") as ruckus:
-            pass
+"""Test connecting to a device and issuing commands."""
+import pytest
+
+from aioruckus.exceptions import AuthenticationError
+from tests import connect_ruckus
+
+
+@pytest.mark.asyncio
+async def test_connect_success():
+    """Normal connection / disconnection."""
+    async with connect_ruckus() as ruckus:
+        pass
+
+@pytest.mark.asyncio
+async def test_authentication_error():
+    """Invalid login."""
+    with pytest.raises(AuthenticationError):
+        async with connect_ruckus(password="bad-password") as ruckus:
+            pass
+
+@pytest.mark.asyncio
+async def test_connection_error():
+    """Non- Unleashed/ZoneDirector host."""
+    with pytest.raises(ConnectionError):
+        async with connect_ruckus(host="127.0.0.1") as ruckus:
+            pass
```

### Comparing `aioruckus-0.24/tests/test_data.py` & `aioruckus-0.30/tests/test_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-"""Test data returned from a device."""
-import pytest
-
-from tests import connect_ruckus
-
-
-@pytest.mark.asyncio
-async def test_current_active_clients():
-    async with connect_ruckus() as ruckus:
-        clients = await ruckus.api.get_active_clients()
-        assert clients
-        client = clients[0]
-        assert client["mac"]
-        assert client["ap"]
-        assert client["vap-mac"] # per-radio ssid
-
-@pytest.mark.asyncio
-async def test_mesh_info():
-    """Test we can get mesh info."""
-    async with connect_ruckus() as ruckus:
-        mesh_info = await ruckus.api.get_mesh_info()
-        assert mesh_info["name"]
-
-@pytest.mark.asyncio
-async def test_system_info():
-    """Test we can get system info."""
-    async with connect_ruckus() as ruckus:
-        system_info = await ruckus.api.get_system_info()
-        assert system_info["identity"]["name"]
-        assert system_info["sysinfo"]["serial"]
-        assert system_info["sysinfo"]["version"]
-        assert system_info["port"]["ip"]
-
-@pytest.mark.asyncio
-async def test_ap_info():
-    """Test we can get access point info."""
-    async with connect_ruckus() as ruckus:
-        ap_info = await ruckus.api.get_aps()
-        ap = ap_info[0]
-        assert ap["mac"]
-        assert ap["model"]
-        assert ap["devname"]
-        assert ap["gateway"]
-        assert ap["channel-11ng"]
-        assert ap["channelization-11ng"]
+"""Test data returned from a device."""
+import pytest
+
+from tests import connect_ruckus
+
+
+@pytest.mark.asyncio
+async def test_current_active_clients():
+    async with connect_ruckus() as ruckus:
+        clients = await ruckus.api.get_active_clients()
+        assert clients
+        client = clients[0]
+        assert client["mac"]
+        assert client["ap"]
+        assert client["vap-mac"] # per-radio ssid
+
+@pytest.mark.asyncio
+async def test_mesh_info():
+    """Test we can get mesh info."""
+    async with connect_ruckus() as ruckus:
+        mesh_info = await ruckus.api.get_mesh_info()
+        assert mesh_info["name"]
+
+@pytest.mark.asyncio
+async def test_system_info():
+    """Test we can get system info."""
+    async with connect_ruckus() as ruckus:
+        system_info = await ruckus.api.get_system_info()
+        assert system_info["identity"]["name"]
+        assert system_info["sysinfo"]["serial"]
+        assert system_info["sysinfo"]["version"]
+        assert system_info["port"]["ip"]
+
+@pytest.mark.asyncio
+async def test_ap_info():
+    """Test we can get access point info."""
+    async with connect_ruckus() as ruckus:
+        ap_info = await ruckus.api.get_aps()
+        ap = ap_info[0]
+        assert ap["mac"]
+        assert ap["model"]
+        assert ap["devname"]
+        assert ap["gateway"]
+        assert ap["radio"][0]["channel"]
+        assert ap["radio"][0]["channelization"]
```

