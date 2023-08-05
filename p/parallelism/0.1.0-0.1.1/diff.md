# Comparing `tmp/parallelism-0.1.0.tar.gz` & `tmp/parallelism-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parallelism-0.1.0.tar", last modified: Fri Aug  4 11:50:36 2023, max compression
+gzip compressed data, was "parallelism-0.1.1.tar", last modified: Sat Aug  5 12:40:01 2023, max compression
```

## Comparing `parallelism-0.1.0.tar` & `parallelism-0.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.365749 parallelism-0.1.0/
--rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.0/.gitignore
--rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.0/.readthedocs.yaml
--rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      674 2023-08-04 11:50:36.365749 parallelism-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.218892 parallelism-0.1.0/docs/
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.218892 parallelism-0.1.0/docs/api_reference/
--rw-rw-rw-   0        0        0     5083 2023-08-04 11:42:22.000000 parallelism-0.1.0/docs/api_reference/scheduled_task.rst
--rw-rw-rw-   0        0        0     2945 2023-08-04 11:46:52.000000 parallelism-0.1.0/docs/api_reference/task_scheduler.rst
--rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.0/docs/conf.py
--rw-rw-rw-   0        0        0      986 2023-08-04 09:49:41.000000 parallelism-0.1.0/docs/index.rst
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.250131 parallelism-0.1.0/parallelism/
--rw-rw-rw-   0        0        0      296 2023-08-04 11:48:06.000000 parallelism-0.1.0/parallelism/__init__.py
--rw-rw-rw-   0        0        0     7143 2023-08-04 09:28:23.000000 parallelism-0.1.0/parallelism/api_reference.py
--rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.0/parallelism/config.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.281373 parallelism-0.1.0/parallelism/core/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.0/parallelism/core/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.296994 parallelism-0.1.0/parallelism/core/exceptions/
--rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.0/parallelism/core/exceptions/__init__.py
--rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.0/parallelism/core/exceptions/dependency_error.py
--rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.0/parallelism/core/exceptions/worker_error.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.328238 parallelism-0.1.0/parallelism/core/executors/
--rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.0/parallelism/core/executors/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.0/parallelism/core/executors/process_executor.py
--rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.0/parallelism/core/executors/thread_executor.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.365749 parallelism-0.1.0/parallelism/core/handlers/
--rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.0/parallelism/core/handlers/__init__.py
--rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.0/parallelism/core/handlers/dependency_handler.py
--rw-rw-rw-   0        0        0     6993 2023-08-04 11:46:52.000000 parallelism-0.1.0/parallelism/core/handlers/function_handler.py
--rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.0/parallelism/core/handlers/parameters_handler.py
--rw-rw-rw-   0        0        0     3754 2023-08-04 11:46:52.000000 parallelism-0.1.0/parallelism/core/handlers/shared_memory_handler.py
--rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.0/parallelism/core/raise_exception.py
--rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.0/parallelism/core/return_value.py
--rw-rw-rw-   0        0        0     3182 2023-08-02 21:46:54.000000 parallelism-0.1.0/parallelism/core/scheduled_task.py
--rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.0/parallelism/core/scheduler_result.py
--rw-rw-rw-   0        0        0     7203 2023-08-04 11:48:06.000000 parallelism-0.1.0/parallelism/core/task_scheduler.py
--rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.0/parallelism/logger.py
-drwxrwxrwx   0        0        0        0 2023-08-04 11:50:36.265756 parallelism-0.1.0/parallelism.egg-info/
--rw-rw-rw-   0        0        0      674 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1102 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 11:50:36.000000 parallelism-0.1.0/parallelism.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-04 11:50:36.365749 parallelism-0.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.874193 parallelism-0.1.1/
+-rw-rw-rw-   0        0        0     3238 2023-07-28 18:24:12.000000 parallelism-0.1.1/.gitignore
+-rw-rw-rw-   0        0        0      115 2023-07-29 07:17:10.000000 parallelism-0.1.1/.readthedocs.yaml
+-rw-rw-rw-   0        0        0     1088 2023-07-28 18:24:12.000000 parallelism-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      674 2023-08-05 12:40:01.874193 parallelism-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       54 2023-07-28 18:24:12.000000 parallelism-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.671082 parallelism-0.1.1/docs/
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.686703 parallelism-0.1.1/docs/api_reference/
+-rw-rw-rw-   0        0        0     6550 2023-08-04 23:52:47.000000 parallelism-0.1.1/docs/api_reference/scheduled_task.rst
+-rw-rw-rw-   0        0        0     9746 2023-08-05 12:39:04.000000 parallelism-0.1.1/docs/api_reference/task_scheduler.rst
+-rw-rw-rw-   0        0        0      341 2023-07-29 11:22:19.000000 parallelism-0.1.1/docs/conf.py
+-rw-rw-rw-   0        0        0      986 2023-08-04 09:49:41.000000 parallelism-0.1.1/docs/index.rst
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.717945 parallelism-0.1.1/parallelism/
+-rw-rw-rw-   0        0        0      296 2023-08-05 12:39:19.000000 parallelism-0.1.1/parallelism/__init__.py
+-rw-rw-rw-   0        0        0     8668 2023-08-04 22:27:47.000000 parallelism-0.1.1/parallelism/api_reference.py
+-rw-rw-rw-   0        0        0      395 2023-07-17 16:01:03.000000 parallelism-0.1.1/parallelism/config.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.796064 parallelism-0.1.1/parallelism/core/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:22:05.000000 parallelism-0.1.1/parallelism/core/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.811698 parallelism-0.1.1/parallelism/core/exceptions/
+-rw-rw-rw-   0        0        0        0 2023-07-14 23:41:33.000000 parallelism-0.1.1/parallelism/core/exceptions/__init__.py
+-rw-rw-rw-   0        0        0      369 2023-07-14 23:57:59.000000 parallelism-0.1.1/parallelism/core/exceptions/dependency_error.py
+-rw-rw-rw-   0        0        0      333 2023-07-28 10:57:43.000000 parallelism-0.1.1/parallelism/core/exceptions/worker_error.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.827296 parallelism-0.1.1/parallelism/core/executors/
+-rw-rw-rw-   0        0        0        0 2023-07-10 17:30:09.000000 parallelism-0.1.1/parallelism/core/executors/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-07-13 20:44:05.000000 parallelism-0.1.1/parallelism/core/executors/process_executor.py
+-rw-rw-rw-   0        0        0      890 2023-07-10 17:35:23.000000 parallelism-0.1.1/parallelism/core/executors/thread_executor.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.874193 parallelism-0.1.1/parallelism/core/handlers/
+-rw-rw-rw-   0        0        0        0 2023-07-13 20:15:30.000000 parallelism-0.1.1/parallelism/core/handlers/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-07-29 17:55:18.000000 parallelism-0.1.1/parallelism/core/handlers/dependency_handler.py
+-rw-rw-rw-   0        0        0     7063 2023-08-05 00:35:04.000000 parallelism-0.1.1/parallelism/core/handlers/function_handler.py
+-rw-rw-rw-   0        0        0     2124 2023-07-21 23:15:08.000000 parallelism-0.1.1/parallelism/core/handlers/parameters_handler.py
+-rw-rw-rw-   0        0        0     3778 2023-08-05 00:37:16.000000 parallelism-0.1.1/parallelism/core/handlers/shared_memory_handler.py
+-rw-rw-rw-   0        0        0      344 2023-08-04 11:42:19.000000 parallelism-0.1.1/parallelism/core/raise_exception.py
+-rw-rw-rw-   0        0        0     1275 2023-08-02 21:46:54.000000 parallelism-0.1.1/parallelism/core/return_value.py
+-rw-rw-rw-   0        0        0     3182 2023-08-02 21:46:54.000000 parallelism-0.1.1/parallelism/core/scheduled_task.py
+-rw-rw-rw-   0        0        0      474 2023-08-04 11:46:52.000000 parallelism-0.1.1/parallelism/core/scheduler_result.py
+-rw-rw-rw-   0        0        0     7203 2023-08-04 11:48:06.000000 parallelism-0.1.1/parallelism/core/task_scheduler.py
+-rw-rw-rw-   0        0        0      506 2023-07-14 10:52:01.000000 parallelism-0.1.1/parallelism/logger.py
+drwxrwxrwx   0        0        0        0 2023-08-05 12:40:01.733566 parallelism-0.1.1/parallelism.egg-info/
+-rw-rw-rw-   0        0        0      674 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1102 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-08-05 12:40:01.000000 parallelism-0.1.1/parallelism.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      851 2023-07-28 19:13:04.000000 parallelism-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 12:40:01.874193 parallelism-0.1.1/setup.cfg
```

### Comparing `parallelism-0.1.0/.gitignore` & `parallelism-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/LICENSE` & `parallelism-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/PKG-INFO` & `parallelism-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.1.0
+Version: 0.1.1
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.1.0/docs/api_reference/scheduled_task.rst` & `parallelism-0.1.1/docs/api_reference/scheduled_task.rst`

 * *Files 22% similar despite different names*

```diff
@@ -3,27 +3,28 @@
 
 .. autofunction:: parallelism.scheduled_task
 
 .. automodule:: parallelism.core.scheduled_task
 
    .. py:class:: ScheduledTask
 
