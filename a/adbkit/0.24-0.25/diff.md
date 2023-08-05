# Comparing `tmp/adbkit-0.24.tar.gz` & `tmp/adbkit-0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adbkit-0.24.tar", last modified: Thu Aug  3 05:02:46 2023, max compression
+gzip compressed data, was "adbkit-0.25.tar", last modified: Sat Aug  5 00:14:10 2023, max compression
```

## Comparing `adbkit-0.24.tar` & `adbkit-0.25.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 05:02:46.237656 adbkit-0.24/
--rw-rw-rw-   0        0        0     1148 2023-08-03 05:02:03.000000 adbkit-0.24/LICENSE.rst
--rw-rw-rw-   0        0        0       89 2023-08-03 05:01:59.000000 adbkit-0.24/MANIFEST.in
--rw-rw-rw-   0        0        0   164625 2023-08-03 05:02:46.238631 adbkit-0.24/PKG-INFO
--rw-rw-rw-   0        0        0   162899 2023-08-03 04:58:57.000000 adbkit-0.24/README.md
-drwxrwxrwx   0        0        0        0 2023-08-03 05:02:46.232776 adbkit-0.24/adbkit/
--rw-rw-rw-   0        0        0   162899 2023-08-03 04:58:57.000000 adbkit-0.24/adbkit/README.MD
--rw-rw-rw-   0        0        0   132732 2023-08-03 04:45:19.000000 adbkit-0.24/adbkit/__init__.py
--rw-rw-rw-   0        0        0      696 2023-08-03 05:02:41.000000 adbkit-0.24/adbkit/requirements.txt
--rw-rw-rw-   0        0        0   284867 2023-08-03 05:02:41.000000 adbkit-0.24/adbkit/thirdparty.json
-drwxrwxrwx   0        0        0        0 2023-08-03 05:02:46.236679 adbkit-0.24/adbkit.egg-info/
--rw-rw-rw-   0        0        0   164625 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      284 2023-08-03 05:02:46.000000 adbkit-0.24/adbkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      660 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-03 05:02:45.000000 adbkit-0.24/adbkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       85 2023-08-03 05:02:46.250851 adbkit-0.24/setup.cfg
--rw-rw-rw-   0        0        0     2803 2023-08-03 05:02:41.000000 adbkit-0.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:14:10.888395 adbkit-0.25/
+-rw-rw-rw-   0        0        0     1148 2023-08-05 00:13:34.000000 adbkit-0.25/LICENSE.rst
+-rw-rw-rw-   0        0        0       89 2023-08-05 00:13:32.000000 adbkit-0.25/MANIFEST.in
+-rw-rw-rw-   0        0        0   164625 2023-08-05 00:14:10.889390 adbkit-0.25/PKG-INFO
+-rw-rw-rw-   0        0        0   162899 2023-08-03 05:04:50.000000 adbkit-0.25/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 00:14:10.884521 adbkit-0.25/adbkit/
+-rw-rw-rw-   0        0        0   162899 2023-08-03 05:04:50.000000 adbkit-0.25/adbkit/README.MD
+-rw-rw-rw-   0        0        0   132801 2023-08-05 00:12:10.000000 adbkit-0.25/adbkit/__init__.py
+-rw-rw-rw-   0        0        0      696 2023-08-05 00:14:09.000000 adbkit-0.25/adbkit/requirements.txt
+-rw-rw-rw-   0        0        0   284867 2023-08-05 00:14:09.000000 adbkit-0.25/adbkit/thirdparty.json
+drwxrwxrwx   0        0        0        0 2023-08-05 00:14:10.887447 adbkit-0.25/adbkit.egg-info/
+-rw-rw-rw-   0        0        0   164625 2023-08-05 00:14:10.000000 adbkit-0.25/adbkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      284 2023-08-05 00:14:10.000000 adbkit-0.25/adbkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 00:14:10.000000 adbkit-0.25/adbkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      660 2023-08-05 00:14:10.000000 adbkit-0.25/adbkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 00:14:10.000000 adbkit-0.25/adbkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       85 2023-08-05 00:14:10.890375 adbkit-0.25/setup.cfg
+-rw-rw-rw-   0        0        0     2803 2023-08-05 00:14:09.000000 adbkit-0.25/setup.py
```

### Comparing `adbkit-0.24/LICENSE.rst` & `adbkit-0.25/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `adbkit-0.24/PKG-INFO` & `adbkit-0.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.24
+Version: 0.25
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adbkit-0.24/README.md` & `adbkit-0.25/README.md`

 * *Files identical despite different names*

### Comparing `adbkit-0.24/adbkit/README.MD` & `adbkit-0.25/adbkit/README.MD`

 * *Files identical despite different names*

