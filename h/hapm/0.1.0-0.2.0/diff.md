# Comparing `tmp/hapm-0.1.0.tar.gz` & `tmp/hapm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hapm-0.1.0.tar", last modified: Wed Aug  2 15:27:54 2023, max compression
+gzip compressed data, was "hapm-0.2.0.tar", last modified: Sat Aug  5 12:02:42 2023, max compression
```

## Comparing `hapm-0.1.0.tar` & `hapm-0.2.0.tar`

### file list

```diff
@@ -1,49 +1,72 @@
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.596918 hapm-0.1.0/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1378 2023-08-02 15:27:54.596788 hapm-0.1.0/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1018 2023-08-02 15:17:37.000000 hapm-0.1.0/README.md
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.596474 hapm-0.1.0/hapm.egg-info/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1378 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/PKG-INFO
--rw-r--r--   0 mishamyrt   (501) staff       (20)      948 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/SOURCES.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/dependency_links.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)      103 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/requires.txt
--rw-r--r--   0 mishamyrt   (501) staff       (20)        8 2023-08-02 15:27:54.000000 hapm-0.1.0/hapm.egg-info/top_level.txt
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.591749 hapm-0.1.0/libhapm/
--rw-r--r--   0 mishamyrt   (501) staff       (20)        0 2023-02-17 18:11:43.000000 hapm-0.1.0/libhapm/__init__.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.593304 hapm-0.1.0/libhapm/cli/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      223 2023-08-02 15:03:05.000000 hapm-0.1.0/libhapm/cli/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      390 2023-02-22 19:26:44.000000 hapm-0.1.0/libhapm/cli/ink.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1314 2023-02-25 20:31:31.000000 hapm-0.1.0/libhapm/cli/report_diff.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      200 2023-08-02 13:05:34.000000 hapm-0.1.0/libhapm/cli/report_error.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:31:45.000000 hapm-0.1.0/libhapm/cli/report_list.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      443 2023-02-22 22:14:02.000000 hapm-0.1.0/libhapm/cli/report_no_token.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      930 2023-02-22 20:03:50.000000 hapm-0.1.0/libhapm/cli/report_summary.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      637 2023-02-25 10:20:29.000000 hapm-0.1.0/libhapm/cli/utils.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.593957 hapm-0.1.0/libhapm/github/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      147 2023-02-25 20:18:07.000000 hapm-0.1.0/libhapm/github/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      871 2023-02-25 20:12:15.000000 hapm-0.1.0/libhapm/github/file.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      325 2023-02-25 20:17:01.000000 hapm-0.1.0/libhapm/github/path.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      422 2023-02-25 20:18:42.000000 hapm-0.1.0/libhapm/github/tarball.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.594243 hapm-0.1.0/libhapm/integration/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       71 2023-02-25 10:15:54.000000 hapm-0.1.0/libhapm/integration/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2142 2023-02-26 16:02:42.000000 hapm-0.1.0/libhapm/integration/package.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.594732 hapm-0.1.0/libhapm/manager/
--rw-r--r--   0 mishamyrt   (501) staff       (20)     5085 2023-08-02 13:59:45.000000 hapm-0.1.0/libhapm/manager/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      301 2023-02-22 12:53:26.000000 hapm-0.1.0/libhapm/manager/diff.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      985 2023-02-21 10:33:48.000000 hapm-0.1.0/libhapm/manager/lockfile.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.595176 hapm-0.1.0/libhapm/manifest/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       31 2023-02-20 20:36:51.000000 hapm-0.1.0/libhapm/manifest/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      850 2023-08-02 13:04:20.000000 hapm-0.1.0/libhapm/manifest/manifest.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1107 2023-02-25 11:28:23.000000 hapm-0.1.0/libhapm/manifest/parse.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.595577 hapm-0.1.0/libhapm/package/
--rw-r--r--   0 mishamyrt   (501) staff       (20)      101 2023-02-25 20:13:51.000000 hapm-0.1.0/libhapm/package/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2318 2023-08-02 14:20:33.000000 hapm-0.1.0/libhapm/package/base.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      210 2023-02-25 10:18:53.000000 hapm-0.1.0/libhapm/package/description.py
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.595841 hapm-0.1.0/libhapm/plugin/
--rw-r--r--   0 mishamyrt   (501) staff       (20)       35 2023-08-02 13:59:58.000000 hapm-0.1.0/libhapm/plugin/__init__.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)     2942 2023-08-02 15:16:29.000000 hapm-0.1.0/libhapm/plugin/package.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      961 2023-02-20 20:57:56.000000 hapm-0.1.0/libhapm/versions.py
--rw-r--r--   0 mishamyrt   (501) staff       (20)      397 2023-02-20 20:34:09.000000 hapm-0.1.0/pyproject.toml
-drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-02 15:27:54.596597 hapm-0.1.0/scripts/
--rwxr-xr-x   0 mishamyrt   (501) staff       (20)     1937 2023-08-02 14:16:54.000000 hapm-0.1.0/scripts/hapm
--rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-08-02 15:27:54.596966 hapm-0.1.0/setup.cfg
--rw-r--r--   0 mishamyrt   (501) staff       (20)     1097 2023-08-02 12:19:44.000000 hapm-0.1.0/setup.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.919808 hapm-0.2.0/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.909875 hapm-0.2.0/.github/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.912710 hapm-0.2.0/.github/workflows/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      302 2023-08-05 10:46:22.000000 hapm-0.2.0/.github/workflows/qa.yaml
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      112 2023-08-05 10:29:45.000000 hapm-0.2.0/.gitignore
+-rw-r--r--   0 mishamyrt   (501) staff       (20)    21221 2023-08-05 10:42:30.000000 hapm-0.2.0/.pylintrc
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        6 2023-08-05 12:02:37.000000 hapm-0.2.0/.version
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1073 2023-08-03 13:31:08.000000 hapm-0.2.0/LICENSE
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      870 2023-08-05 12:02:20.000000 hapm-0.2.0/Makefile
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1506 2023-08-05 12:02:42.919644 hapm-0.2.0/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1112 2023-08-05 11:55:11.000000 hapm-0.2.0/README.md
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      138 2023-08-03 13:31:29.000000 hapm-0.2.0/cspell.json
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1178 2023-08-03 13:58:08.000000 hapm-0.2.0/pyproject.toml
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      179 2023-08-03 13:45:10.000000 hapm-0.2.0/requirements.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       38 2023-08-05 12:02:42.919867 hapm-0.2.0/setup.cfg
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.910109 hapm-0.2.0/src/
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.913123 hapm-0.2.0/src/hapm/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        0 2023-02-17 18:11:43.000000 hapm-0.2.0/src/hapm/__init__.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.914815 hapm-0.2.0/src/hapm/cli/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1240 2023-08-05 11:54:18.000000 hapm-0.2.0/src/hapm/cli/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1300 2023-08-05 11:58:36.000000 hapm-0.2.0/src/hapm/cli/common.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      321 2023-08-05 10:23:51.000000 hapm-0.2.0/src/hapm/cli/export.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1423 2023-08-05 11:44:02.000000 hapm-0.2.0/src/hapm/cli/install.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1557 2023-08-05 11:23:46.000000 hapm-0.2.0/src/hapm/cli/versions.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.915251 hapm-0.2.0/src/hapm/color/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      167 2023-08-03 14:15:49.000000 hapm-0.2.0/src/hapm/color/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      151 2023-08-03 14:13:23.000000 hapm-0.2.0/src/hapm/color/constants.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      406 2023-08-03 14:14:34.000000 hapm-0.2.0/src/hapm/color/ink.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.916001 hapm-0.2.0/src/hapm/git/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      171 2023-08-04 22:51:18.000000 hapm-0.2.0/src/hapm/git/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      900 2023-08-04 23:07:07.000000 hapm-0.2.0/src/hapm/git/file.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      161 2023-08-04 22:50:23.000000 hapm-0.2.0/src/hapm/git/path.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      422 2023-02-25 20:18:42.000000 hapm-0.2.0/src/hapm/git/tarball.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      422 2023-08-04 19:14:41.000000 hapm-0.2.0/src/hapm/git/versions.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.916275 hapm-0.2.0/src/hapm/integration/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       71 2023-02-25 10:15:54.000000 hapm-0.2.0/src/hapm/integration/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2133 2023-08-03 14:00:53.000000 hapm-0.2.0/src/hapm/integration/package.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.916696 hapm-0.2.0/src/hapm/manager/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     5766 2023-08-05 11:52:30.000000 hapm-0.2.0/src/hapm/manager/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      298 2023-08-03 13:57:19.000000 hapm-0.2.0/src/hapm/manager/diff.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      982 2023-08-03 13:57:19.000000 hapm-0.2.0/src/hapm/manager/lockfile.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.917252 hapm-0.2.0/src/hapm/manifest/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      149 2023-08-04 22:31:50.000000 hapm-0.2.0/src/hapm/manifest/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      805 2023-08-04 23:56:48.000000 hapm-0.2.0/src/hapm/manifest/category.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2647 2023-08-04 23:05:51.000000 hapm-0.2.0/src/hapm/manifest/location.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2504 2023-08-05 11:49:44.000000 hapm-0.2.0/src/hapm/manifest/manifest.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.917708 hapm-0.2.0/src/hapm/package/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      101 2023-02-25 20:13:51.000000 hapm-0.2.0/src/hapm/package/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2789 2023-08-05 10:37:08.000000 hapm-0.2.0/src/hapm/package/base.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      210 2023-02-25 10:18:53.000000 hapm-0.2.0/src/hapm/package/description.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.918019 hapm-0.2.0/src/hapm/plugin/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       60 2023-08-05 10:33:54.000000 hapm-0.2.0/src/hapm/plugin/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     2928 2023-08-03 14:16:13.000000 hapm-0.2.0/src/hapm/plugin/package.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.919251 hapm-0.2.0/src/hapm/report/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      320 2023-08-04 23:54:42.000000 hapm-0.2.0/src/hapm/report/__init__.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1876 2023-08-04 23:29:22.000000 hapm-0.2.0/src/hapm/report/diff.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1771 2023-08-05 10:36:19.000000 hapm-0.2.0/src/hapm/report/errors.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1284 2023-08-04 23:12:35.000000 hapm-0.2.0/src/hapm/report/lists.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1716 2023-08-05 10:36:37.000000 hapm-0.2.0/src/hapm/report/progress.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      932 2023-08-03 14:36:29.000000 hapm-0.2.0/src/hapm/report/summary.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      634 2023-08-04 22:57:26.000000 hapm-0.2.0/src/hapm/report/utils.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      187 2023-08-04 23:06:25.000000 hapm-0.2.0/src/hapm/repository.py
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      898 2023-08-04 22:21:06.000000 hapm-0.2.0/src/hapm/versions.py
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.914030 hapm-0.2.0/src/hapm.egg-info/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1506 2023-08-05 12:02:42.000000 hapm-0.2.0/src/hapm.egg-info/PKG-INFO
+-rw-r--r--   0 mishamyrt   (501) staff       (20)     1309 2023-08-05 12:02:42.000000 hapm-0.2.0/src/hapm.egg-info/SOURCES.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        1 2023-08-05 12:02:42.000000 hapm-0.2.0/src/hapm.egg-info/dependency_links.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)       40 2023-08-05 12:02:42.000000 hapm-0.2.0/src/hapm.egg-info/entry_points.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      103 2023-08-05 12:02:42.000000 hapm-0.2.0/src/hapm.egg-info/requires.txt
+-rw-r--r--   0 mishamyrt   (501) staff       (20)        5 2023-08-05 12:02:42.000000 hapm-0.2.0/src/hapm.egg-info/top_level.txt
+drwxr-xr-x   0 mishamyrt   (501) staff       (20)        0 2023-08-05 12:02:42.919399 hapm-0.2.0/testdata/
+-rw-r--r--   0 mishamyrt   (501) staff       (20)      149 2023-08-05 11:44:53.000000 hapm-0.2.0/testdata/hapm.yaml
```

### Comparing `hapm-0.1.0/README.md` & `hapm-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -15,44 +15,53 @@
 For example: `github.com/user/integration@v1.0.0`.
 
 The version specifies an existing tag or branch in the specified repository.
 
 A link may not have an https prefix, in which case it will be inserted automatically during the reading phase.
 
 ```yaml
----
 integrations:
   - github.com/mishamyrt/dohome_rgb@v0.3.0
   - github.com/mishamyrt/myrt_desk_hass@master
 ```
 
