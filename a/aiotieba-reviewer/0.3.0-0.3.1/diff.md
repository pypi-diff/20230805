# Comparing `tmp/aiotieba-reviewer-0.3.0.tar.gz` & `tmp/aiotieba-reviewer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotieba-reviewer-0.3.0.tar", last modified: Fri Jul 28 13:33:56 2023, max compression
+gzip compressed data, was "aiotieba-reviewer-0.3.1.tar", last modified: Sat Aug  5 10:50:41 2023, max compression
```

## Comparing `aiotieba-reviewer-0.3.0.tar` & `aiotieba-reviewer-0.3.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2451 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30242 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/perf_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/punish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.760664 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/user_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.756664 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-28 13:33:56.000000 aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    24429 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/examples/cmd_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/examples/reviewer_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-28 13:33:36.000000 aiotieba-reviewer-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 13:33:56.764664 aiotieba-reviewer-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.785951 aiotieba-reviewer-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.777951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30524 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/perf_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/punish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.777951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.777951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comment/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comment/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5338 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/post/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/post/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/thread/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/thread/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/user_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.777951 aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-08-05 10:50:41.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-08-05 10:50:41.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:50:41.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-08-05 10:50:41.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 10:50:41.000000 aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:50:41.781951 aiotieba-reviewer-0.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    24485 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/examples/cmd_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/examples/reviewer_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-08-05 10:50:21.000000 aiotieba-reviewer-0.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:50:41.785951 aiotieba-reviewer-0.3.1/setup.cfg
```

### Comparing `aiotieba-reviewer-0.3.0/LICENSE` & `aiotieba-reviewer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/PKG-INFO` & `aiotieba-reviewer-0.3.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotieba-reviewer
-Version: 0.3.0
+Version: 0.3.1
 Summary: Reviewer Framework based on aiotieba
 Author-email: Starry-OvO <starry.qvq@gmail.com>
 Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
 Project-URL: Documentation, https://review.aiotieba.cc/
 Keywords: baidu,tieba
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -64,25 +64,27 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.07.28更新*
+*2023.08.05更新*
 
