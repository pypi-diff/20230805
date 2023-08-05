# Comparing `tmp/sonnenbatterie-0.2.0.tar.gz` & `tmp/sonnenbatterie-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonnenbatterie-0.2.0.tar", last modified: Fri Jul 21 08:57:44 2023, max compression
+gzip compressed data, was "sonnenbatterie-0.2.2.tar", last modified: Sat Aug  5 09:05:05 2023, max compression
```

## Comparing `sonnenbatterie-0.2.0.tar` & `sonnenbatterie-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.907661 sonnenbatterie-0.2.0/
--rw-rw-rw-   0        0        0    35823 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.0/LICENSE
--rw-rw-rw-   0        0        0      557 2023-07-21 08:57:44.906435 sonnenbatterie-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0       25 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-21 08:57:44.907661 sonnenbatterie-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0      830 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.891443 sonnenbatterie-0.2.0/sonnenbatterie/
--rw-rw-rw-   0        0        0       42 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.0/sonnenbatterie/__init__.py
--rw-rw-rw-   0        0        0     1548 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/sonnenbatterie/const.py
--rw-rw-rw-   0        0        0     6264 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/sonnenbatterie/sonnenbatterie.py
--rw-rw-rw-   0        0        0     5425 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/sonnenbatterie/timeofuse.py
-drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.901434 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/
--rw-rw-rw-   0        0        0      557 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      462 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-21 08:57:44.000000 sonnenbatterie-0.2.0/sonnenbatterie.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-21 08:57:44.906435 sonnenbatterie-0.2.0/test/
--rw-rw-rw-   0        0        0     2158 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_battery_reserve.py
--rw-rw-rw-   0        0        0     1964 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_operating_mode.py
--rw-rw-rw-   0        0        0      985 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_origional_code.py
--rw-rw-rw-   0        0        0     1945 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_timeofuse.py
--rw-rw-rw-   0        0        0     2637 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.0/test/test_timeofuse_lib.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:05:05.186665 sonnenbatterie-0.2.2/
+-rw-rw-rw-   0        0        0    35823 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0      557 2023-08-05 09:05:05.186665 sonnenbatterie-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0       25 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:05:05.186665 sonnenbatterie-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      830 2023-08-05 09:04:59.000000 sonnenbatterie-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:05:05.076892 sonnenbatterie-0.2.2/sonnenbatterie/
+-rw-rw-rw-   0        0        0       42 2023-07-21 08:41:34.000000 sonnenbatterie-0.2.2/sonnenbatterie/__init__.py
+-rw-rw-rw-   0        0        0     1614 2023-08-05 09:04:59.000000 sonnenbatterie-0.2.2/sonnenbatterie/const.py
+-rw-rw-rw-   0        0        0     7284 2023-08-05 09:04:59.000000 sonnenbatterie-0.2.2/sonnenbatterie/sonnenbatterie.py
+-rw-rw-rw-   0        0        0     5425 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.2/sonnenbatterie/timeofuse.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:05:05.171038 sonnenbatterie-0.2.2/sonnenbatterie.egg-info/
+-rw-rw-rw-   0        0        0      557 2023-08-05 09:05:05.000000 sonnenbatterie-0.2.2/sonnenbatterie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      484 2023-08-05 09:05:05.000000 sonnenbatterie-0.2.2/sonnenbatterie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:05:05.000000 sonnenbatterie-0.2.2/sonnenbatterie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-08-05 09:05:05.000000 sonnenbatterie-0.2.2/sonnenbatterie.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-05 09:05:05.000000 sonnenbatterie-0.2.2/sonnenbatterie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 09:05:05.186665 sonnenbatterie-0.2.2/test/
+-rw-rw-rw-   0        0        0     2158 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.2/test/test_battery_reserve.py
+-rw-rw-rw-   0        0        0     1964 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.2/test/test_operating_mode.py
+-rw-rw-rw-   0        0        0      985 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.2/test/test_origional_code.py
+-rw-rw-rw-   0        0        0     1954 2023-08-05 09:04:59.000000 sonnenbatterie-0.2.2/test/test_setpoint.py
+-rw-rw-rw-   0        0        0     1945 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.2/test/test_timeofuse.py
+-rw-rw-rw-   0        0        0     2637 2023-07-21 08:53:03.000000 sonnenbatterie-0.2.2/test/test_timeofuse_lib.py
```

### Comparing `sonnenbatterie-0.2.0/LICENSE` & `sonnenbatterie-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sonnenbatterie-0.2.0/PKG-INFO` & `sonnenbatterie-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonnenbatterie
-Version: 0.2.0
+Version: 0.2.2
 Summary: Access Sonnenbatterie REST API
 Home-page: https://github.com/weltmeyer/python_sonnenbatterie
 Author: Jan Weltmeyer
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sonnenbatterie-0.2.0/setup.py` & `sonnenbatterie-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="sonnenbatterie", # Replace with your own username
-    version="0.2.0",
+    version="0.2.2",
     author="Jan Weltmeyer",
     author_email="author@example.com",
     description="Access Sonnenbatterie REST API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/weltmeyer/python_sonnenbatterie",
     packages=["sonnenbatterie"],