### Comparing `adbkit-0.24/adbkit/__init__.py` & `adbkit-0.25/adbkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,26 +353,39 @@
             for x in regex.findall(rb"cur=(\d{,4}x\d{,4}\b)", p.stdout)[0]
             .lower()
             .split(b"x")
         ]
         print(screenheight, screenwidth)
 
     except Exception:
-        screenwidth, screenheight = (
-            subprocess.run(
-                rf'{adb_path} -s {deviceserial} shell dumpsys window | grep cur= |tr -s " " | cut -d " " -f 4|cut -d "=" -f 2',
-                shell=True,
-                capture_output=True,
-                **invisibledict,
+        try:
+            screenwidth, screenheight = (
+                subprocess.run(
+                    rf'{adb_path} -s {deviceserial} shell dumpsys window | grep cur= |tr -s " " | cut -d " " -f 4|cut -d "=" -f 2',
+                    shell=True,
+                    capture_output=True,
+                    **invisibledict,
+                )
+                .stdout.decode("utf-8", "ignore")
+                .strip()
+                .split("x")
             )
-            .stdout.decode("utf-8", "ignore")
-            .strip()
-            .split("x")
-        )
-        screenwidth, screenheight = int(screenwidth), int(screenheight)
+            screenwidth, screenheight = int(screenwidth), int(screenheight)
+        except Exception as fe:
+            screenshot=_get_n_adb_screenshots(
+                adb_path,
+                deviceserial,
+                sleeptime=None,
+                n=1,
+                gray=False,
+                ADAPTIVE_THRESH_MEAN_C=False,
+                ADAPTIVE_THRESH_GAUSSIAN_C=False,
+                THRESH_OTSU=False,
+            )
+            screenwidth, screenheight=next(screenshot).shape[:2][::-1]
     return screenwidth, screenheight
 
 
 def convert_to_ADAPTIVE_THRESH_MEAN_C(im):
     try:
         ima2 = cv2.adaptiveThreshold(
             open_image_in_cv(im, channels_in_output=2),
@@ -697,15 +710,15 @@
         subcommands=subcommands,
         exit_keys=exit_keys,
         print_output=print_output,
     )
 
 
 def adb_open_shell(adb_path, deviceserial):
-    subprocess.run(f"start cmd /k {adb_path} -s {deviceserial} shell", shell=True)
+    subprocess.run(f"start cmd /k \"{adb_path}\" -s {deviceserial} shell", shell=True)
 
 
 def adb_swipe(
     adb_path,
     deviceserial,
     x0,
     y0,
@@ -3946,28 +3959,15 @@
             THRESH_OTSU=THRESH_OTSU,
         )
 
     def aa_path_exists(self, path):
         return adb_path_exists(self.adb_path, self.deviceserial, path)
 
     def aa_get_screen_resolution(self):
-        try:
-            return get_screen_height_width(self.adb_path, self.deviceserial)
-        except Exception:
-            screenshot=_get_n_adb_screenshots(
-                self.adb_path,
-                self.deviceserial,
-                sleeptime=None,
-                n=1,
-                gray=False,
-                ADAPTIVE_THRESH_MEAN_C=False,
-                ADAPTIVE_THRESH_GAUSSIAN_C=False,
-                THRESH_OTSU=False,
-            )
-            return screenshot.shape[:2][::-1]
+        return get_screen_height_width(self.adb_path, self.deviceserial)
 
     def aa_connect_to_device(self):
         connect_to_adb(self.adb_path, self.deviceserial)
 
     def aa_restart_server(self, killadb=True):
         self.aa_kill_server()
         sleep(2)
```

### Comparing `adbkit-0.24/adbkit/requirements.txt` & `adbkit-0.25/adbkit/requirements.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.24/adbkit/thirdparty.json` & `adbkit-0.25/adbkit/thirdparty.json`

 * *Files identical despite different names*

### Comparing `adbkit-0.24/adbkit.egg-info/PKG-INFO` & `adbkit-0.25/adbkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adbkit
-Version: 0.24
+Version: 0.25
 Summary: Big automation package for ADB
 Home-page: https://github.com/hansalemaos/adbkit
 Author: Johannes Fischer
 Author-email: aulasparticularesdealemaosp@gmail.com
 License: MIT
 Keywords: adb,android,automation,shell,root
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adbkit-0.24/adbkit.egg-info/requires.txt` & `adbkit-0.25/adbkit.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `adbkit-0.24/setup.py` & `adbkit-0.25/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 with open(os.path.join(os.path.abspath(os.path.dirname(__file__)),'README.md'), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()\
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 #long_description = (this_directory / "README.md").read_text()
 
-VERSION = '''0.24'''
+VERSION = '''0.25'''
 DESCRIPTION = '''Big automation package for ADB'''
 
 # Setting up
 setup(
     name="adbkit",
     version=VERSION,
     license='MIT',
```

