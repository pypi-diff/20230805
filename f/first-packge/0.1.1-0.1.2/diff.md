# Comparing `tmp/first_packge-0.1.1.tar.gz` & `tmp/first_packge-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "first_packge-0.1.1.tar", last modified: Sat Aug  5 19:42:06 2023, max compression
+gzip compressed data, was "first_packge-0.1.2.tar", last modified: Sat Aug  5 19:49:36 2023, max compression
```

## Comparing `first_packge-0.1.1.tar` & `first_packge-0.1.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 19:42:06.422571 first_packge-0.1.1/
--rw-rw-rw-   0        0        0      146 2023-08-05 19:42:06.422015 first_packge-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-08-05 19:42:06.421111 first_packge-0.1.1/first_packge.egg-info/
--rw-rw-rw-   0        0        0      146 2023-08-05 19:42:06.000000 first_packge-0.1.1/first_packge.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      152 2023-08-05 19:42:06.000000 first_packge-0.1.1/first_packge.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 19:42:06.000000 first_packge-0.1.1/first_packge.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 19:42:06.000000 first_packge-0.1.1/first_packge.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 19:42:06.423068 first_packge-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      297 2023-08-05 19:41:59.000000 first_packge-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 19:49:36.238537 first_packge-0.1.2/
+-rw-rw-rw-   0        0        0      146 2023-08-05 19:49:36.236318 first_packge-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-08-05 19:49:36.235065 first_packge-0.1.2/first_packge.egg-info/
+-rw-rw-rw-   0        0        0      146 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      152 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 19:49:36.000000 first_packge-0.1.2/first_packge.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 19:49:36.238537 first_packge-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      297 2023-08-05 19:49:12.000000 first_packge-0.1.2/setup.py
```