+## Initialize empty config
+
+```sh
+hapm init
+```
+
 ## Sync remote packages
 
 ```sh
-hapm
+hapm sync
 ```
 
 ## Export 
 
 ```sh
-hapm put <path>
+hapm export <path>
 ```
 
 ## List 
 
 ```sh
 hapm list
 ```
 
 ## Add new package
 
-**not yet implemented**
+```sh
+hapm install -t integrations mishamyrt/assisted_pol@v0.2.4
+```
+
+## Update package
 
 ```sh
-hapm get -t integration https://github.com/AlexxIT/XiaomiGateway3
+hapm install mishamyrt/assisted_pol@v0.2.4
 ```
 
 ## Updates
 
 ```sh
 # Prints updates
 hapm updates
```

### Comparing `hapm-0.1.0/libhapm/cli/report_diff.py` & `hapm-0.2.0/src/hapm/report/diff.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,44 +1,56 @@
 """HAPM CLI diff reporter"""
 from __future__ import annotations
 
 from typing import List
 
-from libhapm.github import repo_name
-from libhapm.manager.diff import PackageDiff
+from hapm.color import ANSI_DIM, ANSI_GREEN, ANSI_RED, ANSI_YELLOW, ink
+from hapm.manager.diff import PackageDiff
+from hapm.repository import repo_name
 
