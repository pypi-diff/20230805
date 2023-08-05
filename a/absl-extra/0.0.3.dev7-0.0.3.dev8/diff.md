# Comparing `tmp/absl_extra-0.0.3.dev7.tar.gz` & `tmp/absl_extra-0.0.3.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "absl_extra-0.0.3.dev7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "absl_extra-0.0.3.dev8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `absl_extra-0.0.3.dev7.tar` & `absl_extra-0.0.3.dev8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1521 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/Readme.md
--rw-r--r--   0        0        0      127 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/__init__.py
--rw-r--r--   0        0        0     1945 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/callbacks.py
--rw-r--r--   0        0        0    18863 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/flax_utils.py
--rw-r--r--   0        0        0     2000 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/jax_utils.py
--rw-r--r--   0        0        0     1184 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/keras_pbar.py
--rw-r--r--   0        0        0     1605 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/logging_utils.py
--rw-r--r--   0        0        0     3238 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/notifier.py
--rw-r--r--   0        0        0       64 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/py.typed
--rw-r--r--   0        0        0     5741 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/tasks.py
--rw-r--r--   0        0        0        0 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/testing/__init__.py
--rw-r--r--   0        0        0     2301 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/testing/lifted_variants.py
--rw-r--r--   0        0        0     4623 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/absl_extra/tf_utils.py
--rw-r--r--   0        0        0     1071 2023-07-19 23:01:31.839002 absl_extra-0.0.3.dev7/pyproject.toml
--rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 absl_extra-0.0.3.dev7/PKG-INFO
+-rw-r--r--   0        0        0     1521 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/Readme.md
+-rw-r--r--   0        0        0      127 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/__init__.py
+-rw-r--r--   0        0        0     1974 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/callbacks.py
+-rw-r--r--   0        0        0    18863 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/flax_utils.py
+-rw-r--r--   0        0        0     2000 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/jax_utils.py
+-rw-r--r--   0        0        0     1184 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/keras_pbar.py
+-rw-r--r--   0        0        0     2663 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/logging_utils.py
+-rw-r--r--   0        0        0     3238 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/notifier.py
+-rw-r--r--   0        0        0       64 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/py.typed
+-rw-r--r--   0        0        0     5090 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/tasks.py
+-rw-r--r--   0        0        0        0 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2301 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/testing/lifted_variants.py
+-rw-r--r--   0        0        0     4623 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/absl_extra/tf_utils.py
+-rw-r--r--   0        0        0     1071 2023-08-01 17:28:05.086189 absl_extra-0.0.3.dev8/pyproject.toml
+-rw-r--r--   0        0        0     2938 1970-01-01 00:00:00.000000 absl_extra-0.0.3.dev8/PKG-INFO
```

### Comparing `absl_extra-0.0.3.dev7/Readme.md` & `absl_extra-0.0.3.dev8/Readme.md`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/absl_extra/callbacks.py` & `absl_extra-0.0.3.dev8/absl_extra/callbacks.py`

 * *Files 5% similar despite different names*

```diff
@@ -69,9 +69,9 @@
 ]
 DEFAULT_POST_CALLBACK = [
     log_shutdown_callback,
 ]
 
 if util.find_spec("tensorflow"):
     DEFAULT_INIT_CALLBACKS.append(log_tensorflow_devices)
-if util.find_spec("jax"):
+if util.find_spec("jax") and util.find_spec("jaxlib"):
     DEFAULT_INIT_CALLBACKS.append(log_jax_devices)
```

### Comparing `absl_extra-0.0.3.dev7/absl_extra/flax_utils.py` & `absl_extra-0.0.3.dev8/absl_extra/flax_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/absl_extra/jax_utils.py` & `absl_extra-0.0.3.dev8/absl_extra/jax_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/absl_extra/keras_pbar.py` & `absl_extra-0.0.3.dev8/absl_extra/keras_pbar.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/absl_extra/logging_utils.py` & `absl_extra-0.0.3.dev8/absl_extra/logging_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -57,7 +57,43 @@
 
     absl.logging.set_verbosity(absl.logging.converter.ABSL_NAMES[log_level])
 
     if util.find_spec("tensorflow"):
         import tensorflow as tf
 
         tf.get_logger().setLevel(log_level)
