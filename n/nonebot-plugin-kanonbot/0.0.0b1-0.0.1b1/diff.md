# Comparing `tmp/nonebot_plugin_kanonbot-0.0.0b1.tar.gz` & `tmp/nonebot_plugin_kanonbot-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_kanonbot-0.0.0b1.tar", last modified: Thu Jul 20 09:15:51 2023, max compression
+gzip compressed data, was "nonebot_plugin_kanonbot-0.0.1b1.tar", last modified: Sat Aug  5 09:16:54 2023, max compression
```

## Comparing `nonebot_plugin_kanonbot-0.0.0b1.tar` & `nonebot_plugin_kanonbot-0.0.1b1.tar`

### file list

```diff
@@ -1,14 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-20 09:15:51.072111 nonebot_plugin_kanonbot-0.0.0b1/
--rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_kanonbot-0.0.0b1/LICENSE
--rw-rw-rw-   0        0        0      276 2023-07-20 09:15:51.071112 nonebot_plugin_kanonbot-0.0.0b1/PKG-INFO
--rw-rw-rw-   0        0        0     1590 2023-07-20 08:52:22.000000 nonebot_plugin_kanonbot-0.0.0b1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-20 09:15:51.060111 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot/
--rw-rw-rw-   0        0        0     4127 2023-07-20 09:10:55.000000 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-20 09:15:51.069109 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot.egg-info/
--rw-rw-rw-   0        0        0      276 2023-07-20 09:15:51.000000 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      296 2023-07-20 09:15:51.000000 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-20 09:15:51.000000 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      111 2023-07-20 09:15:51.000000 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-07-20 09:15:51.000000 nonebot_plugin_kanonbot-0.0.0b1/nonebot_plugin_kanonbot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-20 09:15:51.072111 nonebot_plugin_kanonbot-0.0.0b1/setup.cfg
--rw-rw-rw-   0        0        0      871 2023-07-20 09:14:49.000000 nonebot_plugin_kanonbot-0.0.0b1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:16:54.623489 nonebot_plugin_kanonbot-0.0.1b1/
+-rw-rw-rw-   0        0        0     1078 2023-06-13 02:14:36.000000 nonebot_plugin_kanonbot-0.0.1b1/LICENSE
+-rw-rw-rw-   0        0        0      276 2023-08-05 09:16:54.622489 nonebot_plugin_kanonbot-0.0.1b1/PKG-INFO
+-rw-rw-rw-   0        0        0     2448 2023-08-05 08:32:00.000000 nonebot_plugin_kanonbot-0.0.1b1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 09:16:54.612487 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/
+-rw-rw-rw-   0        0        0    10370 2023-08-05 05:14:26.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/__init__.py
+-rw-rw-rw-   0        0        0     7757 2023-08-05 09:13:37.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/bot_run.py
+-rw-rw-rw-   0        0        0     8483 2023-08-05 07:48:39.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/config.py
+-rw-rw-rw-   0        0        0     2550 2023-08-05 09:11:43.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/plugins.py
+-rw-rw-rw-   0        0        0    10734 2023-08-05 05:14:26.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot/tools.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:16:54.620489 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/
+-rw-rw-rw-   0        0        0      276 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      433 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       24 2023-08-05 09:16:54.000000 nonebot_plugin_kanonbot-0.0.1b1/nonebot_plugin_kanonbot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:16:54.623489 nonebot_plugin_kanonbot-0.0.1b1/setup.cfg
+-rw-rw-rw-   0        0        0      893 2023-08-05 09:16:52.000000 nonebot_plugin_kanonbot-0.0.1b1/setup.py
```

### Comparing `nonebot_plugin_kanonbot-0.0.0b1/LICENSE` & `nonebot_plugin_kanonbot-0.0.1b1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_kanonbot-0.0.0b1/README.md` & `nonebot_plugin_kanonbot-0.0.1b1/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ## 安装
 （以下方法三选一）
 
 ~~一.命令行安装：~~（未上架，无法使用此命令） 
 
     nb plugin install nonebot-plugin-kanonbot
     
-~~二.pip安装：~~（未上传，无法使用此命令） 
+二.pip安装：（目前处于测试版本，pip也许不是最新的） 
 
 1.执行此命令
 
     pip install nonebot-plugin-kanonbot
     
 2.修改pyproject.toml使其可以加载插件
 
@@ -39,21 +39,53 @@
 ## 配置
 在 nonebot2 项目的`.env`文件中选填配置
 
 1.配置管理员账户
 
     SUPERUSERS=["12345678"] # 配置 NoneBot 超级用户
     
-2.插件数据存放位置，默认为 “./”。
+2.插件数据存放位置，默认为 “./KanonBot/”。
+
+    bilipush_basepath="./KanonBot/"
+
+在 KanonBot文件夹 的 kanon_config.toml 文件中选填配置
+
+	[kanon_api]
+	# KanonAPI的url，非必要无需修改。
+	url = "http://cdn.kanon.ink"
+	# 是否开启API，默认开启。目前部署kanon必须开启。
+	state = True
+	# 是否连接为unity_bot
+	# 对接到kanon主服务器的密钥，填”none“为不对接
+	unity_bot = "none"
+	
+	[emoji]
+	# 是否开启emoji的功能。默认开启。
+	state = True
+	# emoji的加载方式。
+	# "file"：下载emoji的数据库文件。
+	mode = "file"
+	
+	[botswift]
+	# 是否开启bot心跳的功能。默认关闭。
+	state = False
+	# 忽略该功能的群
+	ignore_list = ["123456"]
+	
 
-    bilipush_basepath="./"
 
 ## To-Do
 🔵接下来：
  - [ ] 新建更多文件夹
+ - [ ] 新建更多更多更多更多文件夹
+ - [ ] q头像加缓存
+ - [ ] 自动删除缓存
+ - [ ] botswift功能代码
+ - [ ] 指令冷却功能代码
+ - [ ] 优化锁定
  
  🟢已完成：
  - [x] 新建文件夹
  
 ## 更新日志
 ### 0.0.1
 新建文件夹
```

### Comparing `nonebot_plugin_kanonbot-0.0.0b1/setup.py` & `nonebot_plugin_kanonbot-0.0.1b1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,24 +5,25 @@
 # python.exe setup.py sdist bdist_wheel
 # twine upload dist/*
 
 
 def get_install_requires():
     reqs = [
         'pillow>=9.5.0',
-        'requests>=2.31.0',
+        'httpx>=0.24.0',
+        'toml>=0.10.2',
         'nonebot2>=2.0.0',
         'nonebot_adapter_onebot>=2.2.3',
         'nonebot_plugin_apscheduler>=0.2.0'
     ]
     return reqs
 
 
 setup(name='nonebot_plugin_kanonbot',
-      version='0.0.0-beta1',
+      version='0.0.1-beta1',
       description='nonebot plugin kanonbot',
       author='SuperGuGuGu',
       author_email='13680478000@163.com',
       url='https://github.com/SuperGuGuGu/nonebot_plugin_kanonbot',
       packages=find_packages(),
       python_requires=">=3.8",
       install_requires=get_install_requires(),
```