-      A :py:obj:`collections.namedtuple` object representing a task
+      The `ScheduledTask` class, a subclass of `collections.namedtuple`, represents a scheduled task along with its associated return value.
+      This class provides a mechanism to access the return value of the task in a deferred manner using the `ReturnValue` object.
 
       .. py:property:: return_value
 
-         An object containing a reference to the return value of a task
+         A reference to the ReturnValue object associated with this scheduled task.
+         The `ReturnValue` object provides deferred access to the actual return value of the task.
 
 .. automodule:: parallelism.core.return_value
 
    .. py:class:: ReturnValue
 
-      This object implements
-      `__call__`, `__getattribute__` and `__getitem__`
-      to allow getting the desired value at runtime
+      The `ReturnValue` class represents a deferred reference to the return value of a scheduled task.
+      It implements the `__call__`, `__getattribute__`, and `__getitem__` methods to provide flexible access to the actual return value.
 
       .. code-block:: python
       
          from parallelism import scheduled_task
 
          def func1(reverse=False):
             return 54321 if reverse else 12345
@@ -38,141 +39,164 @@
             return [1, 2, 3, 4, 5]
 
          st1 = scheduled_task(executor=..., name='st1', target=func1, ...)
          st2 = scheduled_task(executor=..., name='st2', target=func2, ...)
          st3 = scheduled_task(executor=..., name='st3', target=func3, ...)
          st4 = scheduled_task(executor=..., name='st4', target=func4, ...)
 
