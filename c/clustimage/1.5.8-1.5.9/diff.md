# Comparing `tmp/clustimage-1.5.8.tar.gz` & `tmp/clustimage-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clustimage-1.5.8.tar", last modified: Sat Jul  9 19:58:29 2022, max compression
+gzip compressed data, was "clustimage-1.5.9.tar", last modified: Sat Jul  9 20:28:17 2022, max compression
```

## Comparing `clustimage-1.5.8.tar` & `clustimage-1.5.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2022-07-09 19:58:29.730745 clustimage-1.5.8/
--rw-rw-rw-   0        0        0     1123 2022-05-30 07:51:51.000000 clustimage-1.5.8/LICENSE
--rw-rw-rw-   0        0        0       60 2022-05-30 07:51:51.000000 clustimage-1.5.8/MANIFEST.in
--rw-rw-rw-   0        0        0    11667 2022-07-09 19:58:29.709946 clustimage-1.5.8/PKG-INFO
--rw-rw-rw-   0        0        0    11069 2022-05-30 07:51:51.000000 clustimage-1.5.8/README.md
-drwxrwxrwx   0        0        0        0 2022-07-09 19:58:29.560321 clustimage-1.5.8/clustimage/
--rw-rw-rw-   0        0        0     2065 2022-07-09 19:58:00.000000 clustimage-1.5.8/clustimage/__init__.py
--rw-rw-rw-   0        0        0   104299 2022-07-09 19:53:51.000000 clustimage-1.5.8/clustimage/clustimage.py
--rw-rw-rw-   0        0        0    19837 2022-07-09 16:22:31.000000 clustimage-1.5.8/clustimage/examples.py
-drwxrwxrwx   0        0        0        0 2022-07-09 19:58:29.696179 clustimage-1.5.8/clustimage/tests/
--rw-rw-rw-   0        0        0        0 2022-05-30 07:51:51.000000 clustimage-1.5.8/clustimage/tests/__init__.py
--rw-rw-rw-   0        0        0     6639 2022-06-29 16:43:35.000000 clustimage-1.5.8/clustimage/tests/test_clustimage.py
-drwxrwxrwx   0        0        0        0 2022-07-09 19:58:29.706151 clustimage-1.5.8/clustimage/utils/
--rw-rw-rw-   0        0        0        0 2022-05-30 07:51:51.000000 clustimage-1.5.8/clustimage/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-09 19:58:29.665726 clustimage-1.5.8/clustimage.egg-info/
--rw-rw-rw-   0        0        0    11667 2022-07-09 19:58:28.000000 clustimage-1.5.8/clustimage.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      372 2022-07-09 19:58:29.000000 clustimage-1.5.8/clustimage.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-09 19:58:28.000000 clustimage-1.5.8/clustimage.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      166 2022-07-09 19:58:28.000000 clustimage-1.5.8/clustimage.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2022-07-09 19:58:28.000000 clustimage-1.5.8/clustimage.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-07-09 19:58:29.731749 clustimage-1.5.8/setup.cfg
--rw-rw-rw-   0        0        0     1579 2022-06-03 08:54:33.000000 clustimage-1.5.8/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-09 20:28:17.787635 clustimage-1.5.9/
+-rw-rw-rw-   0        0        0     1123 2022-05-30 07:51:51.000000 clustimage-1.5.9/LICENSE
+-rw-rw-rw-   0        0        0       60 2022-05-30 07:51:51.000000 clustimage-1.5.9/MANIFEST.in
+-rw-rw-rw-   0        0        0    11667 2022-07-09 20:28:17.780507 clustimage-1.5.9/PKG-INFO
+-rw-rw-rw-   0        0        0    11069 2022-05-30 07:51:51.000000 clustimage-1.5.9/README.md
+drwxrwxrwx   0        0        0        0 2022-07-09 20:28:17.610121 clustimage-1.5.9/clustimage/
+-rw-rw-rw-   0        0        0     2065 2022-07-09 20:28:03.000000 clustimage-1.5.9/clustimage/__init__.py
+-rw-rw-rw-   0        0        0   104561 2022-07-09 20:22:33.000000 clustimage-1.5.9/clustimage/clustimage.py
+-rw-rw-rw-   0        0        0    19837 2022-07-09 16:22:31.000000 clustimage-1.5.9/clustimage/examples.py
+drwxrwxrwx   0        0        0        0 2022-07-09 20:28:17.747513 clustimage-1.5.9/clustimage/tests/
+-rw-rw-rw-   0        0        0        0 2022-05-30 07:51:51.000000 clustimage-1.5.9/clustimage/tests/__init__.py
+-rw-rw-rw-   0        0        0     6639 2022-06-29 16:43:35.000000 clustimage-1.5.9/clustimage/tests/test_clustimage.py
+drwxrwxrwx   0        0        0        0 2022-07-09 20:28:17.779016 clustimage-1.5.9/clustimage/utils/
+-rw-rw-rw-   0        0        0        0 2022-05-30 07:51:51.000000 clustimage-1.5.9/clustimage/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2022-07-09 20:28:17.689189 clustimage-1.5.9/clustimage.egg-info/
+-rw-rw-rw-   0        0        0    11667 2022-07-09 20:28:16.000000 clustimage-1.5.9/clustimage.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      372 2022-07-09 20:28:17.000000 clustimage-1.5.9/clustimage.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-09 20:28:16.000000 clustimage-1.5.9/clustimage.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      166 2022-07-09 20:28:16.000000 clustimage-1.5.9/clustimage.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-07-09 20:28:16.000000 clustimage-1.5.9/clustimage.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-07-09 20:28:17.787635 clustimage-1.5.9/setup.cfg
+-rw-rw-rw-   0        0        0     1579 2022-06-03 08:54:33.000000 clustimage-1.5.9/setup.py
```

### Comparing `clustimage-1.5.8/LICENSE` & `clustimage-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clustimage-1.5.8/PKG-INFO` & `clustimage-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clustimage
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python package clustimage is for unsupervised clustering of images.
 Home-page: https://erdogant.github.io/clustimage