-from .ink import ANSI_DIM, ANSI_GREEN, ANSI_RED, ANSI_YELLOW, ink
 from .utils import group_by_kind
 
 
 def _format_kind(kind: str) -> str:
     return ink(kind.capitalize() + ":", effects=ANSI_DIM)
 
+def _format_update(diff: PackageDiff) -> str:
+    full_name = diff["full_name"]
+    next_version = ink(diff["version"], ANSI_YELLOW)
+    current_version = ink(f"({diff['current_version']})", effects=ANSI_DIM)
+    delimiter = ink("@", effects=ANSI_DIM)
+    return f"{full_name}{delimiter}{next_version} {current_version}"
 
-def _format_entry(diff: PackageDiff) -> str:
+def _format_entry(diff: PackageDiff, full_name: bool) -> str:
     version = diff["version"]
     if diff["operation"] == "add":
         prefix = "+"
         color = ANSI_GREEN
         version = ink(version, effects=ANSI_DIM)
     elif diff["operation"] == "switch":
         prefix = "*"
         color = ANSI_YELLOW
         version = f"{ink(diff['current_version'], effects=ANSI_DIM)} → {version}"
     else:
         prefix = "-"
         color = ANSI_RED
         version = ink(version, effects=ANSI_DIM)
-    name = repo_name(diff["full_name"])
+    if full_name:
+        name = diff["full_name"]
+    else:
+        name = repo_name(diff["full_name"])
     title = ink(f"{prefix} {name}", color=color)
