# Comparing `tmp/parallelism-0.1.1.tar.gz` & `tmp/parallelism-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallelism-0.1.1.tar", last modified: Sat Aug  5 12:40:01 2023, max compression
+gzip compressed data, was "parallelism-0.1.2.tar", last modified: Sat Aug  5 13:32:31 2023, max compression
```

## Comparing `parallelism-0.1.1.tar` & `parallelism-0.1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.874193 parallelism-0.1.1/
--rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.1/.gitignore
--rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.1/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      674 2023-08-05 12:40:01.874193 parallelism-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.671082 parallelism-0.1.1/docs/
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.686703 parallelism-0.1.1/docs/api_reference/
--rw-rw-rw-   0        0        0     6550 2023-08-04 23:52:47.000000 parallelism-0.1.1/docs/api_reference/scheduled_task.rst
--rw-rw-rw-   0        0        0     9746 2023-08-05 12:39:04.000000 parallelism-0.1.1/docs/api_reference/task_scheduler.rst
--rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.1/docs/conf.py
--rw-rw-rw-   0        0        0      986 2023-08-04 09:49:41.000000 parallelism-0.1.1/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.717945 parallelism-0.1.1/parallelism/
--rw-rw-rw-   0        0        0      296 2023-08-05 12:39:19.000000 parallelism-0.1.1/parallelism/__init__.py
--rw-rw-rw-   0        0        0     8668 2023-08-04 22:27:47.000000 parallelism-0.1.1/parallelism/api_reference.py
--rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.1/parallelism/config.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.796064 parallelism-0.1.1/parallelism/core/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.1/parallelism/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.811698 parallelism-0.1.1/parallelism/core/exceptions/
--rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.1/parallelism/core/exceptions/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.1/parallelism/core/exceptions/dependency_error.py
--rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.1/parallelism/core/exceptions/worker_error.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.827296 parallelism-0.1.1/parallelism/core/executors/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.1/parallelism/core/executors/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.1/parallelism/core/executors/process_executor.py
--rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.1/parallelism/core/executors/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.874193 parallelism-0.1.1/parallelism/core/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.1/parallelism/core/handlers/__init__.py
--rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.1/parallelism/core/handlers/dependency_handler.py
--rw-rw-rw-   0        0        0     7063 2023-08-05 00:35:04.000000 parallelism-0.1.1/parallelism/core/handlers/function_handler.py
--rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.1/parallelism/core/handlers/parameters_handler.py
--rw-rw-rw-   0        0        0     3778 2023-08-05 00:37:16.000000 parallelism-0.1.1/parallelism/core/handlers/shared_memory_handler.py
--rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.1/parallelism/core/raise_exception.py
--rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.1/parallelism/core/return_value.py
--rw-rw-rw-   0        0        0     3182 2023-08-02 21:46:54.000000 parallelism-0.1.1/parallelism/core/scheduled_task.py
--rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.1/parallelism/core/scheduler_result.py
--rw-rw-rw-   0        0        0     7203 2023-08-04 11:48:06.000000 parallelism-0.1.1/parallelism/core/task_scheduler.py
--rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.1/parallelism/logger.py
-drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.733566 parallelism-0.1.1/parallelism.egg-info/
--rw-rw-rw-   0        0        0      674 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 12:40:01.874193 parallelism-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.103814 parallelism-0.1.2/
+-rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.2/.gitignore
+-rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.2/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2710 2023-08-05 13:32:31.103814 parallelism-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2090 2023-08-05 13:30:29.000000 parallelism-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:30.963221 parallelism-0.1.2/docs/
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:30.978841 parallelism-0.1.2/docs/api_reference/
+-rw-rw-rw-   0        0        0     6550 2023-08-04 23:52:47.000000 parallelism-0.1.2/docs/api_reference/scheduled_task.rst
+-rw-rw-rw-   0        0        0     9746 2023-08-05 12:39:04.000000 parallelism-0.1.2/docs/api_reference/task_scheduler.rst
+-rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.2/docs/conf.py
+-rw-rw-rw-   0        0        0     1367 2023-08-05 13:30:29.000000 parallelism-0.1.2/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:30.994462 parallelism-0.1.2/parallelism/
+-rw-rw-rw-   0        0        0      296 2023-08-05 13:31:54.000000 parallelism-0.1.2/parallelism/__init__.py
+-rw-rw-rw-   0        0        0     8668 2023-08-04 22:27:47.000000 parallelism-0.1.2/parallelism/api_reference.py
+-rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.2/parallelism/config.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.041340 parallelism-0.1.2/parallelism/core/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.2/parallelism/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.056983 parallelism-0.1.2/parallelism/core/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.2/parallelism/core/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.2/parallelism/core/exceptions/dependency_error.py
+-rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.2/parallelism/core/exceptions/worker_error.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.072570 parallelism-0.1.2/parallelism/core/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.2/parallelism/core/executors/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.2/parallelism/core/executors/process_executor.py
+-rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.2/parallelism/core/executors/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.103814 parallelism-0.1.2/parallelism/core/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.2/parallelism/core/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.2/parallelism/core/handlers/dependency_handler.py
+-rw-rw-rw-   0        0        0     7063 2023-08-05 00:35:04.000000 parallelism-0.1.2/parallelism/core/handlers/function_handler.py
+-rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.2/parallelism/core/handlers/parameters_handler.py
+-rw-rw-rw-   0        0        0     3778 2023-08-05 00:37:16.000000 parallelism-0.1.2/parallelism/core/handlers/shared_memory_handler.py
+-rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.2/parallelism/core/raise_exception.py
+-rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.2/parallelism/core/return_value.py
+-rw-rw-rw-   0        0        0     3182 2023-08-02 21:46:54.000000 parallelism-0.1.2/parallelism/core/scheduled_task.py
+-rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.2/parallelism/core/scheduler_result.py
+-rw-rw-rw-   0        0        0     7203 2023-08-04 11:48:06.000000 parallelism-0.1.2/parallelism/core/task_scheduler.py
+-rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.2/parallelism/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-05 13:32:31.010088 parallelism-0.1.2/parallelism.egg-info/
+-rw-rw-rw-   0        0        0     2710 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-05 13:32:30.000000 parallelism-0.1.2/parallelism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 13:32:31.103814 parallelism-0.1.2/setup.cfg
```

### Comparing `parallelism-0.1.1/.gitignore` & `parallelism-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/LICENSE` & `parallelism-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/docs/api_reference/scheduled_task.rst` & `parallelism-0.1.2/docs/api_reference/scheduled_task.rst`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/docs/api_reference/task_scheduler.rst` & `parallelism-0.1.2/docs/api_reference/task_scheduler.rst`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/api_reference.py` & `parallelism-0.1.2/parallelism/api_reference.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/executors/process_executor.py` & `parallelism-0.1.2/parallelism/core/executors/process_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/executors/thread_executor.py` & `parallelism-0.1.2/parallelism/core/executors/thread_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/handlers/dependency_handler.py` & `parallelism-0.1.2/parallelism/core/handlers/dependency_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/handlers/function_handler.py` & `parallelism-0.1.2/parallelism/core/handlers/function_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/handlers/parameters_handler.py` & `parallelism-0.1.2/parallelism/core/handlers/parameters_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/handlers/shared_memory_handler.py` & `parallelism-0.1.2/parallelism/core/handlers/shared_memory_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/return_value.py` & `parallelism-0.1.2/parallelism/core/return_value.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/scheduled_task.py` & `parallelism-0.1.2/parallelism/core/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism/core/task_scheduler.py` & `parallelism-0.1.2/parallelism/core/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/parallelism.egg-info/SOURCES.txt` & `parallelism-0.1.2/parallelism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.1/pyproject.toml` & `parallelism-0.1.2/pyproject.toml`

 * *Files identical despite different names*

