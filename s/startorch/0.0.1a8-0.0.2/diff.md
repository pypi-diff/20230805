# Comparing `tmp/startorch-0.0.1a8.tar.gz` & `tmp/startorch-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "startorch-0.0.1a8.tar", max compression
+gzip compressed data, was "startorch-0.0.2.tar", max compression
```

## Comparing `startorch-0.0.1a8.tar` & `startorch-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,69 @@
--rw-r--r--   0        0        0     1501 2023-07-23 19:18:02.377494 startorch-0.0.1a8/LICENSE
--rw-r--r--   0        0        0       55 2023-07-23 19:18:02.377494 startorch-0.0.1a8/README.md
--rw-r--r--   0        0        0     4105 2023-07-23 19:18:02.377494 startorch-0.0.1a8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/__init__.py
--rw-r--r--   0        0        0     1473 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/random/__init__.py
--rw-r--r--   0        0        0    36850 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/random/bounded.py
--rw-r--r--   0        0        0     1460 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/random/discrete.py
--rw-r--r--   0        0        0     5984 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/random/infinite.py
--rw-r--r--   0        0        0    10653 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/random/semi_infinite.py
--rw-r--r--   0        0        0        0 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/utils/__init__.py
--rw-r--r--   0        0        0     1844 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/utils/seed.py
--rw-r--r--   0        0        0     1065 2023-07-23 19:18:02.377494 startorch-0.0.1a8/src/startorch/utils/tensor.py
--rw-r--r--   0        0        0     1122 1970-01-01 00:00:00.000000 startorch-0.0.1a8/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-08-05 04:34:53.637338 startorch-0.0.2/LICENSE
+-rw-r--r--   0        0        0     4479 2023-08-05 04:34:53.637338 startorch-0.0.2/README.md
+-rw-r--r--   0        0        0     4373 2023-08-05 04:34:53.705341 startorch-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/periodic/__init__.py
+-rw-r--r--   0        0        0      471 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/periodic/sequence/__init__.py
+-rw-r--r--   0        0        0     2373 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/periodic/sequence/base.py
+-rw-r--r--   0        0        0     1767 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/periodic/sequence/repeat.py
+-rw-r--r--   0        0        0     2486 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/periodic/sequence/wave.py
+-rw-r--r--   0        0        0     1473 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/random/__init__.py
+-rw-r--r--   0        0        0    36850 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/random/bounded.py
+-rw-r--r--   0        0        0     1460 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/random/discrete.py
+-rw-r--r--   0        0        0     5984 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/random/infinite.py
+-rw-r--r--   0        0        0    10653 2023-08-05 04:34:53.705341 startorch-0.0.2/src/startorch/random/semi_infinite.py
+-rw-r--r--   0        0        0     7201 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/__init__.py
+-rw-r--r--   0        0        0     4785 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/ar.py
+-rw-r--r--   0        0        0     2927 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/base.py
+-rw-r--r--   0        0        0     6464 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/categorical.py
+-rw-r--r--   0        0        0     9720 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/cauchy.py
+-rw-r--r--   0        0        0     2877 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/choice.py
+-rw-r--r--   0        0        0     2718 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/constant.py
+-rw-r--r--   0        0        0     1507 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/dtype.py
+-rw-r--r--   0        0        0    10761 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/exponential.py
+-rw-r--r--   0        0        0     7503 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/halfcauchy.py
+-rw-r--r--   0        0        0     7377 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/halfnormal.py
+-rw-r--r--   0        0        0     2643 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/joining.py
+-rw-r--r--   0        0        0     2594 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/linear.py
+-rw-r--r--   0        0        0    10014 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/lognormal.py
+-rw-r--r--   0        0        0    18785 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/math.py
+-rw-r--r--   0        0        0     9724 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/normal.py
+-rw-r--r--   0        0        0     2546 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/periodic.py
+-rw-r--r--   0        0        0     5030 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/poisson.py
+-rw-r--r--   0        0        0     1473 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/range.py
+-rw-r--r--   0        0        0     1506 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/sort.py
+-rw-r--r--   0        0        0     1890 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/tensor.py
+-rw-r--r--   0        0        0    11584 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/time.py
+-rw-r--r--   0        0        0     4568 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/trigo.py
+-rw-r--r--   0        0        0    13212 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/uniform.py
+-rw-r--r--   0        0        0     3285 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/wave.py
+-rw-r--r--   0        0        0     3116 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/wiener.py
+-rw-r--r--   0        0        0      814 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/sequence/wrapper.py
+-rw-r--r--   0        0        0     5793 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/__init__.py
+-rw-r--r--   0        0        0     2437 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/base.py
+-rw-r--r--   0        0        0     6154 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/categorical.py
+-rw-r--r--   0        0        0     8058 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/cauchy.py
+-rw-r--r--   0        0        0     2702 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/choice.py
+-rw-r--r--   0        0        0     1268 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/constant.py
+-rw-r--r--   0        0        0     1289 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/dtype.py
+-rw-r--r--   0        0        0     6091 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/exponential.py
+-rw-r--r--   0        0        0     6007 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/halfcauchy.py
+-rw-r--r--   0        0        0     5927 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/halfnormal.py
+-rw-r--r--   0        0        0     8300 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/lognormal.py
+-rw-r--r--   0        0        0    15559 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/math.py
+-rw-r--r--   0        0        0     8039 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/normal.py
+-rw-r--r--   0        0        0     2750 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/poisson.py
+-rw-r--r--   0        0        0     3773 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/trigo.py
+-rw-r--r--   0        0        0     9909 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/uniform.py
+-rw-r--r--   0        0        0      786 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/tensor/wrapper.py
+-rw-r--r--   0        0        0      254 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/testing.py
+-rw-r--r--   0        0        0        0 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/__init__.py
+-rw-r--r--   0        0        0     2248 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/batch.py
+-rw-r--r--   0        0        0      699 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/conversion.py
+-rw-r--r--   0        0        0     2244 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/format.py
+-rw-r--r--   0        0        0     1031 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/imports.py
+-rw-r--r--   0        0        0     4490 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/plot.py
+-rw-r--r--   0        0        0     1844 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/seed.py
+-rw-r--r--   0        0        0     1065 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/tensor.py
+-rw-r--r--   0        0        0     3285 2023-08-05 04:34:53.709342 startorch-0.0.2/src/startorch/utils/weight.py
+-rw-r--r--   0        0        0     5713 1970-01-01 00:00:00.000000 startorch-0.0.2/PKG-INFO
```

### Comparing `startorch-0.0.1a8/LICENSE` & `startorch-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/pyproject.toml` & `startorch-0.0.2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "startorch"
-version = "0.0.1a8"
+version = "0.0.2"
 description = "synthetic time-series generator in PyTorch"
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/startorch"
 repository = "https://github.com/durandtibo/startorch"
 keywords = ["synthetic", "time-series", "pytorch"]
 license = "BSD-3-Clause"
