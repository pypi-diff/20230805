# Comparing `tmp/autoevals-0.0.6.tar.gz` & `tmp/autoevals-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autoevals-0.0.6.tar", last modified: Wed Jul 26 00:11:50 2023, max compression
+gzip compressed data, was "autoevals-0.0.7.tar", last modified: Wed Jul 26 00:12:32 2023, max compression
```

## Comparing `autoevals-0.0.6.tar` & `autoevals-0.0.7.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.881888 autoevals-0.0.6/
--rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-24 12:02:52.000000 autoevals-0.0.6/LICENSE
--rw-r--r--   0 ankur      (501) staff       (20)       30 2023-07-25 10:30:28.000000 autoevals-0.0.6/MANIFEST.in
--rw-r--r--   0 ankur      (501) staff       (20)     5426 2023-07-26 00:11:50.881772 autoevals-0.0.6/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)     4908 2023-07-26 00:11:49.000000 autoevals-0.0.6/README.md
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.878142 autoevals-0.0.6/py/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.880043 autoevals-0.0.6/py/autoevals/
--rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1506 2023-07-25 12:23:28.000000 autoevals-0.0.6/py/autoevals/base.py
--rw-r--r--   0 ankur      (501) staff       (20)     7383 2023-07-25 12:33:25.000000 autoevals-0.0.6/py/autoevals/llm.py
--rw-r--r--   0 ankur      (501) staff       (20)     1866 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)      612 2023-07-25 12:23:44.000000 autoevals-0.0.6/py/autoevals/string.py
--rw-r--r--   0 ankur      (501) staff       (20)     5132 2023-07-25 12:28:11.000000 autoevals-0.0.6/py/autoevals/test_llm.py
--rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/test_string.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-25 10:30:28.000000 autoevals-0.0.6/py/autoevals/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-25 10:30:45.000000 autoevals-0.0.6/py/autoevals/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.880599 autoevals-0.0.6/py/autoevals.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)     5426 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      651 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)      259 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-26 00:11:50.000000 autoevals-0.0.6/py/autoevals.egg-info/top_level.txt
--rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-24 12:02:52.000000 autoevals-0.0.6/pyproject.toml
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-26 00:11:50.881926 autoevals-0.0.6/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1575 2023-07-25 10:30:28.000000 autoevals-0.0.6/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:11:50.881622 autoevals-0.0.6/templates/
--rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/battle.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/closed_q_a.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/factuality.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/humor.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/possible.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/security.yaml
--rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/sql.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/summary.yaml
--rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-25 10:30:28.000000 autoevals-0.0.6/templates/translation.yaml
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:12:32.022911 autoevals-0.0.7/
+-rw-r--r--   0 ankur      (501) staff       (20)     1072 2023-07-24 12:02:52.000000 autoevals-0.0.7/LICENSE
+-rw-r--r--   0 ankur      (501) staff       (20)       30 2023-07-25 10:30:28.000000 autoevals-0.0.7/MANIFEST.in
+-rw-r--r--   0 ankur      (501) staff       (20)     5426 2023-07-26 00:12:32.022783 autoevals-0.0.7/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)     4908 2023-07-26 00:12:30.000000 autoevals-0.0.7/README.md
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:12:32.019187 autoevals-0.0.7/py/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:12:32.020884 autoevals-0.0.7/py/autoevals/
+-rw-r--r--   0 ankur      (501) staff       (20)       61 2023-07-25 10:30:28.000000 autoevals-0.0.7/py/autoevals/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1506 2023-07-25 12:23:28.000000 autoevals-0.0.7/py/autoevals/base.py
+-rw-r--r--   0 ankur      (501) staff       (20)     7383 2023-07-25 12:33:25.000000 autoevals-0.0.7/py/autoevals/llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1866 2023-07-25 10:30:28.000000 autoevals-0.0.7/py/autoevals/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)      612 2023-07-25 12:23:44.000000 autoevals-0.0.7/py/autoevals/string.py
+-rw-r--r--   0 ankur      (501) staff       (20)     5132 2023-07-25 12:28:11.000000 autoevals-0.0.7/py/autoevals/test_llm.py
+-rw-r--r--   0 ankur      (501) staff       (20)      546 2023-07-25 10:30:28.000000 autoevals-0.0.7/py/autoevals/test_string.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-07-25 10:30:28.000000 autoevals-0.0.7/py/autoevals/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-07-26 00:12:24.000000 autoevals-0.0.7/py/autoevals/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:12:32.021557 autoevals-0.0.7/py/autoevals.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)     5426 2023-07-26 00:12:32.000000 autoevals-0.0.7/py/autoevals.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      651 2023-07-26 00:12:32.000000 autoevals-0.0.7/py/autoevals.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-07-26 00:12:32.000000 autoevals-0.0.7/py/autoevals.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      259 2023-07-26 00:12:32.000000 autoevals-0.0.7/py/autoevals.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       10 2023-07-26 00:12:32.000000 autoevals-0.0.7/py/autoevals.egg-info/top_level.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       31 2023-07-24 12:02:52.000000 autoevals-0.0.7/pyproject.toml
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-07-26 00:12:32.022945 autoevals-0.0.7/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1575 2023-07-25 10:30:28.000000 autoevals-0.0.7/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-07-26 00:12:32.022628 autoevals-0.0.7/templates/
+-rw-r--r--   0 ankur      (501) staff       (20)      355 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/battle.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      312 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/closed_q_a.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1121 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/factuality.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      107 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/humor.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      636 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/possible.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      109 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/security.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)     1076 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/sql.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      356 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/summary.yaml
+-rw-r--r--   0 ankur      (501) staff       (20)      683 2023-07-25 10:30:28.000000 autoevals-0.0.7/templates/translation.yaml
```

### Comparing `autoevals-0.0.6/LICENSE` & `autoevals-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/PKG-INFO` & `autoevals-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.6
+Version: 0.0.7
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.6/README.md` & `autoevals-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals/base.py` & `autoevals-0.0.7/py/autoevals/base.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals/llm.py` & `autoevals-0.0.7/py/autoevals/llm.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals/oai.py` & `autoevals-0.0.7/py/autoevals/oai.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals/string.py` & `autoevals-0.0.7/py/autoevals/string.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals/test_llm.py` & `autoevals-0.0.7/py/autoevals/test_llm.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals/test_string.py` & `autoevals-0.0.7/py/autoevals/test_string.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/py/autoevals.egg-info/PKG-INFO` & `autoevals-0.0.7/py/autoevals.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autoevals
-Version: 0.0.6
+Version: 0.0.7
 Summary: Universal library for evaluating AI models
 Home-page: https://www.braintrustdata.com
 Author: BrainTrust
 Author-email: info@braintrustdata.com
 Project-URL: Bug Tracker, https://github.com/braintrustdata/autoevals
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `autoevals-0.0.6/py/autoevals.egg-info/SOURCES.txt` & `autoevals-0.0.7/py/autoevals.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/setup.py` & `autoevals-0.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/templates/factuality.yaml` & `autoevals-0.0.7/templates/factuality.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/templates/possible.yaml` & `autoevals-0.0.7/templates/possible.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/templates/sql.yaml` & `autoevals-0.0.7/templates/sql.yaml`

 * *Files identical despite different names*

### Comparing `autoevals-0.0.6/templates/translation.yaml` & `autoevals-0.0.7/templates/translation.yaml`

 * *Files identical despite different names*

