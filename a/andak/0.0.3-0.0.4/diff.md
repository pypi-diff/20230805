# Comparing `tmp/andak-0.0.3.tar.gz` & `tmp/andak-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "andak-0.0.3.tar", last modified: Thu Aug  3 23:40:02 2023, max compression
+gzip compressed data, was "andak-0.0.4.tar", last modified: Sat Aug  5 18:25:57 2023, max compression
```

## Comparing `andak-0.0.3.tar` & `andak-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:40:02.581427 andak-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-03 23:39:57.000000 andak-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-03 23:40:02.581427 andak-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-03 23:39:57.000000 andak-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:40:02.581427 andak-0.0.3/andak/
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-08-03 23:39:57.000000 andak-0.0.3/andak/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:40:02.581427 andak-0.0.3/andak.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-03 23:40:02.000000 andak-0.0.3/andak.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-03 23:40:02.000000 andak-0.0.3/andak.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:40:02.000000 andak-0.0.3/andak.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-03 23:40:02.000000 andak-0.0.3/andak.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-03 23:40:02.000000 andak-0.0.3/andak.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:40:02.581427 andak-0.0.3/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     2520 2023-08-03 23:39:57.000000 andak-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:25:57.657421 andak-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-08-05 18:25:52.000000 andak-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-05 18:25:57.653421 andak-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-08-05 18:25:52.000000 andak-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:25:57.653421 andak-0.0.4/andak/
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-08-05 18:25:52.000000 andak-0.0.4/andak/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 18:25:57.653421 andak-0.0.4/andak.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-08-05 18:25:57.000000 andak-0.0.4/andak.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-05 18:25:57.000000 andak-0.0.4/andak.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 18:25:57.000000 andak-0.0.4/andak.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-08-05 18:25:57.000000 andak-0.0.4/andak.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 18:25:57.000000 andak-0.0.4/andak.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 18:25:57.657421 andak-0.0.4/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2520 2023-08-05 18:25:52.000000 andak-0.0.4/setup.py
```

### Comparing `andak-0.0.3/LICENSE` & `andak-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `andak-0.0.3/andak/__init__.py` & `andak-0.0.4/andak/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,14 +15,26 @@
 ./**/*.x
 - compress x
 """ 
 
 GRepo_Saving_Progress_Lock = threading.Lock()
 GRepo_FileLogging_Lock = threading.Lock()
 
+"""
+def zip_url(self, url,commit,tag):
+	url_builder = self.furl + "/archive"
+	if self.commit:
+		url_builder += f"/{self.commit}.zip"
+	elif self.tag:
+		url_builder += f"/{self.tag}.zip"
+
+	self.zip_url_base = url_builder
+	return self.zip_url_base
+"""
+
 class GRepo_Pod(object):
 	def __init__(self, token:str=None,num_processes:int = 10, delete_paths:bool=False):
 		self.token = token
 		if "GH_TOKEN" not in os.environ:
 			self.login()
 
 		self.g = Github(self.token)
```

### Comparing `andak-0.0.3/setup.py` & `andak-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 DESCRIPTION = 'My short description for my project.'
 GH_NAME = "franceme"
 URL = f"https://github.com/{GH_NAME}/{NAME}"
 long_description = pathlib.Path(f"{here}/README.md").read_text(encoding='utf-8')
 REQUIRES_PYTHON = '>=3.8.0'
 RELEASE = "?"
 entry_point = f"src.{NAME}"
-VERSION = "0.0.3"
+VERSION = "0.0.4"
 
 def zip_program(outputName:str = f"{NAME}.zip"):
 	#http://blog.ablepear.com/2012/10/bundling-python-files-into-stand-alone.html
 	if os.path.exists(outputName):
 		os.system(f"rm {outputName}")
 
 	zipf = zipfile.ZipFile(outputName, 'w', zipfile.ZIP_DEFLATED)
```

