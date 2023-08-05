# Comparing `tmp/tybase-0.2.9.tar.gz` & `tmp/tybase-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.2.9.tar", last modified: Sat Aug  5 08:22:30 2023, max compression
+gzip compressed data, was "tybase-0.3.1.tar", last modified: Sat Aug  5 08:31:41 2023, max compression
```

## Comparing `tybase-0.2.9.tar` & `tybase-0.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.055953 tybase-0.2.9/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.9/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      808 2023-08-05 08:22:30.054431 tybase-0.2.9/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.9/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 08:22:30.056215 tybase-0.2.9/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1097 2023-08-05 08:22:25.000000 tybase-0.2.9/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.038671 tybase-0.2.9/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.9/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.044096 tybase-0.2.9/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.9/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.9/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.9/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.046432 tybase-0.2.9/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.9/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.9/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.9/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.047800 tybase-0.2.9/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.9/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.9/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.053187 tybase-0.2.9/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)     2980 2023-08-04 16:48:57.000000 tybase-0.2.9/tybase/tools/Task.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.9/tybase/tools/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.9/tybase/tools/ali_oss_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     3295 2023-08-05 03:55:59.000000 tybase-0.2.9/tybase/tools/image_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.9/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.9/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1340 2023-08-05 08:21:28.000000 tybase-0.2.9/tybase/tools/video_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.9/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:22:30.042630 tybase-0.2.9/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      808 2023-08-05 08:22:29.000000 tybase-0.2.9/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      589 2023-08-05 08:22:29.000000 tybase-0.2.9/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 08:22:29.000000 tybase-0.2.9/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 08:22:29.000000 tybase-0.2.9/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 08:22:29.000000 tybase-0.2.9/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.488989 tybase-0.3.1/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.3.1/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      838 2023-08-05 08:31:41.488674 tybase-0.3.1/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.3.1/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 08:31:41.489094 tybase-0.3.1/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1127 2023-08-05 08:31:28.000000 tybase-0.3.1/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.476787 tybase-0.3.1/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.3.1/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.480099 tybase-0.3.1/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.3.1/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.3.1/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.3.1/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.481949 tybase-0.3.1/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.3.1/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.3.1/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.3.1/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.483235 tybase-0.3.1/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.3.1/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.3.1/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.487726 tybase-0.3.1/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     2980 2023-08-04 16:48:57.000000 tybase-0.3.1/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.3.1/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.3.1/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     3295 2023-08-05 03:55:59.000000 tybase-0.3.1/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.3.1/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.3.1/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     3379 2023-08-05 08:30:23.000000 tybase-0.3.1/tybase/tools/video_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.3.1/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.479251 tybase-0.3.1/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      838 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      589 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.2.9/PKG-INFO` & `tybase-0.3.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.9
-Summary: 新增,对本地视频进行分割成图片的方法
+Version: 0.3.1
+Summary: 新增,merge_images_and_audio 根据图片和音频,直接合并成视频的方法
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.2.9/setup.py` & `tybase-0.3.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.2.9',
+    version='0.3.1',
     include_package_data=True,
-    description='新增,对本地视频进行分割成图片的方法',
+    description='新增,merge_images_and_audio 根据图片和音频,直接合并成视频的方法',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.2.9/tybase/baidu/kw_tool.py` & `tybase-0.3.1/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/dbtool/data_import.py` & `tybase-0.3.1/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/dbtool/mysql.py` & `tybase-0.3.1/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/lc/eg1.py` & `tybase-0.3.1/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/tools/Task.py` & `tybase-0.3.1/tybase/tools/Task.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/tools/ali_oss_tools.py` & `tybase-0.3.1/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/tools/image_utils.py` & `tybase-0.3.1/tybase/tools/image_utils.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/tools/qiniu_tools.py` & `tybase-0.3.1/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase/tools/riqit_tools.py` & `tybase-0.3.1/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.9/tybase.egg-info/PKG-INFO` & `tybase-0.3.1/tybase.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.9
-Summary: 新增,对本地视频进行分割成图片的方法
+Version: 0.3.1
+Summary: 新增,merge_images_and_audio 根据图片和音频,直接合并成视频的方法
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.2.9/tybase.egg-info/SOURCES.txt` & `tybase-0.3.1/tybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

