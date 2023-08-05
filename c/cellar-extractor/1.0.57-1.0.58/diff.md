# Comparing `tmp/cellar_extractor-1.0.57.tar.gz` & `tmp/cellar_extractor-1.0.58.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cellar_extractor-1.0.57.tar", last modified: Sat Aug  5 16:11:38 2023, max compression
+gzip compressed data, was "cellar_extractor-1.0.58.tar", last modified: Sat Aug  5 16:20:56 2023, max compression
```

## Comparing `cellar_extractor-1.0.57.tar` & `cellar_extractor-1.0.58.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 16:11:38.708184 cellar_extractor-1.0.57/
--rw-rw-rw-   0        0        0     7765 2023-08-05 16:11:38.707183 cellar_extractor-1.0.57/PKG-INFO
--rw-rw-rw-   0        0        0     7318 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 16:11:38.697672 cellar_extractor-1.0.57/cellar_extractor/
--rw-rw-rw-   0        0        0      709 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/Testing_file.py
--rw-rw-rw-   0        0        0      224 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/__init__.py
--rw-rw-rw-   0        0        0     3759 2023-08-05 16:11:32.000000 cellar_extractor-1.0.57/cellar_extractor/cellar.py
--rw-rw-rw-   0        0        0     1005 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/cellar_extra_extract.py
--rw-rw-rw-   0        0        0     5227 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/cellar_queries.py
--rw-rw-rw-   0        0        0    11308 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/citations_adder.py
--rw-rw-rw-   0        0        0     1355 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/csv_extractor.py
--rw-rw-rw-   0        0        0    16726 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/eurlex_scraping.py
--rw-rw-rw-   0        0        0     6477 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/fulltext_saving.py
--rw-rw-rw-   0        0        0     5411 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/json_to_csv.py
--rw-rw-rw-   0        0        0     1145 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/nodes_and_edges.py
--rw-rw-rw-   0        0        0     6834 2023-08-05 16:07:39.000000 cellar_extractor-1.0.57/cellar_extractor/sparql.py
-drwxrwxrwx   0        0        0        0 2023-08-05 16:11:38.705183 cellar_extractor-1.0.57/cellar_extractor.egg-info/
--rw-rw-rw-   0        0        0     7765 2023-08-05 16:11:38.000000 cellar_extractor-1.0.57/cellar_extractor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2023-08-05 16:11:38.000000 cellar_extractor-1.0.57/cellar_extractor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 16:11:38.000000 cellar_extractor-1.0.57/cellar_extractor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-08-05 16:11:38.000000 cellar_extractor-1.0.57/cellar_extractor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-08-05 16:11:38.000000 cellar_extractor-1.0.57/cellar_extractor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 16:11:38.708184 cellar_extractor-1.0.57/setup.cfg
--rw-rw-rw-   0        0        0      974 2023-08-05 16:11:32.000000 cellar_extractor-1.0.57/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:20:56.175376 cellar_extractor-1.0.58/
+-rw-rw-rw-   0        0        0     7765 2023-08-05 16:20:56.173376 cellar_extractor-1.0.58/PKG-INFO
+-rw-rw-rw-   0        0        0     7318 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 16:20:56.164376 cellar_extractor-1.0.58/cellar_extractor/
+-rw-rw-rw-   0        0        0      700 2023-08-05 16:18:25.000000 cellar_extractor-1.0.58/cellar_extractor/Testing_file.py
+-rw-rw-rw-   0        0        0      224 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/__init__.py
+-rw-rw-rw-   0        0        0     3768 2023-08-05 16:20:52.000000 cellar_extractor-1.0.58/cellar_extractor/cellar.py
+-rw-rw-rw-   0        0        0     1005 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/cellar_extra_extract.py
+-rw-rw-rw-   0        0        0     5227 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/cellar_queries.py
+-rw-rw-rw-   0        0        0    11308 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/citations_adder.py
+-rw-rw-rw-   0        0        0     1355 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/csv_extractor.py
+-rw-rw-rw-   0        0        0    16726 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/eurlex_scraping.py
+-rw-rw-rw-   0        0        0     6477 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/fulltext_saving.py
+-rw-rw-rw-   0        0        0     5411 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/json_to_csv.py
+-rw-rw-rw-   0        0        0     1145 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/nodes_and_edges.py
+-rw-rw-rw-   0        0        0     6834 2023-08-05 16:07:39.000000 cellar_extractor-1.0.58/cellar_extractor/sparql.py
+drwxrwxrwx   0        0        0        0 2023-08-05 16:20:56.172377 cellar_extractor-1.0.58/cellar_extractor.egg-info/
+-rw-rw-rw-   0        0        0     7765 2023-08-05 16:20:56.000000 cellar_extractor-1.0.58/cellar_extractor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2023-08-05 16:20:56.000000 cellar_extractor-1.0.58/cellar_extractor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 16:20:56.000000 cellar_extractor-1.0.58/cellar_extractor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-05 16:20:56.000000 cellar_extractor-1.0.58/cellar_extractor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-08-05 16:20:56.000000 cellar_extractor-1.0.58/cellar_extractor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 16:20:56.175376 cellar_extractor-1.0.58/setup.cfg
+-rw-rw-rw-   0        0        0      974 2023-08-05 16:20:52.000000 cellar_extractor-1.0.58/setup.py
```

### Comparing `cellar_extractor-1.0.57/PKG-INFO` & `cellar_extractor-1.0.58/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar_extractor
-Version: 1.0.57
+Version: 1.0.58
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
-Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.57 Summary: Library
+Metadata-Version: 2.1 Name: cellar_extractor Version: 1.0.58 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.57/README.md` & `cellar_extractor-1.0.58/README.md`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/Testing_file.py` & `cellar_extractor-1.0.58/cellar_extractor/Testing_file.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,11 +20,11 @@
 
 if __name__ == '__main__':
    celex = "62004CJ0292"
    site = get_entire_page(celex)
    text = get_full_text_from_html(site)
    cits = get_citations_with_extra_info(text)
    print(cits)
-   data,d2 = get_cellar_extra(sd='2023-01-01',max_ecli=100,save_file='n')
+   data = get_cellar(sd='2023-01-01',max_ecli=100,save_file='n')
    d3 = filter_subject_matter(data, "prices")
    b=2
    pass
```