-    return f"{title} {version}"
+    return f"{title}@{version}"
 
 
-def report_diff(diff: List[PackageDiff]):
+def report_diff(diff: List[PackageDiff], full_name=False, updates_only=False):
     """Prints in stdout diff of packages in a nice way"""
     groups = group_by_kind(diff)
     log = ""
     for kind, packages in groups.items():
         log += f"{_format_kind(kind)}\n"
         for package in packages:
-            log += f"{_format_entry(package)}\n"
+            if updates_only:
+                log += f"  {_format_update(package)}\n"
+            else:
+                log += f"{_format_entry(package, full_name)}\n"
     print(log, end="\r")
```

### Comparing `hapm-0.1.0/libhapm/cli/report_list.py` & `hapm-0.2.0/src/hapm/report/lists.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,42 @@
-"""HAPM CLI list reporter"""
+"""HAPM CLI lists reporter"""
 from __future__ import annotations
 
 from typing import List
 
-from libhapm.github import repo_name
-from libhapm.package import PackageDescription
+from hapm.color import ANSI_DIM, ANSI_YELLOW, ink
+from hapm.package import PackageDescription
 
-from .ink import ANSI_DIM, ink
 from .utils import group_by_kind
 
 
 def _format_kind(kind: str) -> str:
     return ink(kind.capitalize() + ":", effects=ANSI_DIM)
 
 
