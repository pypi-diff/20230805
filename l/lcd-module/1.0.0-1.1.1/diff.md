# Comparing `tmp/lcd_module-1.0.0.tar.gz` & `tmp/lcd_module-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lcd_module-1.0.0.tar", last modified: Sat Aug  5 09:01:12 2023, max compression
+gzip compressed data, was "lcd_module-1.1.1.tar", last modified: Sat Aug  5 10:06:59 2023, max compression
```

## Comparing `lcd_module-1.0.0.tar` & `lcd_module-1.1.1.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 octopi    (1000) octopi    (1000)        0 2023-08-05 09:01:12.398909 lcd_module-1.0.0/
--rw-r--r--   0 octopi    (1000) octopi    (1000)      221 2023-08-05 09:01:12.394909 lcd_module-1.0.0/PKG-INFO
-drwxr-xr-x   0 octopi    (1000) octopi    (1000)        0 2023-08-05 09:01:12.394909 lcd_module-1.0.0/lcd_module.egg-info/
--rw-r--r--   0 octopi    (1000) octopi    (1000)      221 2023-08-05 09:01:11.000000 lcd_module-1.0.0/lcd_module.egg-info/PKG-INFO
--rw-r--r--   0 octopi    (1000) octopi    (1000)      191 2023-08-05 09:01:12.000000 lcd_module-1.0.0/lcd_module.egg-info/SOURCES.txt
--rw-r--r--   0 octopi    (1000) octopi    (1000)        1 2023-08-05 09:01:11.000000 lcd_module-1.0.0/lcd_module.egg-info/dependency_links.txt
--rw-r--r--   0 octopi    (1000) octopi    (1000)       13 2023-08-05 09:01:11.000000 lcd_module-1.0.0/lcd_module.egg-info/requires.txt
--rw-r--r--   0 octopi    (1000) octopi    (1000)       11 2023-08-05 09:01:11.000000 lcd_module-1.0.0/lcd_module.egg-info/top_level.txt
--rw-r--r--   0 octopi    (1000) octopi    (1000)      631 2023-08-03 10:47:54.000000 lcd_module-1.0.0/lcd_module.py
--rw-r--r--   0 octopi    (1000) octopi    (1000)       38 2023-08-05 09:01:12.398909 lcd_module-1.0.0/setup.cfg
--rw-r--r--   0 octopi    (1000) octopi    (1000)      349 2023-08-05 08:58:34.000000 lcd_module-1.0.0/setup.py
+drwxr-xr-x   0 octopi    (1000) octopi    (1000)        0 2023-08-05 10:06:59.720281 lcd_module-1.1.1/
+-rw-r--r--   0 octopi    (1000) octopi    (1000)      221 2023-08-05 10:06:59.720281 lcd_module-1.1.1/PKG-INFO
+-rw-r--r--   0 octopi    (1000) octopi    (1000)      249 2023-08-05 09:34:45.000000 lcd_module-1.1.1/README.txt
+drwxr-xr-x   0 octopi    (1000) octopi    (1000)        0 2023-08-05 10:06:59.720281 lcd_module-1.1.1/lcd_module.egg-info/
+-rw-r--r--   0 octopi    (1000) octopi    (1000)      221 2023-08-05 10:06:59.000000 lcd_module-1.1.1/lcd_module.egg-info/PKG-INFO
+-rw-r--r--   0 octopi    (1000) octopi    (1000)      202 2023-08-05 10:06:59.000000 lcd_module-1.1.1/lcd_module.egg-info/SOURCES.txt
+-rw-r--r--   0 octopi    (1000) octopi    (1000)        1 2023-08-05 10:06:59.000000 lcd_module-1.1.1/lcd_module.egg-info/dependency_links.txt
+-rw-r--r--   0 octopi    (1000) octopi    (1000)       13 2023-08-05 10:06:59.000000 lcd_module-1.1.1/lcd_module.egg-info/requires.txt
+-rw-r--r--   0 octopi    (1000) octopi    (1000)       11 2023-08-05 10:06:59.000000 lcd_module-1.1.1/lcd_module.egg-info/top_level.txt
+-rw-r--r--   0 octopi    (1000) octopi    (1000)     1722 2023-08-05 09:59:58.000000 lcd_module-1.1.1/lcd_module.py
+-rw-r--r--   0 octopi    (1000) octopi    (1000)       38 2023-08-05 10:06:59.720281 lcd_module-1.1.1/setup.cfg
+-rw-r--r--   0 octopi    (1000) octopi    (1000)      349 2023-08-05 10:00:13.000000 lcd_module-1.1.1/setup.py
```

