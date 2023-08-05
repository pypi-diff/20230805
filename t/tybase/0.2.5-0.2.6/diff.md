# Comparing `tmp/tybase-0.2.5.tar.gz` & `tmp/tybase-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.2.5.tar", last modified: Sat Aug  5 03:16:09 2023, max compression
+gzip compressed data, was "tybase-0.2.6.tar", last modified: Sat Aug  5 03:54:29 2023, max compression
```

## Comparing `tybase-0.2.5.tar` & `tybase-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.153523 tybase-0.2.5/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.5/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      783 2023-08-05 03:16:09.153238 tybase-0.2.5/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.5/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 03:16:09.153616 tybase-0.2.5/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1072 2023-08-05 03:16:02.000000 tybase-0.2.5/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.141520 tybase-0.2.5/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.5/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.145312 tybase-0.2.5/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.5/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.5/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.5/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.147271 tybase-0.2.5/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.5/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.5/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.5/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.148841 tybase-0.2.5/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.5/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.5/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.152392 tybase-0.2.5/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)     2980 2023-08-04 16:48:57.000000 tybase-0.2.5/tybase/tools/Task.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.5/tybase/tools/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.5/tybase/tools/ali_oss_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2848 2023-08-05 03:16:02.000000 tybase-0.2.5/tybase/tools/image_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.5/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.5/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.5/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.144602 tybase-0.2.5/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      783 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.980415 tybase-0.2.6/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.6/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      810 2023-08-05 03:54:29.979981 tybase-0.2.6/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.6/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 03:54:29.980655 tybase-0.2.6/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1099 2023-08-05 03:54:18.000000 tybase-0.2.6/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.966567 tybase-0.2.6/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.6/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.970553 tybase-0.2.6/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.6/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.6/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.6/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.973656 tybase-0.2.6/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.6/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.6/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.6/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.975124 tybase-0.2.6/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.6/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.6/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.978795 tybase-0.2.6/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     2980 2023-08-04 16:48:57.000000 tybase-0.2.6/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.6/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.6/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     3230 2023-08-05 03:54:18.000000 tybase-0.2.6/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.6/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.6/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.6/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:54:29.969125 tybase-0.2.6/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      810 2023-08-05 03:54:29.000000 tybase-0.2.6/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-05 03:54:29.000000 tybase-0.2.6/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 03:54:29.000000 tybase-0.2.6/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 03:54:29.000000 tybase-0.2.6/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 03:54:29.000000 tybase-0.2.6/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.2.5/PKG-INFO` & `tybase-0.2.6/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.5
-Summary: 新增 url_to_md5 的方法
+Version: 0.2.6
+Summary: 新增 url_to_md5_without_ext 且不包含md5的方法
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.2.5/setup.py` & `tybase-0.2.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.2.5',
+    version='0.2.6',
     include_package_data=True,
-    description='新增 url_to_md5 的方法',
+    description='新增 url_to_md5_without_ext 且不包含md5的方法',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.2.5/tybase/baidu/kw_tool.py` & `tybase-0.2.6/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/dbtool/data_import.py` & `tybase-0.2.6/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/dbtool/mysql.py` & `tybase-0.2.6/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/lc/eg1.py` & `tybase-0.2.6/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/tools/Task.py` & `tybase-0.2.6/tybase/tools/Task.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/tools/ali_oss_tools.py` & `tybase-0.2.6/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/tools/image_utils.py` & `tybase-0.2.6/tybase/tools/image_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,26 +74,40 @@
     md5 = hashlib.md5()
     md5.update(byte_im)
 
     return md5.hexdigest()
 
 
 def url_to_md5(url):
+    # from tybase.tools.image_utils import url_to_md5
     # 对url的md5进行加密
     # 获取文件名（不包括格式）
     filename = url.split("/")[-1].split(".")[0]
     # 获取格式
     ext = url.split(".")[-1]
 
     # 对文件名进行MD5加密
     m = hashlib.md5()
     m.update(filename.encode('utf-8'))
     md5 = m.hexdigest()
     # 返回MD5哈希值与格式的组合
     return "{}.{}".format(md5, ext)
 
 
+
+def url_to_md5_without_ext(url):
+    """
+    对url进行MD5加密，返回不包含扩展名的MD5值。
+    """
+    # 获取文件名（不包括格式）
+    filename = url.split("/")[-1].split(".")[0]
+
+    # 对文件名进行MD5加密
+    m = hashlib.md5()
+    m.update(filename.encode('utf-8'))
+    return m.hexdigest()
+
 if __name__ == '__main__':
     pass
     # 图片裁剪
     # crop_image_from_url
     # get_md5 获取md5
```

### Comparing `tybase-0.2.5/tybase/tools/qiniu_tools.py` & `tybase-0.2.6/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase/tools/riqit_tools.py` & `tybase-0.2.6/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.5/tybase.egg-info/PKG-INFO` & `tybase-0.2.6/tybase.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.5
-Summary: 新增 url_to_md5 的方法
+Version: 0.2.6
+Summary: 新增 url_to_md5_without_ext 且不包含md5的方法
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.2.5/tybase.egg-info/SOURCES.txt` & `tybase-0.2.6/tybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