-|      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
-| :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 5,158,566  |     1,494,989      |    3,015     |   89,066   |
-|     孙笑川     | 4,370,625  |      601,586       |    4,686     |  189,109   |
-|    原神内鬼    |  613,663   |      408,731       |     765      |   30,952   |
-|      憨批      |   34,574   |      157,889       |    3,902     |   60,238   |
-|    lol半价     | 2,089,892  |       82,061       |     335      |   19,828   |
-|     vtuber     |  226,724   |       12,474       |      79      |   1,063    |
-|    天堂鸡汤    |  372,240   |       10,919       |      77      |   2,326    |
-| vtuber自由讨论 |   17,265   |        994         |      0       |     4      |
+|   吧id   | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
+| :------: | :--------: | :----------------: | :----------: | :--------: |
+| 17019292 | 5,167,171  |     1,406,394      |    2,846     |   87,392   |
+| 21841105 | 4,411,438  |      605,505       |    4,782     |  195,734   |
+| 27497591 |  616,895   |      410,480       |     748      |   31,556   |
+| 13971645 |   36,140   |      167,399       |    4,107     |   64,536   |
+|  414639  | 2,090,330  |       85,129       |     359      |   17,765   |
+| 27400819 |  822,599   |       29,943       |     210      |   11,866   |
+| 19862444 |   69,227   |       27,338       |     113      |   4,044    |
+| 26066262 |  226,854   |       12,665       |      80      |   1,066    |
+| 27782931 |  373,284   |       11,183       |      72      |   2,421    |
+| 24850810 |  277,647   |       8,256        |     117      |   1,072    |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.3.0/README.md` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,90 @@
-## 简介
-
-基于[**aiotieba**](https://github.com/Starry-OvO/aiotieba)实现的百度贴吧高弹性吧务审查框架
-
-+ 类型注解全覆盖，方法注释全覆盖，类属性注释全覆盖，内部命名统一
-+ 支持获取用户主页信息（包括个性签名、发帖量、吧龄、成长等级、ip归属地、虚拟形象信息...）、历史发帖、关注吧、关注用户、粉丝列表...
-+ 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
-+ 支持针对多条相互关联的内容的审查
-+ 支持二维码识别、相似图像查找
-+ 支持用户黑白名单、图片黑白名单
-+ 使用本地缓存避免重复检测，极大提升性能
-+ 优先使用websocket接口，节省带宽
-
-## git安装 (更新较快)
-
-### 安装
-
-```shell
-git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
-cd ./aiotieba-reviewer
-pip install -e .
-```
-
-### 更新
-
-```shell
-git pull
-```
-
-## pip安装 (更新较慢)
-
-### 安装
-
-```shell
-pip install aiotieba-reviewer
-```
-
-### 更新
-
-```shell
-pip install -U aiotieba-reviewer
-```
-
-## 教程
-
-[**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
-
-## 客户名单
-
-*2023.07.28更新*
-
-|      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
-| :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 5,158,566  |     1,494,989      |    3,015     |   89,066   |
-|     孙笑川     | 4,370,625  |      601,586       |    4,686     |  189,109   |
-|    原神内鬼    |  613,663   |      408,731       |     765      |   30,952   |
-|      憨批      |   34,574   |      157,889       |    3,902     |   60,238   |
-|    lol半价     | 2,089,892  |       82,061       |     335      |   19,828   |
-|     vtuber     |  226,724   |       12,474       |      79      |   1,063    |
-|    天堂鸡汤    |  372,240   |       10,919       |      77      |   2,326    |
-| vtuber自由讨论 |   17,265   |        994         |      0       |     4      |
-
-## 友情链接
-
-+ [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
-+ [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
-+ [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
+Metadata-Version: 2.1
+Name: aiotieba-reviewer
+Version: 0.3.1
+Summary: Reviewer Framework based on aiotieba
+Author-email: Starry-OvO <starry.qvq@gmail.com>
+Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
+Project-URL: Documentation, https://review.aiotieba.cc/
+Keywords: baidu,tieba
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Internet :: WWW/HTTP :: Session
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+## 简介
+
+基于[**aiotieba**](https://github.com/Starry-OvO/aiotieba)实现的百度贴吧高弹性吧务审查框架
+
++ 类型注解全覆盖，方法注释全覆盖，类属性注释全覆盖，内部命名统一
++ 支持获取用户主页信息（包括个性签名、发帖量、吧龄、成长等级、ip归属地、虚拟形象信息...）、历史发帖、关注吧、关注用户、粉丝列表...
++ 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
++ 支持针对多条相互关联的内容的审查
++ 支持二维码识别、相似图像查找
++ 支持用户黑白名单、图片黑白名单
++ 使用本地缓存避免重复检测，极大提升性能
++ 优先使用websocket接口，节省带宽
+
+## git安装 (更新较快)
+
+### 安装
+
+```shell
+git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
+cd ./aiotieba-reviewer
+pip install -e .
+```
+
+### 更新
+
+```shell
+git pull
+```
+
+## pip安装 (更新较慢)
+
+### 安装
+
+```shell
+pip install aiotieba-reviewer
+```
+
+### 更新
+
+```shell
+pip install -U aiotieba-reviewer
+```
+
+## 教程
+
+[**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
+
+## 客户名单
+
+*2023.08.05更新*
+
+|   吧id   | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
+| :------: | :--------: | :----------------: | :----------: | :--------: |
+| 17019292 | 5,167,171  |     1,406,394      |    2,846     |   87,392   |
+| 21841105 | 4,411,438  |      605,505       |    4,782     |  195,734   |
+| 27497591 |  616,895   |      410,480       |     748      |   31,556   |
+| 13971645 |   36,140   |      167,399       |    4,107     |   64,536   |
+|  414639  | 2,090,330  |       85,129       |     359      |   17,765   |
+| 27400819 |  822,599   |       29,943       |     210      |   11,866   |
+| 19862444 |   69,227   |       27,338       |     113      |   4,044    |
+| 26066262 |  226,854   |       12,665       |      80      |   1,066    |
+| 27782931 |  373,284   |       11,183       |      72      |   2,421    |
+| 24850810 |  277,647   |       8,256        |     117      |   1,072    |
+
+## 友情链接
+
++ [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
++ [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
++ [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/client.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/database.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import asyncio
 import datetime
 import sqlite3
+import ssl
 from pathlib import Path
 from typing import Any, Callable, Final, List, Optional, Tuple, Union
 
 import aiomysql
 from aiotieba.config import CONFIG
 from aiotieba.logging import get_logger as LOG
 from aiotieba.typing import UserInfo
@@ -80,26 +81,33 @@
 
     async def _create_pool(self) -> None:
         """
         创建连接池
         """
 
         db_config = CONFIG.get('Database', {})
+
+        ssl_ctx = None
+        if cafile := db_config.get('ssl_cafile'):
+            ssl_ctx = ssl.SSLContext(ssl.PROTOCOL_TLS_CLIENT)
+            ssl_ctx.load_verify_locations(cafile=cafile)
+
         self._pool: aiomysql.Pool = await aiomysql.create_pool(
             user=db_config['user'],
             password=db_config['password'],
             db=db_config.get('db', self._default_db_name),
             minsize=db_config.get('minsize', self._default_minsize),
             maxsize=db_config.get('maxsize', self._default_maxsize),
             pool_recycle=db_config.get('pool_recycle', self._default_pool_recycle),
             loop=asyncio.get_running_loop(),
             autocommit=True,
             host=db_config.get('host', 'localhost'),
             port=db_config.get('port', self._default_port),
             unix_socket=db_config.get('unix_socket'),
+            ssl=ssl_ctx,
         )
 
     async def create_database(self) -> bool:
         """
         创建并初始化数据库
 
         Returns:
@@ -113,14 +121,15 @@
                 host=db_config.get('host', 'localhost'),
                 port=db_config.get('port', self._default_port),
                 user=db_config['user'],
                 password=db_config['password'],
                 unix_socket=db_config.get('unix_socket'),
                 autocommit=True,
                 loop=asyncio.get_running_loop(),
+                ssl=self._pool._conn_kwargs['ssl'],
             )
 
             async with conn.cursor() as cursor:
                 db_name = db_config.get('db', self._default_db_name)
                 await cursor.execute(f"CREATE DATABASE IF NOT EXISTS `{db_name}`")
 
             await self._create_pool()
```

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/executor.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/executor.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/imgproc.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/imgproc.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/perf_stat.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/perf_stat.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/punish.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/punish.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/checker.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comment/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comment/runner.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comment/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/producer.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/comments/runner.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/comments/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/entry.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/entry.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/checker.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/post/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/post/runner.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/post/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/producer.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/posts/runner.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/posts/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/checker.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/thread/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/thread/runner.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/thread/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/producer.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/threads/runner.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/threads/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer/reviewer/user_checker.py` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer/reviewer/user_checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/PKG-INFO` & `aiotieba-reviewer-0.3.1/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,69 @@
-Metadata-Version: 2.1
-Name: aiotieba-reviewer
-Version: 0.3.0
-Summary: Reviewer Framework based on aiotieba
-Author-email: Starry-OvO <starry.qvq@gmail.com>
-Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
-Project-URL: Documentation, https://review.aiotieba.cc/
-Keywords: baidu,tieba
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Topic :: Internet :: WWW/HTTP :: Session
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-## 简介
-
-基于[**aiotieba**](https://github.com/Starry-OvO/aiotieba)实现的百度贴吧高弹性吧务审查框架
-
-+ 类型注解全覆盖，方法注释全覆盖，类属性注释全覆盖，内部命名统一
-+ 支持获取用户主页信息（包括个性签名、发帖量、吧龄、成长等级、ip归属地、虚拟形象信息...）、历史发帖、关注吧、关注用户、粉丝列表...
-+ 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
-+ 支持针对多条相互关联的内容的审查
-+ 支持二维码识别、相似图像查找
-+ 支持用户黑白名单、图片黑白名单
-+ 使用本地缓存避免重复检测，极大提升性能
-+ 优先使用websocket接口，节省带宽
-
-## git安装 (更新较快)
-
-### 安装
-
-```shell
-git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
-cd ./aiotieba-reviewer
-pip install -e .
-```
-
-### 更新
-
-```shell
-git pull
-```
-
-## pip安装 (更新较慢)
-
-### 安装
-
-```shell
-pip install aiotieba-reviewer
-```
-
-### 更新
-
-```shell
-pip install -U aiotieba-reviewer
-```
-
-## 教程
-
-[**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
-
-## 客户名单
-
-*2023.07.28更新*
-
-|      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
-| :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 5,158,566  |     1,494,989      |    3,015     |   89,066   |
-|     孙笑川     | 4,370,625  |      601,586       |    4,686     |  189,109   |
-|    原神内鬼    |  613,663   |      408,731       |     765      |   30,952   |
-|      憨批      |   34,574   |      157,889       |    3,902     |   60,238   |
-|    lol半价     | 2,089,892  |       82,061       |     335      |   19,828   |
-|     vtuber     |  226,724   |       12,474       |      79      |   1,063    |
-|    天堂鸡汤    |  372,240   |       10,919       |      77      |   2,326    |
-| vtuber自由讨论 |   17,265   |        994         |      0       |     4      |
-
-## 友情链接
-
-+ [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
-+ [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
-+ [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
+## 简介
+
+基于[**aiotieba**](https://github.com/Starry-OvO/aiotieba)实现的百度贴吧高弹性吧务审查框架
+
++ 类型注解全覆盖，方法注释全覆盖，类属性注释全覆盖，内部命名统一
++ 支持获取用户主页信息（包括个性签名、发帖量、吧龄、成长等级、ip归属地、虚拟形象信息...）、历史发帖、关注吧、关注用户、粉丝列表...
++ 支持富文本解析，获取图片信息、at用户id、链接内容、投票帖、转发帖...
++ 支持针对多条相互关联的内容的审查
++ 支持二维码识别、相似图像查找
++ 支持用户黑白名单、图片黑白名单
++ 使用本地缓存避免重复检测，极大提升性能
++ 优先使用websocket接口，节省带宽
+
+## git安装 (更新较快)
+
+### 安装
+
+```shell
+git clone https://github.com/Starry-OvO/aiotieba-reviewer.git --depth=1 -b develop
+cd ./aiotieba-reviewer
+pip install -e .
+```
+
+### 更新
+
+```shell
+git pull
+```
+
+## pip安装 (更新较慢)
+
+### 安装
+
+```shell
+pip install aiotieba-reviewer
+```
+
+### 更新
+
+```shell
+pip install -U aiotieba-reviewer
+```
+
+## 教程
+
+[**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
+
+## 客户名单
+
+*2023.08.05更新*
+
+|   吧id   | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
+| :------: | :--------: | :----------------: | :----------: | :--------: |
+| 17019292 | 5,167,171  |     1,406,394      |    2,846     |   87,392   |
+| 21841105 | 4,411,438  |      605,505       |    4,782     |  195,734   |
+| 27497591 |  616,895   |      410,480       |     748      |   31,556   |
+| 13971645 |   36,140   |      167,399       |    4,107     |   64,536   |
+|  414639  | 2,090,330  |       85,129       |     359      |   17,765   |
+| 27400819 |  822,599   |       29,943       |     210      |   11,866   |
+| 19862444 |   69,227   |       27,338       |     113      |   4,044    |
+| 26066262 |  226,854   |       12,665       |      80      |   1,066    |
+| 27782931 |  373,284   |       11,183       |      72      |   2,421    |
+| 24850810 |  277,647   |       8,256        |     117      |   1,072    |
+
+## 友情链接
+
++ [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
++ [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
++ [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.3.0/aiotieba_reviewer.egg-info/SOURCES.txt` & `aiotieba-reviewer-0.3.1/aiotieba_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/examples/cmd_handler.py` & `aiotieba-reviewer-0.3.1/examples/cmd_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -637,14 +637,16 @@
 
         for pn in range(1, 0xFFFF):
             threads = await ctx.admin.get_user_threads(user_id, pn)
             for thread in threads:
                 if thread.fname != ctx.fname:
                     continue
                 await ctx.admin.del_post(thread.fid, thread.tid, thread.pid)
+            if len(threads) < 60:
+                break
 
     @check_and_log(need_permission=4, need_arg_num=2)
     async def cmd_set(self, ctx: Context) -> None:
         """
         set指令
         设置用户的权限级别
         """
```

### Comparing `aiotieba-reviewer-0.3.0/examples/reviewer_example.py` & `aiotieba-reviewer-0.3.1/examples/reviewer_example.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.3.0/pyproject.toml` & `aiotieba-reviewer-0.3.1/pyproject.toml`

 * *Files identical despite different names*

