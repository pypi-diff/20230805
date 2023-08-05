# Comparing `tmp/flux-local-3.1.0.tar.gz` & `tmp/flux-local-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-3.1.0.tar", last modified: Thu Jul 20 05:41:16 2023, max compression
+gzip compressed data, was "flux-local-3.1.1.tar", last modified: Sat Aug  5 20:44:01 2023, max compression
```

## Comparing `flux-local-3.1.0.tar` & `flux-local-3.1.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:41:16.216361 flux-local-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-20 05:40:58.000000 flux-local-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-07-20 05:41:16.216361 flux-local-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-07-20 05:40:58.000000 flux-local-3.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:41:16.208361 flux-local-3.1.0/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    23062 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9918 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:41:16.212361 flux-local-3.1.0/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-07-20 05:40:58.000000 flux-local-3.1.0/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:41:16.212361 flux-local-3.1.0/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-07-20 05:41:16.000000 flux-local-3.1.0/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-07-20 05:41:16.000000 flux-local-3.1.0/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 05:41:16.000000 flux-local-3.1.0/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-20 05:41:16.000000 flux-local-3.1.0/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 05:41:16.000000 flux-local-3.1.0/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 05:41:16.000000 flux-local-3.1.0/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-07-20 05:41:16.216361 flux-local-3.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-20 05:40:58.000000 flux-local-3.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 05:41:16.216361 flux-local-3.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-20 05:40:58.000000 flux-local-3.1.0/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-07-20 05:40:58.000000 flux-local-3.1.0/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-20 05:40:58.000000 flux-local-3.1.0/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-07-20 05:40:58.000000 flux-local-3.1.0/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-20 05:40:58.000000 flux-local-3.1.0/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:44:01.411154 flux-local-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 20:43:51.000000 flux-local-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-08-05 20:44:01.411154 flux-local-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11841 2023-08-05 20:43:51.000000 flux-local-3.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:44:01.411154 flux-local-3.1.1/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23062 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7393 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9880 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16252 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:44:01.411154 flux-local-3.1.1/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16498 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7387 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7425 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14123 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10931 2023-08-05 20:43:51.000000 flux-local-3.1.1/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:44:01.411154 flux-local-3.1.1/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-08-05 20:44:01.000000 flux-local-3.1.1/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-08-05 20:44:01.000000 flux-local-3.1.1/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 20:44:01.000000 flux-local-3.1.1/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-05 20:44:01.000000 flux-local-3.1.1/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 20:44:01.000000 flux-local-3.1.1/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 20:44:01.000000 flux-local-3.1.1/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-08-05 20:44:01.411154 flux-local-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-05 20:43:51.000000 flux-local-3.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 20:44:01.411154 flux-local-3.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-05 20:43:51.000000 flux-local-3.1.1/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-08-05 20:43:51.000000 flux-local-3.1.1/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-08-05 20:43:51.000000 flux-local-3.1.1/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5825 2023-08-05 20:43:51.000000 flux-local-3.1.1/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-08-05 20:43:51.000000 flux-local-3.1.1/tests/test_manifest.py
```

### Comparing `flux-local-3.1.0/LICENSE` & `flux-local-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/PKG-INFO` & `flux-local-3.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 3.1.0
+Version: 3.1.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux-local-3.1.0/README.md` & `flux-local-3.1.1/README.md`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/command.py` & `flux-local-3.1.1/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/exceptions.py` & `flux-local-3.1.1/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/git_repo.py` & `flux-local-3.1.1/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/helm.py` & `flux-local-3.1.1/flux_local/helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/kustomize.py` & `flux-local-3.1.1/flux_local/kustomize.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     # Every file resource is read and output
     # Every directory is kustomized
     tasks = []
     filenames = list(await listdir(path))
     filenames.sort()
     for filename in filenames:
         new_path = path / filename
-        if new_path.is_dir() and await can_kustomize_dir(new_path):
+        if new_path.is_dir():
             tasks.append(build(new_path).objects())
         elif filename.endswith(".yaml") or filename.endswith(".yml"):
             tasks.append(yaml_load_all(new_path))
         else:
             continue
 
     results = await asyncio.gather(*tasks)
```

### Comparing `flux-local-3.1.0/flux_local/manifest.py` & `flux-local-3.1.1/flux_local/manifest.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/build.py` & `flux-local-3.1.1/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/diff.py` & `flux-local-3.1.1/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/flux_local.py` & `flux-local-3.1.1/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/format.py` & `flux-local-3.1.1/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/get.py` & `flux-local-3.1.1/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/selector.py` & `flux-local-3.1.1/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/test.py` & `flux-local-3.1.1/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local/tool/visitor.py` & `flux-local-3.1.1/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/flux_local.egg-info/PKG-INFO` & `flux-local-3.1.1/flux_local.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 3.1.0
+Version: 3.1.1
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.10
```

### Comparing `flux-local-3.1.0/flux_local.egg-info/SOURCES.txt` & `flux-local-3.1.1/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/setup.cfg` & `flux-local-3.1.1/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 3.1.0
+version = 3.1.1
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-3.1.0/tests/test_command.py` & `flux-local-3.1.1/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/tests/test_git_repo.py` & `flux-local-3.1.1/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/tests/test_helm.py` & `flux-local-3.1.1/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/tests/test_kustomize.py` & `flux-local-3.1.1/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-3.1.0/tests/test_manifest.py` & `flux-local-3.1.1/tests/test_manifest.py`

 * *Files identical despite different names*