-def _format_entry(package: PackageDescription) -> str:
-    name = repo_name(package["full_name"])
-    version = ink(package["version"], effects=ANSI_DIM)
-    return f"  {name} {version}"
+def _format_package(package: PackageDescription) -> str:
+    name = package["full_name"]
+    version = ink(f"@{package['version']}", effects=ANSI_DIM)
+    return f"  {name}{version}"
+
+def _format_version(package: str, version: str) -> str:
+    line = ink(f"- {package}@", effects=ANSI_DIM)
+    line += ink(version, ANSI_YELLOW)
+    return line
 
 
-def report_list(diff: List[PackageDescription]):
+def report_packages(diff: List[PackageDescription]) -> None:
     """Prints into stdout list of packages in a nice way"""
     groups = group_by_kind(diff)
     log = ""
     for kind, packages in groups.items():
         log += f"{_format_kind(kind)}\n"
         for package in packages:
-            log += f"{_format_entry(package)}\n"
+            log += f"{_format_package(package)}\n"
     print(log, end="\r")
+
+def report_versions(package: str, versions: List[str]) -> None:
+    """Prints package versions in a format suitable for installation"""
+    content = ""
+    for version in versions:
+        content += _format_version(package, version) + "\n"
+    print(content)
```

### Comparing `hapm-0.1.0/libhapm/cli/report_summary.py` & `hapm-0.2.0/src/hapm/report/summary.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """HAPM CLI summary reporter"""
 
 from typing import List
 
-from libhapm.manager.diff import PackageDiff
-
-from .ink import ANSI_B_CYAN, ink
+from hapm.color import ANSI_B_CYAN, ink
+from hapm.manager.diff import PackageDiff
 
 
 def report_summary(diff: List[PackageDiff]):
     """Prints the result of the successful work into the stdout"""
     if len(diff) == 0:
         print("There's nothing to do here")
         return
```

### Comparing `hapm-0.1.0/libhapm/cli/utils.py` & `hapm-0.2.0/src/hapm/report/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """HAPM CLI common utils"""
 from __future__ import annotations
 
 from typing import Dict, List
 
-from libhapm.package import PackageDescription
+from hapm.package import PackageDescription
 
 
 def group_by_kind(packages: List[PackageDescription]) -> Dict[str, List[PackageDescription]]:
     """Groups packages by kind. Returns a dictionary,
     where the key is the kind and the value is an array of packages of the appropriate kind"""
     groups: Dict[str, List[PackageDescription]] = {}
     for package in packages:
```

### Comparing `hapm-0.1.0/libhapm/github/file.py` & `hapm-0.2.0/src/hapm/git/file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """HAPM Github file utils"""
 from __future__ import annotations
 
 from base64 import b64decode
 
-from github import GithubException, Repository
+from github import GithubException
+from github.Repository import Repository
 from requests import get
 
 
 def get_tree_file(repo: Repository, branch: str, path: str) -> str | None:
     """Gets the file from the repository by path and returns its string content."""
     try:
         content = repo.get_contents(path, ref=branch)
