# Comparing `tmp/nonebot_plugin_lostark_wandering_trader-0.0.4.tar.gz` & `tmp/nonebot_plugin_lostark_wandering_trader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_lostark_wandering_trader-0.0.4.tar", last modified: Sat Aug  5 12:40:29 2023, max compression
+gzip compressed data, was "nonebot_plugin_lostark_wandering_trader-0.0.5.tar", last modified: Sat Aug  5 15:31:40 2023, max compression
```

## Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4.tar` & `nonebot_plugin_lostark_wandering_trader-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 12:40:29.002961 nonebot_plugin_lostark_wandering_trader-0.0.4/
--rw-r--r--   0 gongmin    (501) staff       (20)     5850 2023-08-05 12:40:29.002827 nonebot_plugin_lostark_wandering_trader-0.0.4/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)     4034 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/README.md
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 12:40:29.001511 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/
--rw-r--r--   0 gongmin    (501) staff       (20)    10132 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/__init__.py
--rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/config.py
-drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 12:40:29.002537 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/
--rw-r--r--   0 gongmin    (501) staff       (20)     5850 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
--rw-r--r--   0 gongmin    (501) staff       (20)      449 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
--rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      126 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
--rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-05 12:40:28.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
--rw-r--r--   0 gongmin    (501) staff       (20)      764 2023-08-05 12:37:32.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/pyproject.toml
--rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-05 12:40:29.003014 nonebot_plugin_lostark_wandering_trader-0.0.4/setup.cfg
--rw-r--r--   0 gongmin    (501) staff       (20)     1285 2023-08-05 12:37:42.000000 nonebot_plugin_lostark_wandering_trader-0.0.4/setup.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 15:31:40.854972 nonebot_plugin_lostark_wandering_trader-0.0.5/
+-rw-r--r--   0 gongmin    (501) staff       (20)     5850 2023-08-05 15:31:40.854832 nonebot_plugin_lostark_wandering_trader-0.0.5/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)     4034 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/README.md
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 15:31:40.853572 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader/
+-rw-r--r--   0 gongmin    (501) staff       (20)    10132 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader/__init__.py
+-rw-r--r--   0 gongmin    (501) staff       (20)      273 2023-08-05 12:37:24.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader/config.py
+drwxr-xr-x   0 gongmin    (501) staff       (20)        0 2023-08-05 15:31:40.854544 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/
+-rw-r--r--   0 gongmin    (501) staff       (20)     5850 2023-08-05 15:31:40.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO
+-rw-r--r--   0 gongmin    (501) staff       (20)      449 2023-08-05 15:31:40.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/SOURCES.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)        1 2023-08-05 15:31:40.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/dependency_links.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      126 2023-08-05 15:31:40.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/requires.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)       40 2023-08-05 15:31:40.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/top_level.txt
+-rw-r--r--   0 gongmin    (501) staff       (20)      764 2023-08-05 15:30:41.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/pyproject.toml
+-rw-r--r--   0 gongmin    (501) staff       (20)       38 2023-08-05 15:31:40.855026 nonebot_plugin_lostark_wandering_trader-0.0.5/setup.cfg
+-rw-r--r--   0 gongmin    (501) staff       (20)     1285 2023-08-05 15:30:46.000000 nonebot_plugin_lostark_wandering_trader-0.0.5/setup.py
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot_plugin_lostark_wandering_trader
-Version: 0.0.4
+Version: 0.0.5
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: 464723943@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot_plugin_lostark_wandering_trader Version:
-0.0.4 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.5 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: 464723943@qq.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4/README.md` & `nonebot_plugin_lostark_wandering_trader-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader/__init__.py` & `nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader/__init__.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO` & `nonebot_plugin_lostark_wandering_trader-0.0.5/nonebot_plugin_lostark_wandering_trader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-lostark-wandering-trader
-Version: 0.0.4
+Version: 0.0.5
 Summary: NoneBot lostark cn wandering trader plugin
 Home-page: https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader
 Author: EmiyaGm
 Author-email: 464723943@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
```

#### html2text {}

```diff
@@ -1,9 +1,9 @@
 Metadata-Version: 2.1 Name: nonebot-plugin-lostark-wandering-trader Version:
-0.0.4 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
+0.0.5 Summary: NoneBot lostark cn wandering trader plugin Home-page: https://
 github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader Author: EmiyaGm
 Author-email: 464723943@qq.com License: UNKNOWN Project-URL: Bug Tracker,
 https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader/issues
 Description:
                                    [nonebot]
             # nonebot-plugin-lostark-wandering-trader _â¨ NoneBot
                å½è¿æ¹èå½ææµæµªåäººå·æ°æ¶é´æ¥ç
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4/pyproject.toml` & `nonebot_plugin_lostark_wandering_trader-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot_plugin_lostark_wandering_trader"
-version = "0.0.4"
+version = "0.0.5"
 description = "NoneBot lostark cn wandering trader plugin"
 authors = [
     {name = "EmiyaGm", email = "464723943@qq.com"},
 ]
 dependencies = [
     "httpx<1.0.0,>=0.18.0",
     "nonebot_plugin_apscheduler>=0.3.0",
```

### Comparing `nonebot_plugin_lostark_wandering_trader-0.0.4/setup.py` & `nonebot_plugin_lostark_wandering_trader-0.0.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     with io.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
         long_description = '\n' + f.read()
 except FileNotFoundError:
     long_description = "NoneBot lostark cn wandering trader plugin"
 
 setuptools.setup(
     name="nonebot_plugin_lostark_wandering_trader",
-    version="0.0.4",
+    version="0.0.5",
     author="EmiyaGm",
     author_email="464723943@qq.com",
     description="NoneBot lostark cn wandering trader plugin",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/EmiyaGm/nonebot-plugin-lostark-wandering-trader",
     project_urls={
```

