# Comparing `tmp/tech-spec-1.0.29.tar.gz` & `tmp/tech-spec-1.0.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.29.tar", last modified: Sat Aug  5 12:02:13 2023, max compression
+gzip compressed data, was "tech-spec-1.0.30.tar", last modified: Sat Aug  5 12:08:53 2023, max compression
```

## Comparing `tech-spec-1.0.29.tar` & `tech-spec-1.0.30.tar`

### file list

```diff
@@ -1,26 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:02:13.689319 tech-spec-1.0.29/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:02:04.000000 tech-spec-1.0.29/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:02:04.000000 tech-spec-1.0.29/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:02:13.689319 tech-spec-1.0.29/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:02:04.000000 tech-spec-1.0.29/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/groups/stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/schema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.361912 tech-spec-1.0.30/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-05 12:08:44.000000 tech-spec-1.0.30/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:08:53.357912 tech-spec-1.0.30/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:08:44.000000 tech-spec-1.0.30/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:08:44.000000 tech-spec-1.0.30/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:08:53.361912 tech-spec-1.0.30/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:08:44.000000 tech-spec-1.0.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/groups/stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/schema/utils.py
```

### Comparing `tech-spec-1.0.29/setup.py` & `tech-spec-1.0.30/setup.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.29/techspec/cli/groups/schema.py` & `tech-spec-1.0.30/techspec/cli/groups/schema.py`

 * *Files identical despite different names*

