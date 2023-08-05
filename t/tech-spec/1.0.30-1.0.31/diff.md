# Comparing `tmp/tech-spec-1.0.30.tar.gz` & `tmp/tech-spec-1.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.30.tar", last modified: Sat Aug  5 12:08:53 2023, max compression
+gzip compressed data, was "tech-spec-1.0.31.tar", last modified: Sat Aug  5 12:13:06 2023, max compression
```

## Comparing `tech-spec-1.0.30.tar` & `tech-spec-1.0.31.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.361912 tech-spec-1.0.30/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-08-05 12:08:44.000000 tech-spec-1.0.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:08:53.357912 tech-spec-1.0.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:08:44.000000 tech-spec-1.0.30/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:08:44.000000 tech-spec-1.0.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:08:53.361912 tech-spec-1.0.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:08:44.000000 tech-spec-1.0.30/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      506 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:08:53.000000 tech-spec-1.0.30/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/groups/stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:53.357912 tech-spec-1.0.30/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:08:44.000000 tech-spec-1.0.30/techspec/schema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.768698 tech-spec-1.0.31/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-08-05 12:12:52.000000 tech-spec-1.0.31/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:13:06.768698 tech-spec-1.0.31/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:12:52.000000 tech-spec-1.0.31/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:12:52.000000 tech-spec-1.0.31/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:13:06.768698 tech-spec-1.0.31/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:12:52.000000 tech-spec-1.0.31/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.764698 tech-spec-1.0.31/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:13:06.000000 tech-spec-1.0.31/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.764698 tech-spec-1.0.31/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.764698 tech-spec-1.0.31/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.768698 tech-spec-1.0.31/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/groups/stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:13:06.768698 tech-spec-1.0.31/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-08-05 12:12:52.000000 tech-spec-1.0.31/techspec/schema.json
```

### Comparing `tech-spec-1.0.30/setup.py` & `tech-spec-1.0.31/setup.py`

 * *Files identical despite different names*

### Comparing `tech-spec-1.0.30/techspec/cli/groups/schema.py` & `tech-spec-1.0.31/techspec/cli/groups/schema.py`

 * *Files identical despite different names*

