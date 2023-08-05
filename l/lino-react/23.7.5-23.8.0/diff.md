# Comparing `tmp/lino_react-23.7.5.tar.gz` & `tmp/lino_react-23.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.7.5.tar", last modified: Sun Jul 30 09:57:59 2023, max compression
+gzip compressed data, was "lino_react-23.8.0.tar", last modified: Fri Aug  4 15:04:16 2023, max compression
```

## Comparing `lino_react-23.7.5.tar` & `lino_react-23.8.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.713161 lino_react-23.7.5/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.7.5/COPYING
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.7.5/MANIFEST.in
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-07-30 09:57:59.713161 lino_react-23.7.5/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.7.5/README.rst
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4628 2023-06-13 10:46:31.000000 lino_react-23.7.5/lino_react/react/__init__.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/react/__pycache__/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3382 2023-06-15 05:49:26.000000 lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     4030 2023-07-10 10:58:39.000000 lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      160 2023-03-30 05:54:52.000000 lino_react-23.7.5/lino_react/react/__pycache__/models.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/models.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18587 2023-07-24 14:50:37.000000 lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-38.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-06-12 10:17:24.000000 lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-310.pyc
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-38.pyc
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.701161 lino_react-23.7.5/lino_react/react/config/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react/react/config/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1910 2023-07-24 06:45:56.000000 lino_react-23.7.5/lino_react/react/config/react/main.html
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-07-30 07:00:19.000000 lino_react-23.7.5/lino_react/react/config/react/service-worker.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     3952 2023-07-10 10:58:36.000000 lino_react-23.7.5/lino_react/react/icons.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/index.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-03-30 05:51:42.000000 lino_react-23.7.5/lino_react/react/models.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    29603 2023-07-24 14:50:33.000000 lino_react-23.7.5/lino_react/react/renderer.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.701161 lino_react-23.7.5/lino_react/react/static/
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.709161 lino_react-23.7.5/lino_react/react/static/media/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/color.6441e63a.png
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/color.c7a33805.png
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/line.567f5738.gif
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.7.5/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.713161 lino_react-23.7.5/lino_react/react/static/react/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)  1790540 2023-07-30 07:00:19.000000 lino_react-23.7.5/lino_react/react/static/react/main.js
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-07-30 07:00:19.000000 lino_react-23.7.5/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-06-11 15:16:59.000000 lino_react-23.7.5/lino_react/react/views.py
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-07-30 09:57:19.000000 lino_react-23.7.5/lino_react/setup_info.py
-drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-07-30 09:57:59.705161 lino_react-23.7.5/lino_react.egg-info/
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/PKG-INFO
--rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/SOURCES.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/dependency_links.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.7.5/lino_react.egg-info/not-zip-safe
--rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/requires.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-07-30 09:57:59.000000 lino_react-23.7.5/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-07-30 09:57:59.713161 lino_react-23.7.5/setup.cfg
--rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.7.5/setup.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.848993 lino_react-23.8.0/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    34523 2023-02-28 05:23:19.000000 lino_react-23.8.0/COPYING
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      157 2023-02-28 05:23:19.000000 lino_react-23.8.0/MANIFEST.in
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-08-04 15:04:16.848993 lino_react-23.8.0/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      178 2023-02-28 05:23:19.000000 lino_react-23.8.0/README.rst
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.836993 lino_react-23.8.0/lino_react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      283 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.836993 lino_react-23.8.0/lino_react/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4628 2023-06-13 10:46:31.000000 lino_react-23.8.0/lino_react/react/__init__.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.840993 lino_react-23.8.0/lino_react/react/__pycache__/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3382 2023-06-15 05:49:26.000000 lino_react-23.8.0/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2980 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/__pycache__/__init__.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     4030 2023-07-10 10:58:39.000000 lino_react-23.8.0/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3793 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/__pycache__/icons.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      160 2023-03-30 05:54:52.000000 lino_react-23.8.0/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1412 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/__pycache__/models.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18587 2023-07-24 14:50:37.000000 lino_react-23.8.0/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    18127 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/__pycache__/renderer.cpython-38.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20615 2023-06-12 10:17:24.000000 lino_react-23.8.0/lino_react/react/__pycache__/views.cpython-310.pyc
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    20473 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/__pycache__/views.cpython-38.pyc
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.836993 lino_react-23.8.0/lino_react/react/config/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.840993 lino_react-23.8.0/lino_react/react/config/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1910 2023-07-24 06:45:56.000000 lino_react-23.8.0/lino_react/react/config/react/main.html
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    16246 2023-08-04 15:00:16.000000 lino_react-23.8.0/lino_react/react/config/react/service-worker.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     3952 2023-07-10 10:58:36.000000 lino_react-23.8.0/lino_react/react/icons.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       36 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/index.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        0 2023-03-30 05:51:42.000000 lino_react-23.8.0/lino_react/react/models.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    29603 2023-07-24 14:50:33.000000 lino_react-23.8.0/lino_react/react/renderer.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.836993 lino_react-23.8.0/lino_react/react/static/
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.848993 lino_react-23.8.0/lino_react/react/static/media/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    10355 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    13112 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39748 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57384 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39648 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   234640 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    39572 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57560 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)   163568 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    57460 2023-02-28 05:23:19.000000 lino_react-23.8.0/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.848993 lino_react-23.8.0/lino_react/react/static/react/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)  1802225 2023-08-04 15:00:16.000000 lino_react-23.8.0/lino_react/react/static/react/main.js
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     2437 2023-08-04 15:00:16.000000 lino_react-23.8.0/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)    28705 2023-06-11 15:16:59.000000 lino_react-23.8.0/lino_react/react/views.py
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1431 2023-08-04 15:03:24.000000 lino_react-23.8.0/lino_react/setup_info.py
+drwxrwsr-x   0 blurry    (1000) blurry    (1000)        0 2023-08-04 15:04:16.836993 lino_react-23.8.0/lino_react.egg-info/
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1032 2023-08-04 15:04:16.000000 lino_react-23.8.0/lino_react.egg-info/PKG-INFO
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)     1770 2023-08-04 15:04:16.000000 lino_react-23.8.0/lino_react.egg-info/SOURCES.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-08-04 15:04:16.000000 lino_react-23.8.0/lino_react.egg-info/dependency_links.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        1 2023-02-28 05:23:26.000000 lino_react-23.8.0/lino_react.egg-info/not-zip-safe
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)        5 2023-08-04 15:04:16.000000 lino_react-23.8.0/lino_react.egg-info/requires.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       11 2023-08-04 15:04:16.000000 lino_react-23.8.0/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)       38 2023-08-04 15:04:16.848993 lino_react-23.8.0/setup.cfg
+-rw-rw-r--   0 blurry    (1000) blurry    (1000)      183 2023-02-28 05:23:19.000000 lino_react-23.8.0/setup.py
```

### Comparing `lino_react-23.7.5/COPYING` & `lino_react-23.8.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/PKG-INFO` & `lino_react-23.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino_react
-Version: 23.7.5
+Version: 23.8.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
```

### Comparing `lino_react-23.7.5/lino_react/react/__init__.py` & `lino_react-23.8.0/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-310.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/__init__.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/__init__.cpython-38.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-310.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/icons.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/icons.cpython-38.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/icons.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/models.cpython-38.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/models.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-310.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/renderer.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/renderer.cpython-38.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/renderer.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-310.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/views.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/__pycache__/views.cpython-38.pyc` & `lino_react-23.8.0/lino_react/react/__pycache__/views.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/config/react/main.html` & `lino_react-23.8.0/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/config/react/service-worker.js` & `lino_react-23.8.0/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/icons.py` & `lino_react-23.8.0/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/renderer.py` & `lino_react-23.8.0/lino_react/react/renderer.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.8.0/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.8.0/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.8.0/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.8.0/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/static/react/main.js` & `lino_react-23.8.0/lino_react/react/static/react/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -5,15 +5,15 @@
                 "use strict";
                 n.d(t, {
                     v: () => f
                 });
                 var o = n(2437),
                     r = n(6318),
                     i = n.n(r),
