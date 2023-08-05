# Comparing `tmp/acdh-transkribus-utils-2.6.tar.gz` & `tmp/acdh-transkribus-utils-2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acdh-transkribus-utils-2.6.tar", last modified: Thu Jun  1 11:02:02 2023, max compression
+gzip compressed data, was "acdh-transkribus-utils-2.7.tar", last modified: Sat Aug  5 14:50:16 2023, max compression
```

## Comparing `acdh-transkribus-utils-2.6.tar` & `acdh-transkribus-utils-2.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:02:02.745729 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-01 11:02:02.000000 acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 11:02:02.749729 acdh-transkribus-utils-2.6/transkribus_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/iiif.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/mets.py
--rw-r--r--   0 runner    (1001) docker     (123)    18559 2023-06-01 11:01:52.000000 acdh-transkribus-utils-2.6/transkribus_utils/transkribus_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:16.242115 acdh-transkribus-utils-2.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-05 14:50:16.242115 acdh-transkribus-utils-2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:16.238114 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-08-05 14:50:16.000000 acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:50:16.242115 acdh-transkribus-utils-2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:16.242115 acdh-transkribus-utils-2.7/transkribus_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/transkribus_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/transkribus_utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/transkribus_utils/iiif.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/transkribus_utils/mets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18987 2023-08-05 14:50:03.000000 acdh-transkribus-utils-2.7/transkribus_utils/transkribus_utils.py
```

### Comparing `acdh-transkribus-utils-2.6/LICENSE` & `acdh-transkribus-utils-2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.6/PKG-INFO` & `acdh-transkribus-utils-2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-transkribus-utils
-Version: 2.6
+Version: 2.7
 Summary: some utility function to interact with the Transkribus-API
 Home-page: https://github.com/acdh-oeaw/acdh-transkribus-utils
 Author: Peter Andorfer, Matthias Schlögl, Carl Friedrich Haak
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Keywords: acdh-transkribus-utils
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acdh-transkribus-utils-2.6/README.md` & `acdh-transkribus-utils-2.7/README.md`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.6/acdh_transkribus_utils.egg-info/PKG-INFO` & `acdh-transkribus-utils-2.7/acdh_transkribus_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acdh-transkribus-utils
-Version: 2.6
+Version: 2.7
 Summary: some utility function to interact with the Transkribus-API
 Home-page: https://github.com/acdh-oeaw/acdh-transkribus-utils
 Author: Peter Andorfer, Matthias Schlögl, Carl Friedrich Haak
 Author-email: peter.andorfer@oeaw.ac.at
 License: MIT
 Keywords: acdh-transkribus-utils
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `acdh-transkribus-utils-2.6/setup.py` & `acdh-transkribus-utils-2.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as readme_file:
     readme = readme_file.read()
 
 
 setup(
     name="acdh-transkribus-utils",
-    version="v2.6",
+    version="v2.7",
     description="""some utility function to interact with the Transkribus-API""",
     long_description=readme,
     long_description_content_type="text/markdown",
     author="Peter Andorfer, Matthias Schlögl, Carl Friedrich Haak",
     author_email="peter.andorfer@oeaw.ac.at",
     url="https://github.com/acdh-oeaw/acdh-transkribus-utils",
     packages=[
```

### Comparing `acdh-transkribus-utils-2.6/transkribus_utils/cli.py` & `acdh-transkribus-utils-2.7/transkribus_utils/cli.py`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.6/transkribus_utils/mets.py` & `acdh-transkribus-utils-2.7/transkribus_utils/mets.py`

 * *Files identical despite different names*

### Comparing `acdh-transkribus-utils-2.6/transkribus_utils/transkribus_utils.py` & `acdh-transkribus-utils-2.7/transkribus_utils/transkribus_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -66,14 +66,23 @@
         """Helper function to list all collections
         :return: A dict with listing the collections
         """
         url = f"{self.base_url}/collections/list"
         response = requests.get(url, cookies=self.login_cookie)
         return response.json()
 
+    def filter_collections_by_name(self, filter_string):
+        """ lists all collections which names contains 'filter_string' collections
+        :param filter_string: a string the collection name should contain
+        :return: A list with all filtered the collections
+        """
+        cols = self.list_collections()
+        filtered_cols = [x for x in cols if filter_string in x["colName"]]
+        return filtered_cols
+
     def list_docs(self, col_id):
         """Helper function to list all documents in a given collection
         :param col_id: Collection ID
         :return: A dict with listing the collections
         """
         url = f"{self.base_url}/collections/{col_id}/list"
         print(url)
```

