# Comparing `tmp/mojo_testplus-0.0.5.tar.gz` & `tmp/mojo_testplus-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_testplus-0.0.5.tar", max compression
+gzip compressed data, was "mojo_testplus-0.0.8.tar", max compression
```

## Comparing `mojo_testplus-0.0.5.tar` & `mojo_testplus-0.0.8.tar`

### file list

```diff
@@ -1,54 +1,54 @@
--rw-r--r--   0        0        0     1083 2023-03-23 04:58:22.729118 mojo_testplus-0.0.5/LICENSE.txt
--rw-r--r--   0        0        0      195 2023-03-23 07:27:52.484881 mojo_testplus-0.0.5/README.md
--rw-r--r--   0        0        0      704 2023-04-28 01:18:41.245061 mojo_testplus-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      552 2023-04-21 02:42:40.372545 mojo_testplus-0.0.5/source/packages/mojo/factories/testplusfactory.py
--rw-r--r--   0        0        0     1415 2023-03-22 03:44:52.832695 mojo_testplus-0.0.5/source/packages/mojo/testplus/__init__.py
--rw-r--r--   0        0        0        0 2023-03-23 04:51:36.888730 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-22 03:58:12.734868 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/__init__.py
--rw-r--r--   0        0        0      859 2023-03-23 07:58:00.173924 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
--rw-r--r--   0        0        0     3165 2023-03-23 04:58:22.729118 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
--rw-r--r--   0        0        0     6102 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
--rw-r--r--   0        0        0     4130 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
--rw-r--r--   0        0        0    13194 2023-04-21 02:42:40.372545 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
--rw-r--r--   0        0        0     1421 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/testplus_command.py
--rw-r--r--   0        0        0     1941 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/constraints.py
--rw-r--r--   0        0        0      556 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/diagnostics.py
--rw-r--r--   0        0        0     5089 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/entrypoints.py
--rw-r--r--   0        0        0      714 2023-03-21 17:13:07.396394 mojo_testplus-0.0.5/source/packages/mojo/testplus/exceptions.py
--rw-r--r--   0        0        0     4370 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/expressions.py
--rw-r--r--   0        0        0      352 2023-03-23 14:25:46.434788 mojo_testplus-0.0.5/source/packages/mojo/testplus/extensionpoints.py
--rw-r--r--   0        0        0     1532 2023-04-21 02:42:40.368545 mojo_testplus-0.0.5/source/packages/mojo/testplus/initialize.py
--rw-r--r--   0        0        0      526 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/jsos.py
--rw-r--r--   0        0        0     7403 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/markers.py
--rw-r--r--   0        0        0     3988 2023-03-23 07:58:00.173924 mojo_testplus-0.0.5/source/packages/mojo/testplus/parameters.py
--rw-r--r--   0        0        0     3228 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/queries.py
--rw-r--r--   0        0        0    13374 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/recorders.py
--rw-r--r--   0        0        0     1398 2023-03-20 23:24:48.701671 mojo_testplus-0.0.5/source/packages/mojo/testplus/reflection.py
--rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296697 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/__init__.py
--rw-r--r--   0        0        0      691 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/integrationsource.py
--rw-r--r--   0        0        0     2991 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/parameterorigin.py
--rw-r--r--   0        0        0    10904 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourceregistry.py
--rw-r--r--   0        0        0    16262 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcescope.py
--rw-r--r--   0        0        0      636 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcesource.py
--rw-r--r--   0        0        0      743 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/scopesource.py
--rw-r--r--   0        0        0     1575 2023-03-21 17:11:05.906189 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/sourcebase.py
--rw-r--r--   0        0        0      888 2023-03-23 07:58:00.177924 mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/unknownsource.py
--rw-r--r--   0        0        0      391 2023-03-20 23:24:48.709671 mojo_testplus-0.0.5/source/packages/mojo/testplus/resourcelifespan.py
--rw-r--r--   0        0        0     6916 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/resources.py
--rw-r--r--   0        0        0    10718 2023-03-20 23:24:48.705671 mojo_testplus-0.0.5/source/packages/mojo/testplus/results.py
--rwxr-xr-x   0        0        0      959 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/__init__.py
--rw-r--r--   0        0        0    10399 2023-04-19 05:52:19.472744 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.css
--rw-r--r--   0        0        0    38006 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.js
--rw-r--r--   0        0        0    23424 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/w3.css
--rw-r--r--   0        0        0     3190 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-images.html
--rw-r--r--   0        0        0     3385 2023-04-08 22:20:18.965889 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-sounds.html
--rwxr-xr-x   0        0        0     6714 2023-04-19 05:52:19.472744 mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/testsummary.html
--rwxr-xr-x   0        0        0     9165 2023-03-23 07:58:00.173924 mojo_testplus-0.0.5/source/packages/mojo/testplus/testcollector.py
--rw-r--r--   0        0        0     5047 2023-03-23 07:58:03.641945 mojo_testplus-0.0.5/source/packages/mojo/testplus/testgroup.py
--rwxr-xr-x   0        0        0    17780 2023-04-08 22:20:18.969889 mojo_testplus-0.0.5/source/packages/mojo/testplus/testjob.py
--rwxr-xr-x   0        0        0     4516 2023-03-23 07:58:00.169924 mojo_testplus-0.0.5/source/packages/mojo/testplus/testref.py
--rw-r--r--   0        0        0    37901 2023-04-08 22:20:18.969889 mojo_testplus-0.0.5/source/packages/mojo/testplus/testsequencer.py
--rwxr-xr-x   0        0        0     6040 2023-03-20 23:24:48.685671 mojo_testplus-0.0.5/source/packages/mojo/testplus/utilities.py
--rw-r--r--   0        0        0    17353 2023-04-08 22:20:18.969889 mojo_testplus-0.0.5/source/packages/mojo/testplus/verification.py
--rw-r--r--   0        0        0     1173 1970-01-01 00:00:00.000000 mojo_testplus-0.0.5/setup.py
--rw-r--r--   0        0        0      969 1970-01-01 00:00:00.000000 mojo_testplus-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-03-23 04:58:22.729118 mojo_testplus-0.0.8/LICENSE.txt
+-rw-r--r--   0        0        0      248 2023-04-29 15:30:00.317909 mojo_testplus-0.0.8/README.rst
+-rw-r--r--   0        0        0      705 2023-05-06 21:06:30.416221 mojo_testplus-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      552 2023-04-21 02:42:40.372545 mojo_testplus-0.0.8/source/packages/mojo/factories/testplusfactory.py
+-rw-r--r--   0        0        0     1415 2023-03-22 03:44:52.832695 mojo_testplus-0.0.8/source/packages/mojo/testplus/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-23 04:51:36.888730 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-22 03:58:12.734868 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/__init__.py
+-rw-r--r--   0        0        0      859 2023-03-23 07:58:00.173924 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py
+-rw-r--r--   0        0        0     3165 2023-03-23 04:58:22.729118 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py
+-rw-r--r--   0        0        0     6102 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py
+-rw-r--r--   0        0        0     4130 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/query.py
+-rw-r--r--   0        0        0    13194 2023-04-21 02:42:40.372545 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/run.py
+-rw-r--r--   0        0        0     1421 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/testplus_command.py
+-rw-r--r--   0        0        0     1941 2023-03-20 23:24:48.709671 mojo_testplus-0.0.8/source/packages/mojo/testplus/constraints.py
+-rw-r--r--   0        0        0      556 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/diagnostics.py
+-rw-r--r--   0        0        0     5089 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/entrypoints.py
+-rw-r--r--   0        0        0      714 2023-03-21 17:13:07.396394 mojo_testplus-0.0.8/source/packages/mojo/testplus/exceptions.py
+-rw-r--r--   0        0        0     4370 2023-03-20 23:24:48.709671 mojo_testplus-0.0.8/source/packages/mojo/testplus/expressions.py
+-rw-r--r--   0        0        0      352 2023-03-23 14:25:46.434788 mojo_testplus-0.0.8/source/packages/mojo/testplus/extensionpoints.py
+-rw-r--r--   0        0        0     1717 2023-04-28 04:46:03.062541 mojo_testplus-0.0.8/source/packages/mojo/testplus/initialize.py
+-rw-r--r--   0        0        0      526 2023-03-20 23:24:48.709671 mojo_testplus-0.0.8/source/packages/mojo/testplus/jsos.py
+-rw-r--r--   0        0        0     7403 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/markers.py
+-rw-r--r--   0        0        0     3988 2023-03-23 07:58:00.173924 mojo_testplus-0.0.8/source/packages/mojo/testplus/parameters.py
+-rw-r--r--   0        0        0     3228 2023-03-23 07:58:00.169924 mojo_testplus-0.0.8/source/packages/mojo/testplus/queries.py
+-rw-r--r--   0        0        0    13374 2023-03-23 07:58:00.169924 mojo_testplus-0.0.8/source/packages/mojo/testplus/recorders.py
+-rw-r--r--   0        0        0     1398 2023-03-20 23:24:48.701671 mojo_testplus-0.0.8/source/packages/mojo/testplus/reflection.py
+-rw-r--r--   0        0        0        0 2022-12-08 19:53:16.296697 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/__init__.py
+-rw-r--r--   0        0        0      691 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/integrationsource.py
+-rw-r--r--   0        0        0     2991 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/parameterorigin.py
+-rw-r--r--   0        0        0    10904 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/resourceregistry.py
+-rw-r--r--   0        0        0    16262 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/resourcescope.py
+-rw-r--r--   0        0        0      636 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/resourcesource.py
+-rw-r--r--   0        0        0      743 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/scopesource.py
+-rw-r--r--   0        0        0     1575 2023-03-21 17:11:05.906189 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/sourcebase.py
+-rw-r--r--   0        0        0      888 2023-03-23 07:58:00.177924 mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/unknownsource.py
+-rw-r--r--   0        0        0      391 2023-03-20 23:24:48.709671 mojo_testplus-0.0.8/source/packages/mojo/testplus/resourcelifespan.py
+-rw-r--r--   0        0        0     6916 2023-03-23 07:58:00.169924 mojo_testplus-0.0.8/source/packages/mojo/testplus/resources.py
+-rw-r--r--   0        0        0    10718 2023-03-20 23:24:48.705671 mojo_testplus-0.0.8/source/packages/mojo/testplus/results.py
+-rwxr-xr-x   0        0        0      959 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/__init__.py
+-rw-r--r--   0        0        0    10399 2023-04-19 05:52:19.472744 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/static/v0/testsummary.css
+-rw-r--r--   0        0        0    38006 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/static/v0/testsummary.js
+-rw-r--r--   0        0        0    23424 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/static/v0/w3.css
+-rw-r--r--   0        0        0     3190 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/tabs/tab-images.html
+-rw-r--r--   0        0        0     3385 2023-04-08 22:20:18.965889 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/tabs/tab-sounds.html
+-rwxr-xr-x   0        0        0     6714 2023-04-19 05:52:19.472744 mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/testsummary.html
+-rwxr-xr-x   0        0        0     9165 2023-03-23 07:58:00.173924 mojo_testplus-0.0.8/source/packages/mojo/testplus/testcollector.py
+-rw-r--r--   0        0        0     5047 2023-03-23 07:58:03.641945 mojo_testplus-0.0.8/source/packages/mojo/testplus/testgroup.py
+-rwxr-xr-x   0        0        0    17780 2023-04-08 22:20:18.969889 mojo_testplus-0.0.8/source/packages/mojo/testplus/testjob.py
+-rwxr-xr-x   0        0        0     4516 2023-03-23 07:58:00.169924 mojo_testplus-0.0.8/source/packages/mojo/testplus/testref.py
+-rw-r--r--   0        0        0    37901 2023-04-08 22:20:18.969889 mojo_testplus-0.0.8/source/packages/mojo/testplus/testsequencer.py
+-rwxr-xr-x   0        0        0     6040 2023-03-20 23:24:48.685671 mojo_testplus-0.0.8/source/packages/mojo/testplus/utilities.py
+-rw-r--r--   0        0        0    17353 2023-04-08 22:20:18.969889 mojo_testplus-0.0.8/source/packages/mojo/testplus/verification.py
+-rw-r--r--   0        0        0     1229 1970-01-01 00:00:00.000000 mojo_testplus-0.0.8/setup.py
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 mojo_testplus-0.0.8/PKG-INFO
```

### Comparing `mojo_testplus-0.0.5/LICENSE.txt` & `mojo_testplus-0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/pyproject.toml` & `mojo_testplus-0.0.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mojo-testplus"
 description = "Automation Mojo TestPlus Test Framework"
