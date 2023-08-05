# Comparing `tmp/tybase-0.2.3.tar.gz` & `tmp/tybase-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.2.3.tar", last modified: Fri Aug  4 16:34:34 2023, max compression
+gzip compressed data, was "tybase-0.2.4.tar", last modified: Fri Aug  4 16:36:35 2023, max compression
```

## Comparing `tybase-0.2.3.tar` & `tybase-0.2.4.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.390956 tybase-0.2.3/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.3/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      783 2023-08-04 16:34:34.390709 tybase-0.2.3/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.3/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-04 16:34:34.391099 tybase-0.2.3/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1072 2023-08-04 16:34:28.000000 tybase-0.2.3/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.381256 tybase-0.2.3/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.3/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.383901 tybase-0.2.3/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.3/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.3/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.3/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.385623 tybase-0.2.3/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.3/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.3/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.3/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.386757 tybase-0.2.3/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.3/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.3/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.390090 tybase-0.2.3/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)     2831 2023-08-04 15:56:07.000000 tybase-0.2.3/tybase/tools/Task.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.3/tybase/tools/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.3/tybase/tools/ali_oss_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2457 2023-08-04 16:34:01.000000 tybase-0.2.3/tybase/tools/image_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.3/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.3/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.3/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:34:34.383349 tybase-0.2.3/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      783 2023-08-04 16:34:34.000000 tybase-0.2.3/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-04 16:34:34.000000 tybase-0.2.3/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-04 16:34:34.000000 tybase-0.2.3/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-04 16:34:34.000000 tybase-0.2.3/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-04 16:34:34.000000 tybase-0.2.3/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.524077 tybase-0.2.4/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.4/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      783 2023-08-04 16:36:35.523672 tybase-0.2.4/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.4/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-04 16:36:35.524218 tybase-0.2.4/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1072 2023-08-04 16:36:25.000000 tybase-0.2.4/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.509288 tybase-0.2.4/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.4/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.512538 tybase-0.2.4/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.4/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.4/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.4/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.514631 tybase-0.2.4/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.4/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.4/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.4/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.516012 tybase-0.2.4/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.4/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.4/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.522785 tybase-0.2.4/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     2831 2023-08-04 15:56:07.000000 tybase-0.2.4/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.4/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.4/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2456 2023-08-04 16:36:29.000000 tybase-0.2.4/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.4/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.4/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.4/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.511512 tybase-0.2.4/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      783 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.2.3/PKG-INFO` & `tybase-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.3
+Version: 0.2.4
 Summary: 修复图像裁剪的问题
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tybase-0.2.3/setup.py` & `tybase-0.2.4/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.2.3',
+    version='0.2.4',
     include_package_data=True,
     description='修复图像裁剪的问题',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
```

### Comparing `tybase-0.2.3/tybase/baidu/kw_tool.py` & `tybase-0.2.4/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/dbtool/data_import.py` & `tybase-0.2.4/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/dbtool/mysql.py` & `tybase-0.2.4/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/lc/eg1.py` & `tybase-0.2.4/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/tools/Task.py` & `tybase-0.2.4/tybase/tools/Task.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/tools/ali_oss_tools.py` & `tybase-0.2.4/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/tools/image_utils.py` & `tybase-0.2.4/tybase/tools/image_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 
     if max(image.shape[:2]) <= max_dimension:
         loguru.logger.info("不需要裁剪,直接保存")
         save_image(image, save_path)
     else:
         resized_image = resize_image(image, max_dimension)
         save_image(resized_image, save_path)
-
     return save_path
 
 
 def get_md5(img, ext='.jpg'):
     # Convert image to byte array
     is_success, im_buf_arr = cv2.imencode(ext, img)
     byte_im = im_buf_arr.tobytes()
```

### Comparing `tybase-0.2.3/tybase/tools/qiniu_tools.py` & `tybase-0.2.4/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase/tools/riqit_tools.py` & `tybase-0.2.4/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.3/tybase.egg-info/PKG-INFO` & `tybase-0.2.4/tybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.3
+Version: 0.2.4
 Summary: 修复图像裁剪的问题
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tybase-0.2.3/tybase.egg-info/SOURCES.txt` & `tybase-0.2.4/tybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

