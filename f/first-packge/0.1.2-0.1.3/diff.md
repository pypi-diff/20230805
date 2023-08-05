# Comparing `tmp/first_packge-0.1.2.tar.gz` & `tmp/first_packge-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first_packge-0.1.2.tar", last modified: Sat Aug  5 19:49:36 2023, max compression
+gzip compressed data, was "first_packge-0.1.3.tar", last modified: Sat Aug  5 19:57:17 2023, max compression
```

## Comparing `first_packge-0.1.2.tar` & `first_packge-0.1.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 19:49:36.238537 first_packge-0.1.2/
--rw-rw-rw-   0        0        0      146 2023-08-05 19:49:36.236318 first_packge-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 19:49:36.235065 first_packge-0.1.2/first_packge.egg-info/
--rw-rw-rw-   0        0        0      146 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 19:49:36.238537 first_packge-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-08-05 19:49:12.000000 first_packge-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 19:57:17.667374 first_packge-0.1.3/
+-rw-rw-rw-   0        0        0      318 2023-08-05 19:57:17.666853 first_packge-0.1.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 19:57:17.665927 first_packge-0.1.3/first_packge.egg-info/
+-rw-rw-rw-   0        0        0      318 2023-08-05 19:57:17.000000 first_packge-0.1.3/first_packge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-08-05 19:57:17.000000 first_packge-0.1.3/first_packge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 19:57:17.000000 first_packge-0.1.3/first_packge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 19:57:17.000000 first_packge-0.1.3/first_packge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 19:57:17.667870 first_packge-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      462 2023-08-05 19:57:11.000000 first_packge-0.1.3/setup.py
```

