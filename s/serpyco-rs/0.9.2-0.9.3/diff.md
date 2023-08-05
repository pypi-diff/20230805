# Comparing `tmp/serpyco_rs-0.9.2.tar.gz` & `tmp/serpyco_rs-0.9.3.tar.gz`

## Comparing `serpyco_rs-0.9.2.tar` & `serpyco_rs-0.9.3.tar`

### file list

```diff
@@ -1,64 +1,65 @@
--rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 serpyco_rs-0.9.2/Cargo.toml
--rw-r--r--   0     1001      123       25 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.envrc.example
--rw-r--r--   0     1001      123      196 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.github/dependabot.yml
--rw-r--r--   0     1001      123     4009 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/.gitignore
--rw-r--r--   0     1001      123     1069 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/LICENSE
--rw-r--r--   0     1001      123       34 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/MANIFEST.in
--rw-r--r--   0     1001      123     8943 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/README.md
--rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/__init__.py
--rw-r--r--   0     1001      123     1832 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/graph.py
--rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/__init__.py
--rw-r--r--   0     1001      123      645 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/base.py
--rw-r--r--   0     1001      123      356 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/marshmallow.py
--rw-r--r--   0     1001      123      704 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/mashumaro.py
--rw-r--r--   0     1001      123      521 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/pydantic.py
--rw-r--r--   0     1001      123      355 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/serpyco.py
--rw-r--r--   0     1001      123      361 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/libs/serpyco_rs.py
--rw-r--r--   0     1001      123     1642 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/compare/test_benchmarks.py
--rw-r--r--   0     1001      123     6092 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/test_encoders.py
--rw-r--r--   0     1001      123      803 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/test_full.py
--rw-r--r--   0     1001      123      197 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/bench/utils.py
--rw-r--r--   0     1001      123     2289 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/noxfile.py
--rw-r--r--   0     1001      123      948 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/pyproject.toml
--rw-r--r--   0     1001      123      152 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/__init__.py
--rw-r--r--   0     1001      123    16825 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_describe.py
--rw-r--r--   0     1001      123       72 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_impl.py
--rw-r--r--   0     1001      123      320 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_impl.pyi
--rw-r--r--   0     1001      123      199 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/__init__.py
--rw-r--r--   0     1001      123     6015 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_convert.py
--rw-r--r--   0     1001      123     5094 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_entities.py
--rw-r--r--   0     1001      123     1035 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_validate.py
--rw-r--r--   0     1001      123     1234 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_main.py
--rw-r--r--   0     1001      123      166 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/_utils.py
--rw-r--r--   0     1001      123      364 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/exceptions.py
--rw-r--r--   0     1001      123     1464 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/metadata.py
--rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/python/serpyco_rs/py.typed
--rw-r--r--   0     1001      123      110 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/bench.txt
--rw-r--r--   0     1001      123       78 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/dev.txt
--rw-r--r--   0     1001      123       29 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/lint.txt
--rw-r--r--   0     1001      123       47 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/requirements/type_check.txt
--rwxr-xr-x   0     1001      123     1013 2023-04-26 18:01:37.000000 serpyco_rs-0.9.2/run-maturin-action.sh
--rw-r--r--   0     1001      123       54 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/build.rs
--rw-r--r--   0     1001      123      297 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/lib.rs
--rw-r--r--   0     1001      123     4430 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/dateutil.rs
--rw-r--r--   0     1001      123    13465 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/encoders.rs
--rw-r--r--   0     1001      123     2252 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/macros.rs
--rw-r--r--   0     1001      123     9108 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/main.rs
--rw-r--r--   0     1001      123     5126 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/py.rs
--rw-r--r--   0     1001      123     7134 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer/types.rs
--rw-r--r--   0     1001      123      152 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/src/serializer.rs
--rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/__init__.py
--rw-r--r--   0     1001      123        0 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/json_schema/__init__.py
--rw-r--r--   0     1001      123    11743 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/json_schema/test_convert.py
--rw-r--r--   0     1001      123     6944 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/json_schema/test_validator.py
--rw-r--r--   0     1001      123    20837 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test__describe.py
--rw-r--r--   0     1001      123     1234 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_custom_encoder.py
--rw-r--r--   0     1001      123     5798 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_encoders.py
--rw-r--r--   0     1001      123     1496 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_metadata.py
--rw-r--r--   0     1001      123     2567 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_recursive.py
--rw-r--r--   0     1001      123     6100 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_simple.py
--rw-r--r--   0     1001      123     4304 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/tests/test_union.py
--rw-r--r--   0     1001      123    14885 2023-04-26 18:01:08.000000 serpyco_rs-0.9.2/Cargo.lock
--rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 serpyco_rs-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0      588 1970-01-01 00:00:00.000000 serpyco_rs-0.9.3/Cargo.toml
+-rw-r--r--   0     1001      123       25 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/.envrc.example
+-rw-r--r--   0     1001      123      196 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/.github/dependabot.yml
+-rw-r--r--   0     1001      123     4009 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/.gitignore
+-rw-r--r--   0     1001      123     1069 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/LICENSE
+-rw-r--r--   0     1001      123       34 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/MANIFEST.in
+-rw-r--r--   0     1001      123     8943 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/README.md
+-rw-r--r--   0     1001      123        0 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/__init__.py
+-rw-r--r--   0     1001      123     1832 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/graph.py
+-rw-r--r--   0     1001      123        0 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/__init__.py
+-rw-r--r--   0     1001      123      645 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/base.py
+-rw-r--r--   0     1001      123      356 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/marshmallow.py
+-rw-r--r--   0     1001      123      704 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/mashumaro.py
+-rw-r--r--   0     1001      123      521 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/pydantic.py
+-rw-r--r--   0     1001      123      355 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/serpyco.py
+-rw-r--r--   0     1001      123      361 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/libs/serpyco_rs.py
+-rw-r--r--   0     1001      123     1642 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/compare/test_benchmarks.py
+-rw-r--r--   0     1001      123     6092 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/test_encoders.py
+-rw-r--r--   0     1001      123      803 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/test_full.py
+-rw-r--r--   0     1001      123      197 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/bench/utils.py
+-rw-r--r--   0     1001      123     2289 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/noxfile.py
+-rw-r--r--   0     1001      123      948 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/pyproject.toml
+-rw-r--r--   0     1001      123      152 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/__init__.py
+-rw-r--r--   0     1001      123    17521 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_describe.py
+-rw-r--r--   0     1001      123       72 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_impl.py
+-rw-r--r--   0     1001      123      320 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_impl.pyi
+-rw-r--r--   0     1001      123      199 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/__init__.py
+-rw-r--r--   0     1001      123     6015 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/_convert.py
+-rw-r--r--   0     1001      123     5094 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/_entities.py
+-rw-r--r--   0     1001      123     1035 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/_validate.py
+-rw-r--r--   0     1001      123     1234 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_main.py
+-rw-r--r--   0     1001      123      166 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/_utils.py
+-rw-r--r--   0     1001      123      364 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/exceptions.py
+-rw-r--r--   0     1001      123     1464 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/metadata.py
+-rw-r--r--   0     1001      123        0 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/python/serpyco_rs/py.typed
+-rw-r--r--   0     1001      123      110 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/requirements/bench.txt
+-rw-r--r--   0     1001      123       78 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/requirements/dev.txt
+-rw-r--r--   0     1001      123       29 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/requirements/lint.txt
+-rw-r--r--   0     1001      123       47 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/requirements/type_check.txt
+-rwxr-xr-x   0     1001      123     1013 2023-04-30 22:49:17.000000 serpyco_rs-0.9.3/run-maturin-action.sh
+-rw-r--r--   0     1001      123       54 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/build.rs
+-rw-r--r--   0     1001      123      297 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/lib.rs
+-rw-r--r--   0     1001      123     4430 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer/dateutil.rs
+-rw-r--r--   0     1001      123    13465 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer/encoders.rs
+-rw-r--r--   0     1001      123     2252 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer/macros.rs
+-rw-r--r--   0     1001      123     9108 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer/main.rs
+-rw-r--r--   0     1001      123     5126 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer/py.rs
+-rw-r--r--   0     1001      123     7134 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer/types.rs
+-rw-r--r--   0     1001      123      152 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/src/serializer.rs
+-rw-r--r--   0     1001      123        0 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/__init__.py
+-rw-r--r--   0     1001      123        0 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/json_schema/__init__.py
+-rw-r--r--   0     1001      123    11743 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/json_schema/test_convert.py
+-rw-r--r--   0     1001      123     6944 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/json_schema/test_validator.py
+-rw-r--r--   0     1001      123    20843 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test__describe.py
+-rw-r--r--   0     1001      123     1234 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_custom_encoder.py
+-rw-r--r--   0     1001      123     5798 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_encoders.py
+-rw-r--r--   0     1001      123     6747 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_generics.py
+-rw-r--r--   0     1001      123     1496 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_metadata.py
+-rw-r--r--   0     1001      123     2472 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_recursive.py
+-rw-r--r--   0     1001      123     6100 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_simple.py
+-rw-r--r--   0     1001      123     4304 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/tests/test_union.py
+-rw-r--r--   0     1001      123    14885 2023-04-30 22:48:43.000000 serpyco_rs-0.9.3/Cargo.lock
+-rw-r--r--   0        0        0     9858 1970-01-01 00:00:00.000000 serpyco_rs-0.9.3/PKG-INFO
```

