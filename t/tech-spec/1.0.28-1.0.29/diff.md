# Comparing `tmp/tech-spec-1.0.28.tar.gz` & `tmp/tech-spec-1.0.29.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tech-spec-1.0.28.tar", last modified: Sat Aug  5 11:49:00 2023, max compression
+gzip compressed data, was "tech-spec-1.0.29.tar", last modified: Sat Aug  5 12:02:13 2023, max compression
```

## Comparing `tech-spec-1.0.28.tar` & `tech-spec-1.0.29.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:00.676956 tech-spec-1.0.28/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 11:49:00.676956 tech-spec-1.0.28/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 11:48:52.000000 tech-spec-1.0.28/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 11:48:52.000000 tech-spec-1.0.28/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 11:49:00.676956 tech-spec-1.0.28/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-08-05 11:48:52.000000 tech-spec-1.0.28/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:00.676956 tech-spec-1.0.28/tech_spec.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 11:49:00.000000 tech-spec-1.0.28/tech_spec.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-08-05 11:49:00.000000 tech-spec-1.0.28/tech_spec.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:49:00.000000 tech-spec-1.0.28/tech_spec.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 11:49:00.000000 tech-spec-1.0.28/tech_spec.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 11:49:00.000000 tech-spec-1.0.28/tech_spec.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:00.676956 tech-spec-1.0.28/techspec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:00.676956 tech-spec-1.0.28/techspec/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:00.676956 tech-spec-1.0.28/techspec/cli/groups/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/cli/groups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/cli/groups/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/cli/groups/stderr.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:49:00.676956 tech-spec-1.0.28/techspec/schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/schema/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 11:48:52.000000 tech-spec-1.0.28/techspec/schema/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:02:13.689319 tech-spec-1.0.29/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-08-05 12:02:04.000000 tech-spec-1.0.29/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-08-05 12:02:04.000000 tech-spec-1.0.29/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 12:02:13.689319 tech-spec-1.0.29/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-08-05 12:02:04.000000 tech-spec-1.0.29/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/tech_spec.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-08-05 12:02:13.000000 tech-spec-1.0.29/tech_spec.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/cli/groups/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/groups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/groups/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/groups/stderr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:13.689319 tech-spec-1.0.29/techspec/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/schema/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-08-05 12:02:04.000000 tech-spec-1.0.29/techspec/schema/utils.py
```

### Comparing `tech-spec-1.0.28/setup.py` & `tech-spec-1.0.29/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 setup(
     name="tech-spec",
     version=os.environ["GITHUB_REF_NAME"],
     description="Tech spec for code generation",
     author="Vladimir Vojtenko",
     author_email="vladimirdev635@gmail.com",
     license="MIT",
+    install_requires=["typer[all]", "pyyaml", "jsonschema"],
     packages=find_packages(exclude=["__tests__*"]),
     include_package_data=True,
     long_description=(Path(__file__).parent / "README.md").read_text(),
     long_description_content_type="text/markdown",
     entry_points={"console_scripts": ["techspecpy=techspec.cli:cli_main"]},
 )
```

### Comparing `tech-spec-1.0.28/techspec/cli/groups/schema.py` & `tech-spec-1.0.29/techspec/cli/groups/schema.py`

 * *Files identical despite different names*

