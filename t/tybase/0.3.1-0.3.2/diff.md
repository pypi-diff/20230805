# Comparing `tmp/tybase-0.3.1.tar.gz` & `tmp/tybase-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.3.1.tar", last modified: Sat Aug  5 08:31:41 2023, max compression
+gzip compressed data, was "tybase-0.3.2.tar", last modified: Sat Aug  5 11:46:38 2023, max compression
```

## Comparing `tybase-0.3.1.tar` & `tybase-0.3.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.488989 tybase-0.3.1/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.3.1/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      838 2023-08-05 08:31:41.488674 tybase-0.3.1/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.3.1/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 08:31:41.489094 tybase-0.3.1/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1127 2023-08-05 08:31:28.000000 tybase-0.3.1/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.476787 tybase-0.3.1/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.3.1/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.480099 tybase-0.3.1/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.3.1/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.3.1/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.3.1/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.481949 tybase-0.3.1/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.3.1/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.3.1/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.3.1/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.483235 tybase-0.3.1/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.3.1/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.3.1/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.487726 tybase-0.3.1/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)     2980 2023-08-04 16:48:57.000000 tybase-0.3.1/tybase/tools/Task.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.3.1/tybase/tools/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.3.1/tybase/tools/ali_oss_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     3295 2023-08-05 03:55:59.000000 tybase-0.3.1/tybase/tools/image_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.3.1/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.3.1/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     3379 2023-08-05 08:30:23.000000 tybase-0.3.1/tybase/tools/video_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.3.1/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 08:31:41.479251 tybase-0.3.1/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      838 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      589 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 08:31:41.000000 tybase-0.3.1/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.367439 tybase-0.3.2/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.3.2/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      820 2023-08-05 11:46:38.367156 tybase-0.3.2/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.3.2/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 11:46:38.367544 tybase-0.3.2/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1109 2023-08-05 11:46:16.000000 tybase-0.3.2/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.353223 tybase-0.3.2/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.3.2/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.356725 tybase-0.3.2/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.3.2/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.3.2/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.3.2/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.358963 tybase-0.3.2/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.3.2/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.3.2/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.3.2/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.360154 tybase-0.3.2/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.3.2/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.3.2/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.366698 tybase-0.3.2/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     3195 2023-08-05 09:35:25.000000 tybase-0.3.2/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.3.2/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.3.2/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     3295 2023-08-05 03:55:59.000000 tybase-0.3.2/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.3.2/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.3.2/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     5853 2023-08-05 11:46:16.000000 tybase-0.3.2/tybase/tools/video_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.3.2/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.355888 tybase-0.3.2/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      820 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      589 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.3.1/setup.py` & `tybase-0.3.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.3.1',
+    version='0.3.2',
     include_package_data=True,
-    description='新增,merge_images_and_audio 根据图片和音频,直接合并成视频的方法',
+    description='新增,convert_and_split_video 用于按帧率分割视频图片',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.3.1/tybase/baidu/kw_tool.py` & `tybase-0.3.2/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/dbtool/data_import.py` & `tybase-0.3.2/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/dbtool/mysql.py` & `tybase-0.3.2/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/lc/eg1.py` & `tybase-0.3.2/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/tools/Task.py` & `tybase-0.3.2/tybase/tools/Task.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,27 +25,31 @@
                 print(f'Notify failed due to: {str(e)}')
 
 
         def my_work_function(param1, param2):
             # 这里执行你的实际工作
             return "result"
 
+        from concurrent.futures import ThreadPoolExecutor
+        executor = ThreadPoolExecutor(max_workers=1)
+
 
         # 创建后台任务
         task = TaskRunner.Task(my_work_function, {'param1': 'value1', 'param2': 'value2'}, callback=my_notify_callback)
 
         redis_config = {
             'host': '',
             'port': '',
             'password': '',
             'decode_responses': True  # 或者 False，根据你的需求
         }
         runner = TaskRunner(redis_config, my_notify_callback)
 
         runner.run_task(task)
+        executor.submit(run_task, task)  # 异步执行
 
     #不返回值,可以通过回调函数来通知
     def my_notify_callback(task):
         print('Task ID:', task.id)
         print('Task status:', task.status)
         print('Task result:', task.result)
         # ...
@@ -86,12 +90,13 @@
                 if self.callback:
                     self.callback(self)
 
     def run_task(self, task):
         logger.info(f'Setting task {task.id} to Redis')
         self.r.setex(task.id, 2 * 60 * 60, pickle.dumps(task))
         task.run()
+        # 创建并启动线程来运行任务
         self.r.setex(task.id, 2 * 60 * 60, pickle.dumps(task))
 
 
 if __name__ == '__main__':
     pass
```

### Comparing `tybase-0.3.1/tybase/tools/ali_oss_tools.py` & `tybase-0.3.2/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/tools/image_utils.py` & `tybase-0.3.2/tybase/tools/image_utils.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/tools/qiniu_tools.py` & `tybase-0.3.2/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase/tools/riqit_tools.py` & `tybase-0.3.2/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.1/tybase.egg-info/SOURCES.txt` & `tybase-0.3.2/tybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