+      Accessing a Return Value:
+
       >>> st1.return_value
       ReturnValue(task=ScheduledTask(executor=..., name='st1', target='__main__.func1', ...))
-
-      In this case, the return value will be `12345`
+      # At runtime: 12345
 
       .. py:method:: __call__(self, *args, **kwargs)
 
+         Invokes the `ReturnValue` object as a callable.
+         This method is used to retrieve the actual return value of the scheduled task.
+
+         Invoking the Return Value as a Callable:
+
          >>> st2.return_value()
          ReturnValue(task=ScheduledTask(executor=..., name='st2', target='__main__.func2', ...)))
+         # At runtime: 12345
 
-         In this case, the return value will be `12345`
+         Invoking the Return Value with Parameters:
 
          >>> st2.return_value(reverse=True)
          ReturnValue(task=ScheduledTask(executor=..., name='st2', target='__main__.func2', ...)))
-
-         In this case, the return value will be `54321`
+         # At runtime: 54321
 
       .. py:method:: __getattribute__(self, name)
 
+         Retrieves an attribute or method of the actual return value.
+         This method allows access to properties and methods of the return value without directly referencing it.
+
+         Accessing a Specific Key in the Return Dictionary:
+
          >>> st3.return_value.get('b')
          ReturnValue(task=ScheduledTask(executor=..., name='st3', target='__main__.func3', ...))
-
-         In this case, the return value will be `45`
+         # At runtime: 45
 
       .. py:method:: __getitem__(self, key)
 
+         Retrieves an item from the actual return value using the provided key.
+         This method allows accessing elements of the return value, such as lists, dictionaries, etc.
+
+         Accessing an Element by Index:
+
          >>> st4.return_value[2]
          ReturnValue(task=ScheduledTask(executor=..., name='st4', target='__main__.func4', ...)))
