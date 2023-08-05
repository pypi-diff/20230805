# Comparing `tmp/pyggc-1.0.0.tar.gz` & `tmp/pyggc-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/py-git-ghcli/py-git-ghcli/dist/.tmp-1ryruiga/pyggc-1.0.0.tar", last modified: Sat Aug  5 09:33:47 2023, max compression
+gzip compressed data, was "/home/runner/work/py-git-ghcli/py-git-ghcli/dist/.tmp-my6lgig7/pyggc-1.1.0.tar", last modified: Sat Aug  5 13:21:40 2023, max compression
```

## Comparing `pyggc-1.0.0.tar` & `pyggc-1.1.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:47.000000 pyggc-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-05 09:33:39.000000 pyggc-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-05 09:33:47.000000 pyggc-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-08-05 09:33:39.000000 pyggc-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc/ghcli/
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-08-05 09:33:39.000000 pyggc-1.0.0/pyggc/ghcli/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc/git/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-05 09:33:39.000000 pyggc-1.0.0/pyggc/git/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 09:33:47.000000 pyggc-1.0.0/pyggc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-05 09:33:40.000000 pyggc-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 09:33:47.000000 pyggc-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:21:40.000000 pyggc-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-08-05 13:21:34.000000 pyggc-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-05 13:21:40.000000 pyggc-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-08-05 13:21:34.000000 pyggc-1.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc/ghcli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-08-05 13:21:34.000000 pyggc-1.1.0/pyggc/ghcli/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc/git/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-08-05 13:21:34.000000 pyggc-1.1.0/pyggc/git/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 13:21:40.000000 pyggc-1.1.0/pyggc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-05 13:21:34.000000 pyggc-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:21:40.000000 pyggc-1.1.0/setup.cfg
```

### Comparing `pyggc-1.0.0/LICENSE` & `pyggc-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyggc-1.0.0/PKG-INFO` & `pyggc-1.1.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,11 @@
-Metadata-Version: 2.1
-Name: pyggc
-Version: 1.0.0
-Summary: Bunch of Python functions for Git and GitHub CLI tasks.
-Author-email: Nicholas Valentinus <nicho@scapeville.com>
-License: MIT
-Project-URL: Repository, https://github.com/scapeville/py-git-ghcli
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Py-Git-GhCli
 
+[![Run tests](https://github.com/scapeville/py-git-ghcli/actions/workflows/run-tests.yml/badge.svg)](https://github.com/scapeville/py-git-ghcli/actions/workflows/run-tests.yml)
+
 Bunch of Python functions for Git and GitHub CLI tasks.
 
 
 ## Install
 
 ```shell
 pip install pyggc
@@ -45,8 +36,8 @@
 stars = get_stargazers(owner='scapeville', repo='py-git-ghcli')
 print(stars)
 ```
 
 
 ## License
 
-The scripts and documentation in this project are released under the MIT License.
+The scripts and documentation in this project are released under the MIT License.
```

### Comparing `pyggc-1.0.0/pyggc/ghcli/simple.py` & `pyggc-1.1.0/pyggc/ghcli/simple.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,68 @@
 import json as _json
 import subprocess as _sp
+from typing import (
+    Dict as _Dict
+)
 
 
 def total_stargazers(owner:str, *, gh_cli_bin:str='gh') -> int:
-    """Get the total stargazers count for all `owner` GitHub public repos"""
+    """
+    Get the total stargazers count for all `owner` GitHub public repos
+
+    ---
+
+    ## Params
+    - `owner`: GitHub username
+
+    ## Exceptions
+    - `subprocess.CalledProcessError`: if `owner` is not found
+    """
 
     cmd = [gh_cli_bin, 'repo', 'list', owner, '--visibility', 'public', '--json', 'stargazerCount']
     output = _sp.check_output(cmd, text=True)
 
     parsed = _json.loads(output)
     num_stargazers = sum([d['stargazerCount'] for d in parsed])
 
     return num_stargazers
 
 
-def get_stargazers(owner:str, repo:str, *, gh_cli_bin:str='gh') -> int:
+def pack_stargazers(owner:str, *, gh_cli_bin:str='gh') -> _Dict[str, int]:
     """
-    Get GitHub repo stargazers count.
+    Return a dictionary of stargazer counts for every repository
 
     ---
 
     ## Params
     - `owner`: GitHub username
-    - `repo` : GitHub repository name
+
+    ## Exceptions
+    - `subprocess.CalledProcessError`: if `owner` is not found
     """
 
     cmd = [gh_cli_bin, 'repo', 'list', owner, '--visibility', 'public', '--json', 'name,stargazerCount']
     output = _sp.check_output(cmd, text=True)
 
     parsed = _json.loads(output)
-    transformed = {d['name']: d['stargazerCount'] for d in parsed}
-    num_stargazers = transformed[repo]
+    pack = {d['name']: d['stargazerCount'] for d in parsed}
+
+    return pack
 
+
+def get_stargazers(owner:str, repo:str, *, gh_cli_bin:str='gh') -> int:
+    """
+    Get GitHub repo stargazers count.
+
+    ---
+
+    ## Params
+    - `owner`: GitHub username
+    - `repo` : GitHub repository name
+
+    ## Exceptions
+    - `subprocess.CalledProcessError`: if `owner` is not found
+    - `KeyError`: if `repo` is not found
+    """
+    pack = pack_stargazers(owner)
+    num_stargazers = pack[repo]
     return num_stargazers
```

### Comparing `pyggc-1.0.0/pyggc/git/simple.py` & `pyggc-1.1.0/pyggc/git/simple.py`

 * *Files identical despite different names*

### Comparing `pyggc-1.0.0/pyggc.egg-info/PKG-INFO` & `pyggc-1.1.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: pyggc
-Version: 1.0.0
+Version: 1.1.0
 Summary: Bunch of Python functions for Git and GitHub CLI tasks.
 Author-email: Nicholas Valentinus <nicho@scapeville.com>
 License: MIT
 Project-URL: Repository, https://github.com/scapeville/py-git-ghcli
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Py-Git-GhCli
 
+[![Run tests](https://github.com/scapeville/py-git-ghcli/actions/workflows/run-tests.yml/badge.svg)](https://github.com/scapeville/py-git-ghcli/actions/workflows/run-tests.yml)
+
 Bunch of Python functions for Git and GitHub CLI tasks.
 
 
 ## Install
 
 ```shell
 pip install pyggc
```

