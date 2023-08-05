# Comparing `tmp/win32_classics-0.0.3.tar.gz` & `tmp/win32_classics-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "win32_classics-0.0.3.tar", last modified: Thu Jul 27 19:55:03 2023, max compression
+gzip compressed data, was "win32_classics-0.0.4.tar", last modified: Sat Aug  5 11:04:45 2023, max compression
```

## Comparing `win32_classics-0.0.3.tar` & `win32_classics-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-27 19:55:03.181908 win32_classics-0.0.3/
--rw-rw-rw-   0        0        0     1095 2022-09-12 12:38:00.000000 win32_classics-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      580 2023-07-27 19:55:03.180909 win32_classics-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0       40 2022-09-12 15:48:04.000000 win32_classics-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-07-27 19:55:03.182909 win32_classics-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1203 2023-07-27 19:54:30.000000 win32_classics-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:55:03.169637 win32_classics-0.0.3/win32_classics/
--rw-rw-rw-   0        0        0     1166 2023-07-27 19:54:29.000000 win32_classics-0.0.3/win32_classics/__init__.py
--rw-rw-rw-   0        0        0    17000 2023-07-27 19:45:43.000000 win32_classics-0.0.3/win32_classics/fenster_aktionen.py
-drwxrwxrwx   0        0        0        0 2023-07-27 19:55:03.178909 win32_classics-0.0.3/win32_classics.egg-info/
--rw-rw-rw-   0        0        0      580 2023-07-27 19:55:02.000000 win32_classics-0.0.3/win32_classics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      277 2023-07-27 19:55:03.000000 win32_classics-0.0.3/win32_classics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-27 19:55:02.000000 win32_classics-0.0.3/win32_classics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-07-27 19:55:02.000000 win32_classics-0.0.3/win32_classics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-27 19:55:02.000000 win32_classics-0.0.3/win32_classics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 11:04:45.552099 win32_classics-0.0.4/
+-rw-rw-rw-   0        0        0     1095 2022-09-12 12:38:00.000000 win32_classics-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0      580 2023-08-05 11:04:45.551099 win32_classics-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0       40 2022-09-12 15:48:04.000000 win32_classics-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-05 11:04:45.552099 win32_classics-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1203 2023-08-05 11:03:58.000000 win32_classics-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:04:45.539034 win32_classics-0.0.4/win32_classics/
+-rw-rw-rw-   0        0        0     1166 2023-08-05 11:04:12.000000 win32_classics-0.0.4/win32_classics/__init__.py
+-rw-rw-rw-   0        0        0    16943 2023-08-05 11:03:28.000000 win32_classics-0.0.4/win32_classics/fenster_aktionen.py
+drwxrwxrwx   0        0        0        0 2023-08-05 11:04:45.549272 win32_classics-0.0.4/win32_classics.egg-info/
+-rw-rw-rw-   0        0        0      580 2023-08-05 11:04:45.000000 win32_classics-0.0.4/win32_classics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      277 2023-08-05 11:04:45.000000 win32_classics-0.0.4/win32_classics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 11:04:45.000000 win32_classics-0.0.4/win32_classics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-08-05 11:04:45.000000 win32_classics-0.0.4/win32_classics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-05 11:04:45.000000 win32_classics-0.0.4/win32_classics.egg-info/top_level.txt
```

### Comparing `win32_classics-0.0.3/LICENSE` & `win32_classics-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `win32_classics-0.0.3/PKG-INFO` & `win32_classics-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win32_classics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simplify win32 actions
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `win32_classics-0.0.3/setup.py` & `win32_classics-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 DESCRIPTION = "Simplify win32 actions"
 
 # Setting up
 setup(
     name="win32_classics",
     version=VERSION,
     author="André Herber",
```

### Comparing `win32_classics-0.0.3/win32_classics/__init__.py` & `win32_classics-0.0.4/win32_classics/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,8 +33,8 @@
     set_window_mid_medium,
     set_window_mid_large,
     minimize_window,
     maximize_window,
     show_window_normally,
 )
 
-__version__ = "0.0.3"
+__version__ = "0.0.4"
```

### Comparing `win32_classics-0.0.3/win32_classics/fenster_aktionen.py` & `win32_classics-0.0.4/win32_classics/fenster_aktionen.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     GetWindowText,
     SetForegroundWindow,
     SetWindowPos,
     ShowWindow,
     FindWindow,
 )
 from colorful_terminal import *
-from exception_details import print_exception_details
+from exception_details import *
 
 
 def get_monitor_infos():
     mons = get_monitors()
     mons = sorted(mons, key=lambda item: item.x)
     return mons
 
@@ -57,16 +57,18 @@
         if w == None:
             w = w_
         if h == None:
             h = h_
 
     try:
         SetWindowPos(hWnd, insert_after, x, y, w, h, flag)
+        return 0
     except Exception as exc:
         title = GetWindowText(hWnd)
+        return get_exception_details_str(exc)
         # colored_print(Fore.RED + f"Fehler für '{title}':")
         # print_exception_details(exc)
 
 
 def maximize_current_window():
     hwnd = GetForegroundWindow()
     ShowWindow(hwnd, SW_MAXIMIZE)
@@ -248,32 +250,27 @@
         else:
             if acknowledge_case:
                 if title == dic["name"]:
                     result.append(dic)
             else:
                 if title.lower() == dic["name"].lower():
                     result.append(dic)
-    if len(result) == 1:
-        return result[0]
-    elif len(result) == 0:
-        return None
-    else:
-        return result
+    return result
 
 
 def get_WindowHandle_from_ExePath(
     path,
     contains: bool = False,
     pre_filter_invisible_windows: bool = True,
     acknowledge_case: bool = True,
 ) -> list[dict]:
     result = get_WindowHandle_plus_from_ExePath(
         path, contains, pre_filter_invisible_windows, acknowledge_case
     )
-    if result == None:
+    if result == None or result == []:
         return None
     try:
         return result[0]["hwnd"]
     except:
         return result["hwnd"]
```

### Comparing `win32_classics-0.0.3/win32_classics.egg-info/PKG-INFO` & `win32_classics-0.0.4/win32_classics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: win32-classics
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simplify win32 actions
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