+         # At runtime: 3
 
-         In this case, the return value will be `3`
+         Accessing a Slice of Elements:
 
          >>> st4.return_value[3:]
          ReturnValue(task=ScheduledTask(executor=..., name='st4', target='__main__.func4', ...)))
-
-         In this case, the return value will be `45`
+         # At runtime: 45
 
 Examples
 --------
 
 .. code-block:: python
 
    # Built-in modules
    from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor
    from multiprocessing import Process
    from threading import Thread
    
    # Third-party packages
    from parallelism import scheduled_task
 
-Minimalistic
-************
+Executor
+********
 
-An example of basic usage for creating a `ScheduledTask` instances:
+Running Different Concurrent Environments:
+
+In this example, `scheduled_task` is used to create a scheduled task named `p` that runs as a `multiprocessing.Process`,
+and another task named `t` that runs as a `threading.Thread`.
+Both tasks execute the same function, `func`.
 
 >>> def func():
 ...     pass
 ...
 >>> p = scheduled_task(Process, 'p', func)
 >>> t = scheduled_task(Thread, 't', func)
 
-In this case, both `p` and `t` will be the same except that `p` will run as `multiprocessing.Process` and `t` will run as `threading.Thread`
+Args & Kwargs
+*************
 
-Parameters
-**********
+Passing Arguments and Dependencies:
 
-An example of basic usage for `args` and `kwargs`:
+Here, `scheduled_task` demonstrates passing arguments and dependencies.
+`p` calculates the sum of `1 + 2 + 3`, and `t` uses the return value of `p` as an argument.
 
 >>> def func1(a, b, c):
 ...     return a + b + c
 ...
 >>> def func2(x):
 ...     print(x)
 ...
 >>> p = scheduled_task(Process, 'p', func1, args=(1, 2), kwargs={'c': 3})
 >>> t = scheduled_task(Thread, 't', func2, kwargs={'x': p.return_value})
 
-In this case, `t` will start only after `p` completed, and the parameter `x` will be equal to `6`
-
 Dependencies
 ************
 
-An example of basic usage for `dependencies`:
+Managing Task Dependencies:
 
->>> def func1():
-...     # Saving a local file or updating a database record
+This example showcases task dependencies.
+`t` depends on the completion of `p` before starting its execution.
+
+>>> def func1(path, text):
+...     with open(path, 'w') as file:
+...         file.write(text)
 ...
->>> def func2():
-...     # Reading a local file or retrieving a record from the database
+>>> def func2(path):
+...     with open(path, 'r') as file:
+...         return file.read()
 ...
->>> p = scheduled_task(Process, 'p', func1)
->>> t = scheduled_task(Thread, 't', func2, dependencies=(p,))
+>>> p = scheduled_task(Process, 'p', func1, kwargs={'path': 'example.txt', 'text': 'Hello, World!'})
+>>> t = scheduled_task(Thread, 't', func2, kwargs={'path': 'example.txt'}, dependencies=(p,))
 
-In this case, `t` will start only after `p` completed
+Priority
+********
 
-Priorities
-**********
+Setting Task Priority:
 
-An example of basic usage for `priority`:
+In this scenario, tasks are assigned priorities.
+`t` is given higher priority than `p`, affecting their order of execution.
 
 >>> def func():
 ...     pass
 ...
 >>> p = scheduled_task(Process, 'p', func, priority=2)
 >>> t = scheduled_task(Thread, 't', func, priority=1)
 
-In this case, `t` will be prioritize over `p`
+Processes & Threads
+*******************
 
-Workers
-*******
+Balancing Processes and Threads:
 
-An example of basic usage for `processes` and `threads`:
+Here, `scheduled_task` is used to distribute workload across processes and threads based on specified weights.
 
 >>> def func():
 ...     with ProcessPoolExecutor(max_workers=2) as executor:
 ...         pass
 ...     with ThreadPoolExecutor(max_workers=4) as executor:
 ...         pass
 ...
 >>> p = scheduled_task(Process, 'p', func, processes=2, threads=4)
 
-In this case, 'p' will get additional weight of number of processes and threads
+Continual
+*********
 
