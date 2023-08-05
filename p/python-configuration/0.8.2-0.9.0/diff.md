# Comparing `tmp/python-configuration-0.8.2.tar.gz` & `tmp/python_configuration-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-configuration-0.8.2.tar", last modified: Sat Jan 30 12:33:01 2021, max compression
+gzip compressed data, was "python_configuration-0.9.0.tar", max compression
```

## Comparing `python-configuration-0.8.2.tar` & `python_configuration-0.9.0.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0     1071 2019-01-16 09:12:21.684138 python-configuration-0.8.2/LICENSE
--rw-r--r--   0        0        0    10002 2020-07-07 17:32:20.554447 python-configuration-0.8.2/README.md
--rw-r--r--   0        0        0    24412 2021-01-30 12:19:44.856634 python-configuration-0.8.2/config/__init__.py
--rw-r--r--   0        0        0    12462 2021-01-29 21:33:48.670680 python-configuration-0.8.2/config/configuration.py
--rw-r--r--   0        0        0     7391 2021-01-30 12:21:04.840439 python-configuration-0.8.2/config/configuration_set.py
--rw-r--r--   0        0        0       43 2020-01-08 17:02:05.030775 python-configuration-0.8.2/config/contrib/__init__.py
--rw-r--r--   0        0        0     4880 2020-08-01 13:58:43.787841 python-configuration-0.8.2/config/contrib/aws.py
--rw-r--r--   0        0        0     5288 2020-08-01 13:58:43.787841 python-configuration-0.8.2/config/contrib/azure.py
--rw-r--r--   0        0        0     5498 2020-08-01 13:58:43.787841 python-configuration-0.8.2/config/contrib/gcp.py
--rw-r--r--   0        0        0     5825 2020-08-05 03:15:23.012345 python-configuration-0.8.2/config/helpers.py
--rw-r--r--   0        0        0        0 2019-11-21 05:36:35.056467 python-configuration-0.8.2/config/py.typed
--rw-r--r--   0        0        0     1974 2021-01-30 12:27:28.335387 python-configuration-0.8.2/pyproject.toml
--rw-r--r--   0        0        0    11323 2021-01-30 12:33:01.860991 python-configuration-0.8.2/setup.py
--rw-r--r--   0        0        0    11252 2021-01-30 12:33:01.862513 python-configuration-0.8.2/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 23:07:27.752618 python_configuration-0.9.0/LICENSE
+-rw-r--r--   0        0        0    10396 2023-08-05 03:31:32.197905 python_configuration-0.9.0/README.md
+-rw-r--r--   0        0        0    27447 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/__init__.py
+-rw-r--r--   0        0        0    12554 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/configuration.py
+-rw-r--r--   0        0        0     7369 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/configuration_set.py
+-rw-r--r--   0        0        0       43 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/contrib/__init__.py
+-rw-r--r--   0        0        0     4880 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/contrib/aws.py
+-rw-r--r--   0        0        0     5257 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/contrib/azure.py
+-rw-r--r--   0        0        0     5639 2023-08-05 03:31:32.197905 python_configuration-0.9.0/config/contrib/gcp.py
+-rw-r--r--   0        0        0     5965 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/helpers.py
+-rw-r--r--   0        0        0        0 2023-08-04 23:07:27.752618 python_configuration-0.9.0/config/py.typed
+-rw-r--r--   0        0        0     1849 2023-08-05 03:31:32.197905 python_configuration-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0    11610 1970-01-01 00:00:00.000000 python_configuration-0.9.0/PKG-INFO
```

### Comparing `python-configuration-0.8.2/LICENSE` & `python_configuration-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-configuration-0.8.2/README.md` & `python_configuration-0.9.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,72 +1,90 @@
 # python-configuration
 > A library to load configuration parameters hierarchically from multiple sources and formats
 
 [![version](https://img.shields.io/pypi/v/python-configuration)](https://pypi.org/project/python-configuration/)
 ![python](https://img.shields.io/pypi/pyversions/python-configuration)
 ![wheel](https://img.shields.io/pypi/wheel/python-configuration)
 ![license](https://img.shields.io/pypi/l/python-configuration)
-[![build](https://img.shields.io/travis/tr11/python-configuration)](https://travis-ci.org/tr11/python-configuration)
-[![codecov](https://codecov.io/gh/tr11/python-configuration/branch/master/graph/badge.svg)](https://codecov.io/gh/tr11/python-configuration)
+[![tests](https://github.com/tr11/python-configuration/actions/workflows/run_tests.yml/badge.svg)](https://github.com/tr11/python-configuration/actions/workflows/run_tests.yml)
+[![codecov](https://codecov.io/gh/tr11/python-configuration/branch/main/graph/badge.svg?token=5zRYlGnDs7)](https://codecov.io/gh/tr11/python-configuration)
 [![Documentation Status](https://readthedocs.org/projects/python-configuration/badge/?version=latest)](https://python-configuration.readthedocs.io/en/latest/?badge=latest)
 
-This library is intended as a helper mechanism to load configuration files
-hierarchically.  Current format types are:
+This library is intended as a helper mechanism to load configuration files hierarchically.  Supported format types are:
+
 * Python files
 * Dictionaries
 * Environment variables
 * Filesystem paths
 * JSON files
 * INI files
 * dotenv type files
 
 and optionally
+
 * YAML files
 * TOML files
 * Azure Key Vault credentials
 * AWS Secrets Manager credentials
 * GCP Secret Manager credentials
 
 ## Installing
 
 To install the library:
+
 ```shell
 pip install python-configuration
 ```
 
-To include the optional TOML and/or YAML loaders, install the optional
-dependencies `toml` and ` yaml`. For example,
+To include the optional TOML and/or YAML loaders, install the optional dependencies `toml` and ` yaml`. For example,
+
 ```shell
 pip install python-configuration[toml,yaml]
 ```
 
 ## Getting started
 
-This library converts the config types above into dictionaries with 
-dotted-based keys. That is, given a config `cfg` from the structure
-```python
+`python-configuration` converts the various config types into dictionaries with dotted-based keys. For example, given this JSON configuration
+
+```json
 {
-    'a': {
-        'b': 'value'
+    "a": {
+        "b": "value"
     }
 }
 ```
-we are able to refer to the parameter above as any of 
+
+We can use the `config_from_json` method to parse it:
+
+```python
+from config import config_from_json
+
+cfg = config_from_json("my_config_file.json", read_from_file=True)
+```
+
+(Similar methods exist for all the other supported configuration formats (eg. `config_from_toml`, etc.).)
+
+We are then able to refer to the parameters in the config above using any of:
+
 ```python
 cfg['a.b']
 cfg['a']['b']
 cfg['a'].b
 cfg.a.b
 ```
+
 and extract specific data types such as dictionaries:
+
 ```python
 cfg['a'].as_dict == {'b': 'value'}
 ```
+
 This is particularly useful in order to isolate group parameters.
 For example, with the JSON configuration
+
 ```json
 {
   "database.host": "something",
   "database.port": 12345,
   "database.driver": "name",
   "app.debug": true,
   "app.environment": "development",
@@ -74,230 +92,241 @@
   "logging": {
     "service": "service",
     "token": "token",
     "tags": "tags"
   }
 }
 ```
-one can retrieve the dictionaries as 
+
+one can retrieve the dictionaries as
+
 ```python
 cfg.database.as_dict()
 cfg.app.as_dict()
 cfg.logging.as_dict()
 ```
-or simply as 
+
+or simply as
+
 ```python
 dict(cfg.database)
 dict(cfg.app)
 dict(cfg.logging)
 ```
+
 ## Configuration
-There are two general types of objects in this library. The first one is the `Configuration`,
-which represents a single config source.  The second is a `ConfigurationSet` that allows for
-multiple `Configuration` objects to be specified.
+
+There are two general types of objects in this library. The first one is the `Configuration`, which represents a single config source.  The second is a `ConfigurationSet` that allows for multiple `Configuration` objects to be specified.
 
 ### Single Config
 
 #### Python Files
+
 To load a configuration from a Python module, the `config_from_python` can be used.
 The first parameter must be a Python module and can be specified as an absolute path to the Python file or as an importable module.
 
-Optional parameters are the `prefix` and `separator`.  The following call 
+Optional parameters are the `prefix` and `separator`.  The following call
+
 ```python
 config_from_python('foo.bar', prefix='CONFIG', separator='__')
 ```
-will read every variable in the `foo.bar` module that starts with `CONFIG__` and replace
-every occurrence of `__` with a `.`. For example,
+
+will read every variable in the `foo.bar` module that starts with `CONFIG__` and replace every occurrence of `__` with a `.`. For example,
+
 ```python
 # foo.bar
 CONFIG__AA__BB_C = 1
 CONFIG__AA__BB__D = 2
 CONF__AA__BB__D = 3
 ```
+
 would result in the configuration
+
 ```python
 {
     'aa.bb_c': 1,
     'aa.bb.d': 2,
 }
 ```
-Note that the single underscore in `BB_C` is not replaced and the last line is not
-prefixed by `CONFIG`. 
+
+Note that the single underscore in `BB_C` is not replaced and the last line is not prefixed by `CONFIG`.
 
 #### Dictionaries
-Dictionaries are loaded with `config_from_dict` and are converted internally to a 
-flattened `dict`. 
+
+Dictionaries are loaded with `config_from_dict` and are converted internally to a flattened `dict`.
+
 ```python
 {
     'a': {
         'b': 'value'
     }
 }
 ```
+
 becomes
+
 ```python
 {
     'a.b': 'value'
 }
 ```
 
 #### Environment Variables
+
 Environment variables starting with `prefix` can be read with `config_from_env`:
+
 ```python
 config_from_env(prefix, separator='_')
 ```
 
 #### Filesystem Paths
-Folders with files named as `xxx.yyy.zzz` can be loaded with the `config_from_path` function.  This format is useful to load mounted
-Kubernetes [ConfigMaps](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/#populate-a-volume-with-data-stored-in-a-configmap)
-or [Secrets](https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#create-a-pod-that-has-access-to-the-secret-data-through-a-volume).
+
+Folders with files named as `xxx.yyy.zzz` can be loaded with the `config_from_path` function.  This format is useful to load mounted Kubernetes [ConfigMaps](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/#populate-a-volume-with-data-stored-in-a-configmap) or [Secrets](https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#create-a-pod-that-has-access-to-the-secret-data-through-a-volume).
 
 #### JSON, INI, .env, YAML, TOML
+
 JSON, INI, YAML, TOML files are loaded respectively with
 `config_from_json`,
 `config_from_ini`,
 `config_from_dotenv`,
 `config_from_yaml`, and
 `config_from_toml`.
-The parameter `read_from_file` controls
-whether a string should be interpreted as a filename.
+The parameter `read_from_file` controls whether a string should be interpreted as a filename.
 
 ###### Caveats
-In order for `Configuration` objects to act as `dict` and allow the syntax
-`dict(cfg)`, the `keys()` method is implemented as the typical `dict` keys.
-If `keys` is an element in the configuration `cfg` then the `dict(cfg)` call will fail.
-In that case, it's necessary to use the `cfg.as_dict()` method to retrieve the
-`dict` representation for the `Configuration` object.
+
+In order for `Configuration` objects to act as `dict` and allow the syntax `dict(cfg)`, the `keys()` method is implemented as the typical `dict` keys. If `keys` is an element in the configuration `cfg` then the `dict(cfg)` call will fail. In that case, it's necessary to use the `cfg.as_dict()` method to retrieve the `dict` representation for the `Configuration` object.
 
 The same applies to the methods `values()` and `items()`.
- 
+
 
 ### Configuration Sets
-Configuration sets are used to hierarchically load configurations and merge
-settings. Sets can be loaded by constructing a `ConfigurationSet` object directly or
-using the simplified `config` function.
+
+Configuration sets are used to hierarchically load configurations and merge settings. Sets can be loaded by constructing a `ConfigurationSet` object directly or using the simplified `config` function.
 
 To construct a `ConfigurationSet`, pass in as many of the simple `Configuration` objects as needed:
+
 ```python
 cfg = ConfigurationSet(
     config_from_env(prefix=PREFIX),
     config_from_json(path, read_from_file=True),
     config_from_dict(DICT),
 )
 ```
-The example above will read first from Environment variables prefixed with `PREFIX`, 
-and fallback first to the JSON file at `path`, and finally use the dictionary `DICT`.
+The example above will read first from Environment variables prefixed with `PREFIX`, and fallback first to the JSON file at `path`, and finally use the dictionary `DICT`.
 
 The `config` function simplifies loading sets by assuming some defaults.
 The example above can also be obtained by
+
 ```python
 cfg = config(
     ('env', PREFIX),
     ('json', path, True),
     ('dict', DICT),
 )
 ```
+
 or, even simpler if `path` points to a file with a `.json` suffix:
+
 ```python
 cfg = config('env', path, DICT, prefix=PREFIX)
 ```
+
 The `config` function automatically detects the following:
+
 * extension `.py` for python modules
 * dot-separated python identifiers as a python module (e.g. `foo.bar`)
 * extension `.json` for JSON files
 * extension `.yaml` for YAML files
 * extension `.toml` for TOML files
 * extension `.ini` for INI files
 * extension `.env` for dotenv type files
 * filesystem folders as Filesystem Paths
 * the strings `env` or `environment` for Environment Variables
 
 #### Merging Values
+
 `ConfigurationSet` instances are constructed by inspecting each configuration source, taking into account nested dictionaries, and merging at the most granular level.
 For example, the instance obtained from `cfg = config(d1, d2)` for the dictionaries below
 
 ```python
 d1 = {'sub': {'a': 1, 'b': 4}}
 d2 = {'sub': {'b': 2, 'c': 3}}
 ```
 
 is such that `cfg['sub']` equals
 
 ```python
 {'a': 1, 'b': 4, 'c': 3}
 ```
 
-Note that the nested dictionaries of `'sub'` in each of `d1` and `d2` do not overwrite each other, but are merged into a single
-dictionary with keys from both `d1` and `d2`, giving priority to the values of `d1` over those from `d2`.
+Note that the nested dictionaries of `'sub'` in each of `d1` and `d2` do not overwrite each other, but are merged into a single dictionary with keys from both `d1` and `d2`, giving priority to the values of `d1` over those from `d2`.
 
 
 ###### Caveats
-As long as the data types are consistent across all the configurations that are
-part of a `ConfigurationSet`, the behavior should be straightforward.  When different
-configuration objects are specified with competing data types, the first configuration to
-define the elements sets its datatype. For example, if in the example above 
-`element` is interpreted as a `dict` from environment variables, but the 
-JSON file specifies it as anything else besides a mapping, then the JSON value will be
-dropped automatically. 
+
+As long as the data types are consistent across all the configurations that are part of a `ConfigurationSet`, the behavior should be straightforward.  When different configuration objects are specified with competing data types, the first configuration to define the elements sets its datatype. For example, if in the example above `element` is interpreted as a `dict` from environment variables, but the JSON file specifies it as anything else besides a mapping, then the JSON value will be dropped automatically.
 
 ## Other Features
 
 ###### String Interpolation
-When setting the `interpolate` parameter in any `Configuration` instance, the library will
-perform a string interpolation step using the [str.format](https://docs.python.org/3/library/string.html#formatstrings)
-syntax.  In particular, this allows to format configuration values automatically:
+
+When setting the `interpolate` parameter in any `Configuration` instance, the library will perform a string interpolation step using the [str.format](https://docs.python.org/3/library/string.html#formatstrings) syntax.  In particular, this allows to format configuration values automatically:
+
 ```python
 cfg = config_from_dict({
     "percentage": "{val:.3%}",
     "with_sign": "{val:+f}",
     "val": 1.23456}, interpolate=True)
 
 assert cfg.val == 1.23456
 assert cfg.with_sign == "+1.234560"
 assert cfg.percentage == "123.456%"
 ```
 
 ## Extras
-The `config.contrib` package contains extra implementations of the `Configuration` class
-used for special cases. Currently the following are implemented:
+
+The `config.contrib` package contains extra implementations of the `Configuration` class used for special cases. Currently the following are implemented:
+
 * `AzureKeyVaultConfiguration` in `config.contrib.azure`, which takes Azure Key Vault
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
+
   ```shell
   pip install python-configuration[azure]
   ```
+
 * `AWSSecretsManagerConfiguration` in `config.contrib.aws`, which takes AWS Secrets Manager
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
+
   ```shell
   pip install python-configuration[aws]
   ```
+
 * `GCPSecretManagerConfiguration` in `config.contrib.gcp`, which takes GCP Secret Manager
   credentials into a `Configuration`-compatible instance. To install the needed dependencies
   execute
+
   ```shell
   pip install python-configuration[gcp]
   ```
 
-## Developing
-
-To develop this library, download the source code and install a local version.
-
-
 ## Features
 
 * Load multiple configuration types
 * Hierarchical configuration
 * Ability to override with environment variables
 * Merge parameters from different configuration types
 
-## Contributing
+## Contributing :tada:
+
+If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are welcome.
 
-If you'd like to contribute, please fork the repository and use a feature
-branch. Pull requests are welcome.
+See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the details.
 
 ## Links
 
 - Repository: https://github.com/tr11/python-configuration
 - Issue tracker: https://github.com/tr11/python-configuration/issues
 - Documentation: https://python-configuration.readthedocs.io
```

### Comparing `python-configuration-0.8.2/config/__init__.py` & `python_configuration-0.9.0/config/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """python-configuration module."""
 
 import json
 import os
 from importlib.abc import InspectLoader
 from types import ModuleType
-from typing import Any, Dict, Iterable, List, Optional, TextIO, Union, cast
+from typing import Any, Dict, Iterable, List, Mapping, Optional, TextIO, Union, cast
 
 try:
     import yaml
 except ImportError:  # pragma: no cover
-    yaml = None  # type: ignore
+    yaml = None
 try:
     import toml
 except ImportError:  # pragma: no cover
-    toml = None  # type: ignore
+    toml = None
 
 
 from .configuration import Configuration
 from .configuration_set import ConfigurationSet
 from .helpers import InterpolateEnumType, InterpolateType
 
 
@@ -56,15 +56,15 @@
         "lowercase_keys": lowercase_keys,
         # for Configuration Sets, interpolate parameters should be at the Set level
         "interpolate": False,
         "interpolate_type": InterpolateEnumType.STANDARD,
     }
 
     for config_ in configs:
-        if isinstance(config_, dict):
+        if isinstance(config_, Mapping):
             instances.append(config_from_dict(config_, **default_kwargs))
             continue
         elif isinstance(config_, str):
             if config_.endswith(".py"):
                 config_ = ("python", config_, *default_args)
             elif config_.endswith(".json"):
                 config_ = ("json", config_, True)
@@ -79,15 +79,15 @@
             elif os.path.isdir(config_):
                 config_ = ("path", config_, remove_level)
             elif config_ in ("env", "environment"):
                 config_ = ("env", *default_args)
             elif all(s and s.isidentifier() for s in config_.split(".")):
                 config_ = ("python", config_, *default_args)
             else:
-                raise ValueError('Cannot determine config type from "%s"' % config_)
+                raise ValueError(f'Cannot determine config type from "{config_}"')
 
         if not isinstance(config_, (tuple, list)) or len(config_) == 0:
             raise ValueError(
                 "configuration parameters must be a list of dictionaries,"
                 " strings, or non-empty tuples/lists"
             )
         type_ = config_[0]
@@ -138,15 +138,15 @@
         elif type_ == "path":
             try:
                 instances.append(config_from_path(*config_[1:], **default_kwargs))
             except FileNotFoundError:
                 if not ignore_missing_paths:
                     raise
         else:
-            raise ValueError('Unknown configuration type "%s"' % type_)
+            raise ValueError(f'Unknown configuration type "{type_}"')
 
     return ConfigurationSet(
         *instances, interpolate=interpolate, interpolate_type=interpolate_type
     )
 
 
 class EnvConfiguration(Configuration):
@@ -318,15 +318,15 @@
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
     ):
         """
         Constructor.
 
-        :param data: path to a JSON file or contents
+        :param data: path to a config file, or its contents
         :param read_from_file: whether to read from a file path or to interpret
                the :attr:`data` as the contents of the file.
         :param lowercase_keys: whether to convert every key to lower case.
         """
         super().__init__(
             {},
             lowercase_keys=lowercase_keys,
@@ -388,38 +388,65 @@
         interpolate_type=interpolate_type,
     )
 
 
 class INIConfiguration(FileConfiguration):
     """Configuration from an INI file input."""
 
+    def __init__(
+        self,
+        data: Union[str, TextIO],
+        read_from_file: bool = False,
+        *,
+        section_prefix: str = "",
+        lowercase_keys: bool = False,
+        interpolate: InterpolateType = False,
+        interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ):
+        self._section_prefix = section_prefix
+        super().__init__(
+            data=data,
+            read_from_file=read_from_file,
+            lowercase_keys=lowercase_keys,
+            interpolate=interpolate,
+            interpolate_type=interpolate_type,
+        )
+
     def _reload(self, data: Union[str, TextIO], read_from_file: bool = False) -> None:
         """Reload the INI data."""
         import configparser
 
+        lowercase = self._lowercase
+
+        class ConfigParser(configparser.RawConfigParser):
+            def optionxform(self, optionstr: str) -> str:
+                return super().optionxform(optionstr) if lowercase else optionstr
+
         if read_from_file:
             if isinstance(data, str):
                 data = open(data, "rt").read()
             else:
                 data = data.read()
         data = cast(str, data)
-        cfg = configparser.RawConfigParser()
+        cfg = ConfigParser()
         cfg.read_string(data)
         result = {
-            section + "." + k: v
+            section[len(self._section_prefix) :] + "." + k: v
             for section, values in cfg.items()
             for k, v in values.items()
+            if section.startswith(self._section_prefix)
         }
         self._config = self._flatten_dict(result)
 
 
 def config_from_ini(
     data: Union[str, TextIO],
     read_from_file: bool = False,
     *,
+    section_prefix: str = "",
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from an INI file.
 
@@ -429,42 +456,79 @@
     :param lowercase_keys: whether to convert every key to lower case.
     :param interpolate: whether to apply string interpolation when looking for items
     :return: a :class:`Configuration` instance
     """
     return INIConfiguration(
         data,
         read_from_file,
+        section_prefix=section_prefix,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
     )
 
 
 class DotEnvConfiguration(FileConfiguration):
     """Configuration from a .env type file input."""
 
-    def _reload(self, data: Union[str, TextIO], read_from_file: bool = False) -> None:
+    def __init__(
+        self,
+        data: Union[str, TextIO],
+        read_from_file: bool = False,
+        prefix: str = "",
+        separator: str = "__",
+        *,
+        lowercase_keys: bool = False,
+        interpolate: InterpolateType = False,
+        interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+    ):
+        self._prefix = prefix
+        self._separator = separator
+        super().__init__(
+            data=data,
+            read_from_file=read_from_file,
+            lowercase_keys=lowercase_keys,
+            interpolate=interpolate,
+            interpolate_type=interpolate_type,
+        )
+
+    def _reload(
+        self,
+        data: Union[str, TextIO],
+        read_from_file: bool = False,
+    ) -> None:
         """Reload the .env data."""
         if read_from_file:
             if isinstance(data, str):
                 data = open(data, "rt").read()
             else:
                 data = data.read()
         data = cast(str, data)
         result: Dict[str, Any] = dict(
             (y.strip() for y in x.split("=", 1))  # type: ignore
             for x in data.splitlines()
             if x
         )
+
+        result = {
+            k[len(self._prefix) :].replace(self._separator, ".").strip("."): v
+            for k, v in result.items()
+            if k.startswith(self._prefix)
+        }
+
+        print(self._prefix, self._separator, result)
+
         self._config = self._flatten_dict(result)
 
 
 def config_from_dotenv(
     data: Union[str, TextIO],
     read_from_file: bool = False,
+    prefix: str = "",
+    separator: str = "__",
     *,
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from a .env type file.
@@ -475,14 +539,16 @@
     :param lowercase_keys: whether to convert every key to lower case.
     :param interpolate: whether to apply string interpolation when looking for items
     :return: a :class:`Configuration` instance
     """
     return DotEnvConfiguration(
         data,
         read_from_file,
+        prefix=prefix,
+        separator=separator,
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
     )
 
 
 class PythonConfiguration(Configuration):
@@ -505,16 +571,20 @@
         :param prefix: prefix to use to filter object names
         :param separator: separator to replace by dots
         :param lowercase_keys: whether to convert every key to lower case.
         """
         if isinstance(module, str):
             if module.endswith(".py"):
                 import importlib.util
+                from importlib import machinery
 
-                spec = importlib.util.spec_from_file_location(module, module)
+                spec = cast(
+                    machinery.ModuleSpec,
+                    importlib.util.spec_from_file_location(module, module),
+                )
                 module = importlib.util.module_from_spec(spec)
                 spec.loader = cast(InspectLoader, spec.loader)
                 spec.loader.exec_module(module)
             else:
                 import importlib
 
                 module = importlib.import_module(module)
@@ -576,15 +646,15 @@
         lowercase_keys=lowercase_keys,
         interpolate=interpolate,
         interpolate_type=interpolate_type,
     )
 
 
 def config_from_dict(
-    data: dict,
+    data: Mapping,
     *,
     lowercase_keys: bool = False,
     interpolate: InterpolateType = False,
     interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
 ) -> Configuration:
     """
     Create a :class:`Configuration` instance from a dictionary.
@@ -634,15 +704,15 @@
             self, data: Union[str, TextIO], read_from_file: bool = False
         ) -> None:
             """Reload the YAML data."""
             if read_from_file and isinstance(data, str):
                 loaded = yaml.load(open(data, "rt"), Loader=yaml.FullLoader)
             else:
                 loaded = yaml.load(data, Loader=yaml.FullLoader)
-            if not isinstance(loaded, dict):
+            if not isinstance(loaded, Mapping):
                 raise ValueError("Data should be a dictionary")
             self._config = self._flatten_dict(loaded)
 
     def config_from_yaml(
         data: Union[str, TextIO],
         read_from_file: bool = False,
         *,
@@ -669,33 +739,60 @@
 
 
 if toml is not None:  # pragma: no branch
 
     class TOMLConfiguration(FileConfiguration):
         """Configuration from a TOML input."""
 
+        def __init__(
+            self,
+            data: Union[str, TextIO],
+            read_from_file: bool = False,
+            *,
+            section_prefix: str = "",
+            lowercase_keys: bool = False,
+            interpolate: InterpolateType = False,
+            interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
+        ):
+            self._section_prefix = section_prefix
+            super().__init__(
+                data=data,
+                read_from_file=read_from_file,
+                lowercase_keys=lowercase_keys,
+                interpolate=interpolate,
+                interpolate_type=interpolate_type,
+            )
+
         def _reload(
             self, data: Union[str, TextIO], read_from_file: bool = False
         ) -> None:
             """Reload the TOML data."""
             if read_from_file:
                 if isinstance(data, str):
                     loaded = toml.load(open(data, "rt"))
                 else:
                     loaded = toml.load(data)
             else:
                 data = cast(str, data)
                 loaded = toml.loads(data)
             loaded = cast(dict, loaded)
-            self._config = self._flatten_dict(loaded)
+
+            result = {
+                k[len(self._section_prefix) :]: v
+                for k, v in self._flatten_dict(loaded).items()
+                if k.startswith(self._section_prefix)
+            }
+
+            self._config = result
 
     def config_from_toml(
         data: Union[str, TextIO],
         read_from_file: bool = False,
         *,
+        section_prefix: str = "",
         lowercase_keys: bool = False,
         interpolate: InterpolateType = False,
         interpolate_type: InterpolateEnumType = InterpolateEnumType.STANDARD,
     ) -> Configuration:
         """
         Return a Configuration instance from TOML files.
 
@@ -704,11 +801,12 @@
         :param lowercase_keys: whether to convert every key to lower case.
         :param interpolate: whether to apply string interpolation when looking for items
         :return: a Configuration instance
         """
         return TOMLConfiguration(
             data,
             read_from_file,
+            section_prefix=section_prefix,
             lowercase_keys=lowercase_keys,
             interpolate=interpolate,
             interpolate_type=interpolate_type,
         )
```

### Comparing `python-configuration-0.8.2/config/configuration.py` & `python_configuration-0.9.0/config/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,14 +65,16 @@
         self._interpolate = {} if interpolate is True else interpolate
         self._interpolate_type = interpolate_type
         self._config: Dict[str, Any] = self._flatten_dict(config_)
         self._default_levels: Optional[int] = 1
 
     def __eq__(self, other):  # type: ignore
         """Equality operator."""
+        if not isinstance(other, (Configuration, Mapping)):
+            return False
         return self.as_dict() == Configuration(other).as_dict()
 
     def _filter_dict(self, d: Dict[str, Any], prefix: str) -> Dict[str, Any]:
         """
         Filter a dictionary and return the items that are prefixed by :attr:`prefix`.
 
         :param d: dictionary
@@ -95,34 +97,36 @@
     def _flatten_dict(self, d: Mapping[str, Any]) -> Dict[str, Any]:
         """
         Flatten one level of a dictionary.
 
         :param d: dict
         :return: a flattened dict
         """
-        nested = {k for k, v in d.items() if isinstance(v, (dict, Configuration))}
+        nested = {k for k, v in d.items() if isinstance(v, (Mapping, Configuration))}
         if self._lowercase:
             result = {
                 k.lower() + "." + ki: vi
                 for k in nested
                 for ki, vi in self._flatten_dict(d[k]).items()
             }
             result.update(
                 (k.lower(), v)
                 for k, v in d.items()
-                if not isinstance(v, (dict, Configuration))
+                if not isinstance(v, (Mapping, Configuration))
             )
         else:
             result = {
                 k + "." + ki: vi
                 for k in nested
                 for ki, vi in self._flatten_dict(d[k]).items()
             }
             result.update(
-                (k, v) for k, v in d.items() if not isinstance(v, (dict, Configuration))
+                (k, v)
+                for k, v in d.items()
+                if not isinstance(v, (Mapping, Configuration))
             )
         return result
 
     def _get_subset(self, prefix: str) -> Union[Dict[str, Any], Any]:
         """
         Return the subset of the config dictionary whose keys start with :attr:`prefix`.
 
@@ -149,19 +153,19 @@
         return deepcopy(d)
 
     def __getitem__(self, item: str) -> Union["Configuration", Any]:  # noqa: D105
         v = self._get_subset(item)
 
         if v == {}:
             raise KeyError(item)
-        if isinstance(v, dict):
+        if isinstance(v, Mapping):
             return Configuration(v)
         elif self._interpolate is not False:
             d = self.as_dict()
-            d.update(cast(Dict[str, str], self._interpolate))
+            d.update(self._interpolate)
             return interpolate_object(item, v, [d], self._interpolate_type)
         else:
             return v
 
     def __getattr__(self, item: str) -> Any:  # noqa: D105
         try:
             return self[item]
@@ -182,15 +186,15 @@
         """Return the representation as a dictionary."""
         return self._config
 
     def as_attrdict(self) -> AttributeDict:
         """Return the representation as an attribute dictionary."""
         return AttributeDict(
             {
-                x: Configuration(v).as_attrdict() if isinstance(v, dict) else v
+                x: Configuration(v).as_attrdict() if isinstance(v, Mapping) else v
                 for x, v in self.items(levels=1)
             }
         )
 
     def get_bool(self, item: str) -> bool:
         """
         Get the item value as a bool.
@@ -303,17 +307,15 @@
             return {k: self._get_subset(k) for k in keys}.items()
 
     def __iter__(self) -> Iterator[Tuple[str, Any]]:  # noqa: D105
         return iter(dict(self.items()))  # type: ignore
 
     def __reversed__(self) -> Iterator[Tuple[str, Any]]:  # noqa: D105
         if version_info < (3, 8):
-            return OrderedDict(  # type: ignore
-                reversed(list(self.items()))
-            )  # pragma: no cover
+            return OrderedDict(reversed(list(self.items())))  # type: ignore  # pragma: no cover
         else:
             return reversed(dict(self.items()))  # type: ignore
 
     def __len__(self) -> int:  # noqa: D105
         return len(self.keys())
 
     def __setitem__(self, key: str, value: Any) -> None:  # noqa: D105
@@ -400,11 +402,11 @@
         self._default_levels = None
         try:
             yield self
         finally:
             self._default_levels = 1
 
     def __repr__(self) -> str:  # noqa: D105
-        return "<Configuration: %s>" % hex(id(self))
+        return "<%s: %s>" % (type(self).__name__, hex(id(self)))
 
     def __str__(self) -> str:  # noqa: D105
         return str({k: clean(k, v) for k, v in sorted(self.as_dict().items())})
```

### Comparing `python-configuration-0.8.2/config/configuration_set.py` & `python_configuration-0.9.0/config/configuration_set.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             for v in values[::-1]:
                 if not isinstance(v, Configuration):
                     continue
                 result.update(v)
             return Configuration(result)
         elif self._interpolate is not False:
             d = [d.as_dict() for d in self._configs]
-            d[0].update(cast(Dict[str, str], self._interpolate))
+            d[0].update(self._interpolate)
             return interpolate_object(args[0], values[0], d, self._interpolate_type)
         else:
             return values[0]
 
     def _writable_config(self) -> Configuration:
         if not self._writable:
             lowercase = bool(self._configs and self._configs[0]._lowercase)
```

### Comparing `python-configuration-0.8.2/config/contrib/aws.py` & `python_configuration-0.9.0/config/contrib/aws.py`

 * *Files identical despite different names*

### Comparing `python-configuration-0.8.2/config/contrib/azure.py` & `python_configuration-0.9.0/config/contrib/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 import time
 from typing import Any, Dict, ItemsView, KeysView, Optional, Union, ValuesView, cast
 
 from azure.core.exceptions import ResourceNotFoundError
 from azure.identity import ClientSecretCredential
 from azure.keyvault.secrets import SecretClient
 
+
 from .. import Configuration, InterpolateType
 
 
 class Cache:
     """Cache class."""
 
-    def __init__(self, value: str, ts: float):  # noqa: D107
+    def __init__(self, value: Optional[str], ts: float):  # noqa: D107
         self.value = value
         self.ts = ts
 
 
 class AzureKeyVaultConfiguration(Configuration):
     """
     Azure Configuration class.
@@ -51,17 +52,15 @@
         :param cache_expiration: Cache expiration (in seconds)
         """
         credentials = ClientSecretCredential(
             client_id=az_client_id,
             client_secret=az_client_secret,
             tenant_id=az_tenant_id,
         )
-        vault_url = "https://{az_vault_name}.vault.azure.net/".format(
-            az_vault_name=az_vault_name
-        )
+        vault_url = f"https://{az_vault_name}.vault.azure.net/"
         self._kv_client = SecretClient(vault_url=vault_url, credential=credentials)
         self._cache_expiration = cache_expiration
         self._cache: Dict[str, Cache] = {}
         self._interpolate = {} if interpolate is True else interpolate
         self._default_levels = None
 
     def _get_secret(self, key: str) -> Optional[str]:
@@ -69,15 +68,15 @@
         now = time.time()
         from_cache = self._cache.get(key)
         if from_cache and from_cache.ts + self._cache_expiration > now:
             return from_cache.value
         try:
             secret = self._kv_client.get_secret(key)
             self._cache[key] = Cache(value=secret.value, ts=now)
-            return cast(str, secret.value)
+            return secret.value
         except ResourceNotFoundError:
             if key in self._cache:
                 del self._cache[key]
             return None
 
     def __getitem__(self, item: str) -> Any:  # noqa: D105
         secret = self._get_secret(item)
@@ -121,35 +120,35 @@
         self, levels: Optional[int] = None
     ) -> Union["Configuration", Any, ValuesView[Any]]:
         """Return a set-like object providing a view on the configuration values."""
         assert not levels  # Azure Key Vaults don't support separators
         return cast(
             ValuesView[str],
             (
-                self._get_secret(k.name)
+                self._get_secret(cast(str, k.name))
                 for k in self._kv_client.list_properties_of_secrets()
             ),
         )
 
     def items(
         self, levels: Optional[int] = None
     ) -> Union["Configuration", Any, ItemsView[str, Any]]:
         """Return a set-like object providing a view on the configuration items."""
         assert not levels  # Azure Key Vaults don't support separators
         return cast(
             ItemsView[str, Any],
             (
-                (k.name, self._get_secret(k.name))
+                (k.name, self._get_secret(cast(str, k.name)))
                 for k in self._kv_client.list_properties_of_secrets()
             ),
         )
 
     def reload(self) -> None:
         """Reload the configuration."""
         self._cache.clear()
 
     def __repr__(self) -> str:  # noqa: D105
-        return "<AzureKeyVaultConfiguration: %r>" % self._kv_client.vault_url
+        return f"<AzureKeyVaultConfiguration: {repr(self._kv_client.vault_url)}>"
 
     @property
     def _config(self) -> Dict[str, Any]:  # type: ignore
         return dict(self.items())
```

### Comparing `python-configuration-0.8.2/config/contrib/gcp.py` & `python_configuration-0.9.0/config/contrib/gcp.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import time
 from typing import Any, Dict, ItemsView, KeysView, Optional, Union, ValuesView, cast
 
 from google.api_core.client_options import ClientOptions
 from google.api_core.exceptions import NotFound
 from google.auth.credentials import Credentials
-from google.cloud import secretmanager
+from google.cloud import secretmanager_v1
 
 from .. import Configuration, InterpolateType
 
 
 class Cache:
     """Cache class."""
 
@@ -33,49 +33,51 @@
         - values must be strings.
     """
 
     def __init__(
         self,
         project_id: str,
         credentials: Credentials = None,
-        client_options: ClientOptions = None,
+        client_options: Optional[ClientOptions] = None,
         cache_expiration: int = 5 * 60,
         interpolate: InterpolateType = False,
     ) -> None:
         """
         Constructor.
 
         See https://googleapis.dev/python/secretmanager/latest/gapic/v1/api.html#google.cloud.secretmanager_v1.SecretManagerServiceClient
         for more details on credentials and options.
 
         :param project_id: GCP Project ID
         :param credentials: GCP credentials
         :param client_options: GCP client_options
         :param cache_expiration: Cache expiration (in seconds)
         """  # noqa: E501
-        self._client = secretmanager.SecretManagerServiceClient(
+        self._client = secretmanager_v1.SecretManagerServiceClient(
             credentials=credentials, client_options=client_options
         )
         self._project_id = project_id
-        self._parent = self._client.project_path(project_id)
+        self._parent = f"projects/{project_id}"
         self._cache_expiration = cache_expiration
         self._cache: Dict[str, Cache] = {}
         self._interpolate = {} if interpolate is True else interpolate
         self._default_levels = None
 
     def _get_secret(self, key: str) -> Optional[str]:
         now = time.time()
         from_cache = self._cache.get(key)
         if from_cache and from_cache.ts + self._cache_expiration > now:
             return from_cache.value
         try:
-            path = self._client.secret_version_path(self._project_id, key, "latest")
-            secret = self._client.access_secret_version(path).payload.data.decode()
+            path = f"projects/{self._project_id}/secrets/{key}/versions/latest"
+            secret = self._client.access_secret_version(
+                request={"name": path}
+            ).payload.data.decode()
             self._cache[key] = Cache(value=secret, ts=now)
-            return cast(str, secret)
+            return secret
         except NotFound:
             if key in self._cache:
                 del self._cache[key]
             return None
 
     def __getitem__(self, item: str) -> Any:  # noqa: D105
         secret = self._get_secret(item)
@@ -108,40 +110,43 @@
     def keys(
         self, levels: Optional[int] = None
     ) -> Union["Configuration", Any, KeysView[str]]:
         """Return a set-like object providing a view on the configuration keys."""
         assert not levels  # GCP Secret Manager secrets don't support separators
         return cast(
             KeysView[str],
-            (k.name.split("/")[-1] for k in self._client.list_secrets(self._parent)),
+            (
+                k.name.split("/")[-1]
+                for k in self._client.list_secrets(request={"parent": self._parent})
+            ),
         )
 
     def values(
         self, levels: Optional[int] = None
     ) -> Union["Configuration", Any, ValuesView[Any]]:
         """Return a set-like object providing a view on the configuration values."""
         assert not levels  # GCP Secret Manager secrets don't support separators
         return cast(
             ValuesView[str],
             (
                 self._get_secret(k.name.split("/")[-1])
-                for k in self._client.list_secrets(self._parent)
+                for k in self._client.list_secrets(request={"parent": self._parent})
             ),
         )
 
     def items(
         self, levels: Optional[int] = None
     ) -> Union["Configuration", Any, ItemsView[str, Any]]:
         """Return a set-like object providing a view on the configuration items."""
         assert not levels  # GCP Secret Manager secrets don't support separators
         return cast(
             ItemsView[str, Any],
             (
                 (k.name.split("/")[-1], self._get_secret(k.name.split("/")[-1]))
-                for k in self._client.list_secrets(self._parent)
+                for k in self._client.list_secrets(request={"parent": self._parent})
             ),
         )
 
     def reload(self) -> None:
         """Reload the configuration."""
         self._cache.clear()
```

### Comparing `python-configuration-0.8.2/config/helpers.py` & `python_configuration-0.9.0/config/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import string
 from enum import Enum
 from typing import Any, Dict, List, Set, Tuple, Union
 
 
 TRUTH_TEXT = frozenset(("t", "true", "y", "yes", "on", "1"))
 FALSE_TEXT = frozenset(("f", "false", "n", "no", "off", "0", ""))
-PROTECTED_KEYS = frozenset(("secret", "password", "passwd", "pwd"))
+PROTECTED_KEYS = frozenset(("secret", "password", "passwd", "pwd", "token"))
 
 InterpolateType = Union[bool, Dict[str, str]]
 
 
 class InterpolateEnumType(Enum):
     """Interpolation Method."""
 
@@ -194,10 +194,13 @@
             InterpolateEnumType.DEEP,
             InterpolateEnumType.DEEP_NO_BACKTRACK,
         ):
             return interpolate_deep(attr, obj, d, {}, {}, method)
         else:
             raise ValueError('Invalid interpolation method "%s"' % method)
     elif hasattr(obj, "__iter__"):
-        return [interpolate_object(attr, x, d, method) for x in obj]
+        if isinstance(obj, tuple):
+            return tuple(interpolate_object(attr, x, d, method) for x in obj)
+        else:
+            return [interpolate_object(attr, x, d, method) for x in obj]
     else:
         return obj
```

### Comparing `python-configuration-0.8.2/pyproject.toml` & `python_configuration-0.9.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,44 +5,43 @@
 include = ["config/py.typed"]
 keywords = ['configuration', 'settings', 'json', 'yaml', 'toml', 'ini']
 license = "MIT"
 name = "python-configuration"
 packages = [{ include = "config" }]
 readme = 'README.md'
 repository = "https://github.com/tr11/python-configuration"
-version = "0.8.2"
+version = "0.9.0"
 
 [tool.poetry.dependencies]
-azure-identity = { version = "^1.5.0", optional = true }
-azure-keyvault = { version = "^4.0.0", optional = true }
-boto3 = { version = "^1.10.48", optional = true }
-google-cloud-secret-manager = { version = "^2.0.0", optional = true }
-python = "^3.6"
-pyyaml = { version = "^5.1", optional = true }
+python = "^3.8.1"
+azure-identity = { version = "^1.13.0", optional = true }
+azure-keyvault = { version = "^4.2.0", optional = true }
+boto3 = { version = "^1.28.20", optional = true }
+google-cloud-secret-manager = { version = "^2.16.3", optional = true }
+pyyaml = { version = "^6.0", optional = true }
 toml = { version = "^0.10.0", optional = true }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 flake8-blind-except = "^0.2.0"
-flake8-bugbear = "^20.11"
-flake8-builtins = "^1.4"
+flake8-bugbear = "^23.7.10"
+flake8-builtins = "^2.1.0"
 flake8-comprehensions = "^3.3.1"
 flake8-docstrings = "^1.3"
 flake8-import-order = "^0.18.0"
-mypy = "^0.800"
-pydocstyle = "^4.0"
-pytest = "^6.2.1"
-pytest-black = "^0.3.7"
-pytest-cov = "^2.6"
-pytest-flake8 = "^1.0"
-pytest-mypy = "^0.8.0"
+mypy = "^1.4.1"
+pydocstyle = "^6.0"
+pytest = "^7.4.0"
+pytest-black = "^0.3.12"
+pytest-cov = "^4.1.0"
+pytest-flake8 = "^1.1.1"
+pytest-mypy = "^0.10.3"
 pytest-mock = "^3.5.0"
-sphinx = "^3.4"
-sphinx-autodoc-typehints = "^1.11.0"
-# need to allow pre-releases to address a recent change in pytest-black. See https://github.com/shopkeep/pytest-black/issues/45
-black = { version = "*", allow-prereleases = true }
+sphinx = "^7.1.2"
+sphinx-autodoc-typehints = "^1.24.0"
+black = "^23.7.0"
 
 [tool.poetry.extras]
 aws = ["boto3"]
 azure = ["azure-keyvault", "azure-identity"]
 gcp = ["google-cloud-secret-manager"]
 toml = ["toml"]
 yaml = ["pyyaml"]
@@ -50,19 +49,19 @@
 [tool.black]
 line-length = 88
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 isolated_build = true
-envlist = py36, py37, py38
+envlist = py38, py39, py310, py311
 
 [testenv]
-whitelist_externals = poetry
+allowlist_externals = poetry
 commands =
-    poetry install -v -E toml -E yaml -E azure -E aws
+    poetry install -v -E toml -E yaml -E azure -E aws -E gcp
     poetry run pytest
 """
 
 [build-system]
 build-backend = "poetry.masonry.api"
-requires = ["poetry>=1.1.4"]
+requires = ["poetry>=1.5.0"]
```

### Comparing `python-configuration-0.8.2/setup.py` & `python_configuration-0.9.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,365 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: python-configuration
+Version: 0.9.0
+Summary: A library to load configuration parameters from multiple sources and formats
+Home-page: https://github.com/tr11/python-configuration
+License: MIT
+Keywords: configuration,settings,json,yaml,toml,ini
+Author: Tiago Requeijo
+Author-email: tiago.requeijo.dev@gmail.com
+Requires-Python: >=3.8.1,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: aws
+Provides-Extra: azure
+Provides-Extra: gcp
+Provides-Extra: toml
+Provides-Extra: yaml
+Requires-Dist: azure-identity (>=1.13.0,<2.0.0) ; extra == "azure"
+Requires-Dist: azure-keyvault (>=4.2.0,<5.0.0) ; extra == "azure"
+Requires-Dist: boto3 (>=1.28.20,<2.0.0) ; extra == "aws"
+Requires-Dist: google-cloud-secret-manager (>=2.16.3,<3.0.0) ; extra == "gcp"
+Requires-Dist: pyyaml (>=6.0,<7.0) ; extra == "yaml"
+Requires-Dist: toml (>=0.10.0,<0.11.0) ; extra == "toml"
+Project-URL: Repository, https://github.com/tr11/python-configuration
+Description-Content-Type: text/markdown
 
-packages = \
-['config', 'config.contrib']
+# python-configuration
+> A library to load configuration parameters hierarchically from multiple sources and formats
 
-package_data = \
-{'': ['*']}
+[![version](https://img.shields.io/pypi/v/python-configuration)](https://pypi.org/project/python-configuration/)
+![python](https://img.shields.io/pypi/pyversions/python-configuration)
+![wheel](https://img.shields.io/pypi/wheel/python-configuration)
+![license](https://img.shields.io/pypi/l/python-configuration)
+[![tests](https://github.com/tr11/python-configuration/actions/workflows/run_tests.yml/badge.svg)](https://github.com/tr11/python-configuration/actions/workflows/run_tests.yml)
+[![codecov](https://codecov.io/gh/tr11/python-configuration/branch/main/graph/badge.svg?token=5zRYlGnDs7)](https://codecov.io/gh/tr11/python-configuration)
+[![Documentation Status](https://readthedocs.org/projects/python-configuration/badge/?version=latest)](https://python-configuration.readthedocs.io/en/latest/?badge=latest)
 
-extras_require = \
-{'aws': ['boto3>=1.10.48,<2.0.0'],
- 'azure': ['azure-identity>=1.5.0,<2.0.0', 'azure-keyvault>=4.0.0,<5.0.0'],
- 'gcp': ['google-cloud-secret-manager>=2.0.0,<3.0.0'],
- 'toml': ['toml>=0.10.0,<0.11.0'],
- 'yaml': ['pyyaml>=5.1,<6.0']}
-
-setup_kwargs = {
-    'name': 'python-configuration',
-    'version': '0.8.2',
-    'description': 'A library to load configuration parameters from multiple sources and formats',
-    'long_description': '# python-configuration\n> A library to load configuration parameters hierarchically from multiple sources and formats\n\n[![version](https://img.shields.io/pypi/v/python-configuration)](https://pypi.org/project/python-configuration/)\n![python](https://img.shields.io/pypi/pyversions/python-configuration)\n![wheel](https://img.shields.io/pypi/wheel/python-configuration)\n![license](https://img.shields.io/pypi/l/python-configuration)\n[![build](https://img.shields.io/travis/tr11/python-configuration)](https://travis-ci.org/tr11/python-configuration)\n[![codecov](https://codecov.io/gh/tr11/python-configuration/branch/master/graph/badge.svg)](https://codecov.io/gh/tr11/python-configuration)\n[![Documentation Status](https://readthedocs.org/projects/python-configuration/badge/?version=latest)](https://python-configuration.readthedocs.io/en/latest/?badge=latest)\n\nThis library is intended as a helper mechanism to load configuration files\nhierarchically.  Current format types are:\n* Python files\n* Dictionaries\n* Environment variables\n* Filesystem paths\n* JSON files\n* INI files\n* dotenv type files\n\nand optionally\n* YAML files\n* TOML files\n* Azure Key Vault credentials\n* AWS Secrets Manager credentials\n* GCP Secret Manager credentials\n\n## Installing\n\nTo install the library:\n```shell\npip install python-configuration\n```\n\nTo include the optional TOML and/or YAML loaders, install the optional\ndependencies `toml` and ` yaml`. For example,\n```shell\npip install python-configuration[toml,yaml]\n```\n\n## Getting started\n\nThis library converts the config types above into dictionaries with \ndotted-based keys. That is, given a config `cfg` from the structure\n```python\n{\n    \'a\': {\n        \'b\': \'value\'\n    }\n}\n```\nwe are able to refer to the parameter above as any of \n```python\ncfg[\'a.b\']\ncfg[\'a\'][\'b\']\ncfg[\'a\'].b\ncfg.a.b\n```\nand extract specific data types such as dictionaries:\n```python\ncfg[\'a\'].as_dict == {\'b\': \'value\'}\n```\nThis is particularly useful in order to isolate group parameters.\nFor example, with the JSON configuration\n```json\n{\n  "database.host": "something",\n  "database.port": 12345,\n  "database.driver": "name",\n  "app.debug": true,\n  "app.environment": "development",\n  "app.secrets": "super secret",\n  "logging": {\n    "service": "service",\n    "token": "token",\n    "tags": "tags"\n  }\n}\n```\none can retrieve the dictionaries as \n```python\ncfg.database.as_dict()\ncfg.app.as_dict()\ncfg.logging.as_dict()\n```\nor simply as \n```python\ndict(cfg.database)\ndict(cfg.app)\ndict(cfg.logging)\n```\n## Configuration\nThere are two general types of objects in this library. The first one is the `Configuration`,\nwhich represents a single config source.  The second is a `ConfigurationSet` that allows for\nmultiple `Configuration` objects to be specified.\n\n### Single Config\n\n#### Python Files\nTo load a configuration from a Python module, the `config_from_python` can be used.\nThe first parameter must be a Python module and can be specified as an absolute path to the Python file or as an importable module.\n\nOptional parameters are the `prefix` and `separator`.  The following call \n```python\nconfig_from_python(\'foo.bar\', prefix=\'CONFIG\', separator=\'__\')\n```\nwill read every variable in the `foo.bar` module that starts with `CONFIG__` and replace\nevery occurrence of `__` with a `.`. For example,\n```python\n# foo.bar\nCONFIG__AA__BB_C = 1\nCONFIG__AA__BB__D = 2\nCONF__AA__BB__D = 3\n```\nwould result in the configuration\n```python\n{\n    \'aa.bb_c\': 1,\n    \'aa.bb.d\': 2,\n}\n```\nNote that the single underscore in `BB_C` is not replaced and the last line is not\nprefixed by `CONFIG`. \n\n#### Dictionaries\nDictionaries are loaded with `config_from_dict` and are converted internally to a \nflattened `dict`. \n```python\n{\n    \'a\': {\n        \'b\': \'value\'\n    }\n}\n```\nbecomes\n```python\n{\n    \'a.b\': \'value\'\n}\n```\n\n#### Environment Variables\nEnvironment variables starting with `prefix` can be read with `config_from_env`:\n```python\nconfig_from_env(prefix, separator=\'_\')\n```\n\n#### Filesystem Paths\nFolders with files named as `xxx.yyy.zzz` can be loaded with the `config_from_path` function.  This format is useful to load mounted\nKubernetes [ConfigMaps](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/#populate-a-volume-with-data-stored-in-a-configmap)\nor [Secrets](https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#create-a-pod-that-has-access-to-the-secret-data-through-a-volume).\n\n#### JSON, INI, .env, YAML, TOML\nJSON, INI, YAML, TOML files are loaded respectively with\n`config_from_json`,\n`config_from_ini`,\n`config_from_dotenv`,\n`config_from_yaml`, and\n`config_from_toml`.\nThe parameter `read_from_file` controls\nwhether a string should be interpreted as a filename.\n\n###### Caveats\nIn order for `Configuration` objects to act as `dict` and allow the syntax\n`dict(cfg)`, the `keys()` method is implemented as the typical `dict` keys.\nIf `keys` is an element in the configuration `cfg` then the `dict(cfg)` call will fail.\nIn that case, it\'s necessary to use the `cfg.as_dict()` method to retrieve the\n`dict` representation for the `Configuration` object.\n\nThe same applies to the methods `values()` and `items()`.\n \n\n### Configuration Sets\nConfiguration sets are used to hierarchically load configurations and merge\nsettings. Sets can be loaded by constructing a `ConfigurationSet` object directly or\nusing the simplified `config` function.\n\nTo construct a `ConfigurationSet`, pass in as many of the simple `Configuration` objects as needed:\n```python\ncfg = ConfigurationSet(\n    config_from_env(prefix=PREFIX),\n    config_from_json(path, read_from_file=True),\n    config_from_dict(DICT),\n)\n```\nThe example above will read first from Environment variables prefixed with `PREFIX`, \nand fallback first to the JSON file at `path`, and finally use the dictionary `DICT`.\n\nThe `config` function simplifies loading sets by assuming some defaults.\nThe example above can also be obtained by\n```python\ncfg = config(\n    (\'env\', PREFIX),\n    (\'json\', path, True),\n    (\'dict\', DICT),\n)\n```\nor, even simpler if `path` points to a file with a `.json` suffix:\n```python\ncfg = config(\'env\', path, DICT, prefix=PREFIX)\n```\nThe `config` function automatically detects the following:\n* extension `.py` for python modules\n* dot-separated python identifiers as a python module (e.g. `foo.bar`)\n* extension `.json` for JSON files\n* extension `.yaml` for YAML files\n* extension `.toml` for TOML files\n* extension `.ini` for INI files\n* extension `.env` for dotenv type files\n* filesystem folders as Filesystem Paths\n* the strings `env` or `environment` for Environment Variables\n\n#### Merging Values\n`ConfigurationSet` instances are constructed by inspecting each configuration source, taking into account nested dictionaries, and merging at the most granular level.\nFor example, the instance obtained from `cfg = config(d1, d2)` for the dictionaries below\n\n```python\nd1 = {\'sub\': {\'a\': 1, \'b\': 4}}\nd2 = {\'sub\': {\'b\': 2, \'c\': 3}}\n```\n\nis such that `cfg[\'sub\']` equals\n\n```python\n{\'a\': 1, \'b\': 4, \'c\': 3}\n```\n\nNote that the nested dictionaries of `\'sub\'` in each of `d1` and `d2` do not overwrite each other, but are merged into a single\ndictionary with keys from both `d1` and `d2`, giving priority to the values of `d1` over those from `d2`.\n\n\n###### Caveats\nAs long as the data types are consistent across all the configurations that are\npart of a `ConfigurationSet`, the behavior should be straightforward.  When different\nconfiguration objects are specified with competing data types, the first configuration to\ndefine the elements sets its datatype. For example, if in the example above \n`element` is interpreted as a `dict` from environment variables, but the \nJSON file specifies it as anything else besides a mapping, then the JSON value will be\ndropped automatically. \n\n## Other Features\n\n###### String Interpolation\nWhen setting the `interpolate` parameter in any `Configuration` instance, the library will\nperform a string interpolation step using the [str.format](https://docs.python.org/3/library/string.html#formatstrings)\nsyntax.  In particular, this allows to format configuration values automatically:\n```python\ncfg = config_from_dict({\n    "percentage": "{val:.3%}",\n    "with_sign": "{val:+f}",\n    "val": 1.23456}, interpolate=True)\n\nassert cfg.val == 1.23456\nassert cfg.with_sign == "+1.234560"\nassert cfg.percentage == "123.456%"\n```\n\n## Extras\nThe `config.contrib` package contains extra implementations of the `Configuration` class\nused for special cases. Currently the following are implemented:\n* `AzureKeyVaultConfiguration` in `config.contrib.azure`, which takes Azure Key Vault\n  credentials into a `Configuration`-compatible instance. To install the needed dependencies\n  execute\n  ```shell\n  pip install python-configuration[azure]\n  ```\n* `AWSSecretsManagerConfiguration` in `config.contrib.aws`, which takes AWS Secrets Manager\n  credentials into a `Configuration`-compatible instance. To install the needed dependencies\n  execute\n  ```shell\n  pip install python-configuration[aws]\n  ```\n* `GCPSecretManagerConfiguration` in `config.contrib.gcp`, which takes GCP Secret Manager\n  credentials into a `Configuration`-compatible instance. To install the needed dependencies\n  execute\n  ```shell\n  pip install python-configuration[gcp]\n  ```\n\n## Developing\n\nTo develop this library, download the source code and install a local version.\n\n\n## Features\n\n* Load multiple configuration types\n* Hierarchical configuration\n* Ability to override with environment variables\n* Merge parameters from different configuration types\n\n## Contributing\n\nIf you\'d like to contribute, please fork the repository and use a feature\nbranch. Pull requests are welcome.\n\n## Links\n\n- Repository: https://github.com/tr11/python-configuration\n- Issue tracker: https://github.com/tr11/python-configuration/issues\n- Documentation: https://python-configuration.readthedocs.io\n\n## Licensing\n\nThe code in this project is licensed under MIT license.\n',
-    'author': 'Tiago Requeijo',
-    'author_email': 'tiago.requeijo.dev@gmail.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/tr11/python-configuration',
-    'packages': packages,
-    'package_data': package_data,
-    'extras_require': extras_require,
-    'python_requires': '>=3.6,<4.0',
+This library is intended as a helper mechanism to load configuration files hierarchically.  Supported format types are:
+
+* Python files
+* Dictionaries
+* Environment variables
+* Filesystem paths
+* JSON files
+* INI files
+* dotenv type files
+
+and optionally
+
+* YAML files
+* TOML files
+* Azure Key Vault credentials
+* AWS Secrets Manager credentials
+* GCP Secret Manager credentials
+
+## Installing
+
+To install the library:
+
+```shell
+pip install python-configuration
+```
+
+To include the optional TOML and/or YAML loaders, install the optional dependencies `toml` and ` yaml`. For example,
+
+```shell
+pip install python-configuration[toml,yaml]
+```
+
+## Getting started
+
+`python-configuration` converts the various config types into dictionaries with dotted-based keys. For example, given this JSON configuration
+
+```json
+{
+    "a": {
+        "b": "value"
+    }
 }
+```
+
+We can use the `config_from_json` method to parse it:
+
+```python
+from config import config_from_json
+
+cfg = config_from_json("my_config_file.json", read_from_file=True)
+```
+
+(Similar methods exist for all the other supported configuration formats (eg. `config_from_toml`, etc.).)
+
+We are then able to refer to the parameters in the config above using any of:
+
+```python
+cfg['a.b']
+cfg['a']['b']
+cfg['a'].b
+cfg.a.b
+```
+
+and extract specific data types such as dictionaries:
+
+```python
+cfg['a'].as_dict == {'b': 'value'}
+```
+
+This is particularly useful in order to isolate group parameters.
+For example, with the JSON configuration
+
+```json
+{
+  "database.host": "something",
+  "database.port": 12345,
+  "database.driver": "name",
+  "app.debug": true,
+  "app.environment": "development",
+  "app.secrets": "super secret",
+  "logging": {
+    "service": "service",
+    "token": "token",
+    "tags": "tags"
+  }
+}
+```
+
+one can retrieve the dictionaries as
+
+```python
+cfg.database.as_dict()
+cfg.app.as_dict()
+cfg.logging.as_dict()
+```
+
+or simply as
+
+```python
+dict(cfg.database)
+dict(cfg.app)
+dict(cfg.logging)
+```
+
+## Configuration
+
+There are two general types of objects in this library. The first one is the `Configuration`, which represents a single config source.  The second is a `ConfigurationSet` that allows for multiple `Configuration` objects to be specified.
+
+### Single Config
+
+#### Python Files
+
+To load a configuration from a Python module, the `config_from_python` can be used.
+The first parameter must be a Python module and can be specified as an absolute path to the Python file or as an importable module.
+
+Optional parameters are the `prefix` and `separator`.  The following call
+
+```python
+config_from_python('foo.bar', prefix='CONFIG', separator='__')
+```
+
+will read every variable in the `foo.bar` module that starts with `CONFIG__` and replace every occurrence of `__` with a `.`. For example,
+
+```python
+# foo.bar
+CONFIG__AA__BB_C = 1
+CONFIG__AA__BB__D = 2
+CONF__AA__BB__D = 3
+```
+
+would result in the configuration
+
+```python
+{
+    'aa.bb_c': 1,
+    'aa.bb.d': 2,
+}
+```
+
+Note that the single underscore in `BB_C` is not replaced and the last line is not prefixed by `CONFIG`.
+
+#### Dictionaries
+
+Dictionaries are loaded with `config_from_dict` and are converted internally to a flattened `dict`.
+
+```python
+{
+    'a': {
+        'b': 'value'
+    }
+}
+```
+
+becomes
+
+```python
+{
+    'a.b': 'value'
+}
+```
+
+#### Environment Variables
+
+Environment variables starting with `prefix` can be read with `config_from_env`:
+
+```python
+config_from_env(prefix, separator='_')
+```
+
+#### Filesystem Paths
+
+Folders with files named as `xxx.yyy.zzz` can be loaded with the `config_from_path` function.  This format is useful to load mounted Kubernetes [ConfigMaps](https://kubernetes.io/docs/tasks/configure-pod-container/configure-pod-configmap/#populate-a-volume-with-data-stored-in-a-configmap) or [Secrets](https://kubernetes.io/docs/tasks/inject-data-application/distribute-credentials-secure/#create-a-pod-that-has-access-to-the-secret-data-through-a-volume).
+
+#### JSON, INI, .env, YAML, TOML
+
+JSON, INI, YAML, TOML files are loaded respectively with
+`config_from_json`,
+`config_from_ini`,
+`config_from_dotenv`,
+`config_from_yaml`, and
+`config_from_toml`.
+The parameter `read_from_file` controls whether a string should be interpreted as a filename.
+
+###### Caveats
+
+In order for `Configuration` objects to act as `dict` and allow the syntax `dict(cfg)`, the `keys()` method is implemented as the typical `dict` keys. If `keys` is an element in the configuration `cfg` then the `dict(cfg)` call will fail. In that case, it's necessary to use the `cfg.as_dict()` method to retrieve the `dict` representation for the `Configuration` object.
+
+The same applies to the methods `values()` and `items()`.
+
+
+### Configuration Sets
+
+Configuration sets are used to hierarchically load configurations and merge settings. Sets can be loaded by constructing a `ConfigurationSet` object directly or using the simplified `config` function.
+
+To construct a `ConfigurationSet`, pass in as many of the simple `Configuration` objects as needed:
+
+```python
+cfg = ConfigurationSet(
+    config_from_env(prefix=PREFIX),
+    config_from_json(path, read_from_file=True),
+    config_from_dict(DICT),
+)
+```
+The example above will read first from Environment variables prefixed with `PREFIX`, and fallback first to the JSON file at `path`, and finally use the dictionary `DICT`.
+
+The `config` function simplifies loading sets by assuming some defaults.
+The example above can also be obtained by
+
+```python
+cfg = config(
+    ('env', PREFIX),
+    ('json', path, True),
+    ('dict', DICT),
+)
+```
+
+or, even simpler if `path` points to a file with a `.json` suffix:
+
+```python
+cfg = config('env', path, DICT, prefix=PREFIX)
+```
+
+The `config` function automatically detects the following:
+
+* extension `.py` for python modules
+* dot-separated python identifiers as a python module (e.g. `foo.bar`)
+* extension `.json` for JSON files
+* extension `.yaml` for YAML files
+* extension `.toml` for TOML files
+* extension `.ini` for INI files
+* extension `.env` for dotenv type files
+* filesystem folders as Filesystem Paths
+* the strings `env` or `environment` for Environment Variables
+
+#### Merging Values
+
+`ConfigurationSet` instances are constructed by inspecting each configuration source, taking into account nested dictionaries, and merging at the most granular level.
+For example, the instance obtained from `cfg = config(d1, d2)` for the dictionaries below
+
+```python
+d1 = {'sub': {'a': 1, 'b': 4}}
+d2 = {'sub': {'b': 2, 'c': 3}}
+```
+
+is such that `cfg['sub']` equals
+
+```python
+{'a': 1, 'b': 4, 'c': 3}
+```
+
+Note that the nested dictionaries of `'sub'` in each of `d1` and `d2` do not overwrite each other, but are merged into a single dictionary with keys from both `d1` and `d2`, giving priority to the values of `d1` over those from `d2`.
+
+
+###### Caveats
+
+As long as the data types are consistent across all the configurations that are part of a `ConfigurationSet`, the behavior should be straightforward.  When different configuration objects are specified with competing data types, the first configuration to define the elements sets its datatype. For example, if in the example above `element` is interpreted as a `dict` from environment variables, but the JSON file specifies it as anything else besides a mapping, then the JSON value will be dropped automatically.
+
+## Other Features
+
+###### String Interpolation
+
+When setting the `interpolate` parameter in any `Configuration` instance, the library will perform a string interpolation step using the [str.format](https://docs.python.org/3/library/string.html#formatstrings) syntax.  In particular, this allows to format configuration values automatically:
+
+```python
+cfg = config_from_dict({
+    "percentage": "{val:.3%}",
+    "with_sign": "{val:+f}",
+    "val": 1.23456}, interpolate=True)
+
+assert cfg.val == 1.23456
+assert cfg.with_sign == "+1.234560"
+assert cfg.percentage == "123.456%"
+```
+
+## Extras
+
+The `config.contrib` package contains extra implementations of the `Configuration` class used for special cases. Currently the following are implemented:
+
+* `AzureKeyVaultConfiguration` in `config.contrib.azure`, which takes Azure Key Vault
+  credentials into a `Configuration`-compatible instance. To install the needed dependencies
+  execute
+
+  ```shell
+  pip install python-configuration[azure]
+  ```
+
+* `AWSSecretsManagerConfiguration` in `config.contrib.aws`, which takes AWS Secrets Manager
+  credentials into a `Configuration`-compatible instance. To install the needed dependencies
+  execute
+
+  ```shell
+  pip install python-configuration[aws]
+  ```
+
+* `GCPSecretManagerConfiguration` in `config.contrib.gcp`, which takes GCP Secret Manager
+  credentials into a `Configuration`-compatible instance. To install the needed dependencies
+  execute
+
+  ```shell
+  pip install python-configuration[gcp]
+  ```
+
+## Features
+
+* Load multiple configuration types
+* Hierarchical configuration
+* Ability to override with environment variables
+* Merge parameters from different configuration types
+
+## Contributing :tada:
+
+If you'd like to contribute, please fork the repository and use a feature branch. Pull requests are welcome.
+
+See [`CONTRIBUTING.md`](CONTRIBUTING.md) for the details.
+
+## Links
+
+- Repository: https://github.com/tr11/python-configuration
+- Issue tracker: https://github.com/tr11/python-configuration/issues
+- Documentation: https://python-configuration.readthedocs.io
+
+## Licensing
 
+The code in this project is licensed under MIT license.
 
-setup(**setup_kwargs)
```

