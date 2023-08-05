# Comparing `tmp/NiantongEEG-0.1.3.8.tar.gz` & `tmp/NiantongEEG-0.1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NiantongEEG-0.1.3.8.tar", last modified: Fri Aug  4 13:16:21 2023, max compression
+gzip compressed data, was "NiantongEEG-0.1.3.9.tar", last modified: Fri Aug  4 13:15:28 2023, max compression
```

## Comparing `NiantongEEG-0.1.3.8.tar` & `NiantongEEG-0.1.3.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 13:16:21.952993 NiantongEEG-0.1.3.8/
-drwxrwxrwx   0        0        0        0 2023-08-04 13:16:21.952993 NiantongEEG-0.1.3.8/NiantongEEG.egg-info/
--rw-rw-rw-   0        0        0      183 2023-08-04 13:16:21.000000 NiantongEEG-0.1.3.8/NiantongEEG.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2023-08-04 13:16:21.000000 NiantongEEG-0.1.3.8/NiantongEEG.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 13:16:21.000000 NiantongEEG-0.1.3.8/NiantongEEG.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-08-04 13:16:21.000000 NiantongEEG-0.1.3.8/NiantongEEG.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        1 2023-08-04 13:16:21.000000 NiantongEEG-0.1.3.8/NiantongEEG.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      183 2023-08-04 13:16:21.952993 NiantongEEG-0.1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-08-04 13:16:21.952993 NiantongEEG-0.1.3.8/setup.cfg
--rw-rw-rw-   0        0        0      231 2023-08-04 13:15:58.000000 NiantongEEG-0.1.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 13:15:28.047926 NiantongEEG-0.1.3.9/
+drwxrwxrwx   0        0        0        0 2023-08-04 13:15:28.047926 NiantongEEG-0.1.3.9/NiantongEEG.egg-info/
+-rw-rw-rw-   0        0        0      174 2023-08-04 13:15:28.000000 NiantongEEG-0.1.3.9/NiantongEEG.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2023-08-04 13:15:28.000000 NiantongEEG-0.1.3.9/NiantongEEG.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 13:15:28.000000 NiantongEEG-0.1.3.9/NiantongEEG.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-08-04 13:15:28.000000 NiantongEEG-0.1.3.9/NiantongEEG.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        1 2023-08-04 13:15:28.000000 NiantongEEG-0.1.3.9/NiantongEEG.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      174 2023-08-04 13:15:28.047926 NiantongEEG-0.1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-08-04 13:15:28.047926 NiantongEEG-0.1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      231 2023-08-04 13:15:11.000000 NiantongEEG-0.1.3.9/setup.py
```