### Comparing `serpyco_rs-0.9.2/Cargo.toml` & `serpyco_rs-0.9.3/Cargo.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "serpyco-rs"
-version = "0.9.2"
+version = "0.9.3"
 edition = "2021"
 homepage = "https://github.com/ermakov-oleg/serpyco-rs"
 repository = "https://github.com/ermakov-oleg/serpyco-rs"
 
 [package.metadata.maturin]
 python-source = "python"
 name = "serpyco_rs._serpyco_rs"
```

### Comparing `serpyco_rs-0.9.2/.github/workflows/CI.yml` & `serpyco_rs-0.9.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/.gitignore` & `serpyco_rs-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/LICENSE` & `serpyco_rs-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/README.md` & `serpyco_rs-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/compare/graph.py` & `serpyco_rs-0.9.3/bench/compare/graph.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/compare/libs/base.py` & `serpyco_rs-0.9.3/bench/compare/libs/base.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/compare/libs/mashumaro.py` & `serpyco_rs-0.9.3/bench/compare/libs/mashumaro.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/compare/libs/pydantic.py` & `serpyco_rs-0.9.3/bench/compare/libs/pydantic.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/compare/test_benchmarks.py` & `serpyco_rs-0.9.3/bench/compare/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/test_encoders.py` & `serpyco_rs-0.9.3/bench/test_encoders.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/bench/test_full.py` & `serpyco_rs-0.9.3/bench/test_full.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/noxfile.py` & `serpyco_rs-0.9.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/pyproject.toml` & `serpyco_rs-0.9.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/python/serpyco_rs/_describe.py` & `serpyco_rs-0.9.3/python/serpyco_rs/_describe.py`

 * *Files 6% similar despite different names*

```diff
@@ -156,15 +156,15 @@
 
 @dataclasses.dataclass
 class EntityType(Type):
     cls: type[Any]
     name: str
     fields: Sequence[EntityField]
     omit_none: bool = False
