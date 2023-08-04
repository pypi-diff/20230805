# Comparing `tmp/cmeel_example-0.5.1.tar.gz` & `tmp/cmeel_example-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmeel_example-0.5.1.tar", last modified: Fri Aug  4 16:32:46 2023, max compression
+gzip compressed data, was "cmeel_example-0.5.2.tar", last modified: Fri Aug  4 16:35:31 2023, max compression
```

## Comparing `cmeel_example-0.5.1.tar` & `cmeel_example-0.5.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.cirrus.yml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.git-blame-ignore-revs
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/docs/release.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-08-04 16:32:42.145391 cmeel_example-0.5.1/docs/release.sh
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/include/cmeel/example/adder.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/package.xml
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/python/cmeel_example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/python/cmeel_example/mult.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/python/module.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/src/adder.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/src/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/tests/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/tests/add.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/tests/python/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/tests/python/test_add.py
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-04 16:32:42.149391 cmeel_example-0.5.1/tests/python/test_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-04 16:32:46.789613 cmeel_example-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.cirrus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.git-blame-ignore-revs
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4303 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/docs/release.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      593 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/docs/release.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/include/cmeel/example/adder.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/package.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/python/cmeel_example/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/python/cmeel_example/mult.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/python/module.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/src/adder.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/src/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/tests/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/tests/add.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/tests/python/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/tests/python/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-04 16:35:25.398231 cmeel_example-0.5.2/tests/python/test_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-08-04 16:35:31.242354 cmeel_example-0.5.2/PKG-INFO
```

### Comparing `cmeel_example-0.5.1/.cirrus.yml` & `cmeel_example-0.5.2/.cirrus.yml`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/.github/workflows/release.yml` & `cmeel_example-0.5.2/.github/workflows/release.yml`

 * *Files 2% similar despite different names*

```diff
@@ -37,16 +37,16 @@
         with:
           platforms: all
       - run: pipx install cibuildwheel
       - run: cibuildwheel --output-dir wh
         env:
           CIBW_BUILD: ${{ matrix.build }}
           CIBW_ARCHS: ${{ matrix.arch }}
-          CIBW_MANYLINUX_X86_64_IMAGE: "quay.io/pypa/manylinux2014_x86_64"
-          CIBW_MANYLINUX_PYPY_X86_64_IMAGE: "quay.io/pypa/manylinux2014_x86_64"
+          CIBW_MANYLINUX_X86_64_IMAGE: "quay.io/pypa/manylinux_2_28_x86_64"
+          CIBW_MANYLINUX_PYPY_X86_64_IMAGE: "quay.io/pypa/manylinux_2_28_x86_64"
           CIBW_MANYLINUX_AARCH64_IMAGE: "quay.io/pypa/manylinux_2_28_aarch64"
           CIBW_REPAIR_WHEEL_COMMAND: ""
           CIBW_ENVIRONMENT: CMEEL_LOG_LEVEL="DEBUG"
       - uses: actions/upload-artifact@v3
         with:
           path: wh
```

### Comparing `cmeel_example-0.5.1/.github/workflows/test.yml` & `cmeel_example-0.5.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/.gitlab-ci.yml` & `cmeel_example-0.5.2/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/.pre-commit-config.yaml` & `cmeel_example-0.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/CHANGELOG.md` & `cmeel_example-0.5.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/CMakeLists.txt` & `cmeel_example-0.5.2/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/LICENSE` & `cmeel_example-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/README.md` & `cmeel_example-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/docs/release.sh` & `cmeel_example-0.5.2/docs/release.sh`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/package.xml` & `cmeel_example-0.5.2/package.xml`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/pyproject.toml` & `cmeel_example-0.5.2/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -13,15 +13,15 @@
   "Topic :: System :: Archiving :: Packaging",
   "Topic :: System :: Software Distribution"
 ]
 description = "This is an example project, to show how to use cmeel"
 license = "BSD-2-Clause"
 name = "cmeel-example"
 requires-python = ">= 3.8"
-version = "0.5.1"
+version = "0.5.2"
 
 [project.urls]
 changelog = "https://github.com/cmake-wheel/cmeel-example/blob/main/CHANGELOG.md"
 homepage = "https://github.com/cmake-wheel/cmeel-example"
 repository = "https://github.com/cmake-wheel/cmeel-example.git"
 
 [tool.isort]
```

### Comparing `cmeel_example-0.5.1/python/CMakeLists.txt` & `cmeel_example-0.5.2/python/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `cmeel_example-0.5.1/PKG-INFO` & `cmeel_example-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cmeel-example
-Version: 0.5.1
+Version: 0.5.2
 Summary: This is an example project, to show how to use cmeel
 Requires-Python: >= 3.8
 License-Expression: BSD-2-Clause
 Author-email: Guilhem Saurel <guilhem.saurel@laas.fr>
 Project-URL: Changelog, https://github.com/cmake-wheel/cmeel-example/blob/main/CHANGELOG.md
 Home-page: https://github.com/cmake-wheel/cmeel-example
 Project-URL: Repository, https://github.com/cmake-wheel/cmeel-example.git
```