@@ -25,38 +25,50 @@
 
 packages = [
     { include = "startorch", from = "src" },
 ]
 
 [tool.poetry.dependencies]
 # Core dependencies
+coola = ">=0.0.18,<1.0"
+objectory = ">=0.0.6,<1.0"
 python = "^3.9"
-#redcat = ">=0.0.6,<1.0"
-torch = ">=1.10,<3.0"
+redcat = ">=0.0.7,<1.0"
+torch = ">=2.0,<3.0"
 
 # Optional dependencies
-
+matplotlib = { version = "^3.7", optional = true }
 
 [tool.poetry.extras]
-all = []
+all = ["matplotlib"]
+
+[tool.poetry.group.exp]
+optional = true
+
+[tool.poetry.group.exp.dependencies]
+jupyterlab = "^4.0"
+seaborn = "^0.12"
+
+[tool.poetry.group.docs]
+optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs-material = "^9.1"
 mkdocstrings = "^0.22"
 
 [tool.poetry.group.dev.dependencies]
 black = ">=23.7"
 coverage = { extras = ["toml"], version = "^7.2" }
 docformatter = { extras = ["tomli"], version = "^1.7" }
 pre-commit = "^3.3"
 pylint = "^2.17"
 pytest = "^7.4"
 pytest-cov = "^4.1"
 pytest-timeout = "^2.1"
-ruff = ">=0.0.280,<1.0"
+ruff = ">=0.0.282,<1.0"
 xdoctest = "^1.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.coverage.paths]
```

### Comparing `startorch-0.0.1a8/src/startorch/random/__init__.py` & `startorch-0.0.2/src/startorch/random/__init__.py`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/src/startorch/random/bounded.py` & `startorch-0.0.2/src/startorch/random/bounded.py`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/src/startorch/random/discrete.py` & `startorch-0.0.2/src/startorch/random/discrete.py`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/src/startorch/random/infinite.py` & `startorch-0.0.2/src/startorch/random/infinite.py`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/src/startorch/random/semi_infinite.py` & `startorch-0.0.2/src/startorch/random/semi_infinite.py`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/src/startorch/utils/seed.py` & `startorch-0.0.2/src/startorch/utils/seed.py`

 * *Files identical despite different names*

### Comparing `startorch-0.0.1a8/src/startorch/utils/tensor.py` & `startorch-0.0.2/src/startorch/utils/tensor.py`

 * *Files identical despite different names*

