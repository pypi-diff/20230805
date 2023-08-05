# Comparing `tmp/openshift-python-utilities-4.14.2.tar.gz` & `tmp/openshift-python-utilities-4.14.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift-python-utilities-4.14.2.tar", last modified: Tue Jun 20 09:56:51 2023, max compression
+gzip compressed data, was "openshift-python-utilities-4.14.4.tar", last modified: Sat Aug  5 16:10:28 2023, max compression
```

## Comparing `openshift-python-utilities-4.14.2.tar` & `openshift-python-utilities-4.14.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:51.696307 openshift-python-utilities-4.14.2/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1455 2023-06-20 09:56:51.695307 openshift-python-utilities-4.14.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      670 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/README.md
--rw-r--r--   0 root         (0) root         (0)        7 2023-06-20 09:56:50.000000 openshift-python-utilities-4.14.2/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:51.695307 openshift-python-utilities-4.14.2/ocp_utilities/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/__init__.py
--rw-r--r--   0 root         (0) root         (0)      517 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/debugger.py
--rw-r--r--   0 root         (0) root         (0)      452 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/exceptions.py
--rw-r--r--   0 root         (0) root         (0)    13883 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/infra.py
--rw-r--r--   0 root         (0) root         (0)     6799 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/monitoring.py
--rw-r--r--   0 root         (0) root         (0)     1877 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/must_gather.py
--rw-r--r--   0 root         (0) root         (0)    12232 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/operators.py
--rw-r--r--   0 root         (0) root         (0)     3104 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/ocp_utilities/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-20 09:56:51.695307 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1455 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      499 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      112 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-06-20 09:56:51.000000 openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1494 2023-06-20 09:56:47.000000 openshift-python-utilities-4.14.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-20 09:56:51.696307 openshift-python-utilities-4.14.2/setup.cfg
+drwxr-xr-x   0 podman    (1000) podman    (1000)        0 2023-08-05 16:10:28.441895 openshift-python-utilities-4.14.4/
+-rw-r--r--   0 podman    (1000) podman    (1000)    11357 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/LICENSE
+-rw-r--r--   0 podman    (1000) podman    (1000)     1455 2023-08-05 16:10:28.441895 openshift-python-utilities-4.14.4/PKG-INFO
+-rw-r--r--   0 podman    (1000) podman    (1000)      670 2023-08-05 16:10:25.000000 openshift-python-utilities-4.14.4/README.md
+-rw-r--r--   0 podman    (1000) podman    (1000)        7 2023-08-05 16:10:25.000000 openshift-python-utilities-4.14.4/VERSION
+drwxr-xr-x   0 podman    (1000) podman    (1000)        0 2023-08-05 16:10:28.440895 openshift-python-utilities-4.14.4/ocp_utilities/
+-rw-r--r--   0 podman    (1000) podman    (1000)        0 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/__init__.py
+-rw-r--r--   0 podman    (1000) podman    (1000)      517 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/debugger.py
+-rw-r--r--   0 podman    (1000) podman    (1000)      452 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/exceptions.py
+-rw-r--r--   0 podman    (1000) podman    (1000)    13883 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/infra.py
+-rw-r--r--   0 podman    (1000) podman    (1000)     7608 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/monitoring.py
+-rw-r--r--   0 podman    (1000) podman    (1000)     1877 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/must_gather.py
+-rw-r--r--   0 podman    (1000) podman    (1000)    12232 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/operators.py
+-rw-r--r--   0 podman    (1000) podman    (1000)     3104 2023-08-05 16:10:24.000000 openshift-python-utilities-4.14.4/ocp_utilities/utils.py
+drwxr-xr-x   0 podman    (1000) podman    (1000)        0 2023-08-05 16:10:28.441895 openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/
+-rw-r--r--   0 podman    (1000) podman    (1000)     1455 2023-08-05 16:10:28.000000 openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 podman    (1000) podman    (1000)      499 2023-08-05 16:10:28.000000 openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 podman    (1000) podman    (1000)        1 2023-08-05 16:10:28.000000 openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 podman    (1000) podman    (1000)      112 2023-08-05 16:10:28.000000 openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/requires.txt
+-rw-r--r--   0 podman    (1000) podman    (1000)       14 2023-08-05 16:10:28.000000 openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/top_level.txt
+-rw-r--r--   0 podman    (1000) podman    (1000)     1494 2023-08-05 16:10:25.000000 openshift-python-utilities-4.14.4/pyproject.toml
+-rw-r--r--   0 podman    (1000) podman    (1000)       38 2023-08-05 16:10:28.441895 openshift-python-utilities-4.14.4/setup.cfg
```

### Comparing `openshift-python-utilities-4.14.2/LICENSE` & `openshift-python-utilities-4.14.4/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/PKG-INFO` & `openshift-python-utilities-4.14.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.14.2
+Version: 4.14.4
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.14.2/README.md` & `openshift-python-utilities-4.14.4/README.md`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/ocp_utilities/debugger.py` & `openshift-python-utilities-4.14.4/ocp_utilities/debugger.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/ocp_utilities/infra.py` & `openshift-python-utilities-4.14.4/ocp_utilities/infra.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/ocp_utilities/monitoring.py` & `openshift-python-utilities-4.14.4/ocp_utilities/monitoring.py`

 * *Files 14% similar despite different names*

