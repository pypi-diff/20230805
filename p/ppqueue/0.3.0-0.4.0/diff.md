# Comparing `tmp/ppqueue-0.3.0.tar.gz` & `tmp/ppqueue-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ppqueue-0.3.0.tar", last modified: Thu Jun 22 04:51:20 2023, max compression
+gzip compressed data, was "ppqueue-0.4.0.tar", last modified: Fri Aug  4 22:13:43 2023, max compression
```

## Comparing `ppqueue-0.3.0.tar` & `ppqueue-0.4.0.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 04:51:20.331953 ppqueue-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1058 2023-06-22 04:39:29.000000 ppqueue-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     5003 2023-06-22 04:51:20.331953 ppqueue-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3299 2023-06-22 04:39:29.000000 ppqueue-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)     4843 2023-06-22 04:39:29.000000 ppqueue-0.3.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 04:51:20.331953 ppqueue-0.3.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 04:51:20.319953 ppqueue-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 04:51:20.323953 ppqueue-0.3.0/src/ppqueue/
--rw-r--r--   0 root         (0) root         (0)       74 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 04:51:20.327953 ppqueue-0.3.0/src/ppqueue/__pycache__/
--rw-r--r--   0 root         (0) root         (0)      222 2023-06-22 04:40:46.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      151 2023-06-22 04:50:59.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/__version__.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)      301 2023-06-22 04:41:06.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/exceptions.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     7343 2023-06-22 04:40:46.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/job.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     6424 2023-06-22 04:40:46.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/plot.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)    26434 2023-06-22 04:40:46.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/queue.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)     2723 2023-06-22 04:40:46.000000 ppqueue-0.3.0/src/ppqueue/__pycache__/utils.cpython-310.pyc
--rw-r--r--   0 root         (0) root         (0)       22 2023-06-22 04:50:59.000000 ppqueue-0.3.0/src/ppqueue/__version__.py
--rw-r--r--   0 root         (0) root         (0)       42 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     8072 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/job.py
--rw-r--r--   0 root         (0) root         (0)     7524 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/plot.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/py.typed
--rw-r--r--   0 root         (0) root         (0)    32299 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/queue.py
--rw-r--r--   0 root         (0) root         (0)     2436 2023-06-22 04:39:29.000000 ppqueue-0.3.0/src/ppqueue/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 04:51:20.323953 ppqueue-0.3.0/src/ppqueue.egg-info/
--rw-r--r--   0 root         (0) root         (0)     5003 2023-06-22 04:51:20.000000 ppqueue-0.3.0/src/ppqueue.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      853 2023-06-22 04:51:20.000000 ppqueue-0.3.0/src/ppqueue.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 04:51:20.000000 ppqueue-0.3.0/src/ppqueue.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-22 04:51:20.000000 ppqueue-0.3.0/src/ppqueue.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      659 2023-06-22 04:51:20.000000 ppqueue-0.3.0/src/ppqueue.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        8 2023-06-22 04:51:20.000000 ppqueue-0.3.0/src/ppqueue.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 04:51:20.331953 ppqueue-0.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)      720 2023-06-22 04:39:29.000000 ppqueue-0.3.0/tests/test_plot.py
--rw-r--r--   0 root         (0) root         (0)      750 2023-06-22 04:39:29.000000 ppqueue-0.3.0/tests/test_queue_processes.py
--rw-r--r--   0 root         (0) root         (0)      616 2023-06-22 04:39:29.000000 ppqueue-0.3.0/tests/test_queue_threads.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-06-22 04:39:29.000000 ppqueue-0.3.0/tests/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:13:43.503801 ppqueue-0.4.0/
+-rw-r--r--   0 root         (0) root         (0)     1058 2023-08-04 22:03:15.000000 ppqueue-0.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-08-04 22:13:43.503801 ppqueue-0.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3309 2023-08-04 22:03:15.000000 ppqueue-0.4.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-04 22:03:15.000000 ppqueue-0.4.0/README.pypi.md
+-rw-r--r--   0 root         (0) root         (0)     4825 2023-08-04 22:03:15.000000 ppqueue-0.4.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 22:13:43.503801 ppqueue-0.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:13:43.459801 ppqueue-0.4.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:13:43.499801 ppqueue-0.4.0/src/ppqueue/
+-rw-r--r--   0 root         (0) root         (0)       74 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:13:43.503801 ppqueue-0.4.0/src/ppqueue/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      222 2023-08-04 22:04:24.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      151 2023-08-04 22:13:23.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      301 2023-08-04 22:04:44.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     7620 2023-08-04 22:04:24.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/job.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6531 2023-08-04 22:04:24.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/plot.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    27596 2023-08-04 22:04:24.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/queue.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2396 2023-08-04 22:04:24.000000 ppqueue-0.4.0/src/ppqueue/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-08-04 22:13:23.000000 ppqueue-0.4.0/src/ppqueue/__version__.py
+-rw-r--r--   0 root         (0) root         (0)       42 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     8349 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/job.py
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/plot.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/py.typed
+-rw-r--r--   0 root         (0) root         (0)    33882 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/queue.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2023-08-04 22:03:15.000000 ppqueue-0.4.0/src/ppqueue/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:13:43.499801 ppqueue-0.4.0/src/ppqueue.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1745 2023-08-04 22:13:43.000000 ppqueue-0.4.0/src/ppqueue.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      868 2023-08-04 22:13:43.000000 ppqueue-0.4.0/src/ppqueue.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 22:13:43.000000 ppqueue-0.4.0/src/ppqueue.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-04 22:13:43.000000 ppqueue-0.4.0/src/ppqueue.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      659 2023-08-04 22:13:43.000000 ppqueue-0.4.0/src/ppqueue.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-08-04 22:13:43.000000 ppqueue-0.4.0/src/ppqueue.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:13:43.503801 ppqueue-0.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      720 2023-08-04 22:03:15.000000 ppqueue-0.4.0/tests/test_plot.py
+-rw-r--r--   0 root         (0) root         (0)      750 2023-08-04 22:03:15.000000 ppqueue-0.4.0/tests/test_queue_processes.py
+-rw-r--r--   0 root         (0) root         (0)      616 2023-08-04 22:03:15.000000 ppqueue-0.4.0/tests/test_queue_threads.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-08-04 22:03:15.000000 ppqueue-0.4.0/tests/test_utils.py
```

### Comparing `ppqueue-0.3.0/LICENSE` & `ppqueue-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ppqueue-0.3.0/README.md` & `ppqueue-0.4.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 # ppqueue
 
-> Parallel Process Queue (ppqueue) for Python
+> A Parallel Process Queue for Python.
 
-> Formerly known as `ezpq`
-
-| Links         |                        |
-|---------------|------------------------|
-| Code Repo     | https://www.github.com/fresh2dev/ppqueue           |
-| Mirror Repo   | https://www.Fresh2.dev/code/r/ppqueue        |
-| Documentation | https://www.Fresh2.dev/code/r/ppqueue/i           |
-| Changelog     | https://www.Fresh2.dev/code/r/ppqueue/i/changelog |
-| License       | https://www.Fresh2.dev/code/r/ppqueue/i/license   |
-| Funding       | https://www.Fresh2.dev/funding        |
-
-[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/ppqueue/releases)
-[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/ppqueue/releases)
-[![License](https://img.shields.io/github/license/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.Fresh2.dev/code/r/ppqueue/i/license)
+| Links         |                                          |
+|---------------|------------------------------------------|
+| Code Repo     | https://www.github.com/fresh2dev/ppqueue |
+| Mirror Repo   | https://www.f2dv.com/r/ppqueue           |
+| Documentation | https://www.f2dv.com/r/ppqueue           |
+| Changelog     | https://www.f2dv.com/r/ppqueue/changelog |
+| License       | https://www.f2dv.com/r/ppqueue/license   |
+| Funding       | https://www.f2dv.com/fund                |
+
+[![GitHub release (latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.f2dv.com/r/ppqueue/changelog)
+[![GitHub Release Date](https://img.shields.io/github/release-date/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.f2dv.com/r/ppqueue/changelog)
+[![License](https://img.shields.io/github/license/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.f2dv.com/r/ppqueue/license)
+[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/ppqueue&Date)
 [![GitHub issues](https://img.shields.io/github/issues-raw/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/ppqueue/issues)
 [![GitHub pull requests](https://img.shields.io/github/issues-pr-raw/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/ppqueue/pulls)
-[![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/ppqueue&Date)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/ppqueue?color=blue&style=for-the-badge)](https://pypi.org/project/ppqueue)
-[![Docs Website](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.Fresh2.dev/code/r/ppqueue/i)](https://www.Fresh2.dev/code/r/ppqueue/i)
-[![Coverage Website](https://img.shields.io/website?down_message=unavailable&label=coverage&style=for-the-badge&up_color=blue&up_message=available&url=https://www.Fresh2.dev/code/r/ppqueue/i/tests/coverage)](https://www.Fresh2.dev/code/r/ppqueue/i/tests/coverage)
-[![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.Fresh2.dev/funding)
+[![Docker Pulls](https://img.shields.io/docker/pulls/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://hub.docker.com/r/fresh2dev/ppqueue)
+[![Changelog](https://img.shields.io/website?down_message=unavailable&label=docs&style=for-the-badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/ppqueue/changelog)](https://www.f2dv.com/r/ppqueue/changelog)
+[![Funding](https://img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://www.f2dv.com/fund)
 
+---
 
 ## Overview
 
 `ppqueue` is a Python module that serves as an abstraction layer to both `multiprocessing.Process` and `threading.Thread`. I built `ppqueue` because I too often notice that parallelizing code results in *ugly* code. With this simple Queue, you can parallelize code easily and attractively. ppqueue offers:
 
 - a single API for parallel execution using processes or threads.
 - FIFO priority queueing.
@@ -50,12 +49,16 @@
 
 https://www.f2dv.com/code/r/ppqueue/i/page/examples/
 
 And more examples are provided in the reference docs:
 
 https://www.f2dv.com/code/r/ppqueue/i/reference/
 
+## Support
+
+If this project delivers value to you, please [provide feedback](https://www.github.com/fresh2dev/ppqueue/issues), code contributions, and/or [funding](https://www.f2dv.com/fund).
+
 ---
 
 *Brought to you by...*
 
-<a href="https://www.fresh2.dev"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
+<a href="https://www.f2dv.com"><img src="https://img.fresh2.dev/fresh2dev.svg" style="filter: invert(50%);"></img></a>
```

#### html2text {}

```diff
@@ -1,43 +1,42 @@
-# ppqueue > Parallel Process Queue (ppqueue) for Python > Formerly known as
-`ezpq` | Links | | |---------------|------------------------| | Code Repo |
-https://www.github.com/fresh2dev/ppqueue | | Mirror Repo | https://
-www.Fresh2.dev/code/r/ppqueue | | Documentation | https://www.Fresh2.dev/code/
-r/ppqueue/i | | Changelog | https://www.Fresh2.dev/code/r/ppqueue/i/changelog |
-| License | https://www.Fresh2.dev/code/r/ppqueue/i/license | | Funding |
-https://www.Fresh2.dev/funding | [![GitHub release (latest SemVer)](https://
-img.shields.io/github/v/release/fresh2dev/ppqueue?color=blue&style=for-the-
-badge)](https://www.github.com/fresh2dev/ppqueue/releases) [![GitHub Release
-Date](https://img.shields.io/github/release-date/fresh2dev/
-ppqueue?color=blue&style=for-the-badge)](https://www.github.com/fresh2dev/
-ppqueue/releases) [![License](https://img.shields.io/github/license/fresh2dev/
-ppqueue?color=blue&style=for-the-badge)](https://www.Fresh2.dev/code/r/ppqueue/
-i/license) [![GitHub issues](https://img.shields.io/github/issues-raw/
+# ppqueue > A Parallel Process Queue for Python. | Links | | |---------------|-
+-----------------------------------------| | Code Repo | https://
+www.github.com/fresh2dev/ppqueue | | Mirror Repo | https://www.f2dv.com/r/
+ppqueue | | Documentation | https://www.f2dv.com/r/ppqueue | | Changelog |
+https://www.f2dv.com/r/ppqueue/changelog | | License | https://www.f2dv.com/r/
+ppqueue/license | | Funding | https://www.f2dv.com/fund | [![GitHub release
+(latest SemVer)](https://img.shields.io/github/v/release/fresh2dev/
+ppqueue?color=blue&style=for-the-badge)](https://www.f2dv.com/r/ppqueue/
+changelog) [![GitHub Release Date](https://img.shields.io/github/release-date/
+fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.f2dv.com/r/
+ppqueue/changelog) [![License](https://img.shields.io/github/license/fresh2dev/
+ppqueue?color=blue&style=for-the-badge)](https://www.f2dv.com/r/ppqueue/
+license) [![GitHub Repo stars](https://img.shields.io/github/stars/fresh2dev/
+ppqueue?color=blue&style=for-the-badge)](https://star-history.com/#fresh2dev/
+ppqueue&Date) [![GitHub issues](https://img.shields.io/github/issues-raw/
 fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://www.github.com/
 fresh2dev/ppqueue/issues) [![GitHub pull requests](https://img.shields.io/
 github/issues-pr-raw/fresh2dev/ppqueue?color=blue&style=for-the-badge)](https:/
-/www.github.com/fresh2dev/ppqueue/pulls) [![GitHub Repo stars](https://
-img.shields.io/github/stars/fresh2dev/ppqueue?color=blue&style=for-the-badge)]
-(https://star-history.com/#fresh2dev/ppqueue&Date) [![PyPI - Downloads](https:/
-/img.shields.io/pypi/dm/ppqueue?color=blue&style=for-the-badge)](https://
-pypi.org/project/ppqueue) [![Docs Website](https://img.shields.io/
+/www.github.com/fresh2dev/ppqueue/pulls) [![PyPI - Downloads](https://
+img.shields.io/pypi/dm/ppqueue?color=blue&style=for-the-badge)](https://
+pypi.org/project/ppqueue) [![Docker Pulls](https://img.shields.io/docker/pulls/
+fresh2dev/ppqueue?color=blue&style=for-the-badge)](https://hub.docker.com/r/
+fresh2dev/ppqueue) [![Changelog](https://img.shields.io/
 website?down_message=unavailable&label=docs&style=for-the-
-badge&up_color=blue&up_message=available&url=https://www.Fresh2.dev/code/r/
-ppqueue/i)](https://www.Fresh2.dev/code/r/ppqueue/i) [![Coverage Website]
-(https://img.shields.io/
-website?down_message=unavailable&label=coverage&style=for-the-
-badge&up_color=blue&up_message=available&url=https://www.Fresh2.dev/code/r/
-ppqueue/i/tests/coverage)](https://www.Fresh2.dev/code/r/ppqueue/i/tests/
-coverage) [![Funding](https://img.shields.io/badge/funding-%24%24%24-
-blue?style=for-the-badge)](https://www.Fresh2.dev/funding) ## Overview
-`ppqueue` is a Python module that serves as an abstraction layer to both
-`multiprocessing.Process` and `threading.Thread`. I built `ppqueue` because I
-too often notice that parallelizing code results in *ugly* code. With this
-simple Queue, you can parallelize code easily and attractively. ppqueue offers:
-- a single API for parallel execution using processes or threads. - FIFO
-priority queueing. - Gantt charts of job execution (thanks `plotnine` +
-`pandas`) - progress bars (thanks to `tqdm`) ![](https://img.fresh2.dev/
-1687407526_84b23a13b5f.svg) ## Install Install from PyPi: ```python pip install
-ppqueue[plot] ``` ## Examples An notebook of examples is available at: https://
-www.f2dv.com/code/r/ppqueue/i/page/examples/ And more examples are provided in
-the reference docs: https://www.f2dv.com/code/r/ppqueue/i/reference/ --
-- *Brought to you by...* [https://img.fresh2.dev/fresh2dev.svg]
+badge&up_color=blue&up_message=available&url=https://www.f2dv.com/r/ppqueue/
+changelog)](https://www.f2dv.com/r/ppqueue/changelog) [![Funding](https://
+img.shields.io/badge/funding-%24%24%24-blue?style=for-the-badge)](https://
+www.f2dv.com/fund) --- ## Overview `ppqueue` is a Python module that serves as
+an abstraction layer to both `multiprocessing.Process` and `threading.Thread`.
+I built `ppqueue` because I too often notice that parallelizing code results in
+*ugly* code. With this simple Queue, you can parallelize code easily and
+attractively. ppqueue offers: - a single API for parallel execution using
+processes or threads. - FIFO priority queueing. - Gantt charts of job execution
+(thanks `plotnine` + `pandas`) - progress bars (thanks to `tqdm`) ![](https://
+img.fresh2.dev/1687407526_84b23a13b5f.svg) ## Install Install from PyPi:
+```python pip install ppqueue[plot] ``` ## Examples An notebook of examples is
+available at: https://www.f2dv.com/code/r/ppqueue/i/page/examples/ And more
+examples are provided in the reference docs: https://www.f2dv.com/code/r/
+ppqueue/i/reference/ ## Support If this project delivers value to you, please
+[provide feedback](https://www.github.com/fresh2dev/ppqueue/issues), code
+contributions, and/or [funding](https://www.f2dv.com/fund). --- *Brought to you
+by...* [https://img.fresh2.dev/fresh2dev.svg]
```

### Comparing `ppqueue-0.3.0/pyproject.toml` & `ppqueue-0.4.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools>=64", "build==0.*", "wheel==0.*", "twine==4.*"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ppqueue"
 authors = [
-    {name = "Donald Mellenbruch", email = "hello@Fresh2.dev"},
+    {name = "Donald Mellenbruch", email = "hello@f2dv.com"},
 ]
-description = "Parallel Process Queue (ppqueue) for Python"
-readme = "README.md"
+description = "A Parallel Process Queue for Python."
+readme = "README.pypi.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["version"]
 dependencies = [
@@ -21,15 +21,15 @@
 ]
 
 [project.optional-dependencies]
 dev = [
     "python-lsp-server[rope]==1.*",
     "pylint==2.*",
     "pylint-pytest==1.*",
-    "mypy[reports]==0.*",
+    "mypy[reports]==1.*",
     "ruff==0.*",
     "black[jupyter]==23.*",
     "isort==5.*",
     "bump2version==1.*",
     "pdbpp",
     # python -m ipykernel install --user --name ppqueue
     "ipykernel",
@@ -65,17 +65,17 @@
 ]
 extras = [
     "pandas>=1,<=2",
     "plotnine==0.*",
 ]
 
 [project.urls]
-Homepage = "https://www.Fresh2.dev/code/r/ppqueue/i"
+Homepage = "https://www.f2dv.com/r/ppqueue"
 Repository = "https://www.github.com/fresh2dev/ppqueue"
-Funding = "https://www.Fresh2.dev/funding"
+Funding = "https://www.f2dv.com/fund"
 
 [project.scripts]
 ppqueue = "ppqueue.__main__:main"
 
 [tool.setuptools.package-data]
 "*" = ["**"]
 [tool.setuptools.packages.find]
```

### Comparing `ppqueue-0.3.0/src/ppqueue/__pycache__/job.cpython-310.pyc` & `ppqueue-0.4.0/src/ppqueue/__pycache__/job.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 22 04:39:29 2023 UTC, .py size: 8072 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 81d0 9364 881f 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 a375 cd64 9d20 0000  o........u.d. ..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0005 0000 0040 0000 0173 b400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6400 6402 6c04 5a04 6400 6403 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 6d06 5a06 0100 6400 6404 6c07 6d08 5a08  m.Z...d.d.l.m.Z.
 00000060: 6d09 5a09 0100 6400 6405 6c0a 6d0a 5a0a  m.Z...d.d.l.m.Z.
 00000070: 0100 6400 6406 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
@@ -61,15 +61,15 @@
 000003c0: 6409 6414 6418 8d02 5a17 6421 6504 6422  d.d.d...Z.d!e.d"
 000003d0: 3c00 0900 6505 6409 6414 6418 8d02 5a18  <...e.d.d.d...Z.
 000003e0: 640a 6504 6423 3c00 0900 6505 6409 6414  d.e.d#<...e.d.d.
 000003f0: 6418 8d02 5a19 640a 6504 6424 3c00 0900  d...Z.d.e.d$<...
 00000400: 6505 6409 6414 6418 8d02 5a1a 640f 6504  e.d.d.d...Z.d.e.
 00000410: 6425 3c00 6505 6409 6414 6418 8d02 5a1b  d%<.e.d.d.d...Z.
 00000420: 6426 6504 6427 3c00 645c 642a 642b 8404  d&e.d'<.d\d*d+..
-00000430: 5a1c 645d 642e 642f 8404 5a1d 645e 6430  Z.d]d.d/..Z.d^d0
+00000430: 5a1c 645d 642d 642e 8404 5a1d 645e 6430  Z.d]d-d...Z.d^d0
 00000440: 6431 8404 5a1e 645e 6432 6433 8404 5a1f  d1..Z.d^d2d3..Z.
 00000450: 645e 6434 6435 8404 5a20 645e 6436 6437  d^d4d5..Z d^d6d7
 00000460: 8404 5a21 645e 6438 6439 8404 5a22 645e  ..Z!d^d8d9..Z"d^
 00000470: 643a 643b 8404 5a23 645f 643c 643d 8404  d:d;..Z#d_d<d=..
 00000480: 5a24 645f 643e 643f 8404 5a25 645c 6440  Z$d_d>d?..Z%d\d@
 00000490: 6441 8404 5a26 6460 6442 6443 8404 5a27  dA..Z&d`dBdC..Z'
 000004a0: 645c 6444 6445 8404 5a28 645c 6446 6447  d\dDdE..Z(d\dFdG
@@ -120,340 +120,358 @@
 00000770: 1e00 0000 da0a 6973 696e 7374 616e 6365  ......isinstance
 00000780: da03 7374 7272 0300 0000 721f 0000 00a9  ..strr....r.....
 00000790: 01da 0473 656c 6672 1a00 0000 721a 0000  ...selfr....r...
 000007a0: 0072 1b00 0000 da0d 5f5f 706f 7374 5f69  .r......__post_i
 000007b0: 6e69 745f 5f3e 0000 0073 0e00 0000 0a01  nit__>...s......
 000007c0: 0801 1801 0a01 0a02 0a01 04ff 7a11 4a6f  ............z.Jo
 000007d0: 622e 5f5f 706f 7374 5f69 6e69 745f 5fda  b.__post_init__.
-000007e0: 036a 6f62 da06 6f62 6a65 6374 6302 0000  .job..objectc...
-000007f0: 0000 0000 0000 0000 0002 0000 0005 0000  ................
-00000800: 0043 0000 0173 1200 0000 7400 7c00 7c01  .C...s....t.|.|.
-00000810: 6401 6402 6702 6403 8d03 5300 2904 6100  d.d.g.d...S.).a.
-00000820: 0100 0063 6f6d 7061 7265 7320 7477 6f20  ...compares two 
-00000830: 6a6f 6273 2062 7920 7072 696f 7269 7479  jobs by priority
-00000840: 206f 7220 696e 6465 782e 0a0a 2020 2020   or index...    
-00000850: 2020 2020 4172 6775 6d65 6e74 733a 0a20      Arguments:. 
-00000860: 2020 2020 2020 2020 2020 206a 6f62 207b             job {
-00000870: 7070 7175 6575 652e 4a6f 627d 0a0a 2020  ppqueue.Job}..  
-00000880: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
-00000890: 2020 2020 2020 2020 2020 2069 6e74 202d             int -
-000008a0: 2d20 6031 6020 6966 2060 7365 6c66 6020  - `1` if `self` 
-000008b0: 6973 2067 7265 6174 6572 2074 6861 6e20  is greater than 
-000008c0: 636f 6d70 6172 6973 6f6e 2c0a 2020 2020  comparison,.    
-000008d0: 2020 2020 2020 2020 2020 2020 2020 602d                `-
-000008e0: 3160 2069 6620 6073 656c 6660 2069 7320  1` if `self` is 
-000008f0: 6c65 7373 2074 6861 6e2c 0a20 2020 2020  less than,.     
-00000900: 2020 2020 2020 2020 2020 2020 2060 3060               `0`
-00000910: 2069 6620 6571 7561 6c2e 0a20 2020 2020   if equal..     
-00000920: 2020 2072 2300 0000 722e 0000 0029 015a     r#...r....).Z
-00000930: 0262 7972 0f00 0000 a902 7240 0000 0072  .byr......r@...r
-00000940: 4200 0000 721a 0000 0072 1a00 0000 721b  B...r....r....r.
-00000950: 0000 00da 085f 636f 6d70 6172 6547 0000  ....._compareG..
-00000960: 0073 0200 0000 120b 7a0c 4a6f 622e 5f63  .s......z.Job._c
-00000970: 6f6d 7061 7265 6302 0000 0000 0000 0000  omparec.........
-00000980: 0000 0002 0000 0003 0000 0043 0000 0173  ...........C...s
-00000990: 0e00 0000 7c00 a000 7c01 a101 6401 6b02  ....|...|...d.k.
-000009a0: 5300 a902 4e72 0100 0000 a901 7245 0000  S...Nr......rE..
-000009b0: 0072 4400 0000 721a 0000 0072 1a00 0000  .rD...r....r....
-000009c0: 721b 0000 00da 065f 5f65 715f 5f54 0000  r......__eq__T..
-000009d0: 00f3 0200 0000 0e01 7a0a 4a6f 622e 5f5f  ........z.Job.__
-000009e0: 6571 5f5f 6302 0000 0000 0000 0000 0000  eq__c...........
-000009f0: 0002 0000 0003 0000 0043 0000 0173 0e00  .........C...s..
-00000a00: 0000 7c00 a000 7c01 a101 6401 6b03 5300  ..|...|...d.k.S.
-00000a10: 7246 0000 0072 4700 0000 7244 0000 0072  rF...rG...rD...r
-00000a20: 1a00 0000 721a 0000 0072 1b00 0000 da06  ....r....r......
-00000a30: 5f5f 6e65 5f5f 5700 0000 7249 0000 007a  __ne__W...rI...z
-00000a40: 0a4a 6f62 2e5f 5f6e 655f 5f63 0200 0000  .Job.__ne__c....
-00000a50: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000a60: 4300 0001 730e 0000 007c 00a0 007c 01a1  C...s....|...|..
-00000a70: 0164 016b 0053 0072 4600 0000 7247 0000  .d.k.S.rF...rG..
-00000a80: 0072 4400 0000 721a 0000 0072 1a00 0000  .rD...r....r....
-00000a90: 721b 0000 00da 065f 5f6c 745f 5f5a 0000  r......__lt__Z..
-00000aa0: 0072 4900 0000 7a0a 4a6f 622e 5f5f 6c74  .rI...z.Job.__lt
-00000ab0: 5f5f 6302 0000 0000 0000 0000 0000 0002  __c.............
-00000ac0: 0000 0003 0000 0043 0000 0173 0e00 0000  .......C...s....
-00000ad0: 7c00 a000 7c01 a101 6401 6b01 5300 7246  |...|...d.k.S.rF
-00000ae0: 0000 0072 4700 0000 7244 0000 0072 1a00  ...rG...rD...r..
-00000af0: 0000 721a 0000 0072 1b00 0000 da06 5f5f  ..r....r......__
-00000b00: 6c65 5f5f 5d00 0000 7249 0000 007a 0a4a  le__]...rI...z.J
-00000b10: 6f62 2e5f 5f6c 655f 5f63 0200 0000 0000  ob.__le__c......
-00000b20: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
-00000b30: 0001 730e 0000 007c 00a0 007c 01a1 0164  ..s....|...|...d
-00000b40: 016b 0453 0072 4600 0000 7247 0000 0072  .k.S.rF...rG...r
-00000b50: 4400 0000 721a 0000 0072 1a00 0000 721b  D...r....r....r.
-00000b60: 0000 00da 065f 5f67 745f 5f60 0000 0072  .....__gt__`...r
-00000b70: 4900 0000 7a0a 4a6f 622e 5f5f 6774 5f5f  I...z.Job.__gt__
-00000b80: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00000b90: 0003 0000 0043 0000 0173 0e00 0000 7c00  .....C...s....|.
-00000ba0: a000 7c01 a101 6401 6b05 5300 7246 0000  ..|...d.k.S.rF..
-00000bb0: 0072 4700 0000 7244 0000 0072 1a00 0000  .rG...rD...r....
-00000bc0: 721a 0000 0072 1b00 0000 da06 5f5f 6765  r....r......__ge
-00000bd0: 5f5f 6300 0000 7249 0000 007a 0a4a 6f62  __c...rI...z.Job
-00000be0: 2e5f 5f67 655f 5f63 0100 0000 0000 0000  .__ge__c........
-00000bf0: 0000 0000 0100 0000 0200 0000 4300 0001  ............C...
-00000c00: 7314 0000 007c 006a 0064 0075 016f 097c  s....|.j.d.u.o.|
-00000c10: 006a 00a0 01a1 0053 0072 3c00 0000 2902  .j.....S.r<...).
-00000c20: 7239 0000 00da 0869 735f 616c 6976 6572  r9.....is_aliver
-00000c30: 3f00 0000 721a 0000 0072 1a00 0000 721b  ?...r....r....r.
-00000c40: 0000 00da 0a69 735f 7275 6e6e 696e 6766  .....is_runningf
-00000c50: 0000 0073 0200 0000 1401 7a0e 4a6f 622e  ...s......z.Job.
-00000c60: 6973 5f72 756e 6e69 6e67 6301 0000 0000  is_runningc.....
-00000c70: 0000 0000 0000 0001 0000 0003 0000 0043  ...............C
-00000c80: 0000 0173 3a00 0000 7c00 a000 a100 6f1c  ...s:...|.....o.
-00000c90: 7c00 6a01 6401 6b04 6f1c 7c00 6a02 6400  |.j.d.k.o.|.j.d.
-00000ca0: 7501 6f1c 7c00 6a03 6400 7500 6f1c 7c00  u.o.|.j.d.u.o.|.
-00000cb0: 6a02 7c00 6a01 1700 7404 a004 a100 6b00  j.|.j...t.....k.
-00000cc0: 5300 7246 0000 0029 0572 5000 0000 7227  S.rF...).rP...r'
-00000cd0: 0000 0072 3200 0000 7233 0000 00da 0474  ...r2...r3.....t
-00000ce0: 696d 6572 3f00 0000 721a 0000 0072 1a00  imer?...r....r..
-00000cf0: 0000 721b 0000 00da 0a69 735f 6578 7069  ..r......is_expi
-00000d00: 7265 6469 0000 0073 1200 0000 0802 0801  redi...s........
-00000d10: 02ff 0802 02fe 0803 02fd 1204 02fb 7a0e  ..............z.
-00000d20: 4a6f 622e 6973 5f65 7870 6972 6564 6301  Job.is_expiredc.
-00000d30: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-00000d40: 0000 004f 0000 0173 2400 0000 7c00 6a00  ...O...s$...|.j.
-00000d50: 6400 7501 7210 7c00 6a00 6a01 7c01 6900  d.u.r.|.j.j.|.i.
-00000d60: 7c02 a401 8e01 0100 6400 5300 6400 5300  |.......d.S.d.S.
-00000d70: 723c 0000 0029 0272 3900 0000 da04 6a6f  r<...).r9.....jo
-00000d80: 696e 2903 7240 0000 0072 1e00 0000 721f  in).r@...r....r.
-00000d90: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00000da0: 0000 7253 0000 0072 0000 0073 0600 0000  ..rS...r...s....
-00000db0: 0a02 1601 04ff 7a08 4a6f 622e 6a6f 696e  ......z.Job.join
-00000dc0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000dd0: 0003 0000 0043 0000 0173 2a00 0000 7c00  .....C...s*...|.
-00000de0: 6a00 720f 7401 7c00 6a00 6401 8302 720f  j.r.t.|.j.d...r.
-00000df0: 7c00 6a00 6a02 6402 7500 7211 6402 5300  |.j.j.d.u.r.d.S.
-00000e00: 7c00 6a00 6a02 5300 2903 7a15 4578 6974  |.j.j.S.).z.Exit
-00000e10: 2063 6f64 6520 6f66 2074 6865 206a 6f62   code of the job
-00000e20: 2e72 3800 0000 4e29 0372 3900 0000 da07  .r8...N).r9.....
-00000e30: 6861 7361 7474 7272 3800 0000 723f 0000  hasattrr8...r?..
-00000e40: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00000e50: da0d 6765 745f 6578 6974 5f63 6f64 6577  ..get_exit_codew
-00000e60: 0000 0073 0e00 0000 0403 02ff 0a02 02fe  ...s............
-00000e70: 0c03 0402 0801 7a11 4a6f 622e 6765 745f  ......z.Job.get_
-00000e80: 6578 6974 5f63 6f64 6563 0100 0000 0000  exit_codec......
-00000e90: 0000 0000 0000 0100 0000 0200 0000 4300  ..............C.
-00000ea0: 0001 731c 0000 007c 006a 0064 0075 0172  ..s....|.j.d.u.r
-00000eb0: 0c7c 006a 00a0 01a1 0001 0064 0053 0064  .|.j.......d.S.d
-00000ec0: 0053 0072 3c00 0000 2902 7239 0000 00da  .S.r<...).r9....
-00000ed0: 0974 6572 6d69 6e61 7465 723f 0000 0072  .terminater?...r
-00000ee0: 1a00 0000 721a 0000 0072 1b00 0000 7256  ....r....r....rV
-00000ef0: 0000 0081 0000 0073 0600 0000 0a01 0e01  .......s........
-00000f00: 04ff 7a0d 4a6f 622e 7465 726d 696e 6174  ..z.Job.terminat
-00000f10: 6563 0100 0000 0000 0000 0000 0000 0100  ec..............
-00000f20: 0000 0400 0000 4300 0001 7362 0000 007c  ......C...sb...|
-00000f30: 006a 0072 077c 00a0 01a1 0073 0964 0053  .j.r.|.....s.d.S
-00000f40: 0074 027c 006a 0064 0183 0273 1674 03a0  .t.|.j.d...s.t..
-00000f50: 0464 02a1 0101 0064 0053 007c 006a 00a0  .d.....d.S.|.j..
-00000f60: 05a1 0001 007c 006a 00a0 06a1 0001 0074  .....|.j.......t
-00000f70: 07a0 07a1 007c 005f 0864 037c 005f 0974  .....|._.d.|._.t
-00000f80: 03a0 0a64 047c 006a 0ba1 0201 0064 0053  ...d.|.j.....d.S
-00000f90: 0029 054e 7256 0000 007a 1b55 6e61 626c  .).NrV...z.Unabl
-00000fa0: 6520 746f 2074 6572 6d69 6e61 7465 2074  e to terminate t
-00000fb0: 6872 6561 642e 547a 1253 746f 7070 6564  hread.Tz.Stopped
-00000fc0: 2064 6174 613a 2027 2564 2729 0c72 3900   data: '%d').r9.
-00000fd0: 0000 7250 0000 0072 5400 0000 da03 6c6f  ..rP...rT.....lo
-00000fe0: 6772 3700 0000 7256 0000 0072 5300 0000  gr7...rV...rS...
-00000ff0: 7251 0000 0072 3300 0000 722f 0000 00da  rQ...r3...r/....
-00001000: 0564 6562 7567 722e 0000 0072 3f00 0000  .debugr....r?...
-00001010: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00001020: 0473 746f 7085 0000 0073 1200 0000 0e02  .stop....s......
-00001030: 0401 0c01 0e01 0a02 0a01 0a01 0601 1201  ................
-00001040: 7a08 4a6f 622e 7374 6f70 6301 0000 0000  z.Job.stopc.....
-00001050: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-00001060: 0000 0173 1c00 0000 7c00 6a00 7206 7c00  ...s....|.j.r.|.
-00001070: 6a01 7308 6401 5300 7c00 6a01 7c00 6a00  j.s.d.S.|.j.|.j.
-00001080: 1800 5300 2902 6199 0100 0054 6865 206e  ..S.).a....The n
-00001090: 756d 6265 7220 6f66 2073 6563 6f6e 6473  umber of seconds
-000010a0: 2061 206a 6f62 2077 6173 2072 756e 6e69   a job was runni
-000010b0: 6e67 2066 6f72 2e0a 0a20 2020 2020 2020  ng for...       
-000010c0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-000010d0: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
-000010e0: 7070 7175 6575 6520 696d 706f 7274 2051  ppqueue import Q
-000010f0: 7565 7565 0a20 2020 2020 2020 2020 2020  ueue.           
-00001100: 203e 3e3e 2066 726f 6d20 7469 6d65 2069   >>> from time i
-00001110: 6d70 6f72 7420 736c 6565 700a 2020 2020  mport sleep.    
-00001120: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00001130: 2020 2020 2020 2020 3e3e 3e20 7769 7468          >>> with
-00001140: 2051 7565 7565 2829 2061 7320 7175 6575   Queue() as queu
-00001150: 653a 0a20 2020 2020 2020 2020 2020 202e  e:.            .
-00001160: 2e2e 2020 2020 2066 6f72 2069 2069 6e20  ..     for i in 
-00001170: 7261 6e67 6528 3529 3a0a 2020 2020 2020  range(5):.      
-00001180: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
-00001190: 2020 6a6f 6273 203d 2071 7565 7565 2e6d    jobs = queue.m
-000011a0: 6170 2873 6c65 6570 2c20 5b31 2c20 322c  ap(sleep, [1, 2,
-000011b0: 2033 5d29 0a20 2020 2020 2020 2020 2020   3]).           
-000011c0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-000011d0: 203e 3e3e 205b 696e 7428 6a6f 622e 6765   >>> [int(job.ge
-000011e0: 745f 7365 636f 6e64 735f 7275 6e6e 696e  t_seconds_runnin
-000011f0: 6728 2929 2066 6f72 206a 6f62 2069 6e20  g()) for job in 
-00001200: 6a6f 6273 5d0a 2020 2020 2020 2020 2020  jobs].          
-00001210: 2020 5b31 2c20 322c 2033 5d0a 2020 2020    [1, 2, 3].    
-00001220: 2020 2020 4e29 0272 3200 0000 7233 0000      N).r2...r3..
-00001230: 0072 3f00 0000 721a 0000 0072 1a00 0000  .r?...r....r....
-00001240: 721b 0000 00da 1367 6574 5f73 6563 6f6e  r......get_secon
-00001250: 6473 5f72 756e 6e69 6e67 9200 0000 7306  ds_running....s.
-00001260: 0000 000c 0e04 010c 017a 174a 6f62 2e67  .........z.Job.g
-00001270: 6574 5f73 6563 6f6e 6473 5f72 756e 6e69  et_seconds_runni
-00001280: 6e67 6301 0000 0000 0000 0000 0000 0001  ngc.............
-00001290: 0000 0002 0000 0043 0000 01f3 2a00 0000  .......C....*...
-000012a0: 7c00 6a00 7305 6401 5300 7c00 6a01 730f  |.j.s.d.S.|.j.s.
-000012b0: 7402 a002 a100 7c00 6a00 1800 5300 7c00  t.....|.j...S.|.
-000012c0: 6a01 7c00 6a00 1800 5300 2902 7a91 5468  j.|.j...S.).z.Th
-000012d0: 6520 616d 6f75 6e74 206f 6620 7469 6d65  e amount of time
-000012e0: 2061 2064 6174 6120 6861 7320 7370 656e   a data has spen
-000012f0: 7420 696e 2074 6865 2077 6169 7469 6e67  t in the waiting
-00001300: 2071 7565 7565 2e0a 0a20 2020 2020 2020   queue...       
-00001310: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-00001320: 2020 2020 2020 203e 3e3e 206a 6f62 2e67         >>> job.g
-00001330: 6574 5f73 6563 6f6e 6473 5f77 6169 7469  et_seconds_waiti
-00001340: 6e67 2829 2020 2320 646f 6374 6573 743a  ng()  # doctest:
-00001350: 202b 534b 4950 0a20 2020 2020 2020 204e   +SKIP.        N
-00001360: 2903 7231 0000 0072 3200 0000 7251 0000  ).r1...r2...rQ..
-00001370: 0072 3f00 0000 721a 0000 0072 1a00 0000  .r?...r....r....
-00001380: 721b 0000 00da 1367 6574 5f73 6563 6f6e  r......get_secon
-00001390: 6473 5f77 6169 7469 6e67 a400 0000 f30a  ds_waiting......
-000013a0: 0000 0006 0604 0106 020e 010c 027a 174a  .............z.J
-000013b0: 6f62 2e67 6574 5f73 6563 6f6e 6473 5f77  ob.get_seconds_w
-000013c0: 6169 7469 6e67 6301 0000 0000 0000 0000  aitingc.........
-000013d0: 0000 0001 0000 0002 0000 0043 0000 0172  ...........C...r
-000013e0: 5b00 0000 2902 7a89 5265 7475 726e 7320  [...).z.Returns 
-000013f0: 7468 6520 7761 6974 696e 6720 2b20 7275  the waiting + ru
-00001400: 6e6e 696e 6720 6475 7261 7469 6f6e 206f  nning duration o
-00001410: 6620 7468 6973 206a 6f62 2e0a 0a20 2020  f this job...   
-00001420: 2020 2020 2045 7861 6d70 6c65 733a 0a20       Examples:. 
-00001430: 2020 2020 2020 2020 2020 203e 3e3e 206a             >>> j
-00001440: 6f62 2e67 6574 5f73 6563 6f6e 6473 5f74  ob.get_seconds_t
-00001450: 6f74 616c 2829 2020 2320 646f 6374 6573  otal()  # doctes
-00001460: 743a 202b 534b 4950 0a20 2020 2020 2020  t: +SKIP.       
-00001470: 204e 2903 7231 0000 0072 3300 0000 7251   N).r1...r3...rQ
-00001480: 0000 0072 3f00 0000 721a 0000 0072 1a00  ...r?...r....r..
-00001490: 0000 721b 0000 00da 1167 6574 5f73 6563  ..r......get_sec
-000014a0: 6f6e 6473 5f74 6f74 616c b200 0000 725d  onds_total....r]
-000014b0: 0000 007a 154a 6f62 2e67 6574 5f73 6563  ...z.Job.get_sec
-000014c0: 6f6e 6473 5f74 6f74 616c fa0f 6461 7465  onds_total..date
-000014d0: 7469 6d65 207c 204e 6f6e 6563 0100 0000  time | Nonec....
-000014e0: 0000 0000 0000 0000 0100 0000 0300 0000  ................
-000014f0: 4300 0001 f316 0000 007c 006a 0072 0974  C........|.j.r.t
-00001500: 01a0 027c 006a 00a1 0153 0064 0153 0029  ...|.j...S.d.S.)
-00001510: 027a 7954 6865 2074 696d 6520 7468 6973  .zyThe time this
-00001520: 206a 6f62 2077 6173 2073 7562 6d69 7474   job was submitt
-00001530: 6564 2e0a 0a20 2020 2020 2020 2045 7861  ed...        Exa
-00001540: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
-00001550: 2020 203e 3e3e 206a 6f62 2e67 6574 5f73     >>> job.get_s
-00001560: 7562 6d69 745f 7469 6d65 7374 616d 7028  ubmit_timestamp(
-00001570: 2920 2023 2064 6f63 7465 7374 3a20 2b53  )  # doctest: +S
-00001580: 4b49 500a 2020 2020 2020 2020 4e29 0372  KIP.        N).r
-00001590: 3100 0000 7206 0000 00da 1075 7463 6672  1...r......utcfr
-000015a0: 6f6d 7469 6d65 7374 616d 7072 3f00 0000  omtimestampr?...
-000015b0: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-000015c0: 1467 6574 5f73 7562 6d69 745f 7469 6d65  .get_submit_time
-000015d0: 7374 616d 70c0 0000 0073 0600 0000 0606  stamp....s......
-000015e0: 0c01 0401 7a18 4a6f 622e 6765 745f 7375  ....z.Job.get_su
-000015f0: 626d 6974 5f74 696d 6573 7461 6d70 6301  bmit_timestampc.
-00001600: 0000 0000 0000 0000 0000 0001 0000 0003  ................
-00001610: 0000 0043 0000 0172 6000 0000 2902 7a3c  ...C...r`...).z<
-00001620: 5265 7475 726e 7320 6120 6461 7465 7469  Returns a dateti
-00001630: 6d65 206f 626a 6563 7420 6f66 2074 6865  me object of the
-00001640: 2074 696d 6520 7468 6973 2064 6174 6120   time this data 
-00001650: 7761 7320 7374 6172 7465 642e 4e29 0372  was started.N).r
-00001660: 3200 0000 7206 0000 0072 6100 0000 723f  2...r....ra...r?
-00001670: 0000 0072 1a00 0000 721a 0000 0072 1b00  ...r....r....r..
-00001680: 0000 da13 6765 745f 7374 6172 745f 7469  ....get_start_ti
-00001690: 6d65 7374 616d 70ca 0000 00f3 0600 0000  mestamp.........
-000016a0: 0602 0c01 0401 7a17 4a6f 622e 6765 745f  ......z.Job.get_
-000016b0: 7374 6172 745f 7469 6d65 7374 616d 7063  start_timestampc
-000016c0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
-000016d0: 0300 0000 4300 0001 7260 0000 0029 027a  ....C...r`...).z
-000016e0: 3952 6574 7572 6e73 2061 2064 6174 6574  9Returns a datet
-000016f0: 696d 6520 6f62 6a65 6374 206f 6620 7468  ime object of th
-00001700: 6520 7469 6d65 2074 6869 7320 6461 7461  e time this data
-00001710: 2066 696e 6973 6865 642e 4e29 0372 3300   finished.N).r3.
-00001720: 0000 7206 0000 0072 6100 0000 723f 0000  ..r....ra...r?..
-00001730: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001740: da14 6765 745f 6669 6e69 7368 5f74 696d  ..get_finish_tim
-00001750: 6573 7461 6d70 d000 0000 7264 0000 007a  estamp....rd...z
-00001760: 184a 6f62 2e67 6574 5f66 696e 6973 685f  .Job.get_finish_
-00001770: 7469 6d65 7374 616d 7063 0100 0000 0000  timestampc......
-00001780: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
-00001790: 0001 7260 0000 0029 027a 3e52 6574 7572  ..r`...).z>Retur
-000017a0: 6e73 2061 2064 6174 6574 696d 6520 6f62  ns a datetime ob
-000017b0: 6a65 6374 206f 6620 7468 6520 7469 6d65  ject of the time
-000017c0: 2074 6869 7320 6461 7461 2077 6173 2070   this data was p
-000017d0: 726f 6365 7373 6564 2e4e 2903 7234 0000  rocessed.N).r4..
-000017e0: 0072 0600 0000 7261 0000 0072 3f00 0000  .r....ra...r?...
-000017f0: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
-00001800: 1767 6574 5f70 726f 6365 7373 6564 5f74  .get_processed_t
-00001810: 696d 6573 7461 6d70 d600 0000 7264 0000  imestamp....rd..
-00001820: 007a 1b4a 6f62 2e67 6574 5f70 726f 6365  .z.Job.get_proce
-00001830: 7373 6564 5f74 696d 6573 7461 6d70 6301  ssed_timestampc.
-00001840: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00001850: 0000 0043 0000 0173 0a00 0000 7c00 6a00  ...C...s....|.j.
-00001860: 6400 7501 5300 723c 0000 0029 0172 3400  d.u.S.r<...).r4.
-00001870: 0000 723f 0000 0072 1a00 0000 721a 0000  ..r?...r....r...
-00001880: 0072 1b00 0000 da0c 6973 5f70 726f 6365  .r......is_proce
-00001890: 7373 6564 dc00 0000 7302 0000 000a 057a  ssed....s......z
-000018a0: 104a 6f62 2e69 735f 7072 6f63 6573 7365  .Job.is_processe
-000018b0: 6472 1100 0000 6301 0000 0000 0000 0000  dr....c.........
-000018c0: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-000018d0: 3800 0000 7c00 6a00 7306 7401 6a02 5300  8...|.j.s.t.j.S.
-000018e0: 7c00 a003 a100 720d 7401 6a04 5300 7c00  |.....r.t.j.S.|.
-000018f0: 6a05 7213 7401 6a06 5300 7c00 6a07 7219  j.r.t.j.S.|.j.r.
-00001900: 7401 6a08 5300 7401 6a09 5300 723c 0000  t.j.S.t.j.S.r<..
-00001910: 0029 0a72 3100 0000 7211 0000 0072 1500  .).r1...r....r..
-00001920: 0000 7250 0000 0072 1600 0000 722f 0000  ..rP...r....r/..
-00001930: 0072 1700 0000 7233 0000 0072 1800 0000  .r....r3...r....
-00001940: 7219 0000 0072 3f00 0000 721a 0000 0072  r....r?...r....r
-00001950: 1a00 0000 721b 0000 00da 0967 6574 5f73  ....r......get_s
-00001960: 7461 7465 e300 0000 7312 0000 0006 0106  tate....s.......
-00001970: 0108 0106 0106 0106 0106 0106 0106 017a  ...............z
-00001980: 0d4a 6f62 2e67 6574 5f73 7461 7465 2902  .Job.get_state).
-00001990: 723a 0000 0072 3b00 0000 2904 7242 0000  r:...r;...).rB..
-000019a0: 0072 4300 0000 723a 0000 0072 2200 0000  .rC...r:...r"...
-000019b0: 2904 7242 0000 0072 4300 0000 723a 0000  ).rB...rC...r:..
-000019c0: 0072 2800 0000 2902 723a 0000 0072 2800  .r(...).r:...r(.
-000019d0: 0000 2902 723a 0000 0072 2400 0000 2902  ..).r:...r$...).
-000019e0: 723a 0000 0072 3000 0000 2902 723a 0000  r:...r0...).r:..
-000019f0: 0072 5f00 0000 2902 723a 0000 0072 1100  .r_...).r:...r..
-00001a00: 0000 2933 7212 0000 0072 1300 0000 7214  ..)3r....r....r.
-00001a10: 0000 00da 075f 5f64 6f63 5f5f da0f 5f5f  .....__doc__..__
-00001a20: 616e 6e6f 7461 7469 6f6e 735f 5f72 0500  annotations__r..
-00001a30: 0000 da04 6c69 7374 721e 0000 00da 0464  ....listr......d
-00001a40: 6963 7472 1f00 0000 7220 0000 0072 2300  ictr....r ...r#.
-00001a50: 0000 7225 0000 0072 2700 0000 7229 0000  ..r%...r'...r)..
-00001a60: 0072 2a00 0000 722d 0000 0072 2e00 0000  .r*...r-...r....
-00001a70: 722f 0000 0072 3100 0000 7232 0000 0072  r/...r1...r2...r
-00001a80: 3300 0000 7234 0000 0072 3500 0000 7236  3...r4...r5...r6
-00001a90: 0000 0072 3700 0000 7238 0000 0072 3900  ...r7...r8...r9.
-00001aa0: 0000 7241 0000 0072 4500 0000 7248 0000  ..rA...rE...rH..
-00001ab0: 0072 4a00 0000 724b 0000 0072 4c00 0000  .rJ...rK...rL...
-00001ac0: 724d 0000 0072 4e00 0000 7250 0000 0072  rM...rN...rP...r
-00001ad0: 5200 0000 7253 0000 0072 5500 0000 7256  R...rS...rU...rV
-00001ae0: 0000 0072 5900 0000 725a 0000 0072 5c00  ...rY...rZ...r\.
-00001af0: 0000 725e 0000 0072 6200 0000 7263 0000  ..r^...rb...rc..
-00001b00: 0072 6500 0000 7266 0000 0072 6700 0000  .re...rf...rg...
-00001b10: 7268 0000 0072 1a00 0000 721a 0000 0072  rh...r....r....r
-00001b20: 1a00 0000 721b 0000 0072 1c00 0000 1900  ....r....r......
-00001b30: 0000 7370 0000 000a 0004 0208 0212 0112  ..sp............
-00001b40: 010c 010c 010c 010c 010c 010c 0114 0202  ................
-00001b50: 0114 0102 0114 0102 0114 0102 0114 0102  ................
-00001b60: 0114 0102 0114 0102 0114 0102 0114 0102  ................
-00001b70: 0114 0102 0114 0114 010a 020a 090a 0d0a  ................
-00001b80: 030a 030a 030a 030a 030a 030a 030a 090a  ................
-00001b90: 050a 0a0a 040a 0d0a 120a 0e0a 0e0a 0a0a  ................
-00001ba0: 060a 060a 060e 0772 1c00 0000 291b da0a  .......r....)...
-00001bb0: 5f5f 6675 7475 7265 5f5f 7202 0000 00da  __future__r.....
-00001bc0: 076c 6f67 6769 6e67 7257 0000 0072 5100  .loggingrW...rQ.
-00001bd0: 0000 da0f 636f 6c6c 6563 7469 6f6e 732e  ....collections.
-00001be0: 6162 6372 0300 0000 da0b 6461 7461 636c  abcr......datacl
-00001bf0: 6173 7365 7372 0400 0000 7205 0000 0072  assesr....r....r
-00001c00: 0600 0000 da04 656e 756d 7207 0000 0072  ......enumr....r
-00001c10: 0800 0000 da0f 6d75 6c74 6970 726f 6365  ......multiproce
-00001c20: 7373 696e 6772 0900 0000 da09 7468 7265  ssingr......thre
-00001c30: 6164 696e 6772 0a00 0000 da06 7479 7069  adingr......typi
-00001c40: 6e67 720b 0000 0072 0c00 0000 720d 0000  ngr....r....r...
-00001c50: 00da 0575 7469 6c73 7210 0000 0072 1100  ...utilsr....r..
-00001c60: 0000 7243 0000 0072 1c00 0000 721a 0000  ..rC...r....r...
-00001c70: 0072 1a00 0000 721a 0000 0072 1b00 0000  .r....r....r....
-00001c80: da08 3c6d 6f64 756c 653e 0100 0000 731c  ..<module>....s.
-00001c90: 0000 000c 0008 0208 010c 0110 010c 0110  ................
-00001ca0: 010c 010c 0114 010c 0210 0302 0916 01    ...............
+000007e0: 036a 6f62 6302 0000 0000 0000 0000 0000  .jobc...........
+000007f0: 0002 0000 0005 0000 0043 0000 0173 1200  .........C...s..
+00000800: 0000 7400 7c00 7c01 6401 6402 6702 6403  ..t.|.|.d.d.g.d.
+00000810: 8d03 5300 2904 7ae4 636f 6d70 6172 6573  ..S.).z.compares
+00000820: 2074 776f 206a 6f62 7320 6279 2070 7269   two jobs by pri
+00000830: 6f72 6974 7920 6f72 2069 6e64 6578 2e0a  ority or index..
+00000840: 0a20 2020 2020 2020 2041 7267 756d 656e  .        Argumen
+00000850: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00000860: 6a6f 623a 202e 2e2e 0a0a 2020 2020 2020  job: .....      
+00000870: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+00000880: 2020 2020 2020 2060 3160 2069 6620 6073         `1` if `s
+00000890: 656c 6660 2069 7320 6772 6561 7465 7220  elf` is greater 
+000008a0: 7468 616e 2063 6f6d 7061 7269 736f 6e2c  than comparison,
+000008b0: 0a20 2020 2020 2020 2020 2020 2060 2d31  .            `-1
+000008c0: 6020 6966 2060 7365 6c66 6020 6973 206c  ` if `self` is l
+000008d0: 6573 7320 7468 616e 2c0a 2020 2020 2020  ess than,.      
+000008e0: 2020 2020 2020 6030 6020 6966 2065 7175        `0` if equ
+000008f0: 616c 2e0a 2020 2020 2020 2020 7223 0000  al..        r#..
+00000900: 0072 2e00 0000 2901 5a02 6279 720f 0000  .r....).Z.byr...
+00000910: 00a9 0272 4000 0000 7242 0000 0072 1a00  ...r@...rB...r..
+00000920: 0000 721a 0000 0072 1b00 0000 da08 5f63  ..r....r......_c
+00000930: 6f6d 7061 7265 4700 0000 7302 0000 0012  ompareG...s.....
+00000940: 0b7a 0c4a 6f62 2e5f 636f 6d70 6172 65da  .z.Job._compare.
+00000950: 066f 626a 6563 7463 0200 0000 0000 0000  .objectc........
+00000960: 0000 0000 0200 0000 0300 0000 4300 0001  ............C...
+00000970: 730e 0000 007c 00a0 007c 01a1 0164 016b  s....|...|...d.k
+00000980: 0253 00a9 024e 7201 0000 00a9 0172 4400  .S...Nr......rD.
+00000990: 0000 7243 0000 0072 1a00 0000 721a 0000  ..rC...r....r...
+000009a0: 0072 1b00 0000 da06 5f5f 6571 5f5f 5400  .r......__eq__T.
+000009b0: 0000 f302 0000 000e 017a 0a4a 6f62 2e5f  .........z.Job._
+000009c0: 5f65 715f 5f63 0200 0000 0000 0000 0000  _eq__c..........
+000009d0: 0000 0200 0000 0300 0000 4300 0001 730e  ..........C...s.
+000009e0: 0000 007c 00a0 007c 01a1 0164 016b 0353  ...|...|...d.k.S
+000009f0: 0072 4600 0000 7247 0000 0072 4300 0000  .rF...rG...rC...
+00000a00: 721a 0000 0072 1a00 0000 721b 0000 00da  r....r....r.....
+00000a10: 065f 5f6e 655f 5f57 0000 0072 4900 0000  .__ne__W...rI...
+00000a20: 7a0a 4a6f 622e 5f5f 6e65 5f5f 6302 0000  z.Job.__ne__c...
+00000a30: 0000 0000 0000 0000 0002 0000 0003 0000  ................
+00000a40: 0043 0000 0173 0e00 0000 7c00 a000 7c01  .C...s....|...|.
+00000a50: a101 6401 6b00 5300 7246 0000 0072 4700  ..d.k.S.rF...rG.
+00000a60: 0000 7243 0000 0072 1a00 0000 721a 0000  ..rC...r....r...
+00000a70: 0072 1b00 0000 da06 5f5f 6c74 5f5f 5a00  .r......__lt__Z.
+00000a80: 0000 7249 0000 007a 0a4a 6f62 2e5f 5f6c  ..rI...z.Job.__l
+00000a90: 745f 5f63 0200 0000 0000 0000 0000 0000  t__c............
+00000aa0: 0200 0000 0300 0000 4300 0001 730e 0000  ........C...s...
+00000ab0: 007c 00a0 007c 01a1 0164 016b 0153 0072  .|...|...d.k.S.r
+00000ac0: 4600 0000 7247 0000 0072 4300 0000 721a  F...rG...rC...r.
+00000ad0: 0000 0072 1a00 0000 721b 0000 00da 065f  ...r....r......_
+00000ae0: 5f6c 655f 5f5d 0000 0072 4900 0000 7a0a  _le__]...rI...z.
+00000af0: 4a6f 622e 5f5f 6c65 5f5f 6302 0000 0000  Job.__le__c.....
+00000b00: 0000 0000 0000 0002 0000 0003 0000 0043  ...............C
+00000b10: 0000 0173 0e00 0000 7c00 a000 7c01 a101  ...s....|...|...
+00000b20: 6401 6b04 5300 7246 0000 0072 4700 0000  d.k.S.rF...rG...
+00000b30: 7243 0000 0072 1a00 0000 721a 0000 0072  rC...r....r....r
+00000b40: 1b00 0000 da06 5f5f 6774 5f5f 6000 0000  ......__gt__`...
+00000b50: 7249 0000 007a 0a4a 6f62 2e5f 5f67 745f  rI...z.Job.__gt_
+00000b60: 5f63 0200 0000 0000 0000 0000 0000 0200  _c..............
+00000b70: 0000 0300 0000 4300 0001 730e 0000 007c  ......C...s....|
+00000b80: 00a0 007c 01a1 0164 016b 0553 0072 4600  ...|...d.k.S.rF.
+00000b90: 0000 7247 0000 0072 4300 0000 721a 0000  ..rG...rC...r...
+00000ba0: 0072 1a00 0000 721b 0000 00da 065f 5f67  .r....r......__g
+00000bb0: 655f 5f63 0000 0072 4900 0000 7a0a 4a6f  e__c...rI...z.Jo
+00000bc0: 622e 5f5f 6765 5f5f 6301 0000 0000 0000  b.__ge__c.......
+00000bd0: 0000 0000 0001 0000 0002 0000 0043 0000  .............C..
+00000be0: 0173 1400 0000 7c00 6a00 6400 7501 6f09  .s....|.j.d.u.o.
+00000bf0: 7c00 6a00 a001 a100 5300 723c 0000 0029  |.j.....S.r<...)
+00000c00: 0272 3900 0000 da08 6973 5f61 6c69 7665  .r9.....is_alive
+00000c10: 723f 0000 0072 1a00 0000 721a 0000 0072  r?...r....r....r
+00000c20: 1b00 0000 da0a 6973 5f72 756e 6e69 6e67  ......is_running
+00000c30: 6600 0000 7302 0000 0014 017a 0e4a 6f62  f...s......z.Job
+00000c40: 2e69 735f 7275 6e6e 696e 6763 0100 0000  .is_runningc....
+00000c50: 0000 0000 0000 0000 0100 0000 0300 0000  ................
+00000c60: 4300 0001 733a 0000 007c 00a0 00a1 006f  C...s:...|.....o
+00000c70: 1c7c 006a 0164 016b 046f 1c7c 006a 0264  .|.j.d.k.o.|.j.d
+00000c80: 0075 016f 1c7c 006a 0364 0075 006f 1c7c  .u.o.|.j.d.u.o.|
+00000c90: 006a 027c 006a 0117 0074 04a0 04a1 006b  .j.|.j...t.....k
+00000ca0: 0053 0072 4600 0000 2905 7250 0000 0072  .S.rF...).rP...r
+00000cb0: 2700 0000 7232 0000 0072 3300 0000 da04  '...r2...r3.....
+00000cc0: 7469 6d65 723f 0000 0072 1a00 0000 721a  timer?...r....r.
+00000cd0: 0000 0072 1b00 0000 da0a 6973 5f65 7870  ...r......is_exp
+00000ce0: 6972 6564 6900 0000 7312 0000 0008 0208  iredi...s.......
+00000cf0: 0102 ff08 0202 fe08 0302 fd12 0402 fb7a  ...............z
+00000d00: 0e4a 6f62 2e69 735f 6578 7069 7265 6463  .Job.is_expiredc
+00000d10: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+00000d20: 0400 0000 4f00 0001 7324 0000 007c 006a  ....O...s$...|.j
+00000d30: 0064 0075 0172 107c 006a 006a 017c 0169  .d.u.r.|.j.j.|.i
+00000d40: 007c 02a4 018e 0101 0064 0053 0064 0053  .|.......d.S.d.S
+00000d50: 0072 3c00 0000 2902 7239 0000 00da 046a  .r<...).r9.....j
+00000d60: 6f69 6e29 0372 4000 0000 721e 0000 0072  oin).r@...r....r
+00000d70: 1f00 0000 721a 0000 0072 1a00 0000 721b  ....r....r....r.
+00000d80: 0000 0072 5300 0000 7200 0000 7306 0000  ...rS...r...s...
+00000d90: 000a 0216 0104 ff7a 084a 6f62 2e6a 6f69  .......z.Job.joi
+00000da0: 6e63 0100 0000 0000 0000 0000 0000 0100  nc..............
+00000db0: 0000 0300 0000 4300 0001 732a 0000 007c  ......C...s*...|
+00000dc0: 006a 0072 0f74 017c 006a 0064 0183 0272  .j.r.t.|.j.d...r
+00000dd0: 0f7c 006a 006a 0264 0275 0072 1164 0253  .|.j.j.d.u.r.d.S
+00000de0: 007c 006a 006a 0253 0029 037a 4045 7869  .|.j.j.S.).z@Exi
+00000df0: 7420 636f 6465 206f 6620 7468 6520 6a6f  t code of the jo
+00000e00: 622e 0a0a 2020 2020 2020 2020 5265 7475  b...        Retu
+00000e10: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00000e20: 202e 2e2e 0a20 2020 2020 2020 2072 3800   ....        r8.
+00000e30: 0000 4e29 0372 3900 0000 da07 6861 7361  ..N).r9.....hasa
+00000e40: 7474 7272 3800 0000 723f 0000 0072 1a00  ttrr8...r?...r..
+00000e50: 0000 721a 0000 0072 1b00 0000 da0d 6765  ..r....r......ge
+00000e60: 745f 6578 6974 5f63 6f64 6577 0000 0073  t_exit_codew...s
+00000e70: 0e00 0000 0407 02ff 0a02 02fe 0c03 0402  ................
+00000e80: 0801 7a11 4a6f 622e 6765 745f 6578 6974  ..z.Job.get_exit
+00000e90: 5f63 6f64 6563 0100 0000 0000 0000 0000  _codec..........
+00000ea0: 0000 0100 0000 0200 0000 4300 0001 731c  ..........C...s.
+00000eb0: 0000 007c 006a 0064 0075 0172 0c7c 006a  ...|.j.d.u.r.|.j
+00000ec0: 00a0 01a1 0001 0064 0053 0064 0053 0072  .......d.S.d.S.r
+00000ed0: 3c00 0000 2902 7239 0000 00da 0974 6572  <...).r9.....ter
+00000ee0: 6d69 6e61 7465 723f 0000 0072 1a00 0000  minater?...r....
+00000ef0: 721a 0000 0072 1b00 0000 7256 0000 0085  r....r....rV....
+00000f00: 0000 0073 0600 0000 0a01 0e01 04ff 7a0d  ...s..........z.
+00000f10: 4a6f 622e 7465 726d 696e 6174 6563 0100  Job.terminatec..
+00000f20: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000f30: 0000 4300 0001 7362 0000 007c 006a 0072  ..C...sb...|.j.r
+00000f40: 077c 00a0 01a1 0073 0964 0053 0074 027c  .|.....s.d.S.t.|
+00000f50: 006a 0064 0183 0273 1674 03a0 0464 02a1  .j.d...s.t...d..
+00000f60: 0101 0064 0053 007c 006a 00a0 05a1 0001  ...d.S.|.j......
+00000f70: 007c 006a 00a0 06a1 0001 0074 07a0 07a1  .|.j.......t....
+00000f80: 007c 005f 0864 037c 005f 0974 03a0 0a64  .|._.d.|._.t...d
+00000f90: 047c 006a 0ba1 0201 0064 0053 0029 054e  .|.j.....d.S.).N
+00000fa0: 7256 0000 007a 1b55 6e61 626c 6520 746f  rV...z.Unable to
+00000fb0: 2074 6572 6d69 6e61 7465 2074 6872 6561   terminate threa
+00000fc0: 642e 547a 1253 746f 7070 6564 2064 6174  d.Tz.Stopped dat
+00000fd0: 613a 2027 2564 2729 0c72 3900 0000 7250  a: '%d').r9...rP
+00000fe0: 0000 0072 5400 0000 da03 6c6f 6772 3700  ...rT.....logr7.
+00000ff0: 0000 7256 0000 0072 5300 0000 7251 0000  ..rV...rS...rQ..
+00001000: 0072 3300 0000 722f 0000 00da 0564 6562  .r3...r/.....deb
+00001010: 7567 722e 0000 0072 3f00 0000 721a 0000  ugr....r?...r...
+00001020: 0072 1a00 0000 721b 0000 00da 0473 746f  .r....r......sto
+00001030: 7089 0000 0073 1200 0000 0e02 0401 0c01  p....s..........
+00001040: 0e01 0a02 0a01 0a01 0601 1201 7a08 4a6f  ............z.Jo
+00001050: 622e 7374 6f70 6301 0000 0000 0000 0000  b.stopc.........
+00001060: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
+00001070: 1c00 0000 7c00 6a00 7206 7c00 6a01 7308  ....|.j.r.|.j.s.
+00001080: 6401 5300 7c00 6a01 7c00 6a00 1800 5300  d.S.|.j.|.j...S.
+00001090: 2902 61bb 0100 0054 6865 206e 756d 6265  ).a....The numbe
+000010a0: 7220 6f66 2073 6563 6f6e 6473 2061 206a  r of seconds a j
+000010b0: 6f62 2077 6173 2072 756e 6e69 6e67 2066  ob was running f
+000010c0: 6f72 2e0a 0a20 2020 2020 2020 2052 6574  or...        Ret
+000010d0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000010e0: 2020 2e2e 2e0a 0a20 2020 2020 2020 2045    .....        E
+000010f0: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
+00001100: 2020 2020 203e 3e3e 2066 726f 6d20 7070       >>> from pp
+00001110: 7175 6575 6520 696d 706f 7274 2051 7565  queue import Que
+00001120: 7565 0a20 2020 2020 2020 2020 2020 203e  ue.            >
+00001130: 3e3e 2066 726f 6d20 7469 6d65 2069 6d70  >> from time imp
+00001140: 6f72 7420 736c 6565 700a 2020 2020 2020  ort sleep.      
+00001150: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00001160: 2020 2020 2020 3e3e 3e20 7769 7468 2051        >>> with Q
+00001170: 7565 7565 2829 2061 7320 7175 6575 653a  ueue() as queue:
+00001180: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00001190: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+000011a0: 6e67 6528 3529 3a0a 2020 2020 2020 2020  nge(5):.        
+000011b0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+000011c0: 6a6f 6273 203d 2071 7565 7565 2e6d 6170  jobs = queue.map
+000011d0: 2873 6c65 6570 2c20 5b31 2c20 322c 2033  (sleep, [1, 2, 3
+000011e0: 5d29 0a20 2020 2020 2020 2020 2020 202e  ]).            .
+000011f0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
+00001200: 3e3e 205b 696e 7428 6a6f 622e 6765 745f  >> [int(job.get_
+00001210: 7365 636f 6e64 735f 7275 6e6e 696e 6728  seconds_running(
+00001220: 2929 2066 6f72 206a 6f62 2069 6e20 6a6f  )) for job in jo
+00001230: 6273 5d0a 2020 2020 2020 2020 2020 2020  bs].            
+00001240: 5b31 2c20 322c 2033 5d0a 2020 2020 2020  [1, 2, 3].      
+00001250: 2020 4e29 0272 3200 0000 7233 0000 0072    N).r2...r3...r
+00001260: 3f00 0000 721a 0000 0072 1a00 0000 721b  ?...r....r....r.
+00001270: 0000 00da 1367 6574 5f73 6563 6f6e 6473  .....get_seconds
+00001280: 5f72 756e 6e69 6e67 9600 0000 7306 0000  _running....s...
+00001290: 000c 1104 010c 017a 174a 6f62 2e67 6574  .......z.Job.get
+000012a0: 5f73 6563 6f6e 6473 5f72 756e 6e69 6e67  _seconds_running
+000012b0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+000012c0: 0002 0000 0043 0000 01f3 2a00 0000 7c00  .....C....*...|.
+000012d0: 6a00 7305 6401 5300 7c00 6a01 730f 7402  j.s.d.S.|.j.s.t.
+000012e0: a002 a100 7c00 6a00 1800 5300 7c00 6a01  ....|.j...S.|.j.
+000012f0: 7c00 6a00 1800 5300 2902 7ab3 5468 6520  |.j...S.).z.The 
+00001300: 616d 6f75 6e74 206f 6620 7469 6d65 2061  amount of time a
+00001310: 2064 6174 6120 6861 7320 7370 656e 7420   data has spent 
+00001320: 696e 2074 6865 2077 6169 7469 6e67 2071  in the waiting q
+00001330: 7565 7565 2e0a 0a20 2020 2020 2020 2052  ueue...        R
+00001340: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00001350: 2020 2020 2e2e 2e0a 0a20 2020 2020 2020      .....       
+00001360: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+00001370: 2020 2020 2020 203e 3e3e 206a 6f62 2e67         >>> job.g
+00001380: 6574 5f73 6563 6f6e 6473 5f77 6169 7469  et_seconds_waiti
+00001390: 6e67 2829 2020 2320 646f 6374 6573 743a  ng()  # doctest:
+000013a0: 202b 534b 4950 0a20 2020 2020 2020 204e   +SKIP.        N
+000013b0: 2903 7231 0000 0072 3200 0000 7251 0000  ).r1...r2...rQ..
+000013c0: 0072 3f00 0000 721a 0000 0072 1a00 0000  .r?...r....r....
+000013d0: 721b 0000 00da 1367 6574 5f73 6563 6f6e  r......get_secon
+000013e0: 6473 5f77 6169 7469 6e67 ab00 0000 f30a  ds_waiting......
+000013f0: 0000 0006 0904 0106 020e 010c 027a 174a  .............z.J
+00001400: 6f62 2e67 6574 5f73 6563 6f6e 6473 5f77  ob.get_seconds_w
+00001410: 6169 7469 6e67 6301 0000 0000 0000 0000  aitingc.........
+00001420: 0000 0001 0000 0002 0000 0043 0000 0172  ...........C...r
+00001430: 5b00 0000 2902 7aab 5265 7475 726e 7320  [...).z.Returns 
+00001440: 7468 6520 7761 6974 696e 6720 2b20 7275  the waiting + ru
+00001450: 6e6e 696e 6720 6475 7261 7469 6f6e 206f  nning duration o
+00001460: 6620 7468 6973 206a 6f62 2e0a 0a20 2020  f this job...   
+00001470: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00001480: 2020 2020 2020 2020 2020 2e2e 2e0a 0a20            ..... 
+00001490: 2020 2020 2020 2045 7861 6d70 6c65 733a         Examples:
+000014a0: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+000014b0: 206a 6f62 2e67 6574 5f73 6563 6f6e 6473   job.get_seconds
+000014c0: 5f74 6f74 616c 2829 2020 2320 646f 6374  _total()  # doct
+000014d0: 6573 743a 202b 534b 4950 0a20 2020 2020  est: +SKIP.     
+000014e0: 2020 204e 2903 7231 0000 0072 3300 0000     N).r1...r3...
+000014f0: 7251 0000 0072 3f00 0000 721a 0000 0072  rQ...r?...r....r
+00001500: 1a00 0000 721b 0000 00da 1167 6574 5f73  ....r......get_s
+00001510: 6563 6f6e 6473 5f74 6f74 616c bc00 0000  econds_total....
+00001520: 725d 0000 007a 154a 6f62 2e67 6574 5f73  r]...z.Job.get_s
+00001530: 6563 6f6e 6473 5f74 6f74 616c fa0f 6461  econds_total..da
+00001540: 7465 7469 6d65 207c 204e 6f6e 6563 0100  tetime | Nonec..
+00001550: 0000 0000 0000 0000 0000 0100 0000 0300  ................
+00001560: 0000 4300 0001 f316 0000 007c 006a 0072  ..C........|.j.r
+00001570: 0974 01a0 027c 006a 00a1 0153 0064 0153  .t...|.j...S.d.S
+00001580: 0029 027a 9b54 6865 2074 696d 6520 7468  .).z.The time th
+00001590: 6973 206a 6f62 2077 6173 2073 7562 6d69  is job was submi
+000015a0: 7474 6564 2e0a 0a20 2020 2020 2020 2052  tted...        R
+000015b0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+000015c0: 2020 2020 2e2e 2e0a 0a20 2020 2020 2020      .....       
+000015d0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+000015e0: 2020 2020 2020 203e 3e3e 206a 6f62 2e67         >>> job.g
+000015f0: 6574 5f73 7562 6d69 745f 7469 6d65 7374  et_submit_timest
+00001600: 616d 7028 2920 2023 2064 6f63 7465 7374  amp()  # doctest
+00001610: 3a20 2b53 4b49 500a 2020 2020 2020 2020  : +SKIP.        
+00001620: 4e29 0372 3100 0000 7206 0000 00da 1075  N).r1...r......u
+00001630: 7463 6672 6f6d 7469 6d65 7374 616d 7072  tcfromtimestampr
+00001640: 3f00 0000 721a 0000 0072 1a00 0000 721b  ?...r....r....r.
+00001650: 0000 00da 1467 6574 5f73 7562 6d69 745f  .....get_submit_
+00001660: 7469 6d65 7374 616d 70cd 0000 0073 0600  timestamp....s..
+00001670: 0000 0609 0c01 0401 7a18 4a6f 622e 6765  ........z.Job.ge
+00001680: 745f 7375 626d 6974 5f74 696d 6573 7461  t_submit_timesta
+00001690: 6d70 6301 0000 0000 0000 0000 0000 0001  mpc.............
+000016a0: 0000 0003 0000 0043 0000 0172 6000 0000  .......C...r`...
+000016b0: 2902 7a67 5265 7475 726e 7320 6120 6461  ).zgReturns a da
+000016c0: 7465 7469 6d65 206f 626a 6563 7420 6f66  tetime object of
+000016d0: 2074 6865 2074 696d 6520 7468 6973 2064   the time this d
+000016e0: 6174 6120 7761 7320 7374 6172 7465 642e  ata was started.
+000016f0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+00001700: 733a 0a20 2020 2020 2020 2020 2020 202e  s:.            .
+00001710: 2e2e 0a20 2020 2020 2020 204e 2903 7232  ...        N).r2
+00001720: 0000 0072 0600 0000 7261 0000 0072 3f00  ...r....ra...r?.
+00001730: 0000 721a 0000 0072 1a00 0000 721b 0000  ..r....r....r...
+00001740: 00da 1367 6574 5f73 7461 7274 5f74 696d  ...get_start_tim
+00001750: 6573 7461 6d70 da00 0000 f306 0000 0006  estamp..........
+00001760: 060c 0104 017a 174a 6f62 2e67 6574 5f73  .....z.Job.get_s
+00001770: 7461 7274 5f74 696d 6573 7461 6d70 6301  tart_timestampc.
+00001780: 0000 0000 0000 0000 0000 0001 0000 0003  ................
+00001790: 0000 0043 0000 0172 6000 0000 2902 7a64  ...C...r`...).zd
+000017a0: 5265 7475 726e 7320 6120 6461 7465 7469  Returns a dateti
+000017b0: 6d65 206f 626a 6563 7420 6f66 2074 6865  me object of the
+000017c0: 2074 696d 6520 7468 6973 2064 6174 6120   time this data 
+000017d0: 6669 6e69 7368 6564 2e0a 0a20 2020 2020  finished...     
+000017e0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+000017f0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00001800: 2020 2020 4e29 0372 3300 0000 7206 0000      N).r3...r...
+00001810: 0072 6100 0000 723f 0000 0072 1a00 0000  .ra...r?...r....
+00001820: 721a 0000 0072 1b00 0000 da14 6765 745f  r....r......get_
+00001830: 6669 6e69 7368 5f74 696d 6573 7461 6d70  finish_timestamp
+00001840: e400 0000 7264 0000 007a 184a 6f62 2e67  ....rd...z.Job.g
+00001850: 6574 5f66 696e 6973 685f 7469 6d65 7374  et_finish_timest
+00001860: 616d 7063 0100 0000 0000 0000 0000 0000  ampc............
+00001870: 0100 0000 0300 0000 4300 0001 7260 0000  ........C...r`..
+00001880: 0029 027a 6952 6574 7572 6e73 2061 2064  .).ziReturns a d
+00001890: 6174 6574 696d 6520 6f62 6a65 6374 206f  atetime object o
+000018a0: 6620 7468 6520 7469 6d65 2074 6869 7320  f the time this 
+000018b0: 6461 7461 2077 6173 2070 726f 6365 7373  data was process
+000018c0: 6564 2e0a 0a20 2020 2020 2020 2052 6574  ed...        Ret
+000018d0: 7572 6e73 3a0a 2020 2020 2020 2020 2020  urns:.          
+000018e0: 2020 2e2e 2e0a 2020 2020 2020 2020 4e29    ....        N)
+000018f0: 0372 3400 0000 7206 0000 0072 6100 0000  .r4...r....ra...
+00001900: 723f 0000 0072 1a00 0000 721a 0000 0072  r?...r....r....r
+00001910: 1b00 0000 da17 6765 745f 7072 6f63 6573  ......get_proces
+00001920: 7365 645f 7469 6d65 7374 616d 70ee 0000  sed_timestamp...
+00001930: 0072 6400 0000 7a1b 4a6f 622e 6765 745f  .rd...z.Job.get_
+00001940: 7072 6f63 6573 7365 645f 7469 6d65 7374  processed_timest
+00001950: 616d 7063 0100 0000 0000 0000 0000 0000  ampc............
+00001960: 0100 0000 0200 0000 4300 0001 730a 0000  ........C...s...
+00001970: 007c 006a 0064 0075 0153 0072 3c00 0000  .|.j.d.u.S.r<...
+00001980: 2901 7234 0000 0072 3f00 0000 721a 0000  ).r4...r?...r...
+00001990: 0072 1a00 0000 721b 0000 00da 0c69 735f  .r....r......is_
+000019a0: 7072 6f63 6573 7365 64f8 0000 0073 0200  processed....s..
+000019b0: 0000 0a05 7a10 4a6f 622e 6973 5f70 726f  ....z.Job.is_pro
+000019c0: 6365 7373 6564 7211 0000 0063 0100 0000  cessedr....c....
+000019d0: 0000 0000 0000 0000 0100 0000 0200 0000  ................
+000019e0: 4300 0001 7338 0000 007c 006a 0073 0674  C...s8...|.j.s.t
+000019f0: 016a 0253 007c 00a0 03a1 0072 0d74 016a  .j.S.|.....r.t.j
+00001a00: 0453 007c 006a 0572 1374 016a 0653 007c  .S.|.j.r.t.j.S.|
+00001a10: 006a 0772 1974 016a 0853 0074 016a 0953  .j.r.t.j.S.t.j.S
+00001a20: 0072 3c00 0000 290a 7231 0000 0072 1100  .r<...).r1...r..
+00001a30: 0000 7215 0000 0072 5000 0000 7216 0000  ..r....rP...r...
+00001a40: 0072 2f00 0000 7217 0000 0072 3300 0000  .r/...r....r3...
+00001a50: 7218 0000 0072 1900 0000 723f 0000 0072  r....r....r?...r
+00001a60: 1a00 0000 721a 0000 0072 1b00 0000 da09  ....r....r......
+00001a70: 6765 745f 7374 6174 65ff 0000 0073 1200  get_state....s..
+00001a80: 0000 0601 0601 0801 0601 0601 0601 0601  ................
+00001a90: 0601 0601 7a0d 4a6f 622e 6765 745f 7374  ....z.Job.get_st
+00001aa0: 6174 6529 0272 3a00 0000 723b 0000 0029  ate).r:...r;...)
+00001ab0: 0472 4200 0000 721c 0000 0072 3a00 0000  .rB...r....r:...
+00001ac0: 7222 0000 0029 0472 4200 0000 7245 0000  r"...).rB...rE..
+00001ad0: 0072 3a00 0000 7228 0000 0029 0272 3a00  .r:...r(...).r:.
+00001ae0: 0000 7228 0000 0029 0272 3a00 0000 7224  ..r(...).r:...r$
+00001af0: 0000 0029 0272 3a00 0000 7230 0000 0029  ...).r:...r0...)
+00001b00: 0272 3a00 0000 725f 0000 0029 0272 3a00  .r:...r_...).r:.
+00001b10: 0000 7211 0000 0029 3372 1200 0000 7213  ..r....)3r....r.
+00001b20: 0000 0072 1400 0000 da07 5f5f 646f 635f  ...r......__doc_
+00001b30: 5fda 0f5f 5f61 6e6e 6f74 6174 696f 6e73  _..__annotations
+00001b40: 5f5f 7205 0000 00da 046c 6973 7472 1e00  __r......listr..
+00001b50: 0000 da04 6469 6374 721f 0000 0072 2000  ....dictr....r .
+00001b60: 0000 7223 0000 0072 2500 0000 7227 0000  ..r#...r%...r'..
+00001b70: 0072 2900 0000 722a 0000 0072 2d00 0000  .r)...r*...r-...
+00001b80: 722e 0000 0072 2f00 0000 7231 0000 0072  r....r/...r1...r
+00001b90: 3200 0000 7233 0000 0072 3400 0000 7235  2...r3...r4...r5
+00001ba0: 0000 0072 3600 0000 7237 0000 0072 3800  ...r6...r7...r8.
+00001bb0: 0000 7239 0000 0072 4100 0000 7244 0000  ..r9...rA...rD..
+00001bc0: 0072 4800 0000 724a 0000 0072 4b00 0000  .rH...rJ...rK...
+00001bd0: 724c 0000 0072 4d00 0000 724e 0000 0072  rL...rM...rN...r
+00001be0: 5000 0000 7252 0000 0072 5300 0000 7255  P...rR...rS...rU
+00001bf0: 0000 0072 5600 0000 7259 0000 0072 5a00  ...rV...rY...rZ.
+00001c00: 0000 725c 0000 0072 5e00 0000 7262 0000  ..r\...r^...rb..
+00001c10: 0072 6300 0000 7265 0000 0072 6600 0000  .rc...re...rf...
+00001c20: 7267 0000 0072 6800 0000 721a 0000 0072  rg...rh...r....r
+00001c30: 1a00 0000 721a 0000 0072 1b00 0000 721c  ....r....r....r.
+00001c40: 0000 0019 0000 0073 7000 0000 0a00 0402  .......sp.......
+00001c50: 0802 1201 1201 0c01 0c01 0c01 0c01 0c01  ................
+00001c60: 0c01 1402 0201 1401 0201 1401 0201 1401  ................
+00001c70: 0201 1401 0201 1401 0201 1401 0201 1401  ................
+00001c80: 0201 1401 0201 1401 0201 1401 1401 0a02  ................
+00001c90: 0a09 0a0d 0a03 0a03 0a03 0a03 0a03 0a03  ................
+00001ca0: 0a03 0a09 0a05 0a0e 0a04 0a0d 0a15 0a11  ................
+00001cb0: 0a11 0a0d 0a0a 0a0a 0a0a 0e07 721c 0000  ............r...
+00001cc0: 0029 1bda 0a5f 5f66 7574 7572 655f 5f72  .)...__future__r
+00001cd0: 0200 0000 da07 6c6f 6767 696e 6772 5700  ......loggingrW.
+00001ce0: 0000 7251 0000 00da 0f63 6f6c 6c65 6374  ..rQ.....collect
+00001cf0: 696f 6e73 2e61 6263 7203 0000 00da 0b64  ions.abcr......d
+00001d00: 6174 6163 6c61 7373 6573 7204 0000 0072  ataclassesr....r
+00001d10: 0500 0000 7206 0000 00da 0465 6e75 6d72  ....r......enumr
+00001d20: 0700 0000 7208 0000 00da 0f6d 756c 7469  ....r......multi
+00001d30: 7072 6f63 6573 7369 6e67 7209 0000 00da  processingr.....
+00001d40: 0974 6872 6561 6469 6e67 720a 0000 00da  .threadingr.....
+00001d50: 0674 7970 696e 6772 0b00 0000 720c 0000  .typingr....r...
+00001d60: 0072 0d00 0000 da05 7574 696c 7372 1000  .r......utilsr..
+00001d70: 0000 7211 0000 0072 4500 0000 721c 0000  ..r....rE...r...
+00001d80: 0072 1a00 0000 721a 0000 0072 1a00 0000  .r....r....r....
+00001d90: 721b 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00001da0: 0000 0073 1c00 0000 0c00 0802 0801 0c01  ...s............
+00001db0: 1001 0c01 1001 0c01 0c01 1401 0c02 1003  ................
+00001dc0: 0209 1601                                ....
```

### Comparing `ppqueue-0.3.0/src/ppqueue/__pycache__/plot.cpython-310.pyc` & `ppqueue-0.4.0/src/ppqueue/__pycache__/plot.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 22 04:39:29 2023 UTC, .py size: 7524 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 81d0 9364 641d 0000  o..........dd...
+00000000: 6f0d 0d0a 0000 0000 a375 cd64 cf1d 0000  o........u.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0009 0000 0040 0000 0173 dc00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a03 6400 6403 6c04 6d05 5a05 6d06 5a06  Z.d.d.l.m.Z.m.Z.
 00000050: 0100 6400 6402 6c07 5a08 6400 6402 6c09  ..d.d.l.Z.d.d.l.
 00000060: 5a0a 6404 6405 6c0b 6d0c 5a0c 0100 6404  Z.d.d.l.m.Z...d.
 00000070: 6406 6c0d 6d0e 5a0e 0100 6700 6407 a201  d.l.m.Z...g.d...
@@ -305,98 +305,105 @@
 00001300: 5000 0000 7251 0000 0072 3b00 0000 7252  P...rQ...r;...rR
 00001310: 0000 0072 5300 0000 7254 0000 0072 5500  ...rS...rT...rU.
 00001320: 0000 7256 0000 0072 5700 0000 723f 0000  ..rV...rW...r?..
 00001330: 0072 5800 0000 6300 0000 0000 0000 0008  .rX...c.........
 00001340: 0000 0009 0000 000a 0000 0047 0000 0173  ...........G...s
 00001350: 1e00 0000 7400 7c08 8e00 6a01 7c01 7c02  ....t.|...j.|.|.
 00001360: 7c03 7c05 7c06 7c00 7c07 7c04 6401 8d08  |.|.|.|.|.|.d...
-00001370: 5300 2902 61a9 0300 000a 0a20 2020 2041  S.).a......    A
-00001380: 7267 733a 0a20 2020 2020 2020 2074 6974  rgs:.        tit
-00001390: 6c65 3a0a 2020 2020 2020 2020 636f 6c6f  le:.        colo
-000013a0: 725f 6279 3a0a 2020 2020 2020 2020 6661  r_by:.        fa
-000013b0: 6365 745f 6279 3a0a 2020 2020 2020 2020  cet_by:.        
-000013c0: 6661 6365 745f 7363 616c 653a 0a20 2020  facet_scale:.   
-000013d0: 2020 2020 2074 6865 6d65 3a0a 2020 2020       theme:.    
-000013e0: 2020 2020 6e6f 5f6c 6567 656e 643a 0a20      no_legend:. 
-000013f0: 2020 2020 2020 2062 6172 5f77 6964 7468         bar_width
-00001400: 3a0a 2020 2020 2020 2020 636f 6c6f 725f  :.        color_
-00001410: 7061 6c3a 2061 2073 6571 7565 6e63 6520  pal: a sequence 
-00001420: 6f66 2063 6f6c 6f72 7320 7573 6564 2074  of colors used t
-00001430: 6f20 636f 6c6f 7220 6561 6368 2067 726f  o color each gro
-00001440: 7570 206f 6620 6063 6f6c 6f72 5f62 7960  up of `color_by`
-00001450: 2e0a 0a20 2020 2045 7861 6d70 6c65 733a  ...    Examples:
-00001460: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
-00001470: 6d20 7070 7175 6575 6520 696d 706f 7274  m ppqueue import
-00001480: 2051 7565 7565 0a20 2020 2020 2020 203e   Queue.        >
-00001490: 3e3e 2066 726f 6d20 7070 7175 6575 652e  >> from ppqueue.
-000014a0: 706c 6f74 2069 6d70 6f72 7420 706c 6f74  plot import plot
-000014b0: 5f6a 6f62 730a 2020 2020 2020 2020 3e3e  _jobs.        >>
-000014c0: 3e20 6672 6f6d 2074 696d 6520 696d 706f  > from time impo
-000014d0: 7274 2073 6c65 6570 0a20 2020 2020 2020  rt sleep.       
-000014e0: 202e 2e2e 0a20 2020 2020 2020 203e 3e3e   ....        >>>
-000014f0: 2077 6974 6820 5175 6575 6528 2920 6173   with Queue() as
-00001500: 2071 7565 7565 3a0a 2020 2020 2020 2020   queue:.        
-00001510: 2e2e 2e20 2020 2020 7131 5f6a 6f62 7320  ...     q1_jobs 
-00001520: 3d20 7175 6575 652e 6d61 7028 736c 6565  = queue.map(slee
-00001530: 702c 205b 312c 2032 2c20 332c 2034 2c20  p, [1, 2, 3, 4, 
-00001540: 355d 290a 2020 2020 2020 2020 2e2e 2e0a  5]).        ....
+00001370: 5300 2902 6114 0400 000a 0a20 2020 2041  S.).a......    A
+00001380: 7267 733a 0a20 2020 2020 2020 202a 6172  rgs:.        *ar
+00001390: 6773 3a20 5365 7175 656e 6365 7320 6f66  gs: Sequences of
+000013a0: 2060 4a6f 6260 2069 6e73 7461 6e63 6573   `Job` instances
+000013b0: 2074 6f20 706c 6f74 2e0a 2020 2020 2020   to plot..      
+000013c0: 2020 7469 746c 653a 202e 2e2e 0a20 2020    title: ....   
+000013d0: 2020 2020 2063 6f6c 6f72 5f62 793a 202e       color_by: .
+000013e0: 2e2e 0a20 2020 2020 2020 2066 6163 6574  ...        facet
+000013f0: 5f62 793a 202e 2e2e 0a20 2020 2020 2020  _by: ....       
+00001400: 2066 6163 6574 5f73 6361 6c65 3a20 2e2e   facet_scale: ..
+00001410: 2e0a 2020 2020 2020 2020 7468 656d 653a  ..        theme:
+00001420: 202e 2e2e 0a20 2020 2020 2020 206e 6f5f   ....        no_
+00001430: 6c65 6765 6e64 3a20 2e2e 2e0a 2020 2020  legend: ....    
+00001440: 2020 2020 6261 725f 7769 6474 683a 202e      bar_width: .
+00001450: 2e2e 0a20 2020 2020 2020 2063 6f6c 6f72  ...        color
+00001460: 5f70 616c 3a20 6120 7365 7175 656e 6365  _pal: a sequence
+00001470: 206f 6620 636f 6c6f 7273 2075 7365 6420   of colors used 
+00001480: 746f 2063 6f6c 6f72 2065 6163 6820 6772  to color each gr
+00001490: 6f75 7020 6f66 2060 636f 6c6f 725f 6279  oup of `color_by
+000014a0: 602e 0a0a 2020 2020 5265 7475 726e 733a  `...    Returns:
+000014b0: 0a20 2020 2020 2020 202e 2e2e 0a0a 2020  .        .....  
+000014c0: 2020 4578 616d 706c 6573 3a0a 2020 2020    Examples:.    
+000014d0: 2020 2020 3e3e 3e20 6672 6f6d 2070 7071      >>> from ppq
+000014e0: 7565 7565 2069 6d70 6f72 7420 5175 6575  ueue import Queu
+000014f0: 650a 2020 2020 2020 2020 3e3e 3e20 6672  e.        >>> fr
+00001500: 6f6d 2070 7071 7565 7565 2e70 6c6f 7420  om ppqueue.plot 
+00001510: 696d 706f 7274 2070 6c6f 745f 6a6f 6273  import plot_jobs
+00001520: 0a20 2020 2020 2020 203e 3e3e 2066 726f  .        >>> fro
+00001530: 6d20 7469 6d65 2069 6d70 6f72 7420 736c  m time import sl
+00001540: 6565 700a 2020 2020 2020 2020 2e2e 2e0a  eep.        ....
 00001550: 2020 2020 2020 2020 3e3e 3e20 7769 7468          >>> with
 00001560: 2051 7565 7565 2829 2061 7320 7175 6575   Queue() as queu
 00001570: 653a 0a20 2020 2020 2020 202e 2e2e 2020  e:.        ...  
-00001580: 2020 2071 325f 6a6f 6273 203d 2071 7565     q2_jobs = que
+00001580: 2020 2071 315f 6a6f 6273 203d 2071 7565     q1_jobs = que
 00001590: 7565 2e6d 6170 2873 6c65 6570 2c20 5b31  ue.map(sleep, [1
 000015a0: 2c20 322c 2033 2c20 342c 2035 5d29 0a20  , 2, 3, 4, 5]). 
 000015b0: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
-000015c0: 2020 203e 3e3e 2070 6c6f 7420 3d20 706c     >>> plot = pl
-000015d0: 6f74 5f6a 6f62 7328 0a20 2020 2020 2020  ot_jobs(.       
-000015e0: 202e 2e2e 2020 2020 2071 315f 6a6f 6273   ...     q1_jobs
-000015f0: 2c20 7132 5f6a 6f62 732c 0a20 2020 2020  , q2_jobs,.     
-00001600: 2020 202e 2e2e 2020 2020 2074 6974 6c65     ...     title
-00001610: 3d27 4465 6d6f 272c 0a20 2020 2020 2020  ='Demo',.       
-00001620: 202e 2e2e 2020 2020 2063 6f6c 6f72 5f62   ...     color_b
-00001630: 793d 506c 6f74 436f 6c6f 7242 792e 5149  y=PlotColorBy.QI
-00001640: 442c 0a20 2020 2020 2020 202e 2e2e 2020  D,.        ...  
-00001650: 2020 2066 6163 6574 5f62 793d 506c 6f74     facet_by=Plot
-00001660: 4661 6365 7442 792e 5149 442c 0a20 2020  FacetBy.QID,.   
-00001670: 2020 2020 202e 2e2e 2020 2020 2074 6865       ...     the
-00001680: 6d65 3d50 6c6f 7454 6865 6d65 2e44 4152  me=PlotTheme.DAR
-00001690: 4b2c 0a20 2020 2020 2020 202e 2e2e 2020  K,.        ...  
-000016a0: 2020 2062 6172 5f77 6964 7468 3d32 2c0a     bar_width=2,.
-000016b0: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-000016c0: 636f 6c6f 725f 7061 6c3d 5b27 7265 6427  color_pal=['red'
-000016d0: 2c20 2762 6c75 6527 5d0a 2020 2020 2020  , 'blue'].      
-000016e0: 2020 2e2e 2e20 290a 2020 2020 2020 2020    ... ).        
-000016f0: 2e2e 2e0a 2020 2020 2020 2020 3e3e 3e20  ....        >>> 
-00001700: 7072 696e 7428 706c 6f74 2920 2023 2064  print(plot)  # d
-00001710: 6f63 7465 7374 3a20 2b53 4b49 500a 2020  octest: +SKIP.  
-00001720: 2020 2908 724f 0000 0072 5000 0000 7251    ).rO...rP...rQ
-00001730: 0000 0072 5200 0000 7254 0000 0072 4e00  ...rR...rT...rN.
-00001740: 0000 7256 0000 0072 3b00 0000 2902 7222  ..rV...r;...).r"
-00001750: 0000 0072 6800 0000 2909 724e 0000 0072  ...rh...).rN...r
-00001760: 4f00 0000 7250 0000 0072 5100 0000 723b  O...rP...rQ...r;
-00001770: 0000 0072 5200 0000 7254 0000 0072 5600  ...rR...rT...rV.
-00001780: 0000 7223 0000 0072 1700 0000 7217 0000  ..r#...r....r...
-00001790: 0072 1800 0000 7208 0000 00d3 0000 0073  .r....r........s
-000017a0: 1400 0000 082f 0201 0201 0201 0201 0201  ...../..........
-000017b0: 0201 0201 0201 06f8 7208 0000 0029 1472  ........r....).r
-000017c0: 2300 0000 7224 0000 0072 4e00 0000 723e  #...r$...rN...r>
-000017d0: 0000 0072 4f00 0000 7209 0000 0072 5000  ...rO...r....rP.
-000017e0: 0000 720a 0000 0072 5100 0000 720b 0000  ..r....rQ...r...
-000017f0: 0072 3b00 0000 720d 0000 0072 5200 0000  .r;...r....rR...
-00001800: 7253 0000 0072 5400 0000 7255 0000 0072  rS...rT...rU...r
-00001810: 5600 0000 7257 0000 0072 3f00 0000 7258  V...rW...r?...rX
-00001820: 0000 0029 1ada 0a5f 5f66 7574 7572 655f  ...)...__future_
-00001830: 5f72 0200 0000 da07 6c6f 6767 696e 6772  _r......loggingr
-00001840: 6600 0000 da04 656e 756d 7203 0000 0072  f.....enumr....r
-00001850: 0400 0000 da06 7061 6e64 6173 7233 0000  ......pandasr3..
-00001860: 005a 0870 6c6f 746e 696e 6572 4900 0000  .Z.plotninerI...
-00001870: da03 6a6f 6272 0600 0000 da05 7574 696c  ..jobr......util
-00001880: 7372 0700 0000 da07 5f5f 616c 6c5f 5f72  sr......__all__r
-00001890: 0900 0000 720a 0000 0072 0d00 0000 720b  ....r....r....r.
-000018a0: 0000 0072 0c00 0000 7222 0000 0072 1400  ...r....r"...r..
-000018b0: 0000 721c 0000 0072 1a00 0000 7208 0000  ..r....r....r...
-000018c0: 0072 1700 0000 7217 0000 0072 1700 0000  .r....r....r....
-000018d0: 7218 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
-000018e0: 0000 0073 3000 0000 0c00 0802 1001 0802  ...s0...........
-000018f0: 0801 0c02 0c01 0802 100a 100d 100d 100f  ................
-00001900: 1007 0e07 007f 0209 0401 0401 0401 0401  ................
-00001910: 0201 0201 0201 12f7                      ........
+000015c0: 2020 203e 3e3e 2077 6974 6820 5175 6575     >>> with Queu
+000015d0: 6528 2920 6173 2071 7565 7565 3a0a 2020  e() as queue:.  
+000015e0: 2020 2020 2020 2e2e 2e20 2020 2020 7132        ...     q2
+000015f0: 5f6a 6f62 7320 3d20 7175 6575 652e 6d61  _jobs = queue.ma
+00001600: 7028 736c 6565 702c 205b 312c 2032 2c20  p(sleep, [1, 2, 
+00001610: 332c 2034 2c20 355d 290a 2020 2020 2020  3, 4, 5]).      
+00001620: 2020 2e2e 2e0a 2020 2020 2020 2020 3e3e    ....        >>
+00001630: 3e20 706c 6f74 203d 2070 6c6f 745f 6a6f  > plot = plot_jo
+00001640: 6273 280a 2020 2020 2020 2020 2e2e 2e20  bs(.        ... 
+00001650: 2020 2020 7131 5f6a 6f62 732c 2071 325f      q1_jobs, q2_
+00001660: 6a6f 6273 2c0a 2020 2020 2020 2020 2e2e  jobs,.        ..
+00001670: 2e20 2020 2020 7469 746c 653d 2744 656d  .     title='Dem
+00001680: 6f27 2c0a 2020 2020 2020 2020 2e2e 2e20  o',.        ... 
+00001690: 2020 2020 636f 6c6f 725f 6279 3d50 6c6f      color_by=Plo
+000016a0: 7443 6f6c 6f72 4279 2e51 4944 2c0a 2020  tColorBy.QID,.  
+000016b0: 2020 2020 2020 2e2e 2e20 2020 2020 6661        ...     fa
+000016c0: 6365 745f 6279 3d50 6c6f 7446 6163 6574  cet_by=PlotFacet
+000016d0: 4279 2e51 4944 2c0a 2020 2020 2020 2020  By.QID,.        
+000016e0: 2e2e 2e20 2020 2020 7468 656d 653d 506c  ...     theme=Pl
+000016f0: 6f74 5468 656d 652e 4441 524b 2c0a 2020  otTheme.DARK,.  
+00001700: 2020 2020 2020 2e2e 2e20 2020 2020 6261        ...     ba
+00001710: 725f 7769 6474 683d 322c 0a20 2020 2020  r_width=2,.     
+00001720: 2020 202e 2e2e 2020 2020 2063 6f6c 6f72     ...     color
+00001730: 5f70 616c 3d5b 2772 6564 272c 2027 626c  _pal=['red', 'bl
+00001740: 7565 275d 0a20 2020 2020 2020 202e 2e2e  ue'].        ...
+00001750: 2029 0a20 2020 2020 2020 202e 2e2e 0a20   ).        .... 
+00001760: 2020 2020 2020 203e 3e3e 2070 7269 6e74         >>> print
+00001770: 2870 6c6f 7429 2020 2320 646f 6374 6573  (plot)  # doctes
+00001780: 743a 202b 534b 4950 0a20 2020 2029 0872  t: +SKIP.    ).r
+00001790: 4f00 0000 7250 0000 0072 5100 0000 7252  O...rP...rQ...rR
+000017a0: 0000 0072 5400 0000 724e 0000 0072 5600  ...rT...rN...rV.
+000017b0: 0000 723b 0000 0029 0272 2200 0000 7268  ..r;...).r"...rh
+000017c0: 0000 0029 0972 4e00 0000 724f 0000 0072  ...).rN...rO...r
+000017d0: 5000 0000 7251 0000 0072 3b00 0000 7252  P...rQ...r;...rR
+000017e0: 0000 0072 5400 0000 7256 0000 0072 2300  ...rT...rV...r#.
+000017f0: 0000 7217 0000 0072 1700 0000 7218 0000  ..r....r....r...
+00001800: 0072 0800 0000 d300 0000 7314 0000 0008  .r........s.....
+00001810: 3302 0102 0102 0102 0102 0102 0102 0102  3...............
+00001820: 0106 f872 0800 0000 2914 7223 0000 0072  ...r....).r#...r
+00001830: 2400 0000 724e 0000 0072 3e00 0000 724f  $...rN...r>...rO
+00001840: 0000 0072 0900 0000 7250 0000 0072 0a00  ...r....rP...r..
+00001850: 0000 7251 0000 0072 0b00 0000 723b 0000  ..rQ...r....r;..
+00001860: 0072 0d00 0000 7252 0000 0072 5300 0000  .r....rR...rS...
+00001870: 7254 0000 0072 5500 0000 7256 0000 0072  rT...rU...rV...r
+00001880: 5700 0000 723f 0000 0072 5800 0000 291a  W...r?...rX...).
+00001890: da0a 5f5f 6675 7475 7265 5f5f 7202 0000  ..__future__r...
+000018a0: 00da 076c 6f67 6769 6e67 7266 0000 00da  ...loggingrf....
+000018b0: 0465 6e75 6d72 0300 0000 7204 0000 00da  .enumr....r.....
+000018c0: 0670 616e 6461 7372 3300 0000 5a08 706c  .pandasr3...Z.pl
+000018d0: 6f74 6e69 6e65 7249 0000 00da 036a 6f62  otninerI.....job
+000018e0: 7206 0000 00da 0575 7469 6c73 7207 0000  r......utilsr...
+000018f0: 00da 075f 5f61 6c6c 5f5f 7209 0000 0072  ...__all__r....r
+00001900: 0a00 0000 720d 0000 0072 0b00 0000 720c  ....r....r....r.
+00001910: 0000 0072 2200 0000 7214 0000 0072 1c00  ...r"...r....r..
+00001920: 0000 721a 0000 0072 0800 0000 7217 0000  ..r....r....r...
+00001930: 0072 1700 0000 7217 0000 0072 1800 0000  .r....r....r....
+00001940: da08 3c6d 6f64 756c 653e 0100 0000 7330  ..<module>....s0
+00001950: 0000 000c 0008 0210 0108 0208 010c 020c  ................
+00001960: 0108 0210 0a10 0d10 0d10 0f10 070e 0700  ................
+00001970: 7f02 0904 0104 0104 0104 0102 0102 0102  ................
+00001980: 0112 f7                                  ...
```

### Comparing `ppqueue-0.3.0/src/ppqueue/__pycache__/queue.cpython-310.pyc` & `ppqueue-0.4.0/src/ppqueue/__pycache__/queue.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 22 04:39:29 2023 UTC, .py size: 32299 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 18% similar despite different names*

```diff
@@ -1,1653 +1,1725 @@
-00000000: 6f0d 0d0a 0000 0000 81d0 9364 2b7e 0000  o..........d+~..
+00000000: 6f0d 0d0a 0000 0000 a375 cd64 5a84 0000  o........u.dZ...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0173 be00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0173 ba00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a04 6400 6402 6c05  Z.d.d.l.Z.d.d.l.
 00000050: 5a05 6400 6402 6c06 5a06 6400 6402 6c07  Z.d.d.l.Z.d.d.l.
 00000060: 5a07 6400 6403 6c08 6d09 5a09 6d0a 5a0a  Z.d.d.l.m.Z.m.Z.
 00000070: 0100 6400 6404 6c0b 6d0c 5a0c 6d0d 5a0d  ..d.d.l.m.Z.m.Z.
-00000080: 6d0e 5a0e 6d0f 5a0f 0100 6400 6405 6c10  m.Z.m.Z...d.d.l.
-00000090: 6d11 5a11 0100 6400 6406 6c12 6d13 5a13  m.Z...d.d.l.m.Z.
-000000a0: 0100 6407 6408 6c14 6d15 5a15 0100 6407  ..d.d.l.m.Z...d.
-000000b0: 6409 6c16 6d17 5a17 6d18 5a18 0100 6517  d.l.m.Z.m.Z...e.
-000000c0: 6519 6502 6a1a 640a 8d02 5a1b 4700 640b  e.e.j.d...Z.G.d.
-000000d0: 640c 8400 640c 8302 5a1c 4700 640d 640e  d...d...Z.G.d.d.
-000000e0: 8400 640e 8302 5a1d 6402 5300 290f e900  ..d...Z.d.S.)...
-000000f0: 0000 0029 01da 0b61 6e6e 6f74 6174 696f  ...)...annotatio
-00000100: 6e73 4e29 02da 0768 6561 7070 6f70 da08  nsN)...heappop..
-00000110: 6865 6170 7075 7368 2904 da03 416e 79da  heappush)...Any.
-00000120: 0843 616c 6c61 626c 65da 0853 6571 7565  .Callable..Seque
-00000130: 6e63 65da 0454 7970 6529 01da 0575 7569  nce..Type)...uui
-00000140: 6434 2901 da04 7471 646d e901 0000 0029  d4)...tqdm.....)
-00000150: 01da 034a 6f62 2902 da0a 6765 745f 6c6f  ...Job)...get_lo
-00000160: 6767 6572 da0d 6973 5f77 696e 646f 7773  gger..is_windows
-00000170: 5f6f 7329 01da 056c 6576 656c 6300 0000  _os)...levelc...
-00000180: 0000 0000 0000 0000 0000 0000 0004 0000  ................
-00000190: 0040 0000 0173 5400 0000 6500 5a01 6400  .@...sT...e.Z.d.
-000001a0: 5a02 6401 5a03 6419 6409 640a 8404 5a04  Z.d.Z.d.d.d...Z.
-000001b0: 641a 640d 640e 8404 5a05 641a 640f 6410  d.d.d...Z.d.d.d.
-000001c0: 8404 5a06 641a 6411 6412 8404 5a07 6508  ..Z.d.d.d...Z.e.
-000001d0: 641b 6414 6415 8404 8301 5a09 6508 641b  d.d.d.....Z.e.d.
-000001e0: 6416 6417 8404 8301 5a0a 6418 5300 291c  d.d.....Z.d.S.).
-000001f0: da0a 5075 6c73 6554 696d 6572 7a68 5065  ..PulseTimerzhPe
-00000200: 7269 6f64 6963 616c 6c79 2072 756e 7320  riodically runs 
-00000210: 6120 6675 6e63 7469 6f6e 2069 6e20 6120  a function in a 
-00000220: 6261 636b 6772 6f75 6e64 2074 6872 6561  background threa
-00000230: 642e 0a0a 2020 2020 7265 663a 2068 7474  d...    ref: htt
-00000240: 7073 3a2f 2f73 7461 636b 6f76 6572 666c  ps://stackoverfl
-00000250: 6f77 2e63 6f6d 2f61 2f31 3331 3531 3239  ow.com/a/1315129
-00000260: 390a 2020 2020 da04 6172 6773 7205 0000  9.    ..argsr...
-00000270: 00da 0b69 6e74 6572 7661 6c5f 6d73 da03  ...interval_ms..
-00000280: 696e 74da 0366 756e fa12 4361 6c6c 6162  int..fun..Callab
-00000290: 6c65 5b2e 2e2e 2c20 416e 795d da06 6b77  le[..., Any]..kw
-000002a0: 6172 6773 6301 0000 0000 0000 0002 0000  argsc...........
-000002b0: 0005 0000 0002 0000 004f 0000 0173 2e00  .........O...s..
-000002c0: 0000 6400 7c00 5f00 7c01 7c00 5f01 7c02  ..d.|._.|.|._.|.
-000002d0: 7c00 5f02 7c03 7c00 5f03 7c04 7c00 5f04  |._.|.|._.|.|._.
-000002e0: 6401 7c00 5f05 6401 7c00 5f06 6400 5300  d.|._.d.|._.d.S.
-000002f0: a902 4e46 2907 da06 5f74 696d 6572 da09  ..NF)..._timer..
-00000300: 5f69 6e74 6572 7661 6cda 095f 6675 6e63  _interval.._func
-00000310: 7469 6f6e da05 5f61 7267 73da 075f 6b77  tion.._args.._kw
-00000320: 6172 6773 da0b 5f69 735f 656e 6162 6c65  args.._is_enable
-00000330: 64da 0b5f 6973 5f72 756e 6e69 6e67 2905  d.._is_running).
-00000340: da04 7365 6c66 7212 0000 0072 1400 0000  ..selfr....r....
-00000350: 7211 0000 0072 1600 0000 a900 7220 0000  r....r......r ..
-00000360: 00fa 1f2f 6472 6f6e 652f 7372 632f 7372  .../drone/src/sr
-00000370: 632f 7070 7175 6575 652f 7175 6575 652e  c/ppqueue/queue.
-00000380: 7079 da08 5f5f 696e 6974 5f5f 1a00 0000  py..__init__....
-00000390: 730e 0000 0006 0706 0106 0106 0106 0106  s...............
-000003a0: 010a 017a 1350 756c 7365 5469 6d65 722e  ...z.PulseTimer.
-000003b0: 5f5f 696e 6974 5f5f da06 7265 7475 726e  __init__..return
-000003c0: da04 4e6f 6e65 6301 0000 0000 0000 0000  ..Nonec.........
-000003d0: 0000 0001 0000 0004 0000 0043 0000 0173  ...........C...s
-000003e0: 2600 0000 6401 7c00 5f00 7c00 a001 a100  &...d.|._.|.....
-000003f0: 0100 7c00 6a02 7c00 6a03 6900 7c00 6a04  ..|.j.|.j.i.|.j.
-00000400: a401 8e01 0100 6400 5300 7217 0000 0029  ......d.S.r....)
-00000410: 0572 1e00 0000 da05 7374 6172 7472 1a00  .r......startr..
-00000420: 0000 721b 0000 0072 1c00 0000 a901 721f  ..r....r......r.
-00000430: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00000440: 0000 da04 5f72 756e 2900 0000 7306 0000  ...._run)...s...
-00000450: 0006 0108 0118 017a 0f50 756c 7365 5469  .......z.PulseTi
-00000460: 6d65 722e 5f72 756e 6301 0000 0000 0000  mer._runc.......
-00000470: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
-00000480: 0173 3600 0000 7c00 6a00 7316 7401 a002  .s6...|.j.s.t...
-00000490: 7c00 6a03 6401 1b00 7c00 6a04 a102 7c00  |.j.d...|.j...|.
-000004a0: 5f05 7c00 6a05 a006 a100 0100 6402 7c00  _.|.j.......d.|.
-000004b0: 5f00 6402 7c00 5f07 6400 5300 2903 4ee9  _.d.|._.d.S.).N.
-000004c0: e803 0000 5429 0872 1e00 0000 da09 7468  ....T).r......th
-000004d0: 7265 6164 696e 67da 0554 696d 6572 7219  reading..Timerr.
-000004e0: 0000 0072 2700 0000 7218 0000 0072 2500  ...r'...r....r%.
-000004f0: 0000 721d 0000 0072 2600 0000 7220 0000  ..r....r&...r ..
-00000500: 0072 2000 0000 7221 0000 0072 2500 0000  .r ...r!...r%...
-00000510: 2e00 0000 730a 0000 0006 0116 010a 0106  ....s...........
-00000520: 010a 027a 1050 756c 7365 5469 6d65 722e  ...z.PulseTimer.
-00000530: 7374 6172 7463 0100 0000 0000 0000 0000  startc..........
-00000540: 0000 0100 0000 0200 0000 4300 0001 7324  ..........C...s$
-00000550: 0000 007c 006a 0064 0075 0172 0a7c 006a  ...|.j.d.u.r.|.j
-00000560: 00a0 01a1 0001 0064 017c 005f 0264 017c  .......d.|._.d.|
-00000570: 005f 0364 0053 0072 1700 0000 2904 7218  ._.d.S.r....).r.
-00000580: 0000 00da 0663 616e 6365 6c72 1d00 0000  .....cancelr....
-00000590: 721e 0000 0072 2600 0000 7220 0000 0072  r....r&...r ...r
-000005a0: 2000 0000 7221 0000 00da 0473 746f 7036   ...r!.....stop6
-000005b0: 0000 0073 0800 0000 0a01 0a01 0602 0a01  ...s............
-000005c0: 7a0f 5075 6c73 6554 696d 6572 2e73 746f  z.PulseTimer.sto
-000005d0: 70da 0462 6f6f 6c63 0100 0000 0000 0000  p..boolc........
-000005e0: 0000 0000 0100 0000 0100 0000 4300 0001  ............C...
-000005f0: f306 0000 007c 006a 0053 00a9 014e 2901  .....|.j.S...N).
-00000600: 721e 0000 0072 2600 0000 7220 0000 0072  r....r&...r ...r
-00000610: 2000 0000 7221 0000 00da 0a69 735f 7275   ...r!.....is_ru
-00000620: 6e6e 696e 673d 0000 00f3 0200 0000 0602  nning=..........
-00000630: 7a15 5075 6c73 6554 696d 6572 2e69 735f  z.PulseTimer.is_
-00000640: 7275 6e6e 696e 6763 0100 0000 0000 0000  runningc........
-00000650: 0000 0000 0100 0000 0100 0000 4300 0001  ............C...
-00000660: 722e 0000 0072 2f00 0000 2901 721d 0000  r....r/...).r...
-00000670: 0072 2600 0000 7220 0000 0072 2000 0000  .r&...r ...r ...
-00000680: 7221 0000 00da 0a69 735f 656e 6162 6c65  r!.....is_enable
-00000690: 6441 0000 0072 3100 0000 7a15 5075 6c73  dA...r1...z.Puls
-000006a0: 6554 696d 6572 2e69 735f 656e 6162 6c65  eTimer.is_enable
-000006b0: 644e 2908 7211 0000 0072 0500 0000 7212  dN).r....r....r.
-000006c0: 0000 0072 1300 0000 7214 0000 0072 1500  ...r....r....r..
-000006d0: 0000 7216 0000 0072 0500 0000 a902 7223  ..r....r......r#
-000006e0: 0000 0072 2400 0000 a902 7223 0000 0072  ...r$.....r#...r
-000006f0: 2d00 0000 290b da08 5f5f 6e61 6d65 5f5f  -...)...__name__
-00000700: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00000710: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00000720: 635f 5f72 2200 0000 7227 0000 0072 2500  c__r"...r'...r%.
-00000730: 0000 722c 0000 00da 0870 726f 7065 7274  ..r,.....propert
-00000740: 7972 3000 0000 7232 0000 0072 2000 0000  yr0...r2...r ...
-00000750: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-00000760: 1000 0000 1400 0000 7314 0000 0008 0004  ........s.......
-00000770: 010a 050a 0f0a 050a 0802 070c 0102 0310  ................
-00000780: 0172 1000 0000 6300 0000 0000 0000 0000  .r....c.........
-00000790: 0000 0000 0000 000b 0000 0040 0000 0173  ...........@...s
-000007a0: 5e02 0000 6500 5a01 6400 5a02 5500 6401  ^...e.Z.d.Z.U.d.
-000007b0: 5a03 6402 6504 6403 3c00 6505 a006 a100  Z.d.e.d.<.e.....
-000007c0: 6601 6404 6507 6a08 6401 6401 6405 6405  f.d.e.j.d.d.d.d.
-000007d0: 6405 6406 6405 6407 9c09 6496 6417 6418  d.d.d.d...d.d.d.
-000007e0: 8407 5a09 6497 641e 641f 8404 5a0a 6498  ..Z.d.d.d...Z.d.
-000007f0: 6422 6423 8404 5a0b 6498 6424 6425 8404  d"d#..Z.d.d$d%..
-00000800: 5a0c 6498 6426 6427 8404 5a0d 6498 6428  Z.d.d&d'..Z.d.d(
-00000810: 6429 8404 5a0e 6498 642a 642b 8404 5a0f  d)..Z.d.d*d+..Z.
-00000820: 642c 642d 9c01 6499 642f 6430 8406 5a10  d,d-..d.d/d0..Z.
-00000830: 649a 6431 6432 8404 5a11 649b 6433 6434  d.d1d2..Z.d.d3d4
-00000840: 8404 5a12 649a 6435 6436 8404 5a13 649c  ..Z.d.d5d6..Z.d.
-00000850: 6438 6439 8404 5a14 6498 643a 643b 8404  d8d9..Z.d.d:d;..
-00000860: 5a15 649d 643c 643d 8404 5a16 649d 643e  Z.d.d<d=..Z.d.d>
-00000870: 643f 8404 5a17 649d 6440 6441 8404 5a18  d?..Z.d.d@dA..Z.
-00000880: 649d 6442 6443 8404 5a19 6405 6405 6405  d.dBdC..Z.d.d.d.
-00000890: 6444 9c03 649e 6449 644a 8406 5a1a 649d  dD..d.dIdJ..Z.d.
-000008a0: 644b 644c 8404 5a1b 6405 6405 6405 6444  dKdL..Z.d.d.d.dD
-000008b0: 9c03 649f 644d 644e 8406 5a1c 64a0 644f  ..d.dMdN..Z.d.dO
-000008c0: 6450 8404 5a1d 64a0 6451 6452 8404 5a1e  dP..Z.d.dQdR..Z.
-000008d0: 64a0 6453 6454 8404 5a1f 64a0 6455 6456  d.dSdT..Z.d.dUdV
-000008e0: 8404 5a20 649d 6457 6458 8404 5a21 6404  ..Z d.dWdX..Z!d.
-000008f0: 6404 6404 6401 6459 9c04 64a1 645f 6460  d.d.d.dY..d.d_d`
-00000900: 8406 5a22 6523 64a2 6465 6466 8404 8301  ..Z"e#d.dedf....
-00000910: 5a24 64a3 6468 6469 8404 5a25 64a4 646a  Z$d.dhdi..Z%d.dj
-00000920: 646b 8404 5a26 0901 0901 0901 0906 0901  dk..Z&..........
-00000930: 0904 0905 0905 64a5 64a6 6472 6473 8405  ......d.d.drds..
-00000940: 5a27 649d 6474 6475 8404 5a28 6404 6401  Z'd.dtdu..Z(d.d.
-00000950: 6476 9c02 64a7 647a 647b 8406 5a29 6404  dv..d.dzd{..Z)d.
-00000960: 6401 6476 9c02 64a8 647d 647e 8406 5a2a  d.dv..d.d}d~..Z*
-00000970: 6404 6401 6476 9c02 64a9 6480 6481 8406  d.d.dv..d.d.d...
-00000980: 5a2b 6405 6405 6482 9c02 64aa 6485 6486  Z+d.d.d...d.d.d.
-00000990: 8406 5a2c 64ab 6487 6488 8404 5a2d 64ab  ..Z,d.d.d...Z-d.
-000009a0: 6489 648a 8404 5a2e 64ac 64ad 648b 648c  d.d...Z.d.d.d.d.
-000009b0: 8405 5a2f 6530 649d 648d 648e 8404 8301  ..Z/e0d.d.d.....
-000009c0: 5a31 6531 6a32 64ae 6490 648e 8404 8301  Z1e1j2d.d.d.....
-000009d0: 5a31 6530 649d 6491 6492 8404 8301 5a33  Z1e0d.d.d.....Z3
-000009e0: 6533 6a32 64af 6493 6492 8404 8301 5a33  e3j2d.d.d.....Z3
-000009f0: 6530 64a0 6494 6495 8404 8301 5a34 6401  e0d.d.d.....Z4d.
-00000a00: 5300 29b0 da05 5175 6575 654e fa0a 696e  S.)...QueueN..in
-00000a10: 7420 7c20 4e6f 6e65 da0d 4445 4641 554c  t | None..DEFAUL
-00000a20: 545f 4752 4f55 5072 0100 0000 46e9 6400  T_GROUPr....F.d.
-00000a30: 0000 2909 da08 6d61 785f 7369 7a65 da06  ..)...max_size..
-00000a40: 656e 6769 6e65 da04 6e61 6d65 da08 6361  engine..name..ca
-00000a50: 6c6c 6261 636b da0d 7368 6f77 5f70 726f  llback..show_pro
-00000a60: 6772 6573 73da 0d64 726f 705f 6669 6e69  gress..drop_fini
-00000a70: 7368 6564 da0e 7374 6f70 5f77 6865 6e5f  shed..stop_when_
-00000a80: 6964 6c65 da0d 7075 6c73 655f 6672 6571  idle..pulse_freq
-00000a90: 5f6d 73da 086e 6f5f 7374 6172 74da 0e6d  _ms..no_start..m
-00000aa0: 6178 5f63 6f6e 6375 7272 656e 7472 1300  ax_concurrentr..
-00000ab0: 0000 723e 0000 0072 3f00 0000 fa29 5479  ..r>...r?....)Ty
-00000ac0: 7065 5b74 6872 6561 6469 6e67 2e54 6872  pe[threading.Thr
-00000ad0: 6561 645d 207c 2054 7970 655b 6d70 2e50  ead] | Type[mp.P
-00000ae0: 726f 6365 7373 5d72 4000 0000 fa0a 7374  rocess]r@.....st
-00000af0: 7220 7c20 4e6f 6e65 7241 0000 00fa 1b43  r | NonerA.....C
-00000b00: 616c 6c61 626c 655b 5b4a 6f62 5d2c 2041  allable[[Job], A
-00000b10: 6e79 5d20 7c20 4e6f 6e65 7242 0000 0072  ny] | NonerB...r
-00000b20: 2d00 0000 7243 0000 0072 4400 0000 7245  -...rC...rD...rE
-00000b30: 0000 0072 4600 0000 6302 0000 0000 0000  ...rF...c.......
-00000b40: 0009 0000 000b 0000 0004 0000 0043 0000  .............C..
-00000b50: 0173 0001 0000 7c04 7204 7c04 6e08 7400  .s....|.r.|.n.t.
-00000b60: 7401 8300 8301 6401 6402 8502 1900 7c00  t.....d.d.....|.
-00000b70: 5f02 7c06 7c00 5f03 7c02 7c00 5f04 6403  _.|.|._.|.|._.d.
-00000b80: 7c00 5f05 6403 7c00 5f06 7c01 7c00 5f07  |._.d.|._.|.|._.
-00000b90: 7c05 7c00 5f08 7409 a00a a100 7c00 5f0b  |.|._.t.....|._.
-00000ba0: 7c03 740c 6a0d 7500 7232 740e 8300 7232  |.t.j.u.r2t...r2
-00000bb0: 740f a010 6404 a101 0100 7c03 7c00 5f11  t...d.....|.|._.
-00000bc0: 6401 6700 6901 7c00 5f12 6900 7c00 5f13  d.g.i.|._.i.|._.
-00000bd0: 6700 7c00 5f14 7c07 7c00 5f15 6401 7c00  g.|._.|.|._.d.|.
-00000be0: 5f16 7c00 0100 7c00 6a11 740c 6a0d 7500  _.|...|.j.t.j.u.
-00000bf0: 725a 740c a017 a100 7c00 5f16 7c00 6a16  rZt.....|._.|.j.
-00000c00: a018 a100 7c00 5f19 6e03 6900 7c00 5f19  ....|._.n.i.|._.
-00000c10: 740f a01a 6405 7c00 6a07 a102 0100 7c09  t...d.|.j.....|.
-00000c20: 7c00 5f1b 741c 7c00 6a1b 7c00 6a1d 6406  |._.t.|.j.|.j.d.
-00000c30: 8d02 7c00 5f1e 7c0a 7376 7c00 a01f a100  ..|._.|.sv|.....
-00000c40: 0100 7c08 7c00 5f20 740f a01a 6407 a101  ..|.|._ t...d...
-00000c50: 0100 6401 5300 2908 6136 0400 000a 0a20  ..d.S.).a6..... 
-00000c60: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-00000c70: 2020 2020 2020 2020 206d 6178 5f63 6f6e           max_con
-00000c80: 6375 7272 656e 743a 206d 6178 206e 756d  current: max num
-00000c90: 6265 7220 6f66 2063 6f6e 6375 7272 656e  ber of concurren
-00000ca0: 746c 7920 7275 6e6e 696e 6720 6a6f 6273  tly running jobs
-00000cb0: 2e0a 2020 2020 2020 2020 2020 2020 6d61  ..            ma
-00000cc0: 785f 7369 7a65 3a20 6d61 7820 7369 7a65  x_size: max size
-00000cd0: 206f 6620 7468 6520 7175 6575 6520 2864   of the queue (d
-00000ce0: 6566 6175 6c74 3d30 2c20 756e 6c69 6d69  efault=0, unlimi
-00000cf0: 7465 6429 2e0a 2020 2020 2020 2020 2020  ted)..          
-00000d00: 2020 656e 6769 6e65 3a20 7468 6520 656e    engine: the en
-00000d10: 6769 6e65 2075 7365 6420 746f 2072 756e  gine used to run
-00000d20: 206a 6f62 733b 2074 6872 6561 6473 2028   jobs; threads (
-00000d30: 6465 6661 756c 7429 206f 7220 7072 6f63  default) or proc
-00000d40: 6573 7365 732e 0a20 2020 2020 2020 2020  esses..         
-00000d50: 2020 206e 616d 653a 2061 6e20 6964 656e     name: an iden
-00000d60: 7469 6669 6572 2066 6f72 2074 6869 7320  tifier for this 
-00000d70: 7175 6575 652e 0a20 2020 2020 2020 2020  queue..         
-00000d80: 2020 2063 616c 6c62 6163 6b3a 2061 2063     callback: a c
-00000d90: 616c 6c61 626c 6520 7468 6174 2069 7320  allable that is 
-00000da0: 6361 6c6c 6564 2069 6d6d 6564 6961 7465  called immediate
-00000db0: 6c79 2061 6674 6572 2065 6163 6820 6a6f  ly after each jo
-00000dc0: 6220 6973 2066 696e 6973 6865 642e 0a20  b is finished.. 
-00000dd0: 2020 2020 2020 2020 2020 2073 686f 775f             show_
-00000de0: 7072 6f67 7265 7373 3a20 676c 6f62 616c  progress: global
-00000df0: 2073 6574 7469 6e67 2066 6f72 2073 686f   setting for sho
-00000e00: 7769 6e67 2070 726f 6772 6573 7320 6261  wing progress ba
-00000e10: 7273 2e0a 2020 2020 2020 2020 2020 2020  rs..            
-00000e20: 6472 6f70 5f66 696e 6973 6865 643a 2069  drop_finished: i
-00000e30: 6620 5472 7565 2c20 7468 6520 7175 6575  f True, the queu
-00000e40: 6520 7769 6c6c 206e 6f74 2073 746f 7265  e will not store
-00000e50: 2066 696e 6973 6865 6420 6a6f 6273 2066   finished jobs f
-00000e60: 6f72 2072 6574 7269 6576 616c 2e0a 2020  or retrieval..  
-00000e70: 2020 2020 2020 2020 2020 7374 6f70 5f77            stop_w
-00000e80: 6865 6e5f 6964 6c65 3a20 6966 2054 7275  hen_idle: if Tru
-00000e90: 652c 2074 6865 2071 7565 7565 2077 696c  e, the queue wil
-00000ea0: 6c20 7374 6f70 2074 6865 2070 756c 7365  l stop the pulse
-00000eb0: 2077 6865 6e20 616c 6c20 6a6f 6273 2061   when all jobs a
-00000ec0: 7265 2066 696e 6973 6865 642e 0a20 2020  re finished..   
-00000ed0: 2020 2020 2020 2020 2070 756c 7365 5f66           pulse_f
-00000ee0: 7265 715f 6d73 3a20 7468 6520 696e 7465  req_ms: the inte
-00000ef0: 7276 616c 2061 7420 7768 6963 6820 6a6f  rval at which jo
-00000f00: 6273 2061 7265 2074 7261 6e73 6974 696f  bs are transitio
-00000f10: 6e65 6420 6265 7477 6565 6e20 696e 7465  ned between inte
-00000f20: 726e 616c 2071 7565 7565 732e 0a20 2020  rnal queues..   
-00000f30: 2020 2020 2020 2020 206e 6f5f 7374 6172           no_star
-00000f40: 743a 2069 6620 5472 7565 2c20 646f 206e  t: if True, do n
-00000f50: 6f74 2073 7461 7274 2074 6865 2071 7565  ot start the que
-00000f60: 7565 2070 756c 7365 206f 6e20 696e 7374  ue pulse on inst
-00000f70: 616e 7469 6174 696f 6e2e 0a0a 2020 2020  antiation...    
-00000f80: 2020 2020 4578 616d 706c 6573 3a0a 2020      Examples:.  
-00000f90: 2020 2020 2020 2020 2020 3e3e 3e20 6672            >>> fr
-00000fa0: 6f6d 2070 7071 7565 7565 2069 6d70 6f72  om ppqueue impor
-00000fb0: 7420 5175 6575 650a 2020 2020 2020 2020  t Queue.        
-00000fc0: 2020 2020 3e3e 3e20 6672 6f6d 2074 696d      >>> from tim
-00000fd0: 6520 696d 706f 7274 2073 6c65 6570 0a20  e import sleep. 
-00000fe0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
-00000ff0: 2020 2020 2020 2020 2020 203e 3e3e 2077             >>> w
-00001000: 6974 6820 5175 6575 6528 2920 6173 2071  ith Queue() as q
-00001010: 7565 7565 3a0a 2020 2020 2020 2020 2020  ueue:.          
-00001020: 2020 2e2e 2e20 2020 2020 6a6f 6273 203d    ...     jobs =
-00001030: 2071 7565 7565 2e6d 6170 2873 6c65 6570   queue.map(sleep
-00001040: 2c20 5b31 2c20 322c 2033 2c20 342c 2035  , [1, 2, 3, 4, 5
-00001050: 5d29 0a20 2020 2020 2020 2020 2020 202e  ]).            .
-00001060: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-00001070: 3e3e 206c 656e 286a 6f62 7329 0a20 2020  >> len(jobs).   
-00001080: 2020 2020 2020 2020 2035 0a20 2020 2020           5.     
-00001090: 2020 204e e908 0000 0072 0100 0000 7ab0     N.....r....z.
-000010a0: 6d75 6c74 6970 726f 6365 7373 696e 6720  multiprocessing 
-000010b0: 7065 7266 6f72 6d61 6e63 6520 6973 2064  performance is d
-000010c0: 6567 7261 6465 6420 6f6e 2057 696e 646f  egraded on Windo
-000010d0: 7773 2073 7973 7465 6d73 2e20 7365 653a  ws systems. see:
-000010e0: 2068 7474 7073 3a2f 2f64 6f63 732e 7079   https://docs.py
-000010f0: 7468 6f6e 2e6f 7267 2f33 2f6c 6962 7261  thon.org/3/libra
-00001100: 7279 2f6d 756c 7469 7072 6f63 6573 7369  ry/multiprocessi
-00001110: 6e67 2e68 746d 6c3f 6869 6768 6c69 6768  ng.html?highligh
-00001120: 743d 7072 6f63 6573 7323 7468 652d 7370  t=process#the-sp
-00001130: 6177 6e2d 616e 642d 666f 726b 7365 7276  awn-and-forkserv
-00001140: 6572 2d73 7461 7274 2d6d 6574 686f 6473  er-start-methods
-00001150: 7a29 496e 6974 6961 6c69 7a65 6420 7175  z)Initialized qu
-00001160: 6575 6520 7769 7468 2025 6420 6d61 785f  eue with %d max_
-00001170: 636f 6e63 7572 7265 6e74 2e29 0272 1200  concurrent.).r..
-00001180: 0000 7214 0000 007a 1249 6e69 7469 616c  ..r....z.Initial
-00001190: 697a 6564 2070 756c 7365 2e29 21da 0373  ized pulse.)!..s
-000011a0: 7472 7209 0000 00da 045f 7169 6472 4200  trr......_qidrB.
-000011b0: 0000 da09 5f6d 6178 5f73 697a 65da 0c5f  ...._max_size.._
-000011c0: 636f 756e 745f 696e 7075 74da 0d5f 636f  count_input.._co
-000011d0: 756e 745f 6f75 7470 7574 da0f 5f6d 6178  unt_output.._max
-000011e0: 5f63 6f6e 6375 7272 656e 74da 095f 6361  _concurrent.._ca
-000011f0: 6c6c 6261 636b 7229 0000 00da 044c 6f63  llbackr).....Loc
-00001200: 6bda 055f 6c6f 636b da02 6d70 da07 5072  k.._lock..mp..Pr
-00001210: 6f63 6573 7372 0e00 0000 da03 4c4f 47da  ocessr......LOG.
-00001220: 0777 6172 6e69 6e67 da07 5f65 6e67 696e  .warning.._engin
-00001230: 65da 0f5f 7761 6974 696e 675f 6772 6f75  e.._waiting_grou
-00001240: 7073 da0e 5f77 6f72 6b69 6e67 5f71 7565  ps.._working_que
-00001250: 7565 da0f 5f66 696e 6973 6865 645f 7175  ue.._finished_qu
-00001260: 6575 65da 0e5f 6472 6f70 5f66 696e 6973  eue.._drop_finis
-00001270: 6865 64da 0b5f 6d70 5f6d 616e 6167 6572  hed.._mp_manager
-00001280: da07 4d61 6e61 6765 72da 0464 6963 74da  ..Manager..dict.
-00001290: 075f 6f75 7470 7574 da05 6465 6275 67da  ._output..debug.
-000012a0: 0e5f 7075 6c73 655f 6672 6571 5f6d 7372  ._pulse_freq_msr
-000012b0: 1000 0000 da06 5f70 756c 7365 7218 0000  ......_pulser...
-000012c0: 0072 2500 0000 da0f 5f73 746f 705f 7768  .r%....._stop_wh
-000012d0: 656e 5f69 646c 6529 0b72 1f00 0000 7247  en_idle).r....rG
-000012e0: 0000 0072 3e00 0000 723f 0000 0072 4000  ...r>...r?...r@.
-000012f0: 0000 7241 0000 0072 4200 0000 7243 0000  ..rA...rB...rC..
-00001300: 0072 4400 0000 7245 0000 0072 4600 0000  .rD...rE...rF...
-00001310: 7220 0000 0072 2000 0000 7221 0000 0072  r ...r ...r!...r
-00001320: 2200 0000 4900 0000 7344 0000 001c 2706  "...I...sD....'.
-00001330: 0206 0106 0106 0106 0106 0106 0304 ff10  ................
-00001340: 0404 0102 0204 fe06 070a 0206 0106 0106  ................
-00001350: 0206 0104 020c 020a 010e 0106 020e 0206  ................
-00001360: 0202 0104 0104 0108 fe04 0508 0106 020e  ................
-00001370: 027a 0e51 7565 7565 2e5f 5f69 6e69 745f  .z.Queue.__init_
-00001380: 5f72 1400 0000 7215 0000 0072 1100 0000  _r....r....r....
-00001390: 7205 0000 0072 1600 0000 6302 0000 0000  r....r....c.....
-000013a0: 0000 0000 0000 0005 0000 0004 0000 000f  ................
-000013b0: 0000 0173 1c00 0000 8801 a000 a100 0100  ...s............
-000013c0: 640a 8700 8701 6602 6408 6409 840c 7d04  d.....f.d.d...}.
-000013d0: 7c04 5300 290b 4eda 0869 7465 7261 626c  |.S.).N..iterabl
-000013e0: 65fa 0d53 6571 7565 6e63 655b 416e 795d  e..Sequence[Any]
-000013f0: 7211 0000 0072 0500 0000 7216 0000 0072  r....r....r....r
-00001400: 2300 0000 fa09 6c69 7374 5b4a 6f62 5d63  #.....list[Job]c
-00001410: 0100 0000 0000 0000 0000 0000 0500 0000  ................
-00001420: 0600 0000 1f00 0001 733c 0000 007c 0044  ........s<...|.D
-00001430: 005d 0d7d 0388 016a 0088 007c 0367 017c  .].}...j...|.g.|
-00001440: 01a2 017c 0264 018d 0301 0071 0288 01a0  ...|.d.....q....
-00001450: 01a1 0001 0088 01a0 02a1 007d 0488 01a0  ...........}....
-00001460: 03a1 0001 007c 0453 0029 024e 2902 7211  .....|.S.).N).r.
-00001470: 0000 0072 1600 0000 2904 da07 656e 7175  ...r....)...enqu
-00001480: 6575 65da 0477 6169 74da 0763 6f6c 6c65  eue..wait..colle
-00001490: 6374 da07 6469 7370 6f73 6529 0572 6600  ct..dispose).rf.
-000014a0: 0000 7211 0000 0072 1600 0000 da01 78da  ..r....r......x.
-000014b0: 086a 6f62 5f64 6174 61a9 0272 1400 0000  .job_data..r....
-000014c0: 721f 0000 0072 2000 0000 7221 0000 00da  r....r ...r!....
-000014d0: 0977 7261 7070 6564 5f66 a900 0000 730c  .wrapped_f....s.
-000014e0: 0000 0008 0118 0108 0108 0108 0104 017a  ...............z
-000014f0: 2151 7565 7565 2e5f 5f63 616c 6c5f 5f2e  !Queue.__call__.
-00001500: 3c6c 6f63 616c 733e 2e77 7261 7070 6564  <locals>.wrapped
-00001510: 5f66 2908 7266 0000 0072 6700 0000 7211  _f).rf...rg...r.
-00001520: 0000 0072 0500 0000 7216 0000 0072 0500  ...r....r....r..
-00001530: 0000 7223 0000 0072 6800 0000 2901 7225  ..r#...rh...).r%
-00001540: 0000 0029 0572 1f00 0000 7214 0000 0072  ...).r....r....r
-00001550: 1100 0000 7216 0000 0072 7000 0000 7220  ....r....rp...r 
-00001560: 0000 0072 6f00 0000 7221 0000 00da 085f  ...ro...r!....._
-00001570: 5f63 616c 6c5f 5fa6 0000 0073 0600 0000  _call__....s....
-00001580: 0801 1002 0408 7a0e 5175 6575 652e 5f5f  ......z.Queue.__
-00001590: 6361 6c6c 5f5f 7223 0000 0072 2400 0000  call__r#...r$...
-000015a0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-000015b0: 0002 0000 0043 0000 01f3 0c00 0000 7c00  .....C........|.
-000015c0: a000 a100 0100 6400 5300 722f 0000 00a9  ......d.S.r/....
-000015d0: 0172 6c00 0000 7226 0000 0072 2000 0000  .rl...r&...r ...
-000015e0: 7220 0000 0072 2100 0000 da07 5f5f 6465  r ...r!.....__de
-000015f0: 6c5f 5fb3 0000 00f3 0200 0000 0c01 7a0d  l__...........z.
-00001600: 5175 6575 652e 5f5f 6465 6c5f 5f63 0100  Queue.__del__c..
-00001610: 0000 0000 0000 0000 0000 0100 0000 0200  ................
-00001620: 0000 4300 0001 f30e 0000 007c 006a 00a0  ..C........|.j..
-00001630: 01a1 0001 0064 0153 0029 027a 1653 7461  .....d.S.).z.Sta
-00001640: 7274 2074 6865 2071 7565 7565 2070 756c  rt the queue pul
-00001650: 7365 2e4e 2902 7218 0000 0072 2500 0000  se.N).r....r%...
-00001660: 7226 0000 0072 2000 0000 7220 0000 0072  r&...r ...r ...r
-00001670: 2100 0000 7225 0000 00b6 0000 00f3 0200  !...r%..........
-00001680: 0000 0e02 7a0b 5175 6575 652e 7374 6172  ....z.Queue.star
-00001690: 7463 0100 0000 0000 0000 0000 0000 0100  tc..............
-000016a0: 0000 0200 0000 4300 0001 7276 0000 0029  ......C...rv...)
-000016b0: 027a 1553 746f 7020 7468 6520 7175 6575  .z.Stop the queu
-000016c0: 6520 7075 6c73 652e 4e29 0272 1800 0000  e pulse.N).r....
-000016d0: 722c 0000 0072 2600 0000 7220 0000 0072  r,...r&...r ...r
-000016e0: 2000 0000 7221 0000 0072 2c00 0000 ba00   ...r!...r,.....
-000016f0: 0000 7277 0000 007a 0a51 7565 7565 2e73  ..rw...z.Queue.s
-00001700: 746f 7063 0100 0000 0000 0000 0000 0000  topc............
-00001710: 0100 0000 0300 0000 4300 0001 7384 0000  ........C...s...
-00001720: 0074 00a0 0164 01a1 0101 007c 006a 0272  .t...d.....|.j.r
-00001730: 127c 006a 0364 0264 038d 0101 007c 00a0  .|.j.d.d.....|..
-00001740: 04a1 0001 0074 00a0 0164 04a1 0101 0064  .....t...d.....d
-00001750: 057c 005f 0574 00a0 0164 06a1 0101 007c  .|._.t...d.....|
-00001760: 006a 06a0 07a1 0001 0074 00a0 0164 07a1  .j.......t...d..
-00001770: 0101 0064 087c 005f 0864 087c 005f 0974  ...d.|._.d.|._.t
-00001780: 00a0 0164 09a1 0101 007c 006a 0a64 0575  ...d.....|.j.d.u
-00001790: 0172 407c 006a 0aa0 0ba1 0001 0064 0553  .r@|.j.......d.S
-000017a0: 0064 0553 0029 0a7a 4353 746f 7020 7275  .d.S.).zCStop ru
-000017b0: 6e6e 696e 6720 6a6f 6273 2c20 7468 656e  nning jobs, then
-000017c0: 2063 6c65 6172 2074 6865 2071 7565 7565   clear the queue
-000017d0: 2c20 7468 656e 2073 746f 7020 7468 6520  , then stop the 
-000017e0: 7175 6575 6520 7075 6c73 652e 5a09 4469  queue pulse.Z.Di
-000017f0: 7370 6f73 696e 6754 a901 726a 0000 007a  sposingT..rj...z
-00001800: 0d52 656d 6f76 6564 206a 6f62 732e 4e7a  .Removed jobs.Nz
-00001810: 0f52 656d 6f76 6564 206f 7574 7075 742e  .Removed output.
-00001820: 7a11 5265 6d6f 7665 6420 6669 6e69 7368  z.Removed finish
-00001830: 6564 2e72 0100 0000 7a0f 5265 7365 7420  ed.r....z.Reset 
-00001840: 636f 756e 7465 7273 2e29 0c72 5700 0000  counters.).rW...
-00001850: 7262 0000 0072 3000 0000 da09 5f73 746f  rb...r0....._sto
-00001860: 705f 616c 6c72 2c00 0000 7261 0000 0072  p_allr,...ra...r
-00001870: 5c00 0000 da05 636c 6561 7272 4f00 0000  \.....clearrO...
-00001880: 7250 0000 0072 5e00 0000 da08 7368 7574  rP...r^.....shut
-00001890: 646f 776e 7226 0000 0072 2000 0000 7220  downr&...r ...r 
-000018a0: 0000 0072 2100 0000 726c 0000 00be 0000  ...r!...rl......
-000018b0: 0073 1e00 0000 0a02 0602 0c01 0801 0a02  .s..............
-000018c0: 0601 0a01 0a01 0a01 0601 0601 0a01 0a02  ................
-000018d0: 0e01 04ff 7a0d 5175 6575 652e 6469 7370  ....z.Queue.disp
-000018e0: 6f73 6563 0100 0000 0000 0000 0000 0000  osec............
-000018f0: 0600 0000 0800 0000 4300 0001 73ae 0000  ........C...s...
-00001900: 0074 00a0 0164 01a1 0101 007c 006a 028f  .t...d.....|.j..
-00001910: 4501 0074 037c 006a 04a0 05a1 0083 017d  E..t.|.j.......}
-00001920: 017c 0144 005d 327d 027c 006a 04a0 067c  .|.D.]2}.|.j...|
-00001930: 02a1 017d 0374 0774 087c 0383 0183 0144  ...}.t.t.|.....D
-00001940: 005d 1f7d 0474 097c 0383 017d 0564 027c  .].}.t.|...}.d.|
-00001950: 055f 0a74 0ba0 0ba1 007c 055f 0c7c 006a  ._.t.....|._.|.j
-00001960: 0d73 3874 0e7c 006a 0f7c 0583 0201 0071  .s8t.|.j.|.....q
-00001970: 207c 0004 006a 1064 0337 0002 005f 1071   |...j.d.7..._.q
-00001980: 207c 006a 047c 023d 0071 1257 0064 0404   |.j.|.=.q.W.d..
-00001990: 0004 0083 0301 0064 0453 0031 0073 5077  .......d.S.1.sPw
-000019a0: 0101 0001 0001 0059 0001 0064 0453 0029  .......Y...d.S.)
-000019b0: 057a 2043 6c65 6172 2074 6865 2071 7565  .z Clear the que
-000019c0: 7565 206f 6620 7065 6e64 696e 6720 6a6f  ue of pending jo
-000019d0: 6273 2e7a 1643 6c65 6172 696e 6720 7761  bs.z.Clearing wa
-000019e0: 6974 696e 6720 7175 6575 6554 720b 0000  iting queueTr...
-000019f0: 004e 2911 7257 0000 0072 6200 0000 7254  .N).rW...rb...rT
-00001a00: 0000 00da 046c 6973 7472 5a00 0000 da04  .....listrZ.....
-00001a10: 6b65 7973 da03 6765 74da 0572 616e 6765  keys..get..range
-00001a20: da03 6c65 6e72 0300 0000 da09 6361 6e63  ..lenr......canc
-00001a30: 656c 6c65 64da 0474 696d 65da 1170 726f  elled..time..pro
-00001a40: 6365 7373 5f74 696d 6573 7461 6d70 725d  cess_timestampr]
-00001a50: 0000 0072 0400 0000 725c 0000 0072 5000  ...r....r\...rP.
-00001a60: 0000 2906 721f 0000 0072 7d00 0000 da01  ..).r....r}.....
-00001a70: 6bda 0a67 726f 7570 5f6a 6f62 73da 015f  k..group_jobs.._
-00001a80: da03 6a6f 6272 2000 0000 7220 0000 0072  ..jobr ...r ...r
-00001a90: 2100 0000 da0e 5f63 6c65 6172 5f77 6169  !....._clear_wai
-00001aa0: 7469 6e67 d200 0000 731e 0000 000a 0308  ting....s.......
-00001ab0: 010e 0108 010c 0110 0108 0106 010a 0106  ................
-00001ac0: 010e 0110 020a 0102 f622 fe7a 1451 7565  .........".z.Que
-00001ad0: 7565 2e5f 636c 6561 725f 7761 6974 696e  ue._clear_waitin
-00001ae0: 6754 7278 0000 0072 6a00 0000 6301 0000  gTrx...rj...c...
-00001af0: 0000 0000 0001 0000 0005 0000 0004 0000  ................
-00001b00: 0043 0000 0173 5000 0000 7c00 a000 a100  .C...sP...|.....
-00001b10: 0100 7401 7c00 6a02 a003 a100 8301 7d02  ..t.|.j.......}.
-00001b20: 7c02 4400 5d10 7d03 7c00 6a02 a004 7c03  |.D.].}.|.j...|.
-00001b30: a101 7d04 7c04 6401 7501 721d 7c04 a005  ..}.|.d.u.r.|...
-00001b40: a100 0100 710d 7c01 7226 7c00 a006 a100  ....q.|.r&|.....
-00001b50: 0100 6401 5300 6401 5300 2902 7a2d 5374  ..d.S.d.S.).z-St
-00001b60: 6f70 2061 6e64 2072 656d 6f76 6520 616c  op and remove al
-00001b70: 6c20 7275 6e6e 696e 6720 616e 6420 7761  l running and wa
-00001b80: 6974 696e 6720 6a6f 6273 2e4e 2907 7288  iting jobs.N).r.
-00001b90: 0000 0072 7c00 0000 725b 0000 0072 7d00  ...r|...r[...r}.
-00001ba0: 0000 727e 0000 0072 2c00 0000 726a 0000  ..r~...r,...rj..
-00001bb0: 0029 0572 1f00 0000 726a 0000 0072 7d00  .).r....rj...r}.
-00001bc0: 0000 7284 0000 0072 8700 0000 7220 0000  ..r....r....r ..
-00001bd0: 0072 2000 0000 7221 0000 0072 7900 0000  .r ...r!...ry...
-00001be0: e400 0000 7314 0000 0008 030e 0208 010c  ....s...........
-00001bf0: 0108 0108 0102 8004 020c 0104 ff7a 0f51  .............z.Q
-00001c00: 7565 7565 2e5f 7374 6f70 5f61 6c6c 6301  ueue._stop_allc.
-00001c10: 0000 0000 0000 0000 0000 0001 0000 0001  ................
-00001c20: 0000 0043 0000 01f3 0400 0000 7c00 5300  ...C........|.S.
-00001c30: 722f 0000 0072 2000 0000 7226 0000 0072  r/...r ...r&...r
-00001c40: 2000 0000 7220 0000 0072 2100 0000 da09   ...r ...r!.....
-00001c50: 5f5f 656e 7465 725f 5ff2 0000 00f3 0200  __enter__.......
-00001c60: 0000 0401 7a0f 5175 6575 652e 5f5f 656e  ....z.Queue.__en
-00001c70: 7465 725f 5f63 0100 0000 0000 0000 0000  ter__c..........
-00001c80: 0000 0200 0000 0200 0000 4700 0001 7272  ..........G...rr
-00001c90: 0000 0072 2f00 0000 7273 0000 0029 0272  ...r/...rs...).r
-00001ca0: 1f00 0000 7211 0000 0072 2000 0000 7220  ....r....r ...r 
-00001cb0: 0000 0072 2100 0000 da08 5f5f 6578 6974  ...r!.....__exit
-00001cc0: 5f5f f500 0000 7275 0000 007a 0e51 7565  __....ru...z.Que
-00001cd0: 7565 2e5f 5f65 7869 745f 5f63 0100 0000  ue.__exit__c....
-00001ce0: 0000 0000 0000 0000 0100 0000 0100 0000  ................
-00001cf0: 4300 0001 7289 0000 0072 2f00 0000 7220  C...r....r/...r 
-00001d00: 0000 0072 2600 0000 7220 0000 0072 2000  ...r&...r ...r .
-00001d10: 0000 7221 0000 00da 085f 5f69 7465 725f  ..r!.....__iter_
-00001d20: 5ff8 0000 0072 8b00 0000 7a0e 5175 6575  _....r....z.Queu
-00001d30: 652e 5f5f 6974 6572 5f5f 720c 0000 0063  e.__iter__r....c
-00001d40: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00001d50: 0200 0000 4300 0001 7318 0000 007c 00a0  ....C...s....|..
-00001d60: 00a1 007d 017c 0164 0075 0072 0a74 0182  ...}.|.d.u.r.t..
-00001d70: 017c 0153 0072 2f00 0000 2902 da07 6465  .|.S.r/...)...de
-00001d80: 7175 6575 65da 0d53 746f 7049 7465 7261  queue..StopItera
-00001d90: 7469 6f6e 2902 721f 0000 0072 8700 0000  tion).r....r....
-00001da0: 7220 0000 0072 2000 0000 7221 0000 00da  r ...r ...r!....
-00001db0: 085f 5f6e 6578 745f 5ffb 0000 0073 0800  .__next__....s..
-00001dc0: 0000 0801 0801 0401 0401 7a0e 5175 6575  ..........z.Queu
-00001dd0: 652e 5f5f 6e65 7874 5f5f 6301 0000 0000  e.__next__c.....
-00001de0: 0000 0000 0000 000b 0000 000e 0000 0043  ...............C
-00001df0: 0000 0173 6403 0000 7c00 6a00 9001 8fa3  ...sd...|.j.....
-00001e00: 0100 9001 7a89 9001 7a68 7c00 6a01 7216  ....z...zh|.j.r.
-00001e10: 7c00 a002 a100 7216 7c00 a003 a100 0100  |.....r.|.......
-00001e20: 9001 6e59 7c00 6a04 a005 a100 4400 5d0c  ..nY|.j.....D.].
-00001e30: 5c02 7d01 7d02 7c02 a006 a100 7227 7c02  \.}.}.|.....r'|.
-00001e40: a003 a100 0100 711b 7407 7c00 6a04 a008  ......q.t.|.j...
-00001e50: a100 8301 4400 9001 5d01 7d01 7c00 6a04  ....D...].}.|.j.
-00001e60: 7c01 1900 7d02 7c02 a009 a100 9001 7331  |...}.|.......s1
-00001e70: 7c02 a00a a100 9001 7331 7c02 a00b a100  |.......s1|.....
-00001e80: 0100 7c02 6a0c 7376 7a19 7c00 6a0d a00e  ..|.j.svz.|.j...
-00001e90: 7c02 6a0f a101 5c04 7d03 7d04 7d05 7d06  |.j...\.}.}.}.}.
-00001ea0: 7c03 7c02 5f10 7c04 7c02 5f11 7c05 7c02  |.|._.|.|._.|.|.
-00001eb0: 5f12 7c06 7c02 5f13 5700 6e14 0400 7414  _.|.|._.W.n...t.
-00001ec0: 7975 0100 0100 0100 7415 7416 6401 a017  yu......t.t.d...
-00001ed0: 7c02 6a0f a101 8301 8301 7c02 5f18 5900  |.j.......|._.Y.
-00001ee0: 6e01 7700 7c00 6a19 6402 7501 729b 7a08  n.w.|.j.d.u.r.z.
-00001ef0: 7c00 a019 7c02 a101 7c02 5f1a 5700 6e17  |...|...|._.W.n.
-00001f00: 0400 7416 799a 0100 7d07 0100 7a0b 7415  ..t.y...}...z.t.
-00001f10: 7c07 8301 7c02 5f1a 5700 5900 6402 7d07  |...|._.W.Y.d.}.
-00001f20: 7e07 6e05 6402 7d07 7e07 7701 7700 741b  ~.n.d.}.~.w.w.t.
-00001f30: a01b a100 7c02 5f1c 741d a01e 6403 7c02  ....|._.t...d.|.
-00001f40: 6a0f a102 0100 7c00 6a1f 73b1 7420 7c00  j.....|.j.s.t |.
-00001f50: 6a21 7c02 8302 0100 6e07 7c00 0400 6a22  j!|.....n.|...j"
-00001f60: 6404 3700 0200 5f22 7c00 6a04 7c01 3d00  d.7..._"|.j.|.=.
-00001f70: 7c02 6a23 6402 7501 9001 7231 7c02 6a23  |.j#d.u...r1|.j#
-00001f80: 7c00 6a24 6b03 9001 7231 7c00 6a25 a026  |.j$k...r1|.j%.&
-00001f90: 7c02 6a23 a101 7d08 7c08 6402 7501 9001  |.j#..}.|.d.u...
-00001fa0: 7231 6402 7d09 7c02 6a12 7d0a 7427 7c08  r1d.}.|.j.}.t'|.
-00001fb0: 8301 6405 6b04 9001 7215 7428 7c08 8301  ..d.k...r.t(|...
-00001fc0: 7d09 7c0a 6405 6b02 73ec 7c09 6a29 73ed  }.|.d.k.s.|.j)s.
-00001fd0: 6e28 6406 7c09 5f0c 7c0a 7c09 5f12 6407  n(d.|._.|.|._.d.
-00001fe0: a017 7c02 6a0f 7c0a a102 7c09 5f11 741b  ..|.j.|...|._.t.
-00001ff0: a01b a100 7c09 5f1c 7c00 6a1f 9001 730b  ....|._.|.j...s.
-00002000: 7420 7c00 6a21 7c09 8302 0100 6e07 7c00  t |.j!|.....n.|.
-00002010: 0400 6a22 6404 3700 0200 5f22 6402 7d09  ..j"d.7..._"d.}.
-00002020: 71da 7427 7c08 8301 6405 6b02 9001 7221  q.t'|...d.k...r!
-00002030: 7c00 6a25 7c02 6a23 3d00 7c09 6402 7501  |.j%|.j#=.|.d.u.
-00002040: 9001 7231 7c09 7c00 6a04 7c09 6a0f 3c00  ..r1|.|.j.|.j.<.
-00002050: 7c00 a02a 7c09 a101 0100 712f 7427 7c00  |..*|.....q/t'|.
-00002060: 6a25 7c00 6a24 1900 8301 6405 6b04 9001  j%|.j$....d.k...
-00002070: 726f 7c00 6a2b 7c00 a02c a100 1800 6405  ro|.j+|..,....d.
-00002080: 6b04 9001 726f 7428 7c00 6a25 7c00 6a24  k...rot(|.j%|.j$
-00002090: 1900 8301 7d02 7c02 7c00 6a04 7c02 6a0f  ....}.|.|.j.|.j.
-000020a0: 3c00 7c00 a02a 7c02 a101 0100 7427 7c00  <.|..*|.....t'|.
-000020b0: 6a25 7c00 6a24 1900 8301 6405 6b04 9001  j%|.j$....d.k...
-000020c0: 726f 7c00 6a2b 7c00 a02c a100 1800 6405  ro|.j+|..,....d.
-000020d0: 6b04 9001 7347 5700 6e0f 0100 0100 0100  k...sGW.n.......
-000020e0: 7c00 a003 a100 0100 741d a011 742d a02e  |.......t...t-..
-000020f0: a100 a101 0100 5900 5700 741d a01e 6408  ......Y.W.t...d.
-00002100: 7c00 a02f a100 7c00 a02c a100 7c00 a030  |../..|..,..|..0
-00002110: a100 a104 0100 6e0f 741d a01e 6408 7c00  ......n.t...d.|.
-00002120: a02f a100 7c00 a02c a100 7c00 a030 a100  ./..|..,..|..0..
-00002130: a104 0100 7700 5700 6402 0400 0400 8303  ....w.W.d.......
-00002140: 0100 6402 5300 3100 9001 73ab 7701 0100  ..d.S.1...s.w...
-00002150: 0100 0100 5900 0100 6402 5300 2909 7a35  ....Y...d.S.).z5
-00002160: 5573 6564 2069 6e74 6572 6e61 6c6c 793b  Used internally;
-00002170: 206d 616e 6167 6573 2074 6865 2071 7565   manages the que
-00002180: 7565 2073 7973 7465 6d20 6f70 6572 6174  ue system operat
-00002190: 696f 6e73 2e7a 367b 7d0a 0a4e 6f20 6461  ions.z6{}..No da
-000021a0: 7461 2066 6f72 2064 6174 613b 2069 7420  ta for data; it 
-000021b0: 6d61 7920 6861 7665 2065 7869 7465 6420  may have exited 
-000021c0: 756e 6578 7065 6374 6564 6c79 2e4e 7a11  unexpectedly.Nz.
-000021d0: 436f 6d70 6c65 7465 6420 6a6f 623a 2025  Completed job: %
-000021e0: 6472 0b00 0000 7201 0000 0054 7a42 736b  dr....r....TzBsk
-000021f0: 6970 5f6f 6e5f 6772 6f75 705f 6572 726f  ip_on_group_erro
-00002200: 7220 3d20 5472 7565 2061 6e64 2070 7265  r = True and pre
-00002210: 6365 6469 6e67 2064 6174 6120 287b 7d29  ceding data ({})
-00002220: 2065 7869 7420 636f 6465 2069 7320 7b7d   exit code is {}
-00002230: 7a24 7761 6974 696e 673d 2564 3b20 776f  z$waiting=%d; wo
-00002240: 726b 696e 673d 2564 3b20 6669 6e69 7368  rking=%d; finish
-00002250: 6564 3d25 642e 2931 7254 0000 0072 6500  ed=%d.)1rT...re.
-00002260: 0000 da07 6973 5f69 646c 6572 2c00 0000  ....is_idler,...
-00002270: 725b 0000 00da 0569 7465 6d73 da0a 6973  r[.....items..is
-00002280: 5f65 7870 6972 6564 727c 0000 0072 7d00  _expiredr|...r}.
-00002290: 0000 7230 0000 00da 0c69 735f 7072 6f63  ..r0.....is_proc
-000022a0: 6573 7365 64da 046a 6f69 6e72 8100 0000  essed..joinr....
-000022b0: 7261 0000 00da 0370 6f70 da03 6964 78da  ra.....pop..idx.
-000022c0: 0672 6573 756c 74da 0565 7272 6f72 da08  .result..error..
-000022d0: 6578 6974 636f 6465 da10 6669 6e69 7368  exitcode..finish
-000022e0: 5f74 696d 6573 7461 6d70 da08 4b65 7945  _timestamp..KeyE
-000022f0: 7272 6f72 724c 0000 00da 0945 7863 6570  rrorrL.....Excep
-00002300: 7469 6f6e da06 666f 726d 6174 5a0d 6578  tion..formatZ.ex
-00002310: 6365 7074 696f 6e5f 7478 7472 5200 0000  ception_txtrR...
-00002320: da0f 6361 6c6c 6261 636b 5f72 6573 756c  ..callback_resul
-00002330: 7472 8200 0000 7283 0000 0072 5700 0000  tr....r....rW...
-00002340: 7262 0000 0072 5d00 0000 7204 0000 0072  rb...r]...r....r
-00002350: 5c00 0000 7250 0000 00da 0567 726f 7570  \...rP.....group
-00002360: 723c 0000 0072 5a00 0000 727e 0000 0072  r<...rZ...r~...r
-00002370: 8000 0000 7203 0000 00da 1373 6b69 705f  ....r......skip_
-00002380: 6f6e 5f67 726f 7570 5f65 7272 6f72 da0a  on_group_error..
-00002390: 5f73 7461 7274 5f6a 6f62 7247 0000 00da  _start_jobrG....
-000023a0: 0e5f 636f 756e 745f 776f 726b 696e 67da  ._count_working.
-000023b0: 0974 7261 6365 6261 636b da0a 666f 726d  .traceback..form
-000023c0: 6174 5f65 7863 da0e 5f63 6f75 6e74 5f77  at_exc.._count_w
-000023d0: 6169 7469 6e67 da0f 5f63 6f75 6e74 5f66  aiting.._count_f
-000023e0: 696e 6973 6865 6429 0b72 1f00 0000 5a06  inished).r....Z.
-000023f0: 6a6f 625f 6964 7287 0000 00da 0673 7464  job_idr......std
-00002400: 6f75 74da 0673 7464 6572 7272 9a00 0000  out..stderrr....
-00002410: da09 7469 6d65 7374 616d 70da 0265 7872  ..timestamp..exr
-00002420: 8500 0000 5a08 6e65 7874 5f6a 6f62 5a0f  ....Z.next_jobZ.
-00002430: 7061 7265 6e74 5f65 7869 7463 6f64 6572  parent_exitcoder
-00002440: 2000 0000 7220 0000 0072 2100 0000 7264   ...r ...r!...rd
-00002450: 0000 0001 0100 0073 d800 0000 0a04 0801  .......s........
-00002460: 0e01 0c01 1203 0801 0801 0280 1402 0a01  ................
-00002470: 1402 0801 0601 0201 0c06 02fb 0201 0201  ................
-00002480: 0201 0201 0602 0601 0601 0a01 0c01 0201  ................
-00002490: 0201 0201 0801 02fe 0aff 02ff 0a08 0201  ................
-000024a0: 1001 0201 0201 0aff 1603 0880 02fd 0a05  ................
-000024b0: 0e02 0602 0e01 0e02 0802 0c03 0e01 0602  ................
-000024c0: 0401 04ff 0a03 0401 0601 0e01 0801 0803  ................
-000024d0: 0401 02ff 0203 0602 0601 0202 0201 0401  ................
-000024e0: 0201 02fe 04fe 0a07 0801 0201 0401 0201  ................
-000024f0: 06fe 0e05 0401 0201 0e02 0a01 0a02 0c01  ................
-00002500: 0a01 0280 1603 1401 1002 0c01 0a01 16fb  ................
-00002510: 1401 0480 0605 0801 1001 0280 0402 0201  ................
-00002520: 0601 0601 0601 0afc 0201 0601 0601 0601  ................
-00002530: 08fc 2491 7a0c 5175 6575 652e 5f70 756c  ..$.z.Queue._pul
-00002540: 7365 6301 0000 0000 0000 0000 0000 0001  sec.............
-00002550: 0000 0004 0000 0043 0000 0173 1800 0000  .......C...s....
-00002560: 7400 6401 6402 8400 7c00 6a01 a002 a100  t.d.d...|.j.....
-00002570: 4400 8301 8301 5300 2903 7a1f 4765 7420  D.....S.).z.Get 
-00002580: 7468 6520 6e75 6d62 6572 206f 6620 7065  the number of pe
-00002590: 6e64 696e 6720 6a6f 6273 2e63 0100 0000  nding jobs.c....
-000025a0: 0000 0000 0000 0000 0300 0000 0300 0000  ................
-000025b0: 7300 0001 731c 0000 0081 007c 005d 095c  s...s......|.].\
-000025c0: 027d 017d 0274 007c 0283 0156 0001 0071  .}.}.t.|...V...q
-000025d0: 0264 0053 0072 2f00 0000 2901 7280 0000  .d.S.r/...).r...
-000025e0: 0029 03da 022e 3072 8600 0000 da01 7672  .)....0r......vr
-000025f0: 2000 0000 7220 0000 0072 2100 0000 da09   ...r ...r!.....
-00002600: 3c67 656e 6578 7072 3e7d 0100 0073 0400  <genexpr>}...s..
-00002610: 0000 0280 1a00 7a27 5175 6575 652e 5f63  ......z'Queue._c
-00002620: 6f75 6e74 5f77 6169 7469 6e67 2e3c 6c6f  ount_waiting.<lo
-00002630: 6361 6c73 3e2e 3c67 656e 6578 7072 3e29  cals>.<genexpr>)
-00002640: 03da 0373 756d 725a 0000 0072 9200 0000  ...sumrZ...r....
-00002650: 7226 0000 0072 2000 0000 7220 0000 0072  r&...r ...r ...r
-00002660: 2100 0000 72a6 0000 007b 0100 0073 0200  !...r....{...s..
-00002670: 0000 1802 7a14 5175 6575 652e 5f63 6f75  ....z.Queue._cou
-00002680: 6e74 5f77 6169 7469 6e67 6301 0000 0000  nt_waitingc.....
-00002690: 0000 0000 0000 0001 0000 0002 0000 0043  ...............C
-000026a0: 0000 01f3 0a00 0000 7400 7c00 6a01 8301  ........t.|.j...
-000026b0: 5300 2901 7a1f 4765 7420 7468 6520 6e75  S.).z.Get the nu
-000026c0: 6d62 6572 206f 6620 7275 6e6e 696e 6720  mber of running 
-000026d0: 6a6f 6273 2e29 0272 8000 0000 725b 0000  jobs.).r....r[..
-000026e0: 0072 2600 0000 7220 0000 0072 2000 0000  .r&...r ...r ...
-000026f0: 7221 0000 0072 a300 0000 7f01 0000 f302  r!...r..........
-00002700: 0000 000a 027a 1451 7565 7565 2e5f 636f  .....z.Queue._co
-00002710: 756e 745f 776f 726b 696e 6763 0100 0000  unt_workingc....
-00002720: 0000 0000 0000 0000 0100 0000 0200 0000  ................
-00002730: 4300 0001 72b0 0000 0029 017a 2147 6574  C...r....).z!Get
-00002740: 2074 6865 206e 756d 6265 7220 6f66 2063   the number of c
-00002750: 6f6d 706c 6574 6564 206a 6f62 732e 2902  ompleted jobs.).
-00002760: 7280 0000 0072 5c00 0000 7226 0000 0072  r....r\...r&...r
-00002770: 2000 0000 7220 0000 0072 2100 0000 72a7   ...r ...r!...r.
-00002780: 0000 0083 0100 0072 b100 0000 7a15 5175  .......r....z.Qu
-00002790: 6575 652e 5f63 6f75 6e74 5f66 696e 6973  eue._count_finis
-000027a0: 6865 6463 0100 0000 0000 0000 0000 0000  hedc............
-000027b0: 0100 0000 0400 0000 4300 0001 730e 0000  ........C...s...
-000027c0: 007c 006a 0064 0164 0164 028d 0253 0029  .|.j.d.d.d...S.)
-000027d0: 037a 3c47 6574 2074 6865 206e 756d 6265  .z<Get the numbe
-000027e0: 7220 6f66 2075 6e66 696e 6973 6865 6420  r of unfinished 
-000027f0: 6a6f 6273 2028 692e 652e 2c20 7761 6974  jobs (i.e., wait
-00002800: 696e 6720 2b20 776f 726b 696e 6729 2e54  ing + working).T
-00002810: 2902 da07 7761 6974 696e 67da 0777 6f72  )...waiting..wor
-00002820: 6b69 6e67 a901 da04 7369 7a65 7226 0000  king....sizer&..
-00002830: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-00002840: da10 5f63 6f75 6e74 5f72 656d 6169 6e69  .._count_remaini
-00002850: 6e67 8701 0000 7277 0000 007a 1651 7565  ng....rw...z.Que
-00002860: 7565 2e5f 636f 756e 745f 7265 6d61 696e  ue._count_remain
-00002870: 696e 67a9 0372 b200 0000 72b3 0000 00da  ing..r....r.....
-00002880: 0866 696e 6973 6865 6472 b200 0000 72b3  .finishedr....r.
-00002890: 0000 0072 b800 0000 fa09 6c69 7374 5b69  ...r......list[i
-000028a0: 6e74 5d63 0100 0000 0000 0000 0300 0000  nt]c............
-000028b0: 0700 0000 0800 0000 4300 0001 739c 0000  ........C...s...
-000028c0: 0069 007d 0464 017d 057a 3a74 007c 017c  .i.}.d.}.z:t.|.|
-000028d0: 027c 0367 0383 017d 067c 0664 026b 0372  .|.g...}.|.d.k.r
-000028e0: 1e7c 0664 036b 0272 1964 045c 037d 017d  .|.d.k.r.d.\.}.}
-000028f0: 027d 037c 006a 01a0 02a1 007d 057c 0172  .}.|.j.....}.|.r
-00002900: 267c 00a0 03a1 007c 0464 053c 007c 0272  &|.....|.d.<.|.r
-00002910: 2e7c 00a0 04a1 007c 0464 063c 007c 0372  .|.....|.d.<.|.r
-00002920: 367c 00a0 05a1 007c 0464 073c 0057 007c  6|.....|.d.<.W.|
-00002930: 0572 3e7c 006a 01a0 06a1 0001 006e 097c  .r>|.j.......n.|
-00002940: 0572 477c 006a 01a0 06a1 0001 0077 0077  .rG|.j.......w.w
-00002950: 0074 077c 04a0 08a1 0083 0153 0029 0861  .t.|.......S.).a
-00002960: 2402 0000 5265 7475 726e 7320 7468 6520  $...Returns the 
-00002970: 6e75 6d62 6572 206f 6620 6a6f 6273 2069  number of jobs i
-00002980: 6e20 7468 6520 636f 7272 6573 706f 6e64  n the correspond
-00002990: 696e 6720 7175 6575 6528 7329 2e0a 0a20  ing queue(s)... 
-000029a0: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
-000029b0: 2020 2020 2020 2020 2077 6169 7469 6e67           waiting
-000029c0: 3a20 696e 636c 7564 6520 6a6f 6273 2069  : include jobs i
-000029d0: 6e20 7468 6520 7761 6974 696e 6720 7175  n the waiting qu
-000029e0: 6575 653f 0a20 2020 2020 2020 2020 2020  eue?.           
-000029f0: 2020 2020 202d 2041 6363 6570 7473 3a20       - Accepts: 
-00002a00: 626f 6f6c 0a20 2020 2020 2020 2020 2020  bool.           
-00002a10: 2020 2020 202d 2044 6566 6175 6c74 3a20       - Default: 
-00002a20: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
-00002a30: 2020 776f 726b 696e 673a 2069 6e63 6c75    working: inclu
-00002a40: 6465 206a 6f62 7320 696e 2074 6865 2077  de jobs in the w
-00002a50: 6f72 6b69 6e67 2074 6162 6c65 3f0a 2020  orking table?.  
-00002a60: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00002a70: 4163 6365 7074 733a 2062 6f6f 6c0a 2020  Accepts: bool.  
-00002a80: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
-00002a90: 4465 6661 756c 743a 2046 616c 7365 0a20  Default: False. 
-00002aa0: 2020 2020 2020 2020 2020 2066 696e 6973             finis
-00002ab0: 6865 643a 2069 6e63 6c75 6465 206a 6f62  hed: include job
-00002ac0: 7320 696e 2074 6865 2063 6f6d 706c 6574  s in the complet
-00002ad0: 6564 2071 7565 7565 3f0a 2020 2020 2020  ed queue?.      
-00002ae0: 2020 2020 2020 2020 2020 2d20 4163 6365            - Acce
-00002af0: 7074 733a 2062 6f6f 6c0a 2020 2020 2020  pts: bool.      
-00002b00: 2020 2020 2020 2020 2020 2d20 4465 6661            - Defa
-00002b10: 756c 743a 2046 616c 7365 0a0a 2020 2020  ult: False..    
-00002b20: 2020 2020 4e6f 7465 3a20 7768 656e 2061      Note: when a
-00002b30: 6c6c 2061 7265 2046 616c 7365 2c20 616c  ll are False, al
-00002b40: 6c20 6a6f 6273 2061 7265 2063 6f75 6e74  l jobs are count
-00002b50: 6564 2028 6465 6661 756c 7429 2e0a 0a20  ed (default)... 
-00002b60: 2020 2020 2020 2052 6574 7572 6e73 3a0a         Returns:.
-00002b70: 2020 2020 2020 2020 2020 2020 696e 740a              int.
-00002b80: 2020 2020 2020 2020 4672 0b00 0000 7201          Fr....r.
-00002b90: 0000 0029 0354 5454 72b2 0000 0072 b300  ...).TTTr....r..
-00002ba0: 0000 72b8 0000 0029 0972 af00 0000 7254  ..r....).r....rT
-00002bb0: 0000 00da 0761 6371 7569 7265 72a6 0000  .....acquirer...
-00002bc0: 0072 a300 0000 72a7 0000 00da 0772 656c  .r....r......rel
-00002bd0: 6561 7365 727c 0000 00da 0676 616c 7565  easer|.....value
-00002be0: 7329 0772 1f00 0000 72b2 0000 0072 b300  s).r....r....r..
-00002bf0: 0000 72b8 0000 00da 0663 6f75 6e74 735a  ..r......countsZ
-00002c00: 0969 735f 6c6f 636b 6564 5a08 746f 5f74  .is_lockedZ.to_t
-00002c10: 616c 6c79 7220 0000 0072 2000 0000 7221  allyr ...r ...r!
-00002c20: 0000 00da 065f 7369 7a65 738b 0100 0073  ....._sizes....s
-00002c30: 2c00 0000 041a 0402 0202 0e01 0801 0801  ,...............
-00002c40: 0a01 0a02 0402 0c01 0401 0c01 0401 0c01  ................
-00002c50: 0280 0402 0a01 0280 04ff 0c01 02ff 0c03  ................
-00002c60: 7a0c 5175 6575 652e 5f73 697a 6573 6301  z.Queue._sizesc.
-00002c70: 0000 0000 0000 0000 0000 0001 0000 0002  ................
-00002c80: 0000 0043 0000 0173 0800 0000 7c00 a000  ...C...s....|...
-00002c90: a100 5300 722f 0000 0072 b400 0000 7226  ..S.r/...r....r&
-00002ca0: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00002cb0: 0000 da07 5f5f 6c65 6e5f 5fbd 0100 0073  ....__len__....s
-00002cc0: 0200 0000 0801 7a0d 5175 6575 652e 5f5f  ......z.Queue.__
-00002cd0: 6c65 6e5f 5f63 0100 0000 0000 0000 0300  len__c..........
-00002ce0: 0000 0400 0000 0600 0000 4300 0001 7314  ..........C...s.
-00002cf0: 0000 0074 007c 006a 017c 017c 027c 0364  ...t.|.j.|.|.|.d
-00002d00: 018d 0383 0153 0029 0261 f602 0000 4765  .....S.).a....Ge
-00002d10: 7420 7468 6520 6e75 6d62 6572 206f 6620  t the number of 
-00002d20: 6a6f 6273 2069 6e20 7468 6520 7175 6575  jobs in the queu
-00002d30: 6520 696e 2073 7461 7465 3a20 7761 6974  e in state: wait
-00002d40: 696e 672c 2077 6f72 6b69 6e67 2c20 616e  ing, working, an
-00002d50: 642f 6f72 2066 696e 6973 6865 642e 0a0a  d/or finished...
-00002d60: 2020 2020 2020 2020 4966 206e 6f20 6f70          If no op
-00002d70: 7469 6f6e 7320 6172 6520 6769 7665 6e2c  tions are given,
-00002d80: 2074 6865 2074 6f74 616c 206e 756d 6265   the total numbe
-00002d90: 7220 6f66 206a 6f62 7320 696e 2074 6865  r of jobs in the
-00002da0: 2071 7565 7565 2069 7320 7265 7475 726e   queue is return
-00002db0: 6564 2e0a 0a20 2020 2020 2020 2041 7267  ed...        Arg
-00002dc0: 733a 0a20 2020 2020 2020 2020 2020 2077  s:.            w
-00002dd0: 6169 7469 6e67 3a20 696e 636c 7564 6520  aiting: include 
-00002de0: 7761 6974 696e 6720 6a6f 6273 2e0a 2020  waiting jobs..  
-00002df0: 2020 2020 2020 2020 2020 776f 726b 696e            workin
-00002e00: 673a 2069 6e63 6c75 6465 2077 6f72 6b69  g: include worki
-00002e10: 6e67 206a 6f62 732e 0a20 2020 2020 2020  ng jobs..       
-00002e20: 2020 2020 2066 696e 6973 6865 643a 2069       finished: i
-00002e30: 6e63 6c75 6465 2066 696e 6973 6865 6420  nclude finished 
-00002e40: 6a6f 6273 2e0a 0a20 2020 2020 2020 2045  jobs...        E
-00002e50: 7861 6d70 6c65 733a 0a20 2020 2020 2020  xamples:.       
-00002e60: 2020 2020 203e 3e3e 2066 726f 6d20 7070       >>> from pp
-00002e70: 7175 6575 6520 696d 706f 7274 2051 7565  queue import Que
-00002e80: 7565 0a20 2020 2020 2020 2020 2020 202e  ue.            .
-00002e90: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-00002ea0: 3e3e 2064 6566 2061 6464 5f6e 756d 7328  >> def add_nums(
-00002eb0: 783a 2069 6e74 2c20 793a 2069 6e74 2920  x: int, y: int) 
-00002ec0: 2d3e 2069 6e74 3a0a 2020 2020 2020 2020  -> int:.        
-00002ed0: 2020 2020 2e2e 2e20 2020 2020 7265 7475      ...     retu
-00002ee0: 726e 2078 202b 2079 0a20 2020 2020 2020  rn x + y.       
-00002ef0: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00002f00: 2020 2020 203e 3e3e 2077 6974 6820 5175       >>> with Qu
-00002f10: 6575 6528 2920 6173 2071 7565 7565 3a0a  eue() as queue:.
-00002f20: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-00002f30: 2020 2020 666f 7220 6920 696e 2072 616e      for i in ran
-00002f40: 6765 2835 293a 0a20 2020 2020 2020 2020  ge(5):.         
-00002f50: 2020 202e 2e2e 2020 2020 2020 2020 205f     ...         _
-00002f60: 203d 2071 7565 7565 2e65 6e71 7565 7565   = queue.enqueue
-00002f70: 2861 6464 5f6e 756d 732c 2061 7267 733d  (add_nums, args=
-00002f80: 5b69 2c20 3130 305d 290a 2020 2020 2020  [i, 100]).      
-00002f90: 2020 2020 2020 2e2e 2e20 2020 2020 2020        ...       
-00002fa0: 2020 7072 696e 7428 7175 6575 652e 7369    print(queue.si
-00002fb0: 7a65 2829 290a 2020 2020 2020 2020 2020  ze()).          
-00002fc0: 2020 310a 2020 2020 2020 2020 2020 2020    1.            
-00002fd0: 320a 2020 2020 2020 2020 2020 2020 330a  2.            3.
-00002fe0: 2020 2020 2020 2020 2020 2020 340a 2020              4.  
-00002ff0: 2020 2020 2020 2020 2020 350a 2020 2020            5.    
-00003000: 2020 2020 72b7 0000 0029 0272 af00 0000      r....).r....
-00003010: 72be 0000 0029 0472 1f00 0000 72b2 0000  r....).r....r...
-00003020: 0072 b300 0000 72b8 0000 0072 2000 0000  .r....r....r ...
-00003030: 7220 0000 0072 2100 0000 72b5 0000 00c0  r ...r!...r.....
-00003040: 0100 0073 0200 0000 1420 7a0a 5175 6575  ...s..... z.Queu
-00003050: 652e 7369 7a65 6301 0000 0000 0000 0000  e.sizec.........
-00003060: 0000 0001 0000 0002 0000 0043 0000 0173  ...........C...s
-00003070: 1800 0000 7c00 a000 a100 6401 6b02 6f0b  ....|.....d.k.o.
-00003080: 7c00 a001 a100 6401 6b02 5300 2902 4e72  |.....d.k.S.).Nr
-00003090: 0100 0000 2902 72a6 0000 0072 a300 0000  ....).r....r....
-000030a0: 7226 0000 0072 2000 0000 7220 0000 0072  r&...r ...r ...r
-000030b0: 2100 0000 7291 0000 00e2 0100 0073 0200  !...r........s..
-000030c0: 0000 1801 7a0d 5175 6575 652e 6973 5f69  ....z.Queue.is_i
-000030d0: 646c 6563 0100 0000 0000 0000 0000 0000  dlec............
-000030e0: 0100 0000 0300 0000 4300 0001 731a 0000  ........C...s...
-000030f0: 007c 00a0 00a1 0064 016b 0470 0c7c 006a  .|.....d.k.p.|.j
-00003100: 017c 00a0 02a1 006b 0153 0029 027a 4554  .|.....k.S.).zET
-00003110: 7275 6520 6966 206d 6178 2063 6f6e 6375  rue if max concu
-00003120: 7272 656e 7420 6c69 6d69 7420 6973 2072  rrent limit is r
-00003130: 6561 6368 6564 206f 7220 6966 2074 6865  eached or if the
-00003140: 7265 2061 7265 2077 6169 7469 6e67 206a  re are waiting j
-00003150: 6f62 732e 7201 0000 0029 0372 a600 0000  obs.r....).r....
-00003160: 7247 0000 0072 a300 0000 7226 0000 0072  rG...r....r&...r
-00003170: 2000 0000 7220 0000 0072 2100 0000 da07   ...r ...r!.....
-00003180: 6973 5f62 7573 79e5 0100 0073 0200 0000  is_busy....s....
-00003190: 1a02 7a0d 5175 6575 652e 6973 5f62 7573  ..z.Queue.is_bus
-000031a0: 7963 0100 0000 0000 0000 0000 0000 0100  yc..............
-000031b0: 0000 0200 0000 4300 0001 730c 0000 007c  ......C...s....|
-000031c0: 00a0 00a1 0064 016b 0253 0029 027a 2e54  .....d.k.S.).z.T
-000031d0: 7275 6520 6966 2074 6865 7265 2061 7265  rue if there are
-000031e0: 206e 6f20 6a6f 6273 2069 6e20 7468 6520   no jobs in the 
-000031f0: 7175 6575 6520 7379 7374 656d 2e72 0100  queue system.r..
-00003200: 0000 72b4 0000 0072 2600 0000 7220 0000  ..r....r&...r ..
-00003210: 0072 2000 0000 7221 0000 00da 0869 735f  .r ...r!.....is_
-00003220: 656d 7074 79e9 0100 0073 0200 0000 0c02  empty....s......
-00003230: 7a0e 5175 6575 652e 6973 5f65 6d70 7479  z.Queue.is_empty
-00003240: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00003250: 0003 0000 0043 0000 0173 1e00 0000 6401  .....C...s....d.
-00003260: 7c00 6a00 0400 0300 6b00 6f0c 7c00 a001  |.j.....k.o.|...
-00003270: a100 6b01 5300 0200 0100 5300 2902 7a44  ..k.S.....S.).zD
-00003280: 5472 7565 2069 6620 7468 6520 6e75 6d62  True if the numb
-00003290: 6572 206f 6620 6a6f 6273 2069 6e20 7468  er of jobs in th
-000032a0: 6520 7175 6575 6520 7379 7374 656d 2069  e queue system i
-000032b0: 7320 6571 7561 6c20 746f 206d 6178 5f73  s equal to max_s
-000032c0: 697a 652e 7201 0000 0029 0272 4e00 0000  ize.r....).rN...
-000032d0: 72b5 0000 0072 2600 0000 7220 0000 0072  r....r&...r ...r
-000032e0: 2000 0000 7221 0000 00da 0769 735f 6675   ...r!.....is_fu
-000032f0: 6c6c ed01 0000 7302 0000 001e 027a 0d51  ll....s......z.Q
-00003300: 7565 7565 2e69 735f 6675 6c6c 6301 0000  ueue.is_fullc...
-00003310: 0000 0000 0000 0000 0003 0000 0004 0000  ................
-00003320: 004f 0000 01f3 1000 0000 7c00 6a00 7c01  .O........|.j.|.
-00003330: 6900 7c02 a401 8e01 5300 722f 0000 0072  i.|.....S.r/...r
-00003340: 7800 0000 a903 721f 0000 0072 1100 0000  x.....r....r....
-00003350: 7216 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
-00003360: 2100 0000 7295 0000 00f1 0100 0073 0200  !...r........s..
-00003370: 0000 1001 7a0a 5175 6575 652e 6a6f 696e  ....z.Queue.join
-00003380: 2904 da01 6eda 0774 696d 656f 7574 da07  )...n..timeout..
-00003390: 706f 6c6c 5f6d 7372 4200 0000 72c5 0000  poll_msrB...r...
-000033a0: 0072 c600 0000 da05 666c 6f61 7472 c700  .r......floatr..
-000033b0: 0000 fa0b 626f 6f6c 207c 204e 6f6e 6563  ....bool | Nonec
-000033c0: 0100 0000 0000 0000 0400 0000 0e00 0000  ................
-000033d0: 0800 0000 4300 0001 734a 0100 007c 0364  ....C...sJ...|.d
-000033e0: 0175 0073 087c 0364 026b 0172 0c7c 006a  .u.s.|.d.k.r.|.j
-000033f0: 007d 036e 0b7c 037c 006a 006b 0072 1764  .}.n.|.|.j.k.r.d
-00003400: 037d 0574 017c 0583 0182 017c 0464 0175  .}.t.|.....|.d.u
-00003410: 0072 1e7c 006a 027d 0464 017d 0664 017d  .r.|.j.}.d.}.d.}
-00003420: 0764 017d 087c 0164 026b 0172 317c 006a  .d.}.|.d.k.r1|.j
-00003430: 037d 0664 027d 0774 046a 057d 086e 087c  .}.d.}.t.j.}.n.|
-00003440: 006a 067d 067c 017d 0774 046a 077d 087c  .j.}.|.}.t.j.}.|
-00003450: 0683 007d 097c 087c 097c 0783 0273 a374  ...}.|.|.|...s.t
-00003460: 08a0 08a1 007d 0a64 017d 0b7a 537c 0472  .....}.d.}.zS|.r
-00003470: 5074 097c 0964 0464 058d 027d 0b7c 087c  Pt.|.d.d...}.|.|
-00003480: 097c 0783 0273 927c 0264 026b 0273 6174  .|...s.|.d.k.sat
-00003490: 08a0 08a1 007c 0a18 007c 026b 0072 9274  .....|...|.k.r.t
-000034a0: 08a0 0a7c 0364 061b 00a1 0101 007c 0683  ...|.d.......|..
-000034b0: 007d 0c7c 0b64 0175 0072 727c 0c7d 096e  .}.|.d.u.rr|.}.n
-000034c0: 0f7c 097c 0c18 007d 0d7c 0d64 026b 0472  .|.|...}.|.d.k.r
-000034d0: 817c 0c7d 097c 0ba0 0b7c 0da1 0101 007c  .|.}.|...|.....|
-000034e0: 087c 097c 0783 0273 927c 0264 026b 0273  .|.|...s.|.d.k.s
-000034f0: 6174 08a0 08a1 007c 0a18 007c 026b 0073  at.....|...|.k.s
-00003500: 6157 007c 0b72 997c 0ba0 0ca1 0001 007c  aW.|.r.|.......|
-00003510: 0953 007c 0b72 a27c 0ba0 0ca1 0001 0077  .S.|.r.|.......w
-00003520: 0077 007c 0953 0029 0761 5301 0000 5761  .w.|.S.).aS...Wa
-00003530: 6974 2066 6f72 206a 6f62 7320 746f 2066  it for jobs to f
-00003540: 696e 6973 682e 0a0a 2020 2020 2020 2020  inish...        
-00003550: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00003560: 2020 6e3a 2074 6865 206e 756d 6265 7220    n: the number 
-00003570: 6f66 206a 6f62 7320 746f 2077 6169 7420  of jobs to wait 
-00003580: 666f 7220 2864 6566 6175 6c74 3d30 2c20  for (default=0, 
-00003590: 616c 6c29 2e0a 2020 2020 2020 2020 2020  all)..          
-000035a0: 2020 7469 6d65 6f75 743a 2073 6563 6f6e    timeout: secon
-000035b0: 6473 2074 6f20 7761 6974 2062 6566 6f72  ds to wait befor
-000035c0: 6520 7261 6973 696e 6720 6054 696d 656f  e raising `Timeo
-000035d0: 7574 4572 726f 7260 2028 6465 6661 756c  utError` (defaul
-000035e0: 743d 302c 2069 6e64 6566 696e 6974 656c  t=0, indefinitel
-000035f0: 7929 2e0a 2020 2020 2020 2020 2020 2020  y)..            
-00003600: 706f 6c6c 5f6d 733a 206d 696c 6c69 7365  poll_ms: millise
-00003610: 636f 6e64 7320 746f 2070 6175 7365 2062  conds to pause b
-00003620: 6574 7765 656e 2063 6865 636b 7320 2864  etween checks (d
-00003630: 6566 6175 6c74 3d31 3030 292e 0a20 2020  efault=100)..   
-00003640: 2020 2020 2020 2020 2073 686f 775f 7072           show_pr
-00003650: 6f67 7265 7373 3a20 6966 2054 7275 652c  ogress: if True,
-00003660: 2070 7265 7365 6e74 2061 2070 726f 6772   present a progr
-00003670: 6573 7320 6261 722e 0a20 2020 2020 2020  ess bar..       
-00003680: 204e 7201 0000 007a 3260 706f 6c6c 5f6d   Nr....z2`poll_m
-00003690: 7360 206d 7573 7420 6265 203e 3d20 6070  s` must be >= `p
-000036a0: 7071 7565 7565 2e51 7565 7565 2e70 756c  pqueue.Queue.pul
-000036b0: 7365 5f66 7265 715f 6d73 60da 026f 7029  se_freq_ms`..op)
-000036c0: 02da 0574 6f74 616c 5a04 756e 6974 7228  ...totalZ.unitr(
-000036d0: 0000 0029 0d72 6300 0000 da0a 5661 6c75  ...).rc.....Valu
-000036e0: 6545 7272 6f72 7242 0000 0072 b600 0000  eErrorrB...r....
-000036f0: 7213 0000 00da 065f 5f6c 655f 5f72 a700  r......__le__r..
-00003700: 0000 da06 5f5f 6765 5f5f 7282 0000 0072  ....__ge__r....r
-00003710: 0a00 0000 da05 736c 6565 70da 0675 7064  ......sleep..upd
-00003720: 6174 65da 0563 6c6f 7365 290e 721f 0000  ate..close).r...
-00003730: 0072 c500 0000 72c6 0000 0072 c700 0000  .r....r....r....
-00003740: 7242 0000 00da 0365 7272 5a04 5f66 756e  rB.....errZ._fun
-00003750: 5a0d 5f74 6172 6765 745f 7661 6c75 655a  Z._target_valueZ
-00003760: 0b5f 636f 6d70 6172 6174 6f72 5a0d 6375  ._comparatorZ.cu
-00003770: 7272 656e 745f 7661 6c75 6572 2500 0000  rrent_valuer%...
-00003780: da02 7062 da09 746d 705f 7661 6c75 655a  ..pb..tmp_valueZ
-00003790: 0a64 6966 665f 7661 6c75 6572 2000 0000  .diff_valuer ...
-000037a0: 7220 0000 0072 2100 0000 726a 0000 00f4  r ...r!...rj....
-000037b0: 0100 0073 5800 0000 1010 0801 0a01 0401  ...sX...........
-000037c0: 0801 0802 0601 0402 0401 0401 0802 0601  ................
-000037d0: 0401 0801 0602 0401 0601 0602 0a02 0801  ................
-000037e0: 0402 0202 0401 0c01 0a02 1801 0e02 0602  ................
-000037f0: 0801 0601 0802 0801 0401 0a01 0af4 1801  ................
-00003800: 0280 040d 0801 0402 04fd 0a01 02ff 0403  ................
-00003810: 7a0a 5175 6575 652e 7761 6974 da04 5f6a  z.Queue.wait.._j
-00003820: 6f62 7261 0000 00fa 3464 6963 745b 696e  obra....4dict[in
-00003830: 742c 2074 7570 6c65 5b73 7472 207c 204e  t, tuple[str | N
-00003840: 6f6e 652c 2073 7472 207c 204e 6f6e 652c  one, str | None,
-00003850: 2069 6e74 2c20 666c 6f61 745d 5dfa 2974   int, float]].)t
-00003860: 7570 6c65 5b73 7472 207c 204e 6f6e 652c  uple[str | None,
-00003870: 2073 7472 207c 204e 6f6e 652c 2069 6e74   str | None, int
-00003880: 2c20 666c 6f61 745d 6302 0000 0002 0000  , float]c.......
-00003890: 0000 0000 0009 0000 000a 0000 004f 0000  .............O..
-000038a0: 0173 ba00 0000 6401 7d04 6401 7d05 7a4a  .s....d.}.d.}.zJ
-000038b0: 7a0c 7c00 6a00 7c02 6900 7c03 a401 8e01  z.|.j.|.i.|.....
-000038c0: 7d04 6402 7d06 5700 6e1d 0400 7401 792e  }.d.}.W.n...t.y.
-000038d0: 0100 7d07 0100 7a11 7402 a003 a100 7d05  ..}...z.t.....}.
-000038e0: 6403 7d06 7c00 6a04 7324 7c07 8201 5700  d.}.|.j.s$|...W.
-000038f0: 5900 6401 7d07 7e07 6e15 6401 7d07 7e07  Y.d.}.~.n.d.}.~.
-00003900: 7701 7700 5700 7405 a005 a100 7d08 7c04  w.w.W.t.....}.|.
-00003910: 7c05 7c06 7c08 6604 7c01 7c00 6a06 3c00  |.|.|.f.|.|.j.<.
-00003920: 6401 5300 5700 7405 a005 a100 7d08 7c04  d.S.W.t.....}.|.
-00003930: 7c05 7c06 7c08 6604 7c01 7c00 6a06 3c00  |.|.|.f.|.|.j.<.
-00003940: 6401 5300 7405 a005 a100 7d08 7c04 7c05  d.S.t.....}.|.|.
-00003950: 7c06 7c08 6604 7c01 7c00 6a06 3c00 7700  |.|.f.|.|.j.<.w.
-00003960: 2904 7a3f 5573 6564 2069 6e74 6572 6e61  ).z?Used interna
-00003970: 6c6c 7920 746f 2077 7261 7020 6461 7461  lly to wrap data
-00003980: 2c20 6361 7074 7572 6520 6f75 7470 7574  , capture output
-00003990: 2061 6e64 2061 6e79 2065 7863 6570 7469   and any excepti
-000039a0: 6f6e 2e4e 7201 0000 00e9 ffff ffff 2907  on.Nr.........).
-000039b0: 7214 0000 0072 9d00 0000 72a4 0000 0072  r....r....r....r
-000039c0: a500 0000 da0f 7375 7070 7265 7373 5f65  ......suppress_e
-000039d0: 7272 6f72 7372 8200 0000 7297 0000 0029  rrorsr....r....)
-000039e0: 0972 d500 0000 7261 0000 0072 1100 0000  .r....ra...r....
-000039f0: 7216 0000 0072 a800 0000 72a9 0000 0072  r....r....r....r
-00003a00: 9a00 0000 72ab 0000 0072 aa00 0000 7220  ....r....r....r 
-00003a10: 0000 0072 2000 0000 7221 0000 00da 0c5f  ...r ...r!....._
-00003a20: 6a6f 625f 7772 6170 7065 7238 0200 0073  job_wrapper8...s
-00003a30: 2a00 0000 0409 0401 0404 1001 0801 0e01  *...............
-00003a40: 0801 0401 0601 0401 0cff 0880 02fd 02ff  ................
-00003a50: 0807 1601 02fc 0803 1601 08ff 1401 7a12  ..............z.
-00003a60: 5175 6575 652e 5f6a 6f62 5f77 7261 7070  Queue._job_wrapp
-00003a70: 6572 7287 0000 0063 0200 0000 0200 0000  err....c........
-00003a80: 0000 0000 0300 0000 0600 0000 4300 0001  ............C...
-00003a90: 7356 0000 007c 006a 0074 017c 016a 0283  sV...|.j.t.|.j..
-00003aa0: 017c 006a 037c 017c 006a 0467 027c 016a  .|.j.|.|.j.g.|.j
-00003ab0: 05a2 017c 016a 0664 018d 047d 0274 07a0  ...|.j.d...}.t..
-00003ac0: 0864 027c 016a 027c 016a 09a1 0301 007c  .d.|.j.|.j.....|
-00003ad0: 02a0 0aa1 0001 0074 0ba0 0ba1 007c 015f  .......t.....|._
-00003ae0: 0c7c 027c 015f 0d64 0053 0029 034e 2904  .|.|._.d.S.).N).
-00003af0: 7240 0000 00da 0674 6172 6765 7472 1100  r@.....targetr..
-00003b00: 0000 7216 0000 007a 1973 7461 7274 696e  ..r....z.startin
-00003b10: 6720 6a6f 6220 2564 2028 6e61 6d65 3d25  g job %d (name=%
-00003b20: 7329 290e 7259 0000 0072 4c00 0000 7297  s)).rY...rL...r.
-00003b30: 0000 0072 da00 0000 7261 0000 0072 1100  ...r....ra...r..
-00003b40: 0000 7216 0000 0072 5700 0000 7262 0000  ..r....rW...rb..
-00003b50: 0072 4000 0000 7225 0000 0072 8200 0000  .r@...r%...r....
-00003b60: da0f 7374 6172 745f 7469 6d65 7374 616d  ..start_timestam
-00003b70: 70da 0969 6e6e 6572 5f6a 6f62 2903 721f  p..inner_job).r.
-00003b80: 0000 0072 8700 0000 72dd 0000 0072 2000  ...r....r....r .
-00003b90: 0000 7220 0000 0072 2100 0000 72a2 0000  ..r ...r!...r...
-00003ba0: 0052 0200 0073 1400 0000 0401 0801 0401  .R...s..........
-00003bb0: 0e01 0401 06fc 1207 0801 0a02 0a01 7a10  ..............z.
-00003bc0: 5175 6575 652e 5f73 7461 7274 5f6a 6f62  Queue._start_job
-00003bd0: 6302 0000 0002 0000 0000 0000 0003 0000  c...............
-00003be0: 0005 0000 0043 0000 0173 c400 0000 7c00  .....C...s....|.
-00003bf0: 6a00 7401 6a02 7500 720d 7c01 6a03 6401  j.t.j.u.r.|.j.d.
-00003c00: 6b04 720d 4a00 8201 7c00 a004 a100 7215  k.r.J...|.....r.
-00003c10: 7405 6402 8301 8201 7406 a006 a100 7c01  t.d.....t.....|.
-00003c20: 5f07 7c00 6a08 7c01 5f09 7c00 0400 6a0a  _.|.j.|._.|...j.
-00003c30: 6403 3700 0200 5f0a 7c00 6a0a 7c01 5f0b  d.7..._.|.j.|._.
-00003c40: 7c01 6a0c 6404 7500 7232 7c01 6a0b 7c01  |.j.d.u.r2|.j.|.
-00003c50: 5f0c 740d a00e 6405 7c01 6a0b 7c01 6a0c  _.t...d.|.j.|.j.
-00003c60: a103 0100 7c00 6a0f a010 7c01 6a11 a101  ....|.j...|.j...
-00003c70: 7d02 7c02 6404 7501 724e 7412 7c02 7c01  }.|.d.u.rNt.|.|.
-00003c80: 8302 0100 7c01 6a0b 5300 6700 7d02 7c02  ....|.j.S.g.}.|.
-00003c90: 7c00 6a0f 7c01 6a11 3c00 7412 7c00 6a0f  |.j.|.j.<.t.|.j.
-00003ca0: 7c00 6a13 1900 7c01 8302 0100 7c01 6a0b  |.j...|.....|.j.
-00003cb0: 5300 2906 6152 0100 0053 7562 6d69 7473  S.).aR...Submits
-00003cc0: 2061 206a 6f62 2069 6e74 6f20 7468 6520   a job into the 
-00003cd0: 7070 7175 6575 652e 5175 6575 6520 7379  ppqueue.Queue sy
-00003ce0: 7374 656d 2e0a 0a20 2020 2020 2020 2054  stem...        T
-00003cf0: 6872 6f77 7320 616e 2065 7863 6570 7469  hrows an excepti
-00003d00: 6f6e 2069 663a 0a20 2020 2020 2020 2020  on if:.         
-00003d10: 2020 2031 2e20 7468 6520 5175 6575 6520     1. the Queue 
-00003d20: 7573 6573 2061 2054 6872 6561 6420 6a6f  uses a Thread jo
-00003d30: 625f 7275 6e6e 6572 2061 6e64 2074 6869  b_runner and thi
-00003d40: 7320 6461 7461 2068 6173 2061 2074 696d  s data has a tim
-00003d50: 656f 7574 2028 6361 6e27 7420 7465 726d  eout (can't term
-00003d60: 696e 6174 6520 5468 7265 6164 7329 2c0a  inate Threads),.
-00003d70: 2020 2020 2020 2020 2020 2020 322e 2074              2. t
-00003d80: 6865 2051 7565 7565 206d 6178 5f73 697a  he Queue max_siz
-00003d90: 6520 7769 6c6c 2062 6520 6578 6365 6564  e will be exceed
-00003da0: 6564 2061 6674 6572 2061 6464 696e 6720  ed after adding 
-00003db0: 7468 6973 206a 6f62 2e0a 0a20 2020 2020  this job...     
-00003dc0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
-00003dd0: 2020 2020 2020 2020 5468 6520 6e75 6d62          The numb
-00003de0: 6572 206f 6620 6a6f 6273 2073 7562 6d69  er of jobs submi
-00003df0: 7474 6564 2074 6f20 7468 6520 7175 6575  tted to the queu
-00003e00: 652e 0a20 2020 2020 2020 2072 0100 0000  e..        r....
-00003e10: 7a18 4d61 7820 7175 6575 6520 7369 7a65  z.Max queue size
-00003e20: 2065 7863 6565 6465 642e 720b 0000 004e   exceeded.r....N
-00003e30: 7a18 7175 6575 696e 6720 6a6f 6220 2564  z.queuing job %d
-00003e40: 2028 6e61 6d65 3d25 7329 2914 7259 0000   (name=%s)).rY..
-00003e50: 0072 2900 0000 da06 5468 7265 6164 72c6  .r).....Threadr.
-00003e60: 0000 0072 c200 0000 da0d 4f76 6572 666c  ...r......Overfl
-00003e70: 6f77 4572 726f 7272 8200 0000 da10 7375  owErrorr......su
-00003e80: 626d 6974 5f74 696d 6573 7461 6d70 724d  bmit_timestamprM
-00003e90: 0000 00da 0371 6964 724f 0000 0072 9700  .....qidrO...r..
-00003ea0: 0000 7240 0000 0072 5700 0000 7262 0000  ..r@...rW...rb..
-00003eb0: 0072 5a00 0000 727e 0000 0072 a000 0000  .rZ...r~...r....
-00003ec0: 7204 0000 0072 3c00 0000 2903 721f 0000  r....r<...).r...
-00003ed0: 0072 8700 0000 7285 0000 0072 2000 0000  .r....r....r ...
-00003ee0: 7220 0000 0072 2100 0000 da07 5f73 7562  r ...r!....._sub
-00003ef0: 6d69 7460 0200 0073 2400 0000 1a0b 0802  mit`...s$.......
-00003f00: 0801 0a02 0802 0e01 0801 0a02 0801 1202  ................
-00003f10: 0e02 0801 0a01 0609 04f9 0c01 1204 0602  ................
-00003f20: 7a0d 5175 6575 652e 5f73 7562 6d69 74fa  z.Queue._submit.
-00003f30: 1453 6571 7565 6e63 655b 416e 795d 207c  .Sequence[Any] |
-00003f40: 204e 6f6e 65fa 1564 6963 745b 7374 722c   None..dict[str,
-00003f50: 2041 6e79 5d20 7c20 4e6f 6e65 da08 7072   Any] | None..pr
-00003f60: 696f 7269 7479 72a0 0000 0072 d900 0000  iorityr....r....
-00003f70: 72a1 0000 0063 0a00 0000 0200 0000 0000  r....c..........
-00003f80: 0000 0b00 0000 0b00 0000 4300 0001 7324  ..........C...s$
-00003f90: 0000 0074 007c 017c 027c 037c 047c 057c  ...t.|.|.|.|.|.|
-00003fa0: 067c 077c 087c 0964 018d 097d 0a7c 00a0  .|.|.|.d...}.|..
-00003fb0: 017c 0aa1 0153 0029 0261 cf02 0000 4164  .|...S.).a....Ad
-00003fc0: 6473 2061 206a 6f62 2074 6f20 7468 6520  ds a job to the 
-00003fd0: 7175 6575 652e 0a0a 2020 2020 2020 2020  queue...        
-00003fe0: 4172 6773 3a0a 2020 2020 2020 2020 2020  Args:.          
-00003ff0: 2020 6172 6773 3a0a 2020 2020 2020 2020    args:.        
-00004000: 2020 2020 6b77 6172 6773 3a0a 2020 2020      kwargs:.    
-00004010: 2020 2020 2020 2020 6e61 6d65 3a0a 2020          name:.  
-00004020: 2020 2020 2020 2020 2020 7072 696f 7269            priori
-00004030: 7479 3a0a 2020 2020 2020 2020 2020 2020  ty:.            
-00004040: 6772 6f75 703a 0a20 2020 2020 2020 2020  group:.         
-00004050: 2020 2074 696d 656f 7574 3a0a 2020 2020     timeout:.    
-00004060: 2020 2020 2020 2020 7375 7070 7265 7373          suppress
-00004070: 5f65 7272 6f72 733a 0a20 2020 2020 2020  _errors:.       
-00004080: 2020 2020 2073 6b69 705f 6f6e 5f67 726f       skip_on_gro
-00004090: 7570 5f65 7272 6f72 3a0a 0a20 2020 2020  up_error:..     
-000040a0: 2020 2045 7861 6d70 6c65 733a 0a20 2020     Examples:.   
-000040b0: 2020 2020 2020 2020 203e 3e3e 2066 726f           >>> fro
-000040c0: 6d20 7070 7175 6575 6520 696d 706f 7274  m ppqueue import
-000040d0: 2051 7565 7565 0a20 2020 2020 2020 2020   Queue.         
-000040e0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-000040f0: 2020 203e 3e3e 2064 6566 2061 6464 5f6e     >>> def add_n
-00004100: 756d 7328 783a 2069 6e74 2c20 793a 2069  ums(x: int, y: i
-00004110: 6e74 2920 2d3e 2069 6e74 3a0a 2020 2020  nt) -> int:.    
-00004120: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00004130: 7265 7475 726e 2078 202b 2079 0a20 2020  return x + y.   
-00004140: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
-00004150: 2020 2020 2020 2020 203e 3e3e 2077 6974           >>> wit
-00004160: 6820 5175 6575 6528 2920 6173 2071 7565  h Queue() as que
-00004170: 7565 3a0a 2020 2020 2020 2020 2020 2020  ue:.            
-00004180: 2e2e 2e20 2020 2020 666f 7220 6920 696e  ...     for i in
-00004190: 2072 616e 6765 2835 293a 0a20 2020 2020   range(5):.     
-000041a0: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
-000041b0: 2020 205f 203d 2071 7565 7565 2e65 6e71     _ = queue.enq
-000041c0: 7565 7565 2861 6464 5f6e 756d 732c 2061  ueue(add_nums, a
-000041d0: 7267 733d 5b69 2c20 3130 305d 290a 2020  rgs=[i, 100]).  
-000041e0: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-000041f0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
-00004200: 2020 6a6f 6273 203d 2071 7565 7565 2e63    jobs = queue.c
-00004210: 6f6c 6c65 6374 2877 6169 743d 5472 7565  ollect(wait=True
-00004220: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
-00004230: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00004240: 3e20 5b6a 6f62 2e72 6573 756c 7420 666f  > [job.result fo
-00004250: 7220 6a6f 6220 696e 206a 6f62 735d 0a20  r job in jobs]. 
-00004260: 2020 2020 2020 2020 2020 205b 3130 302c             [100,
-00004270: 2031 3031 2c20 3130 322c 2031 3033 2c20   101, 102, 103, 
-00004280: 3130 345d 0a20 2020 2020 2020 2029 0972  104].        ).r
-00004290: 1400 0000 7211 0000 0072 1600 0000 7240  ....r....r....r@
-000042a0: 0000 0072 e500 0000 72a0 0000 0072 c600  ...r....r....r..
-000042b0: 0000 72d9 0000 0072 a100 0000 2902 720c  ..r....r....).r.
-000042c0: 0000 0072 e200 0000 290b 721f 0000 0072  ...r....).r....r
-000042d0: 1400 0000 7211 0000 0072 1600 0000 7240  ....r....r....r@
-000042e0: 0000 0072 e500 0000 72a0 0000 0072 c600  ...r....r....r..
-000042f0: 0000 72d9 0000 0072 a100 0000 7287 0000  ..r....r....r...
-00004300: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-00004310: 7269 0000 0088 0200 0073 1800 0000 0228  ri.......s.....(
-00004320: 0201 0201 0201 0201 0201 0201 0201 0201  ................
-00004330: 0201 06f7 0a0c 7a0d 5175 6575 652e 656e  ......z.Queue.en
-00004340: 7175 6575 6563 0100 0000 0000 0000 0000  queuec..........
-00004350: 0000 0300 0000 0400 0000 4f00 0001 72c3  ..........O...r.
-00004360: 0000 0029 0161 0d02 0000 416c 6961 7320  ...).a....Alias 
-00004370: 666f 7220 6065 6e71 7565 7565 602e 2041  for `enqueue`. A
-00004380: 6464 7320 6120 6a6f 6220 746f 2074 6865  dds a job to the
-00004390: 2071 7565 7565 2e0a 0a20 2020 2020 2020   queue...       
-000043a0: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
-000043b0: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
-000043c0: 7070 7175 6575 6520 696d 706f 7274 2051  ppqueue import Q
-000043d0: 7565 7565 0a20 2020 2020 2020 2020 2020  ueue.           
-000043e0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-000043f0: 203e 3e3e 2064 6566 2061 6464 5f6e 756d   >>> def add_num
-00004400: 7328 783a 2069 6e74 2c20 793a 2069 6e74  s(x: int, y: int
-00004410: 2920 2d3e 2069 6e74 3a0a 2020 2020 2020  ) -> int:.      
-00004420: 2020 2020 2020 2e2e 2e20 2020 2020 7265        ...     re
-00004430: 7475 726e 2078 202b 2079 0a20 2020 2020  turn x + y.     
-00004440: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
-00004450: 2020 2020 2020 203e 3e3e 2077 6974 6820         >>> with 
-00004460: 5175 6575 6528 2920 6173 2071 7565 7565  Queue() as queue
-00004470: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00004480: 2e20 2020 2020 666f 7220 6920 696e 2072  .     for i in r
-00004490: 616e 6765 2835 293a 0a20 2020 2020 2020  ange(5):.       
-000044a0: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
-000044b0: 205f 203d 2071 7565 7565 2e70 7574 2861   _ = queue.put(a
-000044c0: 6464 5f6e 756d 732c 2061 7267 733d 5b69  dd_nums, args=[i
-000044d0: 2c20 3130 305d 290a 2020 2020 2020 2020  , 100]).        
-000044e0: 2020 2020 2e2e 2e20 2020 2020 6a6f 6273      ...     jobs
-000044f0: 203d 2071 7565 7565 2e63 6f6c 6c65 6374   = queue.collect
-00004500: 2877 6169 743d 5472 7565 290a 2020 2020  (wait=True).    
-00004510: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00004520: 2020 2020 2020 2020 3e3e 3e20 5b6a 6f62          >>> [job
-00004530: 2e72 6573 756c 7420 666f 7220 6a6f 6220  .result for job 
-00004540: 696e 206a 6f62 735d 0a20 2020 2020 2020  in jobs].       
-00004550: 2020 2020 205b 3130 302c 2031 3031 2c20       [100, 101, 
-00004560: 3130 322c 2031 3033 2c20 3130 345d 0a20  102, 103, 104]. 
-00004570: 2020 2020 2020 2029 0172 6900 0000 72c4         ).ri...r.
-00004580: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00004590: 0000 da03 7075 74be 0200 00f3 0200 0000  ....put.........
-000045a0: 1012 7a09 5175 6575 652e 7075 7429 0272  ..z.Queue.put).r
-000045b0: c600 0000 7242 0000 0072 6600 0000 7267  ....rB...rf...rg
-000045c0: 0000 0072 6800 0000 6303 0000 0003 0000  ...rh...c.......
-000045d0: 0002 0000 0009 0000 0007 0000 004f 0000  .............O..
-000045e0: 0173 3c00 0000 7c02 4400 5d14 7d07 7400  .s<...|.D.].}.t.
-000045f0: 7c01 7c07 6701 7c05 a201 7401 7c06 8301  |.|.g.|...t.|...
-00004600: 7c03 6401 8d04 7d08 7c00 a002 7c08 a101  |.d...}.|...|...
-00004610: 0100 7102 7c00 6a03 6402 7c04 6403 8d02  ..q.|.j.d.|.d...
-00004620: 5300 2904 61f6 0100 0053 7562 6d69 7473  S.).a....Submits
-00004630: 206d 616e 7920 6a6f 6273 2074 6f20 7468   many jobs to th
-00004640: 6520 7175 6575 6520 2d2d 206f 6e65 2066  e queue -- one f
-00004650: 6f72 2065 6163 6820 6974 656d 2069 6e20  or each item in 
-00004660: 7468 6520 6974 6572 6162 6c65 2e20 5761  the iterable. Wa
-00004670: 6974 7320 666f 7220 616c 6c20 746f 2066  its for all to f
-00004680: 696e 6973 682c 2074 6865 6e20 7265 7475  inish, then retu
-00004690: 726e 7320 7468 6520 7265 7375 6c74 732e  rns the results.
-000046a0: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
-000046b0: 2020 2020 2020 2020 2020 2020 6675 6e3a              fun:
-000046c0: 0a20 2020 2020 2020 2020 2020 2069 7465  .            ite
-000046d0: 7261 626c 653a 0a20 2020 2020 2020 2020  rable:.         
-000046e0: 2020 2074 696d 656f 7574 3a0a 2020 2020     timeout:.    
-000046f0: 2020 2020 2020 2020 7368 6f77 5f70 726f          show_pro
-00004700: 6772 6573 733a 0a0a 2020 2020 2020 2020  gress:..        
-00004710: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
-00004720: 2020 2020 2020 3e3e 3e20 6672 6f6d 2070        >>> from p
-00004730: 7071 7565 7565 2069 6d70 6f72 7420 5175  pqueue import Qu
-00004740: 6575 650a 2020 2020 2020 2020 2020 2020  eue.            
-00004750: 3e3e 3e20 6672 6f6d 2074 696d 6520 696d  >>> from time im
-00004760: 706f 7274 2073 6c65 6570 0a20 2020 2020  port sleep.     
-00004770: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
-00004780: 2020 2020 2020 203e 3e3e 2077 6974 6820         >>> with 
-00004790: 5175 6575 6528 2920 6173 2071 7565 7565  Queue() as queue
-000047a0: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-000047b0: 2e20 2020 2020 6a6f 6273 203d 2071 7565  .     jobs = que
-000047c0: 7565 2e6d 6170 2873 6c65 6570 2c20 5b31  ue.map(sleep, [1
-000047d0: 2c20 322c 2033 2c20 342c 2035 5d29 0a20  , 2, 3, 4, 5]). 
-000047e0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
-000047f0: 2020 2020 2020 2020 2020 203e 3e3e 206c             >>> l
-00004800: 656e 286a 6f62 7329 0a20 2020 2020 2020  en(jobs).       
-00004810: 2020 2020 2035 0a20 2020 2020 2020 20a9       5.        .
-00004820: 0472 1400 0000 7211 0000 0072 1600 0000  .r....r....r....
-00004830: 72c6 0000 0054 a902 726a 0000 0072 4200  r....T..rj...rB.
-00004840: 0000 a904 720c 0000 0072 6000 0000 72e2  ....r....r`...r.
-00004850: 0000 0072 6b00 0000 a909 721f 0000 0072  ...rk.....r....r
-00004860: 1400 0000 7266 0000 0072 c600 0000 7242  ....rf...r....rB
-00004870: 0000 0072 1100 0000 7216 0000 0072 6d00  ...r....r....rm.
-00004880: 0000 7287 0000 0072 2000 0000 7220 0000  ..r....r ...r ..
-00004890: 0072 2100 0000 da03 6d61 70d2 0200 0073  .r!.....map....s
-000048a0: 1200 0000 081c 0201 0201 0801 0601 0201  ................
-000048b0: 06fc 0c06 0e02 7a09 5175 6575 652e 6d61  ......z.Queue.ma
-000048c0: 70fa 1753 6571 7565 6e63 655b 5365 7175  p..Sequence[Sequ
-000048d0: 656e 6365 5b41 6e79 5d5d 6303 0000 0003  ence[Any]]c.....
-000048e0: 0000 0002 0000 0009 0000 0007 0000 004f  ...............O
-000048f0: 0000 0173 3e00 0000 7c02 4400 5d15 7d07  ...s>...|.D.].}.
-00004900: 7400 7c01 6700 7c07 a201 7c05 a201 7401  t.|.g.|...|...t.
-00004910: 7c06 8301 7c03 6401 8d04 7d08 7c00 a002  |...|.d...}.|...
-00004920: 7c08 a101 0100 7102 7c00 6a03 6402 7c04  |.....q.|.j.d.|.
-00004930: 6403 8d02 5300 2904 6187 0200 0053 7562  d...S.).a....Sub
-00004940: 6d69 7473 206d 616e 7920 6a6f 6273 2074  mits many jobs t
-00004950: 6f20 7468 6520 7175 6575 6520 2d2d 206f  o the queue -- o
-00004960: 6e65 2066 6f72 2065 6163 6820 7365 7175  ne for each sequ
-00004970: 656e 6365 2069 6e20 7468 6520 6974 6572  ence in the iter
-00004980: 6162 6c65 2e20 5761 6974 7320 666f 7220  able. Waits for 
-00004990: 616c 6c20 746f 2066 696e 6973 682c 2074  all to finish, t
-000049a0: 6865 6e20 7265 7475 726e 7320 7468 6520  hen returns the 
-000049b0: 7265 7375 6c74 732e 0a0a 2020 2020 2020  results...      
-000049c0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
-000049d0: 2020 2020 6675 6e3a 0a20 2020 2020 2020      fun:.       
-000049e0: 2020 2020 2069 7465 7261 626c 653a 0a20       iterable:. 
-000049f0: 2020 2020 2020 2020 2020 2074 696d 656f             timeo
-00004a00: 7574 3a0a 2020 2020 2020 2020 2020 2020  ut:.            
-00004a10: 7368 6f77 5f70 726f 6772 6573 733a 0a0a  show_progress:..
-00004a20: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
-00004a30: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
-00004a40: 3e20 6672 6f6d 2070 7071 7565 7565 2069  > from ppqueue i
-00004a50: 6d70 6f72 7420 5175 6575 650a 2020 2020  mport Queue.    
-00004a60: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00004a70: 2020 2020 2020 2020 3e3e 3e20 6465 6620          >>> def 
-00004a80: 6164 645f 6e75 6d73 2878 3a20 696e 742c  add_nums(x: int,
-00004a90: 2079 3a20 696e 7429 202d 3e20 696e 743a   y: int) -> int:
-00004aa0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00004ab0: 2020 2020 2072 6574 7572 6e20 7820 2b20       return x + 
-00004ac0: 790a 2020 2020 2020 2020 2020 2020 2e2e  y.            ..
-00004ad0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00004ae0: 3e20 7769 7468 2051 7565 7565 2829 2061  > with Queue() a
-00004af0: 7320 7175 6575 653a 0a20 2020 2020 2020  s queue:.       
-00004b00: 2020 2020 202e 2e2e 2020 2020 206a 6f62       ...     job
-00004b10: 7320 3d20 7175 6575 652e 7374 6172 6d61  s = queue.starma
-00004b20: 7028 0a20 2020 2020 2020 2020 2020 202e  p(.            .
-00004b30: 2e2e 2020 2020 2020 2020 2061 6464 5f6e  ..         add_n
-00004b40: 756d 732c 205b 2831 2c20 3229 2c20 2833  ums, [(1, 2), (3
-00004b50: 2c20 3429 5d0a 2020 2020 2020 2020 2020  , 4)].          
-00004b60: 2020 2e2e 2e20 2020 2020 290a 2020 2020    ...     ).    
-00004b70: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
-00004b80: 2020 2020 2020 2020 3e3e 3e20 5b6a 6f62          >>> [job
-00004b90: 2e72 6573 756c 7420 666f 7220 6a6f 6220  .result for job 
-00004ba0: 696e 206a 6f62 735d 0a20 2020 2020 2020  in jobs].       
-00004bb0: 2020 2020 205b 332c 2037 5d0a 2020 2020       [3, 7].    
-00004bc0: 2020 2020 72e8 0000 0054 72e9 0000 0072      r....Tr....r
-00004bd0: ea00 0000 72eb 0000 0072 2000 0000 7220  ....r....r ...r 
-00004be0: 0000 0072 2100 0000 da07 7374 6172 6d61  ...r!.....starma
-00004bf0: 70f9 0200 0073 1200 0000 0820 0201 0201  p....s..... ....
-00004c00: 0a01 0601 0201 06fc 0c06 0e02 7a0d 5175  ............z.Qu
-00004c10: 6575 652e 7374 6172 6d61 70fa 1853 6571  eue.starmap..Seq
-00004c20: 7565 6e63 655b 6469 6374 5b73 7472 2c20  uence[dict[str, 
-00004c30: 416e 795d 5d63 0300 0000 0300 0000 0200  Any]]c..........
-00004c40: 0000 0900 0000 0700 0000 4f00 0001 733e  ..........O...s>
-00004c50: 0000 007c 0244 005d 157d 0774 007c 0174  ...|.D.].}.t.|.t
-00004c60: 017c 0583 0169 007c 07a5 017c 06a5 017c  .|...i.|...|...|
-00004c70: 0364 018d 047d 087c 00a0 027c 08a1 0101  .d...}.|...|....
-00004c80: 0071 027c 006a 0364 027c 0464 038d 0253  .q.|.j.d.|.d...S
-00004c90: 0029 0461 c602 0000 5375 626d 6974 7320  .).a....Submits 
-00004ca0: 6d61 6e79 206a 6f62 7320 746f 2074 6865  many jobs to the
-00004cb0: 2071 7565 7565 202d 2d20 6f6e 6520 666f   queue -- one fo
-00004cc0: 7220 6561 6368 2064 6963 7469 6f6e 6172  r each dictionar
-00004cd0: 7920 696e 2074 6865 2069 7465 7261 626c  y in the iterabl
-00004ce0: 652e 2057 6169 7473 2066 6f72 2061 6c6c  e. Waits for all
-00004cf0: 2074 6f20 6669 6e69 7368 2c20 7468 656e   to finish, then
-00004d00: 2072 6574 7572 6e73 2074 6865 2072 6573   returns the res
-00004d10: 756c 7473 2e0a 0a20 2020 2020 2020 2041  ults...        A
-00004d20: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00004d30: 2066 756e 3a0a 2020 2020 2020 2020 2020   fun:.          
-00004d40: 2020 6974 6572 6162 6c65 3a0a 2020 2020    iterable:.    
-00004d50: 2020 2020 2020 2020 7469 6d65 6f75 743a          timeout:
-00004d60: 0a20 2020 2020 2020 2020 2020 2073 686f  .            sho
-00004d70: 775f 7072 6f67 7265 7373 3a0a 0a20 2020  w_progress:..   
-00004d80: 2020 2020 2045 7861 6d70 6c65 733a 0a20       Examples:. 
-00004d90: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
-00004da0: 726f 6d20 7070 7175 6575 6520 696d 706f  rom ppqueue impo
-00004db0: 7274 2051 7565 7565 0a20 2020 2020 2020  rt Queue.       
-00004dc0: 2020 2020 203e 3e3e 2066 726f 6d20 7469       >>> from ti
-00004dd0: 6d65 2069 6d70 6f72 7420 736c 6565 700a  me import sleep.
-00004de0: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
-00004df0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
-00004e00: 6465 6620 6164 645f 6e75 6d73 2878 3a20  def add_nums(x: 
-00004e10: 696e 742c 2079 3a20 696e 7429 202d 3e20  int, y: int) -> 
-00004e20: 696e 743a 0a20 2020 2020 2020 2020 2020  int:.           
-00004e30: 202e 2e2e 2020 2020 2072 6574 7572 6e20   ...     return 
-00004e40: 7820 2b20 790a 2020 2020 2020 2020 2020  x + y.          
-00004e50: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00004e60: 2020 3e3e 3e20 7769 7468 2051 7565 7565    >>> with Queue
-00004e70: 2829 2061 7320 7175 6575 653a 0a20 2020  () as queue:.   
-00004e80: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
-00004e90: 206a 6f62 7320 3d20 7175 6575 652e 7374   jobs = queue.st
-00004ea0: 6172 6d61 706b 7728 0a20 2020 2020 2020  armapkw(.       
-00004eb0: 2020 2020 202e 2e2e 2020 2020 2020 2020       ...        
-00004ec0: 2061 6464 5f6e 756d 732c 205b 7b27 7827   add_nums, [{'x'
-00004ed0: 3a20 312c 2027 7927 3a20 327d 2c20 7b27  : 1, 'y': 2}, {'
-00004ee0: 7827 3a20 332c 2027 7927 3a20 347d 5d0a  x': 3, 'y': 4}].
-00004ef0: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
-00004f00: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00004f10: 2020 2e2e 2e0a 2020 2020 2020 2020 2020    ....          
-00004f20: 2020 3e3e 3e20 5b6a 6f62 2e72 6573 756c    >>> [job.resul
-00004f30: 7420 666f 7220 6a6f 6220 696e 206a 6f62  t for job in job
-00004f40: 735d 0a20 2020 2020 2020 2020 2020 205b  s].            [
-00004f50: 332c 2037 5d0a 2020 2020 2020 2020 72e8  3, 7].        r.
-00004f60: 0000 0054 72e9 0000 0029 0472 0c00 0000  ...Tr....).r....
-00004f70: 727c 0000 0072 e200 0000 726b 0000 0072  r|...r....rk...r
-00004f80: eb00 0000 7220 0000 0072 2000 0000 7221  ....r ...r ...r!
-00004f90: 0000 00da 0973 7461 726d 6170 6b77 2403  .....starmapkw$.
-00004fa0: 0000 7312 0000 0008 2102 0102 0106 010a  ..s.....!.......
-00004fb0: 0102 0106 fc0c 060e 027a 0f51 7565 7565  .........z.Queue
-00004fc0: 2e73 7461 726d 6170 6b77 2902 726a 0000  .starmapkw).rj..
-00004fd0: 00da 055f 7065 656b 72f1 0000 00fa 0a4a  ..._peekr......J
-00004fe0: 6f62 207c 204e 6f6e 6563 0100 0000 0000  ob | Nonec......
-00004ff0: 0000 0200 0000 0500 0000 0400 0000 4b00  ..............K.
-00005000: 0001 735e 0000 007c 00a0 00a1 0064 016b  ..s^...|.....d.k
-00005010: 0272 187c 0173 0a64 0253 0064 037c 0364  .r.|.s.d.S.d.|.d
-00005020: 043c 007c 006a 0164 0764 0564 0669 017c  .<.|.j.d.d.d.i.|
-00005030: 03a4 018e 0101 007c 0272 217c 006a 0264  .......|.r!|.j.d
-00005040: 0119 007d 047c 0453 0074 037c 006a 0283  ...}.|.S.t.|.j..
-00005050: 017d 047c 0004 006a 0464 0637 0002 005f  .}.|...j.d.7..._
-00005060: 047c 0453 0029 0861 a602 0000 5265 6d6f  .|.S.).a....Remo
-00005070: 7665 7320 616e 6420 7265 7475 726e 7320  ves and returns 
-00005080: 7468 6520 6a6f 6220 7769 7468 2074 6865  the job with the
-00005090: 2068 6967 6865 7374 2070 7269 6f72 6974   highest priorit
-000050a0: 7920 6672 6f6d 2074 6865 2071 7565 7565  y from the queue
-000050b0: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
-000050c0: 0a20 2020 2020 2020 2020 2020 2077 6169  .            wai
-000050d0: 743a 0a20 2020 2020 2020 2020 2020 202a  t:.            *
-000050e0: 2a6b 7761 7267 733a 2070 6173 7365 6420  *kwargs: passed 
-000050f0: 746f 2060 5175 6575 652e 7761 6974 600a  to `Queue.wait`.
-00005100: 0a20 2020 2020 2020 2045 7861 6d70 6c65  .        Example
-00005110: 733a 0a20 2020 2020 2020 2020 2020 203e  s:.            >
-00005120: 3e3e 2066 726f 6d20 7070 7175 6575 6520  >> from ppqueue 
-00005130: 696d 706f 7274 2051 7565 7565 0a20 2020  import Queue.   
-00005140: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
-00005150: 2020 2020 2020 2020 203e 3e3e 2064 6566           >>> def
-00005160: 2061 6464 5f6e 756d 7328 783a 2069 6e74   add_nums(x: int
-00005170: 2c20 793a 2069 6e74 2920 2d3e 2069 6e74  , y: int) -> int
-00005180: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00005190: 2e20 2020 2020 7265 7475 726e 2078 202b  .     return x +
-000051a0: 2079 0a20 2020 2020 2020 2020 2020 202e   y.            .
-000051b0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
-000051c0: 3e3e 2077 6974 6820 5175 6575 6528 2920  >> with Queue() 
-000051d0: 6173 2071 7565 7565 3a0a 2020 2020 2020  as queue:.      
-000051e0: 2020 2020 2020 2e2e 2e20 2020 2020 666f        ...     fo
-000051f0: 7220 6920 696e 2072 616e 6765 2835 293a  r i in range(5):
-00005200: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
-00005210: 2020 2020 2020 2020 205f 203d 2071 7565           _ = que
-00005220: 7565 2e65 6e71 7565 7565 2861 6464 5f6e  ue.enqueue(add_n
-00005230: 756d 732c 2061 7267 733d 5b69 2c20 3130  ums, args=[i, 10
-00005240: 305d 290a 2020 2020 2020 2020 2020 2020  0]).            
-00005250: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00005260: 2e2e 2e20 2020 2020 6a6f 6273 203d 205b  ...     jobs = [
-00005270: 7175 6575 652e 6465 7175 6575 6528 7761  queue.dequeue(wa
-00005280: 6974 3d54 7275 6529 2066 6f72 205f 2069  it=True) for _ i
-00005290: 6e20 7261 6e67 6528 7175 6575 652e 7369  n range(queue.si
-000052a0: 7a65 2829 295d 0a20 2020 2020 2020 2020  ze())].         
-000052b0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-000052c0: 2020 203e 3e3e 205b 6a6f 622e 7265 7375     >>> [job.resu
-000052d0: 6c74 2066 6f72 206a 6f62 2069 6e20 6a6f  lt for job in jo
-000052e0: 6273 5d0a 2020 2020 2020 2020 2020 2020  bs].            
-000052f0: 5b31 3030 2c20 3130 312c 2031 3032 2c20  [100, 101, 102, 
-00005300: 3130 332c 2031 3034 5d0a 2020 2020 2020  103, 104].      
-00005310: 2020 7201 0000 004e 4672 4200 0000 72c5    r....NFrB...r.
-00005320: 0000 0072 0b00 0000 7220 0000 0029 0572  ...r....r ...).r
-00005330: a700 0000 726a 0000 0072 5c00 0000 7203  ....rj...r\...r.
-00005340: 0000 0072 5000 0000 2905 721f 0000 0072  ...rP...).r....r
-00005350: 6a00 0000 72f1 0000 0072 1600 0000 7287  j...r....r....r.
-00005360: 0000 0072 2000 0000 7220 0000 0072 2100  ...r ...r ...r!.
-00005370: 0000 728e 0000 0050 0300 0073 1600 0000  ..r....P...s....
-00005380: 0c1d 0401 0401 0802 1401 0403 0a01 0405  ................
-00005390: 0afd 0e01 0402 7a0d 5175 6575 652e 6465  ......z.Queue.de
-000053a0: 7175 6575 6563 0100 0000 0000 0000 0000  queuec..........
-000053b0: 0000 0300 0000 0400 0000 4f00 0001 72c3  ..........O...r.
-000053c0: 0000 0029 0161 6502 0000 416c 6961 7320  ...).ae...Alias 
-000053d0: 666f 7220 6064 6571 7565 7565 602e 2052  for `dequeue`. R
-000053e0: 656d 6f76 6573 2061 6e64 2072 6574 7572  emoves and retur
-000053f0: 6e73 2074 6865 206a 6f62 2077 6974 6820  ns the job with 
-00005400: 7468 6520 6869 6768 6573 7420 7072 696f  the highest prio
-00005410: 7269 7479 2066 726f 6d20 7468 6520 7175  rity from the qu
-00005420: 6575 652e 0a0a 2020 2020 2020 2020 4578  eue...        Ex
-00005430: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
-00005440: 2020 2020 3e3e 3e20 6672 6f6d 2070 7071      >>> from ppq
-00005450: 7565 7565 2069 6d70 6f72 7420 5175 6575  ueue import Queu
-00005460: 650a 2020 2020 2020 2020 2020 2020 2e2e  e.            ..
-00005470: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
-00005480: 3e20 6465 6620 6164 645f 6e75 6d73 2878  > def add_nums(x
-00005490: 3a20 696e 742c 2079 3a20 696e 7429 202d  : int, y: int) -
-000054a0: 3e20 696e 743a 0a20 2020 2020 2020 2020  > int:.         
-000054b0: 2020 202e 2e2e 2020 2020 2072 6574 7572     ...     retur
-000054c0: 6e20 7820 2b20 790a 2020 2020 2020 2020  n x + y.        
-000054d0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
-000054e0: 2020 2020 3e3e 3e20 7769 7468 2051 7565      >>> with Que
-000054f0: 7565 2829 2061 7320 7175 6575 653a 0a20  ue() as queue:. 
-00005500: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
-00005510: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
-00005520: 6528 3529 3a0a 2020 2020 2020 2020 2020  e(5):.          
-00005530: 2020 2e2e 2e20 2020 2020 2020 2020 5f20    ...         _ 
-00005540: 3d20 7175 6575 652e 7075 7428 6164 645f  = queue.put(add_
-00005550: 6e75 6d73 2c20 6172 6773 3d5b 692c 2031  nums, args=[i, 1
-00005560: 3030 5d29 0a20 2020 2020 2020 2020 2020  00]).           
-00005570: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00005580: 202e 2e2e 2020 2020 206a 6f62 7320 3d20   ...     jobs = 
-00005590: 5b71 7565 7565 2e70 6f70 2877 6169 743d  [queue.pop(wait=
-000055a0: 5472 7565 2920 666f 7220 5f20 696e 2072  True) for _ in r
-000055b0: 616e 6765 2871 7565 7565 2e73 697a 6528  ange(queue.size(
-000055c0: 2929 5d0a 2020 2020 2020 2020 2020 2020  ))].            
-000055d0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-000055e0: 3e3e 3e20 5b6a 6f62 2e72 6573 756c 7420  >>> [job.result 
-000055f0: 666f 7220 6a6f 6220 696e 206a 6f62 735d  for job in jobs]
-00005600: 0a20 2020 2020 2020 2020 2020 205b 3130  .            [10
-00005610: 302c 2031 3031 2c20 3130 322c 2031 3033  0, 101, 102, 103
-00005620: 2c20 3130 345d 0a20 2020 2020 2020 20a9  , 104].        .
-00005630: 0172 8e00 0000 72c4 0000 0072 2000 0000  .r....r....r ...
-00005640: 7220 0000 0072 2100 0000 7296 0000 007d  r ...r!...r....}
-00005650: 0300 0072 e700 0000 7a09 5175 6575 652e  ...r....z.Queue.
-00005660: 706f 7063 0100 0000 0000 0000 0000 0000  popc............
-00005670: 0300 0000 0500 0000 4f00 0001 7318 0000  ........O...s...
-00005680: 007c 006a 007c 0169 007c 02a4 0164 0164  .|.j.|.i.|...d.d
-00005690: 0269 01a4 018e 0153 0029 0361 2503 0000  .i.....S.).a%...
-000056a0: 5265 7475 726e 7320 7468 6520 6a6f 6220  Returns the job 
-000056b0: 7769 7468 2074 6865 2068 6967 6865 7374  with the highest
-000056c0: 2070 7269 6f72 6974 7920 6672 6f6d 2074   priority from t
-000056d0: 6865 2071 7565 7565 2e20 5369 6d69 6c61  he queue. Simila
-000056e0: 7220 746f 2060 656e 7175 6575 6560 202f  r to `enqueue` /
-000056f0: 2060 706f 7060 2c20 6275 7420 7468 6520   `pop`, but the 
-00005700: 6a6f 6220 7265 6d61 696e 7320 696e 2074  job remains in t
-00005710: 6865 2071 7565 7565 2e0a 0a20 2020 2020  he queue...     
-00005720: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00005730: 2020 2020 202a 6172 6773 3a0a 2020 2020       *args:.    
-00005740: 2020 2020 2020 2020 2a2a 6b77 6172 6773          **kwargs
-00005750: 3a0a 0a20 2020 2020 2020 2045 7861 6d70  :..        Examp
-00005760: 6c65 733a 0a20 2020 2020 2020 2020 2020  les:.           
-00005770: 203e 3e3e 2066 726f 6d20 7070 7175 6575   >>> from ppqueu
-00005780: 6520 696d 706f 7274 2051 7565 7565 0a20  e import Queue. 
-00005790: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
-000057a0: 2020 2020 2020 2020 2020 203e 3e3e 2064             >>> d
-000057b0: 6566 2061 6464 5f6e 756d 7328 783a 2069  ef add_nums(x: i
-000057c0: 6e74 2c20 793a 2069 6e74 2920 2d3e 2069  nt, y: int) -> i
-000057d0: 6e74 3a0a 2020 2020 2020 2020 2020 2020  nt:.            
-000057e0: 2e2e 2e20 2020 2020 7265 7475 726e 2078  ...     return x
-000057f0: 202b 2079 0a20 2020 2020 2020 2020 2020   + y.           
-00005800: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00005810: 203e 3e3e 2077 6974 6820 5175 6575 6528   >>> with Queue(
-00005820: 2920 6173 2071 7565 7565 3a0a 2020 2020  ) as queue:.    
-00005830: 2020 2020 2020 2020 2e2e 2e20 2020 2020          ...     
-00005840: 666f 7220 6920 696e 2072 616e 6765 2835  for i in range(5
-00005850: 293a 0a20 2020 2020 2020 2020 2020 202e  ):.            .
-00005860: 2e2e 2020 2020 2020 2020 205f 203d 2071  ..         _ = q
-00005870: 7565 7565 2e70 7574 2861 6464 5f6e 756d  ueue.put(add_num
-00005880: 732c 2061 7267 733d 5b69 2c20 3130 305d  s, args=[i, 100]
-00005890: 290a 2020 2020 2020 2020 2020 2020 2e2e  ).            ..
-000058a0: 2e0a 2020 2020 2020 2020 2020 2020 2e2e  ..            ..
-000058b0: 2e20 2020 2020 7072 696e 7428 2742 6566  .     print('Bef
-000058c0: 6f72 653a 272c 2071 7565 7565 2e73 697a  ore:', queue.siz
-000058d0: 6528 2929 0a20 2020 2020 2020 2020 2020  e()).           
-000058e0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-000058f0: 202e 2e2e 2020 2020 206a 6f62 203d 2071   ...     job = q
-00005900: 7565 7565 2e70 6565 6b28 7761 6974 3d54  ueue.peek(wait=T
-00005910: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
-00005920: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00005930: 202e 2e2e 2020 2020 2070 7269 6e74 2827   ...     print('
-00005940: 4166 7465 723a 272c 2071 7565 7565 2e73  After:', queue.s
-00005950: 697a 6528 2929 0a20 2020 2020 2020 2020  ize()).         
-00005960: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
-00005970: 2020 2042 6566 6f72 653a 2035 0a20 2020     Before: 5.   
-00005980: 2020 2020 2020 2020 2041 6674 6572 3a20           After: 
-00005990: 350a 2020 2020 2020 2020 2020 2020 3e3e  5.            >>
-000059a0: 3e20 6a6f 622e 7265 7375 6c74 0a20 2020  > job.result.   
-000059b0: 2020 2020 2020 2020 2031 3030 0a20 2020           100.   
-000059c0: 2020 2020 2072 f100 0000 5472 f300 0000       r....Tr....
-000059d0: 72c4 0000 0072 2000 0000 7220 0000 0072  r....r ...r ...r
-000059e0: 2100 0000 da04 7065 656b 9103 0000 7302  !.....peek....s.
-000059f0: 0000 0018 1c7a 0a51 7565 7565 2e70 6565  .....z.Queue.pee
-00005a00: 6b63 0300 0000 0000 0000 0000 0000 0600  kc..............
-00005a10: 0000 0400 0000 0b00 0001 7350 0000 007c  ..........sP...|
-00005a20: 0272 0c88 006a 0064 0664 017c 0169 017c  .r...j.d.d.|.i.|
-00005a30: 03a4 018e 0101 0088 00a0 01a1 007d 047c  .............}.|
-00005a40: 0164 026b 0472 1974 027c 017c 0483 026e  .d.k.r.t.|.|...n
-00005a50: 017c 047d 0574 0387 0066 0164 0364 0484  .|.}.t...f.d.d..
-00005a60: 0874 047c 0583 0144 0083 0183 0153 0029  .t.|...D.....S.)
-00005a70: 0761 1903 0000 5265 6d6f 7665 7320 616e  .a....Removes an
-00005a80: 6420 7265 7475 726e 7320 616c 6c20 6669  d returns all fi
-00005a90: 6e69 7368 6564 206a 6f62 7320 6672 6f6d  nished jobs from
-00005aa0: 2074 6865 2071 7565 7565 2e0a 0a20 2020   the queue...   
-00005ab0: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
-00005ac0: 2020 2020 2020 206e 3a20 636f 6c6c 6563         n: collec
-00005ad0: 7420 7468 6973 206d 616e 7920 6a6f 6273  t this many jobs
-00005ae0: 2028 6465 6661 756c 743d 302c 2061 6c6c   (default=0, all
-00005af0: 290a 2020 2020 2020 2020 2020 2020 7761  ).            wa
-00005b00: 6974 3a20 4966 2054 7275 652c 2062 6c6f  it: If True, blo
-00005b10: 636b 2075 6e74 696c 2074 6869 7320 6d61  ck until this ma
-00005b20: 6e79 206a 6f62 7320 6172 6520 6669 6e69  ny jobs are fini
-00005b30: 7368 6564 2e20 456c 7365 2c20 696d 6d65  shed. Else, imme
-00005b40: 6469 6174 656c 7920 7265 7475 726e 2061  diately return a
-00005b50: 6c6c 2066 696e 6973 6865 642e 0a20 2020  ll finished..   
-00005b60: 2020 2020 2020 2020 202a 2a6b 7761 7267           **kwarg
-00005b70: 733a 206b 7761 7267 7320 6769 7665 6e20  s: kwargs given 
-00005b80: 746f 2060 5175 6575 652e 7761 6974 602e  to `Queue.wait`.
-00005b90: 0a0a 2020 2020 2020 2020 4578 616d 706c  ..        Exampl
-00005ba0: 6573 3a0a 2020 2020 2020 2020 2020 2020  es:.            
-00005bb0: 3e3e 3e20 6672 6f6d 2070 7071 7565 7565  >>> from ppqueue
-00005bc0: 2069 6d70 6f72 7420 5175 6575 650a 2020   import Queue.  
-00005bd0: 2020 2020 2020 2020 2020 2e2e 2e0a 2020            ....  
-00005be0: 2020 2020 2020 2020 2020 3e3e 3e20 6465            >>> de
-00005bf0: 6620 6164 645f 6e75 6d73 2878 3a20 696e  f add_nums(x: in
-00005c00: 742c 2079 3a20 696e 7429 202d 3e20 696e  t, y: int) -> in
-00005c10: 743a 0a20 2020 2020 2020 2020 2020 202e  t:.            .
-00005c20: 2e2e 2020 2020 2072 6574 7572 6e20 7820  ..     return x 
-00005c30: 2b20 790a 2020 2020 2020 2020 2020 2020  + y.            
-00005c40: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
-00005c50: 3e3e 3e20 7769 7468 2051 7565 7565 2829  >>> with Queue()
-00005c60: 2061 7320 7175 6575 653a 0a20 2020 2020   as queue:.     
-00005c70: 2020 2020 2020 202e 2e2e 2020 2020 2066         ...     f
-00005c80: 6f72 2069 2069 6e20 7261 6e67 6528 3529  or i in range(5)
-00005c90: 3a0a 2020 2020 2020 2020 2020 2020 2e2e  :.            ..
-00005ca0: 2e20 2020 2020 2020 2020 5f20 3d20 7175  .         _ = qu
-00005cb0: 6575 652e 656e 7175 6575 6528 6164 645f  eue.enqueue(add_
-00005cc0: 6e75 6d73 2c20 6172 6773 3d5b 692c 2031  nums, args=[i, 1
-00005cd0: 3030 5d29 0a20 2020 2020 2020 2020 2020  00]).           
-00005ce0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
-00005cf0: 202e 2e2e 2020 2020 206a 6f62 7320 3d20   ...     jobs = 
-00005d00: 7175 6575 652e 636f 6c6c 6563 7428 7761  queue.collect(wa
-00005d10: 6974 3d54 7275 6529 0a20 2020 2020 2020  it=True).       
-00005d20: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
-00005d30: 2020 2020 203e 3e3e 2074 7970 6528 6a6f       >>> type(jo
-00005d40: 6273 290a 2020 2020 2020 2020 2020 2020  bs).            
-00005d50: 3c63 6c61 7373 2027 6c69 7374 273e 0a20  <class 'list'>. 
-00005d60: 2020 2020 2020 2020 2020 203e 3e3e 206c             >>> l
-00005d70: 656e 286a 6f62 7329 0a20 2020 2020 2020  en(jobs).       
-00005d80: 2020 2020 2035 0a20 2020 2020 2020 2072       5.        r
-00005d90: c500 0000 7201 0000 0063 0100 0000 0000  ....r....c......
-00005da0: 0000 0000 0000 0200 0000 0300 0000 3300  ..............3.
-00005db0: 0001 7318 0000 0081 007c 005d 077d 0174  ..s......|.].}.t
-00005dc0: 0088 0083 0156 0001 0071 0264 0053 0072  .....V...q.d.S.r
-00005dd0: 2f00 0000 2901 da04 6e65 7874 2902 72ac  /...)...next).r.
-00005de0: 0000 0072 8600 0000 7226 0000 0072 2000  ...r....r&...r .
-00005df0: 0000 7221 0000 0072 ae00 0000 d003 0000  ..r!...r........
-00005e00: 7304 0000 0002 8016 007a 2051 7565 7565  s........z Queue
-00005e10: 2e63 6f6c 6c65 6374 2e3c 6c6f 6361 6c73  .collect.<locals
-00005e20: 3e2e 3c67 656e 6578 7072 3e4e 7220 0000  >.<genexpr>Nr ..
-00005e30: 0029 0572 6a00 0000 72a7 0000 00da 036d  .).rj...r......m
-00005e40: 696e 727c 0000 0072 7f00 0000 2906 721f  inr|...r....).r.
-00005e50: 0000 0072 c500 0000 726a 0000 0072 1600  ...r....rj...r..
-00005e60: 0000 5a0a 6e5f 6669 6e69 7368 6564 5a0c  ..Z.n_finishedZ.
-00005e70: 6e5f 746f 5f63 6f6c 6c65 6374 7220 0000  n_to_collectr ..
-00005e80: 0072 2600 0000 7221 0000 0072 6b00 0000  .r&...r!...rk...
-00005e90: af03 0000 730a 0000 0004 1a14 0108 0216  ....s...........
-00005ea0: 021a 027a 0d51 7565 7565 2e63 6f6c 6c65  ...z.Queue.colle
-00005eb0: 6374 6301 0000 0000 0000 0000 0000 0001  ctc.............
-00005ec0: 0000 0001 0000 0043 0000 0172 2e00 0000  .......C...r....
-00005ed0: 722f 0000 00a9 0172 5100 0000 7226 0000  r/.....rQ...r&..
-00005ee0: 0072 2000 0000 7220 0000 0072 2100 0000  .r ...r ...r!...
-00005ef0: 7247 0000 00d2 0300 0072 3100 0000 7a14  rG.......r1...z.
-00005f00: 5175 6575 652e 6d61 785f 636f 6e63 7572  Queue.max_concur
-00005f10: 7265 6e74 da05 7661 6c75 6563 0200 0000  rent..valuec....
-00005f20: 0000 0000 0000 0000 0200 0000 0200 0000  ................
-00005f30: 4300 0001 f30a 0000 007c 017c 005f 0064  C........|.|._.d
-00005f40: 0053 0072 2f00 0000 72f7 0000 00a9 0272  .S.r/...r......r
-00005f50: 1f00 0000 72f8 0000 0072 2000 0000 7220  ....r....r ...r 
-00005f60: 0000 0072 2100 0000 7247 0000 00d6 0300  ...r!...rG......
-00005f70: 0072 b100 0000 6301 0000 0000 0000 0000  .r....c.........
-00005f80: 0000 0001 0000 0001 0000 0043 0000 0172  ...........C...r
-00005f90: 2e00 0000 722f 0000 00a9 0172 4e00 0000  ....r/.....rN...
-00005fa0: 7226 0000 0072 2000 0000 7220 0000 0072  r&...r ...r ...r
-00005fb0: 2100 0000 723e 0000 00da 0300 0072 3100  !...r>.......r1.
-00005fc0: 0000 7a0e 5175 6575 652e 6d61 785f 7369  ..z.Queue.max_si
-00005fd0: 7a65 6302 0000 0000 0000 0000 0000 0002  zec.............
-00005fe0: 0000 0002 0000 0043 0000 0172 f900 0000  .......C...r....
-00005ff0: 722f 0000 0072 fb00 0000 72fa 0000 0072  r/...r....r....r
-00006000: 2000 0000 7220 0000 0072 2100 0000 723e   ...r ...r!...r>
-00006010: 0000 00de 0300 0072 b100 0000 6301 0000  .......r....c...
-00006020: 0000 0000 0000 0000 0001 0000 0001 0000  ................
-00006030: 0043 0000 0173 0800 0000 7c00 6a00 6a01  .C...s....|.j.j.
-00006040: 5300 722f 0000 0029 0272 1800 0000 7232  S.r/...).r....r2
-00006050: 0000 0072 2600 0000 7220 0000 0072 2000  ...r&...r ...r .
-00006060: 0000 7221 0000 0072 3000 0000 e203 0000  ..r!...r0.......
-00006070: 7302 0000 0008 027a 1051 7565 7565 2e69  s......z.Queue.i
-00006080: 735f 7275 6e6e 696e 6729 1472 4700 0000  s_running).rG...
-00006090: 7213 0000 0072 3e00 0000 7213 0000 0072  r....r>...r....r
-000060a0: 3f00 0000 7248 0000 0072 4000 0000 7249  ?...rH...r@...rI
-000060b0: 0000 0072 4100 0000 724a 0000 0072 4200  ...rA...rJ...rB.
-000060c0: 0000 722d 0000 0072 4300 0000 722d 0000  ..r-...rC...r-..
-000060d0: 0072 4400 0000 722d 0000 0072 4500 0000  .rD...r-...rE...
-000060e0: 7213 0000 0072 4600 0000 722d 0000 0029  r....rF...r-...)
-000060f0: 0672 1400 0000 7215 0000 0072 1100 0000  .r....r....r....
-00006100: 7205 0000 0072 1600 0000 7205 0000 0072  r....r....r....r
-00006110: 3300 0000 2904 726a 0000 0072 2d00 0000  3...).rj...r-...
-00006120: 7223 0000 0072 2400 0000 2902 7223 0000  r#...r$...).r#..
-00006130: 0072 3a00 0000 2904 7211 0000 0072 0500  .r:...).r....r..
-00006140: 0000 7223 0000 0072 2400 0000 2902 7223  ..r#...r$...).r#
-00006150: 0000 0072 0c00 0000 2902 7223 0000 0072  ...r....).r#...r
-00006160: 1300 0000 2908 72b2 0000 0072 2d00 0000  ....).r....r-...
-00006170: 72b3 0000 0072 2d00 0000 72b8 0000 0072  r....r-...r....r
-00006180: 2d00 0000 7223 0000 0072 b900 0000 2908  -...r#...r....).
-00006190: 72b2 0000 0072 2d00 0000 72b3 0000 0072  r....r-...r....r
-000061a0: 2d00 0000 72b8 0000 0072 2d00 0000 7223  -...r....r-...r#
-000061b0: 0000 0072 1300 0000 7234 0000 0029 0a72  ...r....r4...).r
-000061c0: c500 0000 7213 0000 0072 c600 0000 72c8  ....r....r....r.
-000061d0: 0000 0072 c700 0000 7213 0000 0072 4200  ...r....r....rB.
-000061e0: 0000 72c9 0000 0072 2300 0000 7213 0000  ..r....r#...r...
-000061f0: 0029 0a72 d500 0000 720c 0000 0072 6100  .).r....r....ra.
-00006200: 0000 72d6 0000 0072 1100 0000 7205 0000  ..r....r....r...
-00006210: 0072 1600 0000 7205 0000 0072 2300 0000  .r....r....r#...
-00006220: 72d7 0000 0029 0472 8700 0000 720c 0000  r....).r....r...
-00006230: 0072 2300 0000 7224 0000 0029 0472 8700  .r#...r$...).r..
-00006240: 0000 720c 0000 0072 2300 0000 7213 0000  ..r....r#...r...
-00006250: 0029 084e 4e4e 723d 0000 004e 7201 0000  .).NNNr=...Nr...
-00006260: 0046 4629 1472 1100 0000 72e3 0000 0072  .FF).r....r....r
-00006270: 1600 0000 72e4 0000 0072 4000 0000 7249  ....r....r@...rI
-00006280: 0000 0072 e500 0000 7213 0000 0072 a000  ...r....r....r..
-00006290: 0000 723b 0000 0072 c600 0000 72c8 0000  ..r;...r....r...
-000062a0: 0072 d900 0000 722d 0000 0072 a100 0000  .r....r-...r....
-000062b0: 722d 0000 0072 1400 0000 7215 0000 0072  r-...r....r....r
-000062c0: 2300 0000 7213 0000 0029 0e72 1400 0000  #...r....).r....
-000062d0: 7215 0000 0072 6600 0000 7267 0000 0072  r....rf...rg...r
-000062e0: 1100 0000 7205 0000 0072 c600 0000 72c8  ....r....r....r.
-000062f0: 0000 0072 4200 0000 72c9 0000 0072 1600  ...rB...r....r..
-00006300: 0000 7205 0000 0072 2300 0000 7268 0000  ..r....r#...rh..
-00006310: 0029 0e72 1400 0000 7215 0000 0072 6600  .).r....r....rf.
-00006320: 0000 72ed 0000 0072 1100 0000 7205 0000  ..r....r....r...
-00006330: 0072 c600 0000 72c8 0000 0072 4200 0000  .r....r....rB...
-00006340: 72c9 0000 0072 1600 0000 7205 0000 0072  r....r....r....r
-00006350: 2300 0000 7268 0000 0029 0e72 1400 0000  #...rh...).r....
-00006360: 7215 0000 0072 6600 0000 72ef 0000 0072  r....rf...r....r
-00006370: 1100 0000 7205 0000 0072 c600 0000 72c8  ....r....r....r.
-00006380: 0000 0072 4200 0000 72c9 0000 0072 1600  ...rB...r....r..
-00006390: 0000 7205 0000 0072 2300 0000 7268 0000  ..r....r#...rh..
-000063a0: 0029 0872 6a00 0000 722d 0000 0072 f100  .).rj...r-...r..
-000063b0: 0000 722d 0000 0072 1600 0000 7205 0000  ..r-...r....r...
-000063c0: 0072 2300 0000 72f2 0000 0029 0672 1100  .r#...r....).r..
-000063d0: 0000 7205 0000 0072 1600 0000 7205 0000  ..r....r....r...
-000063e0: 0072 2300 0000 72f2 0000 0029 0272 0100  .r#...r....).r..
-000063f0: 0000 4629 0872 c500 0000 7213 0000 0072  ..F).r....r....r
-00006400: 6a00 0000 722d 0000 0072 1600 0000 7205  j...r-...r....r.
-00006410: 0000 0072 2300 0000 7268 0000 0029 0272  ...r#...rh...).r
-00006420: f800 0000 7213 0000 0029 0472 f800 0000  ....r....).r....
-00006430: 7213 0000 0072 2300 0000 7224 0000 0029  r....r#...r$...)
-00006440: 3572 3500 0000 7236 0000 0072 3700 0000  5r5...r6...r7...
-00006450: 723c 0000 00da 0f5f 5f61 6e6e 6f74 6174  r<.....__annotat
-00006460: 696f 6e73 5f5f 7255 0000 00da 0963 7075  ions__rU.....cpu
-00006470: 5f63 6f75 6e74 7229 0000 0072 de00 0000  _countr)...r....
-00006480: 7222 0000 0072 7100 0000 7274 0000 0072  r"...rq...rt...r
-00006490: 2500 0000 722c 0000 0072 6c00 0000 7288  %...r,...rl...r.
-000064a0: 0000 0072 7900 0000 728a 0000 0072 8c00  ...ry...r....r..
-000064b0: 0000 728d 0000 0072 9000 0000 7264 0000  ..r....r....rd..
-000064c0: 0072 a600 0000 72a3 0000 0072 a700 0000  .r....r....r....
-000064d0: 72b6 0000 0072 be00 0000 72bf 0000 0072  r....r....r....r
-000064e0: b500 0000 7291 0000 0072 c000 0000 72c1  ....r....r....r.
-000064f0: 0000 0072 c200 0000 7295 0000 0072 6a00  ...r....r....rj.
-00006500: 0000 da0c 7374 6174 6963 6d65 7468 6f64  ....staticmethod
-00006510: 72da 0000 0072 a200 0000 72e2 0000 0072  r....r....r....r
-00006520: 6900 0000 72e6 0000 0072 ec00 0000 72ee  i...r....r....r.
-00006530: 0000 0072 f000 0000 728e 0000 0072 9600  ...r....r....r..
-00006540: 0000 72f4 0000 0072 6b00 0000 7239 0000  ..r....rk...r9..
-00006550: 0072 4700 0000 da06 7365 7474 6572 723e  .rG.....setterr>
-00006560: 0000 0072 3000 0000 7220 0000 0072 2000  ...r0...r ...r .
-00006570: 0000 7220 0000 0072 2100 0000 723a 0000  ..r ...r!...r:..
-00006580: 0046 0000 0073 b000 0000 0a00 0c01 0604  .F...s..........
-00006590: 02fe 0204 0401 0201 0201 0201 0201 0201  ................
-000065a0: 0201 0201 0ef4 0a5d 0a0d 0a03 0a04 0a04  .......]........
-000065b0: 0a14 1012 0a0e 0a03 0a03 0a03 0a06 0a7a  ...............z
-000065c0: 0a04 0a04 0a04 0207 0201 0201 0efb 0a32  ...............2
-000065d0: 0206 0201 0201 0efb 0a22 0a03 0a04 0a04  ........."......
-000065e0: 0a04 0206 0201 0201 0201 0efa 0244 0c01  .............D..
-000065f0: 0a19 0a0e 022c 0201 0201 0201 0201 0201  .....,..........
-00006600: 0201 0201 0cf5 0a36 021a 0201 0ef9 022d  .......6.......-
-00006610: 0201 0ef9 0231 0201 0ef9 022f 0201 0efc  .....1...../....
-00006620: 0a2d 0a14 0c1e 0223 0c01 0403 0c01 0203  .-.....#........
-00006630: 0c01 0403 0c01 0203 1001 723a 0000 0029  ..........r:...)
-00006640: 1eda 0a5f 5f66 7574 7572 655f 5f72 0200  ...__future__r..
-00006650: 0000 da07 6c6f 6767 696e 67da 0f6d 756c  ....logging..mul
-00006660: 7469 7072 6f63 6573 7369 6e67 7255 0000  tiprocessingrU..
-00006670: 0072 2900 0000 7282 0000 0072 a400 0000  .r)...r....r....
-00006680: da05 6865 6170 7172 0300 0000 7204 0000  ..heapqr....r...
-00006690: 00da 0674 7970 696e 6772 0500 0000 7206  ...typingr....r.
-000066a0: 0000 0072 0700 0000 7208 0000 00da 0475  ...r....r......u
-000066b0: 7569 6472 0900 0000 5a09 7471 646d 2e61  uidr....Z.tqdm.a
-000066c0: 7574 6f72 0a00 0000 7287 0000 0072 0c00  utor....r....r..
-000066d0: 0000 da05 7574 696c 7372 0d00 0000 720e  ....utilsr....r.
-000066e0: 0000 0072 3500 0000 da04 494e 464f 7257  ...r5.....INFOrW
-000066f0: 0000 0072 1000 0000 723a 0000 0072 2000  ...r....r:...r .
-00006700: 0000 7220 0000 0072 2000 0000 7221 0000  ..r ...r ...r!..
-00006710: 00da 083c 6d6f 6475 6c65 3e01 0000 0073  ...<module>....s
-00006720: 1e00 0000 0c00 0802 0801 0801 0801 0801  ................
-00006730: 1001 1801 0c01 0c02 0c02 1001 0e02 0e03  ................
-00006740: 1232                                     .2
+00000080: 6d0e 5a0e 0100 6400 6405 6c0f 6d10 5a10  m.Z...d.d.l.m.Z.
+00000090: 0100 6400 6406 6c11 6d12 5a12 0100 6407  ..d.d.l.m.Z...d.
+000000a0: 6408 6c13 6d14 5a14 0100 6407 6409 6c15  d.l.m.Z...d.d.l.
+000000b0: 6d16 5a16 6d17 5a17 0100 6516 6518 6502  m.Z.m.Z...e.e.e.
+000000c0: 6a19 640a 8d02 5a1a 4700 640b 640c 8400  j.d...Z.G.d.d...
+000000d0: 640c 8302 5a1b 4700 640d 640e 8400 640e  d...Z.G.d.d...d.
+000000e0: 8302 5a1c 6402 5300 290f e900 0000 0029  ..Z.d.S.)......)
+000000f0: 01da 0b61 6e6e 6f74 6174 696f 6e73 4e29  ...annotationsN)
+00000100: 02da 0768 6561 7070 6f70 da08 6865 6170  ...heappop..heap
+00000110: 7075 7368 2903 da03 416e 79da 0843 616c  push)...Any..Cal
+00000120: 6c61 626c 65da 0853 6571 7565 6e63 6529  lable..Sequence)
+00000130: 01da 0575 7569 6434 2901 da04 7471 646d  ...uuid4)...tqdm
+00000140: e901 0000 0029 01da 034a 6f62 2902 da0a  .....)...Job)...
+00000150: 6765 745f 6c6f 6767 6572 da0d 6973 5f77  get_logger..is_w
+00000160: 696e 646f 7773 5f6f 7329 01da 056c 6576  indows_os)...lev
+00000170: 656c 6300 0000 0000 0000 0000 0000 0000  elc.............
+00000180: 0000 0004 0000 0040 0000 0173 5000 0000  .......@...sP...
+00000190: 6500 5a01 6400 5a02 6418 6408 6409 8404  e.Z.d.Z.d.d.d...
+000001a0: 5a03 6419 640c 640d 8404 5a04 6419 640e  Z.d.d.d...Z.d.d.
+000001b0: 640f 8404 5a05 6419 6410 6411 8404 5a06  d...Z.d.d.d...Z.
+000001c0: 6507 641a 6413 6414 8404 8301 5a08 6507  e.d.d.d.....Z.e.
+000001d0: 641a 6415 6416 8404 8301 5a09 6417 5300  d.d.d.....Z.d.S.
+000001e0: 291b da0a 5075 6c73 6554 696d 6572 da04  )...PulseTimer..
+000001f0: 6172 6773 7205 0000 00da 0b69 6e74 6572  argsr......inter
+00000200: 7661 6c5f 6d73 da03 696e 74da 0366 756e  val_ms..int..fun
+00000210: fa12 4361 6c6c 6162 6c65 5b2e 2e2e 2c20  ..Callable[..., 
+00000220: 416e 795d da06 6b77 6172 6773 6301 0000  Any]..kwargsc...
+00000230: 0000 0000 0002 0000 0005 0000 0002 0000  ................
+00000240: 004f 0000 0173 2e00 0000 6400 7c00 5f00  .O...s....d.|._.
+00000250: 7c01 7c00 5f01 7c02 7c00 5f02 7c03 7c00  |.|._.|.|._.|.|.
+00000260: 5f03 7c04 7c00 5f04 6401 7c00 5f05 6401  _.|.|._.d.|._.d.
+00000270: 7c00 5f06 6400 5300 a902 4e46 2907 da06  |._.d.S...NF)...
+00000280: 5f74 696d 6572 da09 5f69 6e74 6572 7661  _timer.._interva
+00000290: 6cda 095f 6675 6e63 7469 6f6e da05 5f61  l.._function.._a
+000002a0: 7267 73da 075f 6b77 6172 6773 da0b 5f69  rgs.._kwargs.._i
+000002b0: 735f 656e 6162 6c65 64da 0b5f 6973 5f72  s_enabled.._is_r
+000002c0: 756e 6e69 6e67 2905 da04 7365 6c66 7211  unning)...selfr.
+000002d0: 0000 0072 1300 0000 7210 0000 0072 1500  ...r....r....r..
+000002e0: 0000 a900 721f 0000 00fa 1f2f 6472 6f6e  ....r....../dron
+000002f0: 652f 7372 632f 7372 632f 7070 7175 6575  e/src/src/ppqueu
+00000300: 652f 7175 6575 652e 7079 da08 5f5f 696e  e/queue.py..__in
+00000310: 6974 5f5f 1800 0000 730e 0000 0006 0706  it__....s.......
+00000320: 0106 0106 0106 0106 010a 017a 1350 756c  ...........z.Pul
+00000330: 7365 5469 6d65 722e 5f5f 696e 6974 5f5f  seTimer.__init__
+00000340: da06 7265 7475 726e da04 4e6f 6e65 6301  ..return..Nonec.
+00000350: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000360: 0000 0043 0000 0173 2600 0000 6401 7c00  ...C...s&...d.|.
+00000370: 5f00 7c00 a001 a100 0100 7c00 6a02 7c00  _.|.......|.j.|.
+00000380: 6a03 6900 7c00 6a04 a401 8e01 0100 6400  j.i.|.j.......d.
+00000390: 5300 7216 0000 0029 0572 1d00 0000 da05  S.r....).r......
+000003a0: 7374 6172 7472 1900 0000 721a 0000 0072  startr....r....r
+000003b0: 1b00 0000 a901 721e 0000 0072 1f00 0000  ......r....r....
+000003c0: 721f 0000 0072 2000 0000 da04 5f72 756e  r....r ....._run
+000003d0: 2700 0000 7306 0000 0006 0108 0118 017a  '...s..........z
+000003e0: 0f50 756c 7365 5469 6d65 722e 5f72 756e  .PulseTimer._run
+000003f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00000400: 0004 0000 0043 0000 0173 3600 0000 7c00  .....C...s6...|.
+00000410: 6a00 7316 7401 a002 7c00 6a03 6401 1b00  j.s.t...|.j.d...
+00000420: 7c00 6a04 a102 7c00 5f05 7c00 6a05 a006  |.j...|._.|.j...
+00000430: a100 0100 6402 7c00 5f00 6402 7c00 5f07  ....d.|._.d.|._.
+00000440: 6400 5300 2903 4ee9 e803 0000 5429 0872  d.S.).N.....T).r
+00000450: 1d00 0000 da09 7468 7265 6164 696e 67da  ......threading.
+00000460: 0554 696d 6572 7218 0000 0072 2600 0000  .Timerr....r&...
+00000470: 7217 0000 0072 2400 0000 721c 0000 0072  r....r$...r....r
+00000480: 2500 0000 721f 0000 0072 1f00 0000 7220  %...r....r....r 
+00000490: 0000 0072 2400 0000 2c00 0000 730a 0000  ...r$...,...s...
+000004a0: 0006 0116 010a 0106 010a 027a 1050 756c  ...........z.Pul
+000004b0: 7365 5469 6d65 722e 7374 6172 7463 0100  seTimer.startc..
+000004c0: 0000 0000 0000 0000 0000 0100 0000 0200  ................
+000004d0: 0000 4300 0001 7324 0000 007c 006a 0064  ..C...s$...|.j.d
+000004e0: 0075 0172 0a7c 006a 00a0 01a1 0001 0064  .u.r.|.j.......d
+000004f0: 017c 005f 0264 017c 005f 0364 0053 0072  .|._.d.|._.d.S.r
+00000500: 1600 0000 2904 7217 0000 00da 0663 616e  ....).r......can
+00000510: 6365 6c72 1c00 0000 721d 0000 0072 2500  celr....r....r%.
+00000520: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00000530: 00da 0473 746f 7034 0000 0073 0800 0000  ...stop4...s....
+00000540: 0a01 0a01 0602 0a01 7a0f 5075 6c73 6554  ........z.PulseT
+00000550: 696d 6572 2e73 746f 70da 0462 6f6f 6c63  imer.stop..boolc
+00000560: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000570: 0100 0000 4300 0001 f306 0000 007c 006a  ....C........|.j
+00000580: 0053 00a9 014e 2901 721d 0000 0072 2500  .S...N).r....r%.
+00000590: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+000005a0: 00da 0a69 735f 7275 6e6e 696e 673b 0000  ...is_running;..
+000005b0: 00f3 0200 0000 0602 7a15 5075 6c73 6554  ........z.PulseT
+000005c0: 696d 6572 2e69 735f 7275 6e6e 696e 6763  imer.is_runningc
+000005d0: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+000005e0: 0100 0000 4300 0001 722d 0000 0072 2e00  ....C...r-...r..
+000005f0: 0000 2901 721c 0000 0072 2500 0000 721f  ..).r....r%...r.
+00000600: 0000 0072 1f00 0000 7220 0000 00da 0a69  ...r....r .....i
+00000610: 735f 656e 6162 6c65 643f 0000 0072 3000  s_enabled?...r0.
+00000620: 0000 7a15 5075 6c73 6554 696d 6572 2e69  ..z.PulseTimer.i
+00000630: 735f 656e 6162 6c65 644e 2908 7210 0000  s_enabledN).r...
+00000640: 0072 0500 0000 7211 0000 0072 1200 0000  .r....r....r....
+00000650: 7213 0000 0072 1400 0000 7215 0000 0072  r....r....r....r
+00000660: 0500 0000 a902 7222 0000 0072 2300 0000  ......r"...r#...
+00000670: a902 7222 0000 0072 2c00 0000 290a da08  ..r"...r,...)...
+00000680: 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f 6475  __name__..__modu
+00000690: 6c65 5f5f da0c 5f5f 7175 616c 6e61 6d65  le__..__qualname
+000006a0: 5f5f 7221 0000 0072 2600 0000 7224 0000  __r!...r&...r$..
+000006b0: 0072 2b00 0000 da08 7072 6f70 6572 7479  .r+.....property
+000006c0: 722f 0000 0072 3100 0000 721f 0000 0072  r/...r1...r....r
+000006d0: 1f00 0000 721f 0000 0072 2000 0000 720f  ....r....r ...r.
+000006e0: 0000 0014 0000 0073 1200 0000 0800 0a04  .......s........
+000006f0: 0a0f 0a05 0a08 0207 0c01 0203 1001 720f  ..............r.
+00000700: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000710: 0000 0000 0b00 0000 4000 0001 735e 0200  ........@...s^..
+00000720: 0065 005a 0164 005a 0255 0064 015a 0364  .e.Z.d.Z.U.d.Z.d
+00000730: 0265 0464 033c 0065 05a0 06a1 0066 0164  .e.d.<.e.....f.d
+00000740: 0465 056a 0764 0164 0164 0564 0564 0564  .e.j.d.d.d.d.d.d
+00000750: 0664 0564 079c 0964 9664 1764 1884 075a  .d.d...d.d.d...Z
+00000760: 0864 9764 1e64 1f84 045a 0964 9864 2264  .d.d.d...Z.d.d"d
+00000770: 2384 045a 0a64 9864 2464 2584 045a 0b64  #..Z.d.d$d%..Z.d
+00000780: 9864 2664 2784 045a 0c64 9864 2864 2984  .d&d'..Z.d.d(d).
+00000790: 045a 0d64 9864 2a64 2b84 045a 0e64 2c64  .Z.d.d*d+..Z.d,d
+000007a0: 2d9c 0164 9964 2f64 3084 065a 0f64 9a64  -..d.d/d0..Z.d.d
+000007b0: 3164 3284 045a 1064 9b64 3364 3484 045a  1d2..Z.d.d3d4..Z
+000007c0: 1164 9a64 3564 3684 045a 1264 9c64 3864  .d.d5d6..Z.d.d8d
+000007d0: 3984 045a 1364 9864 3a64 3b84 045a 1464  9..Z.d.d:d;..Z.d
+000007e0: 9d64 3c64 3d84 045a 1564 9d64 3e64 3f84  .d<d=..Z.d.d>d?.
+000007f0: 045a 1664 9d64 4064 4184 045a 1764 9d64  .Z.d.d@dA..Z.d.d
+00000800: 4264 4384 045a 1864 0564 0564 0564 449c  BdC..Z.d.d.d.dD.
+00000810: 0364 9e64 4964 4a84 065a 1964 9d64 4b64  .d.dIdJ..Z.d.dKd
+00000820: 4c84 045a 1a64 0564 0564 0564 449c 0364  L..Z.d.d.d.dD..d
+00000830: 9f64 4d64 4e84 065a 1b64 a064 4f64 5084  .dMdN..Z.d.dOdP.
+00000840: 045a 1c64 a064 5164 5284 045a 1d64 a064  .Z.d.dQdR..Z.d.d
+00000850: 5364 5484 045a 1e64 a064 5564 5684 045a  SdT..Z.d.dUdV..Z
+00000860: 1f64 9d64 5764 5884 045a 2064 0464 0464  .d.dWdX..Z d.d.d
+00000870: 0464 0164 599c 0464 a164 5f64 6084 065a  .d.dY..d.d_d`..Z
+00000880: 2165 2264 a264 6564 6684 0483 015a 2364  !e"d.dedf....Z#d
+00000890: a364 6864 6984 045a 2464 a464 6a64 6b84  .dhdi..Z$d.djdk.
+000008a0: 045a 2509 0109 0109 0109 0609 0109 0409  .Z%.............
+000008b0: 0509 0564 a564 a664 7264 7384 055a 2664  ...d.d.drds..Z&d
+000008c0: 9d64 7464 7584 045a 2764 0464 0164 769c  .dtdu..Z'd.d.dv.
+000008d0: 0264 a764 7a64 7b84 065a 2864 0464 0164  .d.dzd{..Z(d.d.d
+000008e0: 769c 0264 a864 7d64 7e84 065a 2964 0464  v..d.d}d~..Z)d.d
+000008f0: 0164 769c 0264 a964 8064 8184 065a 2a64  .dv..d.d.d...Z*d
+00000900: 0564 0564 829c 0264 aa64 8564 8684 065a  .d.d...d.d.d...Z
+00000910: 2b64 ab64 8764 8884 045a 2c64 ab64 8964  +d.d.d...Z,d.d.d
+00000920: 8a84 045a 2d64 ac64 ad64 8b64 8c84 055a  ...Z-d.d.d.d...Z
+00000930: 2e65 2f64 9d64 8d64 8e84 0483 015a 3065  .e/d.d.d.....Z0e
+00000940: 306a 3164 ae64 9064 8e84 0483 015a 3065  0j1d.d.d.....Z0e
+00000950: 2f64 9d64 9164 9284 0483 015a 3265 326a  /d.d.d.....Z2e2j
+00000960: 3164 af64 9364 9284 0483 015a 3265 2f64  1d.d.d.....Z2e/d
+00000970: a064 9464 9584 0483 015a 3364 0153 0029  .d.d.....Z3d.S.)
+00000980: b0da 0551 7565 7565 4efa 0a69 6e74 207c  ...QueueN..int |
+00000990: 204e 6f6e 65da 0d44 4546 4155 4c54 5f47   None..DEFAULT_G
+000009a0: 524f 5550 7201 0000 0046 e964 0000 0029  ROUPr....F.d...)
+000009b0: 09da 086d 6178 5f73 697a 65da 0665 6e67  ...max_size..eng
+000009c0: 696e 65da 046e 616d 65da 0863 616c 6c62  ine..name..callb
+000009d0: 6163 6bda 0d73 686f 775f 7072 6f67 7265  ack..show_progre
+000009e0: 7373 da0d 6472 6f70 5f66 696e 6973 6865  ss..drop_finishe
+000009f0: 64da 0e73 746f 705f 7768 656e 5f69 646c  d..stop_when_idl
+00000a00: 65da 0d70 756c 7365 5f66 7265 715f 6d73  e..pulse_freq_ms
+00000a10: da08 6e6f 5f73 7461 7274 da0e 6d61 785f  ..no_start..max_
+00000a20: 636f 6e63 7572 7265 6e74 7212 0000 0072  concurrentr....r
+00000a30: 3c00 0000 723d 0000 00fa 2f73 7472 207c  <...r=..../str |
+00000a40: 2074 7970 655b 6d70 2e50 726f 6365 7373   type[mp.Process
+00000a50: 5d20 7c20 7479 7065 5b74 6872 6561 6469  ] | type[threadi
+00000a60: 6e67 2e54 6872 6561 645d 723e 0000 00fa  ng.Thread]r>....
+00000a70: 0a73 7472 207c 204e 6f6e 6572 3f00 0000  .str | Noner?...
+00000a80: fa1b 4361 6c6c 6162 6c65 5b5b 4a6f 625d  ..Callable[[Job]
+00000a90: 2c20 416e 795d 207c 204e 6f6e 6572 4000  , Any] | Noner@.
+00000aa0: 0000 722c 0000 0072 4100 0000 7242 0000  ..r,...rA...rB..
+00000ab0: 0072 4300 0000 7244 0000 0063 0200 0000  .rC...rD...c....
+00000ac0: 0000 0000 0900 0000 0c00 0000 0400 0000  ................
+00000ad0: 4300 0001 7348 0100 007c 0472 047c 046e  C...sH...|.r.|.n
+00000ae0: 0874 0074 0183 0083 0164 0164 0285 0219  .t.t.....d.d....
+00000af0: 007c 005f 027c 067c 005f 037c 027c 005f  .|._.|.|._.|.|._
+00000b00: 0464 037c 005f 0564 037c 005f 067c 017c  .d.|._.d.|._.|.|
+00000b10: 005f 077c 057c 005f 0874 09a0 0aa1 007c  ._.|.|._.t.....|
+00000b20: 005f 0b74 0c7c 0374 0083 0272 487c 03a0  ._.t.|.t...rH|..
+00000b30: 0da1 0064 0476 0072 3474 096a 0e7d 036e  ...d.v.r4t.j.}.n
+00000b40: 147c 03a0 0da1 0064 0576 0072 3e74 0f6a  .|.....d.v.r>t.j
+00000b50: 107d 036e 0a64 067c 039b 0064 079d 037d  .}.n.d.|...d...}
+00000b60: 0b74 117c 0b83 0182 017c 0374 0f6a 1075  .t.|.....|.t.j.u
+00000b70: 0072 5574 1283 0072 5574 13a0 1464 08a1  .rUt...rUt...d..
+00000b80: 0101 007c 037c 005f 157c 006a 1667 0069  ...|.|._.|.j.g.i
+00000b90: 017c 005f 1769 007c 005f 1867 007c 005f  .|._.i.|._.g.|._
+00000ba0: 197c 077c 005f 1a64 017c 005f 1b7c 0001  .|.|._.d.|._.|..
+00000bb0: 007c 006a 1574 0f6a 1075 0072 7e74 0fa0  .|.j.t.j.u.r~t..
+00000bc0: 1ca1 007c 005f 1b7c 006a 1ba0 1da1 007c  ...|._.|.j.....|
+00000bd0: 005f 1e6e 0369 007c 005f 1e74 13a0 1f64  ._.n.i.|._.t...d
+00000be0: 097c 006a 07a1 0201 007c 097c 005f 2074  .|.j.....|.|._ t
+00000bf0: 217c 006a 207c 006a 2264 0a8d 027c 005f  !|.j |.j"d...|._
+00000c00: 237c 087c 005f 247c 0a73 9d7c 00a0 25a1  #|.|._$|.s.|..%.
+00000c10: 0001 0074 13a0 1f64 0ba1 0101 0064 0153  ...t...d.....d.S
+00000c20: 0029 0c61 4804 0000 4120 7061 7261 6c6c  .).aH...A parall
+00000c30: 656c 2070 726f 6365 7373 696e 6720 6a6f  el processing jo
+00000c40: 6220 7275 6e6e 6572 202f 2064 6174 6120  b runner / data 
+00000c50: 7374 7275 6374 7572 652e 0a0a 2020 2020  structure...    
+00000c60: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00000c70: 2020 2020 2020 6d61 785f 636f 6e63 7572        max_concur
+00000c80: 7265 6e74 3a20 6d61 7820 6e75 6d62 6572  rent: max number
+00000c90: 206f 6620 636f 6e63 7572 7265 6e74 6c79   of concurrently
+00000ca0: 2072 756e 6e69 6e67 206a 6f62 732e 0a20   running jobs.. 
+00000cb0: 2020 2020 2020 2020 2020 206d 6178 5f73             max_s
+00000cc0: 697a 653a 206d 6178 2073 697a 6520 6f66  ize: max size of
+00000cd0: 2074 6865 2071 7565 7565 2028 6465 6661   the queue (defa
+00000ce0: 756c 743d 302c 2075 6e6c 696d 6974 6564  ult=0, unlimited
+00000cf0: 292e 0a20 2020 2020 2020 2020 2020 2065  )..            e
+00000d00: 6e67 696e 653a 2074 6865 2065 6e67 696e  ngine: the engin
+00000d10: 6520 7573 6564 2074 6f20 7275 6e20 6a6f  e used to run jo
+00000d20: 6273 2e0a 2020 2020 2020 2020 2020 2020  bs..            
+00000d30: 6e61 6d65 3a20 616e 2069 6465 6e74 6966  name: an identif
+00000d40: 6965 7220 666f 7220 7468 6973 2071 7565  ier for this que
+00000d50: 7565 2e0a 2020 2020 2020 2020 2020 2020  ue..            
+00000d60: 6361 6c6c 6261 636b 3a20 6120 6361 6c6c  callback: a call
+00000d70: 6162 6c65 2074 6861 7420 6973 2063 616c  able that is cal
+00000d80: 6c65 6420 696d 6d65 6469 6174 656c 7920  led immediately 
+00000d90: 6166 7465 7220 6561 6368 206a 6f62 2069  after each job i
+00000da0: 7320 6669 6e69 7368 6564 2e0a 2020 2020  s finished..    
+00000db0: 2020 2020 2020 2020 7368 6f77 5f70 726f          show_pro
+00000dc0: 6772 6573 733a 2067 6c6f 6261 6c20 7365  gress: global se
+00000dd0: 7474 696e 6720 666f 7220 7368 6f77 696e  tting for showin
+00000de0: 6720 7072 6f67 7265 7373 2062 6172 732e  g progress bars.
+00000df0: 0a20 2020 2020 2020 2020 2020 2064 726f  .            dro
+00000e00: 705f 6669 6e69 7368 6564 3a20 6966 2054  p_finished: if T
+00000e10: 7275 652c 2074 6865 2071 7565 7565 2077  rue, the queue w
+00000e20: 696c 6c20 6e6f 7420 7374 6f72 6520 6669  ill not store fi
+00000e30: 6e69 7368 6564 206a 6f62 7320 666f 7220  nished jobs for 
+00000e40: 7265 7472 6965 7661 6c2e 0a20 2020 2020  retrieval..     
+00000e50: 2020 2020 2020 2073 746f 705f 7768 656e         stop_when
+00000e60: 5f69 646c 653a 2069 6620 5472 7565 2c20  _idle: if True, 
+00000e70: 7468 6520 7175 6575 6520 7769 6c6c 2073  the queue will s
+00000e80: 746f 7020 7468 6520 7075 6c73 6520 7768  top the pulse wh
+00000e90: 656e 2061 6c6c 206a 6f62 7320 6172 6520  en all jobs are 
+00000ea0: 6669 6e69 7368 6564 2e0a 2020 2020 2020  finished..      
+00000eb0: 2020 2020 2020 7075 6c73 655f 6672 6571        pulse_freq
+00000ec0: 5f6d 733a 2074 6865 2069 6e74 6572 7661  _ms: the interva
+00000ed0: 6c20 6174 2077 6869 6368 206a 6f62 7320  l at which jobs 
+00000ee0: 6172 6520 7472 616e 7369 7469 6f6e 6564  are transitioned
+00000ef0: 2062 6574 7765 656e 2069 6e74 6572 6e61   between interna
+00000f00: 6c20 7175 6575 6573 2e0a 2020 2020 2020  l queues..      
+00000f10: 2020 2020 2020 6e6f 5f73 7461 7274 3a20        no_start: 
+00000f20: 6966 2054 7275 652c 2064 6f20 6e6f 7420  if True, do not 
+00000f30: 7374 6172 7420 7468 6520 7175 6575 6520  start the queue 
+00000f40: 7075 6c73 6520 6f6e 2069 6e73 7461 6e74  pulse on instant
+00000f50: 6961 7469 6f6e 2e0a 0a20 2020 2020 2020  iation...       
+00000f60: 2045 7861 6d70 6c65 733a 0a20 2020 2020   Examples:.     
+00000f70: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
+00000f80: 7070 7175 6575 6520 696d 706f 7274 2051  ppqueue import Q
+00000f90: 7565 7565 0a20 2020 2020 2020 2020 2020  ueue.           
+00000fa0: 203e 3e3e 2066 726f 6d20 7469 6d65 2069   >>> from time i
+00000fb0: 6d70 6f72 7420 736c 6565 700a 2020 2020  mport sleep.    
+00000fc0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00000fd0: 2020 2020 2020 2020 3e3e 3e20 7769 7468          >>> with
+00000fe0: 2051 7565 7565 2829 2061 7320 7175 6575   Queue() as queu
+00000ff0: 653a 0a20 2020 2020 2020 2020 2020 202e  e:.            .
+00001000: 2e2e 2020 2020 206a 6f62 7320 3d20 7175  ..     jobs = qu
+00001010: 6575 652e 6d61 7028 736c 6565 702c 205b  eue.map(sleep, [
+00001020: 312c 2032 2c20 332c 2034 2c20 355d 290a  1, 2, 3, 4, 5]).
+00001030: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00001040: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00001050: 6c65 6e28 6a6f 6273 290a 2020 2020 2020  len(jobs).      
+00001060: 2020 2020 2020 350a 2020 2020 2020 2020        5.        
+00001070: 4ee9 0800 0000 7201 0000 0029 03da 0674  N.....r....)...t
+00001080: 6872 6561 64da 0774 6872 6561 6473 7228  hread..threadsr(
+00001090: 0000 0029 04da 0770 726f 6365 7373 da09  ...)...process..
+000010a0: 7072 6f63 6573 7365 735a 0a70 726f 6365  processesZ.proce
+000010b0: 7373 696e 67da 0f6d 756c 7469 7072 6f63  ssing..multiproc
+000010c0: 6573 7369 6e67 7a15 556e 7265 636f 676e  essingz.Unrecogn
+000010d0: 697a 6564 2065 6e67 696e 653a 207a 262e  ized engine: z&.
+000010e0: 2043 686f 6f73 6520 6569 7468 6572 2027   Choose either '
+000010f0: 7072 6f63 6573 7327 206f 7220 2774 6872  process' or 'thr
+00001100: 6561 6427 2e7a b06d 756c 7469 7072 6f63  ead'.z.multiproc
+00001110: 6573 7369 6e67 2070 6572 666f 726d 616e  essing performan
+00001120: 6365 2069 7320 6465 6772 6164 6564 206f  ce is degraded o
+00001130: 6e20 5769 6e64 6f77 7320 7379 7374 656d  n Windows system
+00001140: 732e 2073 6565 3a20 6874 7470 733a 2f2f  s. see: https://
+00001150: 646f 6373 2e70 7974 686f 6e2e 6f72 672f  docs.python.org/
+00001160: 332f 6c69 6272 6172 792f 6d75 6c74 6970  3/library/multip
+00001170: 726f 6365 7373 696e 672e 6874 6d6c 3f68  rocessing.html?h
+00001180: 6967 686c 6967 6874 3d70 726f 6365 7373  ighlight=process
+00001190: 2374 6865 2d73 7061 776e 2d61 6e64 2d66  #the-spawn-and-f
+000011a0: 6f72 6b73 6572 7665 722d 7374 6172 742d  orkserver-start-
+000011b0: 6d65 7468 6f64 737a 2949 6e69 7469 616c  methodsz)Initial
+000011c0: 697a 6564 2071 7565 7565 2077 6974 6820  ized queue with 
+000011d0: 2564 206d 6178 5f63 6f6e 6375 7272 656e  %d max_concurren
+000011e0: 742e 2902 7211 0000 0072 1300 0000 7a12  t.).r....r....z.
+000011f0: 496e 6974 6961 6c69 7a65 6420 7075 6c73  Initialized puls
+00001200: 652e 2926 da03 7374 7272 0800 0000 da04  e.)&..strr......
+00001210: 5f71 6964 7240 0000 00da 095f 6d61 785f  _qidr@....._max_
+00001220: 7369 7a65 da0c 5f63 6f75 6e74 5f69 6e70  size.._count_inp
+00001230: 7574 da0d 5f63 6f75 6e74 5f6f 7574 7075  ut.._count_outpu
+00001240: 74da 0f5f 6d61 785f 636f 6e63 7572 7265  t.._max_concurre
+00001250: 6e74 da09 5f63 616c 6c62 6163 6b72 2800  nt.._callbackr(.
+00001260: 0000 da04 4c6f 636b da05 5f6c 6f63 6bda  ....Lock.._lock.
+00001270: 0a69 7369 6e73 7461 6e63 65da 056c 6f77  .isinstance..low
+00001280: 6572 da06 5468 7265 6164 da02 6d70 da07  er..Thread..mp..
+00001290: 5072 6f63 6573 73da 0a56 616c 7565 4572  Process..ValueEr
+000012a0: 726f 7272 0d00 0000 da03 4c4f 47da 0777  rorr......LOG..w
+000012b0: 6172 6e69 6e67 da07 5f65 6e67 696e 6572  arning.._enginer
+000012c0: 3a00 0000 da0f 5f77 6169 7469 6e67 5f67  :....._waiting_g
+000012d0: 726f 7570 73da 0e5f 776f 726b 696e 675f  roups.._working_
+000012e0: 7175 6575 65da 0f5f 6669 6e69 7368 6564  queue.._finished
+000012f0: 5f71 7565 7565 da0e 5f64 726f 705f 6669  _queue.._drop_fi
+00001300: 6e69 7368 6564 da0b 5f6d 705f 6d61 6e61  nished.._mp_mana
+00001310: 6765 72da 074d 616e 6167 6572 da04 6469  ger..Manager..di
+00001320: 6374 da07 5f6f 7574 7075 74da 0564 6562  ct.._output..deb
+00001330: 7567 da0e 5f70 756c 7365 5f66 7265 715f  ug.._pulse_freq_
+00001340: 6d73 720f 0000 00da 065f 7075 6c73 6572  msr......_pulser
+00001350: 1700 0000 da0f 5f73 746f 705f 7768 656e  ......_stop_when
+00001360: 5f69 646c 6572 2400 0000 290c 721e 0000  _idler$...).r...
+00001370: 0072 4500 0000 723c 0000 0072 3d00 0000  .rE...r<...r=...
+00001380: 723e 0000 0072 3f00 0000 7240 0000 0072  r>...r?...r@...r
+00001390: 4100 0000 7242 0000 0072 4300 0000 7244  A...rB...rC...rD
+000013a0: 0000 00da 0365 7272 721f 0000 0072 1f00  .....errr....r..
+000013b0: 0000 7220 0000 0072 2100 0000 4700 0000  ..r ...r!...G...
+000013c0: 7350 0000 001c 2706 0206 0106 0106 0106  sP....'.........
+000013d0: 0106 010a 030a 020c 0108 010c 0108 060c  ................
+000013e0: 0208 0110 0204 0102 0204 fe06 070c 0206  ................
+000013f0: 0106 0106 0206 0104 020c 020a 010e 0106  ................
+00001400: 020e 0206 0202 0104 0104 0108 fe06 0504  ................
+00001410: 0208 010e 027a 0e51 7565 7565 2e5f 5f69  .....z.Queue.__i
+00001420: 6e69 745f 5f72 1300 0000 7214 0000 0072  nit__r....r....r
+00001430: 1000 0000 7205 0000 0072 1500 0000 6302  ....r....r....c.
+00001440: 0000 0000 0000 0000 0000 0005 0000 0004  ................
+00001450: 0000 000f 0000 0173 1c00 0000 8801 a000  .......s........
+00001460: a100 0100 640a 8700 8701 6602 6408 6409  ....d.....f.d.d.
+00001470: 840c 7d04 7c04 5300 290b 4eda 0869 7465  ..}.|.S.).N..ite
+00001480: 7261 626c 65fa 0d53 6571 7565 6e63 655b  rable..Sequence[
+00001490: 416e 795d 7210 0000 0072 0500 0000 7215  Any]r....r....r.
+000014a0: 0000 0072 2200 0000 fa09 6c69 7374 5b4a  ...r".....list[J
+000014b0: 6f62 5d63 0100 0000 0000 0000 0000 0000  ob]c............
+000014c0: 0500 0000 0600 0000 1f00 0001 733c 0000  ............s<..
+000014d0: 007c 0044 005d 0d7d 0388 016a 0088 007c  .|.D.].}...j...|
+000014e0: 0367 017c 01a2 017c 0264 018d 0301 0071  .g.|...|.d.....q
+000014f0: 0288 01a0 01a1 0001 0088 01a0 02a1 007d  ...............}
+00001500: 0488 01a0 03a1 0001 007c 0453 0029 024e  .........|.S.).N
+00001510: 2902 7210 0000 0072 1500 0000 2904 da07  ).r....r....)...
+00001520: 656e 7175 6575 65da 0477 6169 74da 0763  enqueue..wait..c
+00001530: 6f6c 6c65 6374 da07 6469 7370 6f73 6529  ollect..dispose)
+00001540: 0572 6e00 0000 7210 0000 0072 1500 0000  .rn...r....r....
+00001550: da01 78da 086a 6f62 5f64 6174 61a9 0272  ..x..job_data..r
+00001560: 1300 0000 721e 0000 0072 1f00 0000 7220  ....r....r....r 
+00001570: 0000 00da 0977 7261 7070 6564 5f66 b400  .....wrapped_f..
+00001580: 0000 730c 0000 0008 0118 0108 0108 0108  ..s.............
+00001590: 0104 017a 2151 7565 7565 2e5f 5f63 616c  ...z!Queue.__cal
+000015a0: 6c5f 5f2e 3c6c 6f63 616c 733e 2e77 7261  l__.<locals>.wra
+000015b0: 7070 6564 5f66 2908 726e 0000 0072 6f00  pped_f).rn...ro.
+000015c0: 0000 7210 0000 0072 0500 0000 7215 0000  ..r....r....r...
+000015d0: 0072 0500 0000 7222 0000 0072 7000 0000  .r....r"...rp...
+000015e0: 2901 7224 0000 0029 0572 1e00 0000 7213  ).r$...).r....r.
+000015f0: 0000 0072 1000 0000 7215 0000 0072 7800  ...r....r....rx.
+00001600: 0000 721f 0000 0072 7700 0000 7220 0000  ..r....rw...r ..
+00001610: 00da 085f 5f63 616c 6c5f 5fb1 0000 0073  ...__call__....s
+00001620: 0600 0000 0801 1002 0408 7a0e 5175 6575  ..........z.Queu
+00001630: 652e 5f5f 6361 6c6c 5f5f 7222 0000 0072  e.__call__r"...r
+00001640: 2300 0000 6301 0000 0000 0000 0000 0000  #...c...........
+00001650: 0001 0000 0002 0000 0043 0000 01f3 0c00  .........C......
+00001660: 0000 7c00 a000 a100 0100 6400 5300 722e  ..|.......d.S.r.
+00001670: 0000 00a9 0172 7400 0000 7225 0000 0072  .....rt...r%...r
+00001680: 1f00 0000 721f 0000 0072 2000 0000 da07  ....r....r .....
+00001690: 5f5f 6465 6c5f 5fbe 0000 00f3 0200 0000  __del__.........
+000016a0: 0c01 7a0d 5175 6575 652e 5f5f 6465 6c5f  ..z.Queue.__del_
+000016b0: 5f63 0100 0000 0000 0000 0000 0000 0100  _c..............
+000016c0: 0000 0200 0000 4300 0001 f30e 0000 007c  ......C........|
+000016d0: 006a 00a0 01a1 0001 0064 0153 0029 027a  .j.......d.S.).z
+000016e0: 1653 7461 7274 2074 6865 2071 7565 7565  .Start the queue
+000016f0: 2070 756c 7365 2e4e 2902 7217 0000 0072   pulse.N).r....r
+00001700: 2400 0000 7225 0000 0072 1f00 0000 721f  $...r%...r....r.
+00001710: 0000 0072 2000 0000 7224 0000 00c1 0000  ...r ...r$......
+00001720: 00f3 0200 0000 0e02 7a0b 5175 6575 652e  ........z.Queue.
+00001730: 7374 6172 7463 0100 0000 0000 0000 0000  startc..........
+00001740: 0000 0100 0000 0200 0000 4300 0001 727e  ..........C...r~
+00001750: 0000 0029 027a 1553 746f 7020 7468 6520  ...).z.Stop the 
+00001760: 7175 6575 6520 7075 6c73 652e 4e29 0272  queue pulse.N).r
+00001770: 1700 0000 722b 0000 0072 2500 0000 721f  ....r+...r%...r.
+00001780: 0000 0072 1f00 0000 7220 0000 0072 2b00  ...r....r ...r+.
+00001790: 0000 c500 0000 727f 0000 007a 0a51 7565  ......r....z.Que
+000017a0: 7565 2e73 746f 7063 0100 0000 0000 0000  ue.stopc........
+000017b0: 0000 0000 0100 0000 0300 0000 4300 0001  ............C...
+000017c0: 7384 0000 0074 00a0 0164 01a1 0101 007c  s....t...d.....|
+000017d0: 006a 0272 127c 006a 0364 0264 038d 0101  .j.r.|.j.d.d....
+000017e0: 007c 00a0 04a1 0001 0074 00a0 0164 04a1  .|.......t...d..
+000017f0: 0101 0064 057c 005f 0574 00a0 0164 06a1  ...d.|._.t...d..
+00001800: 0101 007c 006a 06a0 07a1 0001 0074 00a0  ...|.j.......t..
+00001810: 0164 07a1 0101 0064 087c 005f 0864 087c  .d.....d.|._.d.|
+00001820: 005f 0974 00a0 0164 09a1 0101 007c 006a  ._.t...d.....|.j
+00001830: 0a64 0575 0172 407c 006a 0aa0 0ba1 0001  .d.u.r@|.j......
+00001840: 0064 0553 0064 0553 0029 0a7a 4353 746f  .d.S.d.S.).zCSto
+00001850: 7020 7275 6e6e 696e 6720 6a6f 6273 2c20  p running jobs, 
+00001860: 7468 656e 2063 6c65 6172 2074 6865 2071  then clear the q
+00001870: 7565 7565 2c20 7468 656e 2073 746f 7020  ueue, then stop 
+00001880: 7468 6520 7175 6575 6520 7075 6c73 652e  the queue pulse.
+00001890: 5a09 4469 7370 6f73 696e 6754 a901 7272  Z.DisposingT..rr
+000018a0: 0000 007a 0d52 656d 6f76 6564 206a 6f62  ...z.Removed job
+000018b0: 732e 4e7a 0f52 656d 6f76 6564 206f 7574  s.Nz.Removed out
+000018c0: 7075 742e 7a11 5265 6d6f 7665 6420 6669  put.z.Removed fi
+000018d0: 6e69 7368 6564 2e72 0100 0000 7a0f 5265  nished.r....z.Re
+000018e0: 7365 7420 636f 756e 7465 7273 2e29 0c72  set counters.).r
+000018f0: 5e00 0000 7269 0000 0072 2f00 0000 da09  ^...ri...r/.....
+00001900: 5f73 746f 705f 616c 6c72 2b00 0000 7268  _stop_allr+...rh
+00001910: 0000 0072 6300 0000 da05 636c 6561 7272  ...rc.....clearr
+00001920: 5200 0000 7253 0000 0072 6500 0000 da08  R...rS...re.....
+00001930: 7368 7574 646f 776e 7225 0000 0072 1f00  shutdownr%...r..
+00001940: 0000 721f 0000 0072 2000 0000 7274 0000  ..r....r ...rt..
+00001950: 00c9 0000 0073 1e00 0000 0a02 0602 0c01  .....s..........
+00001960: 0801 0a02 0601 0a01 0a01 0a01 0601 0601  ................
+00001970: 0a01 0a02 0e01 04ff 7a0d 5175 6575 652e  ........z.Queue.
+00001980: 6469 7370 6f73 6563 0100 0000 0000 0000  disposec........
+00001990: 0000 0000 0600 0000 0800 0000 4300 0001  ............C...
+000019a0: 73ae 0000 0074 00a0 0164 01a1 0101 007c  s....t...d.....|
+000019b0: 006a 028f 4501 0074 037c 006a 04a0 05a1  .j..E..t.|.j....
+000019c0: 0083 017d 017c 0144 005d 327d 027c 006a  ...}.|.D.]2}.|.j
+000019d0: 04a0 067c 02a1 017d 0374 0774 087c 0383  ...|...}.t.t.|..
+000019e0: 0183 0144 005d 1f7d 0474 097c 0383 017d  ...D.].}.t.|...}
+000019f0: 0564 027c 055f 0a74 0ba0 0ba1 007c 055f  .d.|._.t.....|._
+00001a00: 0c7c 006a 0d73 3874 0e7c 006a 0f7c 0583  .|.j.s8t.|.j.|..
+00001a10: 0201 0071 207c 0004 006a 1064 0337 0002  ...q |...j.d.7..
+00001a20: 005f 1071 207c 006a 047c 023d 0071 1257  ._.q |.j.|.=.q.W
+00001a30: 0064 0004 0004 0083 0301 0064 0053 0031  .d.........d.S.1
+00001a40: 0073 5077 0101 0001 0001 0059 0001 0064  .sPw.......Y...d
+00001a50: 0053 0029 044e 7a16 436c 6561 7269 6e67  .S.).Nz.Clearing
+00001a60: 2077 6169 7469 6e67 2071 7565 7565 5472   waiting queueTr
+00001a70: 0a00 0000 2911 725e 0000 0072 6900 0000  ....).r^...ri...
+00001a80: 7257 0000 00da 046c 6973 7472 6100 0000  rW.....listra...
+00001a90: da04 6b65 7973 da03 6765 74da 0572 616e  ..keys..get..ran
+00001aa0: 6765 da03 6c65 6e72 0300 0000 da09 6361  ge..lenr......ca
+00001ab0: 6e63 656c 6c65 64da 0474 696d 65da 1170  ncelled..time..p
+00001ac0: 726f 6365 7373 5f74 696d 6573 7461 6d70  rocess_timestamp
+00001ad0: 7264 0000 0072 0400 0000 7263 0000 0072  rd...r....rc...r
+00001ae0: 5300 0000 2906 721e 0000 0072 8500 0000  S...).r....r....
+00001af0: da01 6bda 0a67 726f 7570 5f6a 6f62 73da  ..k..group_jobs.
+00001b00: 015f da03 6a6f 6272 1f00 0000 721f 0000  ._..jobr....r...
+00001b10: 0072 2000 0000 da0e 5f63 6c65 6172 5f77  .r ....._clear_w
+00001b20: 6169 7469 6e67 dd00 0000 731e 0000 000a  aiting....s.....
+00001b30: 0108 010e 0108 010c 0110 0108 0106 010a  ................
+00001b40: 0106 010e 0110 020a 0102 f622 fe7a 1451  ...........".z.Q
+00001b50: 7565 7565 2e5f 636c 6561 725f 7761 6974  ueue._clear_wait
+00001b60: 696e 6754 7280 0000 0072 7200 0000 6301  ingTr....rr...c.
+00001b70: 0000 0000 0000 0001 0000 0005 0000 0004  ................
+00001b80: 0000 0043 0000 0173 5000 0000 7c00 a000  ...C...sP...|...
+00001b90: a100 0100 7401 7c00 6a02 a003 a100 8301  ....t.|.j.......
+00001ba0: 7d02 7c02 4400 5d10 7d03 7c00 6a02 a004  }.|.D.].}.|.j...
+00001bb0: 7c03 a101 7d04 7c04 6400 7501 721d 7c04  |...}.|.d.u.r.|.
+00001bc0: a005 a100 0100 710d 7c01 7226 7c00 a006  ......q.|.r&|...
+00001bd0: a100 0100 6400 5300 6400 5300 722e 0000  ....d.S.d.S.r...
+00001be0: 0029 0772 9000 0000 7284 0000 0072 6200  .).r....r....rb.
+00001bf0: 0000 7285 0000 0072 8600 0000 722b 0000  ..r....r....r+..
+00001c00: 0072 7200 0000 2905 721e 0000 0072 7200  .rr...).r....rr.
+00001c10: 0000 7285 0000 0072 8c00 0000 728f 0000  ..r....r....r...
+00001c20: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00001c30: 7281 0000 00ed 0000 0073 1400 0000 0801  r........s......
+00001c40: 0e02 0801 0c01 0801 0801 0280 0402 0c01  ................
+00001c50: 04ff 7a0f 5175 6575 652e 5f73 746f 705f  ..z.Queue._stop_
+00001c60: 616c 6c63 0100 0000 0000 0000 0000 0000  allc............
+00001c70: 0100 0000 0100 0000 4300 0001 f304 0000  ........C.......
+00001c80: 007c 0053 0072 2e00 0000 721f 0000 0072  .|.S.r....r....r
+00001c90: 2500 0000 721f 0000 0072 1f00 0000 7220  %...r....r....r 
+00001ca0: 0000 00da 095f 5f65 6e74 6572 5f5f f900  .....__enter__..
+00001cb0: 0000 f302 0000 0004 017a 0f51 7565 7565  .........z.Queue
+00001cc0: 2e5f 5f65 6e74 6572 5f5f 6301 0000 0000  .__enter__c.....
+00001cd0: 0000 0000 0000 0002 0000 0002 0000 0047  ...............G
+00001ce0: 0000 0172 7a00 0000 722e 0000 0072 7b00  ...rz...r....r{.
+00001cf0: 0000 2902 721e 0000 0072 1000 0000 721f  ..).r....r....r.
+00001d00: 0000 0072 1f00 0000 7220 0000 00da 085f  ...r....r ....._
+00001d10: 5f65 7869 745f 5ffc 0000 0072 7d00 0000  _exit__....r}...
+00001d20: 7a0e 5175 6575 652e 5f5f 6578 6974 5f5f  z.Queue.__exit__
+00001d30: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00001d40: 0001 0000 0043 0000 0172 9100 0000 722e  .....C...r....r.
+00001d50: 0000 0072 1f00 0000 7225 0000 0072 1f00  ...r....r%...r..
+00001d60: 0000 721f 0000 0072 2000 0000 da08 5f5f  ..r....r .....__
+00001d70: 6974 6572 5f5f ff00 0000 7293 0000 007a  iter__....r....z
+00001d80: 0e51 7565 7565 2e5f 5f69 7465 725f 5f72  .Queue.__iter__r
+00001d90: 0b00 0000 6301 0000 0000 0000 0000 0000  ....c...........
+00001da0: 0002 0000 0002 0000 0043 0000 0173 1800  .........C...s..
+00001db0: 0000 7c00 a000 a100 7d01 7c01 6400 7500  ..|.....}.|.d.u.
+00001dc0: 720a 7401 8201 7c01 5300 722e 0000 0029  r.t...|.S.r....)
+00001dd0: 02da 0764 6571 7565 7565 da0d 5374 6f70  ...dequeue..Stop
+00001de0: 4974 6572 6174 696f 6e29 0272 1e00 0000  Iteration).r....
+00001df0: 728f 0000 0072 1f00 0000 721f 0000 0072  r....r....r....r
+00001e00: 2000 0000 da08 5f5f 6e65 7874 5f5f 0201   .....__next__..
+00001e10: 0000 7308 0000 0008 0108 0104 0104 017a  ..s............z
+00001e20: 0e51 7565 7565 2e5f 5f6e 6578 745f 5f63  .Queue.__next__c
+00001e30: 0100 0000 0000 0000 0000 0000 0b00 0000  ................
+00001e40: 0e00 0000 4300 0001 7358 0300 007c 006a  ....C...sX...|.j
+00001e50: 0090 018f 9d01 0090 017a 8390 017a 627c  .........z...zb|
+00001e60: 006a 0172 167c 00a0 02a1 0072 167c 00a0  .j.r.|.....r.|..
+00001e70: 03a1 0001 0090 016e 537c 006a 04a0 05a1  .......nS|.j....
+00001e80: 0044 005d 0c5c 027d 017d 027c 02a0 06a1  .D.].\.}.}.|....
+00001e90: 0072 277c 02a0 03a1 0001 0071 1b74 077c  .r'|.......q.t.|
+00001ea0: 006a 04a0 08a1 0083 0144 0090 015d 017d  .j.......D...].}
+00001eb0: 017c 006a 047c 0119 007d 027c 02a0 09a1  .|.j.|...}.|....
+00001ec0: 0090 0173 317c 02a0 0aa1 0090 0173 317c  ...s1|.......s1|
+00001ed0: 02a0 0ba1 0001 007c 026a 0c73 767a 197c  .......|.j.svz.|
+00001ee0: 006a 0da0 0e7c 026a 0fa1 015c 047d 037d  .j...|.j...\.}.}
+00001ef0: 047d 057d 067c 037c 025f 107c 047c 025f  .}.}.|.|._.|.|._
+00001f00: 117c 057c 025f 127c 067c 025f 1357 006e  .|.|._.|.|._.W.n
+00001f10: 1404 0074 1479 7501 0001 0001 0074 1574  ...t.yu......t.t
+00001f20: 1664 01a0 177c 026a 0fa1 0183 0183 017c  .d...|.j.......|
+00001f30: 025f 1859 006e 0177 007c 006a 1964 0075  ._.Y.n.w.|.j.d.u
+00001f40: 0172 9b7a 087c 00a0 197c 02a1 017c 025f  .r.z.|...|...|._
+00001f50: 1a57 006e 1704 0074 1679 9a01 007d 0701  .W.n...t.y...}..
+00001f60: 007a 0b74 157c 0783 017c 025f 1a57 0059  .z.t.|...|._.W.Y
+00001f70: 0064 007d 077e 076e 0564 007d 077e 0777  .d.}.~.n.d.}.~.w
+00001f80: 0177 0074 1ba0 1ba1 007c 025f 1c74 1da0  .w.t.....|._.t..
+00001f90: 1e64 027c 026a 0fa1 0201 007c 006a 1f73  .d.|.j.....|.j.s
+00001fa0: b174 207c 006a 217c 0283 0201 006e 077c  .t |.j!|.....n.|
+00001fb0: 0004 006a 2264 0337 0002 005f 227c 006a  ...j"d.7..._"|.j
+00001fc0: 047c 013d 007c 026a 2364 0075 0190 0172  .|.=.|.j#d.u...r
+00001fd0: 317c 026a 237c 006a 246b 0390 0172 317c  1|.j#|.j$k...r1|
+00001fe0: 006a 25a0 267c 026a 23a1 017d 087c 0864  .j%.&|.j#..}.|.d
+00001ff0: 0075 0190 0172 3164 007d 097c 026a 127d  .u...r1d.}.|.j.}
+00002000: 0a74 277c 0883 0164 046b 0490 0172 1574  .t'|...d.k...r.t
+00002010: 287c 0883 017d 097c 0a64 046b 0273 ec7c  (|...}.|.d.k.s.|
+00002020: 096a 2973 ed6e 2864 057c 095f 0c7c 0a7c  .j)s.n(d.|._.|.|
+00002030: 095f 1264 06a0 177c 026a 0f7c 0aa1 027c  ._.d...|.j.|...|
+00002040: 095f 1174 1ba0 1ba1 007c 095f 1c7c 006a  ._.t.....|._.|.j
+00002050: 1f90 0173 0b74 207c 006a 217c 0983 0201  ...s.t |.j!|....
+00002060: 006e 077c 0004 006a 2264 0337 0002 005f  .n.|...j"d.7..._
+00002070: 2264 007d 0971 da74 277c 0883 0164 046b  "d.}.q.t'|...d.k
+00002080: 0290 0172 217c 006a 257c 026a 233d 007c  ...r!|.j%|.j#=.|
+00002090: 0964 0075 0190 0172 317c 097c 006a 047c  .d.u...r1|.|.j.|
+000020a0: 096a 0f3c 007c 00a0 2a7c 09a1 0101 0071  .j.<.|..*|.....q
+000020b0: 2f7c 006a 25a0 267c 006a 24a1 0190 0172  /|.j%.&|.j$....r
+000020c0: 697c 006a 2b7c 00a0 2ca1 0018 0064 046b  i|.j+|..,....d.k
+000020d0: 0490 0172 6974 287c 006a 257c 006a 2419  ...rit(|.j%|.j$.
+000020e0: 0083 017d 027c 027c 006a 047c 026a 0f3c  ...}.|.|.j.|.j.<
+000020f0: 007c 00a0 2a7c 02a1 0101 007c 006a 25a0  .|..*|.....|.j%.
+00002100: 267c 006a 24a1 0190 0172 697c 006a 2b7c  &|.j$....ri|.j+|
+00002110: 00a0 2ca1 0018 0064 046b 0490 0173 4457  ..,....d.k...sDW
+00002120: 006e 0f01 0001 0001 007c 00a0 03a1 0001  .n.......|......
+00002130: 0074 1da0 1174 2da0 2ea1 00a1 0101 0059  .t...t-........Y
+00002140: 0057 0074 1da0 1e64 077c 00a0 2fa1 007c  .W.t...d.|../..|
+00002150: 00a0 2ca1 007c 00a0 30a1 00a1 0401 006e  ..,..|..0......n
+00002160: 0f74 1da0 1e64 077c 00a0 2fa1 007c 00a0  .t...d.|../..|..
+00002170: 2ca1 007c 00a0 30a1 00a1 0401 0077 0057  ,..|..0......w.W
+00002180: 0064 0004 0004 0083 0301 0064 0053 0031  .d.........d.S.1
+00002190: 0090 0173 a577 0101 0001 0001 0059 0001  ...s.w.......Y..
+000021a0: 0064 0053 0029 084e 7a36 7b7d 0a0a 4e6f  .d.S.).Nz6{}..No
+000021b0: 2064 6174 6120 666f 7220 6461 7461 3b20   data for data; 
+000021c0: 6974 206d 6179 2068 6176 6520 6578 6974  it may have exit
+000021d0: 6564 2075 6e65 7870 6563 7465 646c 792e  ed unexpectedly.
+000021e0: 7a11 436f 6d70 6c65 7465 6420 6a6f 623a  z.Completed job:
+000021f0: 2025 6472 0a00 0000 7201 0000 0054 7a42   %dr....r....TzB
+00002200: 736b 6970 5f6f 6e5f 6772 6f75 705f 6572  skip_on_group_er
+00002210: 726f 7220 3d20 5472 7565 2061 6e64 2070  ror = True and p
+00002220: 7265 6365 6469 6e67 2064 6174 6120 287b  receding data ({
+00002230: 7d29 2065 7869 7420 636f 6465 2069 7320  }) exit code is 
+00002240: 7b7d 7a24 7761 6974 696e 673d 2564 3b20  {}z$waiting=%d; 
+00002250: 776f 726b 696e 673d 2564 3b20 6669 6e69  working=%d; fini
+00002260: 7368 6564 3d25 642e 2931 7257 0000 0072  shed=%d.)1rW...r
+00002270: 6c00 0000 da07 6973 5f69 646c 6572 2b00  l.....is_idler+.
+00002280: 0000 7262 0000 00da 0569 7465 6d73 da0a  ..rb.....items..
+00002290: 6973 5f65 7870 6972 6564 7284 0000 0072  is_expiredr....r
+000022a0: 8500 0000 722f 0000 00da 0c69 735f 7072  ....r/.....is_pr
+000022b0: 6f63 6573 7365 64da 046a 6f69 6e72 8900  ocessed..joinr..
+000022c0: 0000 7268 0000 00da 0370 6f70 da03 6964  ..rh.....pop..id
+000022d0: 78da 0672 6573 756c 74da 0565 7272 6f72  x..result..error
+000022e0: da08 6578 6974 636f 6465 da10 6669 6e69  ..exitcode..fini
+000022f0: 7368 5f74 696d 6573 7461 6d70 da08 4b65  sh_timestamp..Ke
+00002300: 7945 7272 6f72 724f 0000 00da 0945 7863  yErrorrO.....Exc
+00002310: 6570 7469 6f6e da06 666f 726d 6174 5a0d  eption..formatZ.
+00002320: 6578 6365 7074 696f 6e5f 7478 7472 5500  exception_txtrU.
+00002330: 0000 da0f 6361 6c6c 6261 636b 5f72 6573  ....callback_res
+00002340: 756c 7472 8a00 0000 728b 0000 0072 5e00  ultr....r....r^.
+00002350: 0000 7269 0000 0072 6400 0000 7204 0000  ..ri...rd...r...
+00002360: 0072 6300 0000 7253 0000 00da 0567 726f  .rc...rS.....gro
+00002370: 7570 723a 0000 0072 6100 0000 7286 0000  upr:...ra...r...
+00002380: 0072 8800 0000 7203 0000 00da 1373 6b69  .r....r......ski
+00002390: 705f 6f6e 5f67 726f 7570 5f65 7272 6f72  p_on_group_error
+000023a0: da0a 5f73 7461 7274 5f6a 6f62 7245 0000  .._start_jobrE..
+000023b0: 00da 0e5f 636f 756e 745f 776f 726b 696e  ..._count_workin
+000023c0: 67da 0974 7261 6365 6261 636b da0a 666f  g..traceback..fo
+000023d0: 726d 6174 5f65 7863 da0e 5f63 6f75 6e74  rmat_exc.._count
+000023e0: 5f77 6169 7469 6e67 da0f 5f63 6f75 6e74  _waiting.._count
+000023f0: 5f66 696e 6973 6865 6429 0b72 1e00 0000  _finished).r....
+00002400: 5a06 6a6f 625f 6964 728f 0000 00da 0673  Z.job_idr......s
+00002410: 7464 6f75 74da 0673 7464 6572 7272 a200  tdout..stderrr..
+00002420: 0000 da09 7469 6d65 7374 616d 70da 0265  ....timestamp..e
+00002430: 7872 8d00 0000 5a08 6e65 7874 5f6a 6f62  xr....Z.next_job
+00002440: 5a0f 7061 7265 6e74 5f65 7869 7463 6f64  Z.parent_exitcod
+00002450: 6572 1f00 0000 721f 0000 0072 2000 0000  er....r....r ...
+00002460: 726b 0000 0008 0100 0073 dc00 0000 0a03  rk.......s......
+00002470: 0801 0e01 0c01 1203 0801 0801 0280 1402  ................
+00002480: 0a01 1402 0801 0601 0201 0c06 02fb 0201  ................
+00002490: 0201 0201 0201 0602 0601 0601 0a01 0c01  ................
+000024a0: 0201 0201 0201 0801 02fe 0aff 02ff 0a08  ................
+000024b0: 0201 1001 0201 0201 0aff 1603 0880 02fd  ................
+000024c0: 0a05 0e02 0602 0e01 0e02 0802 0c03 0e01  ................
+000024d0: 0602 0401 04ff 0a03 0401 0601 0e01 0801  ................
+000024e0: 0803 0401 02ff 0203 0602 0601 0202 0201  ................
+000024f0: 0401 0201 02fe 04fe 0a07 0801 0201 0401  ................
+00002500: 0201 06fe 0e05 0401 0201 0e02 0a01 0a02  ................
+00002510: 0c01 0a01 0280 0c03 04ff 1402 1002 0c01  ................
+00002520: 0a01 0cfb 04ff 1402 0480 0605 0801 1001  ................
+00002530: 0280 0402 0201 0601 0601 0601 0afc 0201  ................
+00002540: 0601 0601 0601 08fc 2491 7a0c 5175 6575  ........$.z.Queu
+00002550: 652e 5f70 756c 7365 6301 0000 0000 0000  e._pulsec.......
+00002560: 0000 0000 0001 0000 0004 0000 0043 0000  .............C..
+00002570: 0173 1800 0000 7400 6401 6402 8400 7c00  .s....t.d.d...|.
+00002580: 6a01 a002 a100 4400 8301 8301 5300 2903  j.....D.....S.).
+00002590: 7a42 0a20 2020 2020 2020 2052 6574 7572  zB.        Retur
+000025a0: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+000025b0: 5468 6520 6e75 6d62 6572 206f 6620 7065  The number of pe
+000025c0: 6e64 696e 6720 6a6f 6273 2e0a 2020 2020  nding jobs..    
+000025d0: 2020 2020 6301 0000 0000 0000 0000 0000      c...........
+000025e0: 0003 0000 0003 0000 0073 0000 0173 1c00  .........s...s..
+000025f0: 0000 8100 7c00 5d09 5c02 7d01 7d02 7400  ....|.].\.}.}.t.
+00002600: 7c02 8301 5600 0100 7102 6400 5300 722e  |...V...q.d.S.r.
+00002610: 0000 0029 0172 8800 0000 2903 da02 2e30  ...).r....)....0
+00002620: 728e 0000 00da 0176 721f 0000 0072 1f00  r......vr....r..
+00002630: 0000 7220 0000 00da 093c 6765 6e65 7870  ..r .....<genexp
+00002640: 723e 8601 0000 7304 0000 0002 801a 007a  r>....s........z
+00002650: 2751 7565 7565 2e5f 636f 756e 745f 7761  'Queue._count_wa
+00002660: 6974 696e 672e 3c6c 6f63 616c 733e 2e3c  iting.<locals>.<
+00002670: 6765 6e65 7870 723e 2903 da03 7375 6d72  genexpr>)...sumr
+00002680: 6100 0000 729a 0000 0072 2500 0000 721f  a...r....r%...r.
+00002690: 0000 0072 1f00 0000 7220 0000 0072 ae00  ...r....r ...r..
+000026a0: 0000 8101 0000 7302 0000 0018 057a 1451  ......s......z.Q
+000026b0: 7565 7565 2e5f 636f 756e 745f 7761 6974  ueue._count_wait
+000026c0: 696e 6763 0100 0000 0000 0000 0000 0000  ingc............
+000026d0: 0100 0000 0200 0000 4300 0001 f30a 0000  ........C.......
+000026e0: 0074 007c 006a 0183 0153 0029 017a 420a  .t.|.j...S.).zB.
+000026f0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00002700: 0a20 2020 2020 2020 2020 2020 2054 6865  .            The
+00002710: 206e 756d 6265 7220 6f66 2072 756e 6e69   number of runni
+00002720: 6e67 206a 6f62 732e 0a20 2020 2020 2020  ng jobs..       
+00002730: 2029 0272 8800 0000 7262 0000 0072 2500   ).r....rb...r%.
+00002740: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
+00002750: 0072 ab00 0000 8801 0000 f302 0000 000a  .r..............
+00002760: 057a 1451 7565 7565 2e5f 636f 756e 745f  .z.Queue._count_
+00002770: 776f 726b 696e 6763 0100 0000 0000 0000  workingc........
+00002780: 0000 0000 0100 0000 0200 0000 4300 0001  ............C...
+00002790: 72b8 0000 0029 017a 440a 2020 2020 2020  r....).zD.      
+000027a0: 2020 5265 7475 726e 733a 0a20 2020 2020    Returns:.     
+000027b0: 2020 2020 2020 2054 6865 206e 756d 6265         The numbe
+000027c0: 7220 6f66 2063 6f6d 706c 6574 6564 206a  r of completed j
+000027d0: 6f62 732e 0a20 2020 2020 2020 2029 0272  obs..        ).r
+000027e0: 8800 0000 7263 0000 0072 2500 0000 721f  ....rc...r%...r.
+000027f0: 0000 0072 1f00 0000 7220 0000 0072 af00  ...r....r ...r..
+00002800: 0000 8f01 0000 72b9 0000 007a 1551 7565  ......r....z.Que
+00002810: 7565 2e5f 636f 756e 745f 6669 6e69 7368  ue._count_finish
+00002820: 6564 6301 0000 0000 0000 0000 0000 0001  edc.............
+00002830: 0000 0004 0000 0043 0000 0173 0e00 0000  .......C...s....
+00002840: 7c00 6a00 6401 6401 6402 8d02 5300 2903  |.j.d.d.d...S.).
+00002850: 7a5f 0a20 2020 2020 2020 2052 6574 7572  z_.        Retur
+00002860: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00002870: 5468 6520 6e75 6d62 6572 206f 6620 756e  The number of un
+00002880: 6669 6e69 7368 6564 206a 6f62 7320 2869  finished jobs (i
+00002890: 2e65 2e2c 2077 6169 7469 6e67 202b 2077  .e., waiting + w
+000028a0: 6f72 6b69 6e67 292e 0a20 2020 2020 2020  orking)..       
+000028b0: 2054 2902 da07 7761 6974 696e 67da 0777   T)...waiting..w
+000028c0: 6f72 6b69 6e67 a901 da04 7369 7a65 7225  orking....sizer%
+000028d0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+000028e0: 0000 da10 5f63 6f75 6e74 5f72 656d 6169  ...._count_remai
+000028f0: 6e69 6e67 9601 0000 7302 0000 000e 057a  ning....s......z
+00002900: 1651 7565 7565 2e5f 636f 756e 745f 7265  .Queue._count_re
+00002910: 6d61 696e 696e 67a9 0372 ba00 0000 72bb  maining..r....r.
+00002920: 0000 00da 0866 696e 6973 6865 6472 ba00  .....finishedr..
+00002930: 0000 72bb 0000 0072 c000 0000 fa09 6c69  ..r....r......li
+00002940: 7374 5b69 6e74 5d63 0100 0000 0000 0000  st[int]c........
+00002950: 0300 0000 0700 0000 0800 0000 4300 0001  ............C...
+00002960: 739c 0000 0069 007d 0464 017d 057a 3a74  s....i.}.d.}.z:t
+00002970: 007c 017c 027c 0367 0383 017d 067c 0664  .|.|.|.g...}.|.d
+00002980: 026b 0372 1e7c 0664 036b 0272 1964 045c  .k.r.|.d.k.r.d.\
+00002990: 037d 017d 027d 037c 006a 01a0 02a1 007d  .}.}.}.|.j.....}
+000029a0: 057c 0172 267c 00a0 03a1 007c 0464 053c  .|.r&|.....|.d.<
+000029b0: 007c 0272 2e7c 00a0 04a1 007c 0464 063c  .|.r.|.....|.d.<
+000029c0: 007c 0372 367c 00a0 05a1 007c 0464 073c  .|.r6|.....|.d.<
+000029d0: 0057 007c 0572 3e7c 006a 01a0 06a1 0001  .W.|.r>|.j......
+000029e0: 006e 097c 0572 477c 006a 01a0 06a1 0001  .n.|.rG|.j......
+000029f0: 0077 0077 0074 077c 04a0 08a1 0083 0153  .w.w.t.|.......S
+00002a00: 0029 0861 2402 0000 5265 7475 726e 7320  .).a$...Returns 
+00002a10: 7468 6520 6e75 6d62 6572 206f 6620 6a6f  the number of jo
+00002a20: 6273 2069 6e20 7468 6520 636f 7272 6573  bs in the corres
+00002a30: 706f 6e64 696e 6720 7175 6575 6528 7329  ponding queue(s)
+00002a40: 2e0a 0a20 2020 2020 2020 2041 7267 733a  ...        Args:
+00002a50: 0a20 2020 2020 2020 2020 2020 2077 6169  .            wai
+00002a60: 7469 6e67 3a20 696e 636c 7564 6520 6a6f  ting: include jo
+00002a70: 6273 2069 6e20 7468 6520 7761 6974 696e  bs in the waitin
+00002a80: 6720 7175 6575 653f 0a20 2020 2020 2020  g queue?.       
+00002a90: 2020 2020 2020 2020 202d 2041 6363 6570           - Accep
+00002aa0: 7473 3a20 626f 6f6c 0a20 2020 2020 2020  ts: bool.       
+00002ab0: 2020 2020 2020 2020 202d 2044 6566 6175           - Defau
+00002ac0: 6c74 3a20 4661 6c73 650a 2020 2020 2020  lt: False.      
+00002ad0: 2020 2020 2020 776f 726b 696e 673a 2069        working: i
+00002ae0: 6e63 6c75 6465 206a 6f62 7320 696e 2074  nclude jobs in t
+00002af0: 6865 2077 6f72 6b69 6e67 2074 6162 6c65  he working table
+00002b00: 3f0a 2020 2020 2020 2020 2020 2020 2020  ?.              
+00002b10: 2020 2d20 4163 6365 7074 733a 2062 6f6f    - Accepts: boo
+00002b20: 6c0a 2020 2020 2020 2020 2020 2020 2020  l.              
+00002b30: 2020 2d20 4465 6661 756c 743a 2046 616c    - Default: Fal
+00002b40: 7365 0a20 2020 2020 2020 2020 2020 2066  se.            f
+00002b50: 696e 6973 6865 643a 2069 6e63 6c75 6465  inished: include
+00002b60: 206a 6f62 7320 696e 2074 6865 2063 6f6d   jobs in the com
+00002b70: 706c 6574 6564 2071 7565 7565 3f0a 2020  pleted queue?.  
+00002b80: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00002b90: 4163 6365 7074 733a 2062 6f6f 6c0a 2020  Accepts: bool.  
+00002ba0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00002bb0: 4465 6661 756c 743a 2046 616c 7365 0a0a  Default: False..
+00002bc0: 2020 2020 2020 2020 4e6f 7465 3a20 7768          Note: wh
+00002bd0: 656e 2061 6c6c 2061 7265 2046 616c 7365  en all are False
+00002be0: 2c20 616c 6c20 6a6f 6273 2061 7265 2063  , all jobs are c
+00002bf0: 6f75 6e74 6564 2028 6465 6661 756c 7429  ounted (default)
+00002c00: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00002c10: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00002c20: 696e 740a 2020 2020 2020 2020 4672 0a00  int.        Fr..
+00002c30: 0000 7201 0000 0029 0354 5454 72ba 0000  ..r....).TTTr...
+00002c40: 0072 bb00 0000 72c0 0000 0029 0972 b700  .r....r....).r..
+00002c50: 0000 7257 0000 00da 0761 6371 7569 7265  ..rW.....acquire
+00002c60: 72ae 0000 0072 ab00 0000 72af 0000 00da  r....r....r.....
+00002c70: 0772 656c 6561 7365 7284 0000 00da 0676  .releaser......v
+00002c80: 616c 7565 7329 0772 1e00 0000 72ba 0000  alues).r....r...
+00002c90: 0072 bb00 0000 72c0 0000 00da 0663 6f75  .r....r......cou
+00002ca0: 6e74 735a 0969 735f 6c6f 636b 6564 5a08  ntsZ.is_lockedZ.
+00002cb0: 746f 5f74 616c 6c79 721f 0000 0072 1f00  to_tallyr....r..
+00002cc0: 0000 7220 0000 00da 065f 7369 7a65 739d  ..r ....._sizes.
+00002cd0: 0100 0073 2c00 0000 041a 0402 0202 0e01  ...s,...........
+00002ce0: 0801 0801 0a01 0a02 0402 0c01 0401 0c01  ................
+00002cf0: 0401 0c01 0280 0402 0a01 0280 04ff 0c01  ................
+00002d00: 02ff 0c03 7a0c 5175 6575 652e 5f73 697a  ....z.Queue._siz
+00002d10: 6573 6301 0000 0000 0000 0000 0000 0001  esc.............
+00002d20: 0000 0002 0000 0043 0000 0173 0800 0000  .......C...s....
+00002d30: 7c00 a000 a100 5300 722e 0000 0072 bc00  |.....S.r....r..
+00002d40: 0000 7225 0000 0072 1f00 0000 721f 0000  ..r%...r....r...
+00002d50: 0072 2000 0000 da07 5f5f 6c65 6e5f 5fcf  .r .....__len__.
+00002d60: 0100 0073 0200 0000 0801 7a0d 5175 6575  ...s......z.Queu
+00002d70: 652e 5f5f 6c65 6e5f 5f63 0100 0000 0000  e.__len__c......
+00002d80: 0000 0300 0000 0400 0000 0600 0000 4300  ..............C.
+00002d90: 0001 7314 0000 0074 007c 006a 017c 017c  ..s....t.|.j.|.|
+00002da0: 027c 0364 018d 0383 0153 0029 0261 1803  .|.d.....S.).a..
+00002db0: 0000 4765 7420 7468 6520 6e75 6d62 6572  ..Get the number
+00002dc0: 206f 6620 6a6f 6273 2069 6e20 7468 6520   of jobs in the 
+00002dd0: 7175 6575 6520 696e 2073 7461 7465 3a20  queue in state: 
+00002de0: 7761 6974 696e 672c 2077 6f72 6b69 6e67  waiting, working
+00002df0: 2c20 616e 642f 6f72 2066 696e 6973 6865  , and/or finishe
+00002e00: 642e 0a0a 2020 2020 2020 2020 4966 206e  d...        If n
+00002e10: 6f20 6f70 7469 6f6e 7320 6172 6520 6769  o options are gi
+00002e20: 7665 6e2c 2074 6865 2074 6f74 616c 206e  ven, the total n
+00002e30: 756d 6265 7220 6f66 206a 6f62 7320 696e  umber of jobs in
+00002e40: 2074 6865 2071 7565 7565 2069 7320 7265   the queue is re
+00002e50: 7475 726e 6564 2e0a 0a20 2020 2020 2020  turned...       
+00002e60: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00002e70: 2020 2077 6169 7469 6e67 3a20 696e 636c     waiting: incl
+00002e80: 7564 6520 7761 6974 696e 6720 6a6f 6273  ude waiting jobs
+00002e90: 2e0a 2020 2020 2020 2020 2020 2020 776f  ..            wo
+00002ea0: 726b 696e 673a 2069 6e63 6c75 6465 2077  rking: include w
+00002eb0: 6f72 6b69 6e67 206a 6f62 732e 0a20 2020  orking jobs..   
+00002ec0: 2020 2020 2020 2020 2066 696e 6973 6865           finishe
+00002ed0: 643a 2069 6e63 6c75 6465 2066 696e 6973  d: include finis
+00002ee0: 6865 6420 6a6f 6273 2e0a 0a20 2020 2020  hed jobs...     
+00002ef0: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00002f00: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+00002f10: 2020 2020 2045 7861 6d70 6c65 733a 0a20       Examples:. 
+00002f20: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
+00002f30: 726f 6d20 7070 7175 6575 6520 696d 706f  rom ppqueue impo
+00002f40: 7274 2051 7565 7565 0a20 2020 2020 2020  rt Queue.       
+00002f50: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00002f60: 2020 2020 203e 3e3e 2064 6566 2061 6464       >>> def add
+00002f70: 5f6e 756d 7328 783a 2069 6e74 2c20 793a  _nums(x: int, y:
+00002f80: 2069 6e74 2920 2d3e 2069 6e74 3a0a 2020   int) -> int:.  
+00002f90: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00002fa0: 2020 7265 7475 726e 2078 202b 2079 0a20    return x + y. 
+00002fb0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+00002fc0: 2020 2020 2020 2020 2020 203e 3e3e 2077             >>> w
+00002fd0: 6974 6820 5175 6575 6528 2920 6173 2071  ith Queue() as q
+00002fe0: 7565 7565 3a0a 2020 2020 2020 2020 2020  ueue:.          
+00002ff0: 2020 2e2e 2e20 2020 2020 666f 7220 6920    ...     for i 
+00003000: 696e 2072 616e 6765 2835 293a 0a20 2020  in range(5):.   
+00003010: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
+00003020: 2020 2020 205f 203d 2071 7565 7565 2e65       _ = queue.e
+00003030: 6e71 7565 7565 2861 6464 5f6e 756d 732c  nqueue(add_nums,
+00003040: 2061 7267 733d 5b69 2c20 3130 305d 290a   args=[i, 100]).
+00003050: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00003060: 2020 2020 2020 2020 7072 696e 7428 7175          print(qu
+00003070: 6575 652e 7369 7a65 2829 290a 2020 2020  eue.size()).    
+00003080: 2020 2020 2020 2020 310a 2020 2020 2020          1.      
+00003090: 2020 2020 2020 320a 2020 2020 2020 2020        2.        
+000030a0: 2020 2020 330a 2020 2020 2020 2020 2020      3.          
+000030b0: 2020 340a 2020 2020 2020 2020 2020 2020    4.            
+000030c0: 350a 2020 2020 2020 2020 72bf 0000 0029  5.        r....)
+000030d0: 0272 b700 0000 72c6 0000 0029 0472 1e00  .r....r....).r..
+000030e0: 0000 72ba 0000 0072 bb00 0000 72c0 0000  ..r....r....r...
+000030f0: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00003100: 72bd 0000 00d2 0100 0073 0200 0000 1423  r........s.....#
+00003110: 7a0a 5175 6575 652e 7369 7a65 6301 0000  z.Queue.sizec...
+00003120: 0000 0000 0000 0000 0001 0000 0002 0000  ................
+00003130: 0043 0000 0173 1800 0000 7c00 a000 a100  .C...s....|.....
+00003140: 6401 6b02 6f0b 7c00 a001 a100 6401 6b02  d.k.o.|.....d.k.
+00003150: 5300 2902 4e72 0100 0000 2902 72ae 0000  S.).Nr....).r...
+00003160: 0072 ab00 0000 7225 0000 0072 1f00 0000  .r....r%...r....
+00003170: 721f 0000 0072 2000 0000 7299 0000 00f7  r....r ...r.....
+00003180: 0100 0073 0200 0000 1801 7a0d 5175 6575  ...s......z.Queu
+00003190: 652e 6973 5f69 646c 6563 0100 0000 0000  e.is_idlec......
+000031a0: 0000 0000 0000 0100 0000 0300 0000 4300  ..............C.
+000031b0: 0001 731a 0000 007c 00a0 00a1 0064 016b  ..s....|.....d.k
+000031c0: 0470 0c7c 006a 017c 00a0 02a1 006b 0153  .p.|.j.|.....k.S
+000031d0: 0029 027a 7054 7275 6520 6966 206d 6178  .).zpTrue if max
+000031e0: 2063 6f6e 6375 7272 656e 7420 6c69 6d69   concurrent limi
+000031f0: 7420 6973 2072 6561 6368 6564 206f 7220  t is reached or 
+00003200: 6966 2074 6865 7265 2061 7265 2077 6169  if there are wai
+00003210: 7469 6e67 206a 6f62 732e 0a0a 2020 2020  ting jobs...    
+00003220: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00003230: 2020 2020 2020 2020 202e 2e2e 0a20 2020           ....   
+00003240: 2020 2020 2072 0100 0000 2903 72ae 0000       r....).r...
+00003250: 0072 4500 0000 72ab 0000 0072 2500 0000  .rE...r....r%...
+00003260: 721f 0000 0072 1f00 0000 7220 0000 00da  r....r....r ....
+00003270: 0769 735f 6275 7379 fa01 0000 7302 0000  .is_busy....s...
+00003280: 001a 067a 0d51 7565 7565 2e69 735f 6275  ...z.Queue.is_bu
+00003290: 7379 6301 0000 0000 0000 0000 0000 0001  syc.............
+000032a0: 0000 0002 0000 0043 0000 0173 0c00 0000  .......C...s....
+000032b0: 7c00 a000 a100 6401 6b02 5300 2902 7a59  |.....d.k.S.).zY
+000032c0: 5472 7565 2069 6620 7468 6572 6520 6172  True if there ar
+000032d0: 6520 6e6f 206a 6f62 7320 696e 2074 6865  e no jobs in the
+000032e0: 2071 7565 7565 2073 7973 7465 6d2e 0a0a   queue system...
+000032f0: 2020 2020 2020 2020 5265 7475 726e 733a          Returns:
+00003300: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00003310: 0a20 2020 2020 2020 2072 0100 0000 72bc  .        r....r.
+00003320: 0000 0072 2500 0000 721f 0000 0072 1f00  ...r%...r....r..
+00003330: 0000 7220 0000 00da 0869 735f 656d 7074  ..r .....is_empt
+00003340: 7902 0200 0073 0200 0000 0c06 7a0e 5175  y....s......z.Qu
+00003350: 6575 652e 6973 5f65 6d70 7479 6301 0000  eue.is_emptyc...
+00003360: 0000 0000 0000 0000 0001 0000 0003 0000  ................
+00003370: 0043 0000 0173 1e00 0000 6401 7c00 6a00  .C...s....d.|.j.
+00003380: 0400 0300 6b00 6f0c 7c00 a001 a100 6b01  ....k.o.|.....k.
+00003390: 5300 0200 0100 5300 2902 7a6f 5472 7565  S.....S.).zoTrue
+000033a0: 2069 6620 7468 6520 6e75 6d62 6572 206f   if the number o
+000033b0: 6620 6a6f 6273 2069 6e20 7468 6520 7175  f jobs in the qu
+000033c0: 6575 6520 7379 7374 656d 2069 7320 6571  eue system is eq
+000033d0: 7561 6c20 746f 206d 6178 5f73 697a 652e  ual to max_size.
+000033e0: 0a0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000033f0: 733a 0a20 2020 2020 2020 2020 2020 202e  s:.            .
+00003400: 2e2e 0a20 2020 2020 2020 2072 0100 0000  ...        r....
+00003410: 2902 7251 0000 0072 bd00 0000 7225 0000  ).rQ...r....r%..
+00003420: 0072 1f00 0000 721f 0000 0072 2000 0000  .r....r....r ...
+00003430: da07 6973 5f66 756c 6c0a 0200 0073 0200  ..is_full....s..
+00003440: 0000 1e06 7a0d 5175 6575 652e 6973 5f66  ....z.Queue.is_f
+00003450: 756c 6c63 0100 0000 0000 0000 0000 0000  ullc............
+00003460: 0300 0000 0400 0000 4f00 0001 f310 0000  ........O.......
+00003470: 007c 006a 007c 0169 007c 02a4 018e 0153  .|.j.|.i.|.....S
+00003480: 0072 2e00 0000 7280 0000 00a9 0372 1e00  .r....r......r..
+00003490: 0000 7210 0000 0072 1500 0000 721f 0000  ..r....r....r...
+000034a0: 0072 1f00 0000 7220 0000 0072 9d00 0000  .r....r ...r....
+000034b0: 1202 0000 7302 0000 0010 017a 0a51 7565  ....s......z.Que
+000034c0: 7565 2e6a 6f69 6e29 04da 016e da07 7469  ue.join)...n..ti
+000034d0: 6d65 6f75 74da 0770 6f6c 6c5f 6d73 7240  meout..poll_msr@
+000034e0: 0000 0072 cd00 0000 72ce 0000 00da 0566  ...r....r......f
+000034f0: 6c6f 6174 72cf 0000 00fa 0b62 6f6f 6c20  loatr......bool 
+00003500: 7c20 4e6f 6e65 6301 0000 0000 0000 0004  | Nonec.........
+00003510: 0000 000e 0000 0008 0000 0043 0000 0173  ...........C...s
+00003520: 4a01 0000 7c03 6401 7500 7308 7c03 6402  J...|.d.u.s.|.d.
+00003530: 6b01 720c 7c00 6a00 7d03 6e0b 7c03 7c00  k.r.|.j.}.n.|.|.
+00003540: 6a00 6b00 7217 6403 7d05 7401 7c05 8301  j.k.r.d.}.t.|...
+00003550: 8201 7c04 6401 7500 721e 7c00 6a02 7d04  ..|.d.u.r.|.j.}.
+00003560: 6401 7d06 6401 7d07 6401 7d08 7c01 6402  d.}.d.}.d.}.|.d.
+00003570: 6b01 7231 7c00 6a03 7d06 6402 7d07 7404  k.r1|.j.}.d.}.t.
+00003580: 6a05 7d08 6e08 7c00 6a06 7d06 7c01 7d07  j.}.n.|.j.}.|.}.
+00003590: 7404 6a07 7d08 7c06 8300 7d09 7c08 7c09  t.j.}.|...}.|.|.
+000035a0: 7c07 8302 73a3 7408 a008 a100 7d0a 6401  |...s.t.....}.d.
+000035b0: 7d0b 7a53 7c04 7250 7409 7c09 6404 6405  }.zS|.rPt.|.d.d.
+000035c0: 8d02 7d0b 7c08 7c09 7c07 8302 7392 7c02  ..}.|.|.|...s.|.
+000035d0: 6402 6b02 7361 7408 a008 a100 7c0a 1800  d.k.sat.....|...
+000035e0: 7c02 6b00 7292 7408 a00a 7c03 6406 1b00  |.k.r.t...|.d...
+000035f0: a101 0100 7c06 8300 7d0c 7c0b 6401 7500  ....|...}.|.d.u.
+00003600: 7272 7c0c 7d09 6e0f 7c09 7c0c 1800 7d0d  rr|.}.n.|.|...}.
+00003610: 7c0d 6402 6b04 7281 7c0c 7d09 7c0b a00b  |.d.k.r.|.}.|...
+00003620: 7c0d a101 0100 7c08 7c09 7c07 8302 7392  |.....|.|.|...s.
+00003630: 7c02 6402 6b02 7361 7408 a008 a100 7c0a  |.d.k.sat.....|.
+00003640: 1800 7c02 6b00 7361 5700 7c0b 7299 7c0b  ..|.k.saW.|.r.|.
+00003650: a00c a100 0100 7c09 5300 7c0b 72a2 7c0b  ......|.S.|.r.|.
+00003660: a00c a100 0100 7700 7700 7c09 5300 2907  ......w.w.|.S.).
+00003670: 61da 0100 0057 6169 7420 666f 7220 6a6f  a....Wait for jo
+00003680: 6273 2074 6f20 6669 6e69 7368 2e0a 0a20  bs to finish... 
+00003690: 2020 2020 2020 2041 7267 733a 0a20 2020         Args:.   
+000036a0: 2020 2020 2020 2020 206e 3a20 7468 6520           n: the 
+000036b0: 6e75 6d62 6572 206f 6620 6a6f 6273 2074  number of jobs t
+000036c0: 6f20 7761 6974 2066 6f72 2028 6465 6661  o wait for (defa
+000036d0: 756c 743d 302c 2061 6c6c 292e 0a20 2020  ult=0, all)..   
+000036e0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+000036f0: 3a20 7365 636f 6e64 7320 746f 2077 6169  : seconds to wai
+00003700: 7420 6265 666f 7265 2072 6169 7369 6e67  t before raising
+00003710: 2060 5469 6d65 6f75 7445 7272 6f72 6020   `TimeoutError` 
+00003720: 2864 6566 6175 6c74 3d30 2c20 696e 6465  (default=0, inde
+00003730: 6669 6e69 7465 6c79 292e 0a20 2020 2020  finitely)..     
+00003740: 2020 2020 2020 2070 6f6c 6c5f 6d73 3a20         poll_ms: 
+00003750: 6d69 6c6c 6973 6563 6f6e 6473 2074 6f20  milliseconds to 
+00003760: 7061 7573 6520 6265 7477 6565 6e20 6368  pause between ch
+00003770: 6563 6b73 2028 6465 6661 756c 743d 3130  ecks (default=10
+00003780: 3029 2e0a 2020 2020 2020 2020 2020 2020  0)..            
+00003790: 7368 6f77 5f70 726f 6772 6573 733a 2069  show_progress: i
+000037a0: 6620 5472 7565 2c20 7072 6573 656e 7420  f True, present 
+000037b0: 6120 7072 6f67 7265 7373 2062 6172 2e0a  a progress bar..
+000037c0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+000037d0: 3a0a 2020 2020 2020 2020 2020 2020 4966  :.            If
+000037e0: 2060 6e20 3c3d 2030 602c 2072 6574 7572   `n <= 0`, retur
+000037f0: 6e73 2074 6865 2063 6f75 6e74 206f 6620  ns the count of 
+00003800: 756e 6669 6e69 7368 6564 206a 6f62 732e  unfinished jobs.
+00003810: 0a20 2020 2020 2020 2020 2020 2045 6c73  .            Els
+00003820: 652c 2072 6574 7572 6e73 2074 6865 2063  e, returns the c
+00003830: 6f75 6e74 206f 6620 6669 6e69 7368 6564  ount of finished
+00003840: 206a 6f62 732e 0a20 2020 2020 2020 204e   jobs..        N
+00003850: 7201 0000 007a 3260 706f 6c6c 5f6d 7360  r....z2`poll_ms`
+00003860: 206d 7573 7420 6265 203e 3d20 6070 7071   must be >= `ppq
+00003870: 7565 7565 2e51 7565 7565 2e70 756c 7365  ueue.Queue.pulse
+00003880: 5f66 7265 715f 6d73 60da 026f 7029 02da  _freq_ms`..op)..
+00003890: 0574 6f74 616c 5a04 756e 6974 7227 0000  .totalZ.unitr'..
+000038a0: 0029 0d72 6a00 0000 725d 0000 0072 4000  .).rj...r]...r@.
+000038b0: 0000 72be 0000 0072 1200 0000 da06 5f5f  ..r....r......__
+000038c0: 6c65 5f5f 72af 0000 00da 065f 5f67 655f  le__r......__ge_
+000038d0: 5f72 8a00 0000 7209 0000 00da 0573 6c65  _r....r......sle
+000038e0: 6570 da06 7570 6461 7465 da05 636c 6f73  ep..update..clos
+000038f0: 6529 0e72 1e00 0000 72cd 0000 0072 ce00  e).r....r....r..
+00003900: 0000 72cf 0000 0072 4000 0000 726d 0000  ..r....r@...rm..
+00003910: 005a 045f 6675 6e5a 0d5f 7461 7267 6574  .Z._funZ._target
+00003920: 5f76 616c 7565 5a0b 5f63 6f6d 7061 7261  _valueZ._compara
+00003930: 746f 725a 0d63 7572 7265 6e74 5f76 616c  torZ.current_val
+00003940: 7565 7224 0000 00da 0270 62da 0974 6d70  uer$.....pb..tmp
+00003950: 5f76 616c 7565 5a0a 6469 6666 5f76 616c  _valueZ.diff_val
+00003960: 7565 721f 0000 0072 1f00 0000 7220 0000  uer....r....r ..
+00003970: 0072 7200 0000 1502 0000 7358 0000 0010  .rr.......sX....
+00003980: 1408 010a 0104 0108 0108 0206 0104 0204  ................
+00003990: 0104 0108 0206 0104 0108 0106 0204 0106  ................
+000039a0: 0106 020a 0208 0104 0202 0204 010c 010a  ................
+000039b0: 0218 010e 0206 0208 0106 0108 0208 0104  ................
+000039c0: 010a 010a f418 0102 8004 0d08 0104 0204  ................
+000039d0: fd0a 0102 ff04 037a 0a51 7565 7565 2e77  .......z.Queue.w
+000039e0: 6169 74da 045f 6a6f 6272 6800 0000 fa34  ait.._jobrh....4
+000039f0: 6469 6374 5b69 6e74 2c20 7475 706c 655b  dict[int, tuple[
+00003a00: 7374 7220 7c20 4e6f 6e65 2c20 7374 7220  str | None, str 
+00003a10: 7c20 4e6f 6e65 2c20 696e 742c 2066 6c6f  | None, int, flo
+00003a20: 6174 5d5d fa29 7475 706c 655b 7374 7220  at]].)tuple[str 
+00003a30: 7c20 4e6f 6e65 2c20 7374 7220 7c20 4e6f  | None, str | No
+00003a40: 6e65 2c20 696e 742c 2066 6c6f 6174 5d63  ne, int, float]c
+00003a50: 0200 0000 0200 0000 0000 0000 0900 0000  ................
+00003a60: 0a00 0000 4f00 0001 73ba 0000 0064 007d  ....O...s....d.}
+00003a70: 0464 007d 057a 4a7a 0c7c 006a 007c 0269  .d.}.zJz.|.j.|.i
+00003a80: 007c 03a4 018e 017d 0464 017d 0657 006e  .|.....}.d.}.W.n
+00003a90: 1d04 0074 0179 2e01 007d 0701 007a 1174  ...t.y...}...z.t
+00003aa0: 02a0 03a1 007d 0564 027d 067c 006a 0473  .....}.d.}.|.j.s
+00003ab0: 247c 0782 0157 0059 0064 007d 077e 076e  $|...W.Y.d.}.~.n
+00003ac0: 1564 007d 077e 0777 0177 0057 0074 05a0  .d.}.~.w.w.W.t..
+00003ad0: 05a1 007d 087c 047c 057c 067c 0866 047c  ...}.|.|.|.|.f.|
+00003ae0: 017c 006a 063c 0064 0053 0057 0074 05a0  .|.j.<.d.S.W.t..
+00003af0: 05a1 007d 087c 047c 057c 067c 0866 047c  ...}.|.|.|.|.f.|
+00003b00: 017c 006a 063c 0064 0053 0074 05a0 05a1  .|.j.<.d.S.t....
+00003b10: 007d 087c 047c 057c 067c 0866 047c 017c  .}.|.|.|.|.f.|.|
+00003b20: 006a 063c 0077 0029 034e 7201 0000 00e9  .j.<.w.).Nr.....
+00003b30: ffff ffff 2907 7213 0000 0072 a500 0000  ....).r....r....
+00003b40: 72ac 0000 0072 ad00 0000 da0f 7375 7070  r....r......supp
+00003b50: 7265 7373 5f65 7272 6f72 7372 8a00 0000  ress_errorsr....
+00003b60: 729f 0000 0029 0972 db00 0000 7268 0000  r....).r....rh..
+00003b70: 0072 1000 0000 7215 0000 0072 b000 0000  .r....r....r....
+00003b80: 72b1 0000 0072 a200 0000 72b3 0000 0072  r....r....r....r
+00003b90: b200 0000 721f 0000 0072 1f00 0000 7220  ....r....r....r 
+00003ba0: 0000 00da 0c5f 6a6f 625f 7772 6170 7065  ....._job_wrappe
+00003bb0: 725d 0200 0073 2a00 0000 0409 0401 0404  r]...s*.........
+00003bc0: 1001 0801 0e01 0801 0401 0601 0401 0cff  ................
+00003bd0: 0880 02fd 02ff 0807 1601 02fc 0803 1601  ................
+00003be0: 08ff 1401 7a12 5175 6575 652e 5f6a 6f62  ....z.Queue._job
+00003bf0: 5f77 7261 7070 6572 728f 0000 0063 0200  _wrapperr....c..
+00003c00: 0000 0200 0000 0000 0000 0300 0000 0600  ................
+00003c10: 0000 4300 0001 7356 0000 007c 006a 0074  ..C...sV...|.j.t
+00003c20: 017c 016a 0283 017c 006a 037c 017c 006a  .|.j...|.j.|.|.j
+00003c30: 0467 027c 016a 05a2 017c 016a 0664 018d  .g.|.j...|.j.d..
+00003c40: 047d 0274 07a0 0864 027c 016a 027c 016a  .}.t...d.|.j.|.j
+00003c50: 09a1 0301 007c 02a0 0aa1 0001 0074 0ba0  .....|.......t..
+00003c60: 0ba1 007c 015f 0c7c 027c 015f 0d64 0053  ...|._.|.|._.d.S
+00003c70: 0029 034e 2904 723e 0000 00da 0674 6172  .).N).r>.....tar
+00003c80: 6765 7472 1000 0000 7215 0000 007a 1973  getr....r....z.s
+00003c90: 7461 7274 696e 6720 6a6f 6220 2564 2028  tarting job %d (
+00003ca0: 6e61 6d65 3d25 7329 290e 7260 0000 0072  name=%s)).r`...r
+00003cb0: 4f00 0000 729f 0000 0072 e000 0000 7268  O...r....r....rh
+00003cc0: 0000 0072 1000 0000 7215 0000 0072 5e00  ...r....r....r^.
+00003cd0: 0000 7269 0000 0072 3e00 0000 7224 0000  ..ri...r>...r$..
+00003ce0: 0072 8a00 0000 da0f 7374 6172 745f 7469  .r......start_ti
+00003cf0: 6d65 7374 616d 70da 0969 6e6e 6572 5f6a  mestamp..inner_j
+00003d00: 6f62 2903 721e 0000 0072 8f00 0000 72e3  ob).r....r....r.
+00003d10: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
+00003d20: 0000 72aa 0000 0077 0200 0073 1400 0000  ..r....w...s....
+00003d30: 0401 0801 0401 0e01 0401 06fc 1207 0801  ................
+00003d40: 0a02 0a01 7a10 5175 6575 652e 5f73 7461  ....z.Queue._sta
+00003d50: 7274 5f6a 6f62 6302 0000 0002 0000 0000  rt_jobc.........
+00003d60: 0000 0003 0000 0005 0000 0043 0000 0173  ...........C...s
+00003d70: c400 0000 7c00 6a00 7401 6a02 7500 720d  ....|.j.t.j.u.r.
+00003d80: 7c01 6a03 6401 6b04 720d 4a00 8201 7c00  |.j.d.k.r.J...|.
+00003d90: a004 a100 7215 7405 6402 8301 8201 7406  ....r.t.d.....t.
+00003da0: a006 a100 7c01 5f07 7c00 6a08 7c01 5f09  ....|._.|.j.|._.
+00003db0: 7c00 0400 6a0a 6403 3700 0200 5f0a 7c00  |...j.d.7..._.|.
+00003dc0: 6a0a 7c01 5f0b 7c01 6a0c 6404 7500 7232  j.|._.|.j.d.u.r2
+00003dd0: 7c01 6a0b 7c01 5f0c 740d a00e 6405 7c01  |.j.|._.t...d.|.
+00003de0: 6a0b 7c01 6a0c a103 0100 7c00 6a0f a010  j.|.j.....|.j...
+00003df0: 7c01 6a11 a101 7d02 7c02 6404 7501 724e  |.j...}.|.d.u.rN
+00003e00: 7412 7c02 7c01 8302 0100 7c01 6a0b 5300  t.|.|.....|.j.S.
+00003e10: 6700 7d02 7c02 7c00 6a0f 7c01 6a11 3c00  g.}.|.|.j.|.j.<.
+00003e20: 7412 7c00 6a0f 7c00 6a13 1900 7c01 8302  t.|.j.|.j...|...
+00003e30: 0100 7c01 6a0b 5300 2906 6102 0100 0053  ..|.j.S.).a....S
+00003e40: 7562 6d69 7473 2061 206a 6f62 2069 6e74  ubmits a job int
+00003e50: 6f20 7468 6520 7070 7175 6575 652e 5175  o the ppqueue.Qu
+00003e60: 6575 6520 7379 7374 656d 2e0a 0a20 2020  eue system...   
+00003e70: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00003e80: 2020 2020 2020 206a 6f62 3a20 2e2e 2e0a         job: ....
+00003e90: 0a20 2020 2020 2020 2052 6169 7365 733a  .        Raises:
+00003ea0: 0a20 2020 2020 2020 2020 2020 204f 7665  .            Ove
+00003eb0: 7266 6c6f 7745 7272 6f72 3a20 6966 206d  rflowError: if m
+00003ec0: 6178 5f73 697a 6520 7769 6c6c 2062 6520  ax_size will be 
+00003ed0: 6578 6365 6564 6564 2061 6674 6572 2061  exceeded after a
+00003ee0: 6464 696e 6720 7468 6973 206a 6f62 2e0a  dding this job..
+00003ef0: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00003f00: 3a0a 2020 2020 2020 2020 2020 2020 5468  :.            Th
+00003f10: 6520 6e75 6d62 6572 206f 6620 6a6f 6273  e number of jobs
+00003f20: 2073 7562 6d69 7474 6564 2074 6f20 7468   submitted to th
+00003f30: 6520 7175 6575 652e 0a20 2020 2020 2020  e queue..       
+00003f40: 2072 0100 0000 7a18 4d61 7820 7175 6575   r....z.Max queu
+00003f50: 6520 7369 7a65 2065 7863 6565 6465 642e  e size exceeded.
+00003f60: 720a 0000 004e 7a18 7175 6575 696e 6720  r....Nz.queuing 
+00003f70: 6a6f 6220 2564 2028 6e61 6d65 3d25 7329  job %d (name=%s)
+00003f80: 2914 7260 0000 0072 2800 0000 725a 0000  ).r`...r(...rZ..
+00003f90: 0072 ce00 0000 72ca 0000 00da 0d4f 7665  .r....r......Ove
+00003fa0: 7266 6c6f 7745 7272 6f72 728a 0000 00da  rflowErrorr.....
+00003fb0: 1073 7562 6d69 745f 7469 6d65 7374 616d  .submit_timestam
+00003fc0: 7072 5000 0000 da03 7169 6472 5200 0000  prP.....qidrR...
+00003fd0: 729f 0000 0072 3e00 0000 725e 0000 0072  r....r>...r^...r
+00003fe0: 6900 0000 7261 0000 0072 8600 0000 72a8  i...ra...r....r.
+00003ff0: 0000 0072 0400 0000 723a 0000 0029 0372  ...r....r:...).r
+00004000: 1e00 0000 728f 0000 0072 8d00 0000 721f  ....r....r....r.
+00004010: 0000 0072 1f00 0000 7220 0000 00da 075f  ...r....r ....._
+00004020: 7375 626d 6974 8502 0000 7324 0000 001a  submit....s$....
+00004030: 0d08 0208 010a 0208 020e 0108 010a 0208  ................
+00004040: 0112 020e 0208 010a 0106 0904 f90c 0112  ................
+00004050: 0406 027a 0d51 7565 7565 2e5f 7375 626d  ...z.Queue._subm
+00004060: 6974 fa14 5365 7175 656e 6365 5b41 6e79  it..Sequence[Any
+00004070: 5d20 7c20 4e6f 6e65 fa15 6469 6374 5b73  ] | None..dict[s
+00004080: 7472 2c20 416e 795d 207c 204e 6f6e 65da  tr, Any] | None.
+00004090: 0870 7269 6f72 6974 7972 a800 0000 72df  .priorityr....r.
+000040a0: 0000 0072 a900 0000 630a 0000 0002 0000  ...r....c.......
+000040b0: 0000 0000 000b 0000 000b 0000 0043 0000  .............C..
+000040c0: 0173 2400 0000 7400 7c01 7c02 7c03 7c04  .s$...t.|.|.|.|.
+000040d0: 7c05 7c06 7c07 7c08 7c09 6401 8d09 7d0a  |.|.|.|.|.d...}.
+000040e0: 7c00 a001 7c0a a101 5300 2902 6126 0300  |...|...S.).a&..
+000040f0: 0041 6464 7320 6120 6a6f 6220 746f 2074  .Adds a job to t
+00004100: 6865 2071 7565 7565 2e0a 0a20 2020 2020  he queue...     
+00004110: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
+00004120: 2020 2020 2066 756e 3a20 2e2e 2e0a 2020       fun: ....  
+00004130: 2020 2020 2020 2020 2020 6172 6773 3a20            args: 
+00004140: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00004150: 6b77 6172 6773 3a20 2e2e 2e0a 2020 2020  kwargs: ....    
+00004160: 2020 2020 2020 2020 6e61 6d65 3a20 2e2e          name: ..
+00004170: 2e0a 2020 2020 2020 2020 2020 2020 7072  ..            pr
+00004180: 696f 7269 7479 3a20 2e2e 2e0a 2020 2020  iority: ....    
+00004190: 2020 2020 2020 2020 6772 6f75 703a 202e          group: .
+000041a0: 2e2e 0a20 2020 2020 2020 2020 2020 2074  ...            t
+000041b0: 696d 656f 7574 3a20 2e2e 2e0a 2020 2020  imeout: ....    
+000041c0: 2020 2020 2020 2020 7375 7070 7265 7373          suppress
+000041d0: 5f65 7272 6f72 733a 202e 2e2e 0a20 2020  _errors: ....   
+000041e0: 2020 2020 2020 2020 2073 6b69 705f 6f6e           skip_on
+000041f0: 5f67 726f 7570 5f65 7272 6f72 3a20 2e2e  _group_error: ..
+00004200: 2e0a 0a20 2020 2020 2020 2052 6574 7572  ...        Retur
+00004210: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00004220: 2e2e 2e0a 0a20 2020 2020 2020 2045 7861  .....        Exa
+00004230: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+00004240: 2020 203e 3e3e 2066 726f 6d20 7070 7175     >>> from ppqu
+00004250: 6575 6520 696d 706f 7274 2051 7565 7565  eue import Queue
+00004260: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00004270: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00004280: 2064 6566 2061 6464 5f6e 756d 7328 783a   def add_nums(x:
+00004290: 2069 6e74 2c20 793a 2069 6e74 2920 2d3e   int, y: int) ->
+000042a0: 2069 6e74 3a0a 2020 2020 2020 2020 2020   int:.          
+000042b0: 2020 2e2e 2e20 2020 2020 7265 7475 726e    ...     return
+000042c0: 2078 202b 2079 0a20 2020 2020 2020 2020   x + y.         
+000042d0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+000042e0: 2020 203e 3e3e 2077 6974 6820 5175 6575     >>> with Queu
+000042f0: 6528 2920 6173 2071 7565 7565 3a0a 2020  e() as queue:.  
+00004300: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004310: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00004320: 2835 293a 0a20 2020 2020 2020 2020 2020  (5):.           
+00004330: 202e 2e2e 2020 2020 2020 2020 205f 203d   ...         _ =
+00004340: 2071 7565 7565 2e65 6e71 7565 7565 2861   queue.enqueue(a
+00004350: 6464 5f6e 756d 732c 2061 7267 733d 5b69  dd_nums, args=[i
+00004360: 2c20 3130 305d 290a 2020 2020 2020 2020  , 100]).        
+00004370: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00004380: 2020 2020 2e2e 2e20 2020 2020 6a6f 6273      ...     jobs
+00004390: 203d 2071 7565 7565 2e63 6f6c 6c65 6374   = queue.collect
+000043a0: 2877 6169 743d 5472 7565 290a 2020 2020  (wait=True).    
+000043b0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+000043c0: 2020 2020 2020 2020 3e3e 3e20 5b6a 6f62          >>> [job
+000043d0: 2e72 6573 756c 7420 666f 7220 6a6f 6220  .result for job 
+000043e0: 696e 206a 6f62 735d 0a20 2020 2020 2020  in jobs].       
+000043f0: 2020 2020 205b 3130 302c 2031 3031 2c20       [100, 101, 
+00004400: 3130 322c 2031 3033 2c20 3130 345d 0a20  102, 103, 104]. 
+00004410: 2020 2020 2020 2029 0972 1300 0000 7210         ).r....r.
+00004420: 0000 0072 1500 0000 723e 0000 0072 ea00  ...r....r>...r..
+00004430: 0000 72a8 0000 0072 ce00 0000 72df 0000  ..r....r....r...
+00004440: 0072 a900 0000 2902 720b 0000 0072 e700  .r....).r....r..
+00004450: 0000 290b 721e 0000 0072 1300 0000 7210  ..).r....r....r.
+00004460: 0000 0072 1500 0000 723e 0000 0072 ea00  ...r....r>...r..
+00004470: 0000 72a8 0000 0072 ce00 0000 72df 0000  ..r....r....r...
+00004480: 0072 a900 0000 728f 0000 0072 1f00 0000  .r....r....r....
+00004490: 721f 0000 0072 2000 0000 7271 0000 00af  r....r ...rq....
+000044a0: 0200 0073 1800 0000 022c 0201 0201 0201  ...s.....,......
+000044b0: 0201 0201 0201 0201 0201 0201 06f7 0a0c  ................
+000044c0: 7a0d 5175 6575 652e 656e 7175 6575 6563  z.Queue.enqueuec
+000044d0: 0100 0000 0000 0000 0000 0000 0300 0000  ................
+000044e0: 0400 0000 4f00 0001 72cb 0000 0029 0161  ....O...r....).a
+000044f0: 7802 0000 416c 6961 7320 666f 7220 6065  x...Alias for `e
+00004500: 6e71 7565 7565 602e 0a0a 2020 2020 2020  nqueue`...      
+00004510: 2020 4164 6473 2061 206a 6f62 2074 6f20    Adds a job to 
+00004520: 7468 6520 7175 6575 652e 0a0a 2020 2020  the queue...    
+00004530: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
+00004540: 2020 2020 2020 2a61 7267 733a 202e 2e2e        *args: ...
+00004550: 0a20 2020 2020 2020 2020 2020 202a 2a6b  .            **k
+00004560: 7761 7267 733a 202e 2e2e 0a0a 2020 2020  wargs: .....    
+00004570: 2020 2020 5265 7475 726e 733a 0a20 2020      Returns:.   
+00004580: 2020 2020 2020 2020 202e 2e2e 0a0a 2020           .....  
+00004590: 2020 2020 2020 4578 616d 706c 6573 3a0a        Examples:.
+000045a0: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+000045b0: 6672 6f6d 2070 7071 7565 7565 2069 6d70  from ppqueue imp
+000045c0: 6f72 7420 5175 6575 650a 2020 2020 2020  ort Queue.      
+000045d0: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+000045e0: 2020 2020 2020 3e3e 3e20 6465 6620 6164        >>> def ad
+000045f0: 645f 6e75 6d73 2878 3a20 696e 742c 2079  d_nums(x: int, y
+00004600: 3a20 696e 7429 202d 3e20 696e 743a 0a20  : int) -> int:. 
+00004610: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00004620: 2020 2072 6574 7572 6e20 7820 2b20 790a     return x + y.
+00004630: 2020 2020 2020 2020 2020 2020 2e2e 2e0a              ....
+00004640: 2020 2020 2020 2020 2020 2020 3e3e 3e20              >>> 
+00004650: 7769 7468 2051 7565 7565 2829 2061 7320  with Queue() as 
+00004660: 7175 6575 653a 0a20 2020 2020 2020 2020  queue:.         
+00004670: 2020 202e 2e2e 2020 2020 2066 6f72 2069     ...     for i
+00004680: 2069 6e20 7261 6e67 6528 3529 3a0a 2020   in range(5):.  
+00004690: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+000046a0: 2020 2020 2020 5f20 3d20 7175 6575 652e        _ = queue.
+000046b0: 7075 7428 6164 645f 6e75 6d73 2c20 6172  put(add_nums, ar
+000046c0: 6773 3d5b 692c 2031 3030 5d29 0a20 2020  gs=[i, 100]).   
+000046d0: 2020 2020 2020 2020 202e 2e2e 2020 2020           ...    
+000046e0: 206a 6f62 7320 3d20 7175 6575 652e 636f   jobs = queue.co
+000046f0: 6c6c 6563 7428 7761 6974 3d54 7275 6529  llect(wait=True)
+00004700: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00004710: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00004720: 205b 6a6f 622e 7265 7375 6c74 2066 6f72   [job.result for
+00004730: 206a 6f62 2069 6e20 6a6f 6273 5d0a 2020   job in jobs].  
+00004740: 2020 2020 2020 2020 2020 5b31 3030 2c20            [100, 
+00004750: 3130 312c 2031 3032 2c20 3130 332c 2031  101, 102, 103, 1
+00004760: 3034 5d0a 2020 2020 2020 2020 2901 7271  04].        ).rq
+00004770: 0000 0072 cc00 0000 721f 0000 0072 1f00  ...r....r....r..
+00004780: 0000 7220 0000 00da 0370 7574 e902 0000  ..r .....put....
+00004790: 7302 0000 0010 1b7a 0951 7565 7565 2e70  s......z.Queue.p
+000047a0: 7574 2902 72ce 0000 0072 4000 0000 726e  ut).r....r@...rn
+000047b0: 0000 0072 6f00 0000 7270 0000 0063 0300  ...ro...rp...c..
+000047c0: 0000 0300 0000 0200 0000 0900 0000 0700  ................
+000047d0: 0000 4f00 0001 733c 0000 007c 0244 005d  ..O...s<...|.D.]
+000047e0: 147d 0774 007c 017c 0767 017c 05a2 0174  .}.t.|.|.g.|...t
+000047f0: 017c 0683 017c 0364 018d 047d 087c 00a0  .|...|.d...}.|..
+00004800: 027c 08a1 0101 0071 027c 006a 0364 027c  .|.....q.|.j.d.|
+00004810: 0464 038d 0253 0029 0461 5902 0000 5375  .d...S.).aY...Su
+00004820: 626d 6974 7320 6d61 6e79 206a 6f62 7320  bmits many jobs 
+00004830: 746f 2074 6865 2071 7565 7565 202d 2d20  to the queue -- 
+00004840: 6f6e 6520 666f 7220 6561 6368 2069 7465  one for each ite
+00004850: 6d20 696e 2074 6865 2069 7465 7261 626c  m in the iterabl
+00004860: 652e 2057 6169 7473 2066 6f72 2061 6c6c  e. Waits for all
+00004870: 2074 6f20 6669 6e69 7368 2c20 7468 656e   to finish, then
+00004880: 2072 6574 7572 6e73 2074 6865 2072 6573   returns the res
+00004890: 756c 7473 2e0a 0a20 2020 2020 2020 2041  ults...        A
+000048a0: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+000048b0: 2066 756e 3a20 2e2e 2e0a 2020 2020 2020   fun: ....      
+000048c0: 2020 2020 2020 6974 6572 6162 6c65 3a20        iterable: 
+000048d0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+000048e0: 2a61 7267 733a 202e 2e2e 0a20 2020 2020  *args: ....     
+000048f0: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
+00004900: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00004910: 7368 6f77 5f70 726f 6772 6573 733a 202e  show_progress: .
+00004920: 2e2e 0a20 2020 2020 2020 2020 2020 202a  ...            *
+00004930: 2a6b 7761 7267 733a 202e 2e2e 0a0a 2020  *kwargs: .....  
+00004940: 2020 2020 2020 5265 7475 726e 733a 0a20        Returns:. 
+00004950: 2020 2020 2020 2020 2020 202e 2e2e 0a0a             .....
+00004960: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00004970: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
+00004980: 3e20 6672 6f6d 2070 7071 7565 7565 2069  > from ppqueue i
+00004990: 6d70 6f72 7420 5175 6575 650a 2020 2020  mport Queue.    
+000049a0: 2020 2020 2020 2020 3e3e 3e20 6672 6f6d          >>> from
+000049b0: 2074 696d 6520 696d 706f 7274 2073 6c65   time import sle
+000049c0: 6570 0a20 2020 2020 2020 2020 2020 202e  ep.            .
+000049d0: 2e2e 0a20 2020 2020 2020 2020 2020 203e  ...            >
+000049e0: 3e3e 2077 6974 6820 5175 6575 6528 2920  >> with Queue() 
+000049f0: 6173 2071 7565 7565 3a0a 2020 2020 2020  as queue:.      
+00004a00: 2020 2020 2020 2e2e 2e20 2020 2020 6a6f        ...     jo
+00004a10: 6273 203d 2071 7565 7565 2e6d 6170 2873  bs = queue.map(s
+00004a20: 6c65 6570 2c20 5b31 2c20 322c 2033 2c20  leep, [1, 2, 3, 
+00004a30: 342c 2035 5d29 0a20 2020 2020 2020 2020  4, 5]).         
+00004a40: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00004a50: 2020 203e 3e3e 206c 656e 286a 6f62 7329     >>> len(jobs)
+00004a60: 0a20 2020 2020 2020 2020 2020 2035 0a20  .            5. 
+00004a70: 2020 2020 2020 20a9 0472 1300 0000 7210         ..r....r.
+00004a80: 0000 0072 1500 0000 72ce 0000 0054 a902  ...r....r....T..
+00004a90: 7272 0000 0072 4000 0000 a904 720b 0000  rr...r@.....r...
+00004aa0: 0072 6700 0000 72e7 0000 0072 7300 0000  .rg...r....rs...
+00004ab0: a909 721e 0000 0072 1300 0000 726e 0000  ..r....r....rn..
+00004ac0: 0072 ce00 0000 7240 0000 0072 1000 0000  .r....r@...r....
+00004ad0: 7215 0000 0072 7500 0000 728f 0000 0072  r....ru...r....r
+00004ae0: 1f00 0000 721f 0000 0072 2000 0000 da03  ....r....r .....
+00004af0: 6d61 7006 0300 0073 1200 0000 0821 0201  map....s.....!..
+00004b00: 0201 0801 0601 0201 06fc 0c06 0e02 7a09  ..............z.
+00004b10: 5175 6575 652e 6d61 70fa 1753 6571 7565  Queue.map..Seque
+00004b20: 6e63 655b 5365 7175 656e 6365 5b41 6e79  nce[Sequence[Any
+00004b30: 5d5d 6303 0000 0003 0000 0002 0000 0009  ]]c.............
+00004b40: 0000 0007 0000 004f 0000 0173 3e00 0000  .......O...s>...
+00004b50: 7c02 4400 5d15 7d07 7400 7c01 6700 7c07  |.D.].}.t.|.g.|.
+00004b60: a201 7c05 a201 7401 7c06 8301 7c03 6401  ..|...t.|...|.d.
+00004b70: 8d04 7d08 7c00 a002 7c08 a101 0100 7102  ..}.|...|.....q.
+00004b80: 7c00 6a03 6402 7c04 6403 8d02 5300 2904  |.j.d.|.d...S.).
+00004b90: 613c 0300 0053 7562 6d69 7473 206d 616e  a<...Submits man
+00004ba0: 7920 6a6f 6273 2074 6f20 7468 6520 7175  y jobs to the qu
+00004bb0: 6575 6520 2d2d 206f 6e65 2066 6f72 2065  eue -- one for e
+00004bc0: 6163 6820 7365 7175 656e 6365 2069 6e20  ach sequence in 
+00004bd0: 7468 6520 6974 6572 6162 6c65 2e20 5761  the iterable. Wa
+00004be0: 6974 7320 666f 7220 616c 6c20 746f 2066  its for all to f
+00004bf0: 696e 6973 682c 2074 6865 6e20 7265 7475  inish, then retu
+00004c00: 726e 7320 7468 6520 7265 7375 6c74 732e  rns the results.
+00004c10: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00004c20: 2020 2020 2020 2020 2020 2020 6675 6e3a              fun:
+00004c30: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+00004c40: 2069 7465 7261 626c 653a 202e 2e2e 0a20   iterable: .... 
+00004c50: 2020 2020 2020 2020 2020 202a 6172 6773             *args
+00004c60: 3a20 7374 6174 6963 2061 7267 756d 656e  : static argumen
+00004c70: 7473 2070 6173 7365 6420 746f 2074 6865  ts passed to the
+00004c80: 2066 756e 6374 696f 6e2e 0a20 2020 2020   function..     
+00004c90: 2020 2020 2020 2074 696d 656f 7574 3a20         timeout: 
+00004ca0: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00004cb0: 7368 6f77 5f70 726f 6772 6573 733a 202e  show_progress: .
+00004cc0: 2e2e 0a20 2020 2020 2020 2020 2020 202a  ...            *
+00004cd0: 2a6b 7761 7267 733a 2073 7461 7469 6320  *kwargs: static 
+00004ce0: 6b65 7977 6f72 642d 6172 6775 6d65 6e74  keyword-argument
+00004cf0: 7320 7061 7373 6564 2074 6f20 7468 6520  s passed to the 
+00004d00: 6675 6e63 7469 6f6e 2e0a 0a20 2020 2020  function...     
+00004d10: 2020 2052 6574 7572 6e73 3a0a 2020 2020     Returns:.    
+00004d20: 2020 2020 2020 2020 2e2e 2e0a 0a20 2020          .....   
+00004d30: 2020 2020 2045 7861 6d70 6c65 733a 0a20       Examples:. 
+00004d40: 2020 2020 2020 2020 2020 203e 3e3e 2066             >>> f
+00004d50: 726f 6d20 7070 7175 6575 6520 696d 706f  rom ppqueue impo
+00004d60: 7274 2051 7565 7565 0a20 2020 2020 2020  rt Queue.       
+00004d70: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00004d80: 2020 2020 203e 3e3e 2064 6566 2061 6464       >>> def add
+00004d90: 5f6e 756d 7328 783a 2069 6e74 2c20 793a  _nums(x: int, y:
+00004da0: 2069 6e74 2920 2d3e 2069 6e74 3a0a 2020   int) -> int:.  
+00004db0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00004dc0: 2020 7265 7475 726e 2078 202b 2079 0a20    return x + y. 
+00004dd0: 2020 2020 2020 2020 2020 202e 2e2e 0a20             .... 
+00004de0: 2020 2020 2020 2020 2020 203e 3e3e 2077             >>> w
+00004df0: 6974 6820 5175 6575 6528 2920 6173 2071  ith Queue() as q
+00004e00: 7565 7565 3a0a 2020 2020 2020 2020 2020  ueue:.          
+00004e10: 2020 2e2e 2e20 2020 2020 6a6f 6273 203d    ...     jobs =
+00004e20: 2071 7565 7565 2e73 7461 726d 6170 280a   queue.starmap(.
+00004e30: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00004e40: 2020 2020 2020 2020 6164 645f 6e75 6d73          add_nums
+00004e50: 2c20 5b28 312c 2032 292c 2028 332c 2034  , [(1, 2), (3, 4
+00004e60: 295d 0a20 2020 2020 2020 2020 2020 202e  )].            .
+00004e70: 2e2e 2020 2020 2029 0a20 2020 2020 2020  ..     ).       
+00004e80: 2020 2020 202e 2e2e 0a20 2020 2020 2020       ....       
+00004e90: 2020 2020 203e 3e3e 205b 6a6f 622e 7265       >>> [job.re
+00004ea0: 7375 6c74 2066 6f72 206a 6f62 2069 6e20  sult for job in 
+00004eb0: 6a6f 6273 5d0a 2020 2020 2020 2020 2020  jobs].          
+00004ec0: 2020 5b33 2c20 375d 0a20 2020 2020 2020    [3, 7].       
+00004ed0: 2072 ec00 0000 5472 ed00 0000 72ee 0000   r....Tr....r...
+00004ee0: 0072 ef00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00004ef0: 7220 0000 00da 0773 7461 726d 6170 3203  r .....starmap2.
+00004f00: 0000 7312 0000 0008 2502 0102 010a 0106  ..s.....%.......
+00004f10: 0102 0106 fc0c 060e 027a 0d51 7565 7565  .........z.Queue
+00004f20: 2e73 7461 726d 6170 fa18 5365 7175 656e  .starmap..Sequen
+00004f30: 6365 5b64 6963 745b 7374 722c 2041 6e79  ce[dict[str, Any
+00004f40: 5d5d 6303 0000 0003 0000 0002 0000 0009  ]]c.............
+00004f50: 0000 0007 0000 004f 0000 0173 3e00 0000  .......O...s>...
+00004f60: 7c02 4400 5d15 7d07 7400 7c01 7401 7c05  |.D.].}.t.|.t.|.
+00004f70: 8301 6900 7c07 a501 7c06 a501 7c03 6401  ..i.|...|...|.d.
+00004f80: 8d04 7d08 7c00 a002 7c08 a101 0100 7102  ..}.|...|.....q.
+00004f90: 7c00 6a03 6402 7c04 6403 8d02 5300 2904  |.j.d.|.d...S.).
+00004fa0: 617b 0300 0053 7562 6d69 7473 206d 616e  a{...Submits man
+00004fb0: 7920 6a6f 6273 2074 6f20 7468 6520 7175  y jobs to the qu
+00004fc0: 6575 6520 2d2d 206f 6e65 2066 6f72 2065  eue -- one for e
+00004fd0: 6163 6820 6469 6374 696f 6e61 7279 2069  ach dictionary i
+00004fe0: 6e20 7468 6520 6974 6572 6162 6c65 2e20  n the iterable. 
+00004ff0: 5761 6974 7320 666f 7220 616c 6c20 746f  Waits for all to
+00005000: 2066 696e 6973 682c 2074 6865 6e20 7265   finish, then re
+00005010: 7475 726e 7320 7468 6520 7265 7375 6c74  turns the result
+00005020: 732e 0a0a 2020 2020 2020 2020 4172 6773  s...        Args
+00005030: 3a0a 2020 2020 2020 2020 2020 2020 6675  :.            fu
+00005040: 6e3a 202e 2e2e 0a20 2020 2020 2020 2020  n: ....         
+00005050: 2020 2069 7465 7261 626c 653a 202e 2e2e     iterable: ...
+00005060: 0a20 2020 2020 2020 2020 2020 202a 6172  .            *ar
+00005070: 6773 3a20 7374 6174 6963 2061 7267 756d  gs: static argum
+00005080: 656e 7473 2070 6173 7365 6420 746f 2074  ents passed to t
+00005090: 6865 2066 756e 6374 696f 6e2e 0a20 2020  he function..   
+000050a0: 2020 2020 2020 2020 2074 696d 656f 7574           timeout
+000050b0: 3a20 2e2e 2e0a 2020 2020 2020 2020 2020  : ....          
+000050c0: 2020 7368 6f77 5f70 726f 6772 6573 733a    show_progress:
+000050d0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+000050e0: 202a 2a6b 7761 7267 733a 2073 7461 7469   **kwargs: stati
+000050f0: 6320 6b65 7977 6f72 642d 6172 6775 6d65  c keyword-argume
+00005100: 6e74 7320 7061 7373 6564 2074 6f20 7468  nts passed to th
+00005110: 6520 6675 6e63 7469 6f6e 2e0a 0a20 2020  e function...   
+00005120: 2020 2020 2052 6574 7572 6e73 3a0a 2020       Returns:.  
+00005130: 2020 2020 2020 2020 2020 2e2e 2e0a 0a20            ..... 
+00005140: 2020 2020 2020 2045 7861 6d70 6c65 733a         Examples:
+00005150: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00005160: 2066 726f 6d20 7070 7175 6575 6520 696d   from ppqueue im
+00005170: 706f 7274 2051 7565 7565 0a20 2020 2020  port Queue.     
+00005180: 2020 2020 2020 203e 3e3e 2066 726f 6d20         >>> from 
+00005190: 7469 6d65 2069 6d70 6f72 7420 736c 6565  time import slee
+000051a0: 700a 2020 2020 2020 2020 2020 2020 2e2e  p.            ..
+000051b0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+000051c0: 3e20 6465 6620 6164 645f 6e75 6d73 2878  > def add_nums(x
+000051d0: 3a20 696e 742c 2079 3a20 696e 7429 202d  : int, y: int) -
+000051e0: 3e20 696e 743a 0a20 2020 2020 2020 2020  > int:.         
+000051f0: 2020 202e 2e2e 2020 2020 2072 6574 7572     ...     retur
+00005200: 6e20 7820 2b20 790a 2020 2020 2020 2020  n x + y.        
+00005210: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00005220: 2020 2020 3e3e 3e20 7769 7468 2051 7565      >>> with Que
+00005230: 7565 2829 2061 7320 7175 6575 653a 0a20  ue() as queue:. 
+00005240: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00005250: 2020 206a 6f62 7320 3d20 7175 6575 652e     jobs = queue.
+00005260: 7374 6172 6d61 706b 7728 0a20 2020 2020  starmapkw(.     
+00005270: 2020 2020 2020 202e 2e2e 2020 2020 2020         ...      
+00005280: 2020 2061 6464 5f6e 756d 732c 205b 7b27     add_nums, [{'
+00005290: 7827 3a20 312c 2027 7927 3a20 327d 2c20  x': 1, 'y': 2}, 
+000052a0: 7b27 7827 3a20 332c 2027 7927 3a20 347d  {'x': 3, 'y': 4}
+000052b0: 5d0a 2020 2020 2020 2020 2020 2020 2e2e  ].            ..
+000052c0: 2e20 2020 2020 290a 2020 2020 2020 2020  .     ).        
+000052d0: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+000052e0: 2020 2020 3e3e 3e20 5b6a 6f62 2e72 6573      >>> [job.res
+000052f0: 756c 7420 666f 7220 6a6f 6220 696e 206a  ult for job in j
+00005300: 6f62 735d 0a20 2020 2020 2020 2020 2020  obs].           
+00005310: 205b 332c 2037 5d0a 2020 2020 2020 2020   [3, 7].        
+00005320: 72ec 0000 0054 72ed 0000 0029 0472 0b00  r....Tr....).r..
+00005330: 0000 7284 0000 0072 e700 0000 7273 0000  ..r....r....rs..
+00005340: 0072 ef00 0000 721f 0000 0072 1f00 0000  .r....r....r....
+00005350: 7220 0000 00da 0973 7461 726d 6170 6b77  r .....starmapkw
+00005360: 6203 0000 7312 0000 0008 2602 0102 0106  b...s.....&.....
+00005370: 010a 0102 0106 fc0c 060e 027a 0f51 7565  ...........z.Que
+00005380: 7565 2e73 7461 726d 6170 6b77 2902 7272  ue.starmapkw).rr
+00005390: 0000 00da 055f 7065 656b 72f5 0000 00fa  ....._peekr.....
+000053a0: 0a4a 6f62 207c 204e 6f6e 6563 0100 0000  .Job | Nonec....
+000053b0: 0000 0000 0200 0000 0500 0000 0400 0000  ................
+000053c0: 4b00 0001 735e 0000 007c 00a0 00a1 0064  K...s^...|.....d
+000053d0: 016b 0272 187c 0173 0a64 0253 0064 037c  .k.r.|.s.d.S.d.|
+000053e0: 0364 043c 007c 006a 0164 0764 0564 0669  .d.<.|.j.d.d.d.i
+000053f0: 017c 03a4 018e 0101 007c 0272 217c 006a  .|.......|.r!|.j
+00005400: 0264 0119 007d 047c 0453 0074 037c 006a  .d...}.|.S.t.|.j
+00005410: 0283 017d 047c 0004 006a 0464 0637 0002  ...}.|...j.d.7..
+00005420: 005f 047c 0453 0029 0861 f802 0000 5265  ._.|.S.).a....Re
+00005430: 6d6f 7665 7320 616e 6420 7265 7475 726e  moves and return
+00005440: 7320 7468 6520 6669 6e69 7368 6564 206a  s the finished j
+00005450: 6f62 2077 6974 6820 7468 6520 6869 6768  ob with the high
+00005460: 6573 7420 7072 696f 7269 7479 2066 726f  est priority fro
+00005470: 6d20 7468 6520 7175 6575 652e 0a0a 2020  m the queue...  
+00005480: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00005490: 2020 2020 2020 2020 7761 6974 3a20 6966          wait: if
+000054a0: 206e 6f20 6a6f 6273 2061 7265 2066 696e   no jobs are fin
+000054b0: 6973 6865 642c 2077 6169 7420 666f 7220  ished, wait for 
+000054c0: 6f6e 652e 0a20 2020 2020 2020 2020 2020  one..           
+000054d0: 202a 2a6b 7761 7267 733a 2070 6173 7365   **kwargs: passe
+000054e0: 6420 746f 2060 5175 6575 652e 7761 6974  d to `Queue.wait
+000054f0: 600a 0a20 2020 2020 2020 2052 6574 7572  `..        Retur
+00005500: 6e73 3a0a 2020 2020 2020 2020 2020 2020  ns:.            
+00005510: 2e2e 2e0a 0a20 2020 2020 2020 2045 7861  .....        Exa
+00005520: 6d70 6c65 733a 0a20 2020 2020 2020 2020  mples:.         
+00005530: 2020 203e 3e3e 2066 726f 6d20 7070 7175     >>> from ppqu
+00005540: 6575 6520 696d 706f 7274 2051 7565 7565  eue import Queue
+00005550: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00005560: 0a20 2020 2020 2020 2020 2020 203e 3e3e  .            >>>
+00005570: 2064 6566 2061 6464 5f6e 756d 7328 783a   def add_nums(x:
+00005580: 2069 6e74 2c20 793a 2069 6e74 2920 2d3e   int, y: int) ->
+00005590: 2069 6e74 3a0a 2020 2020 2020 2020 2020   int:.          
+000055a0: 2020 2e2e 2e20 2020 2020 7265 7475 726e    ...     return
+000055b0: 2078 202b 2079 0a20 2020 2020 2020 2020   x + y.         
+000055c0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+000055d0: 2020 203e 3e3e 2077 6974 6820 5175 6575     >>> with Queu
+000055e0: 6528 2920 6173 2071 7565 7565 3a0a 2020  e() as queue:.  
+000055f0: 2020 2020 2020 2020 2020 2e2e 2e20 2020            ...   
+00005600: 2020 666f 7220 6920 696e 2072 616e 6765    for i in range
+00005610: 2835 293a 0a20 2020 2020 2020 2020 2020  (5):.           
+00005620: 202e 2e2e 2020 2020 2020 2020 205f 203d   ...         _ =
+00005630: 2071 7565 7565 2e65 6e71 7565 7565 2861   queue.enqueue(a
+00005640: 6464 5f6e 756d 732c 2061 7267 733d 5b69  dd_nums, args=[i
+00005650: 2c20 3130 305d 290a 2020 2020 2020 2020  , 100]).        
+00005660: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00005670: 2020 2020 2e2e 2e20 2020 2020 6a6f 6273      ...     jobs
+00005680: 203d 205b 7175 6575 652e 6465 7175 6575   = [queue.dequeu
+00005690: 6528 7761 6974 3d54 7275 6529 2066 6f72  e(wait=True) for
+000056a0: 205f 2069 6e20 7261 6e67 6528 7175 6575   _ in range(queu
+000056b0: 652e 7369 7a65 2829 295d 0a20 2020 2020  e.size())].     
+000056c0: 2020 2020 2020 202e 2e2e 0a20 2020 2020         ....     
+000056d0: 2020 2020 2020 203e 3e3e 205b 6a6f 622e         >>> [job.
+000056e0: 7265 7375 6c74 2066 6f72 206a 6f62 2069  result for job i
+000056f0: 6e20 6a6f 6273 5d0a 2020 2020 2020 2020  n jobs].        
+00005700: 2020 2020 5b31 3030 2c20 3130 312c 2031      [100, 101, 1
+00005710: 3032 2c20 3130 332c 2031 3034 5d0a 2020  02, 103, 104].  
+00005720: 2020 2020 2020 7201 0000 004e 4672 4000        r....NFr@.
+00005730: 0000 72cd 0000 0072 0a00 0000 721f 0000  ..r....r....r...
+00005740: 0029 0572 af00 0000 7272 0000 0072 6300  .).r....rr...rc.
+00005750: 0000 7203 0000 0072 5300 0000 2905 721e  ..r....rS...).r.
+00005760: 0000 0072 7200 0000 72f5 0000 0072 1500  ...rr...r....r..
+00005770: 0000 728f 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00005780: 0072 2000 0000 7296 0000 0093 0300 0073  .r ...r........s
+00005790: 1600 0000 0c20 0401 0401 0802 1401 0403  ..... ..........
+000057a0: 0a01 0405 0afd 0e01 0402 7a0d 5175 6575  ..........z.Queu
+000057b0: 652e 6465 7175 6575 6563 0100 0000 0000  e.dequeuec......
+000057c0: 0000 0000 0000 0300 0000 0400 0000 4f00  ..............O.
+000057d0: 0001 72cb 0000 0029 0161 8102 0000 416c  ..r....).a....Al
+000057e0: 6961 7320 666f 7220 6064 6571 7565 7565  ias for `dequeue
+000057f0: 602e 0a0a 2020 2020 2020 2020 4172 6773  `...        Args
+00005800: 3a0a 2020 2020 2020 2020 2020 2020 2a61  :.            *a
+00005810: 7267 733a 202e 2e2e 0a20 2020 2020 2020  rgs: ....       
+00005820: 2020 2020 202a 2a6b 7761 7267 733a 202e       **kwargs: .
+00005830: 2e2e 0a0a 2020 2020 2020 2020 5265 7475  ....        Retu
+00005840: 726e 733a 0a20 2020 2020 2020 2020 2020  rns:.           
+00005850: 202e 2e2e 0a0a 2020 2020 2020 2020 4578   .....        Ex
+00005860: 616d 706c 6573 3a0a 2020 2020 2020 2020  amples:.        
+00005870: 2020 2020 3e3e 3e20 6672 6f6d 2070 7071      >>> from ppq
+00005880: 7565 7565 2069 6d70 6f72 7420 5175 6575  ueue import Queu
+00005890: 650a 2020 2020 2020 2020 2020 2020 2e2e  e.            ..
+000058a0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+000058b0: 3e20 6465 6620 6164 645f 6e75 6d73 2878  > def add_nums(x
+000058c0: 3a20 696e 742c 2079 3a20 696e 7429 202d  : int, y: int) -
+000058d0: 3e20 696e 743a 0a20 2020 2020 2020 2020  > int:.         
+000058e0: 2020 202e 2e2e 2020 2020 2072 6574 7572     ...     retur
+000058f0: 6e20 7820 2b20 790a 2020 2020 2020 2020  n x + y.        
+00005900: 2020 2020 2e2e 2e0a 2020 2020 2020 2020      ....        
+00005910: 2020 2020 3e3e 3e20 7769 7468 2051 7565      >>> with Que
+00005920: 7565 2829 2061 7320 7175 6575 653a 0a20  ue() as queue:. 
+00005930: 2020 2020 2020 2020 2020 202e 2e2e 2020             ...  
+00005940: 2020 2066 6f72 2069 2069 6e20 7261 6e67     for i in rang
+00005950: 6528 3529 3a0a 2020 2020 2020 2020 2020  e(5):.          
+00005960: 2020 2e2e 2e20 2020 2020 2020 2020 5f20    ...         _ 
+00005970: 3d20 7175 6575 652e 7075 7428 6164 645f  = queue.put(add_
+00005980: 6e75 6d73 2c20 6172 6773 3d5b 692c 2031  nums, args=[i, 1
+00005990: 3030 5d29 0a20 2020 2020 2020 2020 2020  00]).           
+000059a0: 202e 2e2e 0a20 2020 2020 2020 2020 2020   ....           
+000059b0: 202e 2e2e 2020 2020 206a 6f62 7320 3d20   ...     jobs = 
+000059c0: 5b71 7565 7565 2e70 6f70 2877 6169 743d  [queue.pop(wait=
+000059d0: 5472 7565 2920 666f 7220 5f20 696e 2072  True) for _ in r
+000059e0: 616e 6765 2871 7565 7565 2e73 697a 6528  ange(queue.size(
+000059f0: 2929 5d0a 2020 2020 2020 2020 2020 2020  ))].            
+00005a00: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00005a10: 3e3e 3e20 5b6a 6f62 2e72 6573 756c 7420  >>> [job.result 
+00005a20: 666f 7220 6a6f 6220 696e 206a 6f62 735d  for job in jobs]
+00005a30: 0a20 2020 2020 2020 2020 2020 205b 3130  .            [10
+00005a40: 302c 2031 3031 2c20 3130 322c 2031 3033  0, 101, 102, 103
+00005a50: 2c20 3130 345d 0a20 2020 2020 2020 20a9  , 104].        .
+00005a60: 0172 9600 0000 72cc 0000 0072 1f00 0000  .r....r....r....
+00005a70: 721f 0000 0072 2000 0000 729e 0000 00c3  r....r ...r.....
+00005a80: 0300 0073 0200 0000 1019 7a09 5175 6575  ...s......z.Queu
+00005a90: 652e 706f 7063 0100 0000 0000 0000 0000  e.popc..........
+00005aa0: 0000 0300 0000 0500 0000 4f00 0001 7318  ..........O...s.
+00005ab0: 0000 007c 006a 007c 0169 007c 02a4 0164  ...|.j.|.i.|...d
+00005ac0: 0164 0269 01a4 018e 0153 0029 0361 5803  .d.i.....S.).aX.
+00005ad0: 0000 5265 7475 726e 7320 7468 6520 6a6f  ..Returns the jo
+00005ae0: 6220 7769 7468 2074 6865 2068 6967 6865  b with the highe
+00005af0: 7374 2070 7269 6f72 6974 7920 6672 6f6d  st priority from
+00005b00: 2074 6865 2071 7565 7565 2e0a 0a20 2020   the queue...   
+00005b10: 2020 2020 2053 696d 696c 6172 2074 6f20       Similar to 
+00005b20: 6064 6571 7565 7565 6020 2f20 6070 6f70  `dequeue` / `pop
+00005b30: 602c 2062 7574 2074 6865 206a 6f62 2072  `, but the job r
+00005b40: 656d 6169 6e73 2069 6e20 7468 6520 7175  emains in the qu
+00005b50: 6575 652e 0a0a 2020 2020 2020 2020 4172  eue...        Ar
+00005b60: 6773 3a0a 2020 2020 2020 2020 2020 2020  gs:.            
+00005b70: 2a61 7267 733a 202e 2e2e 0a20 2020 2020  *args: ....     
+00005b80: 2020 2020 2020 202a 2a6b 7761 7267 733a         **kwargs:
+00005b90: 202e 2e2e 0a0a 2020 2020 2020 2020 5265   .....        Re
+00005ba0: 7475 726e 733a 0a20 2020 2020 2020 2020  turns:.         
+00005bb0: 2020 202e 2e2e 0a0a 2020 2020 2020 2020     .....        
+00005bc0: 4578 616d 706c 6573 3a0a 2020 2020 2020  Examples:.      
+00005bd0: 2020 2020 2020 3e3e 3e20 6672 6f6d 2070        >>> from p
+00005be0: 7071 7565 7565 2069 6d70 6f72 7420 5175  pqueue import Qu
+00005bf0: 6575 650a 2020 2020 2020 2020 2020 2020  eue.            
+00005c00: 2e2e 2e0a 2020 2020 2020 2020 2020 2020  ....            
+00005c10: 3e3e 3e20 6465 6620 6164 645f 6e75 6d73  >>> def add_nums
+00005c20: 2878 3a20 696e 742c 2079 3a20 696e 7429  (x: int, y: int)
+00005c30: 202d 3e20 696e 743a 0a20 2020 2020 2020   -> int:.       
+00005c40: 2020 2020 202e 2e2e 2020 2020 2072 6574       ...     ret
+00005c50: 7572 6e20 7820 2b20 790a 2020 2020 2020  urn x + y.      
+00005c60: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00005c70: 2020 2020 2020 3e3e 3e20 7769 7468 2051        >>> with Q
+00005c80: 7565 7565 2829 2061 7320 7175 6575 653a  ueue() as queue:
+00005c90: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+00005ca0: 2020 2020 2066 6f72 2069 2069 6e20 7261       for i in ra
+00005cb0: 6e67 6528 3529 3a0a 2020 2020 2020 2020  nge(5):.        
+00005cc0: 2020 2020 2e2e 2e20 2020 2020 2020 2020      ...         
+00005cd0: 5f20 3d20 7175 6575 652e 7075 7428 6164  _ = queue.put(ad
+00005ce0: 645f 6e75 6d73 2c20 6172 6773 3d5b 692c  d_nums, args=[i,
+00005cf0: 2031 3030 5d29 0a20 2020 2020 2020 2020   100]).         
+00005d00: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+00005d10: 2020 202e 2e2e 2020 2020 2070 7269 6e74     ...     print
+00005d20: 2827 4265 666f 7265 3a27 2c20 7175 6575  ('Before:', queu
+00005d30: 652e 7369 7a65 2829 290a 2020 2020 2020  e.size()).      
+00005d40: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00005d50: 2020 2020 2020 2e2e 2e20 2020 2020 6a6f        ...     jo
+00005d60: 6220 3d20 7175 6575 652e 7065 656b 2877  b = queue.peek(w
+00005d70: 6169 743d 5472 7565 290a 2020 2020 2020  ait=True).      
+00005d80: 2020 2020 2020 2e2e 2e0a 2020 2020 2020        ....      
+00005d90: 2020 2020 2020 2e2e 2e20 2020 2020 7072        ...     pr
+00005da0: 696e 7428 2741 6674 6572 3a27 2c20 7175  int('After:', qu
+00005db0: 6575 652e 7369 7a65 2829 290a 2020 2020  eue.size()).    
+00005dc0: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00005dd0: 2020 2020 2020 2020 4265 666f 7265 3a20          Before: 
+00005de0: 350a 2020 2020 2020 2020 2020 2020 4166  5.            Af
+00005df0: 7465 723a 2035 0a20 2020 2020 2020 2020  ter: 5.         
+00005e00: 2020 203e 3e3e 206a 6f62 2e72 6573 756c     >>> job.resul
+00005e10: 740a 2020 2020 2020 2020 2020 2020 3130  t.            10
+00005e20: 300a 2020 2020 2020 2020 72f5 0000 0054  0.        r....T
+00005e30: 72f7 0000 0072 cc00 0000 721f 0000 0072  r....r....r....r
+00005e40: 1f00 0000 7220 0000 00da 0470 6565 6bde  ....r .....peek.
+00005e50: 0300 0073 0200 0000 1821 7a0a 5175 6575  ...s.....!z.Queu
+00005e60: 652e 7065 656b 6303 0000 0000 0000 0000  e.peekc.........
+00005e70: 0000 0006 0000 0004 0000 000b 0000 0173  ...............s
+00005e80: 5000 0000 7c02 720c 8800 6a00 6406 6401  P...|.r...j.d.d.
+00005e90: 7c01 6901 7c03 a401 8e01 0100 8800 a001  |.i.|...........
+00005ea0: a100 7d04 7c01 6402 6b04 7219 7402 7c01  ..}.|.d.k.r.t.|.
+00005eb0: 7c04 8302 6e01 7c04 7d05 7403 8700 6601  |...n.|.}.t...f.
+00005ec0: 6403 6404 8408 7404 7c05 8301 4400 8301  d.d...t.|...D...
+00005ed0: 8301 5300 2907 6152 0300 0052 656d 6f76  ..S.).aR...Remov
+00005ee0: 6573 2061 6e64 2072 6574 7572 6e73 2061  es and returns a
+00005ef0: 6c6c 2066 696e 6973 6865 6420 6a6f 6273  ll finished jobs
+00005f00: 2066 726f 6d20 7468 6520 7175 6575 652e   from the queue.
+00005f10: 0a0a 2020 2020 2020 2020 4172 6773 3a0a  ..        Args:.
+00005f20: 2020 2020 2020 2020 2020 2020 6e3a 2063              n: c
+00005f30: 6f6c 6c65 6374 2074 6869 7320 6d61 6e79  ollect this many
+00005f40: 206a 6f62 7320 2864 6566 6175 6c74 3d30   jobs (default=0
+00005f50: 2c20 616c 6c29 0a20 2020 2020 2020 2020  , all).         
+00005f60: 2020 2077 6169 743a 2049 6620 5472 7565     wait: If True
+00005f70: 2c20 626c 6f63 6b20 756e 7469 6c20 7468  , block until th
+00005f80: 6973 206d 616e 7920 6a6f 6273 2061 7265  is many jobs are
+00005f90: 2066 696e 6973 6865 642e 2045 6c73 652c   finished. Else,
+00005fa0: 2069 6d6d 6564 6961 7465 6c79 2072 6574   immediately ret
+00005fb0: 7572 6e20 616c 6c20 6669 6e69 7368 6564  urn all finished
+00005fc0: 2e0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
+00005fd0: 6b77 6172 6773 3a20 6b77 6172 6773 2067  kwargs: kwargs g
+00005fe0: 6976 656e 2074 6f20 6051 7565 7565 2e77  iven to `Queue.w
+00005ff0: 6169 7460 2e0a 0a20 2020 2020 2020 2052  ait`...        R
+00006000: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
+00006010: 2020 2020 6120 6c69 7374 206f 6620 604a      a list of `J
+00006020: 6f62 6020 696e 7374 616e 6365 732e 0a0a  ob` instances...
+00006030: 2020 2020 2020 2020 4578 616d 706c 6573          Examples
+00006040: 3a0a 2020 2020 2020 2020 2020 2020 3e3e  :.            >>
+00006050: 3e20 6672 6f6d 2070 7071 7565 7565 2069  > from ppqueue i
+00006060: 6d70 6f72 7420 5175 6575 650a 2020 2020  mport Queue.    
+00006070: 2020 2020 2020 2020 2e2e 2e0a 2020 2020          ....    
+00006080: 2020 2020 2020 2020 3e3e 3e20 6465 6620          >>> def 
+00006090: 6164 645f 6e75 6d73 2878 3a20 696e 742c  add_nums(x: int,
+000060a0: 2079 3a20 696e 7429 202d 3e20 696e 743a   y: int) -> int:
+000060b0: 0a20 2020 2020 2020 2020 2020 202e 2e2e  .            ...
+000060c0: 2020 2020 2072 6574 7572 6e20 7820 2b20       return x + 
+000060d0: 790a 2020 2020 2020 2020 2020 2020 2e2e  y.            ..
+000060e0: 2e0a 2020 2020 2020 2020 2020 2020 3e3e  ..            >>
+000060f0: 3e20 7769 7468 2051 7565 7565 2829 2061  > with Queue() a
+00006100: 7320 7175 6575 653a 0a20 2020 2020 2020  s queue:.       
+00006110: 2020 2020 202e 2e2e 2020 2020 2066 6f72       ...     for
+00006120: 2069 2069 6e20 7261 6e67 6528 3529 3a0a   i in range(5):.
+00006130: 2020 2020 2020 2020 2020 2020 2e2e 2e20              ... 
+00006140: 2020 2020 2020 2020 5f20 3d20 7175 6575          _ = queu
+00006150: 652e 656e 7175 6575 6528 6164 645f 6e75  e.enqueue(add_nu
+00006160: 6d73 2c20 6172 6773 3d5b 692c 2031 3030  ms, args=[i, 100
+00006170: 5d29 0a20 2020 2020 2020 2020 2020 202e  ]).            .
+00006180: 2e2e 0a20 2020 2020 2020 2020 2020 202e  ...            .
+00006190: 2e2e 2020 2020 206a 6f62 7320 3d20 7175  ..     jobs = qu
+000061a0: 6575 652e 636f 6c6c 6563 7428 7761 6974  eue.collect(wait
+000061b0: 3d54 7275 6529 0a20 2020 2020 2020 2020  =True).         
+000061c0: 2020 202e 2e2e 0a20 2020 2020 2020 2020     ....         
+000061d0: 2020 203e 3e3e 2074 7970 6528 6a6f 6273     >>> type(jobs
+000061e0: 290a 2020 2020 2020 2020 2020 2020 3c63  ).            <c
+000061f0: 6c61 7373 2027 6c69 7374 273e 0a20 2020  lass 'list'>.   
+00006200: 2020 2020 2020 2020 203e 3e3e 206c 656e           >>> len
+00006210: 286a 6f62 7329 0a20 2020 2020 2020 2020  (jobs).         
+00006220: 2020 2035 0a20 2020 2020 2020 2072 cd00     5.        r..
+00006230: 0000 7201 0000 0063 0100 0000 0000 0000  ..r....c........
+00006240: 0000 0000 0200 0000 0300 0000 3300 0001  ............3...
+00006250: 7318 0000 0081 007c 005d 077d 0174 0088  s......|.].}.t..
+00006260: 0083 0156 0001 0071 0264 0053 0072 2e00  ...V...q.d.S.r..
+00006270: 0000 2901 da04 6e65 7874 2902 72b4 0000  ..)...next).r...
+00006280: 0072 8e00 0000 7225 0000 0072 1f00 0000  .r....r%...r....
+00006290: 7220 0000 0072 b600 0000 2504 0000 7304  r ...r....%...s.
+000062a0: 0000 0002 8016 007a 2051 7565 7565 2e63  .......z Queue.c
+000062b0: 6f6c 6c65 6374 2e3c 6c6f 6361 6c73 3e2e  ollect.<locals>.
+000062c0: 3c67 656e 6578 7072 3e4e 721f 0000 0029  <genexpr>Nr....)
+000062d0: 0572 7200 0000 72af 0000 00da 036d 696e  .rr...r......min
+000062e0: 7284 0000 0072 8700 0000 2906 721e 0000  r....r....).r...
+000062f0: 0072 cd00 0000 7272 0000 0072 1500 0000  .r....rr...r....
+00006300: 5a0a 6e5f 6669 6e69 7368 6564 5a0c 6e5f  Z.n_finishedZ.n_
+00006310: 746f 5f63 6f6c 6c65 6374 721f 0000 0072  to_collectr....r
+00006320: 2500 0000 7220 0000 0072 7300 0000 0104  %...r ...rs.....
+00006330: 0000 730a 0000 0004 1d14 0108 0216 021a  ..s.............
+00006340: 027a 0d51 7565 7565 2e63 6f6c 6c65 6374  .z.Queue.collect
+00006350: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
+00006360: 0001 0000 0043 0000 0172 2d00 0000 722e  .....C...r-...r.
+00006370: 0000 00a9 0172 5400 0000 7225 0000 0072  .....rT...r%...r
+00006380: 1f00 0000 721f 0000 0072 2000 0000 7245  ....r....r ...rE
+00006390: 0000 0027 0400 0072 3000 0000 7a14 5175  ...'...r0...z.Qu
+000063a0: 6575 652e 6d61 785f 636f 6e63 7572 7265  eue.max_concurre
+000063b0: 6e74 da05 7661 6c75 6563 0200 0000 0000  nt..valuec......
+000063c0: 0000 0000 0000 0200 0000 0200 0000 4300  ..............C.
+000063d0: 0001 f30a 0000 007c 017c 005f 0064 0053  .......|.|._.d.S
+000063e0: 0072 2e00 0000 72fb 0000 00a9 0272 1e00  .r....r......r..
+000063f0: 0000 72fc 0000 0072 1f00 0000 721f 0000  ..r....r....r...
+00006400: 0072 2000 0000 7245 0000 002b 0400 00f3  .r ...rE...+....
+00006410: 0200 0000 0a02 6301 0000 0000 0000 0000  ......c.........
+00006420: 0000 0001 0000 0001 0000 0043 0000 0172  ...........C...r
+00006430: 2d00 0000 722e 0000 00a9 0172 5100 0000  -...r......rQ...
+00006440: 7225 0000 0072 1f00 0000 721f 0000 0072  r%...r....r....r
+00006450: 2000 0000 723c 0000 002f 0400 0072 3000   ...r<.../...r0.
+00006460: 0000 7a0e 5175 6575 652e 6d61 785f 7369  ..z.Queue.max_si
+00006470: 7a65 6302 0000 0000 0000 0000 0000 0002  zec.............
+00006480: 0000 0002 0000 0043 0000 0172 fd00 0000  .......C...r....
+00006490: 722e 0000 0072 0001 0000 72fe 0000 0072  r....r....r....r
+000064a0: 1f00 0000 721f 0000 0072 2000 0000 723c  ....r....r ...r<
+000064b0: 0000 0033 0400 0072 ff00 0000 6301 0000  ...3...r....c...
+000064c0: 0000 0000 0000 0000 0001 0000 0001 0000  ................
+000064d0: 0043 0000 0173 0800 0000 7c00 6a00 6a01  .C...s....|.j.j.
+000064e0: 5300 722e 0000 0029 0272 1700 0000 7231  S.r....).r....r1
+000064f0: 0000 0072 2500 0000 721f 0000 0072 1f00  ...r%...r....r..
+00006500: 0000 7220 0000 0072 2f00 0000 3704 0000  ..r ...r/...7...
+00006510: 7302 0000 0008 027a 1051 7565 7565 2e69  s......z.Queue.i
+00006520: 735f 7275 6e6e 696e 6729 1472 4500 0000  s_running).rE...
+00006530: 7212 0000 0072 3c00 0000 7212 0000 0072  r....r<...r....r
+00006540: 3d00 0000 7246 0000 0072 3e00 0000 7247  =...rF...r>...rG
+00006550: 0000 0072 3f00 0000 7248 0000 0072 4000  ...r?...rH...r@.
+00006560: 0000 722c 0000 0072 4100 0000 722c 0000  ..r,...rA...r,..
+00006570: 0072 4200 0000 722c 0000 0072 4300 0000  .rB...r,...rC...
+00006580: 7212 0000 0072 4400 0000 722c 0000 0029  r....rD...r,...)
+00006590: 0672 1300 0000 7214 0000 0072 1000 0000  .r....r....r....
+000065a0: 7205 0000 0072 1500 0000 7205 0000 0072  r....r....r....r
+000065b0: 3200 0000 2904 7272 0000 0072 2c00 0000  2...).rr...r,...
+000065c0: 7222 0000 0072 2300 0000 2902 7222 0000  r"...r#...).r"..
+000065d0: 0072 3800 0000 2904 7210 0000 0072 0500  .r8...).r....r..
+000065e0: 0000 7222 0000 0072 2300 0000 2902 7222  ..r"...r#...).r"
+000065f0: 0000 0072 0b00 0000 2902 7222 0000 0072  ...r....).r"...r
+00006600: 1200 0000 2908 72ba 0000 0072 2c00 0000  ....).r....r,...
+00006610: 72bb 0000 0072 2c00 0000 72c0 0000 0072  r....r,...r....r
+00006620: 2c00 0000 7222 0000 0072 c100 0000 2908  ,...r"...r....).
+00006630: 72ba 0000 0072 2c00 0000 72bb 0000 0072  r....r,...r....r
+00006640: 2c00 0000 72c0 0000 0072 2c00 0000 7222  ,...r....r,...r"
+00006650: 0000 0072 1200 0000 7233 0000 0029 0a72  ...r....r3...).r
+00006660: cd00 0000 7212 0000 0072 ce00 0000 72d0  ....r....r....r.
+00006670: 0000 0072 cf00 0000 7212 0000 0072 4000  ...r....r....r@.
+00006680: 0000 72d1 0000 0072 2200 0000 7212 0000  ..r....r"...r...
+00006690: 0029 0a72 db00 0000 720b 0000 0072 6800  .).r....r....rh.
+000066a0: 0000 72dc 0000 0072 1000 0000 7205 0000  ..r....r....r...
+000066b0: 0072 1500 0000 7205 0000 0072 2200 0000  .r....r....r"...
+000066c0: 72dd 0000 0029 0472 8f00 0000 720b 0000  r....).r....r...
+000066d0: 0072 2200 0000 7223 0000 0029 0472 8f00  .r"...r#...).r..
+000066e0: 0000 720b 0000 0072 2200 0000 7212 0000  ..r....r"...r...
+000066f0: 0029 084e 4e4e 723b 0000 004e 7201 0000  .).NNNr;...Nr...
+00006700: 0046 4629 1472 1000 0000 72e8 0000 0072  .FF).r....r....r
+00006710: 1500 0000 72e9 0000 0072 3e00 0000 7247  ....r....r>...rG
+00006720: 0000 0072 ea00 0000 7212 0000 0072 a800  ...r....r....r..
+00006730: 0000 7239 0000 0072 ce00 0000 72d0 0000  ..r9...r....r...
+00006740: 0072 df00 0000 722c 0000 0072 a900 0000  .r....r,...r....
+00006750: 722c 0000 0072 1300 0000 7214 0000 0072  r,...r....r....r
+00006760: 2200 0000 7212 0000 0029 0e72 1300 0000  "...r....).r....
+00006770: 7214 0000 0072 6e00 0000 726f 0000 0072  r....rn...ro...r
+00006780: 1000 0000 7205 0000 0072 ce00 0000 72d0  ....r....r....r.
+00006790: 0000 0072 4000 0000 72d1 0000 0072 1500  ...r@...r....r..
+000067a0: 0000 7205 0000 0072 2200 0000 7270 0000  ..r....r"...rp..
+000067b0: 0029 0e72 1300 0000 7214 0000 0072 6e00  .).r....r....rn.
+000067c0: 0000 72f1 0000 0072 1000 0000 7205 0000  ..r....r....r...
+000067d0: 0072 ce00 0000 72d0 0000 0072 4000 0000  .r....r....r@...
+000067e0: 72d1 0000 0072 1500 0000 7205 0000 0072  r....r....r....r
+000067f0: 2200 0000 7270 0000 0029 0e72 1300 0000  "...rp...).r....
+00006800: 7214 0000 0072 6e00 0000 72f3 0000 0072  r....rn...r....r
+00006810: 1000 0000 7205 0000 0072 ce00 0000 72d0  ....r....r....r.
+00006820: 0000 0072 4000 0000 72d1 0000 0072 1500  ...r@...r....r..
+00006830: 0000 7205 0000 0072 2200 0000 7270 0000  ..r....r"...rp..
+00006840: 0029 0872 7200 0000 722c 0000 0072 f500  .).rr...r,...r..
+00006850: 0000 722c 0000 0072 1500 0000 7205 0000  ..r,...r....r...
+00006860: 0072 2200 0000 72f6 0000 0029 0672 1000  .r"...r....).r..
+00006870: 0000 7205 0000 0072 1500 0000 7205 0000  ..r....r....r...
+00006880: 0072 2200 0000 72f6 0000 0029 0272 0100  .r"...r....).r..
+00006890: 0000 4629 0872 cd00 0000 7212 0000 0072  ..F).r....r....r
+000068a0: 7200 0000 722c 0000 0072 1500 0000 7205  r...r,...r....r.
+000068b0: 0000 0072 2200 0000 7270 0000 0029 0272  ...r"...rp...).r
+000068c0: fc00 0000 7212 0000 0029 0472 fc00 0000  ....r....).r....
+000068d0: 7212 0000 0072 2200 0000 7223 0000 0029  r....r"...r#...)
+000068e0: 3472 3400 0000 7235 0000 0072 3600 0000  4r4...r5...r6...
+000068f0: 723a 0000 00da 0f5f 5f61 6e6e 6f74 6174  r:.....__annotat
+00006900: 696f 6e73 5f5f 725b 0000 00da 0963 7075  ions__r[.....cpu
+00006910: 5f63 6f75 6e74 725c 0000 0072 2100 0000  _countr\...r!...
+00006920: 7279 0000 0072 7c00 0000 7224 0000 0072  ry...r|...r$...r
+00006930: 2b00 0000 7274 0000 0072 9000 0000 7281  +...rt...r....r.
+00006940: 0000 0072 9200 0000 7294 0000 0072 9500  ...r....r....r..
+00006950: 0000 7298 0000 0072 6b00 0000 72ae 0000  ..r....rk...r...
+00006960: 0072 ab00 0000 72af 0000 0072 be00 0000  .r....r....r....
+00006970: 72c6 0000 0072 c700 0000 72bd 0000 0072  r....r....r....r
+00006980: 9900 0000 72c8 0000 0072 c900 0000 72ca  ....r....r....r.
+00006990: 0000 0072 9d00 0000 7272 0000 00da 0c73  ...r....rr.....s
+000069a0: 7461 7469 636d 6574 686f 6472 e000 0000  taticmethodr....
+000069b0: 72aa 0000 0072 e700 0000 7271 0000 0072  r....r....rq...r
+000069c0: eb00 0000 72f0 0000 0072 f200 0000 72f4  ....r....r....r.
+000069d0: 0000 0072 9600 0000 729e 0000 0072 f800  ...r....r....r..
+000069e0: 0000 7273 0000 0072 3700 0000 7245 0000  ..rs...r7...rE..
+000069f0: 00da 0673 6574 7465 7272 3c00 0000 722f  ...setterr<...r/
+00006a00: 0000 0072 1f00 0000 721f 0000 0072 1f00  ...r....r....r..
+00006a10: 0000 7220 0000 0072 3800 0000 4400 0000  ..r ...r8...D...
+00006a20: 73b0 0000 000a 000c 0106 0402 fe02 0404  s...............
+00006a30: 0102 0102 0102 0102 0102 0102 0102 010e  ................
+00006a40: f40a 6a0a 0d0a 030a 040a 040a 1410 100a  ..j.............
+00006a50: 0c0a 030a 030a 030a 060a 790a 070a 070a  ..........y.....
+00006a60: 0702 0a02 0102 010e fb0a 3202 0602 0102  ..........2.....
+00006a70: 010e fb0a 250a 030a 080a 080a 0802 0602  ....%...........
+00006a80: 0102 0102 010e fa02 480c 010a 190a 0e02  ........H.......
+00006a90: 2e02 0102 0102 0102 0102 0102 0102 010c  ................
+00006aa0: f50a 3a02 2302 010e f902 3202 010e f902  ..:.#.....2.....
+00006ab0: 3602 010e f902 3402 010e fc0a 300a 1b0c  6.....4.....0...
+00006ac0: 2302 260c 0104 030c 0102 030c 0104 030c  #.&.............
+00006ad0: 0102 0310 0172 3800 0000 291d da0a 5f5f  .....r8...)...__
+00006ae0: 6675 7475 7265 5f5f 7202 0000 00da 076c  future__r......l
+00006af0: 6f67 6769 6e67 724e 0000 0072 5b00 0000  oggingrN...r[...
+00006b00: 7228 0000 0072 8a00 0000 72ac 0000 00da  r(...r....r.....
+00006b10: 0568 6561 7071 7203 0000 0072 0400 0000  .heapqr....r....
+00006b20: da06 7479 7069 6e67 7205 0000 0072 0600  ..typingr....r..
+00006b30: 0000 7207 0000 00da 0475 7569 6472 0800  ..r......uuidr..
+00006b40: 0000 5a09 7471 646d 2e61 7574 6f72 0900  ..Z.tqdm.autor..
+00006b50: 0000 728f 0000 0072 0b00 0000 da05 7574  ..r....r......ut
+00006b60: 696c 7372 0c00 0000 720d 0000 0072 3400  ilsr....r....r4.
+00006b70: 0000 da04 494e 464f 725e 0000 0072 0f00  ....INFOr^...r..
+00006b80: 0000 7238 0000 0072 1f00 0000 721f 0000  ..r8...r....r...
+00006b90: 0072 1f00 0000 7220 0000 00da 083c 6d6f  .r....r .....<mo
+00006ba0: 6475 6c65 3e01 0000 0073 1e00 0000 0c00  dule>....s......
+00006bb0: 0802 0801 0801 0801 0801 1001 1401 0c01  ................
+00006bc0: 0c02 0c02 1001 0e02 0e03 1230            ...........0
```

### Comparing `ppqueue-0.3.0/src/ppqueue/__pycache__/utils.cpython-310.pyc` & `ppqueue-0.4.0/src/ppqueue/__pycache__/utils.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 22 04:39:29 2023 UTC, .py size: 2436 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 15% similar despite different names*

```diff
@@ -1,171 +1,150 @@
-00000000: 6f0d 0d0a 0000 0000 81d0 9364 8409 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 a375 cd64 3a08 0000  o........u.d:...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0173 7600 0000 6400  .....@...sv...d.
+00000020: 0004 0000 0040 0000 0173 7200 0000 6400  .....@...sr...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 5a02 6400 6402 6c03 5a03 6400 6403 6c04  Z.d.d.l.Z.d.d.l.
-00000050: 6d05 5a05 6d06 5a06 6d07 5a07 6d08 5a08  m.Z.m.Z.m.Z.m.Z.
-00000060: 0100 6422 6423 640a 640b 8405 5a09 6424  ..d"d#d.d...Z.d$
-00000070: 640d 640e 8404 5a0a 6425 6413 6414 8404  d.d...Z.d%d.d...
-00000080: 5a0b 6426 6427 641b 641c 8405 5a0c 6507  Z.d&d'd.d...Z.e.
-00000090: 641d 8301 5a0d 6428 6420 6421 8404 5a0e  d...Z.d(d d!..Z.
-000000a0: 6402 5300 2929 e900 0000 0029 01da 0b61  d.S.)).....)...a
-000000b0: 6e6e 6f74 6174 696f 6e73 4e29 04da 044c  nnotationsN)...L
-000000c0: 6973 74da 084f 7074 696f 6e61 6cda 0754  ist..Optional..T
-000000d0: 7970 6556 6172 da05 556e 696f 6eda 046e  ypeVar..Union..n
-000000e0: 616d 65da 0373 7472 da05 6c65 7665 6cfa  ame..str..level.
-000000f0: 0d4f 7074 696f 6e61 6c5b 696e 745d da06  .Optional[int]..
-00000100: 7265 7475 726e fa0e 6c6f 6767 696e 672e  return..logging.
-00000110: 4c6f 6767 6572 6302 0000 0000 0000 0000  Loggerc.........
-00000120: 0000 0004 0000 0006 0000 0043 0000 0173  ...........C...s
-00000130: 5000 0000 7400 a001 7c00 a101 7d02 7c02  P...t...|...}.|.
-00000140: a002 7c01 6401 7500 720e 7400 6a03 6e01  ..|.d.u.r.t.j.n.
-00000150: 7c01 a101 0100 6402 7c02 5f04 7400 a005  |.....d.|._.t...
-00000160: a100 7d03 7c03 a006 7400 a007 6403 6404  ..}.|...t...d.d.
-00000170: a102 a101 0100 7c02 a008 7c03 a101 0100  ......|...|.....
-00000180: 7c02 5300 2905 7a99 6765 7420 6f72 2063  |.S.).z.get or c
-00000190: 7265 6174 6520 6120 6c6f 6767 6572 2e0a  reate a logger..
-000001a0: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-000001b0: 2020 206e 616d 6520 2873 7472 290a 2020     name (str).  
-000001c0: 2020 2020 2020 6c65 7665 6c20 284f 7074        level (Opt
-000001d0: 696f 6e61 6c5b 696e 745d 293a 2044 6566  ional[int]): Def
-000001e0: 6175 6c74 7320 746f 206c 6f67 6769 6e67  aults to logging
-000001f0: 2e44 4542 5547 2e0a 0a20 2020 2052 6574  .DEBUG...    Ret
-00000200: 7572 6e73 3a0a 2020 2020 2020 2020 6c6f  urns:.        lo
-00000210: 6767 696e 672e 4c6f 6767 6572 0a20 2020  gging.Logger.   
-00000220: 204e 467a 2525 2861 7363 7469 6d65 2973   NFz%%(asctime)s
-00000230: 2025 286c 6576 656c 6e61 6d65 2973 2025   %(levelname)s %
-00000240: 286d 6573 7361 6765 2973 7a11 2559 2d25  (message)sz.%Y-%
-00000250: 6d2d 2564 2025 483a 254d 3a25 5329 09da  m-%d %H:%M:%S)..
-00000260: 076c 6f67 6769 6e67 da09 6765 744c 6f67  .logging..getLog
-00000270: 6765 72da 0873 6574 4c65 7665 6cda 0449  ger..setLevel..I
-00000280: 4e46 4fda 0970 726f 7061 6761 7465 da0d  NFO..propagate..
-00000290: 5374 7265 616d 4861 6e64 6c65 72da 0c73  StreamHandler..s
-000002a0: 6574 466f 726d 6174 7465 72da 0946 6f72  etFormatter..For
-000002b0: 6d61 7474 6572 da0a 6164 6448 616e 646c  matter..addHandl
-000002c0: 6572 2904 7207 0000 0072 0900 0000 da06  er).r....r......
-000002d0: 6c6f 6767 6572 5a0b 6c6f 675f 6861 6e64  loggerZ.log_hand
-000002e0: 6c65 72a9 0072 1700 0000 fa1f 2f64 726f  ler..r....../dro
-000002f0: 6e65 2f73 7263 2f73 7263 2f70 7071 7565  ne/src/src/ppque
-00000300: 7565 2f75 7469 6c73 2e70 79da 0a67 6574  ue/utils.py..get
-00000310: 5f6c 6f67 6765 7208 0000 0073 1200 0000  _logger....s....
-00000320: 0a0a 1802 0601 0802 0401 0a01 04ff 0a03  ................
-00000330: 0402 7219 0000 00da 0462 6f6f 6c63 0000  ..r......boolc..
-00000340: 0000 0000 0000 0000 0000 0000 0000 0200  ................
-00000350: 0000 4300 0001 730a 0000 0074 006a 0164  ..C...s....t.j.d
-00000360: 016b 0253 0029 024e da02 6e74 2902 da02  .k.S.).N..nt)...
-00000370: 6f73 7207 0000 0072 1700 0000 7217 0000  osr....r....r...
-00000380: 0072 1700 0000 7218 0000 00da 0d69 735f  .r....r......is_
-00000390: 7769 6e64 6f77 735f 6f73 2000 0000 7302  windows_os ...s.
-000003a0: 0000 000a 0172 1d00 0000 da04 6e75 6d31  .....r......num1
-000003b0: fa11 556e 696f 6e5b 696e 742c 2066 6c6f  ..Union[int, flo
-000003c0: 6174 5dda 046e 756d 32da 0369 6e74 6302  at]..num2..intc.
-000003d0: 0000 0000 0000 0000 0000 0003 0000 0004  ................
-000003e0: 0000 0043 0000 0173 5800 0000 7c00 7c01  ...C...sX...|.|.
-000003f0: 6b02 7206 6401 5300 7c00 720a 7c00 6e01  k.r.d.S.|.r.|.n.
-00000400: 6401 7c01 720f 7c01 6e01 6401 1800 7d02  d.|.r.|.n.d...}.
-00000410: 7c02 6401 6b02 721a 7400 7c02 8301 5300  |.d.k.r.t.|...S.
-00000420: 7c02 6401 6b04 7225 7401 6402 7400 7c02  |.d.k.r%t.d.t.|.
-00000430: 8301 8302 5300 7402 6403 7400 7c02 8301  ....S.t.d.t.|...
-00000440: 8302 5300 2904 6111 0100 0063 6f6d 7061  ..S.).a....compa
-00000450: 7265 2074 776f 206e 756d 6265 7273 2e0a  re two numbers..
-00000460: 0a20 2020 2041 7267 733a 0a20 2020 2020  .    Args:.     
-00000470: 2020 206e 756d 3120 2855 6e69 6f6e 5b69     num1 (Union[i
-00000480: 6e74 2c20 666c 6f61 745d 293a 2074 6865  nt, float]): the
-00000490: 2072 6566 6572 656e 6365 206e 756d 6265   reference numbe
-000004a0: 722e 0a20 2020 2020 2020 206e 756d 3220  r..        num2 
-000004b0: 2855 6e69 6f6e 5b69 6e74 2c20 666c 6f61  (Union[int, floa
-000004c0: 745d 293a 2074 6865 2063 6f6d 7061 7269  t]): the compari
-000004d0: 736f 6e20 6e75 6d62 6572 2e0a 0a20 2020  son number...   
-000004e0: 2052 6574 7572 6e73 3a0a 2020 2020 2020   Returns:.      
-000004f0: 2020 696e 743a 0a20 2020 2020 2020 2020    int:.         
-00000500: 2020 202a 2030 2020 6966 206e 756d 3120     * 0  if num1 
-00000510: 3d3d 206e 756d 320a 2020 2020 2020 2020  == num2.        
-00000520: 2020 2020 2a20 3120 2069 6620 6e75 6d31      * 1  if num1
-00000530: 203e 206e 756d 320a 2020 2020 2020 2020   > num2.        
-00000540: 2020 2020 2a20 2d31 2069 6620 6e75 6d31      * -1 if num1
-00000550: 203c 206e 756d 320a 2020 2020 7201 0000   < num2.    r...
-00000560: 00e9 0100 0000 e9ff ffff ff29 0372 2100  ...........).r!.
-00000570: 0000 da03 6d61 78da 036d 696e 2903 721e  ....max..min).r.
-00000580: 0000 0072 2000 0000 da04 6469 6666 7217  ...r .....diffr.
-00000590: 0000 0072 1700 0000 7218 0000 00da 0763  ...r....r......c
-000005a0: 6f6d 7061 7265 2400 0000 7310 0000 0008  ompare$...s.....
-000005b0: 0d04 0118 0208 0208 0108 020e 010e 0372  ...............r
-000005c0: 2700 0000 da07 6f62 6a65 6374 31da 066f  '.....object1..o
-000005d0: 626a 6563 74da 076f 626a 6563 7432 da02  bject..object2..
-000005e0: 6279 fa09 4c69 7374 5b73 7472 5dda 065f  by..List[str].._
-000005f0: 7374 6174 6563 0400 0000 0000 0000 0000  statec..........
-00000600: 0000 0500 0000 0600 0000 4300 0001 7352  ..........C...sR
-00000610: 0000 007c 0372 0a7c 0374 007c 0283 016b  ...|.r.|.t.|...k
-00000620: 0572 0a64 0153 0074 0174 027c 007c 027c  .r.d.S.t.t.|.|.|
-00000630: 0319 0083 0274 027c 017c 027c 0319 0083  .....t.|.|.|....
-00000640: 0283 027d 047c 0464 016b 0272 2774 037c  ...}.|.d.k.r't.|
-00000650: 007c 017c 027c 0364 0217 0064 038d 0453  .|.|.|.d...d...S
-00000660: 007c 0453 0029 0461 f001 0000 636f 6d70  .|.S.).a....comp
-00000670: 6172 6520 7477 6f20 6f62 6a65 6374 7320  are two objects 
-00000680: 6279 2061 206c 6973 7420 6f66 2061 7474  by a list of att
-00000690: 7269 6275 7465 732e 0a20 2020 2061 7474  ributes..    att
-000006a0: 7269 6275 7465 7320 6172 6520 636f 6d70  ributes are comp
-000006b0: 6172 6564 2069 7465 7261 7469 7665 6c79  ared iteratively
-000006c0: 2061 6e64 2074 6865 2063 6f6d 7061 7269   and the compari
-000006d0: 736f 6e20 7769 6c6c 0a20 2020 2073 686f  son will.    sho
-000006e0: 7274 2d63 6972 6375 6974 2077 6865 6e2f  rt-circuit when/
-000006f0: 6966 2074 6865 206f 626a 6563 7473 2061  if the objects a
-00000700: 7265 2064 6574 6572 6d69 6e65 6420 756e  re determined un
-00000710: 6571 7561 6c2e 0a0a 2020 2020 4172 6773  equal...    Args
-00000720: 3a0a 2020 2020 2020 2020 5f73 7461 7465  :.        _state
-00000730: 3a0a 2020 2020 2020 2020 6f62 6a65 6374  :.        object
-00000740: 3120 286f 626a 6563 7429 3a20 7468 6520  1 (object): the 
-00000750: 7265 6665 7265 6e63 6520 6f62 6a65 6374  reference object
-00000760: 2e0a 2020 2020 2020 2020 6f62 6a65 6374  ..        object
-00000770: 3220 286f 626a 6563 7429 3a20 7468 6520  2 (object): the 
-00000780: 636f 6d70 6172 6973 6f6e 206f 626a 6563  comparison objec
-00000790: 742e 0a20 2020 2020 2020 2062 7920 284c  t..        by (L
-000007a0: 6973 745b 7374 725d 293a 206c 6973 7420  ist[str]): list 
-000007b0: 6f66 2061 7474 7269 6275 7465 7320 746f  of attributes to
-000007c0: 2063 6f6d 7061 7265 2e0a 0a20 2020 2052   compare...    R
-000007d0: 6574 7572 6e73 3a0a 2020 2020 2020 2020  eturns:.        
-000007e0: 696e 743a 0a20 2020 2020 2020 2020 2020  int:.           
-000007f0: 202a 2030 2020 6966 206f 626a 6563 7431   * 0  if object1
-00000800: 203d 3d20 6f62 6a65 6374 320a 2020 2020   == object2.    
-00000810: 2020 2020 2020 2020 2a20 3120 2069 6620          * 1  if 
-00000820: 6f62 6a65 6374 3120 3e20 6f62 6a65 6374  object1 > object
-00000830: 320a 2020 2020 2020 2020 2020 2020 2a20  2.            * 
-00000840: 2d31 2069 6620 6f62 6a65 6374 3120 3c20  -1 if object1 < 
-00000850: 6f62 6a65 6374 320a 2020 2020 7201 0000  object2.    r...
-00000860: 0072 2200 0000 2902 722b 0000 0072 2d00  .r"...).r+...r-.
-00000870: 0000 2904 da03 6c65 6e72 2700 0000 da07  ..)...lenr'.....
-00000880: 6765 7461 7474 72da 0a63 6f6d 7061 7265  getattr..compare
-00000890: 5f62 7929 0572 2800 0000 722a 0000 0072  _by).r(...r*...r
-000008a0: 2b00 0000 722d 0000 0072 2600 0000 7217  +...r-...r&...r.
-000008b0: 0000 0072 1700 0000 7218 0000 0072 3000  ...r....r....r0.
-000008c0: 0000 4000 0000 730c 0000 0010 1104 031e  ..@...s.........
-000008d0: 0208 0214 0204 0272 3000 0000 da01 54da  .......r0.....T.
-000008e0: 016c fa07 6c69 7374 5b54 5d63 0100 0000  .l..list[T]c....
-000008f0: 0000 0000 0000 0000 0100 0000 0400 0000  ................
-00000900: 4300 0001 7312 0000 0074 0074 01a0 027c  C...s....t.t...|
-00000910: 00a1 01a0 03a1 0083 0153 00a9 014e 2904  .........S...N).
-00000920: da04 6c69 7374 da04 6469 6374 da08 6672  ..list..dict..fr
-00000930: 6f6d 6b65 7973 da04 6b65 7973 2901 7232  omkeys..keys).r2
-00000940: 0000 0072 1700 0000 7217 0000 0072 1800  ...r....r....r..
-00000950: 0000 da0b 6465 6475 7065 5f6c 6973 7462  ....dedupe_listb
-00000960: 0000 0073 0200 0000 1201 7239 0000 0072  ...s......r9...r
-00000970: 3400 0000 2906 7207 0000 0072 0800 0000  4...).r....r....
-00000980: 7209 0000 0072 0a00 0000 720b 0000 0072  r....r....r....r
-00000990: 0c00 0000 2902 720b 0000 0072 1a00 0000  ....).r....r....
-000009a0: 2906 721e 0000 0072 1f00 0000 7220 0000  ).r....r....r ..
-000009b0: 0072 1f00 0000 720b 0000 0072 2100 0000  .r....r....r!...
-000009c0: 2901 7201 0000 0029 0a72 2800 0000 7229  ).r....).r(...r)
-000009d0: 0000 0072 2a00 0000 7229 0000 0072 2b00  ...r*...r)...r+.
-000009e0: 0000 722c 0000 0072 2d00 0000 7221 0000  ..r,...r-...r!..
-000009f0: 0072 0b00 0000 7221 0000 0029 0472 3200  .r....r!...).r2.
-00000a00: 0000 7233 0000 0072 0b00 0000 7233 0000  ..r3...r....r3..
-00000a10: 0029 0fda 0a5f 5f66 7574 7572 655f 5f72  .)...__future__r
-00000a20: 0200 0000 720d 0000 0072 1c00 0000 da06  ....r....r......
-00000a30: 7479 7069 6e67 7203 0000 0072 0400 0000  typingr....r....
-00000a40: 7205 0000 0072 0600 0000 7219 0000 0072  r....r....r....r
-00000a50: 1d00 0000 7227 0000 0072 3000 0000 7231  ....r'...r0...r1
-00000a60: 0000 0072 3900 0000 7217 0000 0072 1700  ...r9...r....r..
-00000a70: 0000 7217 0000 0072 1800 0000 da08 3c6d  ..r....r......<m
-00000a80: 6f64 756c 653e 0100 0000 7314 0000 000c  odule>....s.....
-00000a90: 0008 0208 0118 010c 030a 180a 040c 1c08  ................
-00000aa0: 1f0e 03                                  ...
+00000050: 6d05 5a05 6d06 5a06 6d07 5a07 0100 6422  m.Z.m.Z.m.Z...d"
+00000060: 6423 640a 640b 8405 5a08 6424 640d 640e  d#d.d...Z.d$d.d.
+00000070: 8404 5a09 6425 6413 6414 8404 5a0a 6426  ..Z.d%d.d...Z.d&
+00000080: 6427 641b 641c 8405 5a0b 6507 641d 8301  d'd.d...Z.e.d...
+00000090: 5a0c 6428 6420 6421 8404 5a0d 6402 5300  Z.d(d d!..Z.d.S.
+000000a0: 2929 e900 0000 0029 01da 0b61 6e6e 6f74  )).....)...annot
+000000b0: 6174 696f 6e73 4e29 03da 044c 6973 74da  ationsN)...List.
+000000c0: 084f 7074 696f 6e61 6cda 0754 7970 6556  .Optional..TypeV
+000000d0: 6172 da04 6e61 6d65 da03 7374 72da 056c  ar..name..str..l
+000000e0: 6576 656c fa0d 4f70 7469 6f6e 616c 5b69  evel..Optional[i
+000000f0: 6e74 5dda 0672 6574 7572 6efa 0e6c 6f67  nt]..return..log
+00000100: 6769 6e67 2e4c 6f67 6765 7263 0200 0000  ging.Loggerc....
+00000110: 0000 0000 0000 0000 0400 0000 0600 0000  ................
+00000120: 4300 0001 7350 0000 0074 00a0 017c 00a1  C...sP...t...|..
+00000130: 017d 027c 02a0 027c 0164 0075 0072 0e74  .}.|...|.d.u.r.t
+00000140: 006a 036e 017c 01a1 0101 0064 017c 025f  .j.n.|.....d.|._
+00000150: 0474 00a0 05a1 007d 037c 03a0 0674 00a0  .t.....}.|...t..
+00000160: 0764 0264 03a1 02a1 0101 007c 02a0 087c  .d.d.......|...|
+00000170: 03a1 0101 007c 0253 0029 044e 467a 2525  .....|.S.).NFz%%
+00000180: 2861 7363 7469 6d65 2973 2025 286c 6576  (asctime)s %(lev
+00000190: 656c 6e61 6d65 2973 2025 286d 6573 7361  elname)s %(messa
+000001a0: 6765 2973 7a11 2559 2d25 6d2d 2564 2025  ge)sz.%Y-%m-%d %
+000001b0: 483a 254d 3a25 5329 09da 076c 6f67 6769  H:%M:%S)...loggi
+000001c0: 6e67 da09 6765 744c 6f67 6765 72da 0873  ng..getLogger..s
+000001d0: 6574 4c65 7665 6cda 0449 4e46 4fda 0970  etLevel..INFO..p
+000001e0: 726f 7061 6761 7465 da0d 5374 7265 616d  ropagate..Stream
+000001f0: 4861 6e64 6c65 72da 0c73 6574 466f 726d  Handler..setForm
+00000200: 6174 7465 72da 0946 6f72 6d61 7474 6572  atter..Formatter
+00000210: da0a 6164 6448 616e 646c 6572 2904 7206  ..addHandler).r.
+00000220: 0000 0072 0800 0000 da06 6c6f 6767 6572  ...r......logger
+00000230: 5a0b 6c6f 675f 6861 6e64 6c65 72a9 0072  Z.log_handler..r
+00000240: 1600 0000 fa1f 2f64 726f 6e65 2f73 7263  ....../drone/src
+00000250: 2f73 7263 2f70 7071 7565 7565 2f75 7469  /src/ppqueue/uti
+00000260: 6c73 2e70 79da 0a67 6574 5f6c 6f67 6765  ls.py..get_logge
+00000270: 7208 0000 0073 1200 0000 0a01 1802 0601  r....s..........
+00000280: 0802 0401 0a01 04ff 0a03 0402 7218 0000  ............r...
+00000290: 00da 0462 6f6f 6c63 0000 0000 0000 0000  ...boolc........
+000002a0: 0000 0000 0000 0000 0200 0000 4300 0001  ............C...
+000002b0: 730a 0000 0074 006a 0164 016b 0253 0029  s....t.j.d.k.S.)
+000002c0: 024e da02 6e74 2902 da02 6f73 7206 0000  .N..nt)...osr...
+000002d0: 0072 1600 0000 7216 0000 0072 1600 0000  .r....r....r....
+000002e0: 7217 0000 00da 0d69 735f 7769 6e64 6f77  r......is_window
+000002f0: 735f 6f73 1700 0000 7302 0000 000a 0172  s_os....s......r
+00000300: 1c00 0000 da04 6e75 6d31 fa0b 696e 7420  ......num1..int 
+00000310: 7c20 666c 6f61 74da 046e 756d 32da 0369  | float..num2..i
+00000320: 6e74 6302 0000 0000 0000 0000 0000 0003  ntc.............
+00000330: 0000 0004 0000 0043 0000 0173 5800 0000  .......C...sX...
+00000340: 7c00 7c01 6b02 7206 6401 5300 7c00 720a  |.|.k.r.d.S.|.r.
+00000350: 7c00 6e01 6401 7c01 720f 7c01 6e01 6401  |.n.d.|.r.|.n.d.
+00000360: 1800 7d02 7c02 6401 6b02 721a 7400 7c02  ..}.|.d.k.r.t.|.
+00000370: 8301 5300 7c02 6401 6b04 7225 7401 6402  ..S.|.d.k.r%t.d.
+00000380: 7400 7c02 8301 8302 5300 7402 6403 7400  t.|.....S.t.d.t.
+00000390: 7c02 8301 8302 5300 2904 7aca 436f 6d70  |.....S.).z.Comp
+000003a0: 6172 6520 7477 6f20 6e75 6d62 6572 732e  are two numbers.
+000003b0: 0a0a 2020 2020 4172 6773 3a0a 2020 2020  ..    Args:.    
+000003c0: 2020 2020 6e75 6d31 3a20 7468 6520 7265      num1: the re
+000003d0: 6665 7265 6e63 6520 6e75 6d62 6572 2e0a  ference number..
+000003e0: 2020 2020 2020 2020 6e75 6d32 3a20 7468          num2: th
+000003f0: 6520 636f 6d70 6172 6973 6f6e 206e 756d  e comparison num
+00000400: 6265 722e 0a0a 2020 2020 5265 7475 726e  ber...    Return
+00000410: 733a 0a20 2020 2020 2020 2030 2020 6966  s:.        0  if
+00000420: 206e 756d 3120 3d3d 206e 756d 320a 2020   num1 == num2.  
+00000430: 2020 2020 2020 3120 2069 6620 6e75 6d31        1  if num1
+00000440: 203e 206e 756d 320a 2020 2020 2020 2020   > num2.        
+00000450: 2d31 2069 6620 6e75 6d31 203c 206e 756d  -1 if num1 < num
+00000460: 320a 2020 2020 7201 0000 00e9 0100 0000  2.    r.........
+00000470: e9ff ffff ff29 0372 2000 0000 da03 6d61  .....).r .....ma
+00000480: 78da 036d 696e 2903 721d 0000 0072 1f00  x..min).r....r..
+00000490: 0000 da04 6469 6666 7216 0000 0072 1600  ....diffr....r..
+000004a0: 0000 7217 0000 00da 0763 6f6d 7061 7265  ..r......compare
+000004b0: 1b00 0000 7310 0000 0008 0c04 0118 0208  ....s...........
+000004c0: 0208 0108 020e 010e 0372 2600 0000 da07  .........r&.....
+000004d0: 6f62 6a65 6374 31da 066f 626a 6563 74da  object1..object.
+000004e0: 076f 626a 6563 7432 da02 6279 fa09 4c69  .object2..by..Li
+000004f0: 7374 5b73 7472 5dda 065f 7374 6174 6563  st[str].._statec
+00000500: 0400 0000 0000 0000 0000 0000 0500 0000  ................
+00000510: 0600 0000 4300 0001 7352 0000 007c 0372  ....C...sR...|.r
+00000520: 0a7c 0374 007c 0283 016b 0572 0a64 0153  .|.t.|...k.r.d.S
+00000530: 0074 0174 027c 007c 027c 0319 0083 0274  .t.t.|.|.|.....t
+00000540: 027c 017c 027c 0319 0083 0283 027d 047c  .|.|.|.......}.|
+00000550: 0464 016b 0272 2774 037c 007c 017c 027c  .d.k.r't.|.|.|.|
+00000560: 0364 0217 0064 038d 0453 007c 0453 0029  .d...d...S.|.S.)
+00000570: 0461 a401 0000 436f 6d70 6172 6520 7477  .a....Compare tw
+00000580: 6f20 6f62 6a65 6374 7320 6279 2061 206c  o objects by a l
+00000590: 6973 7420 6f66 2061 7474 7269 6275 7465  ist of attribute
+000005a0: 732e 0a0a 2020 2020 4174 7472 6962 7574  s...    Attribut
+000005b0: 6573 2061 7265 2063 6f6d 7061 7265 6420  es are compared 
+000005c0: 6974 6572 6174 6976 656c 7920 616e 6420  iteratively and 
+000005d0: 7468 6520 636f 6d70 6172 6973 6f6e 2077  the comparison w
+000005e0: 696c 6c0a 2020 2020 7368 6f72 742d 6369  ill.    short-ci
+000005f0: 7263 7569 7420 7768 656e 2f69 6620 7468  rcuit when/if th
+00000600: 6520 6f62 6a65 6374 7320 6172 6520 6465  e objects are de
+00000610: 7465 726d 696e 6564 2075 6e65 7175 616c  termined unequal
+00000620: 2e0a 0a20 2020 2041 7267 733a 0a20 2020  ...    Args:.   
+00000630: 2020 2020 206f 626a 6563 7431 3a20 7468       object1: th
+00000640: 6520 7265 6665 7265 6e63 6520 6f62 6a65  e reference obje
+00000650: 6374 2e0a 2020 2020 2020 2020 6f62 6a65  ct..        obje
+00000660: 6374 323a 2074 6865 2063 6f6d 7061 7269  ct2: the compari
+00000670: 736f 6e20 6f62 6a65 6374 2e0a 2020 2020  son object..    
+00000680: 2020 2020 6279 3a20 6c69 7374 206f 6620      by: list of 
+00000690: 6174 7472 6962 7574 6573 2074 6f20 636f  attributes to co
+000006a0: 6d70 6172 652e 0a0a 2020 2020 5265 7475  mpare...    Retu
+000006b0: 726e 733a 0a20 2020 2020 2020 2030 2020  rns:.        0  
+000006c0: 6966 206f 626a 6563 7431 203d 3d20 6f62  if object1 == ob
+000006d0: 6a65 6374 320a 2020 2020 2020 2020 3120  ject2.        1 
+000006e0: 2069 6620 6f62 6a65 6374 3120 3e20 6f62   if object1 > ob
+000006f0: 6a65 6374 320a 2020 2020 2020 2020 2d31  ject2.        -1
+00000700: 2069 6620 6f62 6a65 6374 3120 3c20 6f62   if object1 < ob
+00000710: 6a65 6374 320a 2020 2020 7201 0000 0072  ject2.    r....r
+00000720: 2100 0000 2902 722a 0000 0072 2c00 0000  !...).r*...r,...
+00000730: 2904 da03 6c65 6e72 2600 0000 da07 6765  )...lenr&.....ge
+00000740: 7461 7474 72da 0a63 6f6d 7061 7265 5f62  tattr..compare_b
+00000750: 7929 0572 2700 0000 7229 0000 0072 2a00  y).r'...r)...r*.
+00000760: 0000 722c 0000 0072 2500 0000 7216 0000  ..r,...r%...r...
+00000770: 0072 1600 0000 7217 0000 0072 2f00 0000  .r....r....r/...
+00000780: 3600 0000 730c 0000 0010 1004 031e 0208  6...s...........
+00000790: 0214 0204 0272 2f00 0000 da01 54da 016c  .....r/.....T..l
+000007a0: fa07 6c69 7374 5b54 5d63 0100 0000 0000  ..list[T]c......
+000007b0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+000007c0: 0001 7312 0000 0074 0074 01a0 027c 00a1  ..s....t.t...|..
+000007d0: 01a0 03a1 0083 0153 00a9 014e 2904 da04  .......S...N)...
+000007e0: 6c69 7374 da04 6469 6374 da08 6672 6f6d  list..dict..from
+000007f0: 6b65 7973 da04 6b65 7973 2901 7231 0000  keys..keys).r1..
+00000800: 0072 1600 0000 7216 0000 0072 1700 0000  .r....r....r....
+00000810: da0b 6465 6475 7065 5f6c 6973 7457 0000  ..dedupe_listW..
+00000820: 0073 0200 0000 1201 7238 0000 0072 3300  .s......r8...r3.
+00000830: 0000 2906 7206 0000 0072 0700 0000 7208  ..).r....r....r.
+00000840: 0000 0072 0900 0000 720a 0000 0072 0b00  ...r....r....r..
+00000850: 0000 2902 720a 0000 0072 1900 0000 2906  ..).r....r....).
+00000860: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
+00000870: 1e00 0000 720a 0000 0072 2000 0000 2901  ....r....r ...).
+00000880: 7201 0000 0029 0a72 2700 0000 7228 0000  r....).r'...r(..
+00000890: 0072 2900 0000 7228 0000 0072 2a00 0000  .r)...r(...r*...
+000008a0: 722b 0000 0072 2c00 0000 7220 0000 0072  r+...r,...r ...r
+000008b0: 0a00 0000 7220 0000 0029 0472 3100 0000  ....r ...).r1...
+000008c0: 7232 0000 0072 0a00 0000 7232 0000 0029  r2...r....r2...)
+000008d0: 0eda 0a5f 5f66 7574 7572 655f 5f72 0200  ...__future__r..
+000008e0: 0000 720c 0000 0072 1b00 0000 da06 7479  ..r....r......ty
+000008f0: 7069 6e67 7203 0000 0072 0400 0000 7205  pingr....r....r.
+00000900: 0000 0072 1800 0000 721c 0000 0072 2600  ...r....r....r&.
+00000910: 0000 722f 0000 0072 3000 0000 7238 0000  ..r/...r0...r8..
+00000920: 0072 1600 0000 7216 0000 0072 1600 0000  .r....r....r....
+00000930: 7217 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000940: 0000 0073 1400 0000 0c00 0802 0801 1401  ...s............
+00000950: 0c03 0a0f 0a04 0c1b 081e 0e03            ............
```

### Comparing `ppqueue-0.3.0/src/ppqueue/job.py` & `ppqueue-0.4.0/src/ppqueue/job.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,24 +64,24 @@
             self.args = []
         elif isinstance(self.args, str) or not isinstance(self.args, Iterable):
             self.args = [self.args]
 
         if self.kwargs is None:
             self.kwargs = {}
 
-    def _compare(self, job: object) -> int:
+    def _compare(self, job: Job) -> int:
         """compares two jobs by priority or index.
 
         Arguments:
-            job {ppqueue.Job}
+            job: ...
 
         Returns:
-            int -- `1` if `self` is greater than comparison,
-                  `-1` if `self` is less than,
-                  `0` if equal.
+            `1` if `self` is greater than comparison,
+            `-1` if `self` is less than,
+            `0` if equal.
         """
         return compare_by(self, job, by=["priority", "idx"])
 
     def __eq__(self, job: object) -> bool:
         return self._compare(job) == 0
 
     def __ne__(self, job: object) -> bool:
@@ -113,15 +113,19 @@
 
     def join(self, *args, **kwargs) -> None:
         # waits for the job to complete.
         if self.inner_job is not None:
             self.inner_job.join(*args, **kwargs)
 
     def get_exit_code(self) -> int | None:
-        """Exit code of the job."""
+        """Exit code of the job.
+
+        Returns:
+            ...
+        """
         if (
             not self.inner_job
             or not hasattr(self.inner_job, "exitcode")
             or self.inner_job.exitcode is None
         ):
             return None
         return self.inner_job.exitcode
@@ -142,14 +146,17 @@
             self.finish_timestamp = time.time()
             self.cancelled = True
             log.debug("Stopped data: '%d'", self.idx)
 
     def get_seconds_running(self) -> float | None:
         """The number of seconds a job was running for.
 
+        Returns:
+            ...
+
         Examples:
             >>> from ppqueue import Queue
             >>> from time import sleep
             ...
             >>> with Queue() as queue:
             ...     for i in range(5):
             ...         jobs = queue.map(sleep, [1, 2, 3])
@@ -160,63 +167,84 @@
         if not self.start_timestamp or not self.finish_timestamp:
             return None
         return self.finish_timestamp - self.start_timestamp
 
     def get_seconds_waiting(self) -> float | None:
         """The amount of time a data has spent in the waiting queue.
 
+        Returns:
+            ...
+
         Examples:
             >>> job.get_seconds_waiting()  # doctest: +SKIP
         """
         if not self.submit_timestamp:
             return None
 
         if not self.start_timestamp:
             return time.time() - self.submit_timestamp
 
         return self.start_timestamp - self.submit_timestamp
 
     def get_seconds_total(self) -> float | None:
         """Returns the waiting + running duration of this job.
 
+        Returns:
+            ...
+
         Examples:
             >>> job.get_seconds_total()  # doctest: +SKIP
         """
         if not self.submit_timestamp:
             return None
 
         if not self.finish_timestamp:
             return time.time() - self.submit_timestamp
 
         return self.finish_timestamp - self.submit_timestamp
 
     def get_submit_timestamp(self) -> datetime | None:
         """The time this job was submitted.
 
+        Returns:
+            ...
+
         Examples:
             >>> job.get_submit_timestamp()  # doctest: +SKIP
         """
         if self.submit_timestamp:
             return datetime.utcfromtimestamp(self.submit_timestamp)
         return None
 
     def get_start_timestamp(self) -> datetime | None:
-        """Returns a datetime object of the time this data was started."""
+        """Returns a datetime object of the time this data was started.
+
+        Returns:
+            ...
+        """
         if self.start_timestamp:
             return datetime.utcfromtimestamp(self.start_timestamp)
         return None
 
     def get_finish_timestamp(self) -> datetime | None:
-        """Returns a datetime object of the time this data finished."""
+        """Returns a datetime object of the time this data finished.
+
+        Returns:
+            ...
+        """
         if self.finish_timestamp:
             return datetime.utcfromtimestamp(self.finish_timestamp)
         return None
 
     def get_processed_timestamp(self) -> datetime | None:
-        """Returns a datetime object of the time this data was processed."""
+        """Returns a datetime object of the time this data was processed.
+
+        Returns:
+            ...
+        """
         if self.process_timestamp:
             return datetime.utcfromtimestamp(self.process_timestamp)
         return None
 
     def is_processed(self) -> bool:
         # Returns true if this data has been processed; false otherwise.
         # A processed data is one that has had its output gathered, callback called,
```

### Comparing `ppqueue-0.3.0/src/ppqueue/plot.py` & `ppqueue-0.4.0/src/ppqueue/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,23 +218,27 @@
     no_legend: bool = False,
     bar_width: int = 1,
     color_pal: list[str] | None = None,
 ) -> gg.ggplot:
     """
 
     Args:
-        title:
-        color_by:
-        facet_by:
-        facet_scale:
-        theme:
-        no_legend:
-        bar_width:
+        *args: Sequences of `Job` instances to plot.
+        title: ...
+        color_by: ...
+        facet_by: ...
+        facet_scale: ...
+        theme: ...
+        no_legend: ...
+        bar_width: ...
         color_pal: a sequence of colors used to color each group of `color_by`.
 
+    Returns:
+        ...
+
     Examples:
         >>> from ppqueue import Queue
         >>> from ppqueue.plot import plot_jobs
         >>> from time import sleep
         ...
         >>> with Queue() as queue:
         ...     q1_jobs = queue.map(sleep, [1, 2, 3, 4, 5])
```

### Comparing `ppqueue-0.3.0/src/ppqueue/queue.py` & `ppqueue-0.4.0/src/ppqueue/queue.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,30 +2,28 @@
 
 import logging
 import multiprocessing as mp
 import threading
 import time
 import traceback
 from heapq import heappop, heappush
-from typing import Any, Callable, Sequence, Type
+from typing import Any, Callable, Sequence
 from uuid import uuid4
 
 from tqdm.auto import tqdm
 
 from .job import Job
 from .utils import get_logger, is_windows_os
 
 LOG = get_logger(__name__, level=logging.INFO)
 
 
 class PulseTimer:
-    """Periodically runs a function in a background thread.
-
-    ref: https://stackoverflow.com/a/13151299
-    """
+    # Periodically runs a function in a background thread.
+    # src: https://stackoverflow.com/a/13151299
 
     def __init__(
         self,
         *args: Any,
         interval_ms: int,
         fun: Callable[..., Any],
         **kwargs: Any,
@@ -71,29 +69,29 @@
     DEFAULT_GROUP: int | None = None
 
     def __init__(
         self,
         max_concurrent: int = mp.cpu_count(),
         *,
         max_size: int = 0,
-        engine: Type[threading.Thread] | Type[mp.Process] = threading.Thread,
+        engine: str | type[mp.Process] | type[threading.Thread] = mp.Process,
         name: str | None = None,
         callback: Callable[[Job], Any] | None = None,
         show_progress: bool = False,
         drop_finished: bool = False,
         stop_when_idle: bool = False,
         pulse_freq_ms: int = 100,
         no_start: bool = False,
     ):
-        """
+        """A parallel processing job runner / data structure.
 
         Args:
             max_concurrent: max number of concurrently running jobs.
             max_size: max size of the queue (default=0, unlimited).
-            engine: the engine used to run jobs; threads (default) or processes.
+            engine: the engine used to run jobs.
             name: an identifier for this queue.
             callback: a callable that is called immediately after each job is finished.
             show_progress: global setting for showing progress bars.
             drop_finished: if True, the queue will not store finished jobs for retrieval.
             stop_when_idle: if True, the queue will stop the pulse when all jobs are finished.
             pulse_freq_ms: the interval at which jobs are transitioned between internal queues.
             no_start: if True, do not start the queue pulse on instantiation.
@@ -114,29 +112,42 @@
         self.show_progress: bool = show_progress
         self._max_size: int = max_size
         self._count_input: int = 0
         self._count_output: int = 0
         self._max_concurrent: int = max_concurrent
         self._callback: Callable[..., Any] | None = callback
 
-        self._lock: threading.Lock = (
-            threading.Lock()
-        )  # https://opensource.com/article/17/4/grok-gil
+        # https://opensource.com/article/17/4/grok-gil
+        self._lock: threading.Lock = threading.Lock()
+
+        if isinstance(engine, str):
+            if engine.lower() in ["thread", "threads", "threading"]:
+                engine = threading.Thread
+            elif engine.lower() in [
+                "process",
+                "processes",
+                "processing",
+                "multiprocessing",
+            ]:
+                engine = mp.Process
+            else:
+                err: str = f"Unrecognized engine: {engine}. Choose either 'process' or 'thread'."
+                raise ValueError(err)
 
         if engine is mp.Process and is_windows_os():
             LOG.warning(
                 (
                     "multiprocessing performance is degraded on Windows systems. see: "
                     "https://docs.python.org/3/library/multiprocessing.html?highlight=process#the-spawn-and-forkserver-start-methods"
                 ),
             )
 
-        self._engine: Type[mp.Process] | Type[threading.Thread] = engine
+        self._engine: type[mp.Process] | type[threading.Thread] = engine
 
-        self._waiting_groups: dict[int | None, list[Job]] = {None: []}
+        self._waiting_groups: dict[int | None, list[Job]] = {self.DEFAULT_GROUP: []}
         self._working_queue: dict[int | None, Job] = {}
         self._finished_queue: list[Job] = []
 
         self._drop_finished: bool = drop_finished
         self._mp_manager: mp.Manager | None = None
 
         self._output: dict[int, Job]
@@ -151,19 +162,19 @@
 
         self._pulse_freq_ms: int = pulse_freq_ms
         self._timer: PulseTimer = PulseTimer(
             interval_ms=self._pulse_freq_ms,
             fun=self._pulse,
         )
 
+        self._stop_when_idle: bool = stop_when_idle
+
         if not no_start:
             self.start()
 
-        self._stop_when_idle: bool = stop_when_idle
-
         LOG.debug("Initialized pulse.")
 
     # decorator
     def __call__(self, fun: Callable[..., Any], *args: Any, **kwargs: Any):
         self.start()
 
         def wrapped_f(iterable: Sequence[Any], *args: Any, **kwargs: Any) -> list[Job]:
@@ -204,16 +215,14 @@
         self._count_output = 0
         LOG.debug("Reset counters.")
 
         if self._mp_manager is not None:
             self._mp_manager.shutdown()
 
     def _clear_waiting(self) -> None:
-        """Clear the queue of pending jobs."""
-
         LOG.debug("Clearing waiting queue")
         with self._lock:
             keys = list(self._waiting_groups.keys())
             for k in keys:
                 group_jobs = self._waiting_groups.get(k)
                 for _ in range(len(group_jobs)):
                     job = heappop(group_jobs)
@@ -222,16 +231,14 @@
                     if not self._drop_finished:
                         heappush(self._finished_queue, job)
                     else:
                         self._count_output += 1
                 del self._waiting_groups[k]
 
     def _stop_all(self, *, wait: bool = True) -> None:
-        """Stop and remove all running and waiting jobs."""
-
         self._clear_waiting()
 
         keys = list(self._working_queue.keys())
         for k in keys:
             job = self._working_queue.get(k)
             if job is not None:
                 job.stop()
@@ -251,16 +258,15 @@
     def __next__(self) -> Job:
         job: Job | None = self.dequeue()
         if job is None:
             raise StopIteration
         return job
 
     def _pulse(self) -> None:
-        # TODO: document this better.
-        """Used internally; manages the queue system operations."""
+        # Used internally; manages the queue system operations.
 
         with self._lock:
             try:
                 if self._stop_when_idle and self.is_idle():
                     self.stop()
                 else:
                     # stop expired jobs.
@@ -355,15 +361,15 @@
                                         del self._waiting_groups[job.group]
 
                                     if next_job is not None:
                                         self._working_queue[next_job.idx] = next_job
                                         self._start_job(next_job)
 
                     while (
-                        len(self._waiting_groups[self.DEFAULT_GROUP]) > 0
+                        self._waiting_groups.get(self.DEFAULT_GROUP)
                         and self.max_concurrent - self._count_working() > 0
                     ):
                         job = heappop(self._waiting_groups[self.DEFAULT_GROUP])
                         self._working_queue[job.idx] = job
                         self._start_job(job)
             except:  # pylint: disable=bare-except
                 self.stop()
@@ -373,27 +379,39 @@
                     "waiting=%d; working=%d; finished=%d.",
                     self._count_waiting(),
                     self._count_working(),
                     self._count_finished(),
                 )
 
     def _count_waiting(self) -> int:
-        """Get the number of pending jobs."""
+        """
+        Returns:
+            The number of pending jobs.
+        """
         return sum(len(v) for _, v in self._waiting_groups.items())
 
     def _count_working(self) -> int:
-        """Get the number of running jobs."""
+        """
+        Returns:
+            The number of running jobs.
+        """
         return len(self._working_queue)
 
     def _count_finished(self) -> int:
-        """Get the number of completed jobs."""
+        """
+        Returns:
+            The number of completed jobs.
+        """
         return len(self._finished_queue)
 
     def _count_remaining(self) -> int:
-        """Get the number of unfinished jobs (i.e., waiting + working)."""
+        """
+        Returns:
+            The number of unfinished jobs (i.e., waiting + working).
+        """
         return self.size(waiting=True, working=True)
 
     def _sizes(
         self,
         *,
         waiting: bool = False,
         working: bool = False,
@@ -457,14 +475,17 @@
         If no options are given, the total number of jobs in the queue is returned.
 
         Args:
             waiting: include waiting jobs.
             working: include working jobs.
             finished: include finished jobs.
 
+        Returns:
+            ...
+
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
             >>> with Queue() as queue:
@@ -479,23 +500,35 @@
         """
         return sum(self._sizes(waiting=waiting, working=working, finished=finished))
 
     def is_idle(self) -> bool:
         return self._count_waiting() == 0 and self._count_working() == 0
 
     def is_busy(self) -> bool:
-        """True if max concurrent limit is reached or if there are waiting jobs."""
+        """True if max concurrent limit is reached or if there are waiting jobs.
+
+        Returns:
+            ...
+        """
         return self._count_waiting() > 0 or self.max_concurrent <= self._count_working()
 
     def is_empty(self) -> bool:
-        """True if there are no jobs in the queue system."""
+        """True if there are no jobs in the queue system.
+
+        Returns:
+            ...
+        """
         return self.size() == 0
 
     def is_full(self) -> bool:
-        """True if the number of jobs in the queue system is equal to max_size."""
+        """True if the number of jobs in the queue system is equal to max_size.
+
+        Returns:
+            ...
+        """
         return 0 < self._max_size <= self.size()
 
     def join(self, *args, **kwargs) -> int:
         return self.wait(*args, **kwargs)
 
     def wait(
         self,
@@ -508,14 +541,18 @@
         """Wait for jobs to finish.
 
         Args:
             n: the number of jobs to wait for (default=0, all).
             timeout: seconds to wait before raising `TimeoutError` (default=0, indefinitely).
             poll_ms: milliseconds to pause between checks (default=100).
             show_progress: if True, present a progress bar.
+
+        Returns:
+            If `n <= 0`, returns the count of unfinished jobs.
+            Else, returns the count of finished jobs.
         """
         if poll_ms is None or poll_ms <= 0:
             poll_ms = self._pulse_freq_ms
         elif poll_ms < self._pulse_freq_ms:
             err: str = "`poll_ms` must be >= `ppqueue.Queue.pulse_freq_ms`"
             raise ValueError(err)
 
@@ -569,15 +606,15 @@
     def _job_wrapper(
         _job: Job,
         _output: dict[int, tuple[str | None, str | None, int, float]],
         /,
         *args: Any,
         **kwargs: Any,
     ) -> tuple[str | None, str | None, int, float]:
-        """Used internally to wrap data, capture output and any exception."""
+        # Used internally to wrap data, capture output and any exception.
         stdout: str | None = None
         stderr: str | None = None
         exitcode: int
         timestamp: float
 
         try:
             stdout = _job.fun(*args, **kwargs)
@@ -604,17 +641,19 @@
 
         job.start_timestamp = time.time()
         job.inner_job = inner_job
 
     def _submit(self, job: Job, /) -> int:
         """Submits a job into the ppqueue.Queue system.
 
-        Throws an exception if:
-            1. the Queue uses a Thread job_runner and this data has a timeout (can't terminate Threads),
-            2. the Queue max_size will be exceeded after adding this job.
+        Args:
+            job: ...
+
+        Raises:
+            OverflowError: if max_size will be exceeded after adding this job.
 
         Returns:
             The number of jobs submitted to the queue.
         """
 
         assert not (self._engine is threading.Thread and job.timeout > 0)
 
@@ -657,22 +696,26 @@
         timeout: float = 0,
         suppress_errors: bool = False,
         skip_on_group_error: bool = False,
     ) -> int:
         """Adds a job to the queue.
 
         Args:
-            args:
-            kwargs:
-            name:
-            priority:
-            group:
-            timeout:
-            suppress_errors:
-            skip_on_group_error:
+            fun: ...
+            args: ...
+            kwargs: ...
+            name: ...
+            priority: ...
+            group: ...
+            timeout: ...
+            suppress_errors: ...
+            skip_on_group_error: ...
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
@@ -696,15 +739,24 @@
             suppress_errors=suppress_errors,
             skip_on_group_error=skip_on_group_error,
         )
 
         return self._submit(job)
 
     def put(self, *args, **kwargs) -> int:
-        """Alias for `enqueue`. Adds a job to the queue.
+        """Alias for `enqueue`.
+
+        Adds a job to the queue.
+
+        Args:
+            *args: ...
+            **kwargs: ...
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
@@ -728,18 +780,23 @@
         timeout: float = 0,
         show_progress: bool | None = None,
         **kwargs: Any,
     ) -> list[Job]:
         """Submits many jobs to the queue -- one for each item in the iterable. Waits for all to finish, then returns the results.
 
         Args:
-            fun:
-            iterable:
-            timeout:
-            show_progress:
+            fun: ...
+            iterable: ...
+            *args: ...
+            timeout: ...
+            show_progress: ...
+            **kwargs: ...
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             >>> from time import sleep
             ...
             >>> with Queue() as queue:
             ...     jobs = queue.map(sleep, [1, 2, 3, 4, 5])
@@ -767,18 +824,23 @@
         timeout: float = 0,
         show_progress: bool | None = None,
         **kwargs: Any,
     ) -> list[Job]:
         """Submits many jobs to the queue -- one for each sequence in the iterable. Waits for all to finish, then returns the results.
 
         Args:
-            fun:
-            iterable:
-            timeout:
-            show_progress:
+            fun: ...
+            iterable: ...
+            *args: static arguments passed to the function.
+            timeout: ...
+            show_progress: ...
+            **kwargs: static keyword-arguments passed to the function.
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
@@ -810,18 +872,23 @@
         timeout: float = 0,
         show_progress: bool | None = None,
         **kwargs: Any,
     ) -> list[Job]:
         """Submits many jobs to the queue -- one for each dictionary in the iterable. Waits for all to finish, then returns the results.
 
         Args:
-            fun:
-            iterable:
-            timeout:
-            show_progress:
+            fun: ...
+            iterable: ...
+            *args: static arguments passed to the function.
+            timeout: ...
+            show_progress: ...
+            **kwargs: static keyword-arguments passed to the function.
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             >>> from time import sleep
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
@@ -848,20 +915,23 @@
     def dequeue(
         self,
         *,
         wait: bool = False,
         _peek: bool = False,
         **kwargs: Any,
     ) -> Job | None:
-        """Removes and returns the job with the highest priority from the queue.
+        """Removes and returns the finished job with the highest priority from the queue.
 
         Args:
-            wait:
+            wait: if no jobs are finished, wait for one.
             **kwargs: passed to `Queue.wait`
 
+        Returns:
+            ...
+
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
             >>> with Queue() as queue:
@@ -887,15 +957,22 @@
         else:
             job = heappop(self._finished_queue)
             self._count_output += 1
 
         return job
 
     def pop(self, *args: Any, **kwargs: Any) -> Job | None:
-        """Alias for `dequeue`. Removes and returns the job with the highest priority from the queue.
+        """Alias for `dequeue`.
+
+        Args:
+            *args: ...
+            **kwargs: ...
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
@@ -907,19 +984,24 @@
             ...
             >>> [job.result for job in jobs]
             [100, 101, 102, 103, 104]
         """
         return self.dequeue(*args, **kwargs)
 
     def peek(self, *args: Any, **kwargs: Any) -> Job | None:
-        """Returns the job with the highest priority from the queue. Similar to `enqueue` / `pop`, but the job remains in the queue.
+        """Returns the job with the highest priority from the queue.
+
+        Similar to `dequeue` / `pop`, but the job remains in the queue.
 
         Args:
-            *args:
-            **kwargs:
+            *args: ...
+            **kwargs: ...
+
+        Returns:
+            ...
 
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
@@ -944,14 +1026,17 @@
         """Removes and returns all finished jobs from the queue.
 
         Args:
             n: collect this many jobs (default=0, all)
             wait: If True, block until this many jobs are finished. Else, immediately return all finished.
             **kwargs: kwargs given to `Queue.wait`.
 
+        Returns:
+            a list of `Job` instances.
+
         Examples:
             >>> from ppqueue import Queue
             ...
             >>> def add_nums(x: int, y: int) -> int:
             ...     return x + y
             ...
             >>> with Queue() as queue:
```

### Comparing `ppqueue-0.3.0/src/ppqueue/utils.py` & `ppqueue-0.4.0/src/ppqueue/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,15 @@
 from __future__ import annotations
 
 import logging
 import os
-from typing import List, Optional, TypeVar, Union
+from typing import List, Optional, TypeVar
 
 
 def get_logger(name: str, level: Optional[int] = None) -> logging.Logger:
-    """get or create a logger.
-
-    Args:
-        name (str)
-        level (Optional[int]): Defaults to logging.DEBUG.
-
-    Returns:
-        logging.Logger
-    """
     logger = logging.getLogger(name)
 
     logger.setLevel(logging.INFO if level is None else level)
     logger.propagate = False
 
     log_handler = logging.StreamHandler()
     log_handler.setFormatter(
@@ -29,26 +20,25 @@
     return logger
 
 
 def is_windows_os() -> bool:
     return os.name == "nt"
 
 
-def compare(num1: Union[int, float], num2: Union[int, float]) -> int:
-    """compare two numbers.
+def compare(num1: int | float, num2: int | float) -> int:
+    """Compare two numbers.
 
     Args:
-        num1 (Union[int, float]): the reference number.
-        num2 (Union[int, float]): the comparison number.
+        num1: the reference number.
+        num2: the comparison number.
 
     Returns:
-        int:
-            * 0  if num1 == num2
-            * 1  if num1 > num2
-            * -1 if num1 < num2
+        0  if num1 == num2
+        1  if num1 > num2
+        -1 if num1 < num2
     """
     if num1 == num2:
         return 0
 
     diff = (num1 if num1 else 0) - (num2 if num2 else 0)
 
     if diff == 0:
@@ -58,29 +48,28 @@
         return max(1, int(diff))
 
     # if diff < 0:
     return min(-1, int(diff))
 
 
 def compare_by(object1: object, object2: object, by: List[str], _state: int = 0) -> int:
-    """compare two objects by a list of attributes.
-    attributes are compared iteratively and the comparison will
+    """Compare two objects by a list of attributes.
+
+    Attributes are compared iteratively and the comparison will
     short-circuit when/if the objects are determined unequal.
 
     Args:
-        _state:
-        object1 (object): the reference object.
-        object2 (object): the comparison object.
-        by (List[str]): list of attributes to compare.
+        object1: the reference object.
+        object2: the comparison object.
+        by: list of attributes to compare.
 
     Returns:
-        int:
-            * 0  if object1 == object2
-            * 1  if object1 > object2
-            * -1 if object1 < object2
+        0  if object1 == object2
+        1  if object1 > object2
+        -1 if object1 < object2
     """
     if _state and _state >= len(by):
         # if we've compared all attributes,
         # these objects are considered equal.
         return 0
 
     diff: int = compare(getattr(object1, by[_state]), getattr(object2, by[_state]))
```

### Comparing `ppqueue-0.3.0/src/ppqueue.egg-info/SOURCES.txt` & `ppqueue-0.4.0/src/ppqueue.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+README.pypi.md
 pyproject.toml
 src/ppqueue/__init__.py
 src/ppqueue/__version__.py
 src/ppqueue/exceptions.py
 src/ppqueue/job.py
 src/ppqueue/plot.py
 src/ppqueue/py.typed
```

### Comparing `ppqueue-0.3.0/src/ppqueue.egg-info/requires.txt` & `ppqueue-0.4.0/src/ppqueue.egg-info/requires.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 [:python_version < "3.10"]
 typing-extensions
 
 [dev]
 python-lsp-server[rope]==1.*
 pylint==2.*
 pylint-pytest==1.*
-mypy[reports]==0.*
+mypy[reports]==1.*
 ruff==0.*
 black[jupyter]==23.*
 isort==5.*
 bump2version==1.*
 pdbpp
 ipykernel
 ipywidgets
```

### Comparing `ppqueue-0.3.0/tests/test_plot.py` & `ppqueue-0.4.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `ppqueue-0.3.0/tests/test_queue_processes.py` & `ppqueue-0.4.0/tests/test_queue_processes.py`

 * *Files identical despite different names*

### Comparing `ppqueue-0.3.0/tests/test_queue_threads.py` & `ppqueue-0.4.0/tests/test_queue_threads.py`

 * *Files identical despite different names*

### Comparing `ppqueue-0.3.0/tests/test_utils.py` & `ppqueue-0.4.0/tests/test_utils.py`

 * *Files identical despite different names*