-Download-URL: https://github.com/erdogant/clustimage/archive/1.5.8.tar.gz
+Download-URL: https://github.com/erdogant/clustimage/archive/1.5.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clustimage-1.5.8/README.md` & `clustimage-1.5.9/README.md`

 * *Files identical despite different names*

### Comparing `clustimage-1.5.8/clustimage/__init__.py` & `clustimage-1.5.9/clustimage/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     wget,
     unzip,
     listdir,
     set_logger)
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '1.5.8'
+__version__ = '1.5.9'
 
 # module level doc-string
 __doc__ = """
 clustimage
 =====================================================================
 
 Description
```

### Comparing `clustimage-1.5.8/clustimage/clustimage.py` & `clustimage-1.5.9/clustimage/clustimage.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,14 +190,18 @@
             logger.warning('Parameter grayscale is set to True coz you are using method="%s"' %(method))
             grayscale=True
         if (dim is None) or ((dim[0]>1024) or (dim[1]>1024)):
             logger.warning('Setting dim > (1024, 1024) is most often not needed and can cause memory and other issues.')
         if method=='crop-resistant-hash':
             logger.info('Hash size is set to 8 for crop-resistant and can not be changed.')
             params_hash['hash_size'] = 8
+        if method=='whash-haar':
+            if (np.ceil(np.log2(params_hash['hash_size'])) != np.floor(np.log2(params_hash['hash_size']))):
+                logger.error('hash_size should be power of 2 (8, 16, 32, 64, ..., etc)')
+                return None
 
         # Find path of xml file containing haarcascade file and load in the cascade classifier
         # self.face_cascade = cv2.CascadeClassifier(cv2.data.haarcascades + 'haarcascade_frontalface_alt2.xml')
         self.params = {}
         self.params['cv2_imread_colorscale'] = cv2.IMREAD_GRAYSCALE if grayscale else cv2.IMREAD_COLOR
         self.params['face_cascade'] = 'cv2.CascadeClassifier(cv2.data.haarcascades + "haarcascade_frontalface_default.xml")'
         self.params['eye_cascade'] = 'cv2.CascadeClassifier(cv2.data.haarcascades + "haarcascade_eye.xml")'
```

### Comparing `clustimage-1.5.8/clustimage/examples.py` & `clustimage-1.5.9/clustimage/examples.py`

 * *Files identical despite different names*

### Comparing `clustimage-1.5.8/clustimage/tests/test_clustimage.py` & `clustimage-1.5.9/clustimage/tests/test_clustimage.py`

 * *Files identical despite different names*

### Comparing `clustimage-1.5.8/clustimage.egg-info/PKG-INFO` & `clustimage-1.5.9/clustimage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: clustimage
-Version: 1.5.8
+Version: 1.5.9
 Summary: Python package clustimage is for unsupervised clustering of images.
 Home-page: https://erdogant.github.io/clustimage
-Download-URL: https://github.com/erdogant/clustimage/archive/1.5.8.tar.gz
+Download-URL: https://github.com/erdogant/clustimage/archive/1.5.9.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `clustimage-1.5.8/setup.py` & `clustimage-1.5.9/setup.py`

 * *Files identical despite different names*

