# Comparing `tmp/tybase-0.2.4.tar.gz` & `tmp/tybase-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.2.4.tar", last modified: Fri Aug  4 16:36:35 2023, max compression
+gzip compressed data, was "tybase-0.2.5.tar", last modified: Sat Aug  5 03:16:09 2023, max compression
```

## Comparing `tybase-0.2.4.tar` & `tybase-0.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.524077 tybase-0.2.4/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.4/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      783 2023-08-04 16:36:35.523672 tybase-0.2.4/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.4/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-04 16:36:35.524218 tybase-0.2.4/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1072 2023-08-04 16:36:25.000000 tybase-0.2.4/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.509288 tybase-0.2.4/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.4/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.512538 tybase-0.2.4/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.4/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.4/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.4/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.514631 tybase-0.2.4/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.4/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.4/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.4/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.516012 tybase-0.2.4/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.4/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.4/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.522785 tybase-0.2.4/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)     2831 2023-08-04 15:56:07.000000 tybase-0.2.4/tybase/tools/Task.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.4/tybase/tools/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.4/tybase/tools/ali_oss_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     2456 2023-08-04 16:36:29.000000 tybase-0.2.4/tybase/tools/image_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.4/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.4/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.4/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-04 16:36:35.511512 tybase-0.2.4/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      783 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-04 16:36:35.000000 tybase-0.2.4/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.153523 tybase-0.2.5/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.2.5/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      783 2023-08-05 03:16:09.153238 tybase-0.2.5/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.2.5/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 03:16:09.153616 tybase-0.2.5/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1072 2023-08-05 03:16:02.000000 tybase-0.2.5/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.141520 tybase-0.2.5/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.2.5/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.145312 tybase-0.2.5/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.2.5/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.2.5/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.2.5/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.147271 tybase-0.2.5/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.2.5/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.2.5/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.2.5/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.148841 tybase-0.2.5/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.2.5/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.2.5/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.152392 tybase-0.2.5/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     2980 2023-08-04 16:48:57.000000 tybase-0.2.5/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.2.5/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.2.5/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     2848 2023-08-05 03:16:02.000000 tybase-0.2.5/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.2.5/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.2.5/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.2.5/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 03:16:09.144602 tybase-0.2.5/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      783 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      561 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 03:16:09.000000 tybase-0.2.5/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.2.4/PKG-INFO` & `tybase-0.2.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.4
-Summary: 修复图像裁剪的问题
+Version: 0.2.5
+Summary: 新增 url_to_md5 的方法
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.2.4/setup.py` & `tybase-0.2.5/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.2.4',
+    version='0.2.5',
     include_package_data=True,
-    description='修复图像裁剪的问题',
+    description='新增 url_to_md5 的方法',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.2.4/tybase/baidu/kw_tool.py` & `tybase-0.2.5/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase/dbtool/data_import.py` & `tybase-0.2.5/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase/dbtool/mysql.py` & `tybase-0.2.5/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase/lc/eg1.py` & `tybase-0.2.5/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase/tools/Task.py` & `tybase-0.2.5/tybase/tools/Task.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,47 +4,48 @@
 import requests
 from loguru import logger
 import time
 
 
 class TaskRunner:
     """
+        from tybase.tools.Task import TaskRunner
         def my_notify_callback(task):
-        url = 'YOUR_NOTIFY_URL'
-        headers = {"TOKEN": "YOUR_NOTIFY_TOKEN"}
-        data = {
-            "queue_id": task.id,
-            "convert_url": task.result,
-            "status": 100 if task.status == "completed" else 250
+            url = 'YOUR_NOTIFY_URL'
+            headers = {"TOKEN": "YOUR_NOTIFY_TOKEN"}
+            data = {
+                "queue_id": task.id,
+                "convert_url": task.result,
+                "status": 100 if task.status == "completed" else 250
+            }
+
+            try:
+                response = requests.post(url, json=data, headers=headers)
+                print(response.status_code, "成功")
+            except Exception as e:
+                print(f'Notify failed due to: {str(e)}')
+
+
+        def my_work_function(param1, param2):
+            # 这里执行你的实际工作
+            return "result"
+
+
+        # 创建后台任务
+        task = TaskRunner.Task(my_work_function, {'param1': 'value1', 'param2': 'value2'}, callback=my_notify_callback)
+
+        redis_config = {
+            'host': '',
+            'port': '',
+            'password': '',
+            'decode_responses': True  # 或者 False，根据你的需求
         }
+        runner = TaskRunner(redis_config, my_notify_callback)
 
-        try:
-            response = requests.post(url, json=data, headers=headers)
-            print(response.status_code, "成功")
-        except Exception as e:
-            print(f'Notify failed due to: {str(e)}')
-
-
-    def my_work_function(param1, param2):
-        # 这里执行你的实际工作
-        return "result"
-
-
-    # 创建后台任务
-    task = TaskRunner.Task(my_work_function, {'param1': 'value1', 'param2': 'value2'}, callback=my_notify_callback)
-
-    redis_config = {
-        'host': '',
-        'port': '',
-        'password': '',
-        'decode_responses': True  # 或者 False，根据你的需求
-    }
-    runner = TaskRunner(redis_config, my_notify_callback)
-
-    runner.run_task(task)
+        runner.run_task(task)
 
     #不返回值,可以通过回调函数来通知
     def my_notify_callback(task):
         print('Task ID:', task.id)
         print('Task status:', task.status)
         print('Task result:', task.result)
         # ...
```

### Comparing `tybase-0.2.4/tybase/tools/ali_oss_tools.py` & `tybase-0.2.5/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase/tools/image_utils.py` & `tybase-0.2.5/tybase/tools/image_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -73,12 +73,27 @@
     # Compute MD5
     md5 = hashlib.md5()
     md5.update(byte_im)
 
     return md5.hexdigest()
 
 
+def url_to_md5(url):
+    # 对url的md5进行加密
+    # 获取文件名（不包括格式）
+    filename = url.split("/")[-1].split(".")[0]
+    # 获取格式
+    ext = url.split(".")[-1]
+
+    # 对文件名进行MD5加密
+    m = hashlib.md5()
+    m.update(filename.encode('utf-8'))
+    md5 = m.hexdigest()
+    # 返回MD5哈希值与格式的组合
+    return "{}.{}".format(md5, ext)
+
+
 if __name__ == '__main__':
     pass
     # 图片裁剪
     # crop_image_from_url
     # get_md5 获取md5
```

### Comparing `tybase-0.2.4/tybase/tools/qiniu_tools.py` & `tybase-0.2.5/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase/tools/riqit_tools.py` & `tybase-0.2.5/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.2.4/tybase.egg-info/PKG-INFO` & `tybase-0.2.5/tybase.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.2.4
-Summary: 修复图像裁剪的问题
+Version: 0.2.5
+Summary: 新增 url_to_md5 的方法
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.2.4/tybase.egg-info/SOURCES.txt` & `tybase-0.2.5/tybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