-Continuity
-**********
+Storing Task Return Values:
 
-An example of basic usage for `continual`:
+This example illustrates how to manage stored return values.
+`p`'s return value is stored due to the `continual=True` parameter, while `t`'s return value is not stored.
 
 >>> def func():
 ...     return 123
 ...
 >>> p = scheduled_task(Process, 'p', func, continual=True)
 >>> t = scheduled_task(Thread, 't', func, continual=False)
-
-In this case, when the task scheduler will complete, it will store only the return value of `p`
```

### Comparing `parallelism-0.1.0/docs/index.rst` & `parallelism-0.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/api_reference.py` & `parallelism-0.1.1/parallelism/api_reference.py`

 * *Files 25% similar despite different names*

```diff
@@ -29,38 +29,55 @@
     dependencies: Tuple[ScheduledTask, ...] = None,
     priority: Union[int, float] = None,
     processes: int = 0,
     threads: int = 0,
     continual: bool = False,
 ) -> ScheduledTask:
     """
-    Schedule a task to be executed at the right moment in the task scheduler
+    The `scheduled_task` function empowers developers to efficiently manage and
+    execute tasks in a parallel computing environment.
+    It is a fundamental tool for creating and scheduling tasks within the task
+    scheduler, allowing for granular control over task execution, dependencies,
+    priorities, and result storage.
 
     Parameters
     ----------
-    executor : type of `multiprocessing.Process` or `threading.Thread`
-        | The execution unit of a task
+    executor : type of multiprocessing.Process or threading.Thread
+        | Specifies the execution unit for the task, either as a
+        `multiprocessing.Process` or a `threading.Thread`.
     name : str
-        | A unique identifier representing a task
+        | A unique identifier representing the task, aiding in differentiation
+        and tracking.
     target : callable
-        | A function to be invoked by a task scheduler
+        | The function to be invoked by the task scheduler upon execution.
     args : tuple, optional
-        | Positional arguments that are related to the target
+        | Positional arguments related to the `target` function.
     kwargs : dict, optional
-        | Keyword arguments that are related to the target
+        | Keyword arguments related to the `target` function.
     dependencies : tuple of ScheduledTask, optional
-        | Certain tasks that create dependencies for the current task
+        | Tasks that the current task depends on, ensuring proper execution
+        order.
     priority : int or float, optional
-        | Priority level of task execution over others
+        | Priority level of task execution, influencing the order of execution
+        among tasks.
+        | Lower values indicate higher priority.
     processes : int, default 0
-        | The number of processes will be allocated retrospectively at runtime
+        | The number of processes to be allocated by the `target` function.
     threads : int, default 0
-        | The number of threads will be allocated retrospectively at runtime
+        | The number of threads to be allocated by the `target` function.
     continual : bool, default False
-        | An indicator to save the result after the task scheduler
+        | A flag indicating whether the task scheduler should store the result
+        of the task after completion.
+        | If `True`, the result is stored for later access.
+
+    Returns
+    -------
+    ScheduledTask
+        A scheduled task instance with configured properties, ready for
+        execution within the task scheduler.
     """
     if args is None:
         args = ()
     if kwargs is None:
         kwargs = {}
     if dependencies is None:
         dependencies = ()
@@ -127,24 +144,39 @@
 def task_scheduler(
     tasks: Tuple[ScheduledTask, ...],
     *,
     processes: int = None,
     threads: int = None,
 ) -> SchedulerResult:
     """
-    Schedule multiple tasks for execution
+    The `task_scheduler` function orchestrates the simultaneous execution of
+    multiple tasks, optimizing parallelism and enhancing computational
+    efficiency.
+    It allows developers to efficiently manage and distribute tasks among
+    processes and threads for improved performance.
 
     Parameters
     ----------
     tasks : tuple of ScheduledTask
-        | Tasks that need to be performed
-    processes : int, default `os.cpu_count()`
-        | The number of processes assigned to perform the tasks
-    threads : int, default `os.cpu_count()`
-        | The number of threads assigned to perform the tasks
+        | A tuple containing instances of ScheduledTask representing the
+        tasks to be executed concurrently.
+    processes : int, default os.cpu_count()
+        | Specifies the total number of parallel processes available for
+        executing all tasks collectively.
+    threads : int, default os.cpu_count()
+        | Specifies the total number of parallel threads available for
+        executing all tasks collectively.
+
+    Returns
+    -------
+    SchedulerResult
+        An instance of the `SchedulerResult` class that encapsulates the
+        outcomes and statistics of task execution.
+        This result provides insights into execution times, elapsed times,
+        exceptions, and return values.
     """
     if processes is None:
         processes = cpu_count() or 1
     if threads is None:
         threads = cpu_count() or 1
     if not isinstance(tasks, tuple):
         pattern = 'The {!r} parameter should be of type {!r}'
