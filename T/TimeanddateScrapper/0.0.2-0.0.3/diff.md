# Comparing `tmp/TimeanddateScrapper-0.0.2.tar.gz` & `tmp/TimeanddateScrapper-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\bibha\Desktop\PIP-2\dist\.tmp-08zqd87g\TimeanddateScrapper-0.0.2.tar", last modified: Thu Aug  3 17:21:21 2023, max compression
+gzip compressed data, was "TimeanddateScrapper-0.0.3.tar", last modified: Sat Aug  5 09:11:45 2023, max compression
```

## Comparing `TimeanddateScrapper-0.0.2.tar` & `TimeanddateScrapper-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/
--rw-rw-rw-   0        0        0     1671 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1045 2023-08-03 17:20:07.000000 TimeanddateScrapper-0.0.2/README.md
--rw-rw-rw-   0        0        0      103 2023-08-03 17:14:48.000000 TimeanddateScrapper-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      767 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper/
--rw-rw-rw-   0        0        0        0 2023-08-03 15:43:16.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper/__init__.py
--rw-rw-rw-   0        0        0     1690 2023-08-03 17:16:56.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper/worldweather.py
-drwxrwxrwx   0        0        0        0 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper.egg-info/
--rw-rw-rw-   0        0        0     1671 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      298 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2023-08-03 17:21:21.000000 TimeanddateScrapper-0.0.2/src/TimeanddateScrapper.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 09:11:45.025449 TimeanddateScrapper-0.0.3/
+-rw-rw-rw-   0        0        0     1775 2023-08-05 09:11:45.026447 TimeanddateScrapper-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1144 2023-08-05 09:06:00.000000 TimeanddateScrapper-0.0.3/README.md
+-rw-rw-rw-   0        0        0      103 2023-08-03 17:14:48.000000 TimeanddateScrapper-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      767 2023-08-05 09:11:45.028447 TimeanddateScrapper-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 09:11:44.996938 TimeanddateScrapper-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 09:11:45.002923 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper/
+-rw-rw-rw-   0        0        0        0 2023-08-03 15:43:16.000000 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper/__init__.py
+-rw-rw-rw-   0        0        0     1737 2023-08-05 09:07:28.000000 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper/worldweather.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:11:45.024446 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper.egg-info/
+-rw-rw-rw-   0        0        0     1775 2023-08-05 09:11:44.000000 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      298 2023-08-05 09:11:44.000000 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:11:44.000000 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-08-05 09:11:44.000000 TimeanddateScrapper-0.0.3/src/TimeanddateScrapper.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `TimeanddateScrapper-0.0.2/PKG-INFO` & `TimeanddateScrapper-0.0.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeanddateScrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Weather Data Scrap Application extracts weather data from the popular website timeanddate.com.
 Home-page: https://github.com/Bibhash7/Weather-Data-Scrap-WWDS
 Author: Bibhash Ghosh
 Author-email: bibhashghosh994@gmail.com
 Project-URL: Bug Tracker, https://github.com/Bibhash7/Weather-Data-Scrap-WWDS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -27,9 +27,13 @@
 ## Functionalities:
 ### worldWideReport(): 
 This Generates the world wide weather reports in list format.
 
 ### saveToExcel(): 
 This Generates the world wide weather reports in an excel sheet.
 
-### Imports
-import TimeanddateScrapper
+### Example
+
+    from TimeanddateScrapper.worldweather import Weather
+    w = Weather()
+    print(w.worldWideReport())
+    w.saveToExcel()
```

### Comparing `TimeanddateScrapper-0.0.2/README.md` & `TimeanddateScrapper-0.0.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -13,9 +13,13 @@
 ## Functionalities:
 ### worldWideReport(): 
 This Generates the world wide weather reports in list format.
 
 ### saveToExcel(): 
 This Generates the world wide weather reports in an excel sheet.
 
-### Imports
-import TimeanddateScrapper
+### Example
+
+    from TimeanddateScrapper.worldweather import Weather
+    w = Weather()
+    print(w.worldWideReport())
+    w.saveToExcel()
```

### Comparing `TimeanddateScrapper-0.0.2/setup.cfg` & `TimeanddateScrapper-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2054 696d 6561 6e64 6461 7465 5363   = TimeanddateSc
 00000020: 7261 7070 6572 0d0a 7665 7273 696f 6e20  rapper..version 
-00000030: 3d20 302e 302e 320d 0a61 7574 686f 7220  = 0.0.2..author 
+00000030: 3d20 302e 302e 330d 0a61 7574 686f 7220  = 0.0.3..author 
 00000040: 3d20 4269 6268 6173 6820 4768 6f73 680d  = Bibhash Ghosh.
 00000050: 0a61 7574 686f 725f 656d 6169 6c20 3d20  .author_email = 
 00000060: 6269 6268 6173 6867 686f 7368 3939 3440  bibhashghosh994@
 00000070: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000080: 6970 7469 6f6e 203d 2054 6865 2057 6561  iption = The Wea
 00000090: 7468 6572 2044 6174 6120 5363 7261 7020  ther Data Scrap 
 000000a0: 4170 706c 6963 6174 696f 6e20 6578 7472  Application extr
```

### Comparing `TimeanddateScrapper-0.0.2/src/TimeanddateScrapper.egg-info/PKG-INFO` & `TimeanddateScrapper-0.0.3/src/TimeanddateScrapper.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TimeanddateScrapper
-Version: 0.0.2
+Version: 0.0.3
 Summary: The Weather Data Scrap Application extracts weather data from the popular website timeanddate.com.
 Home-page: https://github.com/Bibhash7/Weather-Data-Scrap-WWDS
 Author: Bibhash Ghosh
 Author-email: bibhashghosh994@gmail.com
 Project-URL: Bug Tracker, https://github.com/Bibhash7/Weather-Data-Scrap-WWDS/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -27,9 +27,13 @@
 ## Functionalities:
 ### worldWideReport(): 
 This Generates the world wide weather reports in list format.
 
 ### saveToExcel(): 
 This Generates the world wide weather reports in an excel sheet.
 
-### Imports
-import TimeanddateScrapper
+### Example
+
+    from TimeanddateScrapper.worldweather import Weather
+    w = Weather()
+    print(w.worldWideReport())
+    w.saveToExcel()
```