-                    a = n(6149),
+                    a = n(6147),
                     l = (n(3504), n(7705), n(7239));
 
                 function s(e) {
                     return s = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
@@ -743,16 +743,17 @@
                                 miStore: [],
                                 themeName: "default",
                                 onDashboard: !1,
                                 editorDirty: !1,
                                 versionMismatch: !1,
                                 selectedLanguage: null,
                                 scroll: {},
-                                scrollIndex: []
-                            }, _this.rps = {}, _this.setRpRef = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.a_)(_this.rps), _this.dialogRefs = {}, _this.setupDialogRefs = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.a_)(_this.dialogRefs), _this.response_callbacks = {}, _this.createAccount = _this.createAccount.bind(_assertThisInitialized(_this)), _this.messageInterceptor = _this.messageInterceptor.bind(_assertThisInitialized(_this)), _this.onHrefClick = _this.onHrefClick.bind(_assertThisInitialized(_this)), _this.onKeyDown = _this.onKeyDown.bind(_assertThisInitialized(_this)), _this.handleVerification = _this.handleVerification.bind(_assertThisInitialized(_this)), _this.onWrapperClick = _this.onWrapperClick.bind(_assertThisInitialized(_this)), _this.onToggleMenu = _this.onToggleMenu.bind(_assertThisInitialized(_this)), _this.onSidebarClick = _this.onSidebarClick.bind(_assertThisInitialized(_this)), _this.onMenuItemClick = _this.onMenuItemClick.bind(_assertThisInitialized(_this)), _this.onHomeButton = _this.onHomeButton.bind(_assertThisInitialized(_this)), _this.onSignOutIn = _this.onSignOutIn.bind(_assertThisInitialized(_this)), _this.handleActionResponse = _this.handleActionResponse.bind(_assertThisInitialized(_this)), _this.runAction = _this.runAction.bind(_assertThisInitialized(_this)), _this.wrappedRunAction = _this.wrappedRunAction.bind(_assertThisInitialized(_this)), _this.onAuthoritiesSelect = _this.onAuthoritiesSelect.bind(_assertThisInitialized(_this)), _this.add_su = _this.add_su.bind(_assertThisInitialized(_this)), _this.setLoadMask = _this.setLoadMask.bind(_assertThisInitialized(_this)), _this.removeLoadMask = _this.removeLoadMask.bind(_assertThisInitialized(_this)), _this.notification_web_socket = _this.notification_web_socket.bind(_assertThisInitialized(_this)), _this.push = _this.push.bind(_assertThisInitialized(_this)), _this.pushChat = _this.pushChat.bind(_assertThisInitialized(_this)), _this.sendChat = _this.sendChat.bind(_assertThisInitialized(_this)), _this.sendSeenAction = _this.sendSeenAction.bind(_assertThisInitialized(_this)), _this.OpenConversation = _this.OpenConversation.bind(_assertThisInitialized(_this)), _this.onChatButton = _this.onChatButton.bind(_assertThisInitialized(_this)), _this.positionChatOp = _this.positionChatOp.bind(_assertThisInitialized(_this)), _this.chatwindow = react__WEBPACK_IMPORTED_MODULE_0__.createRef(), _this.onMainWindowUpdate = _this.onMainWindowUpdate.bind(_assertThisInitialized(_this)), window.App = _assertThisInitialized(_this), _this
+                                scrollIndex: [],
+                                zoomHandles: {}
+                            }, _this.rps = {}, _this.setRpRef = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.a_)(_this.rps), _this.dialogRefs = {}, _this.setupDialogRefs = (0, _LinoUtils__WEBPACK_IMPORTED_MODULE_17__.a_)(_this.dialogRefs), _this.response_callbacks = {}, _this.createAccount = _this.createAccount.bind(_assertThisInitialized(_this)), _this.handleVerification = _this.handleVerification.bind(_assertThisInitialized(_this)), _this.handleZoom = _this.handleZoom.bind(_assertThisInitialized(_this)), _this.messageInterceptor = _this.messageInterceptor.bind(_assertThisInitialized(_this)), _this.onHrefClick = _this.onHrefClick.bind(_assertThisInitialized(_this)), _this.onKeyDown = _this.onKeyDown.bind(_assertThisInitialized(_this)), _this.registerZoomHandle = _this.registerZoomHandle.bind(_assertThisInitialized(_this)), _this.unregisterZoomHandle = _this.unregisterZoomHandle.bind(_assertThisInitialized(_this)), _this.onWrapperClick = _this.onWrapperClick.bind(_assertThisInitialized(_this)), _this.onToggleMenu = _this.onToggleMenu.bind(_assertThisInitialized(_this)), _this.onSidebarClick = _this.onSidebarClick.bind(_assertThisInitialized(_this)), _this.onMenuItemClick = _this.onMenuItemClick.bind(_assertThisInitialized(_this)), _this.onHomeButton = _this.onHomeButton.bind(_assertThisInitialized(_this)), _this.onSignOutIn = _this.onSignOutIn.bind(_assertThisInitialized(_this)), _this.handleActionResponse = _this.handleActionResponse.bind(_assertThisInitialized(_this)), _this.runAction = _this.runAction.bind(_assertThisInitialized(_this)), _this.wrappedRunAction = _this.wrappedRunAction.bind(_assertThisInitialized(_this)), _this.onAuthoritiesSelect = _this.onAuthoritiesSelect.bind(_assertThisInitialized(_this)), _this.add_su = _this.add_su.bind(_assertThisInitialized(_this)), _this.setLoadMask = _this.setLoadMask.bind(_assertThisInitialized(_this)), _this.removeLoadMask = _this.removeLoadMask.bind(_assertThisInitialized(_this)), _this.notification_web_socket = _this.notification_web_socket.bind(_assertThisInitialized(_this)), _this.push = _this.push.bind(_assertThisInitialized(_this)), _this.pushChat = _this.pushChat.bind(_assertThisInitialized(_this)), _this.sendChat = _this.sendChat.bind(_assertThisInitialized(_this)), _this.sendSeenAction = _this.sendSeenAction.bind(_assertThisInitialized(_this)), _this.OpenConversation = _this.OpenConversation.bind(_assertThisInitialized(_this)), _this.onChatButton = _this.onChatButton.bind(_assertThisInitialized(_this)), _this.positionChatOp = _this.positionChatOp.bind(_assertThisInitialized(_this)), _this.chatwindow = react__WEBPACK_IMPORTED_MODULE_0__.createRef(), _this.onMainWindowUpdate = _this.onMainWindowUpdate.bind(_assertThisInitialized(_this)), window.App = _assertThisInitialized(_this), _this
                         }
                         return _createClass(App, [{
                             key: "componentDidMount",
                             value: function() {
                                 var e = null;
                                 if (Object.keys(query_string__WEBPACK_IMPORTED_MODULE_4__.parse(window.location.search)).includes("update_found")) {
                                     var t = window.location.origin;
@@ -762,14 +763,37 @@
                             }
                         }, {
                             key: "componentWillUnmount",
                             value: function() {
                                 window.removeEventListener("resize", this.positionChatOp), window.removeEventListener("message", this.messageInterceptor), window.removeEventListener("keydown", this.onKeyDown), window.removeEventListener("click", this.onHrefClick)
                             }
                         }, {
+                            key: "registerZoomHandle",
+                            value: function(e, t) {
+                                this.data.zoomHandles[e] = t
+                            }
+                        }, {
+                            key: "unregisterZoomHandle",
+                            value: function(e) {
+                                delete this.data.zoomHandles[e]
+                            }
+                        }, {
+                            key: "handleZoom",
+                            value: function() {
+                                if (this.tbContainer) {
+                                    var e = this.tbContainer.getBoundingClientRect().bottom;
+                                    setInterval((function(t) {
+                                        var n = t.tbContainer.getBoundingClientRect().bottom;
+                                        n != e && (e = n, Object.values(t.data.zoomHandles).forEach((function(e) {
+                                            return e()
+                                        })))
+                                    }), 300, this)
+                                }
+                            }
+                        }, {
                             key: "onHrefClick",
                             value: function(e) {
                                 if (e.ctrlKey && e.target.href && e.target.href.startsWith("javascript")) {
                                     e.preventDefault();
                                     var t = JSON.parse(e.target.href.split("runAction(")[1].slice(0, -1));
                                     Object.assign(t, {
                                         clickCatch: !0
@@ -1171,14 +1195,17 @@
                                 }) : react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     className: t,
                                     onClick: this.onWrapperClick,
                                     ref: function(t) {
                                         return e.topDiv = t
                                     }
                                 }, react__WEBPACK_IMPORTED_MODULE_0__.createElement(_AppTopbar__WEBPACK_IMPORTED_MODULE_11__.w, {
+                                    ref: function(t) {
+                                        return e.topBar = t
+                                    },
                                     onToggleMenu: this.onToggleMenu,
                                     onHomeButton: this.onHomeButton,
                                     WS: this.state.WS,
                                     useChat: this.state.user_settings && this.state.user_settings.logged_in && window.Lino && window.Lino.useChats,
                                     onChatButton: this.onChatButton
                                 }), react__WEBPACK_IMPORTED_MODULE_0__.createElement("div", {
                                     ref: function(t) {
@@ -1997,14 +2024,19 @@
                     function s() {
                         var e;
                         return function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                         }(this, s), (e = l.call(this)).renderChatButton = e.renderChatButton.bind(C(e)), e
                     }
                     return t = s, (n = [{
+                        key: "componentDidMount",
+                        value: function() {
+                            setTimeout(window.App.handleZoom, 1e3)
+                        }
+                    }, {
                         key: "renderChatButton",
                         value: function() {
                             return o.createElement("a", {
                                 onClick: this.props.onChatButton,
                                 ref: function(e) {
                                     return window.App.chatButton = e
                                 }
@@ -2015,14 +2047,17 @@
                             }))
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e;
                             return window.App.data.themeName, o.createElement("div", {
+                                ref: function(e) {
+                                    return window.App.tbContainer = e
+                                },
                                 className: "layout-topbar clearfix"
                             }, o.createElement("a", {
                                 className: "layout-menu-button",
                                 onClick: this.props.onToggleMenu
                             }, o.createElement("span", {
                                 className: "pi pi-bars"
                             })), o.createElement("a", {
@@ -3077,18 +3112,18 @@
                     runWrapper: function(e) {
                         return e()
                     },
                     disabledFields: {}
                 };
                 const __WEBPACK_DEFAULT_EXPORT__ = LinoBbar
             },
-            6149: (e, t, n) => {
+            6147: (e, t, n) => {
                 "use strict";
                 n.d(t, {
-                    Z: () => Ge
+                    Z: () => lt
                 });
                 var o = n(3379),
                     r = n.n(o),
                     i = n(5397);
                 r()(i.Z, {
                     insert: "head",
                     singleton: !1
@@ -3112,153 +3147,154 @@
                     k = n(3215),
                     x = n(9502),
                     E = n(1290),
                     O = n(7881),
                     C = n(7315),
                     S = (n(3723), n(9694), n(7204)),
                     D = (n(2494), n(8727)),
-                    P = n(4029);
+                    P = n(1008),
+                    R = n(4029);
 
-                function R() {
-                    return R = Object.assign || function(e) {
+                function I() {
+                    return I = Object.assign || function(e) {
                         for (var t = 1; t < arguments.length; t++) {
                             var n = arguments[t];
                             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
                         }
                         return e
-                    }, R.apply(this, arguments)
+                    }, I.apply(this, arguments)
                 }
 
-                function I(e, t) {
+                function T(e, t) {
                     var n = Object.keys(e);
                     if (Object.getOwnPropertySymbols) {
                         var o = Object.getOwnPropertySymbols(e);
                         t && (o = o.filter((function(t) {
                             return Object.getOwnPropertyDescriptor(e, t).enumerable
                         }))), n.push.apply(n, o)
                     }
                     return n
                 }
 
-                function T(e) {
+                function q(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? I(Object(n), !0).forEach((function(t) {
-                            q(e, t, n[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : I(Object(n)).forEach((function(t) {
+                        t % 2 ? T(Object(n), !0).forEach((function(t) {
+                            A(e, t, n[t])
+                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : T(Object(n)).forEach((function(t) {
                             Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                         }))
                     }
                     return e
                 }
 
-                function q(e, t, n) {
+                function A(e, t, n) {
                     return t in e ? Object.defineProperty(e, t, {
                         value: n,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
                     }) : e[t] = n, e
                 }
 
-                function A(e) {
-                    return A = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function M(e) {
+                    return M = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, A(e)
+                    }, M(e)
                 }
 
-                function M(e, t) {
+                function L(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }
 
-                function L(e, t) {
+                function j(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function j(e, t, n) {
-                    return t && L(e.prototype, t), n && L(e, n), Object.defineProperty(e, "prototype", {
+                function N(e, t, n) {
+                    return t && j(e.prototype, t), n && j(e, n), Object.defineProperty(e, "prototype", {
                         writable: !1
                     }), e
                 }
 
-                function N(e, t) {
+                function B(e, t) {
                     if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                     Object.defineProperty(e, "prototype", {
                         value: Object.create(t && t.prototype, {
                             constructor: {
                                 value: e,
                                 writable: !0,
                                 configurable: !0
                             }
                         }),
                         writable: !1
-                    }), t && B(e, t)
+                    }), t && F(e, t)
                 }
 
-                function B(e, t) {
-                    return B = Object.setPrototypeOf || function(e, t) {
+                function F(e, t) {
+                    return F = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, B(e, t)
+                    }, F(e, t)
                 }
 
-                function F(e) {
+                function z(e) {
                     var t = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }();
                     return function() {
-                        var n, o = K(e);
+                        var n, o = W(e);
                         if (t) {
-                            var r = K(this).constructor;
+                            var r = W(this).constructor;
                             n = Reflect.construct(o, arguments, r)
                         } else n = o.apply(this, arguments);
-                        return z(this, n)
+                        return U(this, n)
                     }
                 }
 
-                function z(e, t) {
-                    if (t && ("object" === A(t) || "function" == typeof t)) return t;
+                function U(e, t) {
+                    if (t && ("object" === M(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return U(e)
+                    return K(e)
                 }
 
-                function U(e) {
+                function K(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function K(e) {
-                    return K = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function W(e) {
+                    return W = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, K(e)
+                    }, W(e)
                 }
-                r()(P.Z, {
+                r()(R.Z, {
                     insert: "head",
                     singleton: !1
-                }), P.Z.locals;
-                var W = function(e) {
-                        N(n, e);
-                        var t = F(n);
+                }), R.Z.locals;
+                var H = function(e) {
+                        B(n, e);
+                        var t = z(n);
 
                         function n(e) {
                             var o;
-                            return M(this, n), (o = t.call(this, e)).state = {}, o.dragStart = o.dragStart.bind(U(o)), o.drop = o.drop.bind(U(o)), o
+                            return L(this, n), (o = t.call(this, e)).state = {}, o.dragStart = o.dragStart.bind(K(o)), o.drop = o.drop.bind(K(o)), o
                         }
-                        return j(n, [{
+                        return N(n, [{
                             key: "dragOver",
                             value: function(e) {
                                 e.preventDefault()
                             }
                         }, {
                             key: "dragStart",
                             value: function(e) {
@@ -3266,15 +3302,15 @@
                                 "A" === n.nodeName && (n = e.target.querySelector("div")), t = n.attributes.pk.value, e.dataTransfer.setData("pk", t)
                             }
                         }, {
                             key: "drop",
                             value: function(e) {
                                 var t = e.dataTransfer.getData("pk"),
                                     n = this.props.data.filter((function(e) {
-                                        return ![null, void 0].includes(e) && "object" === A(e) && e.meta
+                                        return ![null, void 0].includes(e) && "object" === M(e) && e.meta
                                     }))[0].calDates[this.props.column.col.fields_index];
                                 window.App.runAction({
                                     actorId: "cal.Events",
                                     an: "drag_drop",
                                     sr: [t],
                                     rp: window.Detail,
                                     status: {
@@ -3292,45 +3328,45 @@
                                     onDragOver: this.dragOver,
                                     onDragStart: this.dragStart,
                                     onDrop: this.drop
                                 }, this.props.children)
                             }
                         }]), n
                     }(a.Component),
-                    H = function(e) {
-                        N(n, e);
-                        var t = F(n);
+                    V = function(e) {
+                        B(n, e);
+                        var t = z(n);
 
                         function n(e) {
                             var o;
-                            return M(this, n), (o = t.call(this, e)).state = {
+                            return L(this, n), (o = t.call(this, e)).state = {
                                 toggle_col: !1
                             }, o.component = {}, o.data = {
                                 editingCellIndex: void 0,
                                 editingCol: void 0,
                                 editingPK: void 0,
                                 editingValues: {},
                                 query: "",
                                 rows: e.rows,
                                 ids: e.rows.map((function(t) {
                                     return t[e.actorData.pk_index]
                                 })),
                                 shiftIndex: null,
                                 sr: e.sr
-                            }, o.parent = e.parent, o.component.show_columns = e.show_columns, o.addColHeaderMouseOverEL = o.addColHeaderMouseOverEL.bind(U(o)), o.columnEditor = o.columnEditor.bind(U(o)), o.columnTemplate = o.columnTemplate.bind(U(o)), o.demandsFromChildren = o.demandsFromChildren.bind(U(o)), o.moveColHeaderTooltip = o.moveColHeaderTooltip.bind(U(o)), o.onBeforeEditorHide = o.onBeforeEditorHide.bind(U(o)), o.onBeforeEditorShow = o.onBeforeEditorShow.bind(U(o)), o.onCancel = o.onCancel.bind(U(o)), o.onColReorder = o.onColReorder.bind(U(o)), o.onEditorInit = o.onEditorInit.bind(U(o)), o.onKeyDown = o.onKeyDown.bind(U(o)), o.onSubmit = o.onSubmit.bind(U(o)), o.reload = o.reload.bind(U(o)), o.removeColHeaderMouseOverEL = o.removeColHeaderMouseOverEL.bind(U(o)), o.toggleOffColHeaderTooltip = o.toggleOffColHeaderTooltip.bind(U(o)), o.toggleOnColHeaderTooltip = o.toggleOnColHeaderTooltip.bind(U(o)), o.set_cols = o.set_cols.bind(U(o)), o.update_col_value = o.update_col_value.bind(U(o)), o.set_cols(), o
+                            }, o.parent = e.parent, o.component.show_columns = e.show_columns, o.addColHeaderMouseOverEL = o.addColHeaderMouseOverEL.bind(K(o)), o.columnEditor = o.columnEditor.bind(K(o)), o.columnTemplate = o.columnTemplate.bind(K(o)), o.demandsFromChildren = o.demandsFromChildren.bind(K(o)), o.maintainTableHeight = o.maintainTableHeight.bind(K(o)), o.moveColHeaderTooltip = o.moveColHeaderTooltip.bind(K(o)), o.onBeforeEditorHide = o.onBeforeEditorHide.bind(K(o)), o.onBeforeEditorShow = o.onBeforeEditorShow.bind(K(o)), o.onCancel = o.onCancel.bind(K(o)), o.onColReorder = o.onColReorder.bind(K(o)), o.onEditorInit = o.onEditorInit.bind(K(o)), o.onKeyDown = o.onKeyDown.bind(K(o)), o.onSubmit = o.onSubmit.bind(K(o)), o.reload = o.reload.bind(K(o)), o.removeColHeaderMouseOverEL = o.removeColHeaderMouseOverEL.bind(K(o)), o.toggleOffColHeaderTooltip = o.toggleOffColHeaderTooltip.bind(K(o)), o.toggleOnColHeaderTooltip = o.toggleOnColHeaderTooltip.bind(K(o)), o.set_cols = o.set_cols.bind(K(o)), o.update_col_value = o.update_col_value.bind(K(o)), o.set_cols(), o
                         }
-                        return j(n, [{
+                        return N(n, [{
                             key: "get_full_id",
                             value: function() {
                                 return "".concat(this.props.packId, ".").concat(this.props.actorId)
                             }
                         }, {
                             key: "componentDidMount",
                             value: function() {
-                                this.props.inDetail ? window.postMessage("GridMount", "*") : (window.addEventListener("keydown", this.onKeyDown), this.maintainTableHeight()), this.addColHeaderMouseOverEL()
+                                this.props.inDetail ? window.postMessage("GridMount", "*") : (window.addEventListener("keydown", this.onKeyDown), this.maintainTableHeight()), this.addColHeaderMouseOverEL(), window.App.registerZoomHandle("gridElement_maintainTableHeight", this.maintainTableHeight), console.log("cdm", window.App.data.zoomHandles)
                             }
                         }, {
                             key: "getSnapshotBeforeUpdate",
                             value: function(e, t) {
                                 var n = {};
                                 return this.props.reload_timestamp >= e.reload_timestamp && (p().isEqual(e.rows, this.props.rows) || (n.newValue = !0), p().isEqual(e.show_columns, this.props.show_columns) || (n.newColumns = !0)), Object.keys(n).length ? n : null
                             }
@@ -3352,15 +3388,15 @@
                                         loading: !1
                                     })
                                 }
                             }
                         }, {
                             key: "componentWillUnmount",
                             value: function() {
-                                this.props.inDetail || window.removeEventListener("keydown", this.onKeyDown), this.removeColHeaderMouseOverEL()
+                                this.props.inDetail || window.removeEventListener("keydown", this.onKeyDown), this.removeColHeaderMouseOverEL(), window.App.unregisterZoomHandle("gridElement_maintainTableHeight"), console.log("cwu", window.App.data.zoomHandles)
                             }
                         }, {
                             key: "addColHeaderMouseOverEL",
                             value: function() {
                                 var e = this;
                                 Array.from(document.querySelectorAll("th.l-grid-col")).forEach((function(t) {
                                     t.addEventListener("mouseenter", e.toggleOnColHeaderTooltip), t.addEventListener("mouseleave", e.toggleOffColHeaderTooltip), t.addEventListener("mousemove", e.moveColHeaderTooltip)
@@ -3396,16 +3432,30 @@
                             key: "moveColHeaderTooltip",
                             value: function(e) {
                                 this.data.chEl && (this.data.chEl.style.left = (e.x - 120).toString() + "px", this.data.chEl.style.top = (e.y + 25).toString() + "px")
                             }
                         }, {
                             key: "maintainTableHeight",
                             value: function() {
-                                var e, t, n, o = document.querySelector(".p-paginator.p-component");
-                                o && (e = document.querySelector(".p-datatable-scrollable-header").getBoundingClientRect().height, t = o.getBoundingClientRect().height, (n = window.innerHeight - document.querySelector(".l-grid").getBoundingClientRect().top - e - t) < 350 && (n = 300), document.querySelector(".p-datatable-scrollable-body").style.setProperty("max-height", n.toString() + "px"))
+                                var e = document.querySelector(".p-paginator.p-component");
+                                if (e) {
+                                    var t = this.dataTable.container.children[0].children[0],
+                                        n = e.getBoundingClientRect(),
+                                        o = window.innerHeight - n.bottom,
+                                        r = n.top - t.children[0].getBoundingClientRect().bottom + o;
+                                    r < 350 && (r = 300);
+                                    var i = t.children[1];
+                                    i.style.setProperty("max-height", r.toString() + "px"), o = window.innerHeight - e.getBoundingClientRect().bottom;
+                                    var a, l = i.scrollHeight / this.props.rows.length;
+                                    if (o >= l)(0, x.k_)(this.parent.props.router, (A(a = {}, P.qg, 0), A(a, P.EL, this.props.rows.length + Math.round(o / l)), a), !0);
+                                    else if (i.scrollHeight - i.clientHeight >= l) {
+                                        var s;
+                                        (0, x.k_)(this.parent.props.router, (A(s = {}, P.qg, 0), A(s, P.EL, Math.round(i.clientHeight / l)), s), !0)
+                                    }
+                                }
                             }
                         }, {
                             key: "reload",
                             value: function(e) {
                                 this.parent.setState({
                                     refresh: !0
                                 }), this.parent.refresh(e)
@@ -3433,20 +3483,20 @@
                             }
                         }, {
                             key: "onBeforeEditorShow",
                             value: function(e) {}
                         }, {
                             key: "onEditorInit",
                             value: function(e) {
-                                this.parent.data.editing_mode = !0, this.data.editorDirty = !1, this.data.editingCol = e, this.data.editingPK = e.columnProps.rowData[this.props.actorData.pk_index], this.data.editingValues = Object.assign({}, T({}, e.columnProps.rowData)), this.data.editingCellIndex = e.columnProps.cellIndex, void 0 !== this.data.roger && delete this.data.roger
+                                this.parent.data.editing_mode = !0, this.data.editorDirty = !1, this.data.editingCol = e, this.data.editingPK = e.columnProps.rowData[this.props.actorData.pk_index], this.data.editingValues = Object.assign({}, q({}, e.columnProps.rowData)), this.data.editingCellIndex = e.columnProps.cellIndex, void 0 !== this.data.roger && delete this.data.roger
                             }
                         }, {
                             key: "update_col_value",
                             value: function(e, t, n) {
-                                !this.data.editorDirty && (this.data.editorDirty = !0), this.data.editingValues = Object.assign({}, T({}, e)), this.data.editingCol = n
+                                !this.data.editorDirty && (this.data.editorDirty = !0), this.data.editingValues = Object.assign({}, q({}, e)), this.data.editingCol = n
                             }
                         }, {
                             key: "onSubmit",
                             value: function(e, t, n) {
                                 var o, r = this,
                                     i = e.columnProps,
                                     a = (i.rowData, i.field, i.rowIndex),
@@ -3537,15 +3587,15 @@
                                 }
                             }
                         }, {
                             key: "columnEditor",
                             value: function(e) {
                                 var t = this;
                                 if (this.props.actorData.editable && e.editable) return function(n) {
-                                    var o = T({
+                                    var o = q({
                                         actorId: t.get_full_id(),
                                         data: n.rowData,
                                         actorData: t.props.actorData,
                                         disabled_fields: t.props.disabled_fields || {},
                                         update_value: t.update_col_value,
                                         hide_label: !0,
                                         in_grid: !0,
@@ -3555,15 +3605,15 @@
                                         router: t.props.router,
                                         mk: t.props.mk,
                                         mt: t.props.mt,
                                         refresh: t.props.refresh
                                     }, t.data.roger);
                                     return a.createElement("div", {
                                         onKeyDown: t.onKeyDown
-                                    }, a.createElement(D.ZP, R({}, o, {
+                                    }, a.createElement(D.ZP, I({}, o, {
                                         elem: e
                                     })))
                                 }
                             }
                         }, {
                             key: "columnTemplate",
                             value: function(e) {
@@ -3605,27 +3655,27 @@
                                                 router: t.props.router,
                                                 container: t.dataTable && t.dataTable.table,
                                                 mk: t.props.mk,
                                                 mt: t.props.mt,
                                                 pass_roger: t.demandsFromChildren,
                                                 refresh: t.props.refresh
                                             },
-                                            c = a.createElement(D.ZP, R({}, u, {
+                                            c = a.createElement(D.ZP, I({}, u, {
                                                 elem: e
                                             }));
-                                        return o && (c = a.createElement(W, u, c)), a.createElement(a.Fragment, null, l, a.createElement("div", {
+                                        return o && (c = a.createElement(H, u, c)), a.createElement(a.Fragment, null, l, a.createElement("div", {
                                             style: n
                                         }, c))
                                     }
                             }
                         }, {
                             key: "rowClassName",
                             value: function(e) {
                                 var t = e.filter((function(e) {
-                                        return ![null, void 0].includes(e) && "object" === A(e) && e.meta
+                                        return ![null, void 0].includes(e) && "object" === M(e) && e.meta
                                     }))[0],
                                     n = {};
                                 if (t && t.hasOwnProperty("styleClass")) return n[t.styleClass] = !0, n
                             }
                         }, {
                             key: "set_cols",
                             value: function() {
@@ -3710,116 +3760,116 @@
                                     sortOrder: this.props.sortOrder,
                                     stripedRows: !0,
                                     value: this.data.rows
                                 }, this.component.columns))
                             }
                         }]), n
                     }(a.Component),
-                    V = n(1674),
-                    G = n(9898),
-                    Z = n(813);
+                    G = n(1674),
+                    Z = n(9898),
+                    Y = n(813);
 
-                function Y(e, t) {
+                function X(e, t) {
                     if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                 }
 
-                function X(e, t) {
+                function J(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function J(e, t, n) {
-                    return t && X(e.prototype, t), n && X(e, n), e
+                function Q(e, t, n) {
+                    return t && J(e.prototype, t), n && J(e, n), e
                 }
 
-                function Q(e) {
+                function $(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function $(e, t) {
-                    return $ = Object.setPrototypeOf || function(e, t) {
+                function ee(e, t) {
+                    return ee = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, $(e, t)
+                    }, ee(e, t)
                 }
 
-                function ee(e, t) {
+                function te(e, t) {
                     if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                     e.prototype = Object.create(t && t.prototype, {
                         constructor: {
                             value: e,
                             writable: !0,
                             configurable: !0
                         }
-                    }), t && $(e, t)
+                    }), t && ee(e, t)
                 }
 
-                function te(e) {
-                    return te = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function ne(e) {
+                    return ne = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, te(e)
+                    }, ne(e)
                 }
 
-                function ne(e, t) {
-                    return !t || "object" !== te(t) && "function" != typeof t ? Q(e) : t
+                function oe(e, t) {
+                    return !t || "object" !== ne(t) && "function" != typeof t ? $(e) : t
                 }
 
-                function oe(e) {
-                    return oe = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function re(e) {
+                    return re = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, oe(e)
+                    }, re(e)
                 }
 
-                function re(e, t, n) {
+                function ie(e, t, n) {
                     return t in e ? Object.defineProperty(e, t, {
                         value: n,
                         enumerable: !0,
                         configurable: !0,
                         writable: !0
                     }) : e[t] = n, e
                 }
 
-                function ie() {
-                    return ie = Object.assign || function(e) {
+                function ae() {
+                    return ae = Object.assign || function(e) {
                         for (var t = 1; t < arguments.length; t++) {
                             var n = arguments[t];
                             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
                         }
                         return e
-                    }, ie.apply(this, arguments)
+                    }, ae.apply(this, arguments)
                 }
-                var ae = function(e) {
-                        ee(r, e);
+                var le = function(e) {
+                        te(r, e);
                         var t, n, o = (t = r, n = function() {
                             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                             if (Reflect.construct.sham) return !1;
                             if ("function" == typeof Proxy) return !0;
                             try {
                                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                             } catch (e) {
                                 return !1
                             }
                         }(), function() {
-                            var e, o = oe(t);
+                            var e, o = re(t);
                             if (n) {
-                                var r = oe(this).constructor;
+                                var r = re(this).constructor;
                                 e = Reflect.construct(o, arguments, r)
                             } else e = o.apply(this, arguments);
-                            return ne(this, e)
+                            return oe(this, e)
                         });
 
                         function r(e) {
                             var t;
-                            return Y(this, r), (t = o.call(this, e)).navForward = t.navForward.bind(Q(t)), t.navBackward = t.navBackward.bind(Q(t)), t.next = t.next.bind(Q(t)), t.prev = t.prev.bind(Q(t)), t
+                            return X(this, r), (t = o.call(this, e)).navForward = t.navForward.bind($(t)), t.navBackward = t.navBackward.bind($(t)), t.next = t.next.bind($(t)), t.prev = t.prev.bind($(t)), t
                         }
-                        return J(r, [{
+                        return Q(r, [{
                             key: "step",
                             value: function(e) {
                                 this.itemsContainer && (this.itemsContainer.style.transform = this.isVertical() ? "translate3d(0, ".concat(100 * e, "%, 0)") : "translate3d(".concat(100 * e, "%, 0, 0)"), this.itemsContainer.style.transition = "transform 500ms ease 0s")
                             }
                         }, {
                             key: "next",
                             value: function() {
@@ -3878,44 +3928,44 @@
                                 this.props.autoPlay && this.props.startSlideShow()
                             }
                         }, {
                             key: "renderBackwardNavigator",
                             value: function() {
                                 if (this.props.showItemNavigators) {
                                     var e = !this.props.circular && 0 === this.props.activeItemIndex,
-                                        t = (0, Z.AK)("p-galleria-item-prev p-galleria-item-nav p-link", {
+                                        t = (0, Y.AK)("p-galleria-item-prev p-galleria-item-nav p-link", {
                                             "p-disabled": e
                                         });
                                     return a.createElement("button", {
                                         type: "button",
                                         className: t,
                                         onClick: this.navBackward,
                                         disabled: e
                                     }, a.createElement("span", {
                                         className: "p-galleria-item-prev-icon pi pi-chevron-left"
-                                    }), a.createElement(Z.HW, null))
+                                    }), a.createElement(Y.HW, null))
                                 }
                                 return null
                             }
                         }, {
                             key: "renderForwardNavigator",
                             value: function() {
                                 if (this.props.showItemNavigators) {
                                     var e = !this.props.circular && this.props.activeItemIndex === this.props.value.length - 1,
-                                        t = (0, Z.AK)("p-galleria-item-next p-galleria-item-nav p-link", {
+                                        t = (0, Y.AK)("p-galleria-item-next p-galleria-item-nav p-link", {
                                             "p-disabled": e
                                         });
                                     return a.createElement("button", {
                                         type: "button",
                                         className: t,
                                         onClick: this.navForward,
                                         disabled: e
                                     }, a.createElement("span", {
                                         className: "p-galleria-item-next-icon pi pi-chevron-right"
-                                    }), a.createElement(Z.HW, null))
+                                    }), a.createElement(Y.HW, null))
                                 }
                                 return null
                             }
                         }, {
                             key: "renderCaption",
                             value: function() {
                                 if (this.props.caption) {
@@ -3928,22 +3978,22 @@
                             }
                         }, {
                             key: "renderIndicator",
                             value: function(e) {
                                 var t = this,
                                     n = this.props.indicator && this.props.indicator(e),
                                     o = this.props.activeItemIndex === e,
-                                    r = (0, Z.AK)("p-galleria-indicator", {
+                                    r = (0, Y.AK)("p-galleria-indicator", {
                                         "p-highlight": o
                                     });
                                 return n || (n = a.createElement("button", {
                                     type: "button",
                                     tabIndex: -1,
                                     className: "p-link"
-                                }, a.createElement(Z.HW, null))), a.createElement("li", {
+                                }, a.createElement(Y.HW, null))), a.createElement("li", {
                                     className: r,
                                     key: "p-galleria-indicator-" + e,
                                     tabIndex: 0,
                                     onClick: function() {
                                         return t.onIndicatorClick(e)
                                     },
                                     onMouseEnter: function() {
@@ -3954,15 +4004,15 @@
                                     }
                                 }, n)
                             }
                         }, {
                             key: "renderIndicators",
                             value: function() {
                                 if (this.props.showIndicators) {
-                                    for (var e = (0, Z.AK)("p-galleria-indicators p-reset", this.props.indicatorsContentClassName), t = [], n = 0; n < this.props.value.length; n++) t.push(this.renderIndicator(n));
+                                    for (var e = (0, Y.AK)("p-galleria-indicators p-reset", this.props.indicatorsContentClassName), t = [], n = 0; n < this.props.value.length; n++) t.push(this.renderIndicator(n));
                                     return a.createElement("ul", {
                                         className: e
                                     }, t)
                                 }
                                 return null
                             }
                         }, {
@@ -3983,55 +4033,55 @@
                                     className: "p-galleria-item-container"
                                 }, n, a.createElement("div", {
                                     className: "p-galleria-item"
                                 }, t), o, r), i)
                             }
                         }]), r
                     }(a.Component),
-                    le = a.forwardRef((function(e, t) {
-                        return a.createElement(ae, ie({
+                    se = a.forwardRef((function(e, t) {
+                        return a.createElement(le, ae({
                             forwardRef: t
                         }, e))
                     }));
 
-                function se(e, t) {
+                function pe(e, t) {
                     (null == t || t > e.length) && (t = e.length);
                     for (var n = 0, o = new Array(t); n < t; n++) o[n] = e[n];
                     return o
                 }
 
-                function pe(e) {
+                function ue(e) {
                     var t = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }();
                     return function() {
-                        var n, o = oe(e);
+                        var n, o = re(e);
                         if (t) {
-                            var r = oe(this).constructor;
+                            var r = re(this).constructor;
                             n = Reflect.construct(o, arguments, r)
                         } else n = o.apply(this, arguments);
-                        return ne(this, n)
+                        return oe(this, n)
                     }
                 }
-                var ue = function(e) {
-                    ee(n, e);
-                    var t = pe(n);
+                var ce = function(e) {
+                    te(n, e);
+                    var t = ue(n);
 
                     function n(e) {
                         var o;
-                        return Y(this, n), (o = t.call(this, e)).onItemClick = o.onItemClick.bind(Q(o)), o.onItemKeyDown = o.onItemKeyDown.bind(Q(o)), o
+                        return X(this, n), (o = t.call(this, e)).onItemClick = o.onItemClick.bind($(o)), o.onItemKeyDown = o.onItemKeyDown.bind($(o)), o
                     }
-                    return J(n, [{
+                    return Q(n, [{
                         key: "onItemClick",
                         value: function(e) {
                             this.props.onItemClick({
                                 originalEvent: e,
                                 index: this.props.index
                             })
                         }
@@ -4043,15 +4093,15 @@
                                 index: this.props.index
                             })
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this.props.template && this.props.template(this.props.item),
-                                t = (0, Z.AK)(this.props.className, "p-galleria-thumbnail-item", {
+                                t = (0, Y.AK)(this.props.className, "p-galleria-thumbnail-item", {
                                     "p-galleria-thumbnail-item-current": this.props.current,
                                     "p-galleria-thumbnail-item-active": this.props.active,
                                     "p-galleria-thumbnail-item-start": this.props.start,
                                     "p-galleria-thumbnail-item-end": this.props.end
                                 });
                             return a.createElement("div", {
                                 className: t
@@ -4060,42 +4110,42 @@
                                 tabIndex: this.props.active ? 0 : null,
                                 onClick: this.onItemClick,
                                 onKeyDown: this.onItemKeyDown
                             }, e))
                         }
                     }]), n
                 }(a.Component);
-                re(ue, "defaultProps", {
+                ie(ce, "defaultProps", {
                     index: null,
                     template: null,
                     item: null,
                     current: !1,
                     active: !1,
                     start: !1,
                     end: !1,
                     className: null,
                     onItemClick: null
                 });
-                var ce = function(e) {
-                    ee(n, e);
-                    var t = pe(n);
+                var de = function(e) {
+                    te(n, e);
+                    var t = ue(n);
 
                     function n(e) {
                         var o;
-                        return Y(this, n), (o = t.call(this, e)).state = {
+                        return X(this, n), (o = t.call(this, e)).state = {
                             numVisible: e.numVisible,
                             totalShiftedItems: 0,
                             page: 0
-                        }, o.navForward = o.navForward.bind(Q(o)), o.navBackward = o.navBackward.bind(Q(o)), o.onTransitionEnd = o.onTransitionEnd.bind(Q(o)), o.onTouchStart = o.onTouchStart.bind(Q(o)), o.onTouchMove = o.onTouchMove.bind(Q(o)), o.onTouchEnd = o.onTouchEnd.bind(Q(o)), o.onItemClick = o.onItemClick.bind(Q(o)), o.attributeSelector = (0, Z.Th)(), o
+                        }, o.navForward = o.navForward.bind($(o)), o.navBackward = o.navBackward.bind($(o)), o.onTransitionEnd = o.onTransitionEnd.bind($(o)), o.onTouchStart = o.onTouchStart.bind($(o)), o.onTouchMove = o.onTouchMove.bind($(o)), o.onTouchEnd = o.onTouchEnd.bind($(o)), o.onItemClick = o.onItemClick.bind($(o)), o.attributeSelector = (0, Y.Th)(), o
                     }
-                    return J(n, [{
+                    return Q(n, [{
                         key: "step",
                         value: function(e) {
                             var t = this.state.totalShiftedItems + e;
-                            e < 0 && -1 * t + this.state.numVisible > this.props.value.length - 1 ? t = this.state.numVisible - this.props.value.length : e > 0 && t > 0 && (t = 0), this.props.circular && (e < 0 && this.props.value.length - 1 === this.props.activeItemIndex ? t = 0 : e > 0 && 0 === this.props.activeItemIndex && (t = this.state.numVisible - this.props.value.length)), this.itemsContainer && (Z.p7.removeClass(this.itemsContainer, "p-items-hidden"), this.itemsContainer.style.transform = this.props.isVertical ? "translate3d(0, ".concat(t * (100 / this.state.numVisible), "%, 0)") : "translate3d(".concat(t * (100 / this.state.numVisible), "%, 0, 0)"), this.itemsContainer.style.transition = "transform 500ms ease 0s"), this.setState({
+                            e < 0 && -1 * t + this.state.numVisible > this.props.value.length - 1 ? t = this.state.numVisible - this.props.value.length : e > 0 && t > 0 && (t = 0), this.props.circular && (e < 0 && this.props.value.length - 1 === this.props.activeItemIndex ? t = 0 : e > 0 && 0 === this.props.activeItemIndex && (t = this.state.numVisible - this.props.value.length)), this.itemsContainer && (Y.p7.removeClass(this.itemsContainer, "p-items-hidden"), this.itemsContainer.style.transform = this.props.isVertical ? "translate3d(0, ".concat(t * (100 / this.state.numVisible), "%, 0)") : "translate3d(".concat(t * (100 / this.state.numVisible), "%, 0, 0)"), this.itemsContainer.style.transition = "transform 500ms ease 0s"), this.setState({
                                 totalShiftedItems: t
                             })
                         }
                     }, {
                         key: "stopSlideShow",
                         value: function() {
                             this.props.slideShowActive && this.props.stopSlideShow && this.props.stopSlideShow()
@@ -4137,15 +4187,15 @@
                                     index: t
                                 })
                             }
                         }
                     }, {
                         key: "onTransitionEnd",
                         value: function(e) {
-                            this.itemsContainer && "transform" === e.propertyName && (Z.p7.addClass(this.itemsContainer, "p-items-hidden"), this.itemsContainer.style.transition = "")
+                            this.itemsContainer && "transform" === e.propertyName && (Y.p7.addClass(this.itemsContainer, "p-items-hidden"), this.itemsContainer.style.transition = "")
                         }
                     }, {
                         key: "onTouchStart",
                         value: function(e) {
                             var t = e.changedTouches[0];
                             this.startPos = {
                                 x: t.pageX,
@@ -4176,22 +4226,22 @@
                     }, {
                         key: "createStyle",
                         value: function() {
                             this.thumbnailsStyle || (this.thumbnailsStyle = document.createElement("style"), document.body.appendChild(this.thumbnailsStyle));
                             var e, t = "\n            .p-galleria-thumbnail-items[".concat(this.attributeSelector, "] .p-galleria-thumbnail-item {\n                flex: 1 0 ").concat(100 / this.state.numVisible, "%\n            }\n        ");
                             if (this.props.responsiveOptions) {
                                 this.responsiveOptions = function(e) {
-                                    if (Array.isArray(e)) return se(e)
+                                    if (Array.isArray(e)) return pe(e)
                                 }(e = this.props.responsiveOptions) || function(e) {
                                     if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
                                 }(e) || function(e, t) {
                                     if (e) {
-                                        if ("string" == typeof e) return se(e, t);
+                                        if ("string" == typeof e) return pe(e, t);
                                         var n = Object.prototype.toString.call(e).slice(8, -1);
-                                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? se(e, t) : void 0
+                                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? pe(e, t) : void 0
                                     }
                                 }(e) || function() {
                                     throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
                                 }(), this.responsiveOptions.sort((function(e, t) {
                                     var n = e.breakpoint,
                                         o = t.breakpoint;
                                     return -1 * (null == n && null != o ? -1 : null != n && null == o ? 1 : null == n && null == o ? 0 : "string" == typeof n && "string" == typeof o ? n.localeCompare(o, void 0, {
@@ -4240,15 +4290,15 @@
                         }
                     }, {
                         key: "componentDidUpdate",
                         value: function(e, t) {
                             var n = this.state.totalShiftedItems;
                             t.numVisible === this.state.numVisible && e.activeItemIndex === this.props.activeItemIndex || ((n = this.props.activeItemIndex <= this.getMedianItemIndex() ? 0 : this.props.value.length - this.state.numVisible + this.getMedianItemIndex() < this.props.activeItemIndex ? this.state.numVisible - this.props.value.length : this.props.value.length - this.state.numVisible < this.props.activeItemIndex && this.state.numVisible % 2 == 0 ? -1 * this.props.activeItemIndex + this.getMedianItemIndex() + 1 : -1 * this.props.activeItemIndex + this.getMedianItemIndex()) !== this.state.totalShiftedItems && this.setState({
                                 totalShiftedItems: n
-                            }), this.itemsContainer.style.transform = this.props.isVertical ? "translate3d(0, ".concat(n * (100 / this.state.numVisible), "%, 0)") : "translate3d(".concat(n * (100 / this.state.numVisible), "%, 0, 0)"), e.activeItemIndex !== this.props.activeItemIndex && (Z.p7.removeClass(this.itemsContainer, "p-items-hidden"), this.itemsContainer.style.transition = "transform 500ms ease 0s"))
+                            }), this.itemsContainer.style.transform = this.props.isVertical ? "translate3d(0, ".concat(n * (100 / this.state.numVisible), "%, 0)") : "translate3d(".concat(n * (100 / this.state.numVisible), "%, 0, 0)"), e.activeItemIndex !== this.props.activeItemIndex && (Y.p7.removeClass(this.itemsContainer, "p-items-hidden"), this.itemsContainer.style.transition = "transform 500ms ease 0s"))
                         }
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             this.props.responsiveOptions && this.unbindDocumentListeners()
                         }
                     }, {
@@ -4258,15 +4308,15 @@
                             return this.props.value.map((function(t, n) {
                                 var o = -1 * e.state.totalShiftedItems,
                                     r = o + e.state.numVisible - 1,
                                     i = o <= n && r >= n,
                                     l = o === n,
                                     s = r === n,
                                     p = e.props.activeItemIndex === n;
-                                return a.createElement(ue, {
+                                return a.createElement(ce, {
                                     key: n,
                                     index: n,
                                     template: e.props.itemTemplate,
                                     item: t,
                                     active: i,
                                     start: l,
                                     end: s,
@@ -4276,50 +4326,50 @@
                             }))
                         }
                     }, {
                         key: "renderBackwardNavigator",
                         value: function() {
                             if (this.props.showThumbnailNavigators) {
                                 var e = !this.props.circular && 0 === this.props.activeItemIndex || this.props.value.length <= this.state.numVisible,
-                                    t = (0, Z.AK)("p-galleria-thumbnail-prev p-link", {
+                                    t = (0, Y.AK)("p-galleria-thumbnail-prev p-link", {
                                         "p-disabled": e
                                     }),
-                                    n = (0, Z.AK)("p-galleria-thumbnail-prev-icon pi", {
+                                    n = (0, Y.AK)("p-galleria-thumbnail-prev-icon pi", {
                                         "pi-chevron-left": !this.props.isVertical,
                                         "pi-chevron-up": this.props.isVertical
                                     });
                                 return a.createElement("button", {
                                     className: t,
                                     onClick: this.navBackward,
                                     disabled: e
                                 }, a.createElement("span", {
                                     className: n
-                                }), a.createElement(Z.HW, null))
+                                }), a.createElement(Y.HW, null))
                             }
                             return null
                         }
                     }, {
                         key: "renderForwardNavigator",
                         value: function() {
                             if (this.props.showThumbnailNavigators) {
                                 var e = !this.props.circular && this.props.activeItemIndex === this.props.value.length - 1 || this.props.value.length <= this.state.numVisible,
-                                    t = (0, Z.AK)("p-galleria-thumbnail-next p-link", {
+                                    t = (0, Y.AK)("p-galleria-thumbnail-next p-link", {
                                         "p-disabled": e
                                     }),
-                                    n = (0, Z.AK)("p-galleria-thumbnail-next-icon pi", {
+                                    n = (0, Y.AK)("p-galleria-thumbnail-next-icon pi", {
                                         "pi-chevron-right": !this.props.isVertical,
                                         "pi-chevron-down": this.props.isVertical
                                     });
                                 return a.createElement("button", {
                                     className: t,
                                     onClick: this.navForward,
                                     disabled: e
                                 }, a.createElement("span", {
                                     className: n
-                                }), a.createElement(Z.HW, null))
+                                }), a.createElement(Y.HW, null))
                             }
                             return null
                         }
                     }, {
                         key: "renderContent",
                         value: function() {
                             var e = this,
@@ -4352,67 +4402,67 @@
                             return a.createElement("div", {
                                 className: "p-galleria-thumbnail-wrapper"
                             }, e)
                         }
                     }]), n
                 }(a.Component);
 
-                function de(e, t) {
+                function fe(e, t) {
                     var n = Object.keys(e);
                     if (Object.getOwnPropertySymbols) {
                         var o = Object.getOwnPropertySymbols(e);
                         t && (o = o.filter((function(t) {
                             return Object.getOwnPropertyDescriptor(e, t).enumerable
                         }))), n.push.apply(n, o)
                     }
                     return n
                 }
 
-                function fe(e) {
+                function he(e) {
                     for (var t = 1; t < arguments.length; t++) {
                         var n = null != arguments[t] ? arguments[t] : {};
-                        t % 2 ? de(Object(n), !0).forEach((function(t) {
-                            re(e, t, n[t])
-                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : de(Object(n)).forEach((function(t) {
+                        t % 2 ? fe(Object(n), !0).forEach((function(t) {
+                            ie(e, t, n[t])
+                        })) : Object.getOwnPropertyDescriptors ? Object.defineProperties(e, Object.getOwnPropertyDescriptors(n)) : fe(Object(n)).forEach((function(t) {
                             Object.defineProperty(e, t, Object.getOwnPropertyDescriptor(n, t))
                         }))
                     }
                     return e
                 }
-                var he = function(e) {
-                    ee(r, e);
+                var me = function(e) {
+                    te(r, e);
                     var t, n, o = (t = r, n = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, o = oe(t);
+                        var e, o = re(t);
                         if (n) {
-                            var r = oe(this).constructor;
+                            var r = re(this).constructor;
                             e = Reflect.construct(o, arguments, r)
                         } else e = o.apply(this, arguments);
-                        return ne(this, e)
+                        return oe(this, e)
                     });
 
                     function r(e) {
                         var t;
-                        return Y(this, r), (t = o.call(this, e)).state = {
+                        return X(this, r), (t = o.call(this, e)).state = {
                             visible: !1,
                             numVisible: e.numVisible,
                             slideShowActive: !1
-                        }, t.props.onItemChange || (t.state = fe(fe({}, t.state), {}, {
+                        }, t.props.onItemChange || (t.state = he(he({}, t.state), {}, {
                             activeIndex: e.activeIndex
-                        })), t.onActiveItemChange = t.onActiveItemChange.bind(Q(t)), t.show = t.show.bind(Q(t)), t.hide = t.hide.bind(Q(t)), t.startSlideShow = t.startSlideShow.bind(Q(t)), t.stopSlideShow = t.stopSlideShow.bind(Q(t)), t.onEnter = t.onEnter.bind(Q(t)), t.onEntering = t.onEntering.bind(Q(t)), t.onEntered = t.onEntered.bind(Q(t)), t.onExit = t.onExit.bind(Q(t)), t.onExited = t.onExited.bind(Q(t)), t.galleriaRef = a.createRef(), t
+                        })), t.onActiveItemChange = t.onActiveItemChange.bind($(t)), t.show = t.show.bind($(t)), t.hide = t.hide.bind($(t)), t.startSlideShow = t.startSlideShow.bind($(t)), t.stopSlideShow = t.stopSlideShow.bind($(t)), t.onEnter = t.onEnter.bind($(t)), t.onEntering = t.onEntering.bind($(t)), t.onEntered = t.onEntered.bind($(t)), t.onExit = t.onExit.bind($(t)), t.onExited = t.onExited.bind($(t)), t.galleriaRef = a.createRef(), t
                     }
-                    return J(r, [{
+                    return Q(r, [{
                         key: "activeItemIndex",
                         get: function() {
                             return this.props.onItemChange ? this.props.activeIndex : this.state.activeIndex
                         }
                     }, {
                         key: "onActiveItemChange",
                         value: function(e) {
@@ -4433,35 +4483,35 @@
                             this.setState({
                                 visible: !1
                             })
                         }
                     }, {
                         key: "onEnter",
                         value: function() {
-                            Z.p7.addClass(document.body, "p-overflow-hidden")
+                            Y.p7.addClass(document.body, "p-overflow-hidden")
                         }
                     }, {
                         key: "onEntering",
                         value: function() {
-                            Z.P9.set("modal", this.mask, this.props.baseZIndex), Z.p7.addMultipleClasses(this.mask, "p-component-overlay p-component-overlay-enter")
+                            Y.P9.set("modal", this.mask, this.props.baseZIndex), Y.p7.addMultipleClasses(this.mask, "p-component-overlay p-component-overlay-enter")
                         }
                     }, {
                         key: "onEntered",
                         value: function() {
                             this.props.onShow && this.props.onShow()
                         }
                     }, {
                         key: "onExit",
                         value: function() {
-                            Z.p7.removeClass(document.body, "p-overflow-hidden"), Z.p7.addClass(this.mask, "p-component-overlay-leave")
+                            Y.p7.removeClass(document.body, "p-overflow-hidden"), Y.p7.addClass(this.mask, "p-component-overlay-leave")
                         }
                     }, {
                         key: "onExited",
                         value: function() {
-                            Z.P9.clear(this.mask), this.props.onHide && this.props.onHide()
+                            Y.P9.clear(this.mask), this.props.onHide && this.props.onHide()
                         }
                     }, {
                         key: "isAutoPlayActive",
                         value: function() {
                             return this.state.slideShowActive
                         }
                     }, {
@@ -4505,15 +4555,15 @@
                             }), e.numVisible !== this.props.numVisible && this.setState({
                                 numVisible: this.props.numVisible
                             })
                         }
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
-                            this.state.slideShowActive && this.stopSlideShow(), Z.P9.clear(this.mask)
+                            this.state.slideShowActive && this.stopSlideShow(), Y.P9.clear(this.mask)
                         }
                     }, {
                         key: "renderHeader",
                         value: function() {
                             return this.props.header ? a.createElement("div", {
                                 className: "p-galleria-header"
                             }, this.props.header) : null
@@ -4528,36 +4578,36 @@
                     }, {
                         key: "renderElement",
                         value: function() {
                             var e = this,
                                 t = this.isVertical(),
                                 n = this.props.showThumbnails && this.getPositionClassName("p-galleria-thumbnails", this.props.thumbnailsPosition),
                                 o = this.props.showIndicators && this.getPositionClassName("p-galleria-indicators", this.props.indicatorsPosition),
-                                r = (0, Z.AK)("p-galleria p-component", this.props.className, {
+                                r = (0, Y.AK)("p-galleria p-component", this.props.className, {
                                     "p-galleria-fullscreen": this.props.fullScreen,
                                     "p-galleria-indicator-onitem": this.props.showIndicatorsOnItem,
                                     "p-galleria-item-nav-onhover": this.props.showItemNavigatorsOnHover && !this.props.fullScreen
                                 }, n, o),
                                 i = this.props.fullScreen && a.createElement("button", {
                                     type: "button",
                                     className: "p-galleria-close p-link",
                                     onClick: this.hide
                                 }, a.createElement("span", {
                                     className: "p-galleria-close-icon pi pi-times"
-                                }), a.createElement(Z.HW, null)),
+                                }), a.createElement(Y.HW, null)),
                                 l = this.renderHeader(),
                                 s = this.renderFooter();
                             return a.createElement("div", {
                                 ref: this.galleriaRef,
                                 id: this.props.id,
                                 className: r,
                                 style: this.props.style
                             }, i, l, a.createElement("div", {
                                 className: "p-galleria-content"
-                            }, a.createElement(le, {
+                            }, a.createElement(se, {
                                 ref: function(t) {
                                     return e.previewContent = t
                                 },
                                 value: this.props.value,
                                 activeItemIndex: this.activeItemIndex,
                                 onActiveItemChange: this.onActiveItemChange,
                                 itemTemplate: this.props.item,
@@ -4567,15 +4617,15 @@
                                 changeItemOnIndicatorHover: this.props.changeItemOnIndicatorHover,
                                 indicator: this.props.indicator,
                                 showItemNavigators: this.props.showItemNavigators,
                                 autoPlay: this.props.autoPlay,
                                 slideShowActive: this.state.slideShowActive,
                                 startSlideShow: this.startSlideShow,
                                 stopSlideShow: this.stopSlideShow
-                            }), this.props.showThumbnails && a.createElement(ce, {
+                            }), this.props.showThumbnails && a.createElement(de, {
                                 value: this.props.value,
                                 activeItemIndex: this.activeItemIndex,
                                 onActiveItemChange: this.onActiveItemChange,
                                 itemTemplate: this.props.thumbnail,
                                 numVisible: this.state.numVisible,
                                 responsiveOptions: this.props.responsiveOptions,
                                 circular: this.props.circular,
@@ -4589,23 +4639,23 @@
                         }
                     }, {
                         key: "renderGalleria",
                         value: function() {
                             var e = this,
                                 t = this.renderElement();
                             if (this.props.fullScreen) {
-                                var n = (0, Z.AK)("p-galleria-mask", {
+                                var n = (0, Y.AK)("p-galleria-mask", {
                                         "p-galleria-visible": this.state.visible
                                     }),
                                     o = a.createElement("div", {
                                         ref: function(t) {
                                             return e.mask = t
                                         },
                                         className: n
-                                    }, a.createElement(Z.Kv, {
+                                    }, a.createElement(Y.Kv, {
                                         nodeRef: this.galleriaRef,
                                         classNames: "p-galleria",
                                         in: this.state.visible,
                                         timeout: {
                                             enter: 150,
                                             exit: 150
                                         },
@@ -4613,28 +4663,28 @@
                                         unmountOnExit: !0,
                                         onEnter: this.onEnter,
                                         onEntering: this.onEntering,
                                         onEntered: this.onEntered,
                                         onExit: this.onExit,
                                         onExited: this.onExited
                                     }, t));
-                                return a.createElement(Z.h_, {
+                                return a.createElement(Y.h_, {
                                     element: o
                                 })
                             }
                             return t
                         }
                     }, {
                         key: "render",
                         value: function() {
                             return this.props.value && this.props.value.length > 0 && this.renderGalleria()
                         }
                     }]), r
                 }(a.Component);
-                re(he, "defaultProps", {
+                ie(me, "defaultProps", {
                     id: null,
                     value: null,
                     activeIndex: 0,
                     fullScreen: !1,
                     item: null,
                     thumbnail: null,
                     indicator: null,
@@ -4658,16 +4708,15 @@
                     showIndicators: !1,
                     showIndicatorsOnItem: !1,
                     indicatorsPosition: "bottom",
                     baseZIndex: 0,
                     transitionOptions: null,
                     onItemChange: null
                 }), n(5692);
-                var me = n(1008),
-                    be = n(2289);
+                var be = n(2289);
 
                 function ge(e) {
                     return ge = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
                     }, ge(e)
@@ -4797,28 +4846,28 @@
                                 }) : a.createElement("p", null, e.card_title, " ", a.createElement("span", {
                                     className: "l-span-clickable",
                                     onClick: function(t) {
                                         n.parent.onRowDoubleClick(t, e.id)
                                     }
                                 }, a.createElement("i", {
                                     className: "pi pi-link"
-                                }))), a.createElement(V.Z, {
+                                }))), a.createElement(G.Z, {
                                     title: r,
                                     style: {
                                         margin: "20px"
                                     }
                                 }, o)
                             }
                         }, {
                             key: "render",
                             value: function() {
                                 var e = this;
-                                return this.parent.state.layout === me.dI ? a.createElement("div", {
+                                return this.parent.state.layout === P.dI ? a.createElement("div", {
                                     className: "card l-gallery"
-                                }, a.createElement(he, {
+                                }, a.createElement(me, {
                                     activeIndex: this.state.activeIndex,
                                     circular: !0,
                                     fullScreen: !0,
                                     item: this.imageTemplate,
                                     onItemChange: function(t) {
                                         return e.setState({
                                             activeIndex: t.index
@@ -4876,204 +4925,577 @@
                                                 activeIndex: n
                                             }, (function() {
                                                 return e.galleria.show()
                                             }))
                                         },
                                         src: t.image_src
                                     }))
-                                })))) : a.createElement(G.V, {
+                                })))) : a.createElement(Z.V, {
                                     value: this.parent.data.rows,
                                     layout: this.parent.state.layout,
                                     lazy: !0,
                                     itemTemplate: this.itemTemplate,
                                     itemKey: function(t, n) {
                                         return e.parent.data.rows[n].id
                                     }
                                 })
                             }
                         }]) && ve(t.prototype, n), Object.defineProperty(t, "prototype", {
                             writable: !1
                         }), l
                     }(a.Component),
-                    Ee = n(3504);
+                    Ee = n(3504),
+                    Oe = n(1868);
 
-                function Oe(e) {
-                    return Oe = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function Ce(e, t) {
+                    (null == t || t > e.length) && (t = e.length);
+                    for (var n = 0, o = new Array(t); n < t; n++) o[n] = e[n];
+                    return o
+                }
+
+                function Se(e, t) {
+                    for (var n = 0; n < t.length; n++) {
+                        var o = t[n];
+                        o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
+                    }
+                }
+
+                function De(e) {
+                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                    return e
+                }
+
+                function Pe(e, t) {
+                    return Pe = Object.setPrototypeOf || function(e, t) {
+                        return e.__proto__ = t, e
+                    }, Pe(e, t)
+                }
+
+                function Re(e) {
+                    return Re = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, Oe(e)
+                    }, Re(e)
                 }
 
-                function Ce(e, t) {
+                function Ie(e, t) {
+                    return !t || "object" !== Re(t) && "function" != typeof t ? De(e) : t
+                }
+
+                function Te(e) {
+                    return Te = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                        return e.__proto__ || Object.getPrototypeOf(e)
+                    }, Te(e)
+                }
+                var qe, Ae, Me, Le = function(e) {
+                    ! function(e, t) {
+                        if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
+                        e.prototype = Object.create(t && t.prototype, {
+                            constructor: {
+                                value: e,
+                                writable: !0,
+                                configurable: !0
+                            }
+                        }), t && Pe(e, t)
+                    }(l, e);
+                    var t, n, o, r, i = (o = l, r = function() {
+                        if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
+                        if (Reflect.construct.sham) return !1;
+                        if ("function" == typeof Proxy) return !0;
+                        try {
+                            return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
+                        } catch (e) {
+                            return !1
+                        }
+                    }(), function() {
+                        var e, t = Te(o);
+                        if (r) {
+                            var n = Te(this).constructor;
+                            e = Reflect.construct(t, arguments, n)
+                        } else e = t.apply(this, arguments);
+                        return Ie(this, e)
+                    });
+
+                    function l(e) {
+                        var t;
+                        return function(e, t) {
+                            if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
+                        }(this, l), (t = i.call(this, e)).onBarClick = t.onBarClick.bind(De(t)), t.onKeyDown = t.onKeyDown.bind(De(t)), t.handleIndex = 0, t
+                    }
+                    return t = l, (n = [{
+                        key: "spin",
+                        value: function(e, t) {
+                            var n = (this.props.range ? this.props.value[this.handleIndex] : this.props.value) || 0,
+                                o = (this.props.step || 1) * t;
+                            this.updateValue(e, n + o), e.preventDefault()
+                        }
+                    }, {
+                        key: "onDragStart",
+                        value: function(e, t) {
+                            this.props.disabled || (this.dragging = !0, this.updateDomData(), this.sliderHandleClick = !0, this.handleIndex = t)
+                        }
+                    }, {
+                        key: "onMouseDown",
+                        value: function(e, t) {
+                            this.bindDragListeners(), this.onDragStart(e, t)
+                        }
+                    }, {
+                        key: "onTouchStart",
+                        value: function(e, t) {
+                            this.bindTouchListeners(), this.onDragStart(e, t)
+                        }
+                    }, {
+                        key: "onKeyDown",
+                        value: function(e, t) {
+                            if (!this.props.disabled) {
+                                this.handleIndex = t;
+                                var n = e.key;
+                                "ArrowRight" === n || "ArrowUp" === n ? this.spin(e, 1) : "ArrowLeft" !== n && "ArrowDown" !== n || this.spin(e, -1)
+                            }
+                        }
+                    }, {
+                        key: "onBarClick",
+                        value: function(e) {
+                            this.props.disabled || (this.sliderHandleClick || (this.updateDomData(), this.setValue(e)), this.sliderHandleClick = !1)
+                        }
+                    }, {
+                        key: "onDrag",
+                        value: function(e) {
+                            this.dragging && (this.setValue(e), e.preventDefault())
+                        }
+                    }, {
+                        key: "onDragEnd",
+                        value: function(e) {
+                            this.dragging && (this.dragging = !1, this.props.onSlideEnd && this.props.onSlideEnd({
+                                originalEvent: e,
+                                value: this.props.value
+                            }), this.unbindDragListeners(), this.unbindTouchListeners())
+                        }
+                    }, {
+                        key: "bindDragListeners",
+                        value: function() {
+                            this.dragListener || (this.dragListener = this.onDrag.bind(this), document.addEventListener("mousemove", this.dragListener)), this.dragEndListener || (this.dragEndListener = this.onDragEnd.bind(this), document.addEventListener("mouseup", this.dragEndListener))
+                        }
+                    }, {
+                        key: "unbindDragListeners",
+                        value: function() {
+                            this.dragListener && (document.removeEventListener("mousemove", this.dragListener), this.dragListener = null), this.dragEndListener && (document.removeEventListener("mouseup", this.dragEndListener), this.dragEndListener = null)
+                        }
+                    }, {
+                        key: "bindTouchListeners",
+                        value: function() {
+                            this.dragListener || (this.dragListener = this.onDrag.bind(this), document.addEventListener("touchmove", this.dragListener)), this.dragEndListener || (this.dragEndListener = this.onDragEnd.bind(this), document.addEventListener("touchend", this.dragEndListener))
+                        }
+                    }, {
+                        key: "unbindTouchListeners",
+                        value: function() {
+                            this.dragListener && (document.removeEventListener("touchmove", this.dragListener), this.dragListener = null), this.dragEndListener && (document.removeEventListener("touchend", this.dragEndListener), this.dragEndListener = null)
+                        }
+                    }, {
+                        key: "updateDomData",
+                        value: function() {
+                            var e = this.el.getBoundingClientRect();
+                            this.initX = e.left + Y.p7.getWindowScrollLeft(), this.initY = e.top + Y.p7.getWindowScrollTop(), this.barWidth = this.el.offsetWidth, this.barHeight = this.el.offsetHeight
+                        }
+                    }, {
+                        key: "setValue",
+                        value: function(e) {
+                            var t, n = e.touches ? e.touches[0].pageX : e.pageX,
+                                o = e.touches ? e.touches[0].pageY : e.pageY;
+                            t = "horizontal" === this.props.orientation ? 100 * (n - this.initX) / this.barWidth : 100 * (this.initY + this.barHeight - o) / this.barHeight;
+                            var r = (this.props.max - this.props.min) * (t / 100) + this.props.min;
+                            if (this.props.step) {
+                                var i = this.props.range ? this.props.value[this.handleIndex] : this.props.value,
+                                    a = r - i;
+                                a < 0 ? r = i + Math.ceil(r / this.props.step - i / this.props.step) * this.props.step : a > 0 && (r = i + Math.floor(r / this.props.step - i / this.props.step) * this.props.step)
+                            } else r = Math.floor(r);
+                            this.updateValue(e, r)
+                        }
+                    }, {
+                        key: "updateValue",
+                        value: function(e, t) {
+                            var n, o = parseFloat(t.toFixed(10));
+                            if (this.props.range) {
+                                0 === this.handleIndex ? o < this.props.min ? o = this.props.min : o > this.props.value[1] && (o = this.props.value[1]) : o > this.props.max ? o = this.props.max : o < this.props.value[0] && (o = this.props.value[0]);
+                                var r = function(e) {
+                                    if (Array.isArray(e)) return Ce(e)
+                                }(n = this.props.value) || function(e) {
+                                    if ("undefined" != typeof Symbol && null != e[Symbol.iterator] || null != e["@@iterator"]) return Array.from(e)
+                                }(n) || function(e, t) {
+                                    if (e) {
+                                        if ("string" == typeof e) return Ce(e, t);
+                                        var n = Object.prototype.toString.call(e).slice(8, -1);
+                                        return "Object" === n && e.constructor && (n = e.constructor.name), "Map" === n || "Set" === n ? Array.from(e) : "Arguments" === n || /^(?:Ui|I)nt(?:8|16|32)(?:Clamped)?Array$/.test(n) ? Ce(e, t) : void 0
+                                    }
+                                }(n) || function() {
+                                    throw new TypeError("Invalid attempt to spread non-iterable instance.\nIn order to be iterable, non-array objects must have a [Symbol.iterator]() method.")
+                                }();
+                                r[this.handleIndex] = o, this.props.onChange && this.props.onChange({
+                                    originalEvent: e,
+                                    value: r
+                                })
+                            } else o < this.props.min ? o = this.props.min : o > this.props.max && (o = this.props.max), this.props.onChange && this.props.onChange({
+                                originalEvent: e,
+                                value: o
+                            })
+                        }
+                    }, {
+                        key: "componentWillUnmount",
+                        value: function() {
+                            this.unbindDragListeners(), this.unbindTouchListeners()
+                        }
+                    }, {
+                        key: "renderHandle",
+                        value: function(e, t, n) {
+                            var o = this,
+                                r = (0, Y.AK)("p-slider-handle", {
+                                    "p-slider-handle-start": 0 === n,
+                                    "p-slider-handle-end": 1 === n,
+                                    "p-slider-handle-active": this.handleIndex === n
+                                });
+                            return a.createElement("span", {
+                                onMouseDown: function(e) {
+                                    return o.onMouseDown(e, n)
+                                },
+                                onTouchStart: function(e) {
+                                    return o.onTouchStart(e, n)
+                                },
+                                onKeyDown: function(e) {
+                                    return o.onKeyDown(e, n)
+                                },
+                                tabIndex: this.props.tabIndex,
+                                className: r,
+                                style: {
+                                    transition: this.dragging ? "none" : null,
+                                    left: null !== e && e + "%",
+                                    bottom: t && t + "%"
+                                },
+                                role: "slider",
+                                "aria-valuemin": this.props.min,
+                                "aria-valuemax": this.props.max,
+                                "aria-valuenow": e || t,
+                                "aria-labelledby": this.props.ariaLabelledBy
+                            })
+                        }
+                    }, {
+                        key: "renderRangeSlider",
+                        value: function() {
+                            var e = this.props.value || [0, 0],
+                                t = "horizontal" === this.props.orientation,
+                                n = 100 * (e[0] < this.props.min ? 0 : e[0] - this.props.min) / (this.props.max - this.props.min),
+                                o = 100 * (e[1] > this.props.max ? 100 : e[1] - this.props.min) / (this.props.max - this.props.min),
+                                r = t ? this.renderHandle(n, null, 0) : this.renderHandle(null, n, 0),
+                                i = t ? this.renderHandle(o, null, 1) : this.renderHandle(null, o, 1),
+                                l = t ? {
+                                    left: n + "%",
+                                    width: o - n + "%"
+                                } : {
+                                    bottom: n + "%",
+                                    height: o - n + "%"
+                                };
+                            return a.createElement(a.Fragment, null, a.createElement("span", {
+                                className: "p-slider-range",
+                                style: l
+                            }), r, i)
+                        }
+                    }, {
+                        key: "renderSingleSlider",
+                        value: function() {
+                            var e, t = this.props.value || 0;
+                            e = t < this.props.min ? 0 : t > this.props.max ? 100 : 100 * (t - this.props.min) / (this.props.max - this.props.min);
+                            var n = "horizontal" === this.props.orientation ? {
+                                    width: e + "%"
+                                } : {
+                                    height: e + "%"
+                                },
+                                o = "horizontal" === this.props.orientation ? this.renderHandle(e, null, null) : this.renderHandle(null, e, null);
+                            return a.createElement(a.Fragment, null, a.createElement("span", {
+                                className: "p-slider-range",
+                                style: n
+                            }), o)
+                        }
+                    }, {
+                        key: "render",
+                        value: function() {
+                            var e = this,
+                                t = (0, Y.AK)("p-slider p-component", this.props.className, {
+                                    "p-disabled": this.props.disabled,
+                                    "p-slider-horizontal": "horizontal" === this.props.orientation,
+                                    "p-slider-vertical": "vertical" === this.props.orientation
+                                }),
+                                n = this.props.range ? this.renderRangeSlider() : this.renderSingleSlider();
+                            return a.createElement("div", {
+                                id: this.props.id,
+                                ref: function(t) {
+                                    return e.el = t
+                                },
+                                style: this.props.style,
+                                className: t,
+                                onClick: this.onBarClick
+                            }, n)
+                        }
+                    }]) && Se(t.prototype, n), l
+                }(a.Component);
+
+                function je(e) {
+                    return je = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                        return typeof e
+                    } : function(e) {
+                        return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
+                    }, je(e)
+                }
+
+                function Ne(e, t, n) {
+                    return t in e ? Object.defineProperty(e, t, {
+                        value: n,
+                        enumerable: !0,
+                        configurable: !0,
+                        writable: !0
+                    }) : e[t] = n, e
+                }
+
+                function Be(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function Se(e, t) {
-                    return Se = Object.setPrototypeOf || function(e, t) {
+                function Fe(e, t) {
+                    return Fe = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, Se(e, t)
+                    }, Fe(e, t)
                 }
 
-                function De(e, t) {
-                    if (t && ("object" === Oe(t) || "function" == typeof t)) return t;
+                function ze(e, t) {
+                    if (t && ("object" === je(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return function(e) {
-                        if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
-                        return e
-                    }(e)
+                    return Ue(e)
                 }
 
-                function Pe(e) {
-                    return Pe = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function Ue(e) {
+                    if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
+                    return e
+                }
+
+                function Ke(e) {
+                    return Ke = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, Pe(e)
+                    }, Ke(e)
                 }
-                var Re = function(e) {
+                Me = {
+                    id: null,
+                    value: null,
+                    min: 0,
+                    max: 100,
+                    orientation: "horizontal",
+                    step: null,
+                    range: !1,
+                    style: null,
+                    className: null,
+                    disabled: !1,
+                    tabIndex: 0,
+                    ariaLabelledBy: null,
+                    onChange: null,
+                    onSlideEnd: null
+                }, (Ae = "defaultProps") in(qe = Le) ? Object.defineProperty(qe, Ae, {
+                    value: Me,
+                    enumerable: !0,
+                    configurable: !0,
+                    writable: !0
+                }) : qe[Ae] = Me;
+                var We = function(e) {
                     ! function(e, t) {
                         if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                         Object.defineProperty(e, "prototype", {
                             value: Object.create(t && t.prototype, {
                                 constructor: {
                                     value: e,
                                     writable: !0,
                                     configurable: !0
                                 }
                             }),
                             writable: !1
-                        }), t && Se(e, t)
+                        }), t && Fe(e, t)
                     }(l, e);
                     var t, n, o, r, i = (o = l, r = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, t = Pe(o);
+                        var e, t = Ke(o);
                         if (r) {
-                            var n = Pe(this).constructor;
+                            var n = Ke(this).constructor;
                             e = Reflect.construct(t, arguments, n)
                         } else e = t.apply(this, arguments);
-                        return De(this, e)
+                        return ze(this, e)
                     });
 
                     function l(e) {
                         var t;
                         return function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
-                        }(this, l), (t = i.call(this, e)).state = {}, t.parent = e.parent, t
+                        }(this, l), (t = i.call(this, e)).state = {
+                            slider: e.slider || !1,
+                            sliderShowing: !1,
+                            sliderValue: e.sliderValue
+                        }, t.parent = e.parent, t.setRowsPerPage = t.setRowsPerPage.bind(Ue(t)), t
                     }
-                    return t = l, (n = [{
+                    return t = l, n = [{
+                        key: "setRowsPerPage",
+                        value: function(e) {
+                            var t;
+                            this.parent.data.page = 0, (0, x.k_)(this.props.router, (Ne(t = {}, P.qg, 0), Ne(t, P.EL, e), t), !0)
+                        }
+                    }, {
                         key: "render",
                         value: function() {
                             var e = this;
-                            return 0 === this.parent.props.actorData.preview_limit || 0 === this.parent.data.rows.length || this.parent.data.count < this.parent.data.rowsPerPage || this.parent.props.actorData.simple_paginator ? null : a.createElement(S.D, {
-                                rows: this.parent.data.rowsPerPage,
+                            return 0 === this.parent.props.actorData.preview_limit || 0 === this.parent.data.rows.length || this.parent.data.count < this.parent.data.rowsPerPage || this.parent.props.actorData.simple_paginator ? null : a.createElement("div", {
+                                ref: function(t) {
+                                    return e.container = t
+                                }
+                            }, a.createElement(S.D, {
+                                rows: this.state.sliderValue,
                                 paginator: !0,
-                                first: this.parent.data.topRow,
+                                first: this.parent.data.urlParams[P.qg] || 0,
                                 totalRecords: this.parent.data.count,
                                 template: this.parent.props.actorData.paginator_template || void 0,
                                 onPageChange: function(t) {
-                                    e.parent.reload({
-                                        page: t.page
-                                    })
+                                    e.parent.data.page = t.page, (0, x.k_)(e.props.router, Ne({}, P.qg, t.page * e.state.sliderValue), !0)
                                 },
                                 rightContent: this.parent.data.count && a.createElement("span", {
                                     className: "l-grid-count"
-                                }, "Showing ", a.createElement(C.L, {
+                                }, "Showing ", this.state.slider ? a.createElement(a.Fragment, null, !this.state.sliderShowing && a.createElement(w.z, {
+                                    icon: "pi pi-minus",
+                                    onClick: function(t) {
+                                        return e.setRowsPerPage(e.state.sliderValue - 1)
+                                    },
+                                    type: "button"
+                                }), a.createElement(w.z, {
+                                    type: "button",
+                                    label: this.state.sliderValue.toString(),
+                                    onClick: function(t) {
+                                        e.setState({
+                                            sliderShowing: !e.state.sliderShowing
+                                        }), e.sliderPanel.toggle(t)
+                                    }
+                                }), !this.state.sliderShowing && a.createElement(w.z, {
+                                    icon: "pi pi-plus",
+                                    onClick: function(t) {
+                                        return e.setRowsPerPage(e.state.sliderValue + 1)
+                                    },
+                                    type: "button"
+                                }), a.createElement(Oe.T, {
+                                    ref: function(t) {
+                                        return e.sliderPanel = t
+                                    },
+                                    dismissable: !0
+                                }, a.createElement(Le, {
+                                    animate: !0,
+                                    max: this.parent.data.count,
+                                    onChange: function(t) {
+                                        return e.setState({
+                                            sliderValue: t.value
+                                        })
+                                    },
+                                    onSlideEnd: function(t) {
+                                        return e.setRowsPerPage(t.value)
+                                    },
+                                    orientation: "vertical",
+                                    value: this.state.sliderValue
+                                }))) : a.createElement(C.L, {
                                     style: {
                                         width: "80px"
                                     },
-                                    value: this.parent.data.rowsPerPage,
-                                    placeholder: this.parent.data.rowsPerPage.toString(),
-                                    options: [25, 50, 100, 200, 400, 800],
+                                    value: this.state.sliderValue,
+                                    placeholder: this.state.sliderValue.toString(),
+                                    options: [15, 25, 50, 100, 200, 400, 800],
                                     onChange: function(t) {
-                                        var n = parseInt(t.value);
-                                        e.parent.data.page = 0, e.parent.data.rowsPerPage = n <= e.parent.data.count ? n : e.parent.data.count, e.parent.refresh()
+                                        e.setRowsPerPage(t.value)
                                     }
                                 }), a.createElement("span", null, " of ", this.parent.data.count), " rows")
-                            })
+                            }))
                         }
-                    }]) && Ce(t.prototype, n), Object.defineProperty(t, "prototype", {
+                    }], n && Be(t.prototype, n), Object.defineProperty(t, "prototype", {
                         writable: !1
                     }), l
                 }(a.Component);
 
-                function Ie(e) {
-                    return Ie = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function He(e) {
+                    return He = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, Ie(e)
+                    }, He(e)
                 }
 
-                function Te(e, t) {
+                function Ve(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function qe(e, t) {
-                    return qe = Object.setPrototypeOf || function(e, t) {
+                function Ge(e, t) {
+                    return Ge = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, qe(e, t)
+                    }, Ge(e, t)
                 }
 
-                function Ae(e, t) {
-                    if (t && ("object" === Ie(t) || "function" == typeof t)) return t;
+                function Ze(e, t) {
+                    if (t && ("object" === He(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
                     return function(e) {
                         if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                         return e
                     }(e)
                 }
 
-                function Me(e) {
-                    return Me = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function Ye(e) {
+                    return Ye = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, Me(e)
+                    }, Ye(e)
                 }
-                var Le = function(e) {
+                var Xe = function(e) {
                         ! function(e, t) {
                             if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                             Object.defineProperty(e, "prototype", {
                                 value: Object.create(t && t.prototype, {
                                     constructor: {
                                         value: e,
                                         writable: !0,
                                         configurable: !0
                                     }
                                 }),
                                 writable: !1
-                            }), t && qe(e, t)
+                            }), t && Ge(e, t)
                         }(l, e);
                         var t, n, o, r, i = (o = l, r = function() {
                             if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                             if (Reflect.construct.sham) return !1;
                             if ("function" == typeof Proxy) return !0;
                             try {
                                 return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                             } catch (e) {
                                 return !1
                             }
                         }(), function() {
-                            var e, t = Me(o);
+                            var e, t = Ye(o);
                             if (r) {
-                                var n = Me(this).constructor;
+                                var n = Ye(this).constructor;
                                 e = Reflect.construct(t, arguments, n)
                             } else e = t.apply(this, arguments);
-                            return Ae(this, e)
+                            return Ze(this, e)
                         });
 
                         function l(e) {
                             var t;
                             return function(e, t) {
                                 if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                             }(this, l), (t = i.call(this, e)).state = {}, t.parent = e.parent, t
@@ -5082,152 +5504,152 @@
                             key: "render",
                             value: function() {
                                 return a.createElement(a.Fragment, null, a.createElement("div", {
                                     hidden: !this.parent.state.showPVDialog,
                                     className: "l-params-panel l-header"
                                 }, a.createElement(D.ZP, {
                                     window_layout: this.parent.props.actorData.params_layout,
-                                    window_type: me.Mj,
+                                    window_type: P.Mj,
                                     actorData: this.parent.props.actorData,
                                     data: this.parent.data.params_values,
                                     actorId: this.parent.get_full_id(),
                                     update_value: this.parent.update_params_values,
                                     editing_mode: !0,
                                     mk: this.parent.props.mk,
                                     mt: this.parent.props.actorData.content_type,
                                     router: this.parent.props.router
                                 })))
                             }
-                        }]) && Te(t.prototype, n), Object.defineProperty(t, "prototype", {
+                        }]) && Ve(t.prototype, n), Object.defineProperty(t, "prototype", {
                             writable: !1
                         }), l
                     }(a.Component),
-                    je = n(5783);
+                    Je = n(5783);
 
-                function Ne(e) {
-                    return Ne = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
+                function Qe(e) {
+                    return Qe = "function" == typeof Symbol && "symbol" == typeof Symbol.iterator ? function(e) {
                         return typeof e
                     } : function(e) {
                         return e && "function" == typeof Symbol && e.constructor === Symbol && e !== Symbol.prototype ? "symbol" : typeof e
-                    }, Ne(e)
+                    }, Qe(e)
                 }
 
-                function Be() {
-                    return Be = Object.assign || function(e) {
+                function $e() {
+                    return $e = Object.assign || function(e) {
                         for (var t = 1; t < arguments.length; t++) {
                             var n = arguments[t];
                             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (e[o] = n[o])
                         }
                         return e
-                    }, Be.apply(this, arguments)
+                    }, $e.apply(this, arguments)
                 }
 
-                function Fe(e, t, n, o, r, i, a) {
+                function et(e, t, n, o, r, i, a) {
                     try {
                         var l = e[i](a),
                             s = l.value
                     } catch (e) {
                         return void n(e)
                     }
                     l.done ? t(s) : Promise.resolve(s).then(o, r)
                 }
 
-                function ze(e) {
+                function tt(e) {
                     return function() {
                         var t = this,
                             n = arguments;
                         return new Promise((function(o, r) {
                             var i = e.apply(t, n);
 
                             function a(e) {
-                                Fe(i, o, r, a, l, "next", e)
+                                et(i, o, r, a, l, "next", e)
                             }
 
                             function l(e) {
-                                Fe(i, o, r, a, l, "throw", e)
+                                et(i, o, r, a, l, "throw", e)
                             }
                             a(void 0)
                         }))
                     }
                 }
 
-                function Ue(e, t) {
+                function nt(e, t) {
                     for (var n = 0; n < t.length; n++) {
                         var o = t[n];
                         o.enumerable = o.enumerable || !1, o.configurable = !0, "value" in o && (o.writable = !0), Object.defineProperty(e, o.key, o)
                     }
                 }
 
-                function Ke(e, t) {
-                    return Ke = Object.setPrototypeOf || function(e, t) {
+                function ot(e, t) {
+                    return ot = Object.setPrototypeOf || function(e, t) {
                         return e.__proto__ = t, e
-                    }, Ke(e, t)
+                    }, ot(e, t)
                 }
 
-                function We(e, t) {
-                    if (t && ("object" === Ne(t) || "function" == typeof t)) return t;
+                function rt(e, t) {
+                    if (t && ("object" === Qe(t) || "function" == typeof t)) return t;
                     if (void 0 !== t) throw new TypeError("Derived constructors may only return object or undefined");
-                    return He(e)
+                    return it(e)
                 }
 
-                function He(e) {
+                function it(e) {
                     if (void 0 === e) throw new ReferenceError("this hasn't been initialised - super() hasn't been called");
                     return e
                 }
 
-                function Ve(e) {
-                    return Ve = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
+                function at(e) {
+                    return at = Object.setPrototypeOf ? Object.getPrototypeOf : function(e) {
                         return e.__proto__ || Object.getPrototypeOf(e)
-                    }, Ve(e)
+                    }, at(e)
                 }
-                var Ge = function(e) {
+                var lt = function(e) {
                     ! function(e, t) {
                         if ("function" != typeof t && null !== t) throw new TypeError("Super expression must either be null or a function");
                         Object.defineProperty(e, "prototype", {
                             value: Object.create(t && t.prototype, {
                                 constructor: {
                                     value: e,
                                     writable: !0,
                                     configurable: !0
                                 }
                             }),
                             writable: !1
-                        }), t && Ke(e, t)
+                        }), t && ot(e, t)
                     }(f, e);
                     var t, n, o, r, i, u, d = (i = f, u = function() {
                         if ("undefined" == typeof Reflect || !Reflect.construct) return !1;
                         if (Reflect.construct.sham) return !1;
                         if ("function" == typeof Proxy) return !0;
                         try {
                             return Boolean.prototype.valueOf.call(Reflect.construct(Boolean, [], (function() {}))), !0
                         } catch (e) {
                             return !1
                         }
                     }(), function() {
-                        var e, t = Ve(i);
+                        var e, t = at(i);
                         if (u) {
-                            var n = Ve(this).constructor;
+                            var n = at(this).constructor;
                             e = Reflect.construct(t, arguments, n)
                         } else e = t.apply(this, arguments);
-                        return We(this, e)
+                        return rt(this, e)
                     });
 
                     function f(e) {
                         var t;
                         ! function(e, t) {
                             if (!(e instanceof t)) throw new TypeError("Cannot call a class as a function")
                         }(this, f), t = d.call(this, e);
                         var n = parseInt(e.widthInCh),
                             o = void 0;
                         e.actorData.display_mode && (o = (0, x.ol)(e.actorData.display_mode, n));
                         var r = (0, x.tq)();
                         return window.App.isMobile = r, t.state = {
-                            data_view: !!(e.actorData.contain_media || o && [me.do, me.OW, me.UZ].includes(o)),
+                            data_view: !!(e.actorData.contain_media || o && [P.do, P.OW, P.UZ].includes(o)),
                             isMobile: r,
-                            layout: e.actorData.contain_media ? me.dI : [me.do, me.OW, me.UZ].includes(o) ? o : me.C2,
+                            layout: e.actorData.contain_media ? P.dI : [P.do, P.OW, P.UZ].includes(o) ? o : P.C2,
                             loading: !0,
                             show_top_toolbar: !e.actorData.hide_top_toolbar && !r,
                             showPVDialog: !1,
                             static_page: "show" === e.actorData.default_action,
                             window_width: window.innerWidth
                         }, t.data = {
                             cols: void 0,
@@ -5255,17 +5677,16 @@
                                 return e.fields_index
                             })),
                             sortCol: void 0,
                             sortField: void 0,
                             sortFieldName: void 0,
                             sortOrder: 0,
                             title: "",
-                            topRow: 0,
                             urlParams: (0, x.VW)(e.router)
-                        }, t.actionWrapper = t.actionWrapper.bind(He(t)), t.consumeServerResponse = t.consumeServerResponse.bind(He(t)), t.get_current_grid_config = t.get_current_grid_config.bind(He(t)), t.get_full_id = t.get_full_id.bind(He(t)), t.getData = t.getData.bind(He(t)), t.getOne = t.getOne.bind(He(t)), t.getUri = t.getUri.bind(He(t)), t.handleWindowChange = (0, x.Ds)(t.handleWindowChange.bind(He(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(He(t)), t.registerScroll = t.registerScroll.bind(He(t)), t.multiRowView = t.multiRowView.bind(He(t)), t.onKeyDown = t.onKeyDown.bind(He(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(He(t)), t.onSort = t.onSort.bind(He(t)), t.refresh = t.refresh.bind(He(t)), t.quickFilter = (0, x.Ds)(t.quickFilter.bind(He(t)), 200), t.reload = t.reload.bind(He(t)), t.reset = t.reset.bind(He(t)), t.update_params_values = t.update_params_values.bind(He(t)), t
+                        }, t.actionWrapper = t.actionWrapper.bind(it(t)), t.consumeServerResponse = t.consumeServerResponse.bind(it(t)), t.get_current_grid_config = t.get_current_grid_config.bind(it(t)), t.get_full_id = t.get_full_id.bind(it(t)), t.getData = t.getData.bind(it(t)), t.getOne = t.getOne.bind(it(t)), t.getUri = t.getUri.bind(it(t)), t.handleWindowChange = (0, x.Ds)(t.handleWindowChange.bind(it(t)), 50), t.messageInterceptor = t.messageInterceptor.bind(it(t)), t.registerScroll = t.registerScroll.bind(it(t)), t.multiRowView = t.multiRowView.bind(it(t)), t.onKeyDown = t.onKeyDown.bind(it(t)), t.onRowDoubleClick = t.onRowDoubleClick.bind(it(t)), t.onSort = t.onSort.bind(it(t)), t.refresh = t.refresh.bind(it(t)), t.quickFilter = (0, x.Ds)(t.quickFilter.bind(it(t)), 200), t.reload = t.reload.bind(it(t)), t.reset = t.reset.bind(it(t)), t.update_params_values = t.update_params_values.bind(it(t)), t
                     }
                     return t = f, n = [{
                         key: "get_full_id",
                         value: function() {
                             return "".concat(this.props.packId, ".").concat(this.props.actorId)
                         }
                     }, {
@@ -5288,22 +5709,22 @@
                             }) : this.firstScrollIngonred = !0
                         }
                     }, {
                         key: "getSnapshotBeforeUpdate",
                         value: function(e, t) {
                             var n = {},
                                 o = (0, x.VW)(this.props.router);
-                            (this.props.pk !== e.pk || this.props.mk !== e.mk || this.props.mt !== e.mt || 0 !== e.reload_timestamp && this.props.reload_timestamp !== e.reload_timestamp || !p().isEqual(this.data.urlParams.pv, o.pv)) && (this.data.urlParams = o, n.requireRefresh = !0), e.router.match.isExact === this.props.router.match.isExact && e.actorData.detail_action === this.props.actorData.detail_action || (n.detail_window = !this.props.router.match.isExact || "show" === this.props.actorData.default_action);
+                            (this.props.pk !== e.pk || this.props.mk !== e.mk || this.props.mt !== e.mt || 0 !== e.reload_timestamp && this.props.reload_timestamp !== e.reload_timestamp || !p().isEqual(this.data.urlParams.pv, o.pv)) && (this.data.urlParams = o, n.requireRefresh = !0), this.data.urlParams[P.qg] == o[P.qg] && this.data.urlParams[P.EL] == o[P.EL] || (n.requireReload = !0, this.data.urlParams = o), e.router.match.isExact === this.props.router.match.isExact && e.actorData.detail_action === this.props.actorData.detail_action || (n.detail_window = !this.props.router.match.isExact || "show" === this.props.actorData.default_action);
                             var r = (0, x.eJ)(this.props);
                             return void 0 !== r && void 0 !== this.data.id && r !== this.data.id && (n.id = r), Object.keys(n).length ? n : null
                         }
                     }, {
                         key: "componentDidUpdate",
                         value: function(e, t, n) {
-                            if (null !== n) return n.hasOwnProperty("id") ? (Object.assign(this.data, n), void this.reload()) : n.hasOwnProperty("detail_window") ? (Object.assign(this.data, n), this.data.id = (0, x.eJ)(this.props), void this.reload()) : void(n.hasOwnProperty("requireRefresh") && this.refresh())
+                            if (null !== n) return n.hasOwnProperty("id") ? (Object.assign(this.data, n), void this.reload()) : n.hasOwnProperty("detail_window") ? (Object.assign(this.data, n), this.data.id = (0, x.eJ)(this.props), void this.reload()) : void(n.hasOwnProperty("requireReload") ? this.reload() : n.hasOwnProperty("requireRefresh") && this.refresh())
                         }
                     }, {
                         key: "componentWillUnmount",
                         value: function() {
                             this.controller.abort(), window.removeEventListener("resize", this.handleWindowChange), window.removeEventListener("keydown", this.onKeyDown), window.removeEventListener("message", this.messageInterceptor), this.props.parentBody && window.removeEventListener("scroll", this.registerScroll)
                         }
                     }, {
@@ -5418,24 +5839,24 @@
                             this.setState({
                                 loading: !0
                             }), this.refresh(e)
                         }
                     }, {
                         key: "refresh",
                         value: function(e) {
+                            this.controller.abort(), this.controller = new(m());
                             var t = this.controller.signal;
                             e && e.signal && (t = e.signal);
                             var n = this.queryObject(e);
                             this.data.detail_window ? this.getOne(this.data.id, n, t, !0) : this.getData(this.getUri(n), this.consumeServerResponse, t, !0)
                         }
                     }, {
                         key: "reset",
                         value: function(e, t) {
                             Object.assign(this.data, {
-                                page: 0,
                                 sortOrder: 0,
                                 sr: [],
                                 sortField: void 0
                             }), e.query = "", t || this.data.detail_window ? this.reload(e) : this.refresh(e)
                         }
                     }, {
                         key: "queryObject",
@@ -5451,29 +5872,28 @@
                                 s = void 0 === l ? void 0 : l,
                                 p = e.displayMode,
                                 u = void 0 === p ? void 0 : p,
                                 d = {};
                             d.page = void 0 !== n ? n : this.data.page, d.sortFieldName = void 0 !== a ? a.name : this.data.sortFieldName, d.sortOrder = void 0 !== s ? s : this.data.sortOrder, d.displayMode = void 0 !== u ? u : this.state.layout, Object.assign(this.data, {
                                 page: d.page,
                                 sortFieldName: d.sortFieldName,
-                                sortOrder: d.sortOrder,
-                                topRow: d.page * this.data.rowsPerPage
+                                sortOrder: d.sortOrder
                             });
                             var f = {};
-                            return f[me.Vk] = void 0 !== r ? "" === r ? void 0 : r : this.data.urlParams.query, f[me.i5] = me.oi, f[me.qg] = d.page * this.data.rowsPerPage, f[me.EL] = this.data.rowsPerPage, f[me.mQ] = this.rp || c()(this), f[me.Vp] = d.displayMode, f[me.$S] = me.zf, f[me.xX] = window.App.state.site_data.revision_number, f[me.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, f[me.jT] = window.App.state.site_data[me.jT], void 0 !== d.sortFieldName && (f.sort = d.sortFieldName), 0 !== d.sortOrder && (f.dir = 1 === d.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv ? f[me.ks] = (0, x.ku)(this.props.parent_pv, this.props.actorData.params_fields) : this.props.actorData.params_layout && !this.props.inDetail && (f[me.ks] = this.data.urlParams.pv), void 0 !== this.props.mk && null !== this.props.mt && (f.mk = this.props.mk), void 0 !== this.props.mt && null !== this.props.mt && (f.mt = this.props.mt), window.App.add_su(f), f
+                            return f[P.Vk] = void 0 !== r ? "" === r ? void 0 : r : this.data.urlParams.query, f[P.i5] = P.oi, f[P.qg] = this.data.urlParams[P.qg] || d.page * (this.data.urlParams[P.EL] || this.data.rowsPerPage), f[P.EL] = this.data.urlParams[P.EL] || this.data.rowsPerPage, f[P.mQ] = this.rp || c()(this), f[P.Vp] = d.displayMode, f[P.$S] = P.zf, f[P.xX] = window.App.state.site_data.revision_number, f[P.fH] = window.App.data.selectedLanguage || window.App.state.user_settings.lang, f[P.jT] = window.App.state.site_data[P.jT], void 0 !== d.sortFieldName && (f.sort = d.sortFieldName), 0 !== d.sortOrder && (f.dir = 1 === d.sortOrder ? "ASC" : "DESC"), this.props.actorData.use_detail_params_value && this.props.parent_pv ? f[P.ks] = (0, x.ku)(this.props.parent_pv, this.props.actorData.params_fields) : this.props.actorData.params_layout && !this.props.inDetail && (f[P.ks] = this.data.urlParams.pv), void 0 !== this.props.mk && null !== this.props.mt && (f.mk = this.props.mk), void 0 !== this.props.mt && null !== this.props.mt && (f.mt = this.props.mt), window.App.add_su(f), f
                         }
                     }, {
                         key: "getUri",
                         value: function(e) {
                             var t = "api/".concat(this.props.packId, "/").concat(this.props.actorId);
                             return void 0 !== e && (t += "?".concat(g.stringify(e))), t
                         }
                     }, {
                         key: "getData",
-                        value: (r = ze(y().mark((function e(t, n, o) {
+                        value: (r = tt(y().mark((function e(t, n, o) {
                             var r, i = this,
                                 a = arguments;
                             return y().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return (r = a.length > 3 && void 0 !== a[3] && a[3]) && Object.assign(this.data, {
                                             loading: !0,
@@ -5494,15 +5914,15 @@
                                 }
                             }), e, this)
                         }))), function(e, t, n) {
                             return r.apply(this, arguments)
                         })
                     }, {
                         key: "getOne",
-                        value: (o = ze(y().mark((function e(t, n, o, r) {
+                        value: (o = tt(y().mark((function e(t, n, o, r) {
                             var i = this;
                             return y().wrap((function(e) {
                                 for (;;) switch (e.prev = e.next) {
                                     case 0:
                                         return e.next = 2, (0, b.he)("api/".concat(this.props.packId, "/").concat(this.props.actorId, "/").concat(t, "?").concat(g.stringify(n)), {
                                             signal: o
                                         }).then(window.App.handleAjaxResponse).then((function(e) {
@@ -5538,15 +5958,15 @@
                                             navinfo: e.navinfo,
                                             reload_timestamp: Date.now(),
                                             params_values: e.param_values
                                         })
                                     } else !this.props.actorData.slave && e.status;
                                 else {
                                     if (e.success) {
-                                        var o = Math.floor(e.count / this.data.rowsPerPage);
+                                        var o = Math.floor(e.count / (this.data.urlParams[P.EL] || this.data.rowsPerPage));
                                         Object.assign(this.data, {
                                             count: e.count,
                                             lastPage: o,
                                             loading: !1,
                                             params_values: this.props.inDetail ? {} : e.param_values,
                                             reload_timestamp: Date.now(),
                                             rows: e.rows,
@@ -5601,15 +6021,15 @@
                                         return e.props.col
                                     })),
                                     i = Array.from(document.querySelector("table tr").getElementsByClassName("l-grid-col"));
                                 r.forEach((function(e, r) {
                                     t.push(e.name), n.push(Math.floor(i[r].getBoundingClientRect().width)), o.push(!1)
                                 }))
                             }
-                            return e[me.Td] = t, e[me.SX] = o, e[me.EO] = n, e[me.ks] = this.data.urlParams.pv, e
+                            return e[P.Td] = t, e[P.SX] = o, e[P.EO] = n, e[P.ks] = this.data.urlParams.pv, e
                         }
                     }, {
                         key: "render",
                         value: function() {
                             var e = this,
                                 t = "l-grid ";
                             if ("whitewall" === window.App.data.themeName && (t += "l-whitewall-body "), this.props.actorData.hide_if_empty && this.props.inDetail && 0 === this.data.rows.length) return null;
@@ -5617,28 +6037,28 @@
                                 dangerouslySetInnerHTML: {
                                     __html: this.data.title || this.props.actorData.label || " "
                                 }
                             }), this.props.inDetail ? a.createElement("span", {
                                 style: {
                                     float: "right"
                                 }
-                            }, a.createElement(je.ec, {
+                            }, a.createElement(Je.ec, {
                                 parent: this
                             })) : this.state.isMobile ? a.createElement("div", {
                                 style: {
                                     position: "fixed",
                                     right: "0px",
                                     top: "50%",
                                     transform: "translate(0, -50%)",
                                     maxWidth: "40px",
                                     background: "#2255AA40",
                                     borderRadius: "3px",
                                     zIndex: 999999
                                 }
-                            }, a.createElement(je.ZP, {
+                            }, a.createElement(Je.ZP, {
                                 parent: this,
                                 side: !0
                             })) : a.createElement(k.C, {
                                 style: {
                                     float: "right"
                                 },
                                 checked: this.state.show_top_toolbar,
@@ -5655,30 +6075,30 @@
                             }));
                             return a.createElement(a.Fragment, null, this.props.inDetail ? a.createElement("div", {
                                 className: "p-panel p-component"
                             }, a.createElement("div", {
                                 className: "l-detail-header p-panel-header"
                             }, n)) : a.createElement("div", {
                                 className: "l-detail-header"
-                            }, n), "top" === this.props.actorData.params_panel_pos && this.state.showPVDialog && a.createElement(Le, {
+                            }, n), "top" === this.props.actorData.params_panel_pos && this.state.showPVDialog && a.createElement(Xe, {
                                 parent: this
                             }), !this.props.inDetail && a.createElement("div", {
                                 className: "l-header"
-                            }, a.createElement(je.ZP, {
+                            }, a.createElement(Je.ZP, {
                                 parent: this
                             })), a.createElement("div", {
                                 className: "left" === this.props.actorData.params_panel_pos ? "l-params-panel-left" : "right" === this.props.actorData.params_panel_pos ? "l-params-panel-right" : ""
-                            }, this.props.actorData.hasOwnProperty("params_panel_pos") && "top" !== this.props.actorData.params_panel_pos && a.createElement(Le, {
+                            }, this.props.actorData.hasOwnProperty("params_panel_pos") && "top" !== this.props.actorData.params_panel_pos && a.createElement(Xe, {
                                 parent: this
                             }), a.createElement("div", {
                                 className: t
                             }, !this.state.loading && !this.data.detail_window && !this.state.static_page && a.createElement(a.Fragment, null, a.createElement(l.AW, {
                                 path: this.props.router.match.path,
                                 render: function(t) {
-                                    return a.createElement(a.Fragment, null, e.state.layout === me.C2 ? a.createElement(H, Be({}, e.props, {
+                                    return a.createElement(a.Fragment, null, e.state.layout === P.C2 ? a.createElement(V, $e({}, e.props, {
                                         fetching: e.data.fetching,
                                         parent: e,
                                         loading: e.data.loading,
                                         onRowDoubleClick: e.onRowDoubleClick,
                                         onSort: e.onSort,
                                         pv: e.state.pv,
                                         ref: function(t) {
@@ -5688,24 +6108,29 @@
                                         reload_timestamp: e.data.reload_timestamp,
                                         router: t,
                                         rows: e.data.rows,
                                         sr: e.data.sr,
                                         show_columns: e.data.show_columns,
                                         sortField: e.data.sortField,
                                         sortOrder: e.data.sortOrder
-                                    })) : [me.UZ, me.do].includes(e.state.layout) ? a.createElement("div", {
+                                    })) : [P.UZ, P.do].includes(e.state.layout) ? a.createElement("div", {
                                         dangerouslySetInnerHTML: {
                                             __html: e.data.html_text
                                         }
                                     }) : a.createElement(xe, {
                                         parent: e,
                                         router: t
-                                    }), !e.state.loading && a.createElement(Re, {
+                                    }), !e.state.loading && a.createElement(We, {
                                         parent: e,
-                                        router: t
+                                        ref: function(t) {
+                                            return e.paginator = t
+                                        },
+                                        router: t,
+                                        slider: !0,
+                                        sliderValue: e.data.urlParams[P.EL] || e.data.rowsPerPage
                                     }))
                                 }
                             }))), !this.state.loading && this.data.detail_window && a.createElement(l.AW, {
                                 path: this.state.static_page ? "".concat(this.props.router.match.path) : "".concat(this.props.router.match.path, "/:pk"),
                                 render: function(t) {
                                     var n;
                                     n = "/" === t.location.pathname && window.App.state.user_settings.dashboard_layout ? window.App.state.site_data.choicelists["system.DashboardLayouts"].find((function(e) {
@@ -5758,26 +6183,26 @@
                                 visible: this.state.showPVDialog,
                                 modal: !0,
                                 onHide: function(t) {
                                     e.setState({
                                         showPVDialog: !1
                                     })
                                 }
-                            }, this.props.actorData.params_layout && this.state.showPVDialog && a.createElement(Le, {
+                            }, this.props.actorData.params_layout && this.state.showPVDialog && a.createElement(Xe, {
                                 parent: this
                             })))
                         }
-                    }], n && Ue(t.prototype, n), Object.defineProperty(t, "prototype", {
+                    }], n && nt(t.prototype, n), Object.defineProperty(t, "prototype", {
                         writable: !1
                     }), f
                 }(a.Component);
-                Ge.propTypes = {
+                lt.propTypes = {
                     inDetail: f().bool,
                     depth: f().number
-                }, Ge.defaultProps = {
+                }, lt.defaultProps = {
                     inDetail: !1,
                     depth: 0
                 }
             },
             7573: (e, t, n) => {
                 "use strict";
                 n.d(t, {
@@ -7338,15 +7763,15 @@
                     primereact_fieldset__WEBPACK_IMPORTED_MODULE_9__ = __webpack_require__(2569),
                     primereact_editor__WEBPACK_IMPORTED_MODULE_10__ = __webpack_require__(8221),
                     primereact_button__WEBPACK_IMPORTED_MODULE_11__ = __webpack_require__(3374),
                     primereact_dropdown__WEBPACK_IMPORTED_MODULE_12__ = __webpack_require__(7315),
                     primereact_password__WEBPACK_IMPORTED_MODULE_13__ = __webpack_require__(5016),
                     primereact_progressspinner__WEBPACK_IMPORTED_MODULE_14__ = __webpack_require__(4457),
                     _primereact_fileupload__WEBPACK_IMPORTED_MODULE_15__ = __webpack_require__(996),
-                    _LinoBody__WEBPACK_IMPORTED_MODULE_16__ = __webpack_require__(6149),
+                    _LinoBody__WEBPACK_IMPORTED_MODULE_16__ = __webpack_require__(6147),
                     _SiteContext__WEBPACK_IMPORTED_MODULE_17__ = __webpack_require__(7239),
                     classnames__WEBPACK_IMPORTED_MODULE_18__ = __webpack_require__(5904),
                     classnames__WEBPACK_IMPORTED_MODULE_18___default = __webpack_require__.n(classnames__WEBPACK_IMPORTED_MODULE_18__),
                     _ForeignKeyElement__WEBPACK_IMPORTED_MODULE_19__ = __webpack_require__(6678),
                     _TextFieldElement__WEBPACK_IMPORTED_MODULE_20__ = __webpack_require__(5705),
                     _datetime__WEBPACK_IMPORTED_MODULE_21__ = __webpack_require__(7002),
                     _LinoUtils__WEBPACK_IMPORTED_MODULE_22__ = __webpack_require__(9502),
@@ -55672,15 +56097,15 @@
                 n.d(t, {
                     Z: () => i
                 });
                 var o = n(9481),
                     r = n.n(o)()((function(e) {
                         return e[1]
                     }));
-                r.push([e.id, '@charset "UTF-8";\n/* General */\n/* Menu */\n/* Menu Dark*/\n/* Menu Light*/\n/* Topbar */\n/* Footer */\n.splash-screen {\n  width: 100%;\n  height: 100%;\n  position: fixed;\n  background: #0388E5;\n  /* Old browsers */\n  background: -moz-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* FF3.6+ */\n  background: -webkit-gradient(linear, left top, right top, color-stop(0%, #0388E5), color-stop(100%, #07BDF4));\n  /* Chrome,Safari4+ */\n  background: -webkit-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* Chrome10+,Safari5.1+ */\n  background: -o-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* Opera 11.10+ */\n  background: -ms-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* IE10+ */\n  background: linear-gradient(to right, #0388E5 0%, #07BDF4 100%);\n  /* W3C */\n  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=$left, endColorstr=$right,GradientType=1 );\n  /* IE6-9 */ }\n  .splash-screen .splash-container {\n    width: 40px;\n    height: 40px;\n    margin: 0px auto;\n    position: absolute;\n    left: 50%;\n    top: 50%;\n    margin-left: -20px;\n    margin-top: -20px; }\n  .splash-screen .splash-double-bounce1, .splash-screen .splash-double-bounce2 {\n    width: 100%;\n    height: 100%;\n    border-radius: 50%;\n    background-color: #ffffff;\n    opacity: 0.6;\n    position: absolute;\n    top: 0;\n    left: 0;\n    -webkit-animation: splash-bounce 2.0s infinite ease-in-out;\n    animation: splash-bounce 2.0s infinite ease-in-out; }\n  .splash-screen .splash-double-bounce2 {\n    -webkit-animation-delay: -1.0s;\n    animation-delay: -1.0s; }\n\n@-webkit-keyframes splash-bounce {\n  0%, 100% {\n    -webkit-transform: scale(0); }\n  50% {\n    -webkit-transform: scale(1); } }\n\n@keyframes splash-bounce {\n  0%, 100% {\n    transform: scale(0);\n    -webkit-transform: scale(0); }\n  50% {\n    transform: scale(1);\n    -webkit-transform: scale(1); } }\n\n* {\n  box-sizing: border-box; }\n\nhtml {\n  height: 100%; }\n\nbody {\n  font-family: "Open Sans", "Helvetica Neue", sans-serif;\n  font-size: 14px;\n  color: #333333;\n  background-color: #edf0f5;\n  margin: 0;\n  padding: 0;\n  min-height: 100%; }\n\na {\n  text-decoration: none; }\n\n.layout-wrapper {\n  padding: 0; }\n  .layout-wrapper .layout-topbar {\n    position: fixed;\n    height: 50px;\n    padding: .7em 1.5em 0em 1.5em;\n    color: #ffffff;\n    z-index: 999;\n    right: 0;\n    background: #0388E5;\n    /* Old browsers */\n    background: -moz-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* FF3.6+ */\n    background: -webkit-gradient(linear, left top, right top, color-stop(0%, #0388E5), color-stop(100%, #07BDF4));\n    /* Chrome,Safari4+ */\n    background: -webkit-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* Chrome10+,Safari5.1+ */\n    background: -o-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* Opera 11.10+ */\n    background: -ms-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* IE10+ */\n    background: linear-gradient(to right, #0388E5 0%, #07BDF4 100%);\n    /* W3C */\n    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=$left, endColorstr=$right,GradientType=1 );\n    /* IE6-9 */\n    -moz-transition: left 0.2s;\n    -o-transition: left 0.2s;\n    -webkit-transition: left 0.2s;\n    transition: left 0.2s; }\n    .layout-wrapper .layout-topbar .layout-topbar-icons {\n      float: right;\n      display: block;\n      -moz-animation-duration: .5s;\n      -webkit-animation-duration: .5s;\n      animation-duration: .5s; }\n      .layout-wrapper .layout-topbar .layout-topbar-icons a {\n        position: relative;\n        color: #ffffff;\n        margin-left: 20px;\n        display: inline-block;\n        text-decoration: none;\n        -moz-transition: color 0.2s;\n        -o-transition: color 0.2s;\n        -webkit-transition: color 0.2s;\n        transition: color 0.2s; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a:hover {\n          color: #77c7ff; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-icon {\n          font-size: 2em; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-item-text {\n          font-size: 20px; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-badge {\n          position: absolute;\n          font-size: 10px;\n          right: -5px;\n          top: -5px;\n          width: 16px;\n          height: 16px;\n          text-align: center;\n          line-height: 16px;\n          color: #ffffff;\n          background-color: #ef6262;\n          -moz-border-radius: 50%;\n          -webkit-border-radius: 50%;\n          border-radius: 50%; }\n      .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search {\n        padding: 0;\n        position: relative;\n        display: inline-block;\n        top: -4px; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input {\n          display: inline-block;\n          border: 0 none;\n          font-size: 14px;\n          background: transparent;\n          border-bottom: 2px solid #ffffff;\n          outline: 0 none;\n          -webkit-box-shadow: none;\n          box-shadow: none;\n          color: #ffffff;\n          width: 100px;\n          padding: 1px 20px 1px 1px;\n          margin: 0px;\n          -moz-border-radius: 2px;\n          -webkit-border-radius: 2px;\n          border-radius: 2px; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input::-webkit-input-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input:-moz-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input::-moz-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input:-ms-input-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search .layout-topbar-search-icon {\n          font-size: 18px;\n          position: absolute;\n          top: -1px;\n          right: 0px; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input {\n          border-bottom-color: #77c7ff; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input::-webkit-input-placeholder {\n            opacity: 1; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input:-moz-placeholder {\n            opacity: 1; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input::-moz-placeholder {\n            opacity: 1; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input:-ms-input-placeholder {\n            opacity: 1; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover .layout-topbar-search-icon {\n          color: #77c7ff; }\n    .layout-wrapper .layout-topbar .layout-menu-button {\n      cursor: pointer;\n      display: inline-block;\n      text-decoration: none;\n      color: #ffffff;\n      -moz-transition: color 0.2s;\n      -o-transition: color 0.2s;\n      -webkit-transition: color 0.2s;\n      transition: color 0.2s; }\n      .layout-wrapper .layout-topbar .layout-menu-button span {\n        font-size: 2em; }\n      .layout-wrapper .layout-topbar .layout-menu-button:hover {\n        color: #77c7ff; }\n    .layout-wrapper .layout-topbar .layout-home-button {\n      cursor: pointer;\n      display: inline-block;\n      margin-left: 20px;\n      text-decoration: none;\n      color: #ffffff;\n      -moz-transition: color 0.2s;\n      -o-transition: color 0.2s;\n      -webkit-transition: color 0.2s;\n      transition: color 0.2s; }\n      .layout-wrapper .layout-topbar .layout-home-button span {\n        font-size: 2em; }\n      .layout-wrapper .layout-topbar .layout-home-button:hover {\n        color: #77c7ff; }\n    .layout-wrapper .layout-topbar a {\n      cursor: pointer; }\n  .layout-wrapper .p-scrollpanel {\n    background: transparent;\n    border-radius: 0;\n    border: none; }\n    .layout-wrapper .p-scrollpanel .p-scrollpanel-content {\n      overflow: scroll; }\n    .layout-wrapper .p-scrollpanel .p-scrollpanel-bar {\n      background: #aaaaaa;\n      opacity: 0.3;\n      filter: alpha(opacity=30); }\n    .layout-wrapper .p-scrollpanel .p-scrollpanel-hidden {\n      display: block;\n      visibility: hidden; }\n    .layout-wrapper .p-scrollpanel .layout-sidebar-scroll-content {\n      width: calc(100% + 18px);\n      padding-bottom: 120px; }\n  .layout-wrapper .layout-sidebar {\n    position: fixed;\n    width: 250px;\n    height: 100%;\n    z-index: 999;\n    user-select: none;\n    -moz-user-select: none;\n    -webkit-user-select: none;\n    -moz-transition: left 0.2s;\n    -o-transition: left 0.2s;\n    -webkit-transition: left 0.2s;\n    transition: left 0.2s;\n    background: #f3f4f9;\n    /* Old browsers */\n    background: -moz-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* FF3.6+ */\n    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #f3f4f9), color-stop(100%, #d7dbe8));\n    /* Chrome,Safari4+ */\n    background: -webkit-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* Chrome10+,Safari5.1+ */\n    background: -o-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* Opera 11.10+ */\n    background: -ms-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* IE10+ */\n    background: linear-gradient(to bottom, #f3f4f9 0%, #d7dbe8 100%);\n    /* W3C */\n    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=\'#ffffff\', endColorstr=\'#000000\',GradientType=0 );\n    /* IE6-9 */\n    -webkit-box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.16);\n    -moz-box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.16);\n    box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.16); }\n    .layout-wrapper .layout-sidebar .layout-logo {\n      text-align: center;\n      margin-top: 24px; }\n    .layout-wrapper .layout-sidebar .profile {\n      text-align: center;\n      padding: 20px 0; }\n      .layout-wrapper .layout-sidebar .profile img {\n        width: 56px;\n        margin: 10px; }\n      .layout-wrapper .layout-sidebar .profile .profile-link {\n        cursor: pointer;\n        color: #232428;\n        display: inline-block;\n        margin-bottom: 10px;\n        -moz-transition: color 0.2s;\n        -o-transition: color 0.2s;\n        -webkit-transition: color 0.2s;\n        transition: color 0.2s; }\n        .layout-wrapper .layout-sidebar .profile .profile-link i {\n          display: inline-block;\n          font-size: 16px; }\n        .layout-wrapper .layout-sidebar .profile .profile-link:hover {\n          color: #0388e5; }\n      .layout-wrapper .layout-sidebar .profile > ul {\n        overflow: hidden;\n        background-color: #ffffff;\n        text-align: left;\n        max-height: 0;\n        -moz-transition-duration: 0.2s;\n        -webkit-transition-duration: 0.2s;\n        -o-transition-duration: 0.2s;\n        transition-duration: 0.2s;\n        -webkit-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -moz-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -o-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1); }\n        .layout-wrapper .layout-sidebar .profile > ul.profile-expanded {\n          max-height: 500px; }\n        .layout-wrapper .layout-sidebar .profile > ul li a {\n          border: 0 none; }\n        .layout-wrapper .layout-sidebar .profile > ul li:last-child > a {\n          border: 0 none; }\n    .layout-wrapper .layout-sidebar ul {\n      list-style-type: none;\n      margin: 0;\n      padding: 0; }\n      .layout-wrapper .layout-sidebar ul li a {\n        cursor: pointer;\n        position: relative;\n        /* color: #232428; */\n        text-decoration: none;\n        font-size: 14px;\n        padding: 1em 15px 1em 1em;\n        display: block;\n        border-top: 1px solid rgba(207, 211, 224, 0.6); }\n        .layout-wrapper .layout-sidebar ul li a i {\n          font-size: 18px;\n          vertical-align: middle; }\n        .layout-wrapper .layout-sidebar ul li a span {\n          margin-left: .25em;\n          vertical-align: middle; }\n        .layout-wrapper .layout-sidebar ul li a .menuitem-toggle-icon {\n          float: right; }\n        .layout-wrapper .layout-sidebar ul li a:hover {\n          color: #0388e5; }\n      /* .layout-wrapper .layout-sidebar ul li.active-menuitem > a {\n        background-color: #ffffff;\n        color: #0388e5; } */\n        .layout-wrapper .layout-sidebar ul li.active-menuitem > a .menuitem-toggle-icon:before {\n          content: ""; }\n      .layout-wrapper .layout-sidebar ul li.active-menuitem > ul {\n        max-height: 500px; }\n      .layout-wrapper .layout-sidebar ul li ul {\n        background-color: #ffffff;\n        overflow: hidden;\n        margin-left: 1.5em;\n        max-height: 0;\n        -webkit-transition-property: max-height;\n        -moz-transition-property: max-height;\n        -ms-transition-property: max-height;\n        -o-transition-property: max-height;\n        transition-property: max-height;\n        -moz-transition-duration: 0.4s;\n        -webkit-transition-duration: 0.4s;\n        -o-transition-duration: 0.4s;\n        transition-duration: 0.4s;\n        -webkit-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -moz-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -o-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1); }\n        .layout-wrapper .layout-sidebar ul li ul li a {\n          cursor: pointer;\n          padding: .75em 33px .75em .75em;\n          font-size: 13px;\n          border-top: 0 none; }\n        .layout-wrapper .layout-sidebar ul li ul li:last-child > a {\n          border-bottom: 0 none; }\n      .layout-wrapper .layout-sidebar ul li:last-child > a {\n        border-bottom: 1px solid rgba(207, 211, 224, 0.6); }\n      .layout-wrapper .layout-sidebar ul .menuitem-toggle-icon {\n        float: right;\n        margin-top: 2px; }\n      .layout-wrapper .layout-sidebar ul .menuitem-badge {\n        margin-top: 3px;\n        font-size: 10px;\n        float: right;\n        width: 16px;\n        height: 16px;\n        line-height: 16px;\n        text-align: center;\n        color: #ffffff;\n        background-color: #007be5;\n        -moz-border-radius: 50%;\n        -webkit-border-radius: 50%;\n        border-radius: 50%; }\n    .layout-wrapper .layout-sidebar.layout-sidebar-dark {\n      background: #4d505b;\n      /* Old browsers */\n      background: -moz-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* FF3.6+ */\n      background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #4d505b), color-stop(100%, #3b3e47));\n      /* Chrome,Safari4+ */\n      background: -webkit-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* Chrome10+,Safari5.1+ */\n      background: -o-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* Opera 11.10+ */\n      background: -ms-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* IE10+ */\n      background: linear-gradient(to bottom, #4d505b 0%, #3b3e47 100%);\n      /* W3C */\n      filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=\'#ffffff\', endColorstr=\'#000000\',GradientType=0 );\n      /* IE6-9 */ }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > a {\n        color: #ffffff; }\n        .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > a:hover {\n          color: #0388e5; }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > ul {\n        background-color: #2e3035; }\n        .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > ul li a {\n          border: 0 none; }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li a {\n        /* color: #ffffff; */\n        border-top: 1px solid rgba(52, 56, 65, 0.6); }\n        /* .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li a:hover {\n          color: #0388e5; } */\n      /* .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li.active-menuitem > a {\n        background-color: #2e3035;\n        color: #0388e5; } */\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li ul {\n        background-color: #2e3035; }\n        .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li ul li a {\n          border: none; }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li:last-child > a {\n        border-bottom: 1px solid rgba(52, 56, 65, 0.6); }\n  .layout-wrapper .layout-main {\n    -moz-transition: margin-left 0.2s;\n    -o-transition: margin-left 0.2s;\n    -webkit-transition: margin-left 0.2s;\n    transition: margin-left 0.2s;\n    padding: 66px 16px 16px 16px;\n    display: flex;\n    flex-direction: column;\n    height: 100vh; }\n  .layout-wrapper .layout-footer {\n    -moz-transition: margin-left 0.2s;\n    -o-transition: margin-left 0.2s;\n    -webkit-transition: margin-left 0.2s;\n    transition: margin-left 0.2s;\n    background-color: #ffffff;\n    padding: 1em 2em; }\n    .layout-wrapper .layout-footer img {\n      vertical-align: middle; }\n    .layout-wrapper .layout-footer .footer-text {\n      vertical-align: middle; }\n\n/*.lino-main {\n    flex: auto;\n    display: flex;\n    flex-direction: column;\n}*/\n.dashboard-item-closed {\n  display: none; }\n\n.p-panel {\n  height: inherit; }\n  .p-panel .p-panel-content {\n    height: inherit; }\n  .p-panel .p-toggleable-content {\n    height: inherit; }\n\nbody .lino-panel.p-tabview .p-tabview-panels {\n  padding: .5ch 0.7ch;\n}\n.lino-panel.p-tabview-panel {\n    display: inline;\n}\n.l-panel {\n  height: 100%;\n  width: 100%;\n  flex: auto;\n  display: flex; }\n  .l-panel .l-component {\n    width: 100%;\n    padding: .25em;}\n    .l-panel .l-component .l-label {\n      font-weight: lighter;\n      border-bottom: dotted 1px;\n      white-space: nowrap; }\n      .l-panel .l-component .l-label.l-label--unfilled {\n        color: grey; }\n    .l-panel .l-component .p-checkbox.p-component {\n      padding-top: .5ch; }\n\n.p-autocomplete-list-item {\n  min-height: 28.7px; }\n\nbody .l-ForeignKeyElement {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  margin-right: 1ch;\n  position: relative; }\n  body .l-ForeignKeyElement .p-autocomplete.p-component {\n    width: 100%; }\n  body .l-ForeignKeyElement .l-fk-clear {\n    position: absolute;\n    right: 2.7em;\n    top: 50%;\n    font-size: 1em;\n    height: 1em;\n    margin-top: -.5em;\n    color: #848484; }\n  body .l-ForeignKeyElement .l-fk-clear::before {\n    content: "\\E90B"; }\n  body .l-ForeignKeyElement .l-button-fk {\n    margin-left: 1em;\n    height: 1.5em;\n    width: 1.5em;\n    margin-top: 3px; }\n  body .l-ForeignKeyElement .p-autocomplete {\n    display: inherit; }\n    body .l-ForeignKeyElement .p-autocomplete .p-autocomplete-items > li {\n      min-height: 32px; }\n    body .l-ForeignKeyElement .p-autocomplete .p-autocomplete-dropdown {\n      max-width: 2.257em; }\n  body .l-ForeignKeyElement input {\n    width: calc(100% - 2.357em); }\n  body .l-ForeignKeyElement label {\n    white-space: nowrap; }\n\n.p-calendar input {\n  width: 100%; }\n\n.l-ChoiceListFieldElement .p-dropdown.p-component {\n  padding-right: 1px; }\n\n.l-ChoiceListFieldElement .p-dropdown-clearable > label {\n  margin-right: 16px; }\n\n.l-ChoiceListFieldElement > div {\n  min-width: unset; }\n\n.l-ChoiceListFieldElement label {\n  margin-top: 1px;\n  margin-left: 1px; }\n\n.l-panel-vertical {\n  flex-direction: column; }\n\n.lino-loading-mask {\n  position: absolute;\n  width: 100%;\n  height: 100%;\n  z-index: 9999;\n  opacity: .2;\n  border-radius: 5px; }\n\n.lino-loading-mask > div {\n  position: absolute;\n  top: 50%;\n  right: 50%;\n  transform: translate(50%, -50%); }\n\n.lino-transparent {\n  opacity: 0; }\n\n.l-actas {\n  max-height: calc(-250px + 100vh); }\n  .l-actas .p-card-content {\n    max-height: calc(100vh - 372px);\n    overflow-x: hidden;\n    overflow-y: auto; }\n  .l-actas .p-button {\n    width: 100%;\n    margin-bottom: 2px; }\n\n.p-tabview {\n  flex: auto;\n  display: flex;\n  flex-direction: column; }\n\n.p-tabview-panels {\n  flex: auto;\n  display: flex;\n  flex-direction: column; }\n\n.p-tabview-panel {\n  flex: auto;\n  display: flex; }\n\n.l-editor-wrapper > div {\n  width: 100%;\n  height: 100%; }\n\n.l-editor-wrapper > div > div {\n  width: 100%;\n  height: 100%; }\n\n.p-editor-container {\n  height: 100%;\n  padding-bottom: .5ch;\n  padding-top: .5ch;\n  width: 100%; }\n\n.p-dialog {\n  max-width: 100vw; }\n  .p-dialog .p-dialog-content {\n    max-height: 78vh;\n    width: 100%; }\n    @media (max-width: 600px) {\n      .p-dialog .p-dialog-content {\n        overflow: scroll; } }\n  .p-dialog .p-fileupload-content {\n    min-height: 150px;\n    max-height: 300px;\n    overflow-y: scroll;\n    overflow-x: hidden; }\n\n.p-panel-content {\n  flex: auto; }\n\n.p-panel-content-wrapper-expanded {\n  flex: auto;\n  display: flex; }\n\n.l-slave-summary-panel .p-panel-content .p-button:first-child {\n  float: right;\n  margin-top: -44px; }\n\nbody .p-datatable .p-datatable-tbody > tr.p-highlight a {\n  color: #333333; }\n\nbody table p {\n  margin: unset; }\n\nbody .layout-wrapper .layout-sidebar ul li.active-menuitem > ul {\n  max-height: 200vh; }\n\nbody .l-bbar > * {\n  margin-right: 2px;\n  margin-bottom: 1px; }\n\nbody .l-grid .p-dataview .p-panel-header {\n  padding: 0px 1ch; }\n\nbody .l-grid .p-dataview .p-panel-content {\n  padding-top: 1ch;\n  padding-left: 1ch; }\n\nbody .l-grid .p-dataview p {\n  margin: unset; }\n\n.table-header {\n  display: flex;\n  justify-content: space-between;\n}\n  body .l-grid .table-header .l-DataViewLayoutOptions {\n    display: inline; }\n\nbody .l-grid .p-datatable .p-datatable-thead > tr > th {\n  border-bottom-width: 3px; }\n\nbody .l-grid .p-datatable .p-datatable-tbody > tr > td.p-cell-editing {\n  overflow: unset; }\n  body .l-grid .p-datatable .p-datatable-tbody > tr > td.p-cell-editing .p-datepicker {\n    min-width: max-content;\n    position: fixed;\n    left: unset !important;\n    top: unset !important;\n    width: auto; }\n    body .l-grid .p-datatable .p-datatable-tbody > tr > td.p-cell-editing .p-datepicker table.p-datepicker-calendar {\n      display: block; }\n\nbody .l-grid .p-datatable .p-datatable-header {\n  padding: 0.15em 0.25em; }\n\nbody .l-grid .p-datatable .p-paginator {\n  position: relative; }\n  body .l-grid .p-datatable .p-paginator .p-paginator-right-content {\n    position: absolute;\n    top: 50%;\n    right: 2ch;\n    transform: translateY(-50%); }\n\nbody .l-grid .p-datatable .l-DateFieldElement input {\n  margin-right: -2.357em; }\n\nbody .l-grid .p-datatable .l-DateFieldElement .p-datepicker-trigger {\n  width: 2.357em !important; }\n\n.no-ws {\n  color: grey !important; }\n\n.l-itemTemplate {\n  width: 100%; }\n\n.chatwindow-chats > .p-scrollpanel-content {\n  display: flex;\n  flex-direction: column;\n  margin-top: .6ch; }\n  .chatwindow-chats > .p-scrollpanel-content > div {\n    margin-top: .7ch; }\n\n.chatwindow {\n  max-width: 284px; }\n  .chatwindow .user {\n    font-size: x-small;\n    text-transform: capitalize; }\n  .chatwindow .not-sent .message {\n    background: gray !important; }\n  .chatwindow .message {\n    transition: background-color 1000ms linear;\n    border-radius: 10px;\n    background: #06b4f1;\n    padding-left: 1ch;\n    padding-right: 1ch;\n    overflow-wrap: break-word;\n    max-width: 100%; }\n  .chatwindow .p-scrollpanel-wrapper {\n    border-right: 9px solid #f4f4f4; }\n  .chatwindow .p-scrollpanel-bar {\n    background-color: #1976d2;\n    opacity: 1;\n    transition: background-color .3s; }\n  .chatwindow .p-scrollpanel-bar:hover {\n    background-color: #135ba1; }\n  .chatwindow .p-editor-toolbar {\n    border-top: unset !important;\n    padding: unset !important; }\n  .chatwindow .p-editor-container {\n    padding-bottom: unset; }\n\nbody .l-detail-toolbar .p-toolbar-group-left {\n  display: block; }\n\nbody .l-detail-toolbar .p-button {\n  margin-right: 2px;\n  margin-bottom: 1px; }\n\n@media (max-width: 600px) {\n  .l-panel {\n    flex-direction: column; }\n    .l-panel .l-component {\n      padding-left: unset;\n      padding-right: unset; } }\n\n/* Responsive  larger than 1025px*/\n@media (min-width: 1025px) {\n  .layout-wrapper.layout-overlay .layout-sidebar {\n    left: -250px; }\n  .layout-wrapper.layout-overlay .layout-topbar {\n    left: 0; }\n  .layout-wrapper.layout-overlay .layout-main, .layout-wrapper.layout-overlay .layout-footer {\n    margin-left: 0; }\n  .layout-wrapper.layout-overlay.layout-overlay-sidebar-active .layout-sidebar {\n    left: 0; }\n  .layout-wrapper.layout-overlay.layout-overlay-sidebar-active .layout-topbar {\n    left: 250px; }\n  .layout-wrapper.layout-static .layout-sidebar {\n    left: 0; }\n  .layout-wrapper.layout-static .layout-topbar {\n    left: 250px; }\n  .layout-wrapper.layout-static .layout-main, .layout-wrapper.layout-static .layout-footer {\n    margin-left: 250px; }\n  .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-sidebar {\n    left: -250px; }\n  .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-topbar {\n    left: 0; }\n  .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-main, .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-footer {\n    margin-left: 0; } }\n\n@media (max-width: 1024px) {\n  .layout-wrapper .layout-topbar {\n    left: 0; }\n    .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-item-text {\n      display: none; }\n  .layout-wrapper .layout-main, .layout-wrapper .layout-footer {\n    margin-left: 0; }\n  .layout-wrapper .layout-sidebar {\n    left: -250px;\n    margin-top: 50px; }\n  .layout-wrapper .layout-mask {\n    display: none;\n    position: fixed;\n    width: 100%;\n    height: 100%;\n    top: 50px;\n    left: 0;\n    z-index: 998;\n    background-color: #424242;\n    opacity: 0.7;\n    filter: alpha(opacity=70); }\n  .layout-wrapper.layout-mobile-sidebar-active .layout-sidebar {\n    left: -0; }\n  .layout-wrapper.layout-mobile-sidebar-active .layout-mask {\n    display: block; }\n  .body-overflow-hidden {\n    overflow: hidden; } }\n\n/* Typography */\nh1 {\n  font-weight: normal;\n  margin: 0;\n  font-size: 24px; }\n\nh2 {\n  font-size: 20px;\n  font-weight: normal;\n  margin: 0; }\n\n.card {\n  background-color: #ffffff;\n  padding: 1em;\n  margin-bottom: 16px;\n  -moz-border-radius: 3px;\n  -webkit-border-radius: 3px;\n  border-radius: 3px; }\n  .card.card-w-title {\n    padding-bottom: 2em; }\n  .card h1 {\n    margin: .5em 0 .5em 0;\n    border-bottom: 1px solid #d5d5d5;\n    padding: .1em;\n    font-size: 24px; }\n    .card h1:first-child {\n      margin: 0 0 .5em 0; }\n\n.p-g {\n  -ms-flex-wrap: wrap; }\n\n/* Dashboard */\n.dashboard .summary {\n  position: relative; }\n  .dashboard .summary .title {\n    font-size: 20px; }\n  .dashboard .summary .detail {\n    color: #707070;\n    display: block;\n    margin-top: 10px; }\n  .dashboard .summary .count {\n    color: #ffffff;\n    position: absolute;\n    top: 10px;\n    right: 10px;\n    font-size: 24px;\n    padding: 7px 14px;\n    -moz-border-radius: 3px;\n    -webkit-border-radius: 3px;\n    border-radius: 3px; }\n    .dashboard .summary .count.visitors {\n      background-color: #20d077; }\n    .dashboard .summary .count.purchases {\n      background-color: #f9c851; }\n    .dashboard .summary .count.revenue {\n      background-color: #007be5; }\n\n.dashboard .highlight-box {\n  height: 100px; }\n  .dashboard .highlight-box:after {\n    content: "";\n    display: table;\n    clear: both; }\n  .dashboard .highlight-box .initials {\n    height: 100%;\n    float: left;\n    width: 50%;\n    text-align: center;\n    padding: 1em; }\n    .dashboard .highlight-box .initials > span {\n      font-size: 48px; }\n  .dashboard .highlight-box .highlight-details {\n    height: 100%;\n    background-color: #ffffff;\n    float: left;\n    width: 50%;\n    padding: 1em; }\n    .dashboard .highlight-box .highlight-details i {\n      font-size: 24px;\n      vertical-align: middle;\n      margin-right: .25em; }\n    .dashboard .highlight-box .highlight-details .count {\n      color: #707070;\n      font-size: 36px;\n      display: block; }\n\n.dashboard .task-list {\n  list-style-type: none;\n  margin: 0;\n  padding: 0; }\n  .dashboard .task-list li {\n    padding: .5em .25em;\n    border-bottom: 1px solid #e3e3e3; }\n    .dashboard .task-list li:after {\n      content: "";\n      display: table;\n      clear: both; }\n  .dashboard .task-list .p-checkbox {\n    vertical-align: middle;\n    margin-right: .5em; }\n  .dashboard .task-list .task-name {\n    vertical-align: middle; }\n  .dashboard .task-list .p-button {\n    float: right; }\n    .dashboard .task-list .p-button .p-button-text {\n      padding: .125em; }\n  .dashboard .task-list .p-panel-content {\n    min-height: 256px; }\n\n.dashboard .contact-form .p-panel-content {\n  min-height: 256px; }\n\n.dashboard .contacts ul {\n  list-style-type: none;\n  padding: 0;\n  margin: 0; }\n  .dashboard .contacts ul li {\n    border-bottom: 1px solid #e3e3e3; }\n    .dashboard .contacts ul li a {\n      padding: 9px;\n      width: 100%;\n      box-sizing: border-box;\n      text-decoration: none;\n      position: relative;\n      display: block;\n      -moz-border-radius: 2px;\n      -webkit-border-radius: 2px;\n      border-radius: 2px;\n      -moz-transition: background-color 0.2s;\n      -o-transition: background-color 0.2s;\n      -webkit-transition: background-color 0.2s;\n      transition: background-color 0.2s; }\n      .dashboard .contacts ul li a .name {\n        position: absolute;\n        right: 10px;\n        top: 10px;\n        font-size: 18px; }\n      .dashboard .contacts ul li a .email {\n        position: absolute;\n        right: 10px;\n        top: 30px;\n        font-size: 14px;\n        color: #707070; }\n      .dashboard .contacts ul li a:hover {\n        cursor: pointer;\n        background-color: #eeeeee; }\n    .dashboard .contacts ul li:last-child {\n      border: 0; }\n\n.dashboard .contacts .p-panel-content {\n  min-height: 256px; }\n\n.dashboard .activity-list {\n  list-style-type: none;\n  padding: 0;\n  margin: 0; }\n  .dashboard .activity-list li {\n    border-bottom: 1px solid #e3e3e3;\n    padding: 16px 8px; }\n    .dashboard .activity-list li .count {\n      font-size: 24px;\n      color: #ffffff;\n      background-color: #007be5;\n      font-weight: 700;\n      display: inline-block;\n      padding: .25em .5em;\n      -moz-border-radius: 3px;\n      -webkit-border-radius: 3px;\n      border-radius: 3px; }\n    .dashboard .activity-list li:first-child {\n      border-top: 1px solid #e3e3e3; }\n    .dashboard .activity-list li:last-child {\n      border: 0; }\n    .dashboard .activity-list li .p-g-6:first-child {\n      font-size: 18px;\n      padding-left: 0; }\n    .dashboard .activity-list li .p-g-6:last-child {\n      text-align: right;\n      color: #707070; }\n\n/*!\n * Quill Editor v1.0.0-beta.3\n * https://quilljs.com/\n * Copyright (c) 2014, Jason Chen\n * Copyright (c) 2013, salesforce.com\n */\n.ql-container {\n  box-sizing: border-box;\n  font-family: Helvetica, Arial, sans-serif;\n  font-size: 13px;\n  height: 100%;\n  margin: 0px;\n  position: relative; }\n\n.ql-clipboard {\n  left: -100000px;\n  position: absolute;\n  top: 50%; }\n\n.ql-clipboard p {\n  margin: 0;\n  padding: 0; }\n\n.ql-editor {\n  box-sizing: border-box;\n  cursor: text;\n  line-height: 1.42;\n  height: 100%;\n  outline: none;\n  overflow-y: auto;\n  padding: 12px 15px;\n  tab-size: 4;\n  text-align: left;\n  white-space: pre-wrap; }\n\n.ql-editor p,\n.ql-editor ol,\n.ql-editor ul,\n.ql-editor pre,\n.ql-editor blockquote,\n.ql-editor h1,\n.ql-editor h2,\n.ql-editor h3,\n.ql-editor h4,\n.ql-editor h5,\n.ql-editor h6 {\n  margin: 0;\n  padding: 0;\n  counter-reset: list-1 list-2 list-3 list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol {\n  padding-left: 20px; }\n\n.ql-editor ul {\n  padding-left: 8px;\n  list-style: disc inside; }\n\n.ql-editor ol > li {\n  list-style-type: none; }\n\n.ql-editor ol {\n  list-style-type: none;\n  position: relative; }\n\n.ql-editor ol li {\n  counter-reset: list-1 list-2 list-3 list-4 list-5 list-6 list-7 list-8;\n  counter-increment: list-num; }\n\n.ql-editor ol li:before {\n  content: counter(list-num, decimal) ". ";\n  margin-right: -16px;\n  position: absolute;\n  right: 100%;\n  text-align: right; }\n\n.ql-editor ol li.ql-indent-1 {\n  counter-increment: list-1; }\n\n.ql-editor ol li.ql-indent-1:before {\n  content: counter(list-1, lower-alpha) ". ";\n  margin-right: -56px; }\n\n.ql-editor ol li.ql-indent-1 {\n  counter-reset: list-2 list-3 list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-2 {\n  counter-increment: list-2; }\n\n.ql-editor ol li.ql-indent-2:before {\n  content: counter(list-2, lower-roman) ". ";\n  margin-right: -96px; }\n\n.ql-editor ol li.ql-indent-2 {\n  counter-reset: list-3 list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-3 {\n  counter-increment: list-3; }\n\n.ql-editor ol li.ql-indent-3:before {\n  content: counter(list-3, decimal) ". ";\n  margin-right: -136px; }\n\n.ql-editor ol li.ql-indent-3 {\n  counter-reset: list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-4 {\n  counter-increment: list-4; }\n\n.ql-editor ol li.ql-indent-4:before {\n  content: counter(list-4, lower-alpha) ". ";\n  margin-right: -176px; }\n\n.ql-editor ol li.ql-indent-4 {\n  counter-reset: list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-5 {\n  counter-increment: list-5; }\n\n.ql-editor ol li.ql-indent-5:before {\n  content: counter(list-5, lower-roman) ". ";\n  margin-right: -216px; }\n\n.ql-editor ol li.ql-indent-5 {\n  counter-reset: list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-6 {\n  counter-increment: list-6; }\n\n.ql-editor ol li.ql-indent-6:before {\n  content: counter(list-6, decimal) ". ";\n  margin-right: -256px; }\n\n.ql-editor ol li.ql-indent-6 {\n  counter-reset: list-7 list-8; }\n\n.ql-editor ol li.ql-indent-7 {\n  counter-increment: list-7; }\n\n.ql-editor ol li.ql-indent-7:before {\n  content: counter(list-7, lower-alpha) ". ";\n  margin-right: -296px; }\n\n.ql-editor ol li.ql-indent-7 {\n  counter-reset: list-8; }\n\n.ql-editor ol li.ql-indent-8 {\n  counter-increment: list-8; }\n\n.ql-editor ol li.ql-indent-8:before {\n  content: counter(list-8, lower-roman) ". ";\n  margin-right: -336px; }\n\n.ql-editor .ql-indent-1 {\n  padding-left: 40px; }\n\n.ql-editor .ql-indent-2 {\n  padding-left: 80px; }\n\n.ql-editor .ql-indent-3 {\n  padding-left: 120px; }\n\n.ql-editor .ql-indent-4 {\n  padding-left: 160px; }\n\n.ql-editor .ql-indent-5 {\n  padding-left: 200px; }\n\n.ql-editor .ql-indent-6 {\n  padding-left: 240px; }\n\n.ql-editor .ql-indent-7 {\n  padding-left: 280px; }\n\n.ql-editor .ql-indent-8 {\n  padding-left: 320px; }\n\n.ql-editor .ql-video {\n  display: block; }\n\n.ql-editor .ql-video.ql-align-center {\n  margin: 0 auto; }\n\n.ql-editor .ql-video.ql-align-right {\n  margin: 0 0 0 auto; }\n\n.ql-editor .ql-bg-black {\n  background-color: #000; }\n\n.ql-editor .ql-bg-red {\n  background-color: #e60000; }\n\n.ql-editor .ql-bg-orange {\n  background-color: #f90; }\n\n.ql-editor .ql-bg-yellow {\n  background-color: #ff0; }\n\n.ql-editor .ql-bg-green {\n  background-color: #008a00; }\n\n.ql-editor .ql-bg-blue {\n  background-color: #06c; }\n\n.ql-editor .ql-bg-purple {\n  background-color: #93f; }\n\n.ql-editor .ql-color-white {\n  color: #fff; }\n\n.ql-editor .ql-color-red {\n  color: #e60000; }\n\n.ql-editor .ql-color-orange {\n  color: #f90; }\n\n.ql-editor .ql-color-yellow {\n  color: #ff0; }\n\n.ql-editor .ql-color-green {\n  color: #008a00; }\n\n.ql-editor .ql-color-blue {\n  color: #06c; }\n\n.ql-editor .ql-color-purple {\n  color: #93f; }\n\n.ql-editor .ql-font-serif {\n  font-family: Georgia, Times New Roman, serif; }\n\n.ql-editor .ql-font-monospace {\n  font-family: Monaco, Courier New, monospace; }\n\n.ql-editor .ql-size-small {\n  font-size: 10px; }\n\n.ql-editor .ql-size-large {\n  font-size: 18px; }\n\n.ql-editor .ql-size-huge {\n  font-size: 32px; }\n\n.ql-editor .ql-direction-rtl {\n  direction: rtl;\n  text-align: inherit; }\n\n.ql-editor .ql-align-center {\n  text-align: center; }\n\n.ql-editor .ql-align-justify {\n  text-align: justify; }\n\n.ql-editor .ql-align-right {\n  text-align: right; }\n\n.ql-editor.ql-blank::before {\n  color: rgba(0, 0, 0, 0.6);\n  content: attr(data-placeholder);\n  font-style: italic;\n  pointer-events: none;\n  position: absolute; }\n\n.ql-hidden {\n  display: none; }\n\n.ql-tooltip {\n  position: absolute; }\n\n.ql-tooltip a {\n  cursor: pointer;\n  text-decoration: none; }\n\n.ql-toolbar:before,\n.ql-toolbar:after {\n  content: \' \';\n  display: table; }\n\n.ql-toolbar:after {\n  clear: both; }\n\n.ql-toolbar button {\n  background: none;\n  border: none;\n  cursor: pointer;\n  display: inline-block;\n  float: left;\n  height: 24px;\n  outline: none;\n  padding: 3px 5px;\n  width: 24px; }\n\n.ql-toolbar button svg {\n  height: 100%; }\n\n.ql-toolbar .ql-stroke {\n  fill: none;\n  stroke-linecap: round;\n  stroke-linejoin: round;\n  stroke-width: 2; }\n\n.ql-toolbar .ql-stroke-mitter {\n  fill: none;\n  stroke-mitterlimit: 10;\n  stroke-width: 2; }\n\n.ql-toolbar .ql-empty {\n  fill: none; }\n\n.ql-toolbar .ql-even {\n  fill-rule: evenodd; }\n\n.ql-toolbar .ql-thin,\n.ql-toolbar .ql-stroke.ql-thin {\n  stroke-width: 1; }\n\n.ql-toolbar .ql-transparent {\n  opacity: 0.4; }\n\n.ql-editor h1 {\n  font-size: 2em; }\n\n.ql-editor h2 {\n  font-size: 1.5em; }\n\n.ql-editor h3 {\n  font-size: 1.17em; }\n\n.ql-editor h4 {\n  font-size: 1em; }\n\n.ql-editor h5 {\n  font-size: 0.83em; }\n\n.ql-editor h6 {\n  font-size: 0.67em; }\n\n.ql-editor pre {\n  white-space: pre-wrap; }\n\n.ql-editor a {\n  text-decoration: underline; }\n\n.ql-editor blockquote {\n  border-left: 4px solid #ccc;\n  margin-bottom: 5px;\n  margin-top: 5px;\n  padding-left: 16px; }\n\n.ql-editor pre.hljs {\n  overflow: visible; }\n\n.ql-editor code,\n.ql-editor pre:not(.hljs) {\n  background-color: #f0f0f0; }\n\n.ql-editor code,\n.ql-editor pre {\n  border-radius: 3px; }\n\n.ql-editor code {\n  font-size: 85%;\n  padding-bottom: 2px;\n  padding-top: 2px; }\n\n.ql-editor code:before,\n.ql-editor code:after {\n  content: "\\A0";\n  letter-spacing: -2px; }\n\n.ql-editor *:not(pre) + pre,\n.ql-editor pre:first-of-type {\n  margin-top: 5px;\n  padding-top: 5px; }\n\n.ql-editor pre {\n  margin-bottom: 5px;\n  padding: 0px 10px 5px; }\n\n.ql-editor pre + pre {\n  margin-top: -10px; }\n\n.ql-editor img {\n  max-width: 100%; }\n\n.ql-snow .ql-image-tooltip {\n  padding: 10px;\n  text-align: center;\n  width: 300px; }\n\n.ql-snow .ql-image-tooltip input[type=text] {\n  height: 30px;\n  width: 100%; }\n\n.ql-snow .ql-image-tooltip a.ql-cancel,\n.ql-snow .ql-image-tooltip a.ql-action {\n  border: 1px solid #06c;\n  display: inline-block;\n  float: left;\n  line-height: 18px;\n  padding: 5px;\n  width: 50%; }\n\n.ql-snow .ql-image-tooltip a.ql-cancel::before {\n  color: #06c;\n  content: \'Cancel\'; }\n\n.ql-snow .ql-image-tooltip a.ql-action {\n  background-color: #06c; }\n\n.ql-snow .ql-image-tooltip a.ql-action::before {\n  color: #fff;\n  content: \'Insert\'; }\n\n.ql-snow .ql-image-tooltip .ql-preview {\n  height: 200px;\n  margin: 10px 0px;\n  position: relative; }\n\n.ql-snow .ql-image-tooltip .ql-preview img {\n  bottom: 0;\n  left: 0;\n  margin: auto;\n  max-height: 100%;\n  max-width: 100%;\n  position: absolute;\n  right: 0;\n  top: 0; }\n\n.ql-snow .ql-image-tooltip .ql-empty.ql-preview::before {\n  border: 1px dashed #ccc;\n  color: #ccc;\n  content: \'Preview\';\n  display: block;\n  line-height: 200px; }\n\n.ql-snow .ql-link-tooltip::before {\n  content: "Visit URL:";\n  line-height: 26px;\n  margin-right: 8px; }\n\n.ql-snow .ql-link-tooltip {\n  margin-top: 10px;\n  padding: 5px 12px;\n  white-space: nowrap; }\n\n.ql-snow .ql-link-tooltip input[type=text] {\n  display: none;\n  height: 26px;\n  width: 170px; }\n\n.ql-snow .ql-link-tooltip a.ql-preview {\n  display: inline-block;\n  max-width: 200px;\n  overflow-x: hidden;\n  text-overflow: ellipsis;\n  vertical-align: top; }\n\n.ql-snow .ql-link-tooltip a.ql-action::before {\n  color: #444;\n  content: \'-\';\n  line-height: 26px;\n  margin-left: 8px; }\n\n.ql-snow .ql-link-tooltip a.ql-action::after {\n  border-right: 1px solid #ccc;\n  content: \'Edit\';\n  margin-left: 8px;\n  padding-right: 8px; }\n\n.ql-snow .ql-link-tooltip a.ql-remove::before {\n  content: \'Remove\';\n  margin-left: 8px; }\n\n.ql-snow .ql-link-tooltip a {\n  line-height: 26px; }\n\n.ql-snow .ql-link-tooltip.ql-editing a.ql-preview,\n.ql-snow .ql-link-tooltip.ql-editing a.ql-remove {\n  display: none; }\n\n.ql-snow .ql-link-tooltip.ql-editing input[type=text] {\n  display: inline-block; }\n\n.ql-snow .ql-link-tooltip.ql-editing a.ql-action::after {\n  border-right: 0px;\n  content: \'Save\';\n  padding-right: 0px; }\n\n.ql-toolbar.ql-snow {\n  border: 1px solid #ccc;\n  box-sizing: border-box;\n  font-family: \'Helvetica Neue\', \'Helvetica\', \'Arial\', sans-serif;\n  padding: 8px; }\n\n.ql-toolbar.ql-snow * {\n  box-sizing: border-box; }\n\n.ql-toolbar.ql-snow .ql-formats {\n  display: inline-block;\n  margin-right: 15px;\n  vertical-align: middle; }\n\n.ql-toolbar.ql-snow button:hover,\n.ql-toolbar.ql-snow button.ql-active,\n.ql-toolbar.ql-snow .ql-picker-label:hover,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active,\n.ql-toolbar.ql-snow .ql-picker-item:hover,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected {\n  color: #06c; }\n\n.ql-toolbar.ql-snow button:hover .ql-fill,\n.ql-toolbar.ql-snow button.ql-active .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-fill,\n.ql-toolbar.ql-snow button:hover .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow button.ql-active .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-stroke.ql-fill {\n  fill: #06c; }\n\n.ql-toolbar.ql-snow button:hover .ql-stroke,\n.ql-toolbar.ql-snow button.ql-active .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-stroke,\n.ql-toolbar.ql-snow button:hover .ql-stroke-mitter,\n.ql-toolbar.ql-snow button.ql-active .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-stroke-mitter {\n  stroke: #06c; }\n\n.ql-toolbar.ql-snow .ql-stroke {\n  stroke: #444; }\n\n.ql-toolbar.ql-snow .ql-stroke-mitter {\n  stroke: #444; }\n\n.ql-toolbar.ql-snow .ql-fill,\n.ql-toolbar.ql-snow .ql-stroke.ql-fill {\n  fill: #444; }\n\n.ql-toolbar.ql-snow .ql-direction svg:last-child {\n  display: none; }\n\n.ql-toolbar.ql-snow .ql-direction.ql-active svg:last-child {\n  display: inline; }\n\n.ql-toolbar.ql-snow .ql-direction.ql-active svg:first-child {\n  display: none; }\n\n.ql-toolbar.ql-snow .ql-picker {\n  color: #444;\n  display: inline-block;\n  float: left;\n  font-size: 14px;\n  font-weight: 500;\n  height: 24px;\n  position: relative;\n  vertical-align: middle; }\n\n.ql-toolbar.ql-snow .ql-picker-label {\n  border: 1px solid transparent;\n  cursor: pointer;\n  display: inline-block;\n  height: 100%;\n  padding-left: 8px;\n  padding-right: 2px;\n  position: relative;\n  width: 100%; }\n\n.ql-toolbar.ql-snow .ql-picker-label svg {\n  float: right;\n  height: 18px;\n  margin-top: 2px;\n  width: 18px; }\n\n.ql-toolbar.ql-snow .ql-picker-label::before {\n  vertical-align: middle; }\n\n.ql-toolbar.ql-snow .ql-picker-options {\n  background-color: #fff;\n  border: 1px solid transparent;\n  display: none;\n  min-width: 100%;\n  padding: 4px 8px;\n  position: absolute;\n  white-space: nowrap; }\n\n.ql-toolbar.ql-snow .ql-picker-options .ql-picker-item {\n  cursor: pointer;\n  display: block;\n  padding-bottom: 5px;\n  padding-top: 5px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-label {\n  border-color: #ccc;\n  color: #ccc;\n  z-index: 2; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-label .ql-fill {\n  fill: #ccc; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-label .ql-stroke {\n  stroke: #ccc; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-options {\n  border-color: #ccc;\n  box-shadow: rgba(0, 0, 0, 0.2) 0 2px 8px;\n  display: block;\n  margin-top: -1px;\n  z-index: 1; }\n\n.ql-toolbar.ql-snow .ql-color-picker,\n.ql-toolbar.ql-snow .ql-icon-picker {\n  width: 28px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-label,\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-label {\n  padding: 2px 4px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-label svg,\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-label svg {\n  margin-top: 0px; }\n\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-options {\n  padding: 4px 0px; }\n\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-item {\n  height: 24px;\n  padding: 2px 4px; }\n\n.ql-toolbar.ql-snow .ql-color-picker.ql-expanded .ql-picker-options,\n.ql-toolbar.ql-snow .ql-icon-picker.ql-expanded .ql-picker-options {\n  margin-top: -6px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-options {\n  padding: 5px;\n  width: 152px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item {\n  border: 1px solid transparent;\n  float: left;\n  height: 16px;\n  margin: 2px;\n  padding: 0px;\n  width: 16px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item.ql-primary-color {\n  margin-bottom: toolbarPadding; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item.ql-selected,\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item:hover {\n  border-color: #000; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-label]:not([data-label=\'\'])::before {\n  content: attr(data-label); }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header {\n  width: 98px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item::before {\n  content: \'Normal\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="1"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="1"]::before {\n  content: \'Heading 1\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="2"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="2"]::before {\n  content: \'Heading 2\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="3"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="3"]::before {\n  content: \'Heading 3\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="4"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="4"]::before {\n  content: \'Heading 4\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="5"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="5"]::before {\n  content: \'Heading 5\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="6"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="6"]::before {\n  content: \'Heading 6\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="1"]::before {\n  font-size: 2em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="2"]::before {\n  font-size: 1.5em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="3"]::before {\n  font-size: 1.17em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="4"]::before {\n  font-size: 1em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="5"]::before {\n  font-size: 0.83em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="6"]::before {\n  font-size: 0.67em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font {\n  width: 108px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item::before {\n  content: \'Sans Serif\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label[data-value=serif]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=serif]::before {\n  content: \'Serif\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label[data-value=monospace]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=monospace]::before {\n  content: \'Monospace\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=serif]::before {\n  font-family: Georgia, Times New Roman, serif; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=monospace]::before {\n  font-family: Monaco, Courier New, monospace; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size {\n  width: 98px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item::before {\n  content: \'Normal\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-value=small]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=small]::before {\n  content: \'Small\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-value=large]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=large]::before {\n  content: \'Large\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-value=huge]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=huge]::before {\n  content: \'Huge\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=small]::before {\n  font-size: 10px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=large]::before {\n  font-size: 18px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=huge]::before {\n  font-size: 32px; }\n\n.ql-toolbar.ql-snow .ql-color-picker.ql-background .ql-picker-item {\n  background-color: #fff; }\n\n.ql-toolbar.ql-snow .ql-color-picker.ql-color .ql-picker-item {\n  background-color: #000; }\n\n.ql-toolbar.ql-snow + .ql-container.ql-snow {\n  border-top: 0px; }\n\n.ql-snow .ql-tooltip {\n  background-color: #fff;\n  border: 1px solid #ccc;\n  box-shadow: 0px 0px 5px #ddd;\n  color: #444; }\n\n.ql-snow .ql-tooltip input[type=text] {\n  border: 1px solid #ccc;\n  font-size: 13px;\n  margin: 0px;\n  padding: 3px 5px; }\n\n.ql-container.ql-snow {\n  border: 1px solid #ccc; }\n\n.ql-container.ql-snow a {\n  color: #06c; }\n\n.ql-container.ql-snow * {\n  box-sizing: border-box; }\n\n/* Lino calander CSS */\n.lino-nav-cal {\n    margin-left: 2ch;\n}\n\n.lino-nav-cal h2 {\n  margin-bottom: 2px;\n  white-space: nowrap; }\n\n.lino-nav-cal p {\n  margin: 0;\n  padding: 0; }\n\n.lino-nav-cal h2 > span {\n  width: 14ch;\n  display: inline-block; }\n\n.cal-week {\n  position: relative;\n  right: 2ch; }\n\n.cal-month-table {\n  /* \tdisplay: None; */\n  visibility: hidden;\n  opacity: 0;\n  transition: visibility 0s, opacity 0.5s linear;\n  position: absolute;\n  border: solid;\n  box-sizing: border-box;\n  background-color: #edf0f5;\n  z-index: 1;\n  padding: 12px;\n  border-color: blue;\n  display: inline-block;\n  transform: translate(-50%); }\n\n.cal-month-table a {\n  font-weight: normal; }\n\n.cal-month-cell div.header {\n  padding-bottom: 3px; }\n\n/*.cal-month-cell.other-month h3 a{*/\n/*color: #5c5c5c;*/\n/*}*/\n.cal-month-cell.cal-in-past a {\n  color: darkgray; }\n\n.cal-month-cell.cal-in-past div.header a {\n  color: unset; }\n\n.cal-MonthlyView table[name="cal.MonthlyPlanner.grid"] {\n  height: 100%; }\n\n.cal-MonthlyView table[name="cal.MonthlyPlanner.grid"] tr:nth-child(1) th {\n  height: 1ch; }\n\n.cal-WeeklyView table[name="cal.WeeklyPlanner.grid"] td > a {\n  margin-bottom: 3px;\n  display: block; }\n\n.cal-WeeklyView table[name="cal.WeeklyPlanner.grid"] tr td:nth-child(1) {\n  white-space: nowrap; }\n\n/*For extjs grid of cal view, never going to be used? */\n.cal-MonthlyView td.x-grid3-cell:not(.x-grid3-cell-first) {\n  color: #5c5c5c;\n  min-height: 14ch;\n  border: lightgray solid 1px;\n  padding: 3px;\n  box-sizing: border-box; }\n\n.cal-MonthlyView td.x-grid3-cell-first {\n  vertical-align: middle; }\n\n.lino-nav-cal span > span:hover .cal-month-table {\n  visibility: visible;\n  opacity: 1; }\n\n.other-month {\n  background-color: gainsboro; }\n\n.current-day {\n  background-color: #fbfbfb; }\n\n/* Have "..." overflow*/\n.fixed-table {\n  width: 100%;\n  height: 100%;\n  /*not really necessary, removes extra white space */\n  border-collapse: collapse;\n  border-spacing: 0;\n  border: 0; }\n\n.fixed-table tbody {\n  vertical-align: unset; }\n\n.fixed-table td div {\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis; }\n\n.dot {\n  height: 7px;\n  width: 7px;\n  border-radius: 50%;\n  display: inline-block;\n  vertical-align: middle;\n  margin-right: 0.3ch;\n  margin-left: 0.3ch;\n  margin-bottom: 0.5ch; }\n', ""]);
+                r.push([e.id, '@charset "UTF-8";\n/* General */\n/* Menu */\n/* Menu Dark*/\n/* Menu Light*/\n/* Topbar */\n/* Footer */\n.splash-screen {\n  width: 100%;\n  height: 100%;\n  position: fixed;\n  background: #0388E5;\n  /* Old browsers */\n  background: -moz-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* FF3.6+ */\n  background: -webkit-gradient(linear, left top, right top, color-stop(0%, #0388E5), color-stop(100%, #07BDF4));\n  /* Chrome,Safari4+ */\n  background: -webkit-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* Chrome10+,Safari5.1+ */\n  background: -o-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* Opera 11.10+ */\n  background: -ms-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n  /* IE10+ */\n  background: linear-gradient(to right, #0388E5 0%, #07BDF4 100%);\n  /* W3C */\n  filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=$left, endColorstr=$right,GradientType=1 );\n  /* IE6-9 */ }\n  .splash-screen .splash-container {\n    width: 40px;\n    height: 40px;\n    margin: 0px auto;\n    position: absolute;\n    left: 50%;\n    top: 50%;\n    margin-left: -20px;\n    margin-top: -20px; }\n  .splash-screen .splash-double-bounce1, .splash-screen .splash-double-bounce2 {\n    width: 100%;\n    height: 100%;\n    border-radius: 50%;\n    background-color: #ffffff;\n    opacity: 0.6;\n    position: absolute;\n    top: 0;\n    left: 0;\n    -webkit-animation: splash-bounce 2.0s infinite ease-in-out;\n    animation: splash-bounce 2.0s infinite ease-in-out; }\n  .splash-screen .splash-double-bounce2 {\n    -webkit-animation-delay: -1.0s;\n    animation-delay: -1.0s; }\n\n@-webkit-keyframes splash-bounce {\n  0%, 100% {\n    -webkit-transform: scale(0); }\n  50% {\n    -webkit-transform: scale(1); } }\n\n@keyframes splash-bounce {\n  0%, 100% {\n    transform: scale(0);\n    -webkit-transform: scale(0); }\n  50% {\n    transform: scale(1);\n    -webkit-transform: scale(1); } }\n\n* {\n  box-sizing: border-box; }\n\nhtml {\n  height: 100%; }\n\nbody {\n  font-family: "Open Sans", "Helvetica Neue", sans-serif;\n  font-size: 14px;\n  color: #333333;\n  background-color: #edf0f5;\n  margin: 0;\n  padding: 0;\n  min-height: 100%; }\n\na {\n  text-decoration: none; }\n\n.layout-wrapper {\n  padding: 0; }\n  .layout-wrapper .layout-topbar {\n    position: fixed;\n    padding: .7em 1.5em .7em 1.5em;\n    color: #ffffff;\n    z-index: 999;\n    right: 0;\n    background: #0388E5;\n    /* Old browsers */\n    background: -moz-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* FF3.6+ */\n    background: -webkit-gradient(linear, left top, right top, color-stop(0%, #0388E5), color-stop(100%, #07BDF4));\n    /* Chrome,Safari4+ */\n    background: -webkit-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* Chrome10+,Safari5.1+ */\n    background: -o-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* Opera 11.10+ */\n    background: -ms-linear-gradient(left, #0388E5 0%, #07BDF4 100%);\n    /* IE10+ */\n    background: linear-gradient(to right, #0388E5 0%, #07BDF4 100%);\n    /* W3C */\n    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=$left, endColorstr=$right,GradientType=1 );\n    /* IE6-9 */\n    -moz-transition: left 0.2s;\n    -o-transition: left 0.2s;\n    -webkit-transition: left 0.2s;\n    transition: left 0.2s; }\n    .layout-wrapper .layout-topbar .layout-topbar-icons {\n      float: right;\n      display: block;\n      -moz-animation-duration: .5s;\n      -webkit-animation-duration: .5s;\n      animation-duration: .5s; }\n      .layout-wrapper .layout-topbar .layout-topbar-icons a {\n        position: relative;\n        color: #ffffff;\n        margin-left: 20px;\n        display: inline-block;\n        text-decoration: none;\n        -moz-transition: color 0.2s;\n        -o-transition: color 0.2s;\n        -webkit-transition: color 0.2s;\n        transition: color 0.2s; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a:hover {\n          color: #77c7ff; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-icon {\n          font-size: 2em; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-item-text {\n          font-size: 20px; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-badge {\n          position: absolute;\n          font-size: 10px;\n          right: -5px;\n          top: -5px;\n          width: 16px;\n          height: 16px;\n          text-align: center;\n          line-height: 16px;\n          color: #ffffff;\n          background-color: #ef6262;\n          -moz-border-radius: 50%;\n          -webkit-border-radius: 50%;\n          border-radius: 50%; }\n      .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search {\n        padding: 0;\n        position: relative;\n        display: inline-block;\n        top: -4px; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input {\n          display: inline-block;\n          border: 0 none;\n          font-size: 14px;\n          background: transparent;\n          border-bottom: 2px solid #ffffff;\n          outline: 0 none;\n          -webkit-box-shadow: none;\n          box-shadow: none;\n          color: #ffffff;\n          width: 100px;\n          padding: 1px 20px 1px 1px;\n          margin: 0px;\n          -moz-border-radius: 2px;\n          -webkit-border-radius: 2px;\n          border-radius: 2px; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input::-webkit-input-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input:-moz-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input::-moz-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search input:-ms-input-placeholder {\n            color: #ffffff;\n            opacity: .7;\n            -moz-transition: opacity 0.2s;\n            -o-transition: opacity 0.2s;\n            -webkit-transition: opacity 0.2s;\n            transition: opacity 0.2s; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search .layout-topbar-search-icon {\n          font-size: 18px;\n          position: absolute;\n          top: -1px;\n          right: 0px; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input {\n          border-bottom-color: #77c7ff; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input::-webkit-input-placeholder {\n            opacity: 1; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input:-moz-placeholder {\n            opacity: 1; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input::-moz-placeholder {\n            opacity: 1; }\n          .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover input:-ms-input-placeholder {\n            opacity: 1; }\n        .layout-wrapper .layout-topbar .layout-topbar-icons .layout-topbar-search:hover .layout-topbar-search-icon {\n          color: #77c7ff; }\n    .layout-wrapper .layout-topbar .layout-menu-button {\n      cursor: pointer;\n      display: inline-block;\n      text-decoration: none;\n      color: #ffffff;\n      -moz-transition: color 0.2s;\n      -o-transition: color 0.2s;\n      -webkit-transition: color 0.2s;\n      transition: color 0.2s; }\n      .layout-wrapper .layout-topbar .layout-menu-button span {\n        font-size: 2em; }\n      .layout-wrapper .layout-topbar .layout-menu-button:hover {\n        color: #77c7ff; }\n    .layout-wrapper .layout-topbar .layout-home-button {\n      cursor: pointer;\n      display: inline-block;\n      margin-left: 20px;\n      text-decoration: none;\n      color: #ffffff;\n      -moz-transition: color 0.2s;\n      -o-transition: color 0.2s;\n      -webkit-transition: color 0.2s;\n      transition: color 0.2s; }\n      .layout-wrapper .layout-topbar .layout-home-button span {\n        font-size: 2em; }\n      .layout-wrapper .layout-topbar .layout-home-button:hover {\n        color: #77c7ff; }\n    .layout-wrapper .layout-topbar a {\n      cursor: pointer; }\n  .layout-wrapper .p-scrollpanel {\n    background: transparent;\n    border-radius: 0;\n    border: none; }\n    .layout-wrapper .p-scrollpanel .p-scrollpanel-content {\n      overflow: scroll; }\n    .layout-wrapper .p-scrollpanel .p-scrollpanel-bar {\n      background: #aaaaaa;\n      opacity: 0.3;\n      filter: alpha(opacity=30); }\n    .layout-wrapper .p-scrollpanel .p-scrollpanel-hidden {\n      display: block;\n      visibility: hidden; }\n    .layout-wrapper .p-scrollpanel .layout-sidebar-scroll-content {\n      width: calc(100% + 18px);\n      padding-bottom: 120px; }\n  .layout-wrapper .layout-sidebar {\n    position: fixed;\n    width: 250px;\n    height: 100%;\n    z-index: 999;\n    user-select: none;\n    -moz-user-select: none;\n    -webkit-user-select: none;\n    -moz-transition: left 0.2s;\n    -o-transition: left 0.2s;\n    -webkit-transition: left 0.2s;\n    transition: left 0.2s;\n    background: #f3f4f9;\n    /* Old browsers */\n    background: -moz-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* FF3.6+ */\n    background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #f3f4f9), color-stop(100%, #d7dbe8));\n    /* Chrome,Safari4+ */\n    background: -webkit-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* Chrome10+,Safari5.1+ */\n    background: -o-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* Opera 11.10+ */\n    background: -ms-linear-gradient(top, #f3f4f9 0%, #d7dbe8 100%);\n    /* IE10+ */\n    background: linear-gradient(to bottom, #f3f4f9 0%, #d7dbe8 100%);\n    /* W3C */\n    filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=\'#ffffff\', endColorstr=\'#000000\',GradientType=0 );\n    /* IE6-9 */\n    -webkit-box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.16);\n    -moz-box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.16);\n    box-shadow: 0 0 6px 0 rgba(0, 0, 0, 0.16); }\n    .layout-wrapper .layout-sidebar .layout-logo {\n      text-align: center;\n      margin-top: 24px; }\n    .layout-wrapper .layout-sidebar .profile {\n      text-align: center;\n      padding: 20px 0; }\n      .layout-wrapper .layout-sidebar .profile img {\n        width: 56px;\n        margin: 10px; }\n      .layout-wrapper .layout-sidebar .profile .profile-link {\n        cursor: pointer;\n        color: #232428;\n        display: inline-block;\n        margin-bottom: 10px;\n        -moz-transition: color 0.2s;\n        -o-transition: color 0.2s;\n        -webkit-transition: color 0.2s;\n        transition: color 0.2s; }\n        .layout-wrapper .layout-sidebar .profile .profile-link i {\n          display: inline-block;\n          font-size: 16px; }\n        .layout-wrapper .layout-sidebar .profile .profile-link:hover {\n          color: #0388e5; }\n      .layout-wrapper .layout-sidebar .profile > ul {\n        overflow: hidden;\n        background-color: #ffffff;\n        text-align: left;\n        max-height: 0;\n        -moz-transition-duration: 0.2s;\n        -webkit-transition-duration: 0.2s;\n        -o-transition-duration: 0.2s;\n        transition-duration: 0.2s;\n        -webkit-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -moz-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -o-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1); }\n        .layout-wrapper .layout-sidebar .profile > ul.profile-expanded {\n          max-height: 500px; }\n        .layout-wrapper .layout-sidebar .profile > ul li a {\n          border: 0 none; }\n        .layout-wrapper .layout-sidebar .profile > ul li:last-child > a {\n          border: 0 none; }\n    .layout-wrapper .layout-sidebar ul {\n      list-style-type: none;\n      margin: 0;\n      padding: 0; }\n      .layout-wrapper .layout-sidebar ul li a {\n        cursor: pointer;\n        position: relative;\n        /* color: #232428; */\n        text-decoration: none;\n        font-size: 14px;\n        padding: 1em 15px 1em 1em;\n        display: block;\n        border-top: 1px solid rgba(207, 211, 224, 0.6); }\n        .layout-wrapper .layout-sidebar ul li a i {\n          font-size: 18px;\n          vertical-align: middle; }\n        .layout-wrapper .layout-sidebar ul li a span {\n          margin-left: .25em;\n          vertical-align: middle; }\n        .layout-wrapper .layout-sidebar ul li a .menuitem-toggle-icon {\n          float: right; }\n        .layout-wrapper .layout-sidebar ul li a:hover {\n          color: #0388e5; }\n      /* .layout-wrapper .layout-sidebar ul li.active-menuitem > a {\n        background-color: #ffffff;\n        color: #0388e5; } */\n        .layout-wrapper .layout-sidebar ul li.active-menuitem > a .menuitem-toggle-icon:before {\n          content: ""; }\n      .layout-wrapper .layout-sidebar ul li.active-menuitem > ul {\n        max-height: 500px; }\n      .layout-wrapper .layout-sidebar ul li ul {\n        background-color: #ffffff;\n        overflow: hidden;\n        margin-left: 1.5em;\n        max-height: 0;\n        -webkit-transition-property: max-height;\n        -moz-transition-property: max-height;\n        -ms-transition-property: max-height;\n        -o-transition-property: max-height;\n        transition-property: max-height;\n        -moz-transition-duration: 0.4s;\n        -webkit-transition-duration: 0.4s;\n        -o-transition-duration: 0.4s;\n        transition-duration: 0.4s;\n        -webkit-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -moz-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        -o-transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1);\n        transition-timing-function: cubic-bezier(0.86, 0, 0.07, 1); }\n        .layout-wrapper .layout-sidebar ul li ul li a {\n          cursor: pointer;\n          padding: .75em 33px .75em .75em;\n          font-size: 13px;\n          border-top: 0 none; }\n        .layout-wrapper .layout-sidebar ul li ul li:last-child > a {\n          border-bottom: 0 none; }\n      .layout-wrapper .layout-sidebar ul li:last-child > a {\n        border-bottom: 1px solid rgba(207, 211, 224, 0.6); }\n      .layout-wrapper .layout-sidebar ul .menuitem-toggle-icon {\n        float: right;\n        margin-top: 2px; }\n      .layout-wrapper .layout-sidebar ul .menuitem-badge {\n        margin-top: 3px;\n        font-size: 10px;\n        float: right;\n        width: 16px;\n        height: 16px;\n        line-height: 16px;\n        text-align: center;\n        color: #ffffff;\n        background-color: #007be5;\n        -moz-border-radius: 50%;\n        -webkit-border-radius: 50%;\n        border-radius: 50%; }\n    .layout-wrapper .layout-sidebar.layout-sidebar-dark {\n      background: #4d505b;\n      /* Old browsers */\n      background: -moz-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* FF3.6+ */\n      background: -webkit-gradient(linear, left top, left bottom, color-stop(0%, #4d505b), color-stop(100%, #3b3e47));\n      /* Chrome,Safari4+ */\n      background: -webkit-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* Chrome10+,Safari5.1+ */\n      background: -o-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* Opera 11.10+ */\n      background: -ms-linear-gradient(top, #4d505b 0%, #3b3e47 100%);\n      /* IE10+ */\n      background: linear-gradient(to bottom, #4d505b 0%, #3b3e47 100%);\n      /* W3C */\n      filter: progid:DXImageTransform.Microsoft.gradient( startColorstr=\'#ffffff\', endColorstr=\'#000000\',GradientType=0 );\n      /* IE6-9 */ }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > a {\n        color: #ffffff; }\n        .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > a:hover {\n          color: #0388e5; }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > ul {\n        background-color: #2e3035; }\n        .layout-wrapper .layout-sidebar.layout-sidebar-dark .profile > ul li a {\n          border: 0 none; }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li a {\n        /* color: #ffffff; */\n        border-top: 1px solid rgba(52, 56, 65, 0.6); }\n        /* .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li a:hover {\n          color: #0388e5; } */\n      /* .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li.active-menuitem > a {\n        background-color: #2e3035;\n        color: #0388e5; } */\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li ul {\n        background-color: #2e3035; }\n        .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li ul li a {\n          border: none; }\n      .layout-wrapper .layout-sidebar.layout-sidebar-dark ul li:last-child > a {\n        border-bottom: 1px solid rgba(52, 56, 65, 0.6); }\n  .layout-wrapper .layout-main {\n    -moz-transition: margin-left 0.2s;\n    -o-transition: margin-left 0.2s;\n    -webkit-transition: margin-left 0.2s;\n    transition: margin-left 0.2s;\n    padding: 66px 16px 16px 16px;\n    display: flex;\n    flex-direction: column;\n    height: 100vh; }\n  .layout-wrapper .layout-footer {\n    -moz-transition: margin-left 0.2s;\n    -o-transition: margin-left 0.2s;\n    -webkit-transition: margin-left 0.2s;\n    transition: margin-left 0.2s;\n    background-color: #ffffff;\n    padding: 1em 2em; }\n    .layout-wrapper .layout-footer img {\n      vertical-align: middle; }\n    .layout-wrapper .layout-footer .footer-text {\n      vertical-align: middle; }\n\n/*.lino-main {\n    flex: auto;\n    display: flex;\n    flex-direction: column;\n}*/\n.dashboard-item-closed {\n  display: none; }\n\n.p-panel {\n  height: inherit; }\n  .p-panel .p-panel-content {\n    height: inherit; }\n  .p-panel .p-toggleable-content {\n    height: inherit; }\n\nbody .lino-panel.p-tabview .p-tabview-panels {\n  padding: .5ch 0.7ch;\n}\n.lino-panel.p-tabview-panel {\n    display: inline;\n}\n.l-panel {\n  height: 100%;\n  width: 100%;\n  flex: auto;\n  display: flex; }\n  .l-panel .l-component {\n    width: 100%;\n    padding: .25em;}\n    .l-panel .l-component .l-label {\n      font-weight: lighter;\n      border-bottom: dotted 1px;\n      white-space: nowrap; }\n      .l-panel .l-component .l-label.l-label--unfilled {\n        color: grey; }\n    .l-panel .l-component .p-checkbox.p-component {\n      padding-top: .5ch; }\n\n.p-autocomplete-list-item {\n  min-height: 28.7px; }\n\nbody .l-ForeignKeyElement {\n  display: flex;\n  flex-direction: row;\n  align-items: center;\n  margin-right: 1ch;\n  position: relative; }\n  body .l-ForeignKeyElement .p-autocomplete.p-component {\n    width: 100%; }\n  body .l-ForeignKeyElement .l-fk-clear {\n    position: absolute;\n    right: 2.7em;\n    top: 50%;\n    font-size: 1em;\n    height: 1em;\n    margin-top: -.5em;\n    color: #848484; }\n  body .l-ForeignKeyElement .l-fk-clear::before {\n    content: "\\E90B"; }\n  body .l-ForeignKeyElement .l-button-fk {\n    margin-left: 1em;\n    height: 1.5em;\n    width: 1.5em;\n    margin-top: 3px; }\n  body .l-ForeignKeyElement .p-autocomplete {\n    display: inherit; }\n    body .l-ForeignKeyElement .p-autocomplete .p-autocomplete-items > li {\n      min-height: 32px; }\n    body .l-ForeignKeyElement .p-autocomplete .p-autocomplete-dropdown {\n      max-width: 2.257em; }\n  body .l-ForeignKeyElement input {\n    width: calc(100% - 2.357em); }\n  body .l-ForeignKeyElement label {\n    white-space: nowrap; }\n\n.p-calendar input {\n  width: 100%; }\n\n.l-ChoiceListFieldElement .p-dropdown.p-component {\n  padding-right: 1px; }\n\n.l-ChoiceListFieldElement .p-dropdown-clearable > label {\n  margin-right: 16px; }\n\n.l-ChoiceListFieldElement > div {\n  min-width: unset; }\n\n.l-ChoiceListFieldElement label {\n  margin-top: 1px;\n  margin-left: 1px; }\n\n.l-panel-vertical {\n  flex-direction: column; }\n\n.lino-loading-mask {\n  position: absolute;\n  width: 100%;\n  height: 100%;\n  z-index: 9999;\n  opacity: .2;\n  border-radius: 5px; }\n\n.lino-loading-mask > div {\n  position: absolute;\n  top: 50%;\n  right: 50%;\n  transform: translate(50%, -50%); }\n\n.lino-transparent {\n  opacity: 0; }\n\n.l-actas {\n  max-height: calc(-250px + 100vh); }\n  .l-actas .p-card-content {\n    max-height: calc(100vh - 372px);\n    overflow-x: hidden;\n    overflow-y: auto; }\n  .l-actas .p-button {\n    width: 100%;\n    margin-bottom: 2px; }\n\n.p-tabview {\n  flex: auto;\n  display: flex;\n  flex-direction: column; }\n\n.p-tabview-panels {\n  flex: auto;\n  display: flex;\n  flex-direction: column; }\n\n.p-tabview-panel {\n  flex: auto;\n  display: flex; }\n\n.l-editor-wrapper > div {\n  width: 100%;\n  height: 100%; }\n\n.l-editor-wrapper > div > div {\n  width: 100%;\n  height: 100%; }\n\n.p-editor-container {\n  height: 100%;\n  padding-bottom: .5ch;\n  padding-top: .5ch;\n  width: 100%; }\n\n.p-dialog {\n  max-width: 100vw; }\n  .p-dialog .p-dialog-content {\n    max-height: 78vh;\n    width: 100%; }\n    @media (max-width: 600px) {\n      .p-dialog .p-dialog-content {\n        overflow: scroll; } }\n  .p-dialog .p-fileupload-content {\n    min-height: 150px;\n    max-height: 300px;\n    overflow-y: scroll;\n    overflow-x: hidden; }\n\n.p-panel-content {\n  flex: auto; }\n\n.p-panel-content-wrapper-expanded {\n  flex: auto;\n  display: flex; }\n\n.l-slave-summary-panel .p-panel-content .p-button:first-child {\n  float: right;\n  margin-top: -44px; }\n\nbody .p-datatable .p-datatable-tbody > tr.p-highlight a {\n  color: #333333; }\n\nbody table p {\n  margin: unset; }\n\nbody .layout-wrapper .layout-sidebar ul li.active-menuitem > ul {\n  max-height: 200vh; }\n\nbody .l-bbar > * {\n  margin-right: 2px;\n  margin-bottom: 1px; }\n\nbody .l-grid .p-dataview .p-panel-header {\n  padding: 0px 1ch; }\n\nbody .l-grid .p-dataview .p-panel-content {\n  padding-top: 1ch;\n  padding-left: 1ch; }\n\nbody .l-grid .p-dataview p {\n  margin: unset; }\n\n.table-header {\n  display: flex;\n  justify-content: space-between;\n}\n  body .l-grid .table-header .l-DataViewLayoutOptions {\n    display: inline; }\n\nbody .l-grid .p-datatable .p-datatable-thead > tr > th {\n  border-bottom-width: 3px; }\n\nbody .l-grid .p-datatable .p-datatable-tbody > tr > td.p-cell-editing {\n  overflow: unset; }\n  body .l-grid .p-datatable .p-datatable-tbody > tr > td.p-cell-editing .p-datepicker {\n    min-width: max-content;\n    position: fixed;\n    left: unset !important;\n    top: unset !important;\n    width: auto; }\n    body .l-grid .p-datatable .p-datatable-tbody > tr > td.p-cell-editing .p-datepicker table.p-datepicker-calendar {\n      display: block; }\n\nbody .l-grid .p-datatable .p-datatable-header {\n  padding: 0.15em 0.25em; }\n\nbody .l-grid .p-datatable .p-paginator {\n  position: relative; }\n  body .l-grid .p-datatable .p-paginator .p-paginator-right-content {\n    position: absolute;\n    top: 50%;\n    right: 2ch;\n    transform: translateY(-50%); }\n\nbody .l-grid .p-datatable .l-DateFieldElement input {\n  margin-right: -2.357em; }\n\nbody .l-grid .p-datatable .l-DateFieldElement .p-datepicker-trigger {\n  width: 2.357em !important; }\n\n.no-ws {\n  color: grey !important; }\n\n.l-itemTemplate {\n  width: 100%; }\n\n.chatwindow-chats > .p-scrollpanel-content {\n  display: flex;\n  flex-direction: column;\n  margin-top: .6ch; }\n  .chatwindow-chats > .p-scrollpanel-content > div {\n    margin-top: .7ch; }\n\n.chatwindow {\n  max-width: 284px; }\n  .chatwindow .user {\n    font-size: x-small;\n    text-transform: capitalize; }\n  .chatwindow .not-sent .message {\n    background: gray !important; }\n  .chatwindow .message {\n    transition: background-color 1000ms linear;\n    border-radius: 10px;\n    background: #06b4f1;\n    padding-left: 1ch;\n    padding-right: 1ch;\n    overflow-wrap: break-word;\n    max-width: 100%; }\n  .chatwindow .p-scrollpanel-wrapper {\n    border-right: 9px solid #f4f4f4; }\n  .chatwindow .p-scrollpanel-bar {\n    background-color: #1976d2;\n    opacity: 1;\n    transition: background-color .3s; }\n  .chatwindow .p-scrollpanel-bar:hover {\n    background-color: #135ba1; }\n  .chatwindow .p-editor-toolbar {\n    border-top: unset !important;\n    padding: unset !important; }\n  .chatwindow .p-editor-container {\n    padding-bottom: unset; }\n\nbody .l-detail-toolbar .p-toolbar-group-left {\n  display: block; }\n\nbody .l-detail-toolbar .p-button {\n  margin-right: 2px;\n  margin-bottom: 1px; }\n\n@media (max-width: 600px) {\n  .l-panel {\n    flex-direction: column; }\n    .l-panel .l-component {\n      padding-left: unset;\n      padding-right: unset; } }\n\n/* Responsive  larger than 1025px*/\n@media (min-width: 1025px) {\n  .layout-wrapper.layout-overlay .layout-sidebar {\n    left: -250px; }\n  .layout-wrapper.layout-overlay .layout-topbar {\n    left: 0; }\n  .layout-wrapper.layout-overlay .layout-main, .layout-wrapper.layout-overlay .layout-footer {\n    margin-left: 0; }\n  .layout-wrapper.layout-overlay.layout-overlay-sidebar-active .layout-sidebar {\n    left: 0; }\n  .layout-wrapper.layout-overlay.layout-overlay-sidebar-active .layout-topbar {\n    left: 250px; }\n  .layout-wrapper.layout-static .layout-sidebar {\n    left: 0; }\n  .layout-wrapper.layout-static .layout-topbar {\n    left: 250px; }\n  .layout-wrapper.layout-static .layout-main, .layout-wrapper.layout-static .layout-footer {\n    margin-left: 250px; }\n  .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-sidebar {\n    left: -250px; }\n  .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-topbar {\n    left: 0; }\n  .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-main, .layout-wrapper.layout-static.layout-static-sidebar-inactive .layout-footer {\n    margin-left: 0; } }\n\n@media (max-width: 1024px) {\n  .layout-wrapper .layout-topbar {\n    left: 0; }\n    .layout-wrapper .layout-topbar .layout-topbar-icons a span.layout-topbar-item-text {\n      display: none; }\n  .layout-wrapper .layout-main, .layout-wrapper .layout-footer {\n    margin-left: 0; }\n  .layout-wrapper .layout-sidebar {\n    left: -250px;\n    margin-top: 50px; }\n  .layout-wrapper .layout-mask {\n    display: none;\n    position: fixed;\n    width: 100%;\n    height: 100%;\n    top: 50px;\n    left: 0;\n    z-index: 998;\n    background-color: #424242;\n    opacity: 0.7;\n    filter: alpha(opacity=70); }\n  .layout-wrapper.layout-mobile-sidebar-active .layout-sidebar {\n    left: -0; }\n  .layout-wrapper.layout-mobile-sidebar-active .layout-mask {\n    display: block; }\n  .body-overflow-hidden {\n    overflow: hidden; } }\n\n/* Typography */\nh1 {\n  font-weight: normal;\n  margin: 0;\n  font-size: 24px; }\n\nh2 {\n  font-size: 20px;\n  font-weight: normal;\n  margin: 0; }\n\n.card {\n  background-color: #ffffff;\n  padding: 1em;\n  margin-bottom: 16px;\n  -moz-border-radius: 3px;\n  -webkit-border-radius: 3px;\n  border-radius: 3px; }\n  .card.card-w-title {\n    padding-bottom: 2em; }\n  .card h1 {\n    margin: .5em 0 .5em 0;\n    border-bottom: 1px solid #d5d5d5;\n    padding: .1em;\n    font-size: 24px; }\n    .card h1:first-child {\n      margin: 0 0 .5em 0; }\n\n.p-g {\n  -ms-flex-wrap: wrap; }\n\n/* Dashboard */\n.dashboard .summary {\n  position: relative; }\n  .dashboard .summary .title {\n    font-size: 20px; }\n  .dashboard .summary .detail {\n    color: #707070;\n    display: block;\n    margin-top: 10px; }\n  .dashboard .summary .count {\n    color: #ffffff;\n    position: absolute;\n    top: 10px;\n    right: 10px;\n    font-size: 24px;\n    padding: 7px 14px;\n    -moz-border-radius: 3px;\n    -webkit-border-radius: 3px;\n    border-radius: 3px; }\n    .dashboard .summary .count.visitors {\n      background-color: #20d077; }\n    .dashboard .summary .count.purchases {\n      background-color: #f9c851; }\n    .dashboard .summary .count.revenue {\n      background-color: #007be5; }\n\n.dashboard .highlight-box {\n  height: 100px; }\n  .dashboard .highlight-box:after {\n    content: "";\n    display: table;\n    clear: both; }\n  .dashboard .highlight-box .initials {\n    height: 100%;\n    float: left;\n    width: 50%;\n    text-align: center;\n    padding: 1em; }\n    .dashboard .highlight-box .initials > span {\n      font-size: 48px; }\n  .dashboard .highlight-box .highlight-details {\n    height: 100%;\n    background-color: #ffffff;\n    float: left;\n    width: 50%;\n    padding: 1em; }\n    .dashboard .highlight-box .highlight-details i {\n      font-size: 24px;\n      vertical-align: middle;\n      margin-right: .25em; }\n    .dashboard .highlight-box .highlight-details .count {\n      color: #707070;\n      font-size: 36px;\n      display: block; }\n\n.dashboard .task-list {\n  list-style-type: none;\n  margin: 0;\n  padding: 0; }\n  .dashboard .task-list li {\n    padding: .5em .25em;\n    border-bottom: 1px solid #e3e3e3; }\n    .dashboard .task-list li:after {\n      content: "";\n      display: table;\n      clear: both; }\n  .dashboard .task-list .p-checkbox {\n    vertical-align: middle;\n    margin-right: .5em; }\n  .dashboard .task-list .task-name {\n    vertical-align: middle; }\n  .dashboard .task-list .p-button {\n    float: right; }\n    .dashboard .task-list .p-button .p-button-text {\n      padding: .125em; }\n  .dashboard .task-list .p-panel-content {\n    min-height: 256px; }\n\n.dashboard .contact-form .p-panel-content {\n  min-height: 256px; }\n\n.dashboard .contacts ul {\n  list-style-type: none;\n  padding: 0;\n  margin: 0; }\n  .dashboard .contacts ul li {\n    border-bottom: 1px solid #e3e3e3; }\n    .dashboard .contacts ul li a {\n      padding: 9px;\n      width: 100%;\n      box-sizing: border-box;\n      text-decoration: none;\n      position: relative;\n      display: block;\n      -moz-border-radius: 2px;\n      -webkit-border-radius: 2px;\n      border-radius: 2px;\n      -moz-transition: background-color 0.2s;\n      -o-transition: background-color 0.2s;\n      -webkit-transition: background-color 0.2s;\n      transition: background-color 0.2s; }\n      .dashboard .contacts ul li a .name {\n        position: absolute;\n        right: 10px;\n        top: 10px;\n        font-size: 18px; }\n      .dashboard .contacts ul li a .email {\n        position: absolute;\n        right: 10px;\n        top: 30px;\n        font-size: 14px;\n        color: #707070; }\n      .dashboard .contacts ul li a:hover {\n        cursor: pointer;\n        background-color: #eeeeee; }\n    .dashboard .contacts ul li:last-child {\n      border: 0; }\n\n.dashboard .contacts .p-panel-content {\n  min-height: 256px; }\n\n.dashboard .activity-list {\n  list-style-type: none;\n  padding: 0;\n  margin: 0; }\n  .dashboard .activity-list li {\n    border-bottom: 1px solid #e3e3e3;\n    padding: 16px 8px; }\n    .dashboard .activity-list li .count {\n      font-size: 24px;\n      color: #ffffff;\n      background-color: #007be5;\n      font-weight: 700;\n      display: inline-block;\n      padding: .25em .5em;\n      -moz-border-radius: 3px;\n      -webkit-border-radius: 3px;\n      border-radius: 3px; }\n    .dashboard .activity-list li:first-child {\n      border-top: 1px solid #e3e3e3; }\n    .dashboard .activity-list li:last-child {\n      border: 0; }\n    .dashboard .activity-list li .p-g-6:first-child {\n      font-size: 18px;\n      padding-left: 0; }\n    .dashboard .activity-list li .p-g-6:last-child {\n      text-align: right;\n      color: #707070; }\n\n/*!\n * Quill Editor v1.0.0-beta.3\n * https://quilljs.com/\n * Copyright (c) 2014, Jason Chen\n * Copyright (c) 2013, salesforce.com\n */\n.ql-container {\n  box-sizing: border-box;\n  font-family: Helvetica, Arial, sans-serif;\n  font-size: 13px;\n  height: 100%;\n  margin: 0px;\n  position: relative; }\n\n.ql-clipboard {\n  left: -100000px;\n  position: absolute;\n  top: 50%; }\n\n.ql-clipboard p {\n  margin: 0;\n  padding: 0; }\n\n.ql-editor {\n  box-sizing: border-box;\n  cursor: text;\n  line-height: 1.42;\n  height: 100%;\n  outline: none;\n  overflow-y: auto;\n  padding: 12px 15px;\n  tab-size: 4;\n  text-align: left;\n  white-space: pre-wrap; }\n\n.ql-editor p,\n.ql-editor ol,\n.ql-editor ul,\n.ql-editor pre,\n.ql-editor blockquote,\n.ql-editor h1,\n.ql-editor h2,\n.ql-editor h3,\n.ql-editor h4,\n.ql-editor h5,\n.ql-editor h6 {\n  margin: 0;\n  padding: 0;\n  counter-reset: list-1 list-2 list-3 list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol {\n  padding-left: 20px; }\n\n.ql-editor ul {\n  padding-left: 8px;\n  list-style: disc inside; }\n\n.ql-editor ol > li {\n  list-style-type: none; }\n\n.ql-editor ol {\n  list-style-type: none;\n  position: relative; }\n\n.ql-editor ol li {\n  counter-reset: list-1 list-2 list-3 list-4 list-5 list-6 list-7 list-8;\n  counter-increment: list-num; }\n\n.ql-editor ol li:before {\n  content: counter(list-num, decimal) ". ";\n  margin-right: -16px;\n  position: absolute;\n  right: 100%;\n  text-align: right; }\n\n.ql-editor ol li.ql-indent-1 {\n  counter-increment: list-1; }\n\n.ql-editor ol li.ql-indent-1:before {\n  content: counter(list-1, lower-alpha) ". ";\n  margin-right: -56px; }\n\n.ql-editor ol li.ql-indent-1 {\n  counter-reset: list-2 list-3 list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-2 {\n  counter-increment: list-2; }\n\n.ql-editor ol li.ql-indent-2:before {\n  content: counter(list-2, lower-roman) ". ";\n  margin-right: -96px; }\n\n.ql-editor ol li.ql-indent-2 {\n  counter-reset: list-3 list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-3 {\n  counter-increment: list-3; }\n\n.ql-editor ol li.ql-indent-3:before {\n  content: counter(list-3, decimal) ". ";\n  margin-right: -136px; }\n\n.ql-editor ol li.ql-indent-3 {\n  counter-reset: list-4 list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-4 {\n  counter-increment: list-4; }\n\n.ql-editor ol li.ql-indent-4:before {\n  content: counter(list-4, lower-alpha) ". ";\n  margin-right: -176px; }\n\n.ql-editor ol li.ql-indent-4 {\n  counter-reset: list-5 list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-5 {\n  counter-increment: list-5; }\n\n.ql-editor ol li.ql-indent-5:before {\n  content: counter(list-5, lower-roman) ". ";\n  margin-right: -216px; }\n\n.ql-editor ol li.ql-indent-5 {\n  counter-reset: list-6 list-7 list-8; }\n\n.ql-editor ol li.ql-indent-6 {\n  counter-increment: list-6; }\n\n.ql-editor ol li.ql-indent-6:before {\n  content: counter(list-6, decimal) ". ";\n  margin-right: -256px; }\n\n.ql-editor ol li.ql-indent-6 {\n  counter-reset: list-7 list-8; }\n\n.ql-editor ol li.ql-indent-7 {\n  counter-increment: list-7; }\n\n.ql-editor ol li.ql-indent-7:before {\n  content: counter(list-7, lower-alpha) ". ";\n  margin-right: -296px; }\n\n.ql-editor ol li.ql-indent-7 {\n  counter-reset: list-8; }\n\n.ql-editor ol li.ql-indent-8 {\n  counter-increment: list-8; }\n\n.ql-editor ol li.ql-indent-8:before {\n  content: counter(list-8, lower-roman) ". ";\n  margin-right: -336px; }\n\n.ql-editor .ql-indent-1 {\n  padding-left: 40px; }\n\n.ql-editor .ql-indent-2 {\n  padding-left: 80px; }\n\n.ql-editor .ql-indent-3 {\n  padding-left: 120px; }\n\n.ql-editor .ql-indent-4 {\n  padding-left: 160px; }\n\n.ql-editor .ql-indent-5 {\n  padding-left: 200px; }\n\n.ql-editor .ql-indent-6 {\n  padding-left: 240px; }\n\n.ql-editor .ql-indent-7 {\n  padding-left: 280px; }\n\n.ql-editor .ql-indent-8 {\n  padding-left: 320px; }\n\n.ql-editor .ql-video {\n  display: block; }\n\n.ql-editor .ql-video.ql-align-center {\n  margin: 0 auto; }\n\n.ql-editor .ql-video.ql-align-right {\n  margin: 0 0 0 auto; }\n\n.ql-editor .ql-bg-black {\n  background-color: #000; }\n\n.ql-editor .ql-bg-red {\n  background-color: #e60000; }\n\n.ql-editor .ql-bg-orange {\n  background-color: #f90; }\n\n.ql-editor .ql-bg-yellow {\n  background-color: #ff0; }\n\n.ql-editor .ql-bg-green {\n  background-color: #008a00; }\n\n.ql-editor .ql-bg-blue {\n  background-color: #06c; }\n\n.ql-editor .ql-bg-purple {\n  background-color: #93f; }\n\n.ql-editor .ql-color-white {\n  color: #fff; }\n\n.ql-editor .ql-color-red {\n  color: #e60000; }\n\n.ql-editor .ql-color-orange {\n  color: #f90; }\n\n.ql-editor .ql-color-yellow {\n  color: #ff0; }\n\n.ql-editor .ql-color-green {\n  color: #008a00; }\n\n.ql-editor .ql-color-blue {\n  color: #06c; }\n\n.ql-editor .ql-color-purple {\n  color: #93f; }\n\n.ql-editor .ql-font-serif {\n  font-family: Georgia, Times New Roman, serif; }\n\n.ql-editor .ql-font-monospace {\n  font-family: Monaco, Courier New, monospace; }\n\n.ql-editor .ql-size-small {\n  font-size: 10px; }\n\n.ql-editor .ql-size-large {\n  font-size: 18px; }\n\n.ql-editor .ql-size-huge {\n  font-size: 32px; }\n\n.ql-editor .ql-direction-rtl {\n  direction: rtl;\n  text-align: inherit; }\n\n.ql-editor .ql-align-center {\n  text-align: center; }\n\n.ql-editor .ql-align-justify {\n  text-align: justify; }\n\n.ql-editor .ql-align-right {\n  text-align: right; }\n\n.ql-editor.ql-blank::before {\n  color: rgba(0, 0, 0, 0.6);\n  content: attr(data-placeholder);\n  font-style: italic;\n  pointer-events: none;\n  position: absolute; }\n\n.ql-hidden {\n  display: none; }\n\n.ql-tooltip {\n  position: absolute; }\n\n.ql-tooltip a {\n  cursor: pointer;\n  text-decoration: none; }\n\n.ql-toolbar:before,\n.ql-toolbar:after {\n  content: \' \';\n  display: table; }\n\n.ql-toolbar:after {\n  clear: both; }\n\n.ql-toolbar button {\n  background: none;\n  border: none;\n  cursor: pointer;\n  display: inline-block;\n  float: left;\n  height: 24px;\n  outline: none;\n  padding: 3px 5px;\n  width: 24px; }\n\n.ql-toolbar button svg {\n  height: 100%; }\n\n.ql-toolbar .ql-stroke {\n  fill: none;\n  stroke-linecap: round;\n  stroke-linejoin: round;\n  stroke-width: 2; }\n\n.ql-toolbar .ql-stroke-mitter {\n  fill: none;\n  stroke-mitterlimit: 10;\n  stroke-width: 2; }\n\n.ql-toolbar .ql-empty {\n  fill: none; }\n\n.ql-toolbar .ql-even {\n  fill-rule: evenodd; }\n\n.ql-toolbar .ql-thin,\n.ql-toolbar .ql-stroke.ql-thin {\n  stroke-width: 1; }\n\n.ql-toolbar .ql-transparent {\n  opacity: 0.4; }\n\n.ql-editor h1 {\n  font-size: 2em; }\n\n.ql-editor h2 {\n  font-size: 1.5em; }\n\n.ql-editor h3 {\n  font-size: 1.17em; }\n\n.ql-editor h4 {\n  font-size: 1em; }\n\n.ql-editor h5 {\n  font-size: 0.83em; }\n\n.ql-editor h6 {\n  font-size: 0.67em; }\n\n.ql-editor pre {\n  white-space: pre-wrap; }\n\n.ql-editor a {\n  text-decoration: underline; }\n\n.ql-editor blockquote {\n  border-left: 4px solid #ccc;\n  margin-bottom: 5px;\n  margin-top: 5px;\n  padding-left: 16px; }\n\n.ql-editor pre.hljs {\n  overflow: visible; }\n\n.ql-editor code,\n.ql-editor pre:not(.hljs) {\n  background-color: #f0f0f0; }\n\n.ql-editor code,\n.ql-editor pre {\n  border-radius: 3px; }\n\n.ql-editor code {\n  font-size: 85%;\n  padding-bottom: 2px;\n  padding-top: 2px; }\n\n.ql-editor code:before,\n.ql-editor code:after {\n  content: "\\A0";\n  letter-spacing: -2px; }\n\n.ql-editor *:not(pre) + pre,\n.ql-editor pre:first-of-type {\n  margin-top: 5px;\n  padding-top: 5px; }\n\n.ql-editor pre {\n  margin-bottom: 5px;\n  padding: 0px 10px 5px; }\n\n.ql-editor pre + pre {\n  margin-top: -10px; }\n\n.ql-editor img {\n  max-width: 100%; }\n\n.ql-snow .ql-image-tooltip {\n  padding: 10px;\n  text-align: center;\n  width: 300px; }\n\n.ql-snow .ql-image-tooltip input[type=text] {\n  height: 30px;\n  width: 100%; }\n\n.ql-snow .ql-image-tooltip a.ql-cancel,\n.ql-snow .ql-image-tooltip a.ql-action {\n  border: 1px solid #06c;\n  display: inline-block;\n  float: left;\n  line-height: 18px;\n  padding: 5px;\n  width: 50%; }\n\n.ql-snow .ql-image-tooltip a.ql-cancel::before {\n  color: #06c;\n  content: \'Cancel\'; }\n\n.ql-snow .ql-image-tooltip a.ql-action {\n  background-color: #06c; }\n\n.ql-snow .ql-image-tooltip a.ql-action::before {\n  color: #fff;\n  content: \'Insert\'; }\n\n.ql-snow .ql-image-tooltip .ql-preview {\n  height: 200px;\n  margin: 10px 0px;\n  position: relative; }\n\n.ql-snow .ql-image-tooltip .ql-preview img {\n  bottom: 0;\n  left: 0;\n  margin: auto;\n  max-height: 100%;\n  max-width: 100%;\n  position: absolute;\n  right: 0;\n  top: 0; }\n\n.ql-snow .ql-image-tooltip .ql-empty.ql-preview::before {\n  border: 1px dashed #ccc;\n  color: #ccc;\n  content: \'Preview\';\n  display: block;\n  line-height: 200px; }\n\n.ql-snow .ql-link-tooltip::before {\n  content: "Visit URL:";\n  line-height: 26px;\n  margin-right: 8px; }\n\n.ql-snow .ql-link-tooltip {\n  margin-top: 10px;\n  padding: 5px 12px;\n  white-space: nowrap; }\n\n.ql-snow .ql-link-tooltip input[type=text] {\n  display: none;\n  height: 26px;\n  width: 170px; }\n\n.ql-snow .ql-link-tooltip a.ql-preview {\n  display: inline-block;\n  max-width: 200px;\n  overflow-x: hidden;\n  text-overflow: ellipsis;\n  vertical-align: top; }\n\n.ql-snow .ql-link-tooltip a.ql-action::before {\n  color: #444;\n  content: \'-\';\n  line-height: 26px;\n  margin-left: 8px; }\n\n.ql-snow .ql-link-tooltip a.ql-action::after {\n  border-right: 1px solid #ccc;\n  content: \'Edit\';\n  margin-left: 8px;\n  padding-right: 8px; }\n\n.ql-snow .ql-link-tooltip a.ql-remove::before {\n  content: \'Remove\';\n  margin-left: 8px; }\n\n.ql-snow .ql-link-tooltip a {\n  line-height: 26px; }\n\n.ql-snow .ql-link-tooltip.ql-editing a.ql-preview,\n.ql-snow .ql-link-tooltip.ql-editing a.ql-remove {\n  display: none; }\n\n.ql-snow .ql-link-tooltip.ql-editing input[type=text] {\n  display: inline-block; }\n\n.ql-snow .ql-link-tooltip.ql-editing a.ql-action::after {\n  border-right: 0px;\n  content: \'Save\';\n  padding-right: 0px; }\n\n.ql-toolbar.ql-snow {\n  border: 1px solid #ccc;\n  box-sizing: border-box;\n  font-family: \'Helvetica Neue\', \'Helvetica\', \'Arial\', sans-serif;\n  padding: 8px; }\n\n.ql-toolbar.ql-snow * {\n  box-sizing: border-box; }\n\n.ql-toolbar.ql-snow .ql-formats {\n  display: inline-block;\n  margin-right: 15px;\n  vertical-align: middle; }\n\n.ql-toolbar.ql-snow button:hover,\n.ql-toolbar.ql-snow button.ql-active,\n.ql-toolbar.ql-snow .ql-picker-label:hover,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active,\n.ql-toolbar.ql-snow .ql-picker-item:hover,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected {\n  color: #06c; }\n\n.ql-toolbar.ql-snow button:hover .ql-fill,\n.ql-toolbar.ql-snow button.ql-active .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-fill,\n.ql-toolbar.ql-snow button:hover .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow button.ql-active .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-stroke.ql-fill,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-stroke.ql-fill {\n  fill: #06c; }\n\n.ql-toolbar.ql-snow button:hover .ql-stroke,\n.ql-toolbar.ql-snow button.ql-active .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-stroke,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-stroke,\n.ql-toolbar.ql-snow button:hover .ql-stroke-mitter,\n.ql-toolbar.ql-snow button.ql-active .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-label:hover .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-label.ql-active .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-item:hover .ql-stroke-mitter,\n.ql-toolbar.ql-snow .ql-picker-item.ql-selected .ql-stroke-mitter {\n  stroke: #06c; }\n\n.ql-toolbar.ql-snow .ql-stroke {\n  stroke: #444; }\n\n.ql-toolbar.ql-snow .ql-stroke-mitter {\n  stroke: #444; }\n\n.ql-toolbar.ql-snow .ql-fill,\n.ql-toolbar.ql-snow .ql-stroke.ql-fill {\n  fill: #444; }\n\n.ql-toolbar.ql-snow .ql-direction svg:last-child {\n  display: none; }\n\n.ql-toolbar.ql-snow .ql-direction.ql-active svg:last-child {\n  display: inline; }\n\n.ql-toolbar.ql-snow .ql-direction.ql-active svg:first-child {\n  display: none; }\n\n.ql-toolbar.ql-snow .ql-picker {\n  color: #444;\n  display: inline-block;\n  float: left;\n  font-size: 14px;\n  font-weight: 500;\n  height: 24px;\n  position: relative;\n  vertical-align: middle; }\n\n.ql-toolbar.ql-snow .ql-picker-label {\n  border: 1px solid transparent;\n  cursor: pointer;\n  display: inline-block;\n  height: 100%;\n  padding-left: 8px;\n  padding-right: 2px;\n  position: relative;\n  width: 100%; }\n\n.ql-toolbar.ql-snow .ql-picker-label svg {\n  float: right;\n  height: 18px;\n  margin-top: 2px;\n  width: 18px; }\n\n.ql-toolbar.ql-snow .ql-picker-label::before {\n  vertical-align: middle; }\n\n.ql-toolbar.ql-snow .ql-picker-options {\n  background-color: #fff;\n  border: 1px solid transparent;\n  display: none;\n  min-width: 100%;\n  padding: 4px 8px;\n  position: absolute;\n  white-space: nowrap; }\n\n.ql-toolbar.ql-snow .ql-picker-options .ql-picker-item {\n  cursor: pointer;\n  display: block;\n  padding-bottom: 5px;\n  padding-top: 5px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-label {\n  border-color: #ccc;\n  color: #ccc;\n  z-index: 2; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-label .ql-fill {\n  fill: #ccc; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-label .ql-stroke {\n  stroke: #ccc; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-expanded .ql-picker-options {\n  border-color: #ccc;\n  box-shadow: rgba(0, 0, 0, 0.2) 0 2px 8px;\n  display: block;\n  margin-top: -1px;\n  z-index: 1; }\n\n.ql-toolbar.ql-snow .ql-color-picker,\n.ql-toolbar.ql-snow .ql-icon-picker {\n  width: 28px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-label,\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-label {\n  padding: 2px 4px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-label svg,\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-label svg {\n  margin-top: 0px; }\n\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-options {\n  padding: 4px 0px; }\n\n.ql-toolbar.ql-snow .ql-icon-picker .ql-picker-item {\n  height: 24px;\n  padding: 2px 4px; }\n\n.ql-toolbar.ql-snow .ql-color-picker.ql-expanded .ql-picker-options,\n.ql-toolbar.ql-snow .ql-icon-picker.ql-expanded .ql-picker-options {\n  margin-top: -6px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-options {\n  padding: 5px;\n  width: 152px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item {\n  border: 1px solid transparent;\n  float: left;\n  height: 16px;\n  margin: 2px;\n  padding: 0px;\n  width: 16px; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item.ql-primary-color {\n  margin-bottom: toolbarPadding; }\n\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item.ql-selected,\n.ql-toolbar.ql-snow .ql-color-picker .ql-picker-item:hover {\n  border-color: #000; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-label]:not([data-label=\'\'])::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-label]:not([data-label=\'\'])::before {\n  content: attr(data-label); }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header {\n  width: 98px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item::before {\n  content: \'Normal\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="1"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="1"]::before {\n  content: \'Heading 1\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="2"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="2"]::before {\n  content: \'Heading 2\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="3"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="3"]::before {\n  content: \'Heading 3\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="4"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="4"]::before {\n  content: \'Heading 4\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="5"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="5"]::before {\n  content: \'Heading 5\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-label[data-value="6"]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="6"]::before {\n  content: \'Heading 6\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="1"]::before {\n  font-size: 2em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="2"]::before {\n  font-size: 1.5em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="3"]::before {\n  font-size: 1.17em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="4"]::before {\n  font-size: 1em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="5"]::before {\n  font-size: 0.83em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-header .ql-picker-item[data-value="6"]::before {\n  font-size: 0.67em; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font {\n  width: 108px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item::before {\n  content: \'Sans Serif\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label[data-value=serif]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=serif]::before {\n  content: \'Serif\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-label[data-value=monospace]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=monospace]::before {\n  content: \'Monospace\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=serif]::before {\n  font-family: Georgia, Times New Roman, serif; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-font .ql-picker-item[data-value=monospace]::before {\n  font-family: Monaco, Courier New, monospace; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size {\n  width: 98px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item::before {\n  content: \'Normal\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-value=small]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=small]::before {\n  content: \'Small\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-value=large]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=large]::before {\n  content: \'Large\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-label[data-value=huge]::before,\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=huge]::before {\n  content: \'Huge\'; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=small]::before {\n  font-size: 10px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=large]::before {\n  font-size: 18px; }\n\n.ql-toolbar.ql-snow .ql-picker.ql-size .ql-picker-item[data-value=huge]::before {\n  font-size: 32px; }\n\n.ql-toolbar.ql-snow .ql-color-picker.ql-background .ql-picker-item {\n  background-color: #fff; }\n\n.ql-toolbar.ql-snow .ql-color-picker.ql-color .ql-picker-item {\n  background-color: #000; }\n\n.ql-toolbar.ql-snow + .ql-container.ql-snow {\n  border-top: 0px; }\n\n.ql-snow .ql-tooltip {\n  background-color: #fff;\n  border: 1px solid #ccc;\n  box-shadow: 0px 0px 5px #ddd;\n  color: #444; }\n\n.ql-snow .ql-tooltip input[type=text] {\n  border: 1px solid #ccc;\n  font-size: 13px;\n  margin: 0px;\n  padding: 3px 5px; }\n\n.ql-container.ql-snow {\n  border: 1px solid #ccc; }\n\n.ql-container.ql-snow a {\n  color: #06c; }\n\n.ql-container.ql-snow * {\n  box-sizing: border-box; }\n\n/* Lino calander CSS */\n.lino-nav-cal {\n    margin-left: 2ch;\n}\n\n.lino-nav-cal h2 {\n  margin-bottom: 2px;\n  white-space: nowrap; }\n\n.lino-nav-cal p {\n  margin: 0;\n  padding: 0; }\n\n.lino-nav-cal h2 > span {\n  width: 14ch;\n  display: inline-block; }\n\n.cal-week {\n  position: relative;\n  right: 2ch; }\n\n.cal-month-table {\n  /* \tdisplay: None; */\n  visibility: hidden;\n  opacity: 0;\n  transition: visibility 0s, opacity 0.5s linear;\n  position: absolute;\n  border: solid;\n  box-sizing: border-box;\n  background-color: #edf0f5;\n  z-index: 1;\n  padding: 12px;\n  border-color: blue;\n  display: inline-block;\n  transform: translate(-50%); }\n\n.cal-month-table a {\n  font-weight: normal; }\n\n.cal-month-cell div.header {\n  padding-bottom: 3px; }\n\n/*.cal-month-cell.other-month h3 a{*/\n/*color: #5c5c5c;*/\n/*}*/\n.cal-month-cell.cal-in-past a {\n  color: darkgray; }\n\n.cal-month-cell.cal-in-past div.header a {\n  color: unset; }\n\n.cal-MonthlyView table[name="cal.MonthlyPlanner.grid"] {\n  height: 100%; }\n\n.cal-MonthlyView table[name="cal.MonthlyPlanner.grid"] tr:nth-child(1) th {\n  height: 1ch; }\n\n.cal-WeeklyView table[name="cal.WeeklyPlanner.grid"] td > a {\n  margin-bottom: 3px;\n  display: block; }\n\n.cal-WeeklyView table[name="cal.WeeklyPlanner.grid"] tr td:nth-child(1) {\n  white-space: nowrap; }\n\n/*For extjs grid of cal view, never going to be used? */\n.cal-MonthlyView td.x-grid3-cell:not(.x-grid3-cell-first) {\n  color: #5c5c5c;\n  min-height: 14ch;\n  border: lightgray solid 1px;\n  padding: 3px;\n  box-sizing: border-box; }\n\n.cal-MonthlyView td.x-grid3-cell-first {\n  vertical-align: middle; }\n\n.lino-nav-cal span > span:hover .cal-month-table {\n  visibility: visible;\n  opacity: 1; }\n\n.other-month {\n  background-color: gainsboro; }\n\n.current-day {\n  background-color: #fbfbfb; }\n\n/* Have "..." overflow*/\n.fixed-table {\n  width: 100%;\n  height: 100%;\n  /*not really necessary, removes extra white space */\n  border-collapse: collapse;\n  border-spacing: 0;\n  border: 0; }\n\n.fixed-table tbody {\n  vertical-align: unset; }\n\n.fixed-table td div {\n  white-space: nowrap;\n  overflow: hidden;\n  text-overflow: ellipsis; }\n\n.dot {\n  height: 7px;\n  width: 7px;\n  border-radius: 50%;\n  display: inline-block;\n  vertical-align: middle;\n  margin-right: 0.3ch;\n  margin-left: 0.3ch;\n  margin-bottom: 0.5ch; }\n', ""]);
                 const i = r
             },
             5219: (e, t, n) => {
                 "use strict";
                 n.d(t, {
                     Z: () => i
                 });
```

### Comparing `lino_react-23.7.5/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.8.0/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/react/views.py` & `lino_react-23.8.0/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.7.5/lino_react/setup_info.py` & `lino_react-23.8.0/lino_react/setup_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.7.5',
+    version='23.8.0',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.7.5/lino_react.egg-info/PKG-INFO` & `lino_react-23.8.0/lino_react.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lino-react
-Version: 23.7.5
+Version: 23.8.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 Classifier:   Programming Language :: Python
 Classifier:   Programming Language :: Python :: 3
 Classifier:   Development Status :: 5 - Production/Stable
```

### Comparing `lino_react-23.7.5/lino_react.egg-info/SOURCES.txt` & `lino_react-23.8.0/lino_react.egg-info/SOURCES.txt`

 * *Files identical despite different names*

