# Comparing `tmp/localstack-2.2.0.tar.gz` & `tmp/localstack-2.2.1.dev20230805180111.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-2.2.0.tar", last modified: Thu Jul 20 12:43:00 2023, max compression
+gzip compressed data, was "localstack-2.2.1.dev20230805180111.tar", last modified: Sat Aug  5 18:04:16 2023, max compression
```

## Comparing `localstack-2.2.0.tar` & `localstack-2.2.1.dev20230805180111.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-07-20 12:43:00.093762 localstack-2.2.0/
--rw-rw-r--   0 runner    (1000) runner    (1001)    12353 2023-07-20 12:43:00.093762 localstack-2.2.0/PKG-INFO
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-07-20 12:43:00.093762 localstack-2.2.0/localstack.egg-info/
--rw-rw-r--   0 runner    (1000) runner    (1001)    12353 2023-07-20 12:43:00.000000 localstack-2.2.0/localstack.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-07-20 12:43:00.000000 localstack-2.2.0/localstack.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-07-20 12:43:00.000000 localstack-2.2.0/localstack.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)      169 2023-07-20 12:43:00.000000 localstack-2.2.0/localstack.egg-info/requires.txt
--rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-07-20 12:43:00.000000 localstack-2.2.0/localstack.egg-info/top_level.txt
-drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-07-20 12:43:00.093762 localstack-2.2.0/localstack_cli/
--rw-rw-r--   0 runner    (1000) runner    (1001)       50 2023-07-20 12:42:59.000000 localstack-2.2.0/localstack_cli/__init__.py
--rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-07-20 12:43:00.093762 localstack-2.2.0/setup.cfg
--rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-07-20 12:39:40.000000 localstack-2.2.0/setup.py
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12370 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/PKG-INFO
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/localstack.egg-info/
+-rw-rw-r--   0 runner    (1000) runner    (1001)    12370 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1000) runner    (1001)      204 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)        1 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)      223 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1000) runner    (1001)       15 2023-08-05 18:04:16.000000 localstack-2.2.1.dev20230805180111/localstack.egg-info/top_level.txt
+drwxrwxr-x   0 runner    (1000) runner    (1001)        0 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/localstack_cli/
+-rw-rw-r--   0 runner    (1000) runner    (1001)       68 2023-08-05 18:04:15.000000 localstack-2.2.1.dev20230805180111/localstack_cli/__init__.py
+-rw-rw-r--   0 runner    (1000) runner    (1001)       38 2023-08-05 18:04:16.255018 localstack-2.2.1.dev20230805180111/setup.cfg
+-rw-rw-r--   0 runner    (1000) runner    (1001)     1553 2023-08-05 18:00:56.000000 localstack-2.2.1.dev20230805180111/setup.py
```

### Comparing `localstack-2.2.0/PKG-INFO` & `localstack-2.2.1.dev20230805180111/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.2.0
+Version: 2.2.1.dev20230805180111
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Emulators
 Description-Content-Type: text/markdown
 Provides-Extra: runtime
 Provides-Extra: full
 
 <p align="center">
-:zap: We are thrilled to announce <a href="https://discuss.localstack.cloud/t/localstack-release-v2-1-0/357">LocalStack 2.1</a> which brings new features, enhancements and bugfixes :zap:
+:zap: We are thrilled to announce <a href="https://discuss.localstack.cloud/t/localstack-release-v2-2-0/424">LocalStack 2.2</a> which brings new features, enhancements and bugfixes :zap:
 </p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/localstack/localstack/master/doc/localstack-readme-banner.svg" alt="LocalStack - A fully functional local cloud stack">
 </p>
 
 <p align="center">
@@ -29,15 +29,15 @@
   <a href="https://pypi.org/project/localstack/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/localstack?color=blue"></a>
   <a href="https://hub.docker.com/r/localstack/localstack"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/localstack/localstack"></a>
   <a href="https://pypi.org/project/localstack"><img alt="PyPi downloads" src="https://static.pepy.tech/badge/localstack"></a>
   <a href="#backers"><img alt="Backers on Open Collective" src="https://opencollective.com/localstack/backers/badge.svg"></a>
   <a href="#sponsors"><img alt="Sponsors on Open Collective" src="https://opencollective.com/localstack/sponsors/badge.svg"></a>
   <a href="https://img.shields.io/pypi/l/localstack.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/localstack.svg"></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-  <a href="https://twitter.com/_localstack"><img alt="Twitter" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
+  <a href="https://twitter.com/localstack"><img alt="Twitter" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
 </p>
 
 <p align="center">
   LocalStack provides an easy-to-use test/mocking framework for developing cloud applications.
 </p>
 
 <p align="center">
