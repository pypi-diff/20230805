# Comparing `tmp/accustom-1.3.1.tar.gz` & `tmp/accustom-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accustom-1.3.1.tar", last modified: Thu Mar 16 10:17:38 2023, max compression
+gzip compressed data, was "accustom-1.3.2.tar", last modified: Thu Mar 16 12:49:53 2023, max compression
```

## Comparing `accustom-1.3.1.tar` & `accustom-1.3.2.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0    11358 2021-02-09 23:19:20.931478 accustom-1.3.1/LICENSE.txt
--rw-r--r--   0        0        0       91 2023-03-16 04:29:26.827847 accustom-1.3.1/NOTICE.txt
--rw-r--r--   0        0        0    12888 2023-03-16 04:29:26.828101 accustom-1.3.1/README.md
--rw-r--r--   0        0        0     6148 2023-03-15 14:12:46.047682 accustom-1.3.1/accustom/.DS_Store
--rw-r--r--   0        0        0      482 2023-03-15 08:55:05.350391 accustom-1.3.1/accustom/Exceptions/__init__.py
--rw-r--r--   0        0        0     1767 2023-03-14 02:53:03.638835 accustom-1.3.1/accustom/Exceptions/exceptions.py
--rw-r--r--   0        0        0      526 2023-03-15 07:24:54.382601 accustom-1.3.1/accustom/__init__.py
--rw-r--r--   0        0        0      860 2023-03-15 08:49:06.922189 accustom-1.3.1/accustom/constants.py
--rw-r--r--   0        0        0    24939 2023-03-16 06:36:13.379137 accustom-1.3.1/accustom/decorators.py
--rw-r--r--   0        0        0     9357 2023-03-16 04:29:26.828605 accustom-1.3.1/accustom/redaction.py
--rw-r--r--   0        0        0    13914 2023-03-16 06:16:19.832882 accustom-1.3.1/accustom/response.py
--rw-r--r--   0        0        0     4341 2023-03-16 10:16:02.047437 accustom-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1834 2023-03-15 14:26:09.343146 accustom-1.3.1/tests/int/Makefile
--rw-r--r--   0        0        0     1109 2023-03-16 05:06:59.959818 accustom-1.3.1/tests/int/redact.deploy.yaml
--rw-r--r--   0        0        0     1269 2023-03-15 01:46:59.010776 accustom-1.3.1/tests/int/redact.execute.yaml
--rw-r--r--   0        0        0     1326 2023-03-15 08:49:06.938288 accustom-1.3.1/tests/int/redact.py
--rw-r--r--   0        0        0     4914 2023-03-15 10:00:18.656041 accustom-1.3.1/tests/int/test_redact.py
--rw-r--r--   0        0        0     2083 2023-03-16 06:39:57.462239 accustom-1.3.1/tests/int/test_timeout.py
--rw-r--r--   0        0        0     4253 2023-03-16 05:06:59.956170 accustom-1.3.1/tests/int/timeout.deploy.yaml
--rw-r--r--   0        0        0     1158 2023-03-16 06:37:19.155490 accustom-1.3.1/tests/int/timeout.execute.yaml
--rw-r--r--   0        0        0      722 2023-03-16 06:34:52.321135 accustom-1.3.1/tests/int/timeout.py
--rw-r--r--   0        0        0     1241 2023-03-15 08:49:38.380622 accustom-1.3.1/tests/unit/test_constants.py
--rw-r--r--   0        0        0    29865 2023-03-16 04:29:26.829359 accustom-1.3.1/tests/unit/test_redaction.py
--rw-r--r--   0        0        0     4268 2023-03-16 04:29:26.829477 accustom-1.3.1/tests/unit/test_response.py
--rw-r--r--   0        0        0    13717 1970-01-01 00:00:00.000000 accustom-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11358 2021-02-09 23:19:20.931478 accustom-1.3.2/LICENSE.txt
+-rw-r--r--   0        0        0       91 2023-03-16 10:29:11.763997 accustom-1.3.2/NOTICE.txt
+-rw-r--r--   0        0        0    12888 2023-03-16 10:29:11.764889 accustom-1.3.2/README.md
+-rw-r--r--   0        0        0     6148 2023-03-15 14:12:46.047682 accustom-1.3.2/accustom/.DS_Store
+-rw-r--r--   0        0        0      482 2023-03-15 08:55:05.350391 accustom-1.3.2/accustom/Exceptions/__init__.py
+-rw-r--r--   0        0        0     1767 2023-03-14 02:53:03.638835 accustom-1.3.2/accustom/Exceptions/exceptions.py
+-rw-r--r--   0        0        0       38 2023-03-16 12:48:20.842293 accustom-1.3.2/accustom/Exceptions/py.typed
+-rw-r--r--   0        0        0      526 2023-03-15 07:24:54.382601 accustom-1.3.2/accustom/__init__.py
+-rw-r--r--   0        0        0      860 2023-03-15 08:49:06.922189 accustom-1.3.2/accustom/constants.py
+-rw-r--r--   0        0        0    24939 2023-03-16 10:29:11.766483 accustom-1.3.2/accustom/decorators.py
+-rw-r--r--   0        0        0       38 2023-03-16 12:48:20.842582 accustom-1.3.2/accustom/py.typed
+-rw-r--r--   0        0        0     9357 2023-03-16 10:29:11.767248 accustom-1.3.2/accustom/redaction.py
+-rw-r--r--   0        0        0    13914 2023-03-16 10:29:11.768146 accustom-1.3.2/accustom/response.py
+-rw-r--r--   0        0        0     4341 2023-03-16 12:48:20.843183 accustom-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1834 2023-03-15 14:26:09.343146 accustom-1.3.2/tests/int/Makefile
+-rw-r--r--   0        0        0     1109 2023-03-16 10:29:11.770897 accustom-1.3.2/tests/int/redact.deploy.yaml
+-rw-r--r--   0        0        0     1269 2023-03-15 01:46:59.010776 accustom-1.3.2/tests/int/redact.execute.yaml
+-rw-r--r--   0        0        0     1326 2023-03-15 08:49:06.938288 accustom-1.3.2/tests/int/redact.py
+-rw-r--r--   0        0        0     4914 2023-03-15 10:00:18.656041 accustom-1.3.2/tests/int/test_redact.py
+-rw-r--r--   0        0        0     2083 2023-03-16 10:29:11.771629 accustom-1.3.2/tests/int/test_timeout.py
+-rw-r--r--   0        0        0     4253 2023-03-16 10:29:11.772297 accustom-1.3.2/tests/int/timeout.deploy.yaml
+-rw-r--r--   0        0        0     1158 2023-03-16 10:29:11.772953 accustom-1.3.2/tests/int/timeout.execute.yaml
+-rw-r--r--   0        0        0      722 2023-03-16 10:29:11.773777 accustom-1.3.2/tests/int/timeout.py
+-rw-r--r--   0        0        0     1241 2023-03-15 08:49:38.380622 accustom-1.3.2/tests/unit/test_constants.py
+-rw-r--r--   0        0        0    29865 2023-03-16 10:29:11.774618 accustom-1.3.2/tests/unit/test_redaction.py
+-rw-r--r--   0        0        0     4268 2023-03-16 10:29:11.775390 accustom-1.3.2/tests/unit/test_response.py
+-rw-r--r--   0        0        0    13717 1970-01-01 00:00:00.000000 accustom-1.3.2/PKG-INFO
```

### Comparing `accustom-1.3.1/LICENSE.txt` & `accustom-1.3.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/README.md` & `accustom-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/.DS_Store` & `accustom-1.3.2/accustom/.DS_Store`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/Exceptions/exceptions.py` & `accustom-1.3.2/accustom/Exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/__init__.py` & `accustom-1.3.2/accustom/__init__.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/constants.py` & `accustom-1.3.2/accustom/constants.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/decorators.py` & `accustom-1.3.2/accustom/decorators.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/redaction.py` & `accustom-1.3.2/accustom/redaction.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/accustom/response.py` & `accustom-1.3.2/accustom/response.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/pyproject.toml` & `accustom-1.3.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "accustom"
-version = "1.3.1"
+version = "1.3.2"
 description = "Accustom is a library for responding to Custom Resources in AWS CloudFormation using the decorator pattern."
 authors = [
     { name = "Taylor Bertie", email = "bertiet@amazon.com" },
 ]
 dependencies = [
     "boto3==1.26.91",
     "botocore==1.29.91",
```