-    generics: Mapping[TypeVar, Any] = dataclasses.field(default_factory=dict)
+    generics: Sequence[tuple[TypeVar, Any]] = tuple()
     doc: Optional[str] = None
 
 
 @dataclasses.dataclass
 class OptionalType(Type):
     inner: Type
 
@@ -196,34 +196,49 @@
 
 
 @dataclasses.dataclass
 class AnyType(Type):
     pass
 
 
-@dataclasses.dataclass
-class RecursionHolder(Type):
-    cls: Any
-    name: str
+@dataclasses.dataclass(frozen=True, unsafe_hash=True)
+class _MetaStateKey:
+    cls: type
     field_format: FiledFormat
-    meta: "_Meta"
-    none_format: NoneFormat = KeepNone
-
-    def get_type(self) -> Type:
-        if type_ := self.meta.state[(self.cls, self.field_format, self.none_format)]:
-            return type_
-        raise RuntimeError("Recursive type not resolved")
+    none_format: NoneFormat
+    generics: Sequence[tuple[TypeVar, Any]]
 
 
 @dataclasses.dataclass
 class _Meta:
     globals: dict[str, Any]
-    state: dict[tuple[type, FiledFormat, NoneFormat], Optional[Type]]
+    state: dict[_MetaStateKey, Optional[Type]]
     discriminator_field: Optional[str] = None
 
