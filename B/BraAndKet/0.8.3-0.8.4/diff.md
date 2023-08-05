# Comparing `tmp/BraAndKet-0.8.3.tar.gz` & `tmp/BraAndKet-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BraAndKet-0.8.3.tar", last modified: Fri Jul 28 03:27:24 2023, max compression
+gzip compressed data, was "BraAndKet-0.8.4.tar", last modified: Sat Aug  5 14:50:18 2023, max compression
```

## Comparing `BraAndKet-0.8.3.tar` & `BraAndKet-0.8.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.431944 BraAndKet-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-28 03:27:24.431944 BraAndKet-0.8.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.423944 BraAndKet-0.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/BraAndKet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-28 03:27:24.000000 BraAndKet-0.8.3/src/BraAndKet.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     7094 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8516 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/backend/tensorflow_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/model/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/model/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/space/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/hilbert_space.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/num_space.py
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/space/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6608 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)    11169 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/special.py
--rw-r--r--   0 runner    (1001) docker     (123)    14023 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/tensor/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-28 03:27:24.427944 BraAndKet-0.8.3/src/braandket/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-28 03:27:10.000000 BraAndKet-0.8.3/src/braandket/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.112951 BraAndKet-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-05 14:50:18.112951 BraAndKet-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 14:50:18.112951 BraAndKet-0.8.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.108951 BraAndKet-0.8.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.108951 BraAndKet-0.8.4/src/BraAndKet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-08-05 14:50:18.000000 BraAndKet-0.8.4/src/BraAndKet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-08-05 14:50:18.000000 BraAndKet-0.8.4/src/BraAndKet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:50:18.000000 BraAndKet-0.8.4/src/BraAndKet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-08-05 14:50:18.000000 BraAndKet-0.8.4/src/BraAndKet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-05 14:50:18.000000 BraAndKet-0.8.4/src/BraAndKet.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.108951 BraAndKet-0.8.4/src/braandket/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.108951 BraAndKet-0.8.4/src/braandket/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3886 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/backend/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/backend/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/backend/numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9533 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/backend/tensorflow_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.108951 BraAndKet-0.8.4/src/braandket/model/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3769 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/model/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.108951 BraAndKet-0.8.4/src/braandket/space/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/space/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/space/hilbert_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/space/num_space.py
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/space/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.112951 BraAndKet-0.8.4/src/braandket/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6614 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/tensor/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11193 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/tensor/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14041 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/tensor/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:50:18.112951 BraAndKet-0.8.4/src/braandket/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-08-05 14:49:59.000000 BraAndKet-0.8.4/src/braandket/utils/utils.py
```

### Comparing `BraAndKet-0.8.3/LICENSE` & `BraAndKet-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/PKG-INFO` & `BraAndKet-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BraAndKet
-Version: 0.8.3
+Version: 0.8.4
 Summary: BraAndKet is a library for numeral calculations of discrete quantum systems.
 Author-email: Zheng Keli <zhengkeli2009@126.com>
 Project-URL: repository, https://github.com/ZhengKeli/BraAndKet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `BraAndKet-0.8.3/README.md` & `BraAndKet-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/pyproject.toml` & `BraAndKet-0.8.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "BraAndKet"
-version = "0.8.3"
+version = "0.8.4"
 
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 description = "BraAndKet is a library for numeral calculations of discrete quantum systems."
```

### Comparing `BraAndKet-0.8.3/src/BraAndKet.egg-info/PKG-INFO` & `BraAndKet-0.8.4/src/BraAndKet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BraAndKet
-Version: 0.8.3
+Version: 0.8.4
 Summary: BraAndKet is a library for numeral calculations of discrete quantum systems.
 Author-email: Zheng Keli <zhengkeli2009@126.com>
 Project-URL: repository, https://github.com/ZhengKeli/BraAndKet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
```

### Comparing `BraAndKet-0.8.3/src/BraAndKet.egg-info/SOURCES.txt` & `BraAndKet-0.8.4/src/BraAndKet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/src/braandket/backend/backend.py` & `BraAndKet-0.8.4/src/braandket/backend/backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,144 +1,147 @@
 import abc
 from typing import Any, Generic, Iterable, Optional, TypeVar, Union
 
-ValuesType = TypeVar('ValuesType')
+import numpy as np
 
+BackendValue = TypeVar('BackendValue')
+ArrayLike = Union[BackendValue, np.ndarray, Iterable, bool, int, float, complex, Any]
 
-class Backend(Generic[ValuesType], abc.ABC):
+
+class Backend(Generic[BackendValue], abc.ABC):
 
     def __enter__(self):
         from .default import push_context_backend
         push_context_backend(self)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         from .default import pop_context_backend
         pop_context_backend()
 
     # basics
 
     @abc.abstractmethod