### Comparing `accustom-1.3.1/tests/int/Makefile` & `accustom-1.3.2/tests/int/Makefile`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/redact.deploy.yaml` & `accustom-1.3.2/tests/int/redact.deploy.yaml`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/redact.execute.yaml` & `accustom-1.3.2/tests/int/redact.execute.yaml`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/redact.py` & `accustom-1.3.2/tests/int/redact.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/test_redact.py` & `accustom-1.3.2/tests/int/test_redact.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/test_timeout.py` & `accustom-1.3.2/tests/int/test_timeout.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/timeout.deploy.yaml` & `accustom-1.3.2/tests/int/timeout.deploy.yaml`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/timeout.execute.yaml` & `accustom-1.3.2/tests/int/timeout.execute.yaml`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/int/timeout.py` & `accustom-1.3.2/tests/int/timeout.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/unit/test_constants.py` & `accustom-1.3.2/tests/unit/test_constants.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/unit/test_redaction.py` & `accustom-1.3.2/tests/unit/test_redaction.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/tests/unit/test_response.py` & `accustom-1.3.2/tests/unit/test_response.py`

 * *Files identical despite different names*

### Comparing `accustom-1.3.1/PKG-INFO` & `accustom-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accustom
-Version: 1.3.1
+Version: 1.3.2
 Summary: Accustom is a library for responding to Custom Resources in AWS CloudFormation using the decorator pattern.
 License: Apache-2.0
 Keywords: cloudformation,lambda,custom,resource,decorator
 Author-email: Taylor Bertie <bertiet@amazon.com>
 Requires-Python: >=3, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, <4
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

