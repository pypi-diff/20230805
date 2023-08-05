# Comparing `tmp/neco_f-0.0.5.tar.gz` & `tmp/neco_f-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neco_f-0.0.5.tar", last modified: Fri Aug  4 08:17:10 2023, max compression
+gzip compressed data, was "neco_f-0.0.6.tar", last modified: Sat Aug  5 10:13:18 2023, max compression
```

## Comparing `neco_f-0.0.5.tar` & `neco_f-0.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 08:17:10.388239 neco_f-0.0.5/
--rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 neco_f-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      600 2023-08-04 08:17:10.388239 neco_f-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      163 2023-08-04 07:56:05.000000 neco_f-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 08:17:10.378238 neco_f-0.0.5/neco_f.egg-info/
--rw-rw-rw-   0        0        0      600 2023-08-04 08:17:10.000000 neco_f-0.0.5/neco_f.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      308 2023-08-04 08:17:10.000000 neco_f-0.0.5/neco_f.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 08:17:10.000000 neco_f-0.0.5/neco_f.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      118 2023-08-04 08:17:10.000000 neco_f-0.0.5/neco_f.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-08-04 08:17:10.000000 neco_f-0.0.5/neco_f.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 08:17:10.389238 neco_f-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1166 2023-08-04 08:17:06.000000 neco_f-0.0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-08-04 08:17:10.387239 neco_f-0.0.5/src/
--rw-rw-rw-   0        0        0        0 2023-08-04 08:13:48.000000 neco_f-0.0.5/src/__init__.py
--rw-rw-rw-   0        0        0     7059 2023-08-04 07:10:04.000000 neco_f-0.0.5/src/always_used.py
--rw-rw-rw-   0        0        0     1453 2023-07-21 02:07:41.000000 neco_f-0.0.5/src/api_.py
--rw-rw-rw-   0        0        0      904 2023-08-04 07:05:59.000000 neco_f-0.0.5/src/auto_pip.py
--rw-rw-rw-   0        0        0     4784 2023-03-04 11:15:59.000000 neco_f-0.0.5/src/internet.py
--rw-rw-rw-   0        0        0     1959 2023-06-30 13:15:51.000000 neco_f-0.0.5/src/jiemi.py
--rw-rw-rw-   0        0        0      501 2023-08-02 12:43:35.000000 neco_f-0.0.5/src/logger.py
--rw-rw-rw-   0        0        0     1161 2023-07-27 08:04:13.000000 neco_f-0.0.5/src/os_time.py
--rw-rw-rw-   0        0        0     1750 2023-08-04 07:10:04.000000 neco_f-0.0.5/src/pic_.py
+drwxrwxrwx   0        0        0        0 2023-08-05 10:13:18.675034 neco_f-0.0.6/
+-rw-rw-rw-   0        0        0     1085 2023-08-04 07:53:17.000000 neco_f-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      628 2023-08-05 10:13:18.675034 neco_f-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      189 2023-08-05 10:13:11.000000 neco_f-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 10:13:18.660387 neco_f-0.0.6/neco_f.egg-info/
+-rw-rw-rw-   0        0        0      628 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      308 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      118 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-08-05 10:13:18.000000 neco_f-0.0.6/neco_f.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 10:13:18.676011 neco_f-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1166 2023-08-05 10:12:32.000000 neco_f-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 10:13:18.673081 neco_f-0.0.6/src/
+-rw-rw-rw-   0        0        0        0 2023-08-04 08:13:48.000000 neco_f-0.0.6/src/__init__.py
+-rw-rw-rw-   0        0        0     7064 2023-08-05 09:57:20.000000 neco_f-0.0.6/src/always_used.py
+-rw-rw-rw-   0        0        0     1459 2023-08-05 09:57:20.000000 neco_f-0.0.6/src/api_.py
+-rw-rw-rw-   0        0        0      904 2023-08-04 07:05:59.000000 neco_f-0.0.6/src/auto_pip.py
+-rw-rw-rw-   0        0        0     4774 2023-08-05 09:57:20.000000 neco_f-0.0.6/src/internet.py
+-rw-rw-rw-   0        0        0     1921 2023-08-05 09:56:00.000000 neco_f-0.0.6/src/jiemi.py
+-rw-rw-rw-   0        0        0      505 2023-08-05 10:12:15.000000 neco_f-0.0.6/src/logger.py
+-rw-rw-rw-   0        0        0     1161 2023-07-27 08:04:13.000000 neco_f-0.0.6/src/os_time.py
+-rw-rw-rw-   0        0        0     1750 2023-08-04 07:10:04.000000 neco_f-0.0.6/src/pic_.py
```

### Comparing `neco_f-0.0.5/LICENSE` & `neco_f-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.5/PKG-INFO` & `neco_f-0.0.6/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neco_f
-Version: 0.0.5
+Version: 0.0.6
 Summary: 一个鱼龙混杂的库
 Home-page: https://github.com/sweetnotice/neco_f
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,9 @@
  ## 包括但不限于
  - 网络爬虫
  - 图像处理
  - 字符串处理
  - 彩色打印
  - 音乐播放
  - crypto解密
