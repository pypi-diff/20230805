# Comparing `tmp/idbadapter-1.9.7.tar.gz` & `tmp/idbadapter-1.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idbadapter-1.9.7.tar", last modified: Fri Jul 28 06:44:42 2023, max compression
+gzip compressed data, was "idbadapter-1.9.8.tar", last modified: Sat Aug  5 09:20:27 2023, max compression
```

## Comparing `idbadapter-1.9.7.tar` & `idbadapter-1.9.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 06:44:42.100642 idbadapter-1.9.7/
--rw-rw-rw-   0        0        0    11558 2023-05-15 08:54:26.000000 idbadapter-1.9.7/LICENSE
--rw-rw-rw-   0        0        0      697 2023-07-28 06:44:42.100642 idbadapter-1.9.7/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-05-15 08:54:26.000000 idbadapter-1.9.7/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 06:44:42.076857 idbadapter-1.9.7/idbadapter/
--rw-rw-rw-   0        0        0       61 2023-05-15 08:54:26.000000 idbadapter-1.9.7/idbadapter/__init__.py
--rw-rw-rw-   0        0        0    12475 2023-07-28 06:42:43.000000 idbadapter-1.9.7/idbadapter/schedule_loader.py
-drwxrwxrwx   0        0        0        0 2023-07-28 06:44:42.099563 idbadapter-1.9.7/idbadapter.egg-info/
--rw-rw-rw-   0        0        0      697 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      258 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-07-28 06:44:41.000000 idbadapter-1.9.7/idbadapter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 06:44:42.102436 idbadapter-1.9.7/setup.cfg
--rw-rw-rw-   0        0        0      991 2023-07-28 06:43:02.000000 idbadapter-1.9.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:20:27.229659 idbadapter-1.9.8/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 13:28:55.000000 idbadapter-1.9.8/LICENSE
+-rw-rw-rw-   0        0        0      697 2023-08-05 09:20:27.229659 idbadapter-1.9.8/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-05-05 13:33:15.000000 idbadapter-1.9.8/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 09:20:27.213659 idbadapter-1.9.8/idbadapter/
+-rw-rw-rw-   0        0        0       61 2023-05-22 08:18:39.000000 idbadapter-1.9.8/idbadapter/__init__.py
+-rw-rw-rw-   0        0        0    11882 2023-08-05 09:19:29.000000 idbadapter-1.9.8/idbadapter/schedule_loader.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:20:27.228659 idbadapter-1.9.8/idbadapter.egg-info/
+-rw-rw-rw-   0        0        0      697 2023-08-05 09:20:27.000000 idbadapter-1.9.8/idbadapter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      258 2023-08-05 09:20:27.000000 idbadapter-1.9.8/idbadapter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:20:27.000000 idbadapter-1.9.8/idbadapter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-08-05 09:20:27.000000 idbadapter-1.9.8/idbadapter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-05 09:20:27.000000 idbadapter-1.9.8/idbadapter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:20:27.232659 idbadapter-1.9.8/setup.cfg
+-rw-rw-rw-   0        0        0      991 2023-08-05 09:20:06.000000 idbadapter-1.9.8/setup.py
```

### Comparing `idbadapter-1.9.7/LICENSE` & `idbadapter-1.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `idbadapter-1.9.7/PKG-INFO` & `idbadapter-1.9.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.7
+Version: 1.9.8
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.7/idbadapter/schedule_loader.py` & `idbadapter-1.9.8/idbadapter/schedule_loader.py`

 * *Files 7% similar despite different names*

```diff
@@ -142,30 +142,22 @@
         
         result = response.json()
         df = pd.DataFrame(result)
         return df
     
     def get_all_works_name(self):
         query = f"""
-        select DISTINCT w.name as name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from works w
-        join work_info wi on w.id = wi.id_work 
-        join granulary_works gw on gw.id = wi.id_granulary_work 
-        join typed_lvl2_works tlw on tlw.id = wi.id_typed_lvl2_work 
-        join processed_works pn on pn.id = wi.id_processed_work"""
+        select DISTINCT name, granulary_name, typed_lvl2_name as lvl2_name, processed_name from works_names_mv"""
         
         df = self._execute_query(query)
         return df
     
     def get_all_resources_name(self):
         query = f"""
-        select DISTINCT w.name as name, gw.name as granulary_name, tlw.name as lvl2_name, pn.name as processed_name from basic_resources w
-        join resources_info wi on w.id = wi.id_resource  
-        join granulary_resources gw on gw.id = wi.id_granulary_name
-        join typed_lvl2_resources tlw on tlw.id = wi.id_typed_lvl2_name
-        join processed_resources pn on pn.id = wi.id_processed_name"""
+        select DISTINCT name, granulary_name, typed_lvl2_name as lvl2_name, processed_name from resource_names_mv"""
         df = self._execute_query(query)
         return df
 
     def get_works_by_pulls(self, work_pulls: list, resource_list: list = [], key=GRANULARY, path_to_log="empty_pull.txt", res_key=None):
         if res_key is None:
             res_key = key
         self.path_to_log = path_to_log
@@ -194,15 +186,14 @@
 
                 
             if len(resource_list) != 0:
                 query += f""" and rnm.{res_key["column"]} in ({",".join(map(lambda x: f"'{x}'", resource_list))})"""   
             try:
                 df = self._execute_query(query)
             except ValueError:
-                print(query)
                 print("jsondecodeerror occurred", pull)
                 yield None
                 continue 
 
             if df.empty:
                 with open(self.path_to_log, "a", encoding="UTF-8") as f:
                     print("pull not found", pull, file=f)
```

### Comparing `idbadapter-1.9.7/idbadapter.egg-info/PKG-INFO` & `idbadapter-1.9.8/idbadapter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idbadapter
-Version: 1.9.7
+Version: 1.9.8
 Summary: Сache module for batch loading of data
 Home-page: https://github.com/AnatolyPershinov/gpn_cache_module
 Download-URL: https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip
 Author: Anatoly Pershinov
 Author-email: anatoliypershinov@gmail.com
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `idbadapter-1.9.7/setup.py` & `idbadapter-1.9.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 #!/usr/bin/env python
 
 from distutils.core import setup
 
-version = '1.9.7'
+version = '1.9.8'
 
 long_description = "Сache module for batch loading of data"
 
 setup(name='idbadapter',
-      version='1.9.7',
+      version='1.9.8',
       description='Сache module for batch loading of data',
       long_description=long_description,
       url="https://github.com/AnatolyPershinov/gpn_cache_module",
       download_url='https://github.com/AnatolyPershinov/gpn_cache_module/archive/master.zip',
       author='Anatoly Pershinov',
       author_email='anatoliypershinov@gmail.com',
       packages=['idbadapter'],
```