+    def add_to_state(self, key: _MetaStateKey, value: Optional[Type]) -> None:
+        self.state[key] = value
+
+    def get_from_state(self, key: _MetaStateKey) -> Optional[Type]:
+        return self.state.get(key)
+
+    def has_in_state(self, key: _MetaStateKey) -> bool:
+        return key in self.state
+
+
+@dataclasses.dataclass
+class RecursionHolder(Type):
+    name: str
+    state_key: _MetaStateKey
+    meta: _Meta
+
+    def get_type(self) -> Type:
+        if type_ := self.meta.get_from_state(self.state_key):
+            return type_
+        raise RuntimeError("Recursive type not resolved")
+
 
 def describe_type(t: Any, meta: Optional[_Meta] = None) -> Type:
     parameters: tuple[Any, ...] = ()
     args: tuple[Any, ...] = ()
     metadata = _get_annotated_metadata(t)
     if get_origin(t) == Annotated:  # unwrap annotated
         t = t.__origin__
@@ -241,27 +256,32 @@
         args = (Any,) * len(parameters)
 
     if not meta:
         meta = _Meta(globals=_get_globals(t), state={})
 
     t = _evaluate_forwardref(t, meta)
 
-    generics = dict(zip(parameters, args))
+    generics = tuple((k, v) for k, v in sorted(zip(parameters, args), key=lambda x: repr(x[0])))
     filed_format = _find_metadata(metadata, FiledFormat, NoFormat)
     none_format = _find_metadata(metadata, NoneFormat, KeepNone)
     custom_encoder = _find_metadata(metadata, CustomEncoder)
     annotation_wrapper = _wrap_annotated([filed_format, none_format])
 
-    if (t, filed_format, none_format) in meta.state:
+    meta_key = _MetaStateKey(
+        cls=t,
+        field_format=filed_format,
+        none_format=none_format,
+        generics=generics,
+    )
+
+    if meta.has_in_state(meta_key):
         return RecursionHolder(
-            cls=t,
-            name=_generate_name(t, filed_format, none_format),
-            field_format=filed_format,
-            none_format=none_format,
+            name=_generate_name(t, filed_format, none_format, generics),
             meta=meta,
+            state_key=meta_key,
             custom_encoder=None,
         )
 
     if t is Any:
         return AnyType(custom_encoder=custom_encoder)
 
     if isinstance(t, type):
@@ -335,24 +355,24 @@
                 custom_encoder=custom_encoder,
             )
 
         if issubclass(t, (Enum, IntEnum)):
             return EnumType(cls=t, custom_encoder=custom_encoder)
 
         if dataclasses.is_dataclass(t) or _is_attrs(t):
-            meta.state[(t, filed_format, none_format)] = None
+            meta.add_to_state(meta_key, None)
             entity_type = _describe_entity(
                 t=t,
                 generics=generics,
                 cls_filed_format=filed_format,
                 cls_none_format=none_format,
                 custom_encoder=custom_encoder,
                 meta=meta,
             )
-            meta.state[(t, filed_format, none_format)] = entity_type
+            meta.add_to_state(meta_key, entity_type)
             return entity_type
 
     if _is_literal_type(t):
         if args and all((isinstance(arg, str) for arg in args)):
             return LiteralType(args=args, custom_encoder=custom_encoder)
         raise RuntimeError("Supported only Literal[str, ...]")
 
@@ -393,15 +413,15 @@
     type: type[_T]
     default: Union[_T, NotSet] = NOT_SET
     default_factory: Union[Callable[[], _T], NotSet] = NOT_SET
 
 
 def _describe_entity(
     t: Any,
-    generics: Mapping[TypeVar, Any],
+    generics: Sequence[tuple[TypeVar, Any]],
     cls_filed_format: FiledFormat,
     cls_none_format: NoneFormat,
     custom_encoder: Optional[CustomEncoder[Any, Any]],
     meta: _Meta,
 ) -> EntityType:
     docs = get_attributes_doc(t)
     try:
@@ -432,15 +452,15 @@
                 is_property=False,
                 is_discriminator_field=field.name == discriminator_field,
             )
         )
 
     return EntityType(
         cls=t,
-        name=_generate_name(t, cls_filed_format, cls_none_format),
+        name=_generate_name(t, cls_filed_format, cls_none_format, generics),
         fields=fields,
         omit_none=cls_none_format is OmitNone,
         generics=generics,
         doc=t.__doc__,
         custom_encoder=custom_encoder,
     )
 
@@ -476,20 +496,21 @@
             )
             for f in attr.fields(t)
         ]
 
     raise RuntimeError(f"Unsupported type '{t}'")
 
 
-def _replace_generics(t: Any, generics: Mapping[TypeVar, Any]) -> Any:
+def _replace_generics(t: Any, generics: Sequence[tuple[TypeVar, Any]]) -> Any:
     try:
+        generics_map = dict(generics)
         if parameters := getattr(t, "__parameters__", None):
-            t = t[tuple(generics[parameter] for parameter in parameters)]
+            t = t[tuple(generics_map[parameter] for parameter in parameters)]
         if isinstance(t, TypeVar):
-            t = generics[t]
+            t = generics_map[t]
     except KeyError as exc:
         raise RuntimeError(f"Unfilled TypeVar: {exc.args[0]}") from exc
     return t
 
 
 @overload
 def _find_metadata(annotations: Iterable[Any], type_: type[_T], default: _T) -> _T:
@@ -524,17 +545,23 @@
     if not f or f.format is Format.no_format:
         return value
     if f.format is Format.camel_case:
         return to_camelcase(value)
     assert_never(f.format)
 
 
-def _generate_name(cls: Any, field_format: FiledFormat, none_format: NoneFormat) -> str:
+def _generate_name(
+    cls: Any, field_format: FiledFormat, none_format: NoneFormat, generics: Sequence[tuple[TypeVar, Any]]
+) -> str:
+    name = cls.__name__
+    if generics:
+        cls = _replace_generics(cls, generics)
+        name = repr(cls)
     nones = "omit_nones" if none_format.omit else "keep_nones"
-    return f"{cls.__module__}.{cls.__name__}[{field_format.format.value},{nones}]"
+    return f"{cls.__module__}.{name}[{field_format.format.value},{nones}]"
 
 
 def _get_globals(t: Any) -> dict[str, Any]:
     if t.__module__ in sys.modules:
         return sys.modules[t.__module__].__dict__.copy()
     return {}
```

### Comparing `serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_convert.py` & `serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/_convert.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_entities.py` & `serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/_entities.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/python/serpyco_rs/_json_schema/_validate.py` & `serpyco_rs-0.9.3/python/serpyco_rs/_json_schema/_validate.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/python/serpyco_rs/_main.py` & `serpyco_rs-0.9.3/python/serpyco_rs/_main.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/python/serpyco_rs/metadata.py` & `serpyco_rs-0.9.3/python/serpyco_rs/metadata.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/run-maturin-action.sh` & `serpyco_rs-0.9.3/run-maturin-action.sh`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/src/serializer/dateutil.rs` & `serpyco_rs-0.9.3/src/serializer/dateutil.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/src/serializer/encoders.rs` & `serpyco_rs-0.9.3/src/serializer/encoders.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/src/serializer/macros.rs` & `serpyco_rs-0.9.3/src/serializer/macros.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/src/serializer/main.rs` & `serpyco_rs-0.9.3/src/serializer/main.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/src/serializer/py.rs` & `serpyco_rs-0.9.3/src/serializer/py.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/src/serializer/types.rs` & `serpyco_rs-0.9.3/src/serializer/types.rs`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/json_schema/test_convert.py` & `serpyco_rs-0.9.3/tests/json_schema/test_convert.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/json_schema/test_validator.py` & `serpyco_rs-0.9.3/tests/json_schema/test_validator.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/test__describe.py` & `serpyco_rs-0.9.3/tests/test__describe.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
                             doc=None,
                             default=NOT_SET,
                             default_factory=NOT_SET,
                             is_property=False,
                             dict_key="a",
                         )
                     ],
