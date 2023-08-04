# Comparing `tmp/poetry-kernel-0.1.2.tar.gz` & `tmp/poetry-kernel-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry-kernel-0.1.2.tar", last modified: Wed Mar 30 18:34:11 2022, max compression
+gzip compressed data, was "poetry-kernel-0.1.3.tar", last modified: Fri Aug  4 22:49:47 2023, max compression
```

## Comparing `poetry-kernel-0.1.2.tar` & `poetry-kernel-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 18:34:11.275062 poetry-kernel-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)     1052 2022-03-30 18:34:02.000000 poetry-kernel-0.1.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-03-30 18:34:11.275062 poetry-kernel-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3865 2022-03-30 18:34:02.000000 poetry-kernel-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 18:34:11.271062 poetry-kernel-0.1.2/poetry_kernel/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-30 18:34:02.000000 poetry-kernel-0.1.2/poetry_kernel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1948 2022-03-30 18:34:02.000000 poetry-kernel-0.1.2/poetry_kernel/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      789 2022-03-30 18:34:02.000000 poetry-kernel-0.1.2/poetry_kernel/kernelspec.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-30 18:34:11.275062 poetry-kernel-0.1.2/poetry_kernel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4634 2022-03-30 18:34:11.000000 poetry-kernel-0.1.2/poetry_kernel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      293 2022-03-30 18:34:11.000000 poetry-kernel-0.1.2/poetry_kernel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-30 18:34:11.000000 poetry-kernel-0.1.2/poetry_kernel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-30 18:34:11.000000 poetry-kernel-0.1.2/poetry_kernel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-03-30 18:34:11.000000 poetry-kernel-0.1.2/poetry_kernel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-30 18:34:11.275062 poetry-kernel-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2326 2022-03-30 18:34:02.000000 poetry-kernel-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:49:47.010252 poetry-kernel-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-08-04 22:49:44.000000 poetry-kernel-0.1.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-04 22:49:47.010252 poetry-kernel-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-08-04 22:49:44.000000 poetry-kernel-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:49:47.010252 poetry-kernel-0.1.3/poetry_kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 22:49:44.000000 poetry-kernel-0.1.3/poetry_kernel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-08-04 22:49:44.000000 poetry-kernel-0.1.3/poetry_kernel/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-08-04 22:49:44.000000 poetry-kernel-0.1.3/poetry_kernel/kernelspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 22:49:47.010252 poetry-kernel-0.1.3/poetry_kernel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-04 22:49:47.000000 poetry-kernel-0.1.3/poetry_kernel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-08-04 22:49:47.000000 poetry-kernel-0.1.3/poetry_kernel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 22:49:47.000000 poetry-kernel-0.1.3/poetry_kernel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:49:47.000000 poetry-kernel-0.1.3/poetry_kernel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-08-04 22:49:47.000000 poetry-kernel-0.1.3/poetry_kernel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 22:49:47.014252 poetry-kernel-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-04 22:49:44.000000 poetry-kernel-0.1.3/setup.py
```

### Comparing `poetry-kernel-0.1.2/LICENSE.md` & `poetry-kernel-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `poetry-kernel-0.1.2/PKG-INFO` & `poetry-kernel-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-kernel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Jupyter kernel using Poetry for dependency management
 Home-page: https://github.com/pathbird/poetry-kernel
 Author: Pathbird Inc
 Author-email: oss@pathbird.com
 License: MIT
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: UNKNOWN
```

### Comparing `poetry-kernel-0.1.2/README.md` & `poetry-kernel-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `poetry-kernel-0.1.2/poetry_kernel/__main__.py` & `poetry-kernel-0.1.3/poetry_kernel/__main__.py`

 * *Files identical despite different names*

### Comparing `poetry-kernel-0.1.2/poetry_kernel/kernelspec.py` & `poetry-kernel-0.1.3/poetry_kernel/kernelspec.py`

 * *Files identical despite different names*

### Comparing `poetry-kernel-0.1.2/poetry_kernel.egg-info/PKG-INFO` & `poetry-kernel-0.1.3/poetry_kernel.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-kernel
-Version: 0.1.2
+Version: 0.1.3
 Summary: Python Jupyter kernel using Poetry for dependency management
 Home-page: https://github.com/pathbird/poetry-kernel
 Author: Pathbird Inc
 Author-email: oss@pathbird.com
 License: MIT
 Keywords: Interactive,Interpreter,Shell,Web
 Platform: UNKNOWN
```

### Comparing `poetry-kernel-0.1.2/setup.py` & `poetry-kernel-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     ]
 
 with open(os.path.join(current_dir, "README.md")) as fp:
     README = fp.read()
 
 setup(
     name="poetry-kernel",
-    version="0.1.2",
+    version="0.1.3",
 
     # Package metadata
     author="Pathbird Inc",
     author_email="oss@pathbird.com",
     url="https://github.com/pathbird/poetry-kernel",
     license="MIT",
     description="Python Jupyter kernel using Poetry for dependency management",
@@ -61,12 +61,12 @@
         "Programming Language :: Python :: 3",
     ],
 
     # Actual code stuff
     packages=["poetry_kernel"],
     python_requires=">=3.7",
     install_requires=[
-        "jupyter-client ~= 7.0.1",
+        "jupyter-client >= 7.0.1",
         "colorama ~= 0.4.4",
     ],
     **setup_args,
 )
```

