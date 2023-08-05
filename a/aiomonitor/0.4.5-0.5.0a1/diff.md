# Comparing `tmp/aiomonitor-0.4.5.tar.gz` & `tmp/aiomonitor-0.5.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aiomonitor-0.4.5.tar", last modified: Mon Nov  4 03:30:26 2019, max compression
+gzip compressed data, was "aiomonitor-0.5.0a1.tar", last modified: Thu May  4 04:03:23 2023, max compression
```

## Comparing `aiomonitor-0.4.5.tar` & `aiomonitor-0.5.0a1.tar`

### file list

```diff
@@ -1,20 +1,70 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1622 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/CHANGES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)    11311 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)       99 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)    10334 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     5834 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/README.rst
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor/
--rw-rw-r--   0 travis    (2000) travis    (2000)      774 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/aiomonitor/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      866 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/aiomonitor/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15494 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/aiomonitor/monitor.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/aiomonitor/mypy_types.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4203 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/aiomonitor/utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)    10334 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)      328 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       26 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/aiomonitor.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2019-11-04 03:30:26.000000 aiomonitor-0.4.5/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1876 2019-11-04 03:29:31.000000 aiomonitor-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.384182 aiomonitor-0.5.0a1/
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.376182 aiomonitor-0.5.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.376182 aiomonitor-0.5.0a1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.376182 aiomonitor-0.5.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     3501 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/workflows/ci-cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/workflows/flake8-matcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/workflows/lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.github/workflows/mypy-matcher.json
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.pyup.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11311 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-04 04:03:23.384182 aiomonitor-0.5.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.376182 aiomonitor-0.5.0a1/aiomonitor/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31408 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3565 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9560 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/telnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7904 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/aiomonitor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.376182 aiomonitor-0.5.0a1/aiomonitor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10669 2023-05-04 04:03:23.000000 aiomonitor-0.5.0a1/aiomonitor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-04 04:03:23.000000 aiomonitor-0.5.0a1/aiomonitor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 04:03:23.000000 aiomonitor-0.5.0a1/aiomonitor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 04:03:23.000000 aiomonitor-0.5.0a1/aiomonitor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-04 04:03:23.000000 aiomonitor-0.5.0a1/aiomonitor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 04:03:23.000000 aiomonitor-0.5.0a1/aiomonitor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.380182 aiomonitor-0.5.0a1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5620 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)   365314 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/screenshot-ps-where-example.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1874166 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/tty.gif
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.384182 aiomonitor-0.5.0a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2752 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/cancellation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/console-variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/extension.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/simple_aiohttp_srv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/simple_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/taskgroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/web_srv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/web_srv_custom_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/examples/x.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/requirements-doc.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-04 04:03:23.384182 aiomonitor-0.5.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 04:03:23.384182 aiomonitor-0.5.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7942 2023-05-04 04:03:13.000000 aiomonitor-0.5.0a1/tests/test_monitor.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aiomonitor-0.4.5/LICENSE` & `aiomonitor-0.5.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomonitor-0.4.5/README.rst` & `aiomonitor-0.5.0a1/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 aiomonitor
 ==========