```diff
@@ -129,16 +129,15 @@
                 alert_list.append(alert)
         return alert_list
 
     def get_firing_alerts(self, alert_name):
         """
         get all the firing alerts from list of active alerts
         """
-        alert_list = self.get_all_alerts_by_alert_name(alert_name=alert_name)
-        return [alert for alert in alert_list if alert["state"] == "firing"]
+        return self.get_alerts_by_state(alert_name=alert_name)
 
     def wait_for_firing_alert_sampler(self, alert_name, timeout=TIMEOUT_10MIN):
         """
         Sample output for an alert if found in fired state
 
         Args:
              alert (str): alert name
@@ -146,29 +145,15 @@
 
         Return:
              sample (list): list of all alerts that match the alert name and in firing state
 
         Raise:
              TimeoutExpiredError: if alert is not fired before wait_timeout
         """
-        sampler = TimeoutSampler(
-            wait_timeout=timeout,
-            sleep=self.scrape_interval,
-            func=self.get_firing_alerts,
-            alert_name=alert_name,
-        )
-        try:
-            for sample in sampler:
-                if sample:
-                    LOGGER.info(f"Found alert: {alert_name} in firing state.")
-                    return sample
-
-        except TimeoutExpiredError:
-            LOGGER.error(f"{alert_name} currently not in firing state")
-            raise
+        return self.wait_for_alert_by_state_sampler(alert_name=alert_name)
 
     def get_scrape_interval(self):
         """
         get prometheus scrap interval
 
         Returns:
              int: scrape time interval or default 30 if not found
@@ -213,7 +198,44 @@
             raise
 
     def alerts(self):
         """
         get all the active alerts
         """
         return self._get_response(query=f"{self.api_v1}/alerts")
+
+    def get_alerts_by_state(self, alert_name, state="firing"):
+        """
+        get all the alerts from list of active alerts according the state
+        """
+        alert_list = self.get_all_alerts_by_alert_name(alert_name=alert_name)
+        return [alert for alert in alert_list if alert["state"] == state]
+
+    def wait_for_alert_by_state_sampler(
+        self, alert_name, timeout=TIMEOUT_10MIN, state="firing"
+    ):
+        """
+        Sample output for an alert if found in the state provided in the args.
+
+        Args:
+             alert_name (str): alert name
+             timeout (int): wait time, default is 10 mins
+             state (str): state of the alert to expect, default is firing
+
+        Return:
+             sample (list): list of all alerts that match the alert name and in the state provided in args.
+
+        Raise:
+             TimeoutExpiredError: if alert is not in the state specified before wait_timeout
+        """
+        sampler = TimeoutSampler(
+            wait_timeout=timeout,
+            sleep=self.scrape_interval,
+            func=self.get_alerts_by_state,
+            alert_name=alert_name,
+            state=state,
+        )
+
+        for sample in sampler:
+            if sample:
+                LOGGER.info(f"Found alert: {alert_name} in {state} state.")
+                return sample
```

### Comparing `openshift-python-utilities-4.14.2/ocp_utilities/must_gather.py` & `openshift-python-utilities-4.14.4/ocp_utilities/must_gather.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/ocp_utilities/operators.py` & `openshift-python-utilities-4.14.4/ocp_utilities/operators.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/ocp_utilities/utils.py` & `openshift-python-utilities-4.14.4/ocp_utilities/utils.py`

 * *Files identical despite different names*

### Comparing `openshift-python-utilities-4.14.2/openshift_python_utilities.egg-info/PKG-INFO` & `openshift-python-utilities-4.14.4/openshift_python_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-utilities
-Version: 4.14.2
+Version: 4.14.4
 Summary: A utilities repository for https://github.com/RedHatQE/openshift-python-wrapper
 Author-email: Meni Yakove <myakove@gmail.com>, Ruth Netser <rnetser@gmail.com>
 Project-URL: Homepage, https://github.com/RedHatQE/openshift-python-utilities
 Project-URL: Download, https://pypi.org/project/openshift-python-utilities/
 Project-URL: Bug Tracker, https://github.com/RedHatQE/openshift-python-utilities/issues
 Project-URL: Documentation, https://github.com/RedHatQE/openshift-python-utilities/blob/main/README.md
 Keywords: Openshift
```

### Comparing `openshift-python-utilities-4.14.2/pyproject.toml` & `openshift-python-utilities-4.14.4/pyproject.toml`

 * *Files identical despite different names*

