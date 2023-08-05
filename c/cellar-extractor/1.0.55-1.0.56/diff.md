# Comparing `tmp/cellar_extractor-1.0.55.tar.gz` & `tmp/cellar_extractor-1.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.55.tar", last modified: Fri Aug  4 10:43:06 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.56.tar", last modified: Sat Aug  5 16:09:41 2023, max compression
```

## Comparing `cellar_extractor-1.0.55.tar` & `cellar_extractor-1.0.56.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 10:43:06.026636 cellar_extractor-1.0.55/
--rw-rw-rw-   0        0        0     7765 2023-08-04 10:43:06.025636 cellar_extractor-1.0.55/PKG-INFO
--rw-rw-rw-   0        0        0     7318 2023-08-04 10:40:54.000000 cellar_extractor-1.0.55/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 10:43:06.016636 cellar_extractor-1.0.55/cellar_extractor/
--rw-rw-rw-   0        0        0      709 2023-08-03 09:56:02.000000 cellar_extractor-1.0.55/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      224 2023-08-03 09:50:44.000000 cellar_extractor-1.0.55/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3688 2023-08-04 10:37:49.000000 cellar_extractor-1.0.55/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11308 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1355 2023-08-02 12:06:01.000000 cellar_extractor-1.0.55/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6477 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1145 2023-08-04 10:37:49.000000 cellar_extractor-1.0.55/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2023-07-31 10:47:48.000000 cellar_extractor-1.0.55/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-08-04 10:43:06.024637 cellar_extractor-1.0.55/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     7765 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-04 10:43:05.000000 cellar_extractor-1.0.55/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 10:43:06.027635 cellar_extractor-1.0.55/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-08-04 10:41:46.000000 cellar_extractor-1.0.55/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:09:41.918731 cellar_extractor-1.0.56/
+-rw-rw-rw-   0        0        0     7765 2023-08-05 16:09:41.917724 cellar_extractor-1.0.56/PKG-INFO
+-rw-rw-rw-   0        0        0     7318 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 16:09:41.907997 cellar_extractor-1.0.56/cellar_extractor/
+-rw-rw-rw-   0        0        0      709 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      224 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3750 2023-08-05 16:09:17.000000 cellar_extractor-1.0.56/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11308 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1355 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6477 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1145 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2023-08-05 16:07:39.000000 cellar_extractor-1.0.56/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:09:41.915546 cellar_extractor-1.0.56/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     7765 2023-08-05 16:09:41.000000 cellar_extractor-1.0.56/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-08-05 16:09:41.000000 cellar_extractor-1.0.56/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 16:09:41.000000 cellar_extractor-1.0.56/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-05 16:09:41.000000 cellar_extractor-1.0.56/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-05 16:09:41.000000 cellar_extractor-1.0.56/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 16:09:41.918731 cellar_extractor-1.0.56/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-08-05 16:09:37.000000 cellar_extractor-1.0.56/setup.py
```

### Comparing `cellar_extractor-1.0.55/PKG-INFO` & `cellar_extractor-1.0.56/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.55
+Version: 1.0.56
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.55 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.56 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.55/README.md` & `cellar_extractor-1.0.56/README.md`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.56/cellar_extractor/Testing_file.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/cellar.py` & `cellar_extractor-1.0.56/cellar_extractor/cellar.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,9 +89,11 @@
 def filter_subject_matter(df=None, phrase=None):
     if df is None or phrase is None:
         print("Incorrect input values! \n Returning... \n")
     else:
         try:
             mask = df["LEGAL RESOURCE IS ABOUT SUBJECT MATTER"].str.lower().str.contains(phrase)
             return df[mask]
-        except:
+        except Exception as e:
+            print(e)
             print("Something went wrong!\n Returning... \n")
+            return None
```

### Comparing `cellar_extractor-1.0.55/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.56/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.56/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.56/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.56/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.56/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.56/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.56/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.56/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor/sparql.py` & `cellar_extractor-1.0.56/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.56/cellar_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.55
+Version: 1.0.56
 Summary: Library for extracting cellar data
 Author: LawTech Lab
 Author-email: p.lewandowski@student.maastrichtuniversity.nl
 License: MIT
 Project-URL: Bug Tracker, https://github.com/maastrichtlawtech/extraction_libraries
 Project-URL: Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.55 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.56 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.55/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.56/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.55/setup.py` & `cellar_extractor-1.0.56/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.55',
+    version='1.0.56',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