-.. image:: https://travis-ci.com/aio-libs/aiomonitor.svg?branch=master
-    :target: https://travis-ci.com/aio-libs/aiomonitor
-.. image:: https://codecov.io/gh/aio-libs/aiomonitor/branch/master/graph/badge.svg
-    :target: https://codecov.io/gh/aio-libs/aiomonitor
-.. image:: https://api.codeclimate.com/v1/badges/d14af4cfb0c4ff52b1ef/maintainability
-   :target: https://codeclimate.com/github/aio-libs/aiomonitor/maintainability
-   :alt: Maintainability
-.. image:: https://img.shields.io/pypi/v/aiomonitor.svg
-    :target: https://pypi.python.org/pypi/aiomonitor
-.. image:: https://readthedocs.org/projects/aiomonitor/badge/?version=latest
-    :target: http://aiomonitor.readthedocs.io/en/latest/?badge=latest
-    :alt: Documentation Status
-.. image:: https://badges.gitter.im/Join%20Chat.svg
-    :target: https://gitter.im/aio-libs/Lobby
-    :alt: Chat on Gitter
-
-**aiomonitor** is Python 3.5+ module that adds monitor and cli capabilities
-for asyncio_ application. Idea and code borrowed from curio_ project.
-Task monitor that runs concurrently to the asyncio_ loop (or fast drop in
+
+.. image:: https://github.com/aio-libs/aiomonitor/workflows/CI/badge.svg
+   :target: https://github.com/aio-libs/aiomonitor/actions?query=workflow%3ACI
+   :alt: GitHub Actions status for the main branch
+
+.. image:: https://codecov.io/gh/aio-libs/aiomonitor/branch/main/graph/badge.svg
+   :target: https://codecov.io/gh/aio-libs/aiomonitor
+   :alt: codecov.io status for the main branch
+
+.. image:: https://badge.fury.io/py/aiomonitor.svg
+   :target: https://pypi.org/project/aiomonitor
+   :alt: Latest PyPI package version
+
+.. image:: https://img.shields.io/pypi/dm/aiomonitor
+   :target: https://pypistats.org/packages/aiomonitor
+   :alt: Downloads count
+
+.. image:: https://readthedocs.org/projects/aiomonitor-ng/badge/?version=latest
+   :target: https://aiomonitor.aio-libs.org/en/latest/?badge=latest
+   :alt: Documentation Status
+
+**aiomonitor** is a module that adds monitor and cli capabilities
+for asyncio_ applications. Idea and code were borrowed from curio_ project.
+Task monitor that runs concurrently to the asyncio_ loop (or fast drop-in
 replacement uvloop_) in a separate thread as result monitor will work even if
-event loop is blocked for some reason.
+the event loop is blocked for some reason.
 
-Library provides an python console using aioconsole_ module, it is possible
-to execute asynchronous command inside your running application. Extensible
+This library provides a python console using aioconsole_ module. It is possible
+to execute asynchronous commands inside your running application. Extensible
 with you own commands, in the style of the standard library's cmd_ module
 
-+--------------------------------------------------------------------------------------+
-| .. image:: https://raw.githubusercontent.com/aio-libs/aiomonitor/master/docs/tty.gif |
-+--------------------------------------------------------------------------------------+
+.. image:: https://raw.githubusercontent.com/aio-libs/aiomonitor/main/docs/screenshot-ps-where-example.png
+   :alt: An example to run the aiomonitor shell
 
 Installation
 ------------
 Installation process is simple, just::
 
     $ pip install aiomonitor
 
@@ -41,132 +45,152 @@
 -------
 Monitor has context manager interface:
 
 .. code:: python
 
     import aiomonitor
 
-    loop = asyncio.get_event_loop()
-    with aiomonitor.start_monitor(loop=loop):
-        loop.run_forever()
+    async def main():
+        loop = asyncio.get_running_loop()
+        run_forever = loop.create_future()
+        with aiomonitor.start_monitor(loop):
+            await run_forever
+
+    try:
+        asyncio.run(main())
+    except KeyboardInterrupt:
+        pass
 
 Now from separate terminal it is possible to connect to the application::
 
-    $ nc localhost 50101
+    $ telnet localhost 50101
 
-or using included python client::
+or the included python client::
 
     $ python -m aiomonitor.cli
-
+    
+    
 Tutorial
 --------
 
-Lets create simple aiohttp_ application, and see how ``aiomonitor`` can
-integrates with it.
+Let's create a simple aiohttp_ application, and see how ``aiomonitor`` can
+be integrated with it.
 
 .. code:: python
 
     import asyncio
 
     import aiomonitor
     from aiohttp import web
 
     # Simple handler that returns response after 100s
     async def simple(request):
         loop = request.app.loop
 
         print('Start sleeping')
-        await asyncio.sleep(100, loop=loop)
+        await asyncio.sleep(100)
         return web.Response(text="Simple answer")
 
     loop = asyncio.get_event_loop()
     # create application and register route
-    app = web.Application(loop=loop)
+    app = web.Application()
     app.router.add_get('/simple', simple)
 
-    # it is possible to pass dictionary with local variables
+    # it is possible to pass a dictionary with local variables
     # to the python console environment
     host, port = "localhost", 8090
     locals_ = {"port": port, "host": host}
     # init monitor just before run_app
     with aiomonitor.start_monitor(loop=loop, locals=locals_):
-        # run application with built in aiohttp run_app function
+        # run application with built-in aiohttp run_app function
         web.run_app(app, port=port, host=host)
 
-Lets save this code in file ``simple_srv.py``, so we can run it with command::
+Let's save this code in file ``simple_srv.py``, so we can run it with the following command::
 
     $ python simple_srv.py
     ======== Running on http://localhost:8090 ========
     (Press CTRL+C to quit)
 
-And now one can connect running application from separate terminal, with
-``nc`` command, immediately ``aiomonitor`` will respond with prompt::
+And now one can connect to a running application from a separate terminal, with
+the ``telnet`` command, and ``aiomonitor`` will immediately respond with prompt::
 
-    $ nc localhost 50101
+    $ telnet localhost 50101
     Asyncio Monitor: 1 tasks running
     Type help for commands
     monitor >>>
 
-Now you can type commands, for instance ``help``::
+Now you can type commands, for instance, ``help``::
 
     monitor >>> help
+    Usage: help [OPTIONS] COMMAND [ARGS]...
+    
+      To see the usage of each command, run them with "--help" option.
+    
     Commands:
-                 ps               : Show task table
-                 where taskid     : Show stack frames for a task
-                 cancel taskid    : Cancel an indicated task
-                 signal signame   : Send a Unix signal
-                 stacktrace       : Print a stack trace from the event loop thread
-                 console          : Switch to async Python REPL
-                 quit             : Leave the monitor
+      cancel                  Cancel an indicated task
+      console                 Switch to async Python REPL
+      exit (q,quit)           Leave the monitor client session
+      help (?,h)              Show the list of commands
+      ps (p)                  Show task table
+      ps-terminated (pst,pt)  List recently terminated/cancelled tasks
+      signal                  Send a Unix signal
+      stacktrace (st,stack)   Print a stack trace from the event loop thread
+      where (w)               Show stack frames and the task creation chain of a task
+      where-terminated (wt)   Show stack frames and the termination/cancellation chain of a task
 
-``aiomonitor`` supports also async python console inside running event loop
-so you can explore state of your application::
+``aiomonitor`` also supports async python console inside a running event loop
+so you can explore the state of your application::
 
     monitor >>> console
-    Python 3.5.2 (default, Oct 11 2016, 05:05:28)
-    [GCC 4.2.1 Compatible Apple LLVM 8.0.0 (clang-800.0.38)] on darwin
+    Python 3.10.7 (main, Sep  9 2022, 12:31:20) [Clang 13.1.6 (clang-1316.0.21.2.5)] on darwin
     Type "help", "copyright", "credits" or "license" for more information.
     ---
     This console is running in an asyncio event loop.
     It allows you to wait for coroutines using the 'await' syntax.
-    Try: await asyncio.sleep(1, result=3, loop=loop)
+    Try: await asyncio.sleep(1, result=3)
     ---
-    >>> await asyncio.sleep(1, result=3, loop=loop)
+    >>> await asyncio.sleep(1, result=3)
+    3
+    >>>
 
-To leave console type ``exit()``::
+To leave the console type ``exit()`` or press Ctrl+D::
 
     >>> exit()
+
+    ✓ The console session is closed.
     monitor >>>
 
+Extension
+---------
 
-``aiomonitor`` is very easy to extend with your own console commands.
+Additional console variables
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
-.. code:: python
+You may add more variables that can be directly referenced in the ``console`` command.
+Refer `the console-variables example code <https://github.com/aio-libs/aiomonitor/tree/main/examples/console-variables.py>`_
 
-   class WebMonitor(aiomonitor.Monitor):
-       def do_hello(self, sin, sout, name=None):
-           """Using the /hello GET interface
-
-           There is one optional argument, "name".  This name argument must be
-           provided with proper URL excape codes, like %20 for spaces.
-           """
-           name = '' if name is None else '/' + name
-           r = requests.get('http://localhost:8090/hello' + name)
-           sout.write(r.text + '\n')
+Custom console commands
+~~~~~~~~~~~~~~~~~~~~~~~
 
+``aiomonitor`` is very easy to extend with your own console commands.
+Refer `the extension example code <https://github.com/aio-libs/aiomonitor/tree/main/examples/extension.py>`_
 
 Requirements
 ------------
 
-* Python_ 3.5+
+* Python_ 3.8+ (3.10.7+ recommended)
 * aioconsole_
+* Click_
+* prompt_toolkit_
 * uvloop_ (optional)
 
 
 .. _PEP492: https://www.python.org/dev/peps/pep-0492/
 .. _Python: https://www.python.org
 .. _aioconsole: https://github.com/vxgmichel/aioconsole
-.. _aiohttp: https://github.com/KeepSafe/aiohttp
-.. _asyncio: http://docs.python.org/3.5/library/asyncio.html
+.. _aiohttp: https://github.com/aio-libs/aiohttp
+.. _asyncio: http://docs.python.org/3/library/asyncio.html
+.. _Click: https://click.palletsprojects.com
 .. _curio: https://github.com/dabeaz/curio
+.. _prompt_toolkit: https://python-prompt-toolkit.readthedocs.io
 .. _uvloop: https://github.com/MagicStack/uvloop
 .. _cmd: http://docs.python.org/3/library/cmd.html
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiomonitor-0.4.5/aiomonitor/__init__.py` & `aiomonitor-0.5.0a1/aiomonitor/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,41 @@
 
 To enable the monitor, just use context manager protocol with start function::
 
     import asyncio
     import aiomonitor
 
     loop = asyncio.get_event_loop()
-    with aiomonitor.start_monitor(loop=loop):
+    with aiomonitor.start_monitor():
         print("Now you can connect with: nc localhost 50101")
         loop.run_forever()
 
 Alternatively you can use more verbose try/finally approach::
 
     m = Monitor()
     m.start()
     try:
         loop.run_forever()
     finally:
         m.close()
 """
 
-from .monitor import (Monitor, start_monitor,
-                      MONITOR_HOST, MONITOR_PORT, CONSOLE_PORT)
+from importlib.metadata import version
 
-
-__all__ = ('Monitor', 'start_monitor', 'MONITOR_HOST', 'MONITOR_PORT',
-           'CONSOLE_PORT')
-__version__ = '0.4.5'
+from .monitor import (
+    CONSOLE_PORT,
+    MONITOR_HOST,
+    MONITOR_PORT,
+    Monitor,
+    monitor_cli,
+    start_monitor,
+)
+
+__all__ = (
+    "Monitor",
+    "monitor_cli",
+    "start_monitor",
+    "MONITOR_HOST",
+    "MONITOR_PORT",
+    "CONSOLE_PORT",
+)
+__version__ = version("aiomonitor")
```

### Comparing `aiomonitor-0.4.5/aiomonitor/cli.py` & `aiomonitor-0.5.0a1/aiomonitor/cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,43 @@
 import argparse
-import telnetlib
+import asyncio
 
 from .monitor import MONITOR_HOST, MONITOR_PORT
+from .telnet import TelnetClient
+
+
+async def async_monitor_client(host: str, port: int) -> None:
+    async with TelnetClient(host, port) as client:
+        await client.interact()
 
 
 def monitor_client(host: str, port: int) -> None:
-    tn = telnetlib.Telnet()
-    tn.open(host, port, timeout=1)
     try:
-        tn.interact()
+        asyncio.run(async_monitor_client(host, port))
     except KeyboardInterrupt:
         pass
-    finally:
-        tn.close()
 
 
 def main() -> None:
-    parser = argparse.ArgumentParser('usage: python -m aiomonitor [options]')
-    parser.add_argument('-H', '--host', dest='monitor_host',
-                        default=MONITOR_HOST, type=str,
-                        help='monitor host ip')
-
-    parser.add_argument('-p', '--port', dest='monitor_port',
-                        default=MONITOR_PORT, type=int,
-                        help='monitor port number')
+    parser = argparse.ArgumentParser()
+    parser.add_argument(
+        "-H",
+        "--host",
+        dest="monitor_host",
+        default=MONITOR_HOST,
+        type=str,
+        help="monitor host ip",
+    )
+    parser.add_argument(
+        "-p",
+        "--port",
+        dest="monitor_port",
+        default=MONITOR_PORT,
+        type=int,
+        help="monitor port number",
+    )
     args = parser.parse_args()
     monitor_client(args.monitor_host, args.monitor_port)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