```

### Comparing `parallelism-0.1.0/parallelism/core/executors/process_executor.py` & `parallelism-0.1.1/parallelism/core/executors/process_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/core/executors/thread_executor.py` & `parallelism-0.1.1/parallelism/core/executors/thread_executor.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/core/handlers/dependency_handler.py` & `parallelism-0.1.1/parallelism/core/handlers/dependency_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/core/handlers/function_handler.py` & `parallelism-0.1.1/parallelism/core/handlers/function_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,19 +43,22 @@
 
     def __call__(self, *args: Any, **kwargs: Any) -> None:
         start = time()
         try:
             self.proxy['return_value'] = self.target(*args, **kwargs)
             self.proxy['complete'] = True
         except Exception as exception:
-            self.proxy['raise_exception'] = RaiseException(exception, format_exc())
+            self.proxy['raise_exception'] = RaiseException(
+                exception=exception,
+                traceback=format_exc(),
+            )
         finally:
             end = time()
-            self.proxy['finish'] = True
             self.proxy['elapsed_time'] = end - start
+            self.proxy['finish'] = True
             self.log_current_state()
 
     def log_current_state(
         self,
         blocker: Optional[Dict[str, Any]] = None,
     ) -> None:
         logger = get_logger()
```

### Comparing `parallelism-0.1.0/parallelism/core/handlers/parameters_handler.py` & `parallelism-0.1.1/parallelism/core/handlers/parameters_handler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/core/handlers/shared_memory_handler.py` & `parallelism-0.1.1/parallelism/core/handlers/shared_memory_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,17 @@
         proxy = self.proxy.get(task.name)
         if (
             proxy.get('finish') and
             self.has_shared_memory(task) and
             self.prerequisites_been_initialized(task)
         ):
             self.execution_time[task.name] = proxy.get('execution_time')
-            if proxy.get('elapsed_time'):
+            if proxy.get('elapsed_time') is not None:
                 self.elapsed_time[task.name] = proxy.get('elapsed_time')
-            if proxy.get('raise_exception'):
+            if proxy.get('raise_exception') is not None:
                 self.raise_exception[task.name] = proxy.get('raise_exception')
             elif task.continual:
                 self.return_value[task.name] = proxy.get('return_value')
             self.tasks[index] = ScheduledTask(
                 executor=task.executor.__class__.__base__,
                 name=task.name,
                 target=task.target,
```

### Comparing `parallelism-0.1.0/parallelism/core/return_value.py` & `parallelism-0.1.1/parallelism/core/return_value.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/core/scheduled_task.py` & `parallelism-0.1.1/parallelism/core/scheduled_task.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism/core/task_scheduler.py` & `parallelism-0.1.1/parallelism/core/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/parallelism.egg-info/PKG-INFO` & `parallelism-0.1.1/parallelism.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: parallelism
-Version: 0.1.0
+Version: 0.1.1
 Summary: Empowering workflows with parallelism
 Author: Idan Hazan
 License: MIT
 Project-URL: homepage, https://github.com/idanhazan/parallelism
 Project-URL: repository, https://github.com/idanhazan/parallelism
 Project-URL: documentation, https://parallelism.readthedocs.io
 Keywords: parallelism,parallel,task,scheduler
```

### Comparing `parallelism-0.1.0/parallelism.egg-info/SOURCES.txt` & `parallelism-0.1.1/parallelism.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `parallelism-0.1.0/pyproject.toml` & `parallelism-0.1.1/pyproject.toml`

 * *Files identical despite different names*