@@ -105,15 +105,15 @@
 
      __                     _______ __             __
     / /   ____  _________ _/ / ___// /_____ ______/ /__
    / /   / __ \/ ___/ __ `/ /\__ \/ __/ __ `/ ___/ //_/
   / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,<
  /_____/\____/\___/\__,_/_//____/\__/\__,_/\___/_/|_|
 
- 💻 LocalStack CLI 2.0.0
+ 💻 LocalStack CLI 2.2.0
 
 [20:22:20] starting LocalStack in Docker mode 🐳
 [20:22:21] detaching
 ```
 
 You can query the status of respective services on LocalStack by running:
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.2.0 Summary: LocalStack - A
-fully functional local Cloud stack Home-page: https://github.com/localstack/
-localstack Author: LocalStack Contributors Author-email: info@localstack.cloud
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Emulators Description-Content-Type: text/
-markdown Provides-Extra: runtime Provides-Extra: full
-  :zap: We are thrilled to announce LocalStack_2.1 which brings new features,
+Metadata-Version: 2.1 Name: localstack Version: 2.2.1.dev20230805180111
+Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
+github.com/localstack/localstack Author: LocalStack Contributors Author-email:
+info@localstack.cloud License: Apache License 2.0 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Testing Classifier: Topic :: System :: Emulators Description-
+Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
+  :zap: We are thrilled to announce LocalStack_2.2 which brings new features,
                         enhancements and bugfixes :zap:
               [LocalStack - A fully functional local cloud stack]
  [CircleCI] [Coverage_Status] [PyPI_Version] [Docker_Pulls] [PyPi_downloads]
 [Backers_on_Open_Collective] [Sponsors_on_Open_Collective] [PyPI_License] [Code
                             style:_black] [Twitter]
 LocalStack provides an easy-to-use test/mocking framework for developing cloud
                                  applications.
@@ -51,15 +51,15 @@
 install localstack ``` > **Important**: Do not use `sudo` or run as `root`
 user. LocalStack must be installed and started entirely under a local non-root
 user. If you have problems with permissions in macOS High Sierra, install with
 `pip install --user localstack` ## Example Start LocalStack inside a Docker
 container by running: ``` % localstack start -d __ _______ __ __ / / ____
 _________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/ __
 `/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/\____/
-\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.0.0 [20:22:20]
+\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.2.0 [20:22:20]
 starting LocalStack in Docker mode ð³ [20:22:21] detaching ``` You can query
 the status of respective services on LocalStack by running: ``` % localstack
 status services
 ââââââââââââââââââââââââââââ³ââââââââââââââ
 â Service â Status â
 â¡âââââââââââââââââââââââââââââââââââââââââ©
 â acm â â available â â apigateway â â available â â
```

### Comparing `localstack-2.2.0/localstack.egg-info/PKG-INFO` & `localstack-2.2.1.dev20230805180111/localstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: localstack
-Version: 2.2.0
+Version: 2.2.1.dev20230805180111
 Summary: LocalStack - A fully functional local Cloud stack
 Home-page: https://github.com/localstack/localstack
 Author: LocalStack Contributors
 Author-email: info@localstack.cloud
 License: Apache License 2.0
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: Apache Software License
@@ -12,15 +12,15 @@
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: System :: Emulators
 Description-Content-Type: text/markdown
 Provides-Extra: runtime
 Provides-Extra: full
 
 <p align="center">
-:zap: We are thrilled to announce <a href="https://discuss.localstack.cloud/t/localstack-release-v2-1-0/357">LocalStack 2.1</a> which brings new features, enhancements and bugfixes :zap:
+:zap: We are thrilled to announce <a href="https://discuss.localstack.cloud/t/localstack-release-v2-2-0/424">LocalStack 2.2</a> which brings new features, enhancements and bugfixes :zap:
 </p>
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/localstack/localstack/master/doc/localstack-readme-banner.svg" alt="LocalStack - A fully functional local cloud stack">
 </p>
 
 <p align="center">
@@ -29,15 +29,15 @@
   <a href="https://pypi.org/project/localstack/"><img alt="PyPI Version" src="https://img.shields.io/pypi/v/localstack?color=blue"></a>
   <a href="https://hub.docker.com/r/localstack/localstack"><img alt="Docker Pulls" src="https://img.shields.io/docker/pulls/localstack/localstack"></a>
   <a href="https://pypi.org/project/localstack"><img alt="PyPi downloads" src="https://static.pepy.tech/badge/localstack"></a>
   <a href="#backers"><img alt="Backers on Open Collective" src="https://opencollective.com/localstack/backers/badge.svg"></a>
   <a href="#sponsors"><img alt="Sponsors on Open Collective" src="https://opencollective.com/localstack/sponsors/badge.svg"></a>
   <a href="https://img.shields.io/pypi/l/localstack.svg"><img alt="PyPI License" src="https://img.shields.io/pypi/l/localstack.svg"></a>
   <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
