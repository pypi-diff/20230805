# Comparing `tmp/mkdocs_python_classy-0.1.2.tar.gz` & `tmp/mkdocs_python_classy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs_python_classy-0.1.2.tar", max compression
+gzip compressed data, was "mkdocs_python_classy-0.1.3.tar", max compression
```

## Comparing `mkdocs_python_classy-0.1.2.tar` & `mkdocs_python_classy-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      581 2023-07-28 22:49:04.649912 mkdocs_python_classy-0.1.2/LICENSE
--rw-r--r--   0        0        0      302 2023-07-28 22:49:04.649912 mkdocs_python_classy-0.1.2/NOTICE
--rw-r--r--   0        0        0     3997 2023-07-28 22:49:04.649912 mkdocs_python_classy-0.1.2/README.md
--rw-r--r--   0        0        0     7950 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/__init__.py
--rw-r--r--   0        0        0      288 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/constants.py
--rw-r--r--   0        0        0       32 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/css/classy.css
--rw-r--r--   0        0        0    13361 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/inspector.py
--rw-r--r--   0        0        0     6730 2023-07-28 22:49:04.653912 mkdocs_python_classy-0.1.2/mkdocs_python_classy/utils.py
--rw-r--r--   0        0        0     3254 2023-07-28 22:49:14.693887 mkdocs_python_classy-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4809 1970-01-01 00:00:00.000000 mkdocs_python_classy-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      581 2023-08-04 23:17:46.148421 mkdocs_python_classy-0.1.3/LICENSE
+-rw-r--r--   0        0        0      302 2023-08-04 23:17:46.148421 mkdocs_python_classy-0.1.3/NOTICE
+-rw-r--r--   0        0        0     4286 2023-08-04 23:17:46.148421 mkdocs_python_classy-0.1.3/README.md
+-rw-r--r--   0        0        0     7950 2023-08-04 23:17:46.152421 mkdocs_python_classy-0.1.3/mkdocs_python_classy/__init__.py
+-rw-r--r--   0        0        0      288 2023-08-04 23:17:46.152421 mkdocs_python_classy-0.1.3/mkdocs_python_classy/constants.py
+-rw-r--r--   0        0        0       32 2023-08-04 23:17:46.152421 mkdocs_python_classy-0.1.3/mkdocs_python_classy/css/classy.css
+-rw-r--r--   0        0        0    13361 2023-08-04 23:17:46.152421 mkdocs_python_classy-0.1.3/mkdocs_python_classy/inspector.py
+-rw-r--r--   0        0        0     6730 2023-08-04 23:17:46.152421 mkdocs_python_classy-0.1.3/mkdocs_python_classy/utils.py
+-rw-r--r--   0        0        0     3254 2023-08-04 23:18:02.789364 mkdocs_python_classy-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5098 1970-01-01 00:00:00.000000 mkdocs_python_classy-0.1.3/PKG-INFO
```

### Comparing `mkdocs_python_classy-0.1.2/LICENSE` & `mkdocs_python_classy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_python_classy-0.1.2/README.md` & `mkdocs_python_classy-0.1.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 # mkdocs-python-classy
 
 <p align="center">
 
   <img src="https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-classy/develop/docs/images/icon-mkdocs-python-classy.png" class="logo" height="100px">
   <br>
-  <!-- <a href="https://github.com/networktocode/mkdocs-python-classy/actions"><img src="https://github.com/networktocode/mkdocs-python-classy/actions/workflows/ci.yml/badge.svg?branch=main"></a> -->
-  <a href="/en/latest"><img src="https://readthedocs.org/projects/mkdocs-python-classy/badge/"></a>
+  <a href="https://github.com/itdependsnetworks/mkdocs-python-classy/actions"><img src="https://github.com/itdependsnetworks/mkdocs-python-classy/actions/workflows/ci.yml/badge.svg?branch=main"></a>
+  <a href="https://mkdocs-python-classy.readthedocs.io/en/latest"><img src="https://readthedocs.org/projects/mkdocs-python-classy/badge/"></a>
   <a href="https://pypi.org/project/mkdocs-python-classy/"><img src="https://img.shields.io/pypi/v/mkdocs-python-classy"></a>
   <a href="https://pypi.org/project/mkdocs-python-classy/"><img src="https://img.shields.io/pypi/dm/mkdocs-python-classy"></a>
   <br>