### Comparing `cellar_extractor-1.0.57/cellar_extractor/cellar.py` & `cellar_extractor-1.0.58/cellar_extractor/cellar.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,13 +87,13 @@
 
 
 def filter_subject_matter(df=None, phrase=None):
     if df is None or phrase is None:
         print("Incorrect input values! \n Returning... \n")
     else:
         try:
-            mask = df["LEGAL RESOURCE IS ABOUT SUBJECT MATTER"].str.lower().str.contains(phrase,na=False)
+            mask = df["LEGAL RESOURCE IS ABOUT SUBJECT MATTER"].str.lower().str.contains(phrase.lower(), na=False)
             return df[mask]
         except Exception as e:
             print(e)
             print("Something went wrong!\n Returning... \n")
             return None
```

### Comparing `cellar_extractor-1.0.57/cellar_extractor/cellar_extra_extract.py` & `cellar_extractor-1.0.58/cellar_extractor/cellar_extra_extract.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/cellar_queries.py` & `cellar_extractor-1.0.58/cellar_extractor/cellar_queries.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/citations_adder.py` & `cellar_extractor-1.0.58/cellar_extractor/citations_adder.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/csv_extractor.py` & `cellar_extractor-1.0.58/cellar_extractor/csv_extractor.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/eurlex_scraping.py` & `cellar_extractor-1.0.58/cellar_extractor/eurlex_scraping.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/fulltext_saving.py` & `cellar_extractor-1.0.58/cellar_extractor/fulltext_saving.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/json_to_csv.py` & `cellar_extractor-1.0.58/cellar_extractor/json_to_csv.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/nodes_and_edges.py` & `cellar_extractor-1.0.58/cellar_extractor/nodes_and_edges.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor/sparql.py` & `cellar_extractor-1.0.58/cellar_extractor/sparql.py`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/cellar_extractor.egg-info/PKG-INFO` & `cellar_extractor-1.0.58/cellar_extractor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellar-extractor
-Version: 1.0.57
+Version: 1.0.58
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
-Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.57 Summary: Library
+Metadata-Version: 2.1 Name: cellar-extractor Version: 1.0.58 Summary: Library
 for extracting cellar data Author: LawTech Lab Author-email:
 p.lewandowski@student.maastrichtuniversity.nl License: MIT Project-URL: Bug
 Tracker, https://github.com/maastrichtlawtech/extraction_libraries Project-URL:
 Build Source, https://github.com/maastrichtlawtech/extraction_libraries
 Keywords: cellar,extractor Description-Content-Type: text/markdown ## Cellar
 extractor This library contains two functions to get cellar case law data from
 eurlex. ## Version Python 3.9 ## Contributors
```

### Comparing `cellar_extractor-1.0.57/cellar_extractor.egg-info/SOURCES.txt` & `cellar_extractor-1.0.58/cellar_extractor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellar_extractor-1.0.57/setup.py` & `cellar_extractor-1.0.58/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 p = Path("README.md")
 long_descr = p.read_text()
 
 setup(
     name='cellar_extractor',
     packages=find_packages(include=['cellar_extractor']),
-    version='1.0.57',
+    version='1.0.58',
     description='Library for extracting cellar data',
     author='LawTech Lab',
     license='MIT',
     install_requires=['bs4','SPARQLWrapper==2.0.0', 'requests==2.26.0', 'pandas','lxml==4.6.3','xmltodict==0.13.0','tqdm'],
     author_email='p.lewandowski@student.maastrichtuniversity.nl',
     keywords=['cellar', 'extractor'],
     long_description=long_descr,
```

