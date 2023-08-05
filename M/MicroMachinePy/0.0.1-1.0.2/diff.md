# Comparing `tmp/MicroMachinePy-0.0.1.tar.gz` & `tmp/MicroMachinePy-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicroMachinePy-0.0.1.tar", last modified: Fri Aug  4 16:26:58 2023, max compression
+gzip compressed data, was "MicroMachinePy-1.0.2.tar", last modified: Sat Aug  5 17:05:52 2023, max compression
```

## Comparing `MicroMachinePy-0.0.1.tar` & `MicroMachinePy-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 16:26:58.338273 MicroMachinePy-0.0.1/
--rw-rw-rw-   0        0        0     1061 2023-08-04 16:17:56.000000 MicroMachinePy-0.0.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-08-04 16:26:58.332288 MicroMachinePy-0.0.1/MicroMachinePy.egg-info/
--rw-rw-rw-   0        0        0      656 2023-08-04 16:26:58.000000 MicroMachinePy-0.0.1/MicroMachinePy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      168 2023-08-04 16:26:58.000000 MicroMachinePy-0.0.1/MicroMachinePy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:26:58.000000 MicroMachinePy-0.0.1/MicroMachinePy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 16:26:58.000000 MicroMachinePy-0.0.1/MicroMachinePy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      656 2023-08-04 16:26:58.336278 MicroMachinePy-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 16:26:58.338273 MicroMachinePy-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      958 2023-08-04 16:23:24.000000 MicroMachinePy-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 17:05:52.060566 MicroMachinePy-1.0.2/
+-rw-rw-rw-   0        0        0     1084 2023-08-05 17:05:08.000000 MicroMachinePy-1.0.2/LICENSE
+drwxrwxrwx   0        0        0        0 2023-08-05 17:05:52.056572 MicroMachinePy-1.0.2/MicroMachinePy.egg-info/
+-rw-rw-rw-   0        0        0      629 2023-08-05 17:05:51.000000 MicroMachinePy-1.0.2/MicroMachinePy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      168 2023-08-05 17:05:51.000000 MicroMachinePy-1.0.2/MicroMachinePy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 17:05:51.000000 MicroMachinePy-1.0.2/MicroMachinePy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 17:05:51.000000 MicroMachinePy-1.0.2/MicroMachinePy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      629 2023-08-05 17:05:52.059564 MicroMachinePy-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-05 17:05:52.060566 MicroMachinePy-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      928 2023-08-05 17:04:29.000000 MicroMachinePy-1.0.2/setup.py
```

### Comparing `MicroMachinePy-0.0.1/MicroMachinePy.egg-info/PKG-INFO` & `MicroMachinePy-1.0.2/MicroMachinePy.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: MicroMachinePy
-Version: 0.0.1
-Summary: MicroMachinePy
+Version: 1.0.2
+Summary: MicroPythonPy
 Author: HarshPro
 Author-email: patidarharsh16122008@gmail.com
-Keywords: Machine learning,ESP32,RASPBERRY PI,ARDUINO,Micro python,MachinePy
+Keywords: MACHINE LEARNING,ESP32,RASPBERRY PI,ARDUINO,MicroMachinePy
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package for Machine learning on ESP32, RASPBERRY PI, ARDUINO and many more
+A package for MACHINE LEARNING and using with micro python
```

### Comparing `MicroMachinePy-0.0.1/PKG-INFO` & `MicroMachinePy-1.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: MicroMachinePy
-Version: 0.0.1
-Summary: MicroMachinePy
+Version: 1.0.2
+Summary: MicroPythonPy
 Author: HarshPro
 Author-email: patidarharsh16122008@gmail.com
-Keywords: Machine learning,ESP32,RASPBERRY PI,ARDUINO,Micro python,MachinePy
+Keywords: MACHINE LEARNING,ESP32,RASPBERRY PI,ARDUINO,MicroMachinePy
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-A package for Machine learning on ESP32, RASPBERRY PI, ARDUINO and many more
+A package for MACHINE LEARNING and using with micro python
```

### Comparing `MicroMachinePy-0.0.1/setup.py` & `MicroMachinePy-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
-DESCRIPTION = 'MicroMachinePy'
-LONG_DESCRIPTION = 'A package for Machine learning on ESP32, RASPBERRY PI, ARDUINO and many more'
+VERSION = '1.0.2'
+DESCRIPTION = 'MicroPythonPy'
+LONG_DESCRIPTION = 'A package for MACHINE LEARNING and using with micro python'
 
 # Setting up
 setup(
     name="MicroMachinePy",
     version=VERSION,
     author="HarshPro",
     author_email="patidarharsh16122008@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
     install_requires=[],
-    keywords=["Machine learning", "ESP32", "RASPBERRY PI", "ARDUINO", "Micro python", "MachinePy"],
+    keywords=['MACHINE LEARNING', "ESP32", "RASPBERRY PI", "ARDUINO", "MicroMachinePy"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