```

### Comparing `hapm-0.1.0/libhapm/integration/package.py` & `hapm-0.2.0/src/hapm/integration/package.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from __future__ import annotations
 
 import tarfile
 from os import listdir, mkdir, remove
 from os.path import join
 from shutil import copytree, rmtree
 
-from libhapm.github import get_tarball
-from libhapm.package import BasePackage
+from hapm.git import get_tarball
+from hapm.package import BasePackage
 
 FOLDER_NAME = "custom_components"
 
 
 class IntegrationPackage(BasePackage):
     """IntegrationPackage represent custom_components packages"""
```

### Comparing `hapm-0.1.0/libhapm/manager/__init__.py` & `hapm-0.2.0/src/hapm/manager/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """HAPM manager module"""
 from os import mkdir
 from os.path import isdir, join
 from shutil import rmtree
 from typing import Dict, List
 
-from github import Github
-
-from libhapm.integration import IntegrationPackage
-from libhapm.package import BasePackage, PackageDescription
-from libhapm.plugin import PluginPackage
-from libhapm.versions import is_newer
+from hapm.git import get_versions
+from hapm.integration import IntegrationPackage
+from hapm.manifest import Manifest, PackageLocation
+from hapm.package import BasePackage, PackageDescription
+from hapm.plugin import PluginPackage
+from hapm.versions import find_latest, is_newer
 
 from .diff import PackageDiff
 from .lockfile import Lockfile
 
 PACKAGE_HANDLERS = {
     IntegrationPackage.kind: IntegrationPackage,
     PluginPackage.kind: PluginPackage
@@ -35,42 +35,52 @@
 
         if isdir(self._path):
             if self._lock.exists():
                 self._boot_from_lock()
         else:
             mkdir(self._path)
 
+    def supported_types(self) -> List[str]:
+        """Returns supported types"""
+        return list(PACKAGE_HANDLERS.keys())
+
+    def get_versions(self, location: PackageLocation) -> List[str]:
+        """Returns package version by location"""
+        return get_versions(location["full_name"], self._api_token)
+
     def _boot_from_lock(self):
         descriptions = self._lock.load()
         if len(descriptions) == 0:
             return
         for description in descriptions:
             package = PACKAGE_HANDLERS[description["kind"]](
                 description, self._path, self._api_token)
             self._packages[package.full_name] = package
 
-    def diff(self, update: List[PackageDescription]) -> List[PackageDiff]:
+    def diff(self, update: List[PackageDescription], stable_only=True) -> List[PackageDiff]:
         """Finds the difference between the current state and the list of packets received.
         Returns the modified package description"""
         update_full_names: List[str] = []
         diffs: List[PackageDiff] = []
         for description in update:
+            if description["version"] == "latest":
+                versions = get_versions(description["full_name"], self._api_token)
+                description["version"] = find_latest(versions, stable_only)
             full_name, version = description["full_name"], description["version"]
             update_full_names.append(full_name)
             diff: PackageDiff = description.copy()
             if full_name in self._packages:
                 current_version = self._packages[full_name].version
-                if current_version == version:
-                    continue
-                else:
+                if current_version != version:
                     diff["current_version"] = current_version
                     diff["operation"] = "switch"
             else:
                 diff["operation"] = "add"
-            diffs.append(diff)
+            if "operation" in diff:
+                diffs.append(diff)
         for (full_name, integration) in self._packages.items():
             try:
                 if update_full_names.index(full_name):
                     continue
             except ValueError:
                 diff: PackageDiff = integration.description()
                 diff["operation"] = "delete"
@@ -81,24 +91,26 @@
         """Applies the new configuration.
         Important: this method will make changes to the file system.
         Returns False if no changes were made."""
         full_names_to_remove = []
         for diff in diffs:
             operation = diff["operation"]
             full_name = diff["full_name"]
+            version = diff["version"]
             if operation == "add":
                 package = PACKAGE_HANDLERS[diff["kind"]](
                     diff, self._path, self._api_token)
-                package.initialize()
+                package.setup()
                 self._packages[full_name] = package
             elif operation == "delete":
                 self._packages[full_name].destroy()
                 full_names_to_remove.append(full_name)
             else:
-                self._packages[full_name].switch(diff["version"])
+                package = self._packages[full_name]
+                package.switch(version)
         # Delete keys in a separate loop so as not to change the iterated list
         for full_name in full_names_to_remove:
             self._packages.pop(full_name, None)
         self._lock.dump(self.descriptions())
 
     def export(self, path: str):
         """Deletes the package from the file system"""
@@ -110,19 +122,20 @@
             if integration.kind not in kinds:
                 kinds.append(integration.kind)
                 PACKAGE_HANDLERS[integration.kind].pre_export(path)
             integration.export(path)
         for kind in kinds:
             PACKAGE_HANDLERS[kind].post_export(path)
 
-    def updates(self) -> List[PackageDiff]:
+
+    def updates(self, stable_only=True) -> List[PackageDiff]:
         """Searches for updates for packages, returns list of available updates."""
         updates: List[PackageDiff] = []
         for (_, package) in self._packages.items():
-            latest_version = package.latest_version()
+            latest_version = package.latest_version(stable_only)
             if is_newer(package.version, latest_version):
                 updates.append({
                     "full_name": package.full_name,
                     "kind": package.kind,
                     "version": latest_version,
                     "current_version": package.version,
                     "operation": "switch"
```

### Comparing `hapm-0.1.0/libhapm/manager/lockfile.py` & `hapm-0.2.0/src/hapm/manager/lockfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """HAPM lockfile module"""
 from __future__ import annotations
 
 from json import dump, load
 from os.path import isfile
 from typing import List
 
-from libhapm.package import PackageDescription
+from hapm.package import PackageDescription
 
 
 class Lockfile:
     """Represents an entity that manages a file with descriptions of current package versions"""
     _path: str
     _encoding: str
```

### Comparing `hapm-0.1.0/libhapm/package/base.py` & `hapm-0.2.0/src/hapm/package/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """HAPM package"""
 from __future__ import annotations
 
 from os import remove
 from os.path import join
 
-from libhapm.github import repo_name
+from hapm.git import get_versions
+from hapm.repository import repo_name
+from hapm.versions import find_latest
 
 from .description import PackageDescription
 
 
 class BasePackage:
     """This is an abstract package controller class.
     The class that implements it must be able to control a certain type of package"""
@@ -49,14 +51,26 @@
             version = self.version
         return f"{self.basepath}@{version}.{self.extension}"
 
     def destroy(self) -> None:
         """Deletes the package from the file system"""
         remove(self.path())
 
+    def latest_version(self, stable_only=True) -> str:
+        """Finds the latest available version"""
+        versions = get_versions(self.full_name, self._api_token)
+        return find_latest(versions, stable_only)
+
+    def setup(self) -> None:
+        """Initializes package"""
+        if self.version == "latest":
+            raise TypeError("version is unknown")
+        self.initialize()
+
+
     # Abstract methods to be implemented by all types of package handlers
 
     def initialize(self) -> None:
         """Method will be called if the entity is created for the first time.
         It should initialise the files on the system"""
 
     def switch(self, version: str) -> None:
```

### Comparing `hapm-0.1.0/libhapm/plugin/package.py` & `hapm-0.2.0/src/hapm/plugin/package.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,17 +5,17 @@
 from os.path import join
 from pathlib import Path
 from shutil import copyfile
 
 from git import Repo
 from github import Github
 
-from libhapm.github import get_release_file, get_tree_file
-from libhapm.cli.ink import ink, ANSI_YELLOW, ANSI_DIM
-from libhapm.package import BasePackage
+from hapm.color import ANSI_DIM, ANSI_YELLOW, ink
+from hapm.git import get_release_file, get_tree_file
+from hapm.package import BasePackage
 
 FOLDER_NAME = "www/custom_lovelace"
 RESOURCES_REDIRECT_URL = "https://my.home-assistant.io/redirect/lovelace_resources/"
 
 
 class PluginPackage(BasePackage):
     """PluginPackage represent `.js` plugin packages"""
```