-  <!-- TODO: Replace: /en/latest with https://mkdocs-python-classy.readthedocs.io/en/latest -->
 </p>
 
 ## Overview
 
 A MkDocs plugin that helps you navigate the infuriating challenge of understanding a nested a Python class object. Trying to determine what attributes are available or what method does the class provide, and ultimately understanding the entire MRO (Method Resolution Order).
 
 ## Screenshots
@@ -32,28 +31,28 @@
 
 ![Methods](https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-classy/develop/docs/images/ui-view3.png)
 
 ## Documentation
 
 Full web-based HTML documentation for this library can be found over on the [mkdocs-python-classy Docs](https://mkdocs-python-classy.readthedocs.io) website:
 
-- [User Guide](/en/latest/user/lib_overview/) - Overview, Using the library, Getting Started.
-- [Administrator Guide](/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the library.
-- [Developer Guide](/en/latest/dev/contributing/) - Extending the library, Code Reference, Contribution Guide.
-- [Release Notes / Changelog](/en/latest/admin/release_notes/).
-- [Frequently Asked Questions](/en/latest/user/faq/).
+- [User Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/user/lib_overview/) - Overview, Using the library, Getting Started.
+- [Administrator Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the library.
+- [Developer Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/dev/contributing/) - Extending the library, Code Reference, Contribution Guide.
+- [Release Notes / Changelog](https://mkdocs-python-classy.readthedocs.io/en/latest/admin/release_notes/).
+- [Frequently Asked Questions](https://mkdocs-python-classy.readthedocs.io/en/latest/user/faq/).
 
 ### Contributing to the Docs
 
 All the Markdown source for the library documentation can be found under the [docs](https://github.com/itdependsnetworks/mkdocs-python-classy/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient - clone the repository and edit away.
 
-If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
+If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
 
 Any PRs with fixes or improvements are very welcome!
 
 ### Attribution
 
-This project is largely based on the work of [Classy Class-Based Views.](https://ccbv.co.uk/) and [Classy Django REST Framework](https://www.cdrf.co/), see - [Attribution](/en/latest/dev/contributing/) for more details.
+This project is largely based on the work of [Classy Class-Based Views.](https://ccbv.co.uk/) and [Classy Django REST Framework](https://www.cdrf.co/), see - [Attribution](https://mkdocs-python-classy.readthedocs.io/en/latest/dev/attribution/) for more details.
 
 ## Questions
 
-<!-- For any questions or comments, please check the [FAQ](/en/latest/user/faq/) first. Feel free to also swing by the [Network to Code Slack](https://networktocode.slack.com/) (channel `#networktocode`), sign up [here](http://slack.networktocode.com/) if you don't have an account. -->
+<!-- For any questions or comments, please check the [FAQ](https://mkdocs-python-classy.readthedocs.io/en/latest/user/faq/) first. Feel free to also swing by the [Network to Code Slack](https://networktocode.slack.com/) (channel `#networktocode`), sign up [here](http://slack.networktocode.com/) if you don't have an account. -->
```

#### html2text {}

```diff
@@ -1,13 +1,14 @@
 # mkdocs-python-classy
   [https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-classy/
               develop/docs/images/icon-mkdocs-python-classy.png]
-    [https://readthedocs.org/projects/mkdocs-python-classy/badge/] [https://
- img.shields.io/pypi/v/mkdocs-python-classy] [https://img.shields.io/pypi/dm/
-                            mkdocs-python-classy]
+ [https://github.com/itdependsnetworks/mkdocs-python-classy/actions/workflows/
+ci.yml/badge.svg?branch=main] [https://readthedocs.org/projects/mkdocs-python-
+ classy/badge/] [https://img.shields.io/pypi/v/mkdocs-python-classy] [https://
+                 img.shields.io/pypi/dm/mkdocs-python-classy]
 ## Overview A MkDocs plugin that helps you navigate the infuriating challenge
 of understanding a nested a Python class object. Trying to determine what
 attributes are available or what method does the class provide, and ultimately
 understanding the entire MRO (Method Resolution Order). ## Screenshots The
 library works like any other mkdocs plugin. From here you can see how the MRO
 is described, links to other Classes covered in the docs, and a convenience
 Python import config. ![MRO](https://raw.githubusercontent.com/
@@ -17,28 +18,32 @@
 develop/docs/images/ui-view2.png) From here you can see how the code of the
 method is shown with line numbers, it is collapsible, and will even show
 multiple if the method is provided in multiple Classes in the MRO order!
 Additionally you can see the naviagation pane that is auto generated. !
 [Methods](https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-
 classy/develop/docs/images/ui-view3.png) ## Documentation Full web-based HTML
 documentation for this library can be found over on the [mkdocs-python-classy
-Docs](https://mkdocs-python-classy.readthedocs.io) website: - [User Guide](/en/
-latest/user/lib_overview/) - Overview, Using the library, Getting Started. -
-[Administrator Guide](/en/latest/admin/install/) - How to Install, Configure,
-Upgrade, or Uninstall the library. - [Developer Guide](/en/latest/dev/
-contributing/) - Extending the library, Code Reference, Contribution Guide. -
-[Release Notes / Changelog](/en/latest/admin/release_notes/). - [Frequently
-Asked Questions](/en/latest/user/faq/). ### Contributing to the Docs All the
-Markdown source for the library documentation can be found under the [docs]
-(https://github.com/itdependsnetworks/mkdocs-python-classy/tree/develop/docs)
-folder in this repository. For simple edits, a Markdown capable editor is
-sufficient - clone the repository and edit away. If you need to view the fully
-generated documentation site, you can build it with [mkdocs](https://
-www.mkdocs.org/). A container hosting the docs will be started using the invoke
-commands (details in the [Development Environment Guide](/en/latest/dev/
-dev_environment/#docker-development-environment)) on [http://localhost:8001]
-(http://localhost:8001). As your changes are saved, the live docs will be
-automatically reloaded. Any PRs with fixes or improvements are very welcome!
-### Attribution This project is largely based on the work of [Classy Class-
-Based Views.](https://ccbv.co.uk/) and [Classy Django REST Framework](https://
-www.cdrf.co/), see - [Attribution](/en/latest/dev/contributing/) for more
-details. ## Questions
+Docs](https://mkdocs-python-classy.readthedocs.io) website: - [User Guide]
+(https://mkdocs-python-classy.readthedocs.io/en/latest/user/lib_overview/) -
+Overview, Using the library, Getting Started. - [Administrator Guide](https://
+mkdocs-python-classy.readthedocs.io/en/latest/admin/install/) - How to Install,
+Configure, Upgrade, or Uninstall the library. - [Developer Guide](https://
+mkdocs-python-classy.readthedocs.io/en/latest/dev/contributing/) - Extending
+the library, Code Reference, Contribution Guide. - [Release Notes / Changelog]
+(https://mkdocs-python-classy.readthedocs.io/en/latest/admin/release_notes/). -
+[Frequently Asked Questions](https://mkdocs-python-classy.readthedocs.io/en/
+latest/user/faq/). ### Contributing to the Docs All the Markdown source for the
+library documentation can be found under the [docs](https://github.com/
+itdependsnetworks/mkdocs-python-classy/tree/develop/docs) folder in this
+repository. For simple edits, a Markdown capable editor is sufficient - clone
+the repository and edit away. If you need to view the fully generated
+documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A
+container hosting the docs will be started using the invoke commands (details
+in the [Development Environment Guide](https://mkdocs-python-
+classy.readthedocs.io/en/latest/dev/dev_environment/#docker-development-
+environment)) on [http://localhost:8001](http://localhost:8001). As your
+changes are saved, the live docs will be automatically reloaded. Any PRs with
+fixes or improvements are very welcome! ### Attribution This project is largely
+based on the work of [Classy Class-Based Views.](https://ccbv.co.uk/) and
+[Classy Django REST Framework](https://www.cdrf.co/), see - [Attribution]
+(https://mkdocs-python-classy.readthedocs.io/en/latest/dev/attribution/) for
+more details. ## Questions
```

### Comparing `mkdocs_python_classy-0.1.2/mkdocs_python_classy/__init__.py` & `mkdocs_python_classy-0.1.3/mkdocs_python_classy/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import re
 import os
 
 from shutil import copy
 from string import Template
 from typing import Optional
-from importlib_metadata import version
+from importlib.metadata import version
 
 from mkdocs.config import config_options
 from mkdocs.config.base import Config
 from mkdocs.config.defaults import MkDocsConfig
 from mkdocs.plugins import BasePlugin
 from mkdocs.structure.files import Files
 from mkdocs.structure.pages import Page
```

### Comparing `mkdocs_python_classy-0.1.2/mkdocs_python_classy/inspector.py` & `mkdocs_python_classy-0.1.3/mkdocs_python_classy/inspector.py`

 * *Files identical despite different names*

### Comparing `mkdocs_python_classy-0.1.2/mkdocs_python_classy/utils.py` & `mkdocs_python_classy-0.1.3/mkdocs_python_classy/utils.py`

 * *Files identical despite different names*

### Comparing `mkdocs_python_classy-0.1.2/pyproject.toml` & `mkdocs_python_classy-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mkdocs-python-classy"
-version = "v0.1.2"
+version = "v0.1.3"
 description = "Mkdocs plugin to view Python Classes."
 authors = ["Ken Celenza <ken@celenza.org>"]
 license = "Apache"
 readme = "README.md"
 keywords = ["mkdocs"]
 classifiers = [
     "Intended Audience :: Developers",
```

### Comparing `mkdocs_python_classy-0.1.2/PKG-INFO` & `mkdocs_python_classy-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-python-classy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Mkdocs plugin to view Python Classes.
 License: Apache
 Keywords: mkdocs
 Author: Ken Celenza
 Author-email: ken@celenza.org
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,20 +22,19 @@
 
 # mkdocs-python-classy
 
 <p align="center">
 
   <img src="https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-classy/develop/docs/images/icon-mkdocs-python-classy.png" class="logo" height="100px">
   <br>
-  <!-- <a href="https://github.com/networktocode/mkdocs-python-classy/actions"><img src="https://github.com/networktocode/mkdocs-python-classy/actions/workflows/ci.yml/badge.svg?branch=main"></a> -->
-  <a href="/en/latest"><img src="https://readthedocs.org/projects/mkdocs-python-classy/badge/"></a>
+  <a href="https://github.com/itdependsnetworks/mkdocs-python-classy/actions"><img src="https://github.com/itdependsnetworks/mkdocs-python-classy/actions/workflows/ci.yml/badge.svg?branch=main"></a>
+  <a href="https://mkdocs-python-classy.readthedocs.io/en/latest"><img src="https://readthedocs.org/projects/mkdocs-python-classy/badge/"></a>
   <a href="https://pypi.org/project/mkdocs-python-classy/"><img src="https://img.shields.io/pypi/v/mkdocs-python-classy"></a>
   <a href="https://pypi.org/project/mkdocs-python-classy/"><img src="https://img.shields.io/pypi/dm/mkdocs-python-classy"></a>
   <br>
-  <!-- TODO: Replace: /en/latest with https://mkdocs-python-classy.readthedocs.io/en/latest -->
 </p>
 
 ## Overview
 
 A MkDocs plugin that helps you navigate the infuriating challenge of understanding a nested a Python class object. Trying to determine what attributes are available or what method does the class provide, and ultimately understanding the entire MRO (Method Resolution Order).
 
 ## Screenshots
@@ -54,29 +53,29 @@
 
 ![Methods](https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-classy/develop/docs/images/ui-view3.png)
 
 ## Documentation
 
 Full web-based HTML documentation for this library can be found over on the [mkdocs-python-classy Docs](https://mkdocs-python-classy.readthedocs.io) website:
 
-- [User Guide](/en/latest/user/lib_overview/) - Overview, Using the library, Getting Started.
-- [Administrator Guide](/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the library.
-- [Developer Guide](/en/latest/dev/contributing/) - Extending the library, Code Reference, Contribution Guide.
-- [Release Notes / Changelog](/en/latest/admin/release_notes/).
-- [Frequently Asked Questions](/en/latest/user/faq/).
+- [User Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/user/lib_overview/) - Overview, Using the library, Getting Started.
+- [Administrator Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/admin/install/) - How to Install, Configure, Upgrade, or Uninstall the library.
+- [Developer Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/dev/contributing/) - Extending the library, Code Reference, Contribution Guide.
+- [Release Notes / Changelog](https://mkdocs-python-classy.readthedocs.io/en/latest/admin/release_notes/).
+- [Frequently Asked Questions](https://mkdocs-python-classy.readthedocs.io/en/latest/user/faq/).
 
 ### Contributing to the Docs
 
 All the Markdown source for the library documentation can be found under the [docs](https://github.com/itdependsnetworks/mkdocs-python-classy/tree/develop/docs) folder in this repository. For simple edits, a Markdown capable editor is sufficient - clone the repository and edit away.
 
-If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
+If you need to view the fully generated documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A container hosting the docs will be started using the invoke commands (details in the [Development Environment Guide](https://mkdocs-python-classy.readthedocs.io/en/latest/dev/dev_environment/#docker-development-environment)) on [http://localhost:8001](http://localhost:8001). As your changes are saved, the live docs will be automatically reloaded.
 
 Any PRs with fixes or improvements are very welcome!
 
 ### Attribution
 
-This project is largely based on the work of [Classy Class-Based Views.](https://ccbv.co.uk/) and [Classy Django REST Framework](https://www.cdrf.co/), see - [Attribution](/en/latest/dev/contributing/) for more details.
+This project is largely based on the work of [Classy Class-Based Views.](https://ccbv.co.uk/) and [Classy Django REST Framework](https://www.cdrf.co/), see - [Attribution](https://mkdocs-python-classy.readthedocs.io/en/latest/dev/attribution/) for more details.
 
 ## Questions
 
-<!-- For any questions or comments, please check the [FAQ](/en/latest/user/faq/) first. Feel free to also swing by the [Network to Code Slack](https://networktocode.slack.com/) (channel `#networktocode`), sign up [here](http://slack.networktocode.com/) if you don't have an account. -->
+<!-- For any questions or comments, please check the [FAQ](https://mkdocs-python-classy.readthedocs.io/en/latest/user/faq/) first. Feel free to also swing by the [Network to Code Slack](https://networktocode.slack.com/) (channel `#networktocode`), sign up [here](http://slack.networktocode.com/) if you don't have an account. -->
```

#### html2text {}

```diff
@@ -1,23 +1,24 @@
-Metadata-Version: 2.1 Name: mkdocs-python-classy Version: 0.1.2 Summary: Mkdocs
+Metadata-Version: 2.1 Name: mkdocs-python-classy Version: 0.1.3 Summary: Mkdocs
 plugin to view Python Classes. License: Apache Keywords: mkdocs Author: Ken
 Celenza Author-email: ken@celenza.org Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 5 - Production/Stable Classifier: Intended Audience ::
 Developers Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Requires-Dist: astunparse (>=1.6.3,<2.0.0) ; python_version <
 "3.9" Requires-Dist: mkdocs (>=1.4.0,<2.0.0) Requires-Dist: pymdown-extensions
 (>=6.3) Description-Content-Type: text/markdown # mkdocs-python-classy
   [https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-classy/
               develop/docs/images/icon-mkdocs-python-classy.png]
-    [https://readthedocs.org/projects/mkdocs-python-classy/badge/] [https://
- img.shields.io/pypi/v/mkdocs-python-classy] [https://img.shields.io/pypi/dm/
-                            mkdocs-python-classy]
+ [https://github.com/itdependsnetworks/mkdocs-python-classy/actions/workflows/
+ci.yml/badge.svg?branch=main] [https://readthedocs.org/projects/mkdocs-python-
+ classy/badge/] [https://img.shields.io/pypi/v/mkdocs-python-classy] [https://
+                 img.shields.io/pypi/dm/mkdocs-python-classy]
 ## Overview A MkDocs plugin that helps you navigate the infuriating challenge
 of understanding a nested a Python class object. Trying to determine what
 attributes are available or what method does the class provide, and ultimately
 understanding the entire MRO (Method Resolution Order). ## Screenshots The
 library works like any other mkdocs plugin. From here you can see how the MRO
 is described, links to other Classes covered in the docs, and a convenience
 Python import config. ![MRO](https://raw.githubusercontent.com/
@@ -27,28 +28,32 @@
 develop/docs/images/ui-view2.png) From here you can see how the code of the
 method is shown with line numbers, it is collapsible, and will even show
 multiple if the method is provided in multiple Classes in the MRO order!
 Additionally you can see the naviagation pane that is auto generated. !
 [Methods](https://raw.githubusercontent.com/itdependsnetworks/mkdocs-python-
 classy/develop/docs/images/ui-view3.png) ## Documentation Full web-based HTML
 documentation for this library can be found over on the [mkdocs-python-classy
-Docs](https://mkdocs-python-classy.readthedocs.io) website: - [User Guide](/en/
-latest/user/lib_overview/) - Overview, Using the library, Getting Started. -
-[Administrator Guide](/en/latest/admin/install/) - How to Install, Configure,
-Upgrade, or Uninstall the library. - [Developer Guide](/en/latest/dev/
-contributing/) - Extending the library, Code Reference, Contribution Guide. -
-[Release Notes / Changelog](/en/latest/admin/release_notes/). - [Frequently
-Asked Questions](/en/latest/user/faq/). ### Contributing to the Docs All the
-Markdown source for the library documentation can be found under the [docs]
-(https://github.com/itdependsnetworks/mkdocs-python-classy/tree/develop/docs)
-folder in this repository. For simple edits, a Markdown capable editor is
-sufficient - clone the repository and edit away. If you need to view the fully
-generated documentation site, you can build it with [mkdocs](https://
-www.mkdocs.org/). A container hosting the docs will be started using the invoke
-commands (details in the [Development Environment Guide](/en/latest/dev/
-dev_environment/#docker-development-environment)) on [http://localhost:8001]
-(http://localhost:8001). As your changes are saved, the live docs will be
-automatically reloaded. Any PRs with fixes or improvements are very welcome!
-### Attribution This project is largely based on the work of [Classy Class-
-Based Views.](https://ccbv.co.uk/) and [Classy Django REST Framework](https://
-www.cdrf.co/), see - [Attribution](/en/latest/dev/contributing/) for more
-details. ## Questions
+Docs](https://mkdocs-python-classy.readthedocs.io) website: - [User Guide]
+(https://mkdocs-python-classy.readthedocs.io/en/latest/user/lib_overview/) -
+Overview, Using the library, Getting Started. - [Administrator Guide](https://
+mkdocs-python-classy.readthedocs.io/en/latest/admin/install/) - How to Install,
+Configure, Upgrade, or Uninstall the library. - [Developer Guide](https://
+mkdocs-python-classy.readthedocs.io/en/latest/dev/contributing/) - Extending
+the library, Code Reference, Contribution Guide. - [Release Notes / Changelog]
+(https://mkdocs-python-classy.readthedocs.io/en/latest/admin/release_notes/). -
+[Frequently Asked Questions](https://mkdocs-python-classy.readthedocs.io/en/
+latest/user/faq/). ### Contributing to the Docs All the Markdown source for the
+library documentation can be found under the [docs](https://github.com/
+itdependsnetworks/mkdocs-python-classy/tree/develop/docs) folder in this
+repository. For simple edits, a Markdown capable editor is sufficient - clone
+the repository and edit away. If you need to view the fully generated
+documentation site, you can build it with [mkdocs](https://www.mkdocs.org/). A
+container hosting the docs will be started using the invoke commands (details
+in the [Development Environment Guide](https://mkdocs-python-
+classy.readthedocs.io/en/latest/dev/dev_environment/#docker-development-
+environment)) on [http://localhost:8001](http://localhost:8001). As your
+changes are saved, the live docs will be automatically reloaded. Any PRs with
+fixes or improvements are very welcome! ### Attribution This project is largely
+based on the work of [Classy Class-Based Views.](https://ccbv.co.uk/) and
+[Classy Django REST Framework](https://www.cdrf.co/), see - [Attribution]
+(https://mkdocs-python-classy.readthedocs.io/en/latest/dev/attribution/) for
+more details. ## Questions
```

