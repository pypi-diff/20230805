# Comparing `tmp/argos-translate-files-1.1.2.tar.gz` & `tmp/argos-translate-files-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argos-translate-files-1.1.2.tar", last modified: Sun Apr  2 16:09:52 2023, max compression
+gzip compressed data, was "argos-translate-files-1.1.3.tar", last modified: Wed May  3 06:26:41 2023, max compression
```

## Comparing `argos-translate-files-1.1.2.tar` & `argos-translate-files-1.1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/argos_translate_files.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-04-02 16:09:51.000000 argos-translate-files-1.1.2/argos_translate_files.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-02 16:09:52.000000 argos-translate-files-1.1.2/argos_translate_files.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:09:51.000000 argos-translate-files-1.1.2/argos_translate_files.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-04-02 16:09:51.000000 argos-translate-files-1.1.2/argos_translate_files.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-02 16:09:51.000000 argos-translate-files-1.1.2/argos_translate_files.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/argostranslatefiles/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/abstract_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/argostranslatefiles.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/argostranslatefiles/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/abstract_xml.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/epub.py
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/html.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/argostranslatefiles/formats/opendocument/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/opendocument/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/opendocument/odp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/opendocument/odt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/argostranslatefiles/formats/openxml/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/openxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/openxml/docx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/openxml/pptx.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/argostranslatefiles/formats/txt.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:52.050744 argos-translate-files-1.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-02 16:09:36.000000 argos-translate-files-1.1.2/tests/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.440349 argos-translate-files-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 06:26:41.440349 argos-translate-files-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.436349 argos-translate-files-1.1.3/argos_translate_files.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-05-03 06:26:41.000000 argos-translate-files-1.1.3/argos_translate_files.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-05-03 06:26:41.000000 argos-translate-files-1.1.3/argos_translate_files.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:26:41.000000 argos-translate-files-1.1.3/argos_translate_files.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-03 06:26:41.000000 argos-translate-files-1.1.3/argos_translate_files.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-03 06:26:41.000000 argos-translate-files-1.1.3/argos_translate_files.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.436349 argos-translate-files-1.1.3/argostranslatefiles/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/abstract_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/argostranslatefiles.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.436349 argos-translate-files-1.1.3/argostranslatefiles/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/abstract_xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/epub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/html.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.436349 argos-translate-files-1.1.3/argostranslatefiles/formats/opendocument/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/opendocument/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/opendocument/odp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/opendocument/odt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.436349 argos-translate-files-1.1.3/argostranslatefiles/formats/openxml/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/openxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/openxml/docx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/openxml/pptx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/argostranslatefiles/formats/txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 06:26:41.440349 argos-translate-files-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:41.440349 argos-translate-files-1.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-03 06:26:27.000000 argos-translate-files-1.1.3/tests/test_init.py
```

### Comparing `argos-translate-files-1.1.2/LICENSE` & `argos-translate-files-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/PKG-INFO` & `argos-translate-files-1.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argos-translate-files
-Version: 1.1.2
+Version: 1.1.3
 Summary: Translate files with Argos Translate
 Home-page: https://www.argosopentech.com
 Author: S. Thuret
 Author-email: contact@sebastien-thuret.fr
 License: UNKNOWN
 Description: # Argos Translate Files
```

### Comparing `argos-translate-files-1.1.2/README.md` & `argos-translate-files-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argos_translate_files.egg-info/PKG-INFO` & `argos-translate-files-1.1.3/argos_translate_files.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argos-translate-files
-Version: 1.1.2
+Version: 1.1.3
 Summary: Translate files with Argos Translate
 Home-page: https://www.argosopentech.com
 Author: S. Thuret
 Author-email: contact@sebastien-thuret.fr
 License: UNKNOWN
 Description: # Argos Translate Files
```

### Comparing `argos-translate-files-1.1.2/argos_translate_files.egg-info/SOURCES.txt` & `argos-translate-files-1.1.3/argos_translate_files.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/abstract_file.py` & `argos-translate-files-1.1.3/argostranslatefiles/abstract_file.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/argostranslatefiles.py` & `argos-translate-files-1.1.3/argostranslatefiles/argostranslatefiles.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/abstract_xml.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/abstract_xml.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/epub.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/epub.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/html.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/html.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/opendocument/odt.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/opendocument/odt.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/openxml/docx.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/openxml/docx.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/openxml/pptx.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/openxml/pptx.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/argostranslatefiles/formats/txt.py` & `argos-translate-files-1.1.3/argostranslatefiles/formats/txt.py`

 * *Files identical despite different names*

### Comparing `argos-translate-files-1.1.2/setup.py` & `argos-translate-files-1.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     required_packages = f.read().splitlines()
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="argos-translate-files",
-    version="1.1.2",
+    version="1.1.3",
     description="Translate files with Argos Translate",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="S. Thuret",
     author_email="contact@sebastien-thuret.fr",
     url="https://www.argosopentech.com",
     packages=find_packages(),
```

