# Comparing `tmp/pk4adi-0.1.3.tar.gz` & `tmp/pk4adi-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pk4adi-0.1.3.tar", last modified: Mon Jun 19 22:54:19 2023, max compression
+gzip compressed data, was "pk4adi-0.1.4.tar", last modified: Sat Aug  5 09:44:24 2023, max compression
```

## Comparing `pk4adi-0.1.3.tar` & `pk4adi-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-19 22:54:19.977441 pk4adi-0.1.3/
--rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.3/LICENSE
--rw-rw-rw-   0        0        0     8584 2023-06-19 22:54:19.976447 pk4adi-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     7898 2023-06-19 22:53:05.000000 pk4adi-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-19 22:54:19.927774 pk4adi-0.1.3/pk4adi/
--rw-rw-rw-   0        0        0      282 2023-06-19 22:24:32.000000 pk4adi-0.1.3/pk4adi/__init__.py
--rw-rw-rw-   0        0        0     9735 2023-06-19 22:52:20.000000 pk4adi-0.1.3/pk4adi/pk.py
--rw-rw-rw-   0        0        0     8595 2023-06-19 22:52:27.000000 pk4adi-0.1.3/pk4adi/pkc.py
--rw-rw-rw-   0        0        0      968 2023-06-17 09:21:37.000000 pk4adi-0.1.3/pk4adi/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-19 22:54:19.973468 pk4adi-0.1.3/pk4adi.egg-info/
--rw-rw-rw-   0        0        0     8584 2023-06-19 22:54:19.000000 pk4adi-0.1.3/pk4adi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2023-06-19 22:54:19.000000 pk4adi-0.1.3/pk4adi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-19 22:54:19.000000 pk4adi-0.1.3/pk4adi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-19 22:54:19.000000 pk4adi-0.1.3/pk4adi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-19 22:54:19.000000 pk4adi-0.1.3/pk4adi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-19 22:54:19.978433 pk4adi-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1845 2023-06-19 08:28:36.000000 pk4adi-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:44:24.324833 pk4adi-0.1.4/
+-rw-rw-rw-   0        0        0     1088 2023-01-04 20:12:34.000000 pk4adi-0.1.4/LICENSE
+-rw-rw-rw-   0        0        0     8584 2023-08-05 09:44:24.323331 pk4adi-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     7898 2023-06-19 22:58:25.000000 pk4adi-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 09:44:24.295838 pk4adi-0.1.4/pk4adi/
+-rw-rw-rw-   0        0        0      282 2023-08-05 09:38:51.000000 pk4adi-0.1.4/pk4adi/__init__.py
+-rw-rw-rw-   0        0        0     9735 2023-06-19 22:58:25.000000 pk4adi-0.1.4/pk4adi/pk.py
+-rw-rw-rw-   0        0        0     8609 2023-08-05 09:37:53.000000 pk4adi-0.1.4/pk4adi/pkc.py
+-rw-rw-rw-   0        0        0      968 2023-06-17 09:21:37.000000 pk4adi-0.1.4/pk4adi/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:44:24.321830 pk4adi-0.1.4/pk4adi.egg-info/
+-rw-rw-rw-   0        0        0     8584 2023-08-05 09:44:24.000000 pk4adi-0.1.4/pk4adi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      237 2023-08-05 09:44:24.000000 pk4adi-0.1.4/pk4adi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:44:24.000000 pk4adi-0.1.4/pk4adi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-08-05 09:44:24.000000 pk4adi-0.1.4/pk4adi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 09:44:24.000000 pk4adi-0.1.4/pk4adi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:44:24.324833 pk4adi-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1845 2023-06-19 22:58:25.000000 pk4adi-0.1.4/setup.py
```

### Comparing `pk4adi-0.1.3/LICENSE` & `pk4adi-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.3/PKG-INFO` & `pk4adi-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pk4adi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Using PK to Measure the Performance of Anesthetic Depth Indicators.
 Home-page: https://github.com/xfz329/pk4adi.git
 Author: silencejiang
 Author-email: silencejiang@zju.edu.cn
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pk4adi-0.1.3/README.md` & `pk4adi-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.3/pk4adi/pk.py` & `pk4adi-0.1.4/pk4adi/pk.py`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.3/pk4adi/pkc.py` & `pk4adi-0.1.4/pk4adi/pkc.py`

 * *Files 1% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         current = PKmD[i]
         SumD = SumD + current
         SSD = SSD + current * current
 
     DF = n_case - 1
     PKDJ = n_case * PKD - DF / n_case * SumD
     SEDJ = math.sqrt( DF / n_case * ( SSD - 1 / n_case * SumD * SumD ))
-    TD = PKDJ / SEDJ
+    TD = float(PKDJ) / float(SEDJ)
     TP, TJ = T2P(TD, DF)
 
     # save the variables.
     ans.update({"PKmD": PKmD})
     ans.update({"SumD": SumD})
     ans.update({"SSD": SSD})
     ans.update({"DF": DF})
```

### Comparing `pk4adi-0.1.3/pk4adi/utils.py` & `pk4adi-0.1.4/pk4adi/utils.py`

 * *Files identical despite different names*

### Comparing `pk4adi-0.1.3/pk4adi.egg-info/PKG-INFO` & `pk4adi-0.1.4/pk4adi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pk4adi
-Version: 0.1.3
+Version: 0.1.4
 Summary: Using PK to Measure the Performance of Anesthetic Depth Indicators.
 Home-page: https://github.com/xfz329/pk4adi.git
 Author: silencejiang
 Author-email: silencejiang@zju.edu.cn
 License: MIT License
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pk4adi-0.1.3/setup.py` & `pk4adi-0.1.4/setup.py`

 * *Files identical despite different names*