```

### Comparing `sonnenbatterie-0.2.0/sonnenbatterie/const.py` & `sonnenbatterie-0.2.2/sonnenbatterie/const.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,8 +19,11 @@
 SONNEN_API_PATH_CONFIGURATIONS="v2/configurations"
 SONNEN_API_PATH_LATEST_DATA="v2/latestdata"
 SONNEN_API_PATH_POWER_METER="powermeter"
 SONNEN_API_PATH_BATTERY_SYSTEM="battery_system"
 SONNEN_API_PATH_INVERTER="inverter"
 SONNEN_API_PATH_SYSTEM_DATA="system_data"
 SONNEN_API_PATH_STATUS="v1/status"
-SONNEN_API_PATH_BATTERY="battery"
+SONNEN_API_PATH_BATTERY="battery"
+
+SONNEN_CHARGE_PATH="charge"
+SONNEN_DISCHARGE_PATH="discharge"
```

### Comparing `sonnenbatterie-0.2.0/sonnenbatterie/sonnenbatterie.py` & `sonnenbatterie-0.2.2/sonnenbatterie/sonnenbatterie.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 class sonnenbatterie:
     def __init__(self,username,password,ipaddress):
         self.username=username
         self.password=password
         self.ipaddress=ipaddress
         self.baseurl='http://'+self.ipaddress+'/api/'
+        self.setpoint=self.baseurl+'v2/setpoint/'
         self._login()
 
 
     def _login(self):
         password_sha512 = hashlib.sha512(self.password.encode('utf-8')).hexdigest()
         req_challenge=requests.get(self.baseurl+'challenge')
         req_challenge.raise_for_status()
@@ -51,15 +52,33 @@
         if not isretry and response.status_code==401:
             self._login()
             return self._get(what,True)
         if response.status_code != 200:
             response.raise_for_status()
         return response.json()
 
+    # these are special purpose endpoints, there is no associated data that I'm aware of
+    # while I don't have details I belive this is probabaly onlu useful in manual more
+    # and it's probabaly possible to extact the actuall flow rate in operation  
+    # looking at the status.state_battery_inout value
+    def set_manual_flowrate(self, direction, rate):
+        path=self.setpoint+direction+"/"+str(rate)
+        response=requests.post(url=path,
+            headers={'Auth-Token': self.token,'Content-Type': 'application/json'}
+        )
+        return (response.status_code == 201)
+    
+    def set_discharge(self, rate):
+        return self.set_manual_flowrate(SONNEN_DISCHARGE_PATH, rate)
+    
 