+ - 日志
+ - 文件更新
```

### Comparing `neco_f-0.0.5/neco_f.egg-info/PKG-INFO` & `neco_f-0.0.6/neco_f.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neco-f
-Version: 0.0.5
+Version: 0.0.6
 Summary: 一个鱼龙混杂的库
 Home-page: https://github.com/sweetnotice/neco_f
 Author: neco_arc
 Author-email: 3306601284@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -17,7 +17,9 @@
  ## 包括但不限于
  - 网络爬虫
  - 图像处理
  - 字符串处理
  - 彩色打印
  - 音乐播放
  - crypto解密
+ - 日志
+ - 文件更新
```

### Comparing `neco_f-0.0.5/setup.py` & `neco_f-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open('README.md', mode='r', encoding='utf-8') as f:
     long_description = f.read()
 setup(
     name='neco_f',
-    version='0.0.5',
+    version='0.0.6',
     author='neco_arc',
     author_email='3306601284@qq.com',
     description='一个鱼龙混杂的库',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/sweetnotice/neco_f',
     classifiers=[
```

### Comparing `neco_f-0.0.5/src/always_used.py` & `neco_f-0.0.6/src/always_used.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import json
-from internet import download
+from neco_f.internet import download
 
 
 def format_str(data: str):
     # 去除字符串中的 ' / , \ , " , ? , * , < , > , | , : ,空格'
     return data.replace('/', '').replace('\\', '').replace('"', '').replace('?', '').replace('*', '') \
         .replace('<', '').replace('>', '').replace('|', '').replace(':', '').replace(' ', '')
 
@@ -50,15 +50,17 @@
         play_mp3(music_path, 1)
     # time.sleep(0.1)
     notification.notify(
         title=title,
         message=message,
         app_icon=icon,
         timeout=time_)
- # 打包时要加 --hidden-import plyer.platforms.win.notification
+
+
+# 打包时要加 --hidden-import plyer.platforms.win.notification
 
 
 # 创建文件夹
 def mkdir(path):
     import os
     path = path.strip()
     path = path.rstrip("\\")
@@ -174,17 +176,14 @@
             return json.dumps(data_dict, indent=4, ensure_ascii=False)
         except json.JSONDecodeError as e:
             return f"Error: {e.msg}"
     else:
         return "Error: input data is not a dictionary or a string"
 
 
-
-
-
 # 编写bat脚本，删除旧程序，运行新程序
 def WriteRestartCmd(rename: str, exe_name: str = 'updata.exe', icon=None,
                     download_url: str = ''):  # sourcery skip: ensure-file-closed, use-fstring-for-concatenation
     """
     :param exe_name: 下载的新版软件名字,默认为 updata.exe
     :param icon: 图标
     :param rename: 新软件要改的名字，同时是通知弹窗的标题
```

### Comparing `neco_f-0.0.5/src/api_.py` & `neco_f-0.0.6/src/api_.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 # api
 import requests
 import random
 from pprint import pprint
+
+
 class Api:
     def __init__(self):
         self._key = '5d6ffcb535f0b986622d6c27d155dce2'
 
     def yiyan(self, type='r'):
-
         # (a:动画；b:漫画；c:游戏；d:文学；e:原创；f:来自网络；g:其他；h:影视；i:诗词；j:网易云；k:哲学)
         if type == 'r':  # r:随机
             type = random.choice(['a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k'])
             # print(type)
         resp = requests.get(f'http://api.a20safe.com/api.php?api=6&key={self._key}&type={type}').json()
         # pprint(resp)
         data = resp['data'][0]['motto']
         from_ = resp['data'][0]['from']
         # print(f'「 {data} 」\n\t\t————{from_}')
-        return data,from_
+        return data, from_
 
     def txt_to_mp3(self, txt, speed=3):
         import requests
         resp = requests.get(f'http://api.a20safe.com/api.php?api=8&key={self._key}&text={txt}&spd={speed}').json()
         url = resp['data'][0]["mp3url"]
         # print(url)
         return url
-    def yan_zheng_ma(self,pic_base64):
+
+    def yan_zheng_ma(self, pic_base64):
         resp = requests.get(f'https://api.a20safe.com/api.php?api=13&key={self._key}&imgbase64={pic_base64}').json()
         pprint(resp)
 
 
 if __name__ == '__main__':
     # import pic_
     # pic_base64 = pic_.Pic(r'C:\Users\Administrator\Desktop\Snipaste_2023-07-21_10-00-48.png').base64_pic()
```

### Comparing `neco_f-0.0.5/src/auto_pip.py` & `neco_f-0.0.6/src/auto_pip.py`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.5/src/internet.py` & `neco_f-0.0.6/src/internet.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+import requests
+from tqdm import tqdm
+import os
+
+
 # 请求超时重试
 def request_timeout_retry(url: str, headers: dict = {}, out_time: int = 2, retry_cnt: int = 3):
     '''
     :param url: 地址
     :param data: 请求头
     :param out_time: 超时时间
     :param retry_cnt: 重试次数
@@ -14,16 +19,14 @@
             pass
     print(f'{url} 访问超时！')
     return False
 
 
 # 进度条下载
 def download(url: str, fname: str):
-    import requests
-    from tqdm import tqdm
     resp = requests.get(url, stream=True)  # 用流stream的方式获取url的数据
     total = int(resp.headers.get('content-length', 0))  # 拿到文件的长度，并把total初始化为0
     with open(fname, 'wb') as file, tqdm(  # 初始化tqdm，传入总数，文件名等数据，接着就是写入，更新等操作了
             desc=fname,  # 下载界面显示文件的名称
             total=total,
             unit='iB',
             unit_scale=True,
@@ -48,15 +51,15 @@
     :param timeOut:指定程序进行网络请求的超时时长，默认值为10秒
     :param useKeyBase64:强制使用AES-128解密，并使用输入的Base64String来作为解密KEY
     :param stopSpeed:低于这个速度会重试，默认0
     :param enableDelAfterDone:用于开启程序的下载完成后自动删除临时目录功能，默认开启
     :param enableBinaryMerge:二进制合并,默认关闭
     :param disableIntegrityCheck:不进行完整性检验，默认关闭
     """
-    import os
+
     from threading import Thread
     command = 'N_m3u8DL-CLI.exe'
     command += f' "{fileurl}"'
     if workDir:
         command += f' --workDir "{workDir}"'
     if saveName:
         command += f' --saveName "{saveName}"'
@@ -112,8 +115,8 @@
     from m_f.always_used import wait_threads
 
     threads = []
     for i in range(3):
         threads.append(threading.Thread(target=wget_downloader, args=(
             'https://yunpan.aliyun.com/downloads/apps/desktop/aDrive.exe', r'C:\Users\33066\Desktop', f'{i}.mp4')))
     wait_threads(threads)
-    print('over')
+    print('over')
```

### Comparing `neco_f-0.0.5/src/jiemi.py` & `neco_f-0.0.6/src/jiemi.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-# coding=gbk
+import base64
+import urllib.parse
+from Crypto.Cipher import AES
+import re
+import base64
+import binascii
+
+
 def debase64_(data: str):
-    import base64
     return base64.b64decode(data).decode('utf-8').encode().decode('unicode_escape')
 
 
 def deescape_(data: str):
-    import urllib.parse
     return urllib.parse.unquote(data.replace('%u', '\\u').encode().decode('unicode-escape'))
 
 
 def deunicode_(data: str):
     return data.encode('utf-8').decode('unicode_escape')
 
 
 def deaes_cbc(data: str, key: str, iv: str):
-    from Crypto.Cipher import AES
-    import re
-    import base64
-    import binascii
-
     def add_16(par):  # ²¹Î»µ½16±¶ÊýÎ»
         while len(par) % 16 != 0:
             par += b'\x00'
         return par
 
     # ¶Ôkey½øÐÐ²¹Î» ¡£key£¬iv ½øÐÐ±àÂë£¬°Ñdata±àÂë³É×Ö½Ú
     key = add_16(key.encode('utf-8'))
@@ -53,8 +53,8 @@
     data = re.search('getVideoInfo\("(?P<data>.*?)"\)', resp)['data']
     url = deaes_cbc(data, key, iv)
     return url
 
 
 if __name__ == '__main__':
     url = 'https://danmu.yhdmjx.com/m3u8.php?url=ksxUY0Bd5nJghA51z%2FAPtRkpMKTYl2cAnnQGM3ZLcqRHFyfmO2GUfBvm9fTyDDg0'
-    print(yinhua_jiemi(url))
+    print(yinhua_jiemi(url))
```

### Comparing `neco_f-0.0.5/src/os_time.py` & `neco_f-0.0.6/src/os_time.py`

 * *Files identical despite different names*

### Comparing `neco_f-0.0.5/src/pic_.py` & `neco_f-0.0.6/src/pic_.py`

 * *Files identical despite different names*