-version = "0.0.5"
+version = "0.0.8"
 authors = []
-readme = "README.md"
+readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
 ]
 keywords = [
```

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/factories/testplusfactory.py` & `mojo_testplus-0.0.8/source/packages/mojo/factories/testplusfactory.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/__init__.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/jobs.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/query.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/query.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/cmdtree/testing/run.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/cmdtree/testing/run.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/cli/testplus_command.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/cli/testplus_command.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/constraints.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/constraints.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/diagnostics.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/diagnostics.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/entrypoints.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/entrypoints.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/exceptions.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/exceptions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/expressions.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/expressions.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/initialize.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/initialize.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,30 +4,33 @@
 
 from mojo.xmods.xcollections.context import Context, ContextPaths
 
 from mojo.runtime.initialize import initialize_runtime, MOJO_RUNTIME_STATE
 from mojo.runtime.variables import MOJO_RUNTIME_VARIABLES
 
 TESTPLUS_DIR = os.path.dirname(__file__)
-TEMPLATES_DIR = os.path.join(TESTPLUS_DIR, "templates")
-STATIC_DIR = os.path.join(TEMPLATES_DIR, "static")
+
+class TestPlusVariables:
+    TESTPLUS_TEMPLATES_DIR = os.path.join(TESTPLUS_DIR, "templates")
+    TESTPLUS_RESOURCE_SRC_DIR = os.path.join(TESTPLUS_TEMPLATES_DIR, "static")
+    TESTPLUS_SUMMARY_TEMPLATE = os.path.join(TESTPLUS_TEMPLATES_DIR, "testsummary.html")
 
 def initialize_testplus_runtime():
     if not MOJO_RUNTIME_STATE.INITIALIZED:
         initialize_runtime(name="testplus", logger_name="TP")
     return
 
 def initialize_testplus_results():
     dest_static_dir = os.path.join(MOJO_RUNTIME_VARIABLES.MJR_HOME_DIRECTORY, "results", "static")
 
     if MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR is None:
-        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR = STATIC_DIR
+        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR = TestPlusVariables.TESTPLUS_RESOURCE_SRC_DIR
     if MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR is None:
         MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR = dest_static_dir
     if MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE is None:
-        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE = os.path.join(TEMPLATES_DIR, "testsummary.html")
+        MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE = TestPlusVariables.TESTPLUS_SUMMARY_TEMPLATE
 
     ctx = Context()
     ctx.insert(ContextPaths.DIR_RESULTS_RESOURCE_SRC, MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_SRC_DIR)
     ctx.insert(ContextPaths.DIR_RESULTS_RESOURCE_DEST, MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_RESOURCE_DEST_DIR)
     ctx.insert(ContextPaths.FILE_RESULTS_TEMPLATE, MOJO_RUNTIME_VARIABLES.MJR_RESULTS_STATIC_SUMMARY_TEMPLATE)
     return
```

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/jsos.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/jsos.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/markers.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/markers.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/parameters.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/parameters.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/queries.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/queries.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/recorders.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/recorders.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/reflection.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/reflection.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/integrationsource.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/integrationsource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/parameterorigin.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/parameterorigin.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourceregistry.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/resourceregistry.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcescope.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/resourcescope.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/resourcesource.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/resourcesource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/scopesource.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/scopesource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/sourcebase.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/sourcebase.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/registration/unknownsource.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/registration/unknownsource.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/resources.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/resources.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/results.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/results.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/__init__.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.css` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/static/v0/testsummary.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/testsummary.js` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/static/v0/testsummary.js`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/static/v0/w3.css` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/static/v0/w3.css`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-images.html` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/tabs/tab-images.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/tabs/tab-sounds.html` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/tabs/tab-sounds.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/templates/testsummary.html` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/templates/testsummary.html`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/testcollector.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/testcollector.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/testgroup.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/testgroup.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/testjob.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/testjob.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/testref.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/testref.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/testsequencer.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/testsequencer.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/utilities.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/utilities.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/source/packages/mojo/testplus/verification.py` & `mojo_testplus-0.0.8/source/packages/mojo/testplus/verification.py`

 * *Files identical despite different names*

### Comparing `mojo_testplus-0.0.5/setup.py` & `mojo_testplus-0.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 {'': ['*'], 'mojo.testplus.templates': ['static/v0/*', 'tabs/*']}
 
 install_requires = \
 ['click>=8.1.3,<9.0.0', 'debugpy>=1.6.5,<2.0.0', 'mojo-runtime>=0.0.20,<0.1.0']
 
 setup_kwargs = {
     'name': 'mojo-testplus',
-    'version': '0.0.5',
+    'version': '0.0.8',
     'description': 'Automation Mojo TestPlus Test Framework',
-    'long_description': "# Automation Mojo - Testplus \nThis is preliminary release of the 'testplus' automation framework in a separate package from\nthe AutomationKit.  This release is not ready for public consumption.\n\n",
+    'long_description': "==========================\nAutomation Mojo - Testplus\n==========================\n \nThis is preliminary release of the 'testplus' automation framework in a separate package from\nthe AutomationKit.  This release is not ready for public consumption.\n\n",
     'author': 'None',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `mojo_testplus-0.0.5/PKG-INFO` & `mojo_testplus-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-testplus
-Version: 0.0.5
+Version: 0.0.8
 Summary: Automation Mojo TestPlus Test Framework
 License: LICENSE.txt
 Keywords: python
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: POSIX
@@ -13,14 +13,17 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: debugpy (>=1.6.5,<2.0.0)
 Requires-Dist: mojo-runtime (>=0.0.20,<0.1.0)
-Description-Content-Type: text/markdown
+Description-Content-Type: text/x-rst
 
-# Automation Mojo - Testplus 
+==========================
+Automation Mojo - Testplus
+==========================
+ 
 This is preliminary release of the 'testplus' automation framework in a separate package from
 the AutomationKit.  This release is not ready for public consumption.
```

