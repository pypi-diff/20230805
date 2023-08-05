# Comparing `tmp/notifyemail-1.0.2.tar.gz` & `tmp/notifyemail-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notifyemail-1.0.2.tar", last modified: Fri Aug 20 08:25:42 2021, max compression
+gzip compressed data, was "notifyemail-1.1.1.tar", last modified: Sat Aug  5 13:13:14 2023, max compression
```

## Comparing `notifyemail-1.0.2.tar` & `notifyemail-1.1.1.tar`

### file list

```diff
@@ -1,13 +1,16 @@
-drwxr-xr-x   0 munros     (501) staff       (20)        0 2021-08-20 08:25:42.650029 notifyemail-1.0.2/
--rw-r--r--   0 munros     (501) staff       (20)   281704 2021-08-20 03:51:07.000000 notifyemail-1.0.2/LICENSE.txt
--rw-r--r--   0 munros     (501) staff       (20)     5766 2021-08-20 08:25:42.649886 notifyemail-1.0.2/PKG-INFO
--rw-r--r--   0 munros     (501) staff       (20)     4963 2021-08-20 05:15:06.000000 notifyemail-1.0.2/README.md
-drwxr-xr-x   0 munros     (501) staff       (20)        0 2021-08-20 08:25:42.648922 notifyemail-1.0.2/notifyemail/
--rw-rw-r--   0 munros     (501) staff       (20)    40995 2021-08-20 08:24:35.000000 notifyemail-1.0.2/notifyemail/__init__.py
-drwxr-xr-x   0 munros     (501) staff       (20)        0 2021-08-20 08:25:42.649711 notifyemail-1.0.2/notifyemail.egg-info/
--rw-r--r--   0 munros     (501) staff       (20)     5766 2021-08-20 08:25:42.000000 notifyemail-1.0.2/notifyemail.egg-info/PKG-INFO
--rw-r--r--   0 munros     (501) staff       (20)      194 2021-08-20 08:25:42.000000 notifyemail-1.0.2/notifyemail.egg-info/SOURCES.txt
--rw-r--r--   0 munros     (501) staff       (20)        1 2021-08-20 08:25:42.000000 notifyemail-1.0.2/notifyemail.egg-info/dependency_links.txt
--rw-r--r--   0 munros     (501) staff       (20)       12 2021-08-20 08:25:42.000000 notifyemail-1.0.2/notifyemail.egg-info/top_level.txt
--rw-r--r--   0 munros     (501) staff       (20)       38 2021-08-20 08:25:42.650072 notifyemail-1.0.2/setup.cfg
--rw-r--r--   0 munros     (501) staff       (20)     1130 2021-08-20 08:24:56.000000 notifyemail-1.0.2/setup.py
+drwxr-xr-x   0 munros     (501) staff       (20)        0 2023-08-05 13:13:14.963174 notifyemail-1.1.1/
+-rw-rw-r--   0 munros     (501) staff       (20)    11357 2023-08-05 05:02:51.000000 notifyemail-1.1.1/LICENSE
+-rw-r--r--   0 munros     (501) staff       (20)     6491 2023-08-05 13:13:14.963021 notifyemail-1.1.1/PKG-INFO
+-rw-rw-r--   0 munros     (501) staff       (20)     5678 2023-08-05 13:12:52.000000 notifyemail-1.1.1/README.md
+drwxr-xr-x   0 munros     (501) staff       (20)        0 2023-08-05 13:13:14.962264 notifyemail-1.1.1/notifyemail/
+-rw-rw-r--   0 munros     (501) staff       (20)     3446 2023-08-05 05:02:51.000000 notifyemail-1.1.1/notifyemail/__init__.py
+-rw-rw-r--   0 munros     (501) staff       (20)    23344 2023-08-05 05:02:51.000000 notifyemail-1.1.1/notifyemail/notify_backend.py
+-rw-rw-r--   0 munros     (501) staff       (20)     8757 2023-08-05 05:02:51.000000 notifyemail-1.1.1/notifyemail/notify_frontend.py
+-rw-rw-r--   0 munros     (501) staff       (20)     9959 2023-08-05 05:02:51.000000 notifyemail-1.1.1/notifyemail/tools.py
+drwxr-xr-x   0 munros     (501) staff       (20)        0 2023-08-05 13:13:14.962812 notifyemail-1.1.1/notifyemail.egg-info/
+-rw-r--r--   0 munros     (501) staff       (20)     6491 2023-08-05 13:13:14.000000 notifyemail-1.1.1/notifyemail.egg-info/PKG-INFO
+-rw-r--r--   0 munros     (501) staff       (20)      272 2023-08-05 13:13:14.000000 notifyemail-1.1.1/notifyemail.egg-info/SOURCES.txt
+-rw-r--r--   0 munros     (501) staff       (20)        1 2023-08-05 13:13:14.000000 notifyemail-1.1.1/notifyemail.egg-info/dependency_links.txt
+-rw-r--r--   0 munros     (501) staff       (20)       12 2023-08-05 13:13:14.000000 notifyemail-1.1.1/notifyemail.egg-info/top_level.txt
+-rw-r--r--   0 munros     (501) staff       (20)       38 2023-08-05 13:13:14.963233 notifyemail-1.1.1/setup.cfg
+-rw-rw-r--   0 munros     (501) staff       (20)     1145 2023-08-05 13:13:09.000000 notifyemail-1.1.1/setup.py
```

### Comparing `notifyemail-1.0.2/setup.py` & `notifyemail-1.1.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 from setuptools import find_packages
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(name='notifyemail', # 包名
-      version='1.0.2', # 版本号
-      description='python邮件小工具',
+      version='1.1.1', # 版本号
+      description='python Email notification tool',
 
       long_description=long_description,
       long_description_content_type="text/markdown",
       author='LvShangqing, ZhangTianyi, LeiYanli',
 
       author_email='seblei@163.com',
 
-      url='https://github.com/lsqqqq/notify',
+      url='https://github.com/lsqqqq/notifyemail',
 
       install_requires=[],
       license='BSD License',
       packages=find_packages(),
       platforms=["all"],
       classifiers=[
         'Intended Audience :: Developers',
@@ -30,8 +30,8 @@
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Topic :: Software Development :: Libraries'
     ],
 
-)
+)
```

