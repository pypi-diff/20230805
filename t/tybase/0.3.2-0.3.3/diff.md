# Comparing `tmp/tybase-0.3.2.tar.gz` & `tmp/tybase-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tybase-0.3.2.tar", last modified: Sat Aug  5 11:46:38 2023, max compression
+gzip compressed data, was "tybase-0.3.3.tar", last modified: Sat Aug  5 12:41:57 2023, max compression
```

## Comparing `tybase-0.3.2.tar` & `tybase-0.3.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.367439 tybase-0.3.2/
--rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.3.2/MANIFEST.in
--rw-r--r--   0 zhangte    (501) staff       (20)      820 2023-08-05 11:46:38.367156 tybase-0.3.2/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.3.2/README.md
--rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 11:46:38.367544 tybase-0.3.2/setup.cfg
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1109 2023-08-05 11:46:16.000000 tybase-0.3.2/setup.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.353223 tybase-0.3.2/tybase/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.3.2/tybase/__init__.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.356725 tybase-0.3.2/tybase/baidu/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.3.2/tybase/baidu/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.3.2/tybase/baidu/kw_tool.py
--rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.3.2/tybase/datatest.txt
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.358963 tybase-0.3.2/tybase/dbtool/
--rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.3.2/tybase/dbtool/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.3.2/tybase/dbtool/data_import.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.3.2/tybase/dbtool/mysql.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.360154 tybase-0.3.2/tybase/lc/
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.3.2/tybase/lc/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.3.2/tybase/lc/eg1.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.366698 tybase-0.3.2/tybase/tools/
--rw-r--r--   0 zhangte    (501) staff       (20)     3195 2023-08-05 09:35:25.000000 tybase-0.3.2/tybase/tools/Task.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.3.2/tybase/tools/__init__.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.3.2/tybase/tools/ali_oss_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     3295 2023-08-05 03:55:59.000000 tybase-0.3.2/tybase/tools/image_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.3.2/tybase/tools/qiniu_tools.py
--rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.3.2/tybase/tools/riqit_tools.py
--rw-r--r--   0 zhangte    (501) staff       (20)     5853 2023-08-05 11:46:16.000000 tybase-0.3.2/tybase/tools/video_utils.py
--rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.3.2/tybase/tytest.py
-drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 11:46:38.355888 tybase-0.3.2/tybase.egg-info/
--rw-rw-rw-   0 zhangte    (501) staff       (20)      820 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/PKG-INFO
--rw-rw-rw-   0 zhangte    (501) staff       (20)      589 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/SOURCES.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/dependency_links.txt
--rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/requires.txt
--rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 11:46:38.000000 tybase-0.3.2/tybase.egg-info/top_level.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.850406 tybase-0.3.3/
+-rw-r--r--   0 zhangte    (501) staff       (20)       28 2023-05-04 00:02:42.000000 tybase-0.3.3/MANIFEST.in
+-rw-r--r--   0 zhangte    (501) staff       (20)      816 2023-08-05 12:41:57.850136 tybase-0.3.3/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      365 2023-06-30 10:18:02.000000 tybase-0.3.3/README.md
+-rw-r--r--   0 zhangte    (501) staff       (20)       38 2023-08-05 12:41:57.850494 tybase-0.3.3/setup.cfg
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1105 2023-08-05 12:41:51.000000 tybase-0.3.3/setup.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.837977 tybase-0.3.3/tybase/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-03 23:43:39.000000 tybase-0.3.3/tybase/__init__.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.841267 tybase-0.3.3/tybase/baidu/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-04 01:26:22.000000 tybase-0.3.3/tybase/baidu/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4364 2023-05-09 03:46:53.000000 tybase-0.3.3/tybase/baidu/kw_tool.py
+-rw-r--r--   0 zhangte    (501) staff       (20)        6 2023-05-03 23:45:43.000000 tybase-0.3.3/tybase/datatest.txt
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.843615 tybase-0.3.3/tybase/dbtool/
+-rw-r--r--   0 zhangte    (501) staff       (20)        0 2023-05-13 02:41:28.000000 tybase-0.3.3/tybase/dbtool/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     9531 2023-06-03 13:29:25.000000 tybase-0.3.3/tybase/dbtool/data_import.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     4679 2023-06-30 10:14:32.000000 tybase-0.3.3/tybase/dbtool/mysql.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.844875 tybase-0.3.3/tybase/lc/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-05-08 08:41:12.000000 tybase-0.3.3/tybase/lc/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2995 2023-05-08 10:37:41.000000 tybase-0.3.3/tybase/lc/eg1.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.849430 tybase-0.3.3/tybase/tools/
+-rw-r--r--   0 zhangte    (501) staff       (20)     3195 2023-08-05 09:35:25.000000 tybase-0.3.3/tybase/tools/Task.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)        0 2023-06-15 03:29:17.000000 tybase-0.3.3/tybase/tools/__init__.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     1599 2023-07-20 05:49:19.000000 tybase-0.3.3/tybase/tools/ali_oss_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     3295 2023-08-05 03:55:59.000000 tybase-0.3.3/tybase/tools/image_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     1544 2023-06-18 14:18:28.000000 tybase-0.3.3/tybase/tools/qiniu_tools.py
+-rw-rw-rw-   0 zhangte    (501) staff       (20)     2081 2023-07-20 05:55:08.000000 tybase-0.3.3/tybase/tools/riqit_tools.py
+-rw-r--r--   0 zhangte    (501) staff       (20)     6715 2023-08-05 12:41:25.000000 tybase-0.3.3/tybase/tools/video_utils.py
+-rw-r--r--   0 zhangte    (501) staff       (20)      205 2023-05-03 23:46:43.000000 tybase-0.3.3/tybase/tytest.py
+drwxr-xr-x   0 zhangte    (501) staff       (20)        0 2023-08-05 12:41:57.840397 tybase-0.3.3/tybase.egg-info/
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      816 2023-08-05 12:41:57.000000 tybase-0.3.3/tybase.egg-info/PKG-INFO
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      589 2023-08-05 12:41:57.000000 tybase-0.3.3/tybase.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        1 2023-08-05 12:41:57.000000 tybase-0.3.3/tybase.egg-info/dependency_links.txt
+-rw-rw-rw-   0 zhangte    (501) staff       (20)      158 2023-08-05 12:41:57.000000 tybase-0.3.3/tybase.egg-info/requires.txt
+-rw-r--r--   0 zhangte    (501) staff       (20)        7 2023-08-05 12:41:57.000000 tybase-0.3.3/tybase.egg-info/top_level.txt
```

### Comparing `tybase-0.3.2/PKG-INFO` & `tybase-0.3.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.3.2
-Summary: 新增,convert_and_split_video 用于按帧率分割视频图片
+Version: 0.3.3
+Summary: 新增,synthesize_video 把图片组和音频合并成视频
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.3.2/setup.py` & `tybase-0.3.3/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 setup(
     name='tybase',
-    version='0.3.2',
+    version='0.3.3',
     include_package_data=True,
-    description='新增,convert_and_split_video 用于按帧率分割视频图片',
+    description='新增,synthesize_video 把图片组和音频合并成视频',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',  # 版本描述
     author='Tuya',
     author_email='353335447@qq.com',
     url='https://github.com/yourusername/your_package',
     packages=find_packages(),
     install_requires=[
```

### Comparing `tybase-0.3.2/tybase/baidu/kw_tool.py` & `tybase-0.3.3/tybase/baidu/kw_tool.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/dbtool/data_import.py` & `tybase-0.3.3/tybase/dbtool/data_import.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/dbtool/mysql.py` & `tybase-0.3.3/tybase/dbtool/mysql.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/lc/eg1.py` & `tybase-0.3.3/tybase/lc/eg1.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/tools/Task.py` & `tybase-0.3.3/tybase/tools/Task.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/tools/ali_oss_tools.py` & `tybase-0.3.3/tybase/tools/ali_oss_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/tools/image_utils.py` & `tybase-0.3.3/tybase/tools/image_utils.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/tools/qiniu_tools.py` & `tybase-0.3.3/tybase/tools/qiniu_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/tools/riqit_tools.py` & `tybase-0.3.3/tybase/tools/riqit_tools.py`

 * *Files identical despite different names*

### Comparing `tybase-0.3.2/tybase/tools/video_utils.py` & `tybase-0.3.3/tybase/tools/video_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     frame_rate_str = subprocess.getoutput(cmd).strip()
     numerator, denominator = map(int, frame_rate_str.split('/'))
     return numerator / denominator
 
 
 def convert_and_split_video(video_url: str, target_frame_rate: int, save_path: str):
     """
+    from tybase.tools.video_utils import convert_and_split_video
 
     convert_and_split_video(
         "https://ty-huanlian.oss-cn-shanghai.aliyuncs.com/videos/20230628/74011b30c0cd50cd4a7dd1fa29a6368f_final.mp4",
         15,
         save_path="/root/autodl-tmp/roopapi/res"
     )
     转换并拆分视频为指定帧率的图片帧和音频文件。
@@ -153,7 +154,26 @@
     cmd_audio = f'ffmpeg -i {video_url} -vn -acodec copy {save_path}/audio.aac'
     subprocess.call(cmd_audio, shell=True)
 
     if tmp_video_path and os.path.exists(tmp_video_path):  # 检查文件是否存在
         os.remove(tmp_video_path)  # 删除临时转换后的视频文件
 
     return save_path
+
+
+def synthesize_video(image_directory, audio_path, output_path, frame_rate, crf=20):
+    # 构建图像文件路径，按照给定的命名格式
+    input_images = image_directory + '/frame_%04d.png'
+
+    # 使用 ffmpeg 命令合成视频
+    command = ['ffmpeg',
+               '-framerate', str(frame_rate),  # 设置帧率
+               '-i', input_images,  # 输入图片文件路径
+               '-i', audio_path,  # 输入音频文件路径
+               '-c:v', 'libx264',  # 视频编码格式
+               '-pix_fmt', 'yuv420p',  # 设置像素格式
+               '-crf', f'{crf}',  # 设置质量，数字越小质量越高
+               '-strict', 'experimental',
+               '-y', output_path]  # 输出视频文件路径
+
+    # 执行命令
+    subprocess.run(command)
```

### Comparing `tybase-0.3.2/tybase.egg-info/PKG-INFO` & `tybase-0.3.3/tybase.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: tybase
-Version: 0.3.2
-Summary: 新增,convert_and_split_video 用于按帧率分割视频图片
+Version: 0.3.3
+Summary: 新增,synthesize_video 把图片组和音频合并成视频
 Home-page: https://github.com/yourusername/your_package
 Author: Tuya
 Author-email: 353335447@qq.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
```

### Comparing `tybase-0.3.2/tybase.egg-info/SOURCES.txt` & `tybase-0.3.3/tybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