-  <a href="https://twitter.com/_localstack"><img alt="Twitter" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
+  <a href="https://twitter.com/localstack"><img alt="Twitter" src="https://img.shields.io/twitter/url/http/shields.io.svg?style=social"></a>
 </p>
 
 <p align="center">
   LocalStack provides an easy-to-use test/mocking framework for developing cloud applications.
 </p>
 
 <p align="center">
@@ -105,15 +105,15 @@
 
      __                     _______ __             __
     / /   ____  _________ _/ / ___// /_____ ______/ /__
    / /   / __ \/ ___/ __ `/ /\__ \/ __/ __ `/ ___/ //_/
   / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,<
  /_____/\____/\___/\__,_/_//____/\__/\__,_/\___/_/|_|
 
- 💻 LocalStack CLI 2.0.0
+ 💻 LocalStack CLI 2.2.0
 
 [20:22:20] starting LocalStack in Docker mode 🐳
 [20:22:21] detaching
 ```
 
 You can query the status of respective services on LocalStack by running:
```

#### html2text {}

```diff
@@ -1,16 +1,16 @@
-Metadata-Version: 2.1 Name: localstack Version: 2.2.0 Summary: LocalStack - A
-fully functional local Cloud stack Home-page: https://github.com/localstack/
-localstack Author: LocalStack Contributors Author-email: info@localstack.cloud
-License: Apache License 2.0 Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: Apache Software License Classifier:
-Topic :: Internet Classifier: Topic :: Software Development :: Testing
-Classifier: Topic :: System :: Emulators Description-Content-Type: text/
-markdown Provides-Extra: runtime Provides-Extra: full
-  :zap: We are thrilled to announce LocalStack_2.1 which brings new features,
+Metadata-Version: 2.1 Name: localstack Version: 2.2.1.dev20230805180111
+Summary: LocalStack - A fully functional local Cloud stack Home-page: https://
+github.com/localstack/localstack Author: LocalStack Contributors Author-email:
+info@localstack.cloud License: Apache License 2.0 Classifier: Programming
+Language :: Python :: 3.10 Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Topic :: Internet Classifier: Topic :: Software
+Development :: Testing Classifier: Topic :: System :: Emulators Description-
+Content-Type: text/markdown Provides-Extra: runtime Provides-Extra: full
+  :zap: We are thrilled to announce LocalStack_2.2 which brings new features,
                         enhancements and bugfixes :zap:
               [LocalStack - A fully functional local cloud stack]
  [CircleCI] [Coverage_Status] [PyPI_Version] [Docker_Pulls] [PyPi_downloads]
 [Backers_on_Open_Collective] [Sponsors_on_Open_Collective] [PyPI_License] [Code
                             style:_black] [Twitter]
 LocalStack provides an easy-to-use test/mocking framework for developing cloud
                                  applications.
@@ -51,15 +51,15 @@
 install localstack ``` > **Important**: Do not use `sudo` or run as `root`
 user. LocalStack must be installed and started entirely under a local non-root
 user. If you have problems with permissions in macOS High Sierra, install with
 `pip install --user localstack` ## Example Start LocalStack inside a Docker
 container by running: ``` % localstack start -d __ _______ __ __ / / ____
 _________ _/ / ___// /_____ ______/ /__ / / / __ \/ ___/ __ `/ /\__ \/ __/ __
 `/ ___/ //_/ / /___/ /_/ / /__/ /_/ / /___/ / /_/ /_/ / /__/ ,< /_____/\____/
-\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.0.0 [20:22:20]
+\___/\__,_/_//____/\__/\__,_/\___/_/|_| ð» LocalStack CLI 2.2.0 [20:22:20]
 starting LocalStack in Docker mode ð³ [20:22:21] detaching ``` You can query
 the status of respective services on LocalStack by running: ``` % localstack
 status services
 ââââââââââââââââââââââââââââ³ââââââââââââââ
 â Service â Status â
 â¡âââââââââââââââââââââââââââââââââââââââââ©
 â acm â â available â â apigateway â â available â â
```

### Comparing `localstack-2.2.0/setup.py` & `localstack-2.2.1.dev20230805180111/setup.py`

 * *Files identical despite different names*