-    def convert(self, values: Any) -> ValuesType:
+    def convert(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def copy(self, values: ValuesType) -> ValuesType:
+    def copy(self, value: ArrayLike) -> BackendValue:
         pass
 
     # constructors
 
     @abc.abstractmethod
-    def zeros(self, shape: Iterable[int]) -> ValuesType:
+    def zeros(self, shape: Iterable[int]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def ones(self, shape: Iterable[int]) -> ValuesType:
+    def ones(self, shape: Iterable[int]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def onehot(self, index: int, size: int) -> ValuesType:
+    def onehot(self, index: int, size: int) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def eye(self, size: int) -> ValuesType:
+    def eye(self, size: int) -> BackendValue:
         pass
 
     # linear operations
 
     @abc.abstractmethod
-    def add(self, values0: ValuesType, values1: ValuesType) -> ValuesType:
+    def add(self, value0: ArrayLike, value1: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def sub(self, values0: ValuesType, values1: ValuesType) -> ValuesType:
+    def sub(self, value0: ArrayLike, value1: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def mul(self, values0: ValuesType, values1: ValuesType) -> ValuesType:
+    def mul(self, value0: ArrayLike, value1: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def div(self, values0: ValuesType, values1: ValuesType) -> ValuesType:
+    def div(self, value0: ArrayLike, value1: ArrayLike) -> BackendValue:
         pass
 
     # non-linear operations
 
     @abc.abstractmethod
-    def pow(self, values0: ValuesType, values1: ValuesType) -> ValuesType:
+    def pow(self, value0: ArrayLike, value1: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def square(self, values: ValuesType) -> ValuesType:
+    def square(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def sqrt(self, values: ValuesType) -> ValuesType:
+    def sqrt(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def exp(self, values: ValuesType) -> ValuesType:
+    def exp(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def sin(self, values: ValuesType) -> ValuesType:
+    def sin(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def cos(self, values: ValuesType) -> ValuesType:
+    def cos(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def conj(self, values: ValuesType) -> ValuesType:
+    def conj(self, value: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def abs(self, values: ValuesType) -> ValuesType:
+    def abs(self, value: ArrayLike) -> BackendValue:
         pass
 
     # tensor operations
 
     @abc.abstractmethod
-    def ensure_shape(self, values: ValuesType, shape: Iterable[int]) -> ValuesType:
+    def ensure_shape(self, value: ArrayLike, shape: Iterable[int]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def reshape(self, values: ValuesType, shape: Iterable[int]) -> ValuesType:
+    def reshape(self, value: ArrayLike, shape: Iterable[int]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def transpose(self, values: ValuesType, *, axes: Iterable[int]) -> ValuesType:
+    def transpose(self, value: ArrayLike, *, axes: Iterable[int]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def expand(self, values: ValuesType, axes: Iterable[int], sizes: Optional[Iterable[int]] = None) -> ValuesType:
+    def expand(self, value: ArrayLike, axes: Iterable[int], sizes: Optional[Iterable[int]] = None) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def slice(self, values: ValuesType, *, slices: Union[int, slice, Iterable[Union[int, slice]]]) -> ValuesType:
+    def slice(self, value: ArrayLike, *, slices: Union[int, slice, Iterable[Union[int, slice]]]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def trace(self, values: ValuesType, axes: tuple[Iterable[int], Iterable[int]]) -> ValuesType:
+    def trace(self, value: ArrayLike, axes: tuple[Iterable[int], Iterable[int]]) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def diag(self, values: ValuesType, axes: tuple[Iterable[int], Iterable[int]]) -> ValuesType:
+    def diag(self, value: ArrayLike, axes: tuple[Iterable[int], Iterable[int]]) -> BackendValue:
         pass
 
     @abc.abstractmethod
     def dot(self,
-        values0: ValuesType, values1: ValuesType, *,
+        value0: ArrayLike, value1: ArrayLike, *,
         ndim0: int, ndim1: int,
         dot_axes: tuple[Iterable[int], Iterable[int]],
         bat_axes: tuple[Iterable[int], Iterable[int]],
-    ) -> tuple[ValuesType, tuple[tuple[int, ...], tuple[int, ...]]]:
+    ) -> tuple[BackendValue, tuple[tuple[int, ...], tuple[int, ...]]]:
         pass
 
     # special
 
     @abc.abstractmethod
-    def take(self, values: Iterable[ValuesType], indices: ValuesType) -> ValuesType:
+    def take(self, values: Iterable[ArrayLike], indices: ArrayLike) -> BackendValue:
         pass
 
     @abc.abstractmethod
-    def choose(self, probs: Iterable[ValuesType]) -> ValuesType:
+    def choose(self, probs: Iterable[ArrayLike]) -> BackendValue:
         pass
```

### Comparing `BraAndKet-0.8.3/src/braandket/backend/default.py` & `BraAndKet-0.8.4/src/braandket/backend/default.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/src/braandket/backend/numpy_backend.py` & `BraAndKet-0.8.4/src/braandket/backend/numpy_backend.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,127 +1,127 @@
-from typing import Any, Iterable, Optional, Union
+from typing import Iterable, Optional, Union
 
 import numpy as np
 
-from .backend import Backend, ValuesType
+from .backend import ArrayLike, Backend
 
 
 class NumpyBackend(Backend[np.ndarray]):
 
     # basics
 
-    def convert(self, values: Any, *, dtype=None) -> np.ndarray:
-        return np.asarray(values, dtype=dtype)
+    def convert(self, value: ArrayLike, *, dtype=None) -> np.ndarray:
+        return np.asarray(value, dtype=dtype)
 
-    def copy(self, values: np.ndarray) -> np.ndarray:
-        return np.copy(values)
+    def copy(self, value: ArrayLike) -> np.ndarray:
+        return np.copy(value)
 
     # constructors
 
     def zeros(self, shape: Iterable[int], *, dtype=np.float32) -> np.ndarray:
         return np.zeros(shape, dtype=dtype)
 
     def ones(self, shape: Iterable[int], *, dtype=np.float32) -> np.ndarray:
         return np.ones(shape, dtype=dtype)
 
     def onehot(self, index: int, size: int, *, dtype=np.float32) -> np.ndarray:
-        values = np.zeros(size, dtype=dtype)
-        values[index] = 1.0
-        return values
+        value = np.zeros(size, dtype=dtype)
+        value[index] = 1.0
+        return value
 
     def eye(self, size: int, *, dtype=np.float32) -> np.ndarray:
         return np.eye(size, dtype=dtype)
 
     # unary operations
 
-    def pow(self, values0: np.ndarray, values1: np.ndarray) -> np.ndarray:
-        return np.power(values0, values1)
+    def pow(self, value0: ArrayLike, value1: ArrayLike) -> np.ndarray:
+        return np.power(value0, value1)
 
-    def square(self, values: np.ndarray) -> np.ndarray:
-        return np.square(values)
+    def square(self, value: ArrayLike) -> np.ndarray:
+        return np.square(value)
 
-    def sqrt(self, values: np.ndarray) -> np.ndarray:
-        return np.sqrt(values)
+    def sqrt(self, value: ArrayLike) -> np.ndarray:
+        return np.sqrt(value)
 
-    def exp(self, values: np.ndarray) -> np.ndarray:
-        return np.exp(values)
+    def exp(self, value: ArrayLike) -> np.ndarray:
+        return np.exp(value)
 
-    def sin(self, values: np.ndarray) -> np.ndarray:
-        return np.sin(values)
+    def sin(self, value: ArrayLike) -> np.ndarray:
+        return np.sin(value)
 
-    def cos(self, values: np.ndarray) -> np.ndarray:
-        return np.cos(values)
+    def cos(self, value: ArrayLike) -> np.ndarray:
+        return np.cos(value)
 
-    def conj(self, values: np.ndarray) -> np.ndarray:
-        return np.conj(values)
+    def conj(self, value: ArrayLike) -> np.ndarray:
+        return np.conj(value)
 
-    def abs(self, values: np.ndarray) -> np.ndarray:
-        return np.abs(values)
+    def abs(self, value: ArrayLike) -> np.ndarray:
+        return np.abs(value)
 
     # linear operations
 
-    def add(self, values0: np.ndarray, values1: np.ndarray) -> np.ndarray:
-        return values0 + values1
+    def add(self, value0: ArrayLike, value1: ArrayLike) -> np.ndarray:
+        return value0 + value1
 
-    def sub(self, values0: np.ndarray, values1: np.ndarray) -> np.ndarray:
-        return values0 - values1
+    def sub(self, value0: ArrayLike, value1: ArrayLike) -> np.ndarray:
+        return value0 - value1
 
-    def mul(self, values0: np.ndarray, values1: np.ndarray) -> np.ndarray:
-        return values0 * values1
+    def mul(self, value0: ArrayLike, value1: ArrayLike) -> np.ndarray:
+        return value0 * value1
 
-    def div(self, values0: np.ndarray, values1: np.ndarray) -> np.ndarray:
-        return values0 / values1
+    def div(self, value0: ArrayLike, value1: ArrayLike) -> np.ndarray:
+        return value0 / value1
 
     # tensor operations
 
-    def ensure_shape(self, values: np.ndarray, shape: Iterable[int]):
-        if np.shape(values) != tuple(shape):
-            raise ValueError(f"Unexpected values shape! expected={shape}, actual={np.shape(values)}")
-        return values
+    def ensure_shape(self, value: ArrayLike, shape: Iterable[int]):
+        if np.shape(value) != tuple(shape):
+            raise ValueError(f"Unexpected value shape! expected={shape}, actual={np.shape(value)}")
+        return value
 
-    def reshape(self, values: np.ndarray, shape: Iterable[int]) -> np.ndarray:
-        return np.reshape(values, shape)
+    def reshape(self, value: ArrayLike, shape: Iterable[int]) -> np.ndarray:
+        return np.reshape(value, shape)
 
-    def transpose(self, values: np.ndarray, *, axes: Iterable[int]) -> np.ndarray:
-        return np.transpose(values, axes)
+    def transpose(self, value: ArrayLike, *, axes: Iterable[int]) -> np.ndarray:
+        return np.transpose(value, axes)
 
-    def expand(self, values: np.ndarray, axes: Iterable[int], sizes: Optional[Iterable[int]] = None) -> np.ndarray:
+    def expand(self, value: ArrayLike, axes: Iterable[int], sizes: Optional[Iterable[int]] = None) -> np.ndarray:
         axes = tuple(axes)
-        values = np.expand_dims(values, axes)
+        value = np.expand_dims(value, axes)
         if sizes is not None:
             sizes = tuple(sizes)
             for axis, size in zip(axes, sizes, strict=True):
-                values = np.repeat(values, size, axis)
-        return values
+                value = np.repeat(value, size, axis)
+        return value
 
-    def slice(self, values: np.ndarray, *, slices: Union[int, slice, Iterable[Union[int, slice]]]) -> np.ndarray:
-        return values[slices]
+    def slice(self, value: ArrayLike, *, slices: Union[int, slice, Iterable[Union[int, slice]]]) -> np.ndarray:
+        return value[slices]
 
-    def trace(self, values: np.ndarray, axes: tuple[Iterable[int], Iterable[int]]) -> np.ndarray:
+    def trace(self, value: ArrayLike, axes: tuple[Iterable[int], Iterable[int]]) -> np.ndarray:
         axis_pairs = np.transpose(axes)  # [axes_n, 2]
         while len(axes) > 0:
             axis0, axis1 = axis_pairs[0]
-            values = np.trace(values, axis0, axis1)
+            value = np.trace(value, axis0, axis1)
             axis_pairs = axis_pairs[1:]
             axis_pairs = np.where(axis_pairs > axis0, axis_pairs - 1, axis_pairs)
             axis_pairs = np.where(axis_pairs > axis1, axis_pairs - 1, axis_pairs)
-        return values
+        return value
 
-    def diag(self, values: np.ndarray, axes: tuple[Iterable[int], Iterable[int]]) -> np.ndarray:
+    def diag(self, value: ArrayLike, axes: tuple[Iterable[int], Iterable[int]]) -> np.ndarray:
         axis_pairs = np.transpose(axes)  # [axes_n, 2]
         while len(axes) > 0:
             axis0, axis1 = axis_pairs[0]
-            values = np.diagonal(values, axis0, axis1)
+            value = np.diagonal(value, axis0, axis1)
             axis_pairs = axis_pairs[1:]
             axis_pairs = np.where(axis_pairs > axis0, axis_pairs - 1, axis_pairs)
             axis_pairs = np.where(axis_pairs > axis1, axis_pairs - 1, axis_pairs)
-        return values
+        return value
 
     def dot(self,
-        values0: np.ndarray, values1: np.ndarray, *,
+        value0: ArrayLike, value1: ArrayLike, *,
         ndim0: int, ndim1: int,
         dot_axes: tuple[Iterable[int], Iterable[int]],
         bat_axes: tuple[Iterable[int], Iterable[int]],
     ) -> tuple[np.ndarray, tuple[tuple[int, ...], tuple[int, ...]]]:
         bat_axes0, bat_axes1 = tuple(bat_axes[0]), tuple(bat_axes[1])
         if not len(bat_axes0) == len(bat_axes1):
             raise ValueError("len(bat_axes[0]) != len(bat_axes[1])")
@@ -130,52 +130,52 @@
         dot_axes0, dot_axes1 = tuple(dot_axes[0]), tuple(dot_axes[1])
         if not len(dot_axes0) == len(dot_axes1):
             raise ValueError("len(dot_axes[0]) != len(dot_axes[1])")
         del dot_axes
 
         selected_axes0 = {*bat_axes0, *dot_axes0}
         if len(selected_axes0) != len(bat_axes0) + len(dot_axes0):
-            raise ValueError("Found duplication for axes of values0 !")
+            raise ValueError("Found duplication for axes of value0 !")
         rem_axes0 = tuple(axis for axis in range(ndim0) if axis not in selected_axes0)
 
         selected_axes1 = {*bat_axes1, *dot_axes1}
         if len(selected_axes1) != len(bat_axes1) + len(dot_axes1):
-            raise ValueError("Found duplication for axes of values1 !")
+            raise ValueError("Found duplication for axes of value1 !")
         rem_axes1 = tuple(axis for axis in range(ndim1) if axis not in selected_axes1)
 
-        values0 = np.transpose(values0, [*bat_axes0, *rem_axes0, *dot_axes0])
-        values1 = np.transpose(values1, [*bat_axes1, *rem_axes1, *dot_axes1])
+        value0 = np.transpose(value0, [*bat_axes0, *rem_axes0, *dot_axes0])
+        value1 = np.transpose(value1, [*bat_axes1, *rem_axes1, *dot_axes1])
         # [*bat_axes, *rem_axes, *dot_axes]
 
         bat_axes_n, dot_axes_n = len(bat_axes0), len(dot_axes0)
         rem_axes0_n, rem_axes1_n = len(rem_axes0), len(rem_axes1)
 
-        values0 = np.expand_dims(values0, axis=tuple(bat_axes_n + rem_axes0_n + np.arange(rem_axes1_n)))
-        values1 = np.expand_dims(values1, axis=tuple(bat_axes_n + np.arange(rem_axes0_n)))
+        value0 = np.expand_dims(value0, axis=tuple(bat_axes_n + rem_axes0_n + np.arange(rem_axes1_n)))
+        value1 = np.expand_dims(value1, axis=tuple(bat_axes_n + np.arange(rem_axes0_n)))
         # [*bat_axes, *rem_axes0, *exp_axes0, *dot_axes]
         # [*bat_axes, *exp_axes1, *rem_axes1, *dot_axes]
 
-        values = values0 * values1
+        value = value0 * value1
         # [*bat_axes, *rem_axes0, *rem_axes1, *dot_axes]
 
-        values = np.sum(values, axis=tuple(bat_axes_n + rem_axes0_n + rem_axes1_n + np.arange(dot_axes_n)))
+        value = np.sum(value, axis=tuple(bat_axes_n + rem_axes0_n + rem_axes1_n + np.arange(dot_axes_n)))
         # [*bat_axes, *rem_axes0, *rem_axes1]
 
-        return values, (rem_axes0, rem_axes1)
+        return value, (rem_axes0, rem_axes1)
 
     # special
 
-    def take(self, values: Iterable[ValuesType], indices: np.ndarray) -> np.ndarray:
+    def take(self, values: Iterable[ArrayLike], indices: ArrayLike) -> np.ndarray:
         values = np.stack(values, axis=-1)
         indices = np.expand_dims(indices, axis=-1)
-        values = np.take_along_axis(values, indices, axis=-1)
-        values = np.squeeze(values, axis=-1)
-        return values
+        value = np.take_along_axis(values, indices, axis=-1)
+        value = np.squeeze(value, axis=-1)
+        return value
 
-    def choose(self, probs: Iterable[ValuesType]) -> tuple[np.ndarray, np.ndarray]:
+    def choose(self, probs: Iterable[ArrayLike]) -> tuple[np.ndarray, np.ndarray]:
         probs = np.stack(probs, axis=-1)  # [batch_size, choose_n]
         probs /= np.sum(probs, axis=-1, keepdims=True)
         probs = np.abs(probs)
         choice = np.apply_along_axis(lambda p: np.random.choice(len(p), p=p), axis=-1, arr=probs)  # [batch_size]
         return choice
```

### Comparing `BraAndKet-0.8.3/src/braandket/backend/tensorflow_backend.py` & `BraAndKet-0.8.4/src/braandket/backend/tensorflow_backend.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,209 +1,245 @@
-from typing import Any, Iterable, Optional, Union
+from typing import Iterable, Optional, Union
 
+import numpy as np
 import tensorflow as tf
 
-from .backend import Backend
+from .backend import ArrayLike, Backend
 
 
 class TensorflowBackend(Backend[tf.Tensor]):
 
     # basics
 
-    def convert(self, values: Any, *, dtype=None) -> tf.Tensor:
-        values = tf.convert_to_tensor(values)
-        if dtype is not None:
-            values = tf.cast(values, dtype=dtype)
-        elif values.dtype in (tf.int8, tf.int16, tf.int32, tf.int64):
-            values = tf.cast(values, dtype=tf.int32)
-        elif values.dtype in (tf.float16, tf.float32, tf.float64):
-            values = tf.cast(values, dtype=tf.float32)
-        elif values.dtype in (tf.complex64, tf.complex128):
-            values = tf.cast(values, dtype=tf.complex64)
-        else:
-            raise TypeError(f"Unsupported dtype of values: {values.dtype}")
-        return values
-
-    def copy(self, values: tf.Tensor) -> tf.Tensor:
-        return values
-
-    def _auto_cast(self, values0: tf.Tensor, values1: tf.Tensor) -> tuple[tf.Tensor, tf.Tensor]:
-        ordered_dtypes = [tf.complex64, tf.float32, tf.int32]
-        dt0 = ordered_dtypes.index(values0.dtype)
-        dt1 = ordered_dtypes.index(values1.dtype)
-        dtype = ordered_dtypes[dt0] if dt0 < dt1 else ordered_dtypes[dt1]
-        values0 = tf.cast(values0, dtype=dtype)
-        values1 = tf.cast(values1, dtype=dtype)
-        return values0, values1
+    def convert(self, value: ArrayLike, *values: ArrayLike) -> Union[tf.Tensor, tuple[tf.Tensor, ...]]:
+        value = tf.convert_to_tensor(value)
+        if not values:
+            return value
+
+        values = tuple(tf.convert_to_tensor(v) for v in values)
+        dtype = get_compact_dtype(value.dtype, *(v.dtype for v in values))
+
+        value = tf.cast(value, dtype)
+        values = tuple(tf.cast(v, dtype) for v in values)
+        return value, *values
+
+    def copy(self, values: ArrayLike) -> tf.Tensor:
+        return self.convert(values)
 
     # constructors
 
-    def zeros(self, shape: Iterable[int], *, dtype=tf.complex64) -> tf.Tensor:
+    def zeros(self, shape: Iterable[int], *, dtype=tf.float32) -> tf.Tensor:
         return tf.zeros(shape, dtype=dtype)
 
-    def ones(self, shape: Iterable[int], *, dtype=tf.complex64) -> tf.Tensor:
+    def ones(self, shape: Iterable[int], *, dtype=tf.float32) -> tf.Tensor:
         return tf.ones(shape, dtype=dtype)
 
-    def onehot(self, index: int, size: int, *, dtype=tf.complex64) -> tf.Tensor:
+    def onehot(self, index: int, size: int, *, dtype=tf.float32) -> tf.Tensor:
         one_value = tf.ones((), dtype=dtype)
         zero_value = tf.zeros((), dtype=dtype)
         return tf.one_hot(index, size, on_value=one_value, off_value=zero_value)
 
-    def eye(self, size: int, *, dtype=tf.complex64) -> tf.Tensor:
+    def eye(self, size: int, *, dtype=tf.float32) -> tf.Tensor:
         return tf.eye(size, dtype=dtype)
 
     # unary operations
 
-    def pow(self, values0: tf.Tensor, values1: tf.Tensor) -> tf.Tensor:
-        return tf.pow(values0, values1)
-
-    def square(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.square(values)
-
-    def sqrt(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.sqrt(values)
-
-    def exp(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.exp(values)
-
-    def sin(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.sin(values)
-
-    def cos(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.cos(values)
-
-    def conj(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.math.conj(values)
-
-    def abs(self, values: tf.Tensor) -> tf.Tensor:
-        return tf.abs(values)
+    def pow(self, value0: ArrayLike, value1: ArrayLike) -> tf.Tensor:
+        value0, value1 = self.convert(value0, value1)
+        return tf.pow(value0, value1)
+
+    def square(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.square(value)
+
+    def sqrt(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.sqrt(value)
+
+    def exp(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.exp(value)
+
+    def sin(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.sin(value)
+
+    def cos(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.cos(value)
+
+    def conj(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.math.conj(value)
+
+    def abs(self, value: ArrayLike) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.abs(value)
 
     # linear operations
 
-    def add(self, values0: tf.Tensor, values1: tf.Tensor) -> tf.Tensor:
-        values0, values1 = self._auto_cast(values0, values1)
-        return values0 + values1
-
-    def sub(self, values0: tf.Tensor, values1: tf.Tensor) -> tf.Tensor:
-        values0, values1 = self._auto_cast(values0, values1)
-        return values0 - values1
-
-    def mul(self, values0: tf.Tensor, values1: tf.Tensor) -> tf.Tensor:
-        values0, values1 = self._auto_cast(values0, values1)
-        return values0 * values1
-
-    def div(self, values0: tf.Tensor, values1: tf.Tensor) -> tf.Tensor:
-        values0, values1 = self._auto_cast(values0, values1)
-        return values0 / values1
+    def add(self, value0: ArrayLike, value1: ArrayLike) -> tf.Tensor:
+        value0, value1 = self.convert(value0, value1)
+        return value0 + value1
+
+    def sub(self, value0: ArrayLike, value1: ArrayLike) -> tf.Tensor:
+        value0, value1 = self.convert(value0, value1)
+        return value0 - value1
+
+    def mul(self, value0: ArrayLike, value1: ArrayLike) -> tf.Tensor:
+        value0, value1 = self.convert(value0, value1)
+        return value0 * value1
+
+    def div(self, value0: ArrayLike, value1: ArrayLike) -> tf.Tensor:
+        value0, value1 = self.convert(value0, value1)
+        return value0 / value1
 
     # operator operations
 
-    def ensure_shape(self, values: tf.Tensor, shape: Iterable[int]) -> tf.Tensor:
-        return tf.ensure_shape(values, shape)
-
-    def reshape(self, values: tf.Tensor, shape: Iterable[int]) -> tf.Tensor:
-        return tf.reshape(values, shape)
-
-    def transpose(self, values: tf.Tensor, *, axes: Iterable[int]) -> tf.Tensor:
-        return tf.transpose(values, axes)
+    def ensure_shape(self, value: ArrayLike, shape: Iterable[int]) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.ensure_shape(value, shape)
+
+    def reshape(self, value: ArrayLike, shape: Iterable[int]) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.reshape(value, shape)
+
+    def transpose(self, value: ArrayLike, *, axes: Iterable[int]) -> tf.Tensor:
+        value = self.convert(value)
+        return tf.transpose(value, axes)
 
-    def expand(self, values: tf.Tensor, axes: Iterable[int], sizes: Optional[Iterable[int]] = None) -> tf.Tensor:
+    def expand(self, value: ArrayLike, axes: Iterable[int], sizes: Optional[Iterable[int]] = None) -> tf.Tensor:
+        value = self.convert(value)
         for axis in axes:
-            values = tf.expand_dims(values, axis)
+            value = tf.expand_dims(value, axis)
         if sizes is not None:
             sizes = tuple(sizes)
             for axis, size in zip(axes, sizes, strict=True):
-                values = tf.repeat(values, size, axis)
-        return values
+                value = tf.repeat(value, size, axis)
+        return value
 
-    def slice(self, values: tf.Tensor, *, slices: Union[int, slice, Iterable[Union[int, slice]]]) -> tf.Tensor:
-        return values[slices]
+    def slice(self, value: ArrayLike, *, slices: Union[int, slice, Iterable[Union[int, slice]]]) -> tf.Tensor:
+        value = self.convert(value)
+        return value[slices]
 
-    def trace(self, values: tf.Tensor, axes: tuple[Iterable[int], Iterable[int]]) -> tf.Tensor:
+    def trace(self, value: ArrayLike, axes: tuple[Iterable[int], Iterable[int]]) -> tf.Tensor:
+        value = self.convert(value)
         axis_pairs = tf.transpose(axes)  # [axes_n, 2]
         while len(axes) > 0:
             axis0, axis1 = axis_pairs[0]
-            values = tf.linalg.trace(values, axis0, axis1)
+            value = tf.linalg.trace(value, axis0, axis1)
             axis_pairs = axis_pairs[1:]
             axis_pairs = tf.where(axis_pairs > axis0, axis_pairs - 1, axis_pairs)
             axis_pairs = tf.where(axis_pairs > axis1, axis_pairs - 1, axis_pairs)
-        return values
+        return value
 
-    def diag(self, values: tf.Tensor, axes: tuple[Iterable[int], Iterable[int]]) -> tf.Tensor:
+    def diag(self, value: ArrayLike, axes: tuple[Iterable[int], Iterable[int]]) -> tf.Tensor:
+        value = self.convert(value)
         axis_pairs = tf.transpose(axes)  # [axes_n, 2]
         while len(axes) > 0:
             axis0, axis1 = axis_pairs[0]
-            values = tf.linalg.diag(values, axis0, axis1)
+            value = tf.linalg.diag(value, axis0, axis1)
             axis_pairs = axis_pairs[1:]
             axis_pairs = tf.where(axis_pairs > axis0, axis_pairs - 1, axis_pairs)
             axis_pairs = tf.where(axis_pairs > axis1, axis_pairs - 1, axis_pairs)
-        return values
+        return value
 
     def dot(self,
-        values0: tf.Tensor, values1: tf.Tensor, *,
+        value0: ArrayLike, value1: ArrayLike, *,
         ndim0: int, ndim1: int,
         dot_axes: tuple[Iterable[int], Iterable[int]],
         bat_axes: tuple[Iterable[int], Iterable[int]],
     ) -> tuple[tf.Tensor, tuple[tuple[int, ...], tuple[int, ...]]]:
+        value0, value1 = self.convert(value0, value1)
+
         bat_axes0, bat_axes1 = tuple(bat_axes[0]), tuple(bat_axes[1])
         if not len(bat_axes0) == len(bat_axes1):
             raise ValueError("len(bat_axes[0]) != len(bat_axes[1])")
         del bat_axes
 
         dot_axes0, dot_axes1 = tuple(dot_axes[0]), tuple(dot_axes[1])
         if not len(dot_axes0) == len(dot_axes1):
             raise ValueError("len(dot_axes[0]) != len(dot_axes[1])")
         del dot_axes
 
         selected_axes0 = {*bat_axes0, *dot_axes0}
         if len(selected_axes0) != len(bat_axes0) + len(dot_axes0):
-            raise ValueError("Found duplication for axes of values0 !")
+            raise ValueError("Found duplication for axes of value0 !")
         rem_axes0 = tuple(axis for axis in range(ndim0) if axis not in selected_axes0)
 
         selected_axes1 = {*bat_axes1, *dot_axes1}
         if len(selected_axes1) != len(bat_axes1) + len(dot_axes1):
-            raise ValueError("Found duplication for axes of values1 !")
+            raise ValueError("Found duplication for axes of value1 !")
         rem_axes1 = tuple(axis for axis in range(ndim1) if axis not in selected_axes1)
 
-        values0 = tf.transpose(values0, [*bat_axes0, *rem_axes0, *dot_axes0])
-        values1 = tf.transpose(values1, [*bat_axes1, *rem_axes1, *dot_axes1])
+        value0 = tf.transpose(value0, [*bat_axes0, *rem_axes0, *dot_axes0])
+        value1 = tf.transpose(value1, [*bat_axes1, *rem_axes1, *dot_axes1])
 
         bat_axes_n, dot_axes_n = len(bat_axes0), len(dot_axes0)
         rem_axes0_n, rem_axes1_n = len(rem_axes0), len(rem_axes1)
 
-        values0 = self.expand(values0, tuple((i + bat_axes_n + rem_axes0_n) for i in range(rem_axes1_n)))
-        values1 = self.expand(values1, tuple((i + bat_axes_n) for i in range(rem_axes0_n)))
+        value0 = self.expand(value0, tuple((i + bat_axes_n + rem_axes0_n) for i in range(rem_axes1_n)))
+        value1 = self.expand(value1, tuple((i + bat_axes_n) for i in range(rem_axes0_n)))
         # [*bat_axes, *rem_axes0, *exp_axes0, *dot_axes]
         # [*bat_axes, *exp_axes1, *rem_axes1, *dot_axes]
 
-        values = self.mul(values0, values1)
+        value = self.mul(value0, value1)
         # [*bat_axes, *rem_axes0, *rem_axes1, *dot_axes]
 
-        values = tf.reduce_sum(values, tuple((i + bat_axes_n + rem_axes0_n + rem_axes1_n) for i in range(dot_axes_n)))
+        value = tf.reduce_sum(value, tuple((i + bat_axes_n + rem_axes0_n + rem_axes1_n) for i in range(dot_axes_n)))
         # [*bat_axes, *rem_axes0, *rem_axes1]
 
-        return values, (rem_axes0, rem_axes1)
+        return value, (rem_axes0, rem_axes1)
 
     # special
 
-    def take(self, values: Iterable[tf.Tensor], indices: tf.Tensor) -> tf.Tensor:
+    def take(self, values: Iterable[ArrayLike], indices: ArrayLike) -> tf.Tensor:
+        values = self.convert(values) if isinstance(values, (np.ndarray, tf.Tensor)) else self.convert(*values)
         values = tf.stack(values, axis=-1)
         indices = tf.expand_dims(indices, axis=-1)
         indices = tf.cast(indices, tf.int32)
-        values = tf.experimental.numpy.take_along_axis(values, indices, axis=-1)
-        values = tf.squeeze(values, axis=-1)
-        return values
+        value = tf.experimental.numpy.take_along_axis(values, indices, axis=-1)
+        value = tf.squeeze(value, axis=-1)
+        return value
 
-    def choose(self, probs: Iterable[tf.Tensor]) -> tf.Tensor:
+    def choose(self, probs: Iterable[ArrayLike]) -> tf.Tensor:
+        probs = self.convert(probs) if isinstance(probs, (np.ndarray, tf.Tensor)) else self.convert(*probs)
         probs = tf.stack(probs, axis=-1)  # [*batch_shape, choose_n]
         batch_shape = tf.shape(probs)[:-1]
         batch_size = tf.reduce_prod(batch_shape)
         probs = tf.reshape(probs, [batch_size, -1])  # [batch_size, choose_n]
         logits = tf.math.abs(tf.math.log(probs))
 
         choice = tf.random.categorical(logits, 1)  # [batch_size, 1]
         choice = choice[:, 0]  # [batch_size]
         choice = tf.reshape(choice, batch_shape)  # [*batch_shape]
         return choice
 
 
 tensorflow_backend = TensorflowBackend()
+
+# utils
+
+_grouped_dtypes = (
+    (tf.bool,),
+    (None, tf.int8, tf.int16, tf.int32, tf.int64),
+    (None, None, tf.float16, tf.float32, tf.float64),
+    (None, None, None, tf.complex64, tf.complex128))
+
+_supported_dtypes = tuple(dt for gp in _grouped_dtypes for dt in gp if dt is not None)
+
+
+def get_dtype_indices(dtype: tf.DType) -> tuple[int, int]:
+    for group_i, group in enumerate(_grouped_dtypes):
+        for item_i, dt in enumerate(group):
+            if dtype == dt:
+                return group_i, item_i
+    raise TypeError(f"Unsupported dtype {dtype}! Supported dtypes {','.join(map(repr, _supported_dtypes))}")
+
+
+def get_compact_dtype(dtype0: tf.DType, *dtypes: tf.DType) -> tf.DType:
+    group_i, item_i = get_dtype_indices(dtype0)
+    for dt in dtypes:
+        gi, ii = get_dtype_indices(dt)
+        group_i = max(group_i, gi)
+        item_i = max(item_i, ii)
+    return _grouped_dtypes[group_i][item_i]
```

### Comparing `BraAndKet-0.8.3/src/braandket/model/model.py` & `BraAndKet-0.8.4/src/braandket/model/model.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/src/braandket/space/hilbert_space.py` & `BraAndKet-0.8.4/src/braandket/space/hilbert_space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/src/braandket/space/num_space.py` & `BraAndKet-0.8.4/src/braandket/space/num_space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/src/braandket/space/space.py` & `BraAndKet-0.8.4/src/braandket/space/space.py`

 * *Files identical despite different names*

### Comparing `BraAndKet-0.8.3/src/braandket/tensor/operations.py` & `BraAndKet-0.8.4/src/braandket/tensor/operations.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import math
 from typing import Any, Callable, Iterable, Optional, Union
 
-from braandket.backend import Backend, ValuesType, get_default_backend
+from braandket.backend import Backend, BackendValue, get_default_backend
 from braandket.space import HSpace, KetSpace, NumSpace, Space
 from .special import NumericTensor, OperatorTensor, PureStateTensor
 from .tensor import QTensor
 
 # constants
 
 e = math.e
@@ -135,15 +135,15 @@
 
 def _expand_with_identities(tensor: OperatorTensor, *spaces: KetSpace):
     return prod(tensor, *(space.identity(backend=tensor.backend) for space in spaces))
 
 
 # numeric
 
-def _construct_wrapped_unary_op(func: Callable[[ValuesType], ValuesType]):
+def _construct_wrapped_unary_op(func: Callable[[BackendValue], BackendValue]):
     def wrapped_op(value: Union[NumericTensor, Any]) -> NumericTensor:
         value = NumericTensor.of(value)
         op = getattr(value.backend, func.__name__)
         # noinspection PyProtectedMember
         return value.spawn(op(value._values), value._spaces)
 
     return wrapped_op
```

### Comparing `BraAndKet-0.8.3/src/braandket/tensor/special.py` & `BraAndKet-0.8.4/src/braandket/tensor/special.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import abc
 from typing import Any, Generic, Iterable, Optional, Union
 
-from braandket.backend import Backend, ValuesType, get_default_backend
+from braandket.backend import Backend, BackendValue, get_default_backend
 from braandket.space import KetSpace, NumSpace, Space
 from .tensor import QTensor
 
 
 # special tensors
 
-class NumericTensor(QTensor[ValuesType]):
+class NumericTensor(QTensor[BackendValue]):
 
     @classmethod
     def of(cls,
         values: Union[QTensor, Any],
         spaces: Optional[Iterable[Space]] = None, *,
         backend: Optional[Backend] = None
     ) -> 'NumericTensor':
@@ -39,15 +39,15 @@
 
     # linear operations
 
     def _mul_expanded_num_spaces(self, other: 'QTensor') -> 'NumericTensor':
         return self @ other
 
 
-class StateTensor(QTensor[ValuesType], Generic[ValuesType], abc.ABC):
+class StateTensor(QTensor[BackendValue], Generic[BackendValue], abc.ABC):
     @property
     @abc.abstractmethod
     def ket_spaces(self) -> tuple[KetSpace, ...]:
         pass
 
     # norm
 
@@ -78,19 +78,19 @@
         remain_ket_spaces_set = frozenset(spaces)
         traced_ket_spaces = all_ket_spaces - remain_ket_spaces_set
         return self.trace(*traced_ket_spaces)
 
     @abc.abstractmethod
     def probabilities(self,
         *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
-    ) -> ValuesType:
+    ) -> BackendValue:
         pass
 
 
-class PureStateTensor(StateTensor[ValuesType]):
+class PureStateTensor(StateTensor[BackendValue]):
 
     @classmethod
     def of(cls,
         values: Union[QTensor, Any],
         spaces: Optional[Iterable[Union[NumSpace, KetSpace]]] = None, *,
         backend: Optional[Backend] = None
     ) -> 'PureStateTensor':
@@ -143,25 +143,25 @@
         return PureStateTensor.of(self[indices])
 
     def trace(self, *spaces: KetSpace) -> 'MixedStateTensor':
         return MixedStateTensor.of(self @ self.ct).trace(*spaces)
 
     def amplitudes(self,
         *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
-    ) -> ValuesType:
+    ) -> BackendValue:
         return self.values(*spaces)
 
     def probabilities(self,
         *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
-    ) -> ValuesType:
+    ) -> BackendValue:
         amplitudes = self.amplitudes(*spaces)
         return self.backend.mul(self.backend.conj(amplitudes), amplitudes)
 
 
-class MixedStateTensor(StateTensor[ValuesType]):
+class MixedStateTensor(StateTensor[BackendValue]):
     @classmethod
     def of(cls,
         values: Union[QTensor, Any],
         spaces: Optional[Iterable[Union[NumSpace, KetSpace]]] = None, *,
         backend: Optional[Backend] = None
     ) -> 'MixedStateTensor':
         if isinstance(values, MixedStateTensor):
@@ -207,30 +207,30 @@
     def trace(self, *spaces: KetSpace) -> 'MixedStateTensor':
         values, spaces = self.values_and_slices(*spaces)
         ket_axes, bra_axes = _index_spaces_pairs(spaces)
         return self.backend.trace(values, (ket_axes, bra_axes))
 
     def probabilities(self,
         *spaces: Union[NumSpace, KetSpace, tuple[Union[NumSpace, KetSpace], Union[int, None]]]
-    ) -> ValuesType:
+    ) -> BackendValue:
         bra_spaces = []
         for space_or_pair in spaces:
             if isinstance(space_or_pair, Space):
                 space, index = space_or_pair, None
             else:
                 space, index = space_or_pair
             if isinstance(space, KetSpace):
                 if index is None:
                     bra_spaces.append(space.ct)
                 else:
                     bra_spaces.append((space.ct, index))
         return self.values(*spaces, *bra_spaces)
 
 
-class OperatorTensor(QTensor[ValuesType]):
+class OperatorTensor(QTensor[BackendValue]):
     @classmethod
     def of(cls,
         values: Union[QTensor, Any],
         spaces: Optional[Iterable[Space]] = None, *,
         backend: Optional[Backend] = None
     ) -> 'OperatorTensor':
         if isinstance(values, OperatorTensor):
@@ -238,15 +238,15 @@
         if isinstance(values, QTensor):
             # noinspection PyTypeChecker
             return cls(values._values, values._spaces, values._backend)
         return cls(values, spaces, backend or get_default_backend())
 
     @classmethod
     def from_matrix(cls,
-        matrix: ValuesType,
+        matrix: BackendValue,
         ket_spaces: Iterable[KetSpace] | KetSpace,
         num_spaces: Iterable[NumSpace] | NumSpace = (), *,
         backend: Optional[Backend] = None
     ) -> 'OperatorTensor':
         num_spaces = (num_spaces,) if isinstance(num_spaces, NumSpace) else tuple(num_spaces)
         ket_spaces = (ket_spaces,) if isinstance(ket_spaces, KetSpace) else tuple(ket_spaces)
         bra_spaces = tuple(space.ct for space in ket_spaces)
```

### Comparing `BraAndKet-0.8.3/src/braandket/tensor/tensor.py` & `BraAndKet-0.8.4/src/braandket/tensor/tensor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import abc
 from typing import Any, Generic, Iterable, Optional, Union
 
-from braandket.backend import Backend, ValuesType, get_default_backend
+from braandket.backend import Backend, BackendValue, get_default_backend
 from braandket.space import BraSpace, HSpace, KetSpace, NumSpace, Space
 from braandket.utils import iter_structure
 
 
-class QTensor(Generic[ValuesType], abc.ABC):
+class QTensor(Generic[BackendValue], abc.ABC):
 
     @classmethod
     def of(cls, values: Any, spaces: Iterable[Space], *, backend: Optional[Backend] = None) -> 'QTensor':
         if backend is None:
             backend = get_default_backend()
         spaces = tuple(spaces)
 
@@ -44,34 +44,34 @@
 
         # construct
         self._spaces = spaces
         self._values = values
         self._backend = backend
 
     @property
-    def backend(self) -> Backend[ValuesType]:
+    def backend(self) -> Backend[BackendValue]:
         return self._backend
 
     def spawn(self, values: Any, spaces: Iterable[Space]) -> 'QTensor':
         """ create a new BackendTensor instance with the same backend """
         return QTensor.of(values, spaces, backend=self.backend)
 
     # basic operations
 
     @property
     def spaces(self) -> tuple[Space, ...]:
         return self._spaces
 
-    def values(self, *slices: Union[Space, tuple[Space, Union[int, None]]]) -> ValuesType:
+    def values(self, *slices: Union[Space, tuple[Space, Union[int, None]]]) -> BackendValue:
         """ get values from this tensor """
         return self.values_and_slices(*slices)[0]
 
     def values_and_slices(self,
         *slices: Union[Space, tuple[Space, Union[int, None]]]
-    ) -> tuple[ValuesType, tuple[Union[Space, tuple[Space, int]], ...]]:
+    ) -> tuple[BackendValue, tuple[Union[Space, tuple[Space, int]], ...]]:
         if len(slices) == 0:
             return self._values, self._spaces
 
         # parse arguments
         sp_slices = slices
         spaces = []
         slices = []
@@ -143,15 +143,15 @@
 
     # scalar operations
 
     @property
     def is_scalar(self) -> bool:
         return len(self.spaces) == 0
 
-    def scalar(self) -> ValuesType:
+    def scalar(self) -> BackendValue:
         """ get a scalar value from zero-dimension tensor """
         if not self.is_scalar:
             raise ValueError(f"This QTensor is not a scalar. It has {len(self.spaces)} spaces.")
         return self.values()
 
     def __float__(self) -> float:
         return float(self.scalar())
@@ -305,15 +305,15 @@
         from .special import OperatorTensor
         return OperatorTensor.of(self)
 
     # inflate & flatten
 
     @classmethod
     def inflate(cls,
-        values: ValuesType,
+        values: BackendValue,
         spaces: Iterable[Union[NumSpace, KetSpace, BraSpace, Iterable[Union[NumSpace, KetSpace, BraSpace]]]], *,
         backend: Optional[Backend] = None
     ) -> 'QTensor':
         if backend is None:
             backend = get_default_backend()
         spaces = tuple(iter_structure(spaces))
         shape = tuple(space.n for space in spaces)
@@ -321,15 +321,15 @@
         return cls.of(values, spaces, backend=backend)
 
     def flatten(self,
         spaces: Optional[Iterable[Union[NumSpace, KetSpace, BraSpace]]] = None, *,
         num_spaces: Optional[Iterable[NumSpace]] = None,
         ket_spaces: Optional[Iterable[KetSpace]] = None,
         bra_spaces: Optional[Iterable[BraSpace]] = None,
-    ) -> tuple[ValuesType, tuple[Union[NumSpace, tuple[KetSpace, ...], tuple[BraSpace, ...]], ...]]:
+    ) -> tuple[BackendValue, tuple[Union[NumSpace, tuple[KetSpace, ...], tuple[BraSpace, ...]], ...]]:
         num_spaces_sl = tuple(space for space in self.spaces if isinstance(space, NumSpace))
         ket_spaces_sl = tuple(space for space in self.spaces if isinstance(space, KetSpace))
         bra_spaces_sl = tuple(space for space in self.spaces if isinstance(space, BraSpace))
 
         spaces = tuple(spaces) if spaces is not None else ()
         num_spaces_sp = tuple(space for space in spaces if isinstance(space, NumSpace))
         ket_spaces_sp = tuple(space for space in spaces if isinstance(space, KetSpace))
@@ -358,15 +358,15 @@
         return values, (*num_spaces, tuple(ket_spaces), tuple(bra_spaces))
 
     def flattened_values(self,
         spaces: Optional[Iterable[Union[NumSpace, KetSpace, BraSpace]]] = None, *,
         num_spaces: Optional[Iterable[NumSpace]] = None,
         ket_spaces: Optional[Iterable[KetSpace]] = None,
         bra_spaces: Optional[Iterable[BraSpace]] = None,
-    ) -> ValuesType:
+    ) -> BackendValue:
         return self.flatten(
             spaces,
             num_spaces=num_spaces,
             ket_spaces=ket_spaces,
             bra_spaces=bra_spaces
         )[0]
```

### Comparing `BraAndKet-0.8.3/src/braandket/utils/utils.py` & `BraAndKet-0.8.4/src/braandket/utils/utils.py`

 * *Files identical despite different names*

