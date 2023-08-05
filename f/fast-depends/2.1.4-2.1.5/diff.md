# Comparing `tmp/fast_depends-2.1.4.tar.gz` & `tmp/fast_depends-2.1.5.tar.gz`

## Comparing `fast_depends-2.1.4.tar` & `fast_depends-2.1.5.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.4/CONTRIBUTING.md
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.4/.github/workflows/documentation.yml
--rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.4/.github/workflows/publish_coverage.yml
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.4/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.4/.github/workflows/tests.yml
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/__about__.py
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/__init__.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/_compat.py
--rw-r--r--   0        0        0     4313 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/use.py
--rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/utils.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/core/__init__.py
--rw-r--r--   0        0        0     5455 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/core/build.py
--rw-r--r--   0        0        0    10809 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/core/model.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/dependencies/__init__.py
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/dependencies/model.py
--rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/dependencies/provider.py
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/library/__init__.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.4/fast_depends/library/model.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 fast_depends-2.1.4/scripts/lint.sh
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.4/scripts/publish.sh
--rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.4/scripts/test-cov.sh
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.4/scripts/test.sh
--rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.4/.gitignore
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.4/LICENSE
--rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.4/README.md
--rw-r--r--   0        0        0     4108 2020-02-02 00:00:00.000000 fast_depends-2.1.4/pyproject.toml
--rw-r--r--   0        0        0     6985 2020-02-02 00:00:00.000000 fast_depends-2.1.4/PKG-INFO
+-rw-r--r--   0        0        0     2030 2020-02-02 00:00:00.000000 fast_depends-2.1.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 fast_depends-2.1.5/.github/workflows/documentation.yml
+-rw-r--r--   0        0        0      956 2020-02-02 00:00:00.000000 fast_depends-2.1.5/.github/workflows/publish_coverage.yml
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 fast_depends-2.1.5/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 fast_depends-2.1.5/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/__about__.py
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/__init__.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/_compat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/py.typed
+-rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/use.py
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/utils.py
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/core/__init__.py
+-rw-r--r--   0        0        0     5476 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/core/build.py
+-rw-r--r--   0        0        0    10864 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/core/model.py
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/dependencies/__init__.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/dependencies/model.py
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/dependencies/provider.py
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/library/__init__.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 fast_depends-2.1.5/fast_depends/library/model.py
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 fast_depends-2.1.5/scripts/lint.sh
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 fast_depends-2.1.5/scripts/publish.sh
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 fast_depends-2.1.5/scripts/test-cov.sh
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fast_depends-2.1.5/scripts/test.sh
+-rw-r--r--   0        0        0      215 2020-02-02 00:00:00.000000 fast_depends-2.1.5/.gitignore
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 fast_depends-2.1.5/LICENSE
+-rw-r--r--   0        0        0     4494 2020-02-02 00:00:00.000000 fast_depends-2.1.5/README.md
+-rw-r--r--   0        0        0     4137 2020-02-02 00:00:00.000000 fast_depends-2.1.5/pyproject.toml
+-rw-r--r--   0        0        0     7038 2020-02-02 00:00:00.000000 fast_depends-2.1.5/PKG-INFO
```

### Comparing `fast_depends-2.1.4/CONTRIBUTING.md` & `fast_depends-2.1.5/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/.github/workflows/documentation.yml` & `fast_depends-2.1.5/.github/workflows/documentation.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/.github/workflows/publish_coverage.yml` & `fast_depends-2.1.5/.github/workflows/publish_coverage.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/.github/workflows/publish_pypi.yml` & `fast_depends-2.1.5/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/.github/workflows/tests.yml` & `fast_depends-2.1.5/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/fast_depends/_compat.py` & `fast_depends-2.1.5/fast_depends/_compat.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 if PYDANTIC_V2:
     from pydantic._internal._typing_extra import (
         eval_type_lenient as evaluate_forwardref,
     )
     from pydantic.fields import FieldInfo
 else:
-    from pydantic.fields import ModelField as FieldInfo  # type: ignore[no-redef]
+    from pydantic.fields import ModelField as FieldInfo  # type: ignore
     from pydantic.typing import evaluate_forwardref  # type: ignore[no-redef]
 
 
 __all__ = (
     "BaseModel",
     "FieldInfo",
     "create_model",
```

### Comparing `fast_depends-2.1.4/fast_depends/use.py` & `fast_depends-2.1.5/fast_depends/use.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from contextlib import AsyncExitStack, ExitStack
 from functools import wraps
 from typing import Any, Awaitable, Callable, Optional, Sequence, Union, overload
 
-from typing_extensions import ParamSpec, TypeVar
+from typing_extensions import ParamSpec, Protocol, TypeVar
 
 from fast_depends.core import CallModel, build_call_model
 from fast_depends.dependencies import dependency_provider, model
 
 P = ParamSpec("P")
 T = TypeVar("T")
 
@@ -80,73 +80,80 @@
     if func is None:
         return decorator
 
     else:
         return decorator(func)
 
 
+class _InjectWrapper(Protocol[P, T]):
+    def __call__(
+        self,
+        func: Union[Callable[P, T], Callable[P, Awaitable[T]]],
+        model: Optional[CallModel[P, T]] = None,
+    ) -> Union[Callable[P, T], Callable[P, Awaitable[T]]]:
+        ...
+
+
 def _wrap_inject(
     dependency_overrides_provider: Optional[Any],
     wrap_model: Callable[
         [CallModel[P, T]],
         CallModel[P, T],
     ],
     extra_dependencies: Sequence[model.Depends],
-) -> Callable[
-    [
-        Union[Callable[P, T], Callable[P, Awaitable[T]]],
-        Optional[CallModel[P, T]],
-    ],
-    Union[Callable[P, T], Callable[P, Awaitable[T]]],
-]:
+) -> _InjectWrapper[P, T]:
     if (
         dependency_overrides_provider
         and getattr(dependency_overrides_provider, "dependency_overrides", None)
         is not None
     ):
         overrides = dependency_overrides_provider.dependency_overrides
     else:
         overrides = None
 
     def func_wrapper(
         func: Union[Callable[P, T], Callable[P, Awaitable[T]]],
         model: Optional[CallModel[P, T]] = None,
     ) -> Union[Callable[P, T], Callable[P, Awaitable[T]]]:
         if model is None:
-            model = wrap_model(
+            real_model = wrap_model(
                 build_call_model(
                     func,
                     extra_dependencies=extra_dependencies,
                 )
             )
+        else:
+            real_model = model
 
-        if model.is_async:
+        if real_model.is_async:
 
             @wraps(func)
             async def injected_wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
                 async with AsyncExitStack() as stack:
-                    r = await model.asolve(
+                    r = await real_model.asolve(
                         *args,
                         stack=stack,
                         dependency_overrides=overrides,
                         cache_dependencies={},
                         **kwargs,
                     )
                     return r
+                raise AssertionError("unreachable")
 
         else:
 
             @wraps(func)
             def injected_wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
                 with ExitStack() as stack:
-                    r = model.solve(
+                    r = real_model.solve(
                         *args,
                         stack=stack,
                         dependency_overrides=overrides,
                         cache_dependencies={},
                         **kwargs,
                     )
                     return r
+                raise AssertionError("unreachable")
 
         return injected_wrapper
 
     return func_wrapper
```

### Comparing `fast_depends-2.1.4/fast_depends/utils.py` & `fast_depends-2.1.5/fast_depends/utils.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/fast_depends/core/build.py` & `fast_depends-2.1.5/fast_depends/core/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,14 +90,15 @@
 
                 annotation = type_annotation
             else:
                 annotation = param.annotation
         else:
             annotation = param.annotation
 
+        default: Any
         if param.name == "args":
             default = ()
         elif param.name == "kwargs":
             default = {}
         else:
             default = param.default
```

### Comparing `fast_depends-2.1.4/fast_depends/core/model.py` & `fast_depends-2.1.5/fast_depends/core/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,16 +44,16 @@
 
     params: Dict[str, FieldInfo]
     alias_arguments: List[str]
 
     dependencies: Dict[str, "CallModel[..., Any]"]
     extra_dependencies: Iterable["CallModel[..., Any]"]
     custom_fields: Dict[str, CustomField]
-    keyword_args: Tuple[str]
-    positional_args: Tuple[str]
+    keyword_args: Tuple[str, ...]
+    positional_args: Tuple[str, ...]
 
     # Dependencies and custom fields
     use_cache: bool
     cast: bool
 
     __slots__ = (
         "call",
@@ -109,25 +109,25 @@
     ):
         self.call = call
         self.model = model
         self.response_model = response_model
 
         fields: Dict[str, FieldInfo]
         if PYDANTIC_V2:
-            fields = self.model.model_fields  # type: ignore
+            fields = self.model.model_fields
         else:
             fields = self.model.__fields__  # type: ignore
 
         self.dependencies = dependencies or {}
         self.extra_dependencies = extra_dependencies or []
         self.custom_fields = custom_fields or {}
 
         self.alias_arguments = [f.alias or name for name, f in fields.items()]
-        self.keyword_args = tuple(keyword_args or [])
-        self.positional_args = tuple(positional_args or [])
+        self.keyword_args = tuple(keyword_args or ())
+        self.positional_args = tuple(positional_args or ())
 
         self.params = fields.copy()
         for name in self.dependencies.keys():
             self.params.pop(name, None)
 
         self.use_cache = use_cache
         self.cast = cast
@@ -155,15 +155,15 @@
                 Union[
                     Callable[P, T],
                     Callable[P, Awaitable[T]],
                 ],
             ]
         ] = None,
         **kwargs: P.kwargs,
-    ) -> Generator[Dict[str, Any], Any, T]:
+    ) -> Generator[Tuple[Iterable[Any], Dict[str, Any]], Any, T]:
         if dependency_overrides:
             self.call = dependency_overrides.get(self.call, self.call)
             assert self.is_async or not is_coroutine_callable(
                 self.call
             ), f"You cannot use async dependency `{self.call_name}` at sync main"
 
         if self.use_cache and self.call in cache_dependencies:
@@ -193,28 +193,29 @@
 
         else:
             for arg in self.keyword_args:
                 if args:
                     kw[arg], args = args[0], args[1:]
 
         solved_kw: Dict[str, Any]
-        solved_kw = yield kw
+        solved_kw = yield (), kw
 
         casted_model = self.model(**solved_kw)
 
         kwargs_ = {
             arg: getattr(casted_model, arg, solved_kw.get(arg))
             for arg in (
                 self.keyword_args + self.positional_args
                 if not has_args
                 else self.keyword_args
             )
         }
         kwargs_.update(getattr(casted_model, "kwargs", {}))
 
+        args_: Iterable[Any]
         if has_args:
             args_ = [
                 getattr(casted_model, arg, solved_kw.get(arg))
                 for arg in self.positional_args
             ]
             args_.extend(getattr(casted_model, "args", ()))
         else:
@@ -260,15 +261,15 @@
         cast_gen = self._solve(
             *args,
             cache_dependencies=cache_dependencies,
             dependency_overrides=dependency_overrides,
             **kwargs,
         )
         try:
-            kwargs = next(cast_gen)
+            _, kwargs = next(cast_gen)
         except StopIteration as e:
             cached_value: T = e.value
             return cached_value
 
         for dep in self.extra_dependencies:
             dep.solve(
                 stack=stack,
@@ -336,15 +337,15 @@
         cast_gen = self._solve(
             *args,
             cache_dependencies=cache_dependencies,
             dependency_overrides=dependency_overrides,
             **kwargs,
         )
         try:
-            kwargs = next(cast_gen)
+            _, kwargs = next(cast_gen)
         except StopIteration as e:
             cached_value: T = e.value
             return cached_value
 
         for dep in self.extra_dependencies:
             await dep.asolve(
                 stack=stack,
```

### Comparing `fast_depends-2.1.4/fast_depends/dependencies/model.py` & `fast_depends-2.1.5/fast_depends/dependencies/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/fast_depends/library/model.py` & `fast_depends-2.1.5/fast_depends/library/model.py`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/LICENSE` & `fast_depends-2.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/README.md` & `fast_depends-2.1.5/README.md`

 * *Files identical despite different names*

### Comparing `fast_depends-2.1.4/pyproject.toml` & `fast_depends-2.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
     "fast-depends[test]",
     "fast-depends[doc]",
 
     "mypy>=1.1",
     "black>=23.3.0",
     "isort>=5",
     "ruff>=0.0.260",
+    "pyupgrade-directories",
 ]
 
 [tool.hatch.metadata]
 allow-direct-references = true
 allow-ambiguous-features = true
 
 [tool.hatch.version]
```

### Comparing `fast_depends-2.1.4/PKG-INFO` & `fast_depends-2.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fast-depends
-Version: 2.1.4
+Version: 2.1.5
 Summary: FastDepends - extracted and cleared from HTTP domain logic FastAPI Dependency Injection System. Async and sync are both supported.
 Project-URL: Homepage, https://lancetnik.github.io/FastDepends/
 Project-URL: Documentation, https://lancetnik.github.io/FastDepends/
 Project-URL: Tracker, https://github.com/Lancetnik/FastDepends/issues
 Project-URL: Source, https://github.com/Lancetnik/FastDepends
 Author-email: Pastukhov Nikita <diementros@yandex.ru>
 License-File: LICENSE
@@ -34,14 +34,15 @@
 Requires-Dist: pydantic!=1.8,!=1.8.1,<3.0.0,>=1.7.4
 Provides-Extra: dev
 Requires-Dist: black>=23.3.0; extra == 'dev'
 Requires-Dist: fast-depends[doc]; extra == 'dev'
 Requires-Dist: fast-depends[test]; extra == 'dev'
 Requires-Dist: isort>=5; extra == 'dev'
 Requires-Dist: mypy>=1.1; extra == 'dev'
+Requires-Dist: pyupgrade-directories; extra == 'dev'
 Requires-Dist: ruff>=0.0.260; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material<9.0.0,>=8.1.4; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: asyncmock; python_version < '3.8' and extra == 'test'
```