+    def set_charge(self, rate):
+        return self.set_manual_flowrate(SONNEN_CHARGE_PATH, rate)
+
+    # more general purpose endpoints
     def set_configuration(self, name, value):
         # All configurations names and values are hendled as strings, so force that
         payload = {str(name): str(value)}
         return self._put(SONNEN_API_PATH_CONFIGURATIONS, payload)
 
     def get_powermeter(self):
         return self._get(SONNEN_API_PATH_POWER_METER)
@@ -78,34 +97,36 @@
         
     def get_battery(self):
         return self._get(SONNEN_API_PATH_BATTERY)
         
     def get_latest_data(self):
         return self._get(SONNEN_API_PATH_LATEST_DATA)
     
-    def get_current_charge_level(self):
-        return self.get_latest_data().get(SONNEN_LATEST_DATA_CHARGE_LEVEL)
-    
     def get_configurations(self):
         return self._get(SONNEN_API_PATH_CONFIGURATIONS)
     
     def get_configuration(self, name):
         return self._get(SONNEN_API_PATH_CONFIGURATIONS+"/"+name).get(name) 
+    
+
+    # these have special handling in some form, for example converting a mode as a number into a string
+    def get_current_charge_level(self):
+        return self.get_latest_data().get(SONNEN_LATEST_DATA_CHARGE_LEVEL)
 
     def get_operating_mode(self):
         return self.get_configuration(SONNEN_CONFIGURATION_OPERATING_MODE)
     
     def get_operating_mode_name(self):
         operating_mode_num = self.get_operating_mode()
         return SONNEN_OPERATING_MODES_TO_OPERATING_MODE_NAMES.get(operating_mode_num)
     
     def set_operating_mode(self, operating_mode):
         return self.set_configuration(SONNEN_CONFIGURATION_OPERATING_MODE, operating_mode)
     
-    def set_operaing_mode_by_name(self, operating_mode_name):
+    def set_operating_mode_by_name(self, operating_mode_name):
         return self.set_operating_mode(SONNEN_OPERATING_MODE_NAMES_TO_OPERATING_MODES.get(operating_mode_name))
     
     def get_battery_reserve(self):
         return self.get_configuration(SONNEN_CONFIGURATION_BACKUP_RESERVE)
     
     def set_battery_reserve(self, reserve=5):
         reserve = int(reserve)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sonnenbatterie-0.2.0/sonnenbatterie/timeofuse.py` & `sonnenbatterie-0.2.2/sonnenbatterie/timeofuse.py`

 * *Files identical despite different names*

### Comparing `sonnenbatterie-0.2.0/sonnenbatterie.egg-info/PKG-INFO` & `sonnenbatterie-0.2.2/sonnenbatterie.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonnenbatterie
-Version: 0.2.0
+Version: 0.2.2
 Summary: Access Sonnenbatterie REST API
 Home-page: https://github.com/weltmeyer/python_sonnenbatterie
 Author: Jan Weltmeyer
 Author-email: author@example.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
```

### Comparing `sonnenbatterie-0.2.0/test/test_battery_reserve.py` & `sonnenbatterie-0.2.2/test/test_battery_reserve.py`

 * *Files identical despite different names*

### Comparing `sonnenbatterie-0.2.0/test/test_operating_mode.py` & `sonnenbatterie-0.2.2/test/test_operating_mode.py`

 * *Files identical despite different names*

### Comparing `sonnenbatterie-0.2.0/test/test_origional_code.py` & `sonnenbatterie-0.2.2/test/test_origional_code.py`

 * *Files identical despite different names*

### Comparing `sonnenbatterie-0.2.0/test/test_timeofuse.py` & `sonnenbatterie-0.2.2/test/test_timeofuse.py`

 * *Files identical despite different names*

### Comparing `sonnenbatterie-0.2.0/test/test_timeofuse_lib.py` & `sonnenbatterie-0.2.2/test/test_timeofuse_lib.py`

 * *Files identical despite different names*