+
+
+@toolz.curry
+def log_before(
+    func: Callable[P, T], logger: Callable[[str], None] = logging.debug
+) -> Callable[P, T]:
+    """Log functions argument before calling it."""
+
+    @functools.wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> T:
+        func_args = inspect.signature(func).bind(*args, **kwargs).arguments
+        func_args_str = ", ".join(map("{0[0]} = {0[1]!r}".format, func_args.items()))
+        logger(
+            f"Entered {func.__module__}.{func.__qualname__} with args ( {func_args_str} )"
+        )
+        return func(*args, **kwargs)
+
+    return wrapper
+
+
+@toolz.curry
+def log_after(
+    func: Callable[P, T], logger: Callable[[str], None] = logging.debug
+) -> Callable[P, T]:
+    """Log's function's return value."""
+
+    @functools.wraps(func)
+    def wrapper(*args: P.args, **kwargs: P.kwargs) -> R:
+        retval = func(*args, **kwargs)
+        logger(
+            f"Exited {func.__module__}.{func.__qualname__}(...) with value: "
+            + repr(retval)
+        )
+        return retval
+
+    return wrapper
```

### Comparing `absl_extra-0.0.3.dev7/absl_extra/notifier.py` & `absl_extra-0.0.3.dev8/absl_extra/notifier.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/absl_extra/tasks.py` & `absl_extra-0.0.3.dev8/absl_extra/tasks.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,25 +25,19 @@
 if util.find_spec("pymongo"):
     from pymongo import MongoClient
     from pymongo.collection import Collection
 else:
     Collection = type(None)
     logging.warning("pymongo not installed.")
 
-if util.find_spec("ml_collections"):
-    from ml_collections import ConfigDict, config_flags
-else:
-    logging.warning("ml_collections not installed")
-    ConfigDict = None
-
 if TYPE_CHECKING:
     from absl_extra.callbacks import CallbackFn
 
 
-@dataclasses.dataclass(frozen=True, slots=True)
+@dataclasses.dataclass(frozen=True)
 class MongoConfig:
     uri: str
     db_name: str
     collection: str
 
 
 class _ExceptionHandlerImpl(app.ExceptionHandler):
@@ -52,17 +46,15 @@
         self.notifier = notifier
 
     def handle(self, exception: Exception) -> None:
         self.notifier.notify_task_failed(self.name, exception)
 
 
 class _TaskFn(Protocol):
-    def __call__(
-        self, *, config: ConfigDict = None, db: Collection = None, **kwargs
-    ) -> None:
+    def __call__(self, *, db: Collection = None, **kwargs) -> None:
         ...
 
 
 _TASK_STORE: Dict[str, Callable[[...], None]] = dict()  # type: ignore
 
 
 class NonExistentTaskError(RuntimeError):
@@ -73,62 +65,54 @@
 
 
 def _make_task_func(
     func: _TaskFn,
     *,
     name: str,
     notifier: BaseNotifier | Callable[[], BaseNotifier],
-    config_file: str | None,
     init_callbacks: List[CallbackFn],
     post_callbacks: List[CallbackFn],
-    db: Collection | None,
+    db_factory=None,
 ) -> _TaskFn:
     _name = name
 
     @functools.wraps(func)
     def wrapper(*args, **kwargs):
         app.install_exception_handler(_ExceptionHandlerImpl(name, notifier))  # type: ignore
-        if util.find_spec("ml_collections") and config_file is not None:
-            config = config_flags.DEFINE_config_file("config", default=config_file)
-            config = config.value
-            kwargs["config"] = config
-        else:
-            config = None
-        if db is not None:
+        kwargs = {}
+        if db_factory is not None:
+            db = db_factory()
             kwargs["db"] = db
 
         for hook in init_callbacks:
-            hook(_name, notifier=notifier, config=config, db=db)
+            hook(_name, notifier=notifier, **kwargs)
 
         func(*args, **kwargs)
 
         for hook in post_callbacks:
-            hook(_name, notifier=notifier, config=config, db=db)
+            hook(_name, notifier=notifier, **kwargs)
 
     return wrapper
 
 
 def register_task(
     *,
     name: str = "main",
     notifier: BaseNotifier | Callable[[], BaseNotifier] | None = None,
-    config_file: str | None = None,
     mongo_config: MongoConfig | Mapping[str, Any] | None = None,
     init_callbacks: List[CallbackFn] | None = None,
     post_callbacks: List[CallbackFn] | None = None,
 ) -> Callable[[_TaskFn], None]:
     """
     Parameters
     ----------
     name : str, optional
         The name of the task. Default is "main".
     notifier : BaseNotifier | Callable[[], BaseNotifier] | None, optional
         The notifier object or callable that returns a notifier object. Default is None.
-    config_file : str | None, optional
-        The path to the configuration file. Default is None.
     mongo_config : MongoConfig | Mapping[str, Any] | None, optional
         The configuration object for MongoDB or a mapping of configuration values. Default is None.
     init_callbacks : List[CallbackFn] | None, optional
         The list of callback functions to be executed during task initialization. Default is None.
     post_callbacks : List[CallbackFn] | None, optional
         The list of callback functions to be executed after the task completes. Default is None.
 
@@ -140,40 +124,40 @@
     from absl_extra.callbacks import DEFAULT_INIT_CALLBACKS, DEFAULT_POST_CALLBACK
 
     if isinstance(notifier, Callable):  # type: ignore
         notifier = notifier()  # type: ignore
     if notifier is None:
         notifier = LoggingNotifier()
 
+    kwargs = {}
+
     if util.find_spec("pymongo") and mongo_config is not None:
         if isinstance(mongo_config, Mapping):
             mongo_config = MongoConfig(**mongo_config)
-        db: Collection[Mapping[str, ...]] = (
+        db_factory = lambda: (
             MongoClient(mongo_config.uri)
             .get_database(mongo_config.db_name)
             .get_collection(mongo_config.collection)
         )
-    else:
-        db = None
+        kwargs["db_factory"] = db_factory
 
     if init_callbacks is None:
         init_callbacks = DEFAULT_INIT_CALLBACKS  # type: ignore
 
     if post_callbacks is None:
         post_callbacks = DEFAULT_POST_CALLBACK  # type: ignore
 
     def decorator(func: _TaskFn) -> None:
         _TASK_STORE[name] = functools.partial(  # type: ignore
             _make_task_func,
             name=name,
             notifier=notifier,
             init_callbacks=init_callbacks,
             post_callbacks=post_callbacks,
-            db=db,
-            config_file=config_file,
+            **kwargs,
         )(func)
 
     return decorator
 
 
 def run(argv: List[str] | None = None, **kwargs):
     """
```

### Comparing `absl_extra-0.0.3.dev7/absl_extra/testing/lifted_variants.py` & `absl_extra-0.0.3.dev8/absl_extra/testing/lifted_variants.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/absl_extra/tf_utils.py` & `absl_extra-0.0.3.dev8/absl_extra/tf_utils.py`

 * *Files identical despite different names*

### Comparing `absl_extra-0.0.3.dev7/pyproject.toml` & `absl_extra-0.0.3.dev8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "absl_extra"
-version = "0.0.3dev7"
+version = "0.0.3dev8"
 description = "A wrapper to run and monitor absl app."
 readme = "Readme.md"
 requires-python = ">=3.8"
 authors = [
     { name = "Artem Sereda", email = "artem.sereda.tub@gmail.com" }
 ]
 maintainers = [
```

### Comparing `absl_extra-0.0.3.dev7/PKG-INFO` & `absl_extra-0.0.3.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: absl_extra
-Version: 0.0.3.dev7
+Version: 0.0.3.dev8
 Summary: A wrapper to run and monitor absl app.
 Author-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Maintainer-email: Artem Sereda <artem.sereda.tub@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Requires-Dist: absl_py
```