-                    generics={},
+                    generics=(),
                     doc="SomeOtherEntity(a: int)",
                     custom_encoder=None,
                 ),
                 doc=None,
                 default=NOT_SET,
                 default_factory=NOT_SET,
                 is_property=False,
@@ -249,15 +249,15 @@
                 doc=None,
                 default=NOT_SET,
                 default_factory=NOT_SET,
                 is_property=False,
                 dict_key="p",
             ),
         ],
-        generics={},
+        generics=(),
         doc="Doc",
         custom_encoder=None,
     )
 
 
 def test_describe_dataclass__dict_type__works_without_type_parameters():
     @dataclass
@@ -316,15 +316,15 @@
     class SomeEntity(Generic[T]):
         x: list[T]
 
     result: EntityType = describe_type(SomeEntity)
     assert result.fields[0].type == ArrayType(
         item_type=AnyType(custom_encoder=None), is_sequence=False, custom_encoder=None
     )
-    assert result.generics == {T: Any}
+    assert result.generics == ((T, Any),)
 
 
 def test_describe_dataclass__generic_with_type_params__expected_right_type():
     @dataclass
     class SomeOtherEntity(Generic[T]):
         x: T
 
@@ -336,15 +336,15 @@
     result: EntityType = describe_type(SomeEntity[int])
     assert result.fields[0].type == ArrayType(
         item_type=IntegerType(custom_encoder=None), is_sequence=False, custom_encoder=None
     )
     assert result.fields[1].type == EntityType(
         cls=SomeOtherEntity,
         name=ANY,
-        generics={T: int},
+        generics=((T, int),),
         fields=[EntityField(name="x", type=IntegerType(custom_encoder=None), dict_key="x")],
         doc="SomeOtherEntity(x: ~T)",
         custom_encoder=None,
     )
 
 
 def test_describe_dataclass__used_unknown_type_var__fail():
```

### Comparing `serpyco_rs-0.9.2/tests/test_custom_encoder.py` & `serpyco_rs-0.9.3/tests/test_custom_encoder.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/test_encoders.py` & `serpyco_rs-0.9.3/tests/test_encoders.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/test_metadata.py` & `serpyco_rs-0.9.3/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/test_recursive.py` & `serpyco_rs-0.9.3/tests/test_recursive.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from dataclasses import dataclass
 from typing import Optional
 from unittest.mock import ANY
 
 from serpyco_rs import Serializer
 from serpyco_rs._describe import EntityField, EntityType, OptionalType, RecursionHolder, StringType, describe_type
-from serpyco_rs.metadata import NoFormat
 
 
 @dataclass
 class Node:
     value: str
     next: Optional["Node"] = None
 
@@ -37,18 +36,17 @@
                         ),
                         EntityField(
                             name="next",
                             dict_key="next",
                             default=None,
                             type=OptionalType(
                                 inner=RecursionHolder(
-                                    cls=Node,
                                     name=ANY,
-                                    field_format=NoFormat,
                                     meta=ANY,
+                                    state_key=ANY,
                                     custom_encoder=None,
                                 ),
                                 custom_encoder=None,
                             ),
                         ),
                     ],
                     doc=ANY,
```

### Comparing `serpyco_rs-0.9.2/tests/test_simple.py` & `serpyco_rs-0.9.3/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/tests/test_union.py` & `serpyco_rs-0.9.3/tests/test_union.py`

 * *Files identical despite different names*

### Comparing `serpyco_rs-0.9.2/Cargo.lock` & `serpyco_rs-0.9.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 name = "scratch"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8132065adcfd6e02db789d9285a0deb2f3fcb04002865ab67d5fb103533898"
 
 [[package]]
 name = "serpyco-rs"
-version = "0.9.2"
+version = "0.9.3"
 dependencies = [
  "atomic_refcell",
  "cfg-if",
  "chrono",
  "dyn-clone",
  "pyo3",
  "pyo3-build-config",
```

### Comparing `serpyco_rs-0.9.2/PKG-INFO` & `serpyco_rs-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serpyco-rs
-Version: 0.9.2
+Version: 0.9.3
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

