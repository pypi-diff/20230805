# Comparing `tmp/inducoapi-2.1.0.tar.gz` & `tmp/inducoapi-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "inducoapi-2.1.0.tar", max compression
+gzip compressed data, was "inducoapi-2.1.1.tar", max compression
```

## Comparing `inducoapi-2.1.0.tar` & `inducoapi-2.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11357 2023-06-25 13:26:11.895038 inducoapi-2.1.0/LICENSE
--rw-r--r--   0        0        0     6159 2023-06-25 13:26:11.895038 inducoapi-2.1.0/README.md
--rw-r--r--   0        0        0       88 2023-06-25 13:26:11.895038 inducoapi-2.1.0/inducoapi/__init__.py
--rwxr-xr-x   0        0        0     5431 2023-06-25 13:26:11.895038 inducoapi-2.1.0/inducoapi/__main__.py
--rwxr-xr-x   0        0        0     6149 2023-06-25 13:26:11.895038 inducoapi-2.1.0/inducoapi/inducoapi.py
--rw-r--r--   0        0        0      688 2023-06-25 13:26:11.895038 inducoapi-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     7279 1970-01-01 00:00:00.000000 inducoapi-2.1.0/setup.py
--rw-r--r--   0        0        0     7055 1970-01-01 00:00:00.000000 inducoapi-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-08-05 16:43:34.443171 inducoapi-2.1.1/LICENSE
+-rw-r--r--   0        0        0     6159 2023-08-05 16:43:34.443171 inducoapi-2.1.1/README.md
+-rw-r--r--   0        0        0       88 2023-08-05 16:43:34.447171 inducoapi-2.1.1/inducoapi/__init__.py
+-rwxr-xr-x   0        0        0     5431 2023-08-05 16:43:34.447171 inducoapi-2.1.1/inducoapi/__main__.py
+-rwxr-xr-x   0        0        0     6149 2023-08-05 16:43:34.447171 inducoapi-2.1.1/inducoapi/inducoapi.py
+-rw-r--r--   0        0        0      688 2023-08-05 16:43:34.447171 inducoapi-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7279 1970-01-01 00:00:00.000000 inducoapi-2.1.1/setup.py
+-rw-r--r--   0        0        0     7005 1970-01-01 00:00:00.000000 inducoapi-2.1.1/PKG-INFO
```

### Comparing `inducoapi-2.1.0/LICENSE` & `inducoapi-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `inducoapi-2.1.0/README.md` & `inducoapi-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `inducoapi-2.1.0/inducoapi/__main__.py` & `inducoapi-2.1.1/inducoapi/__main__.py`

 * *Files identical despite different names*

### Comparing `inducoapi-2.1.0/inducoapi/inducoapi.py` & `inducoapi-2.1.1/inducoapi/inducoapi.py`

 * *Files identical despite different names*

### Comparing `inducoapi-2.1.0/pyproject.toml` & `inducoapi-2.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "inducoapi"
-version = "2.1.0"
+version = "2.1.1"
 description = "A simple python program to generate OpenApi documentation by supplying request/response bodies."
 authors = ["Matteo Pergolesi <matpergo@gmail.com>"]
 license = "Apache License 2.0"
 readme = 'README.md'
 repository = "https://github.com/TheWall89/inducoapi"
 homepage = "https://github.com/TheWall89/inducoapi"
 keywords = ['openapi', 'rest']
 
 [tool.poetry.dependencies]
-python = "^3.7.0"
+python = "^3.8.0"
 pyyaml = "^6.0"
-openapi-spec-validator = "^0.5"
+openapi-spec-validator = "^0.6"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 
 [tool.poetry.scripts]
 inducoapi = 'inducoapi.__main__:main'
 [build-system]
```

### Comparing `inducoapi-2.1.0/setup.py` & `inducoapi-2.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,31 @@
 packages = \
 ['inducoapi']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['openapi-spec-validator>=0.5,<0.6', 'pyyaml>=6.0,<7.0']
+['openapi-spec-validator>=0.6,<0.7', 'pyyaml>=6.0,<7.0']
 
 entry_points = \
 {'console_scripts': ['inducoapi = inducoapi.__main__:main']}
 
 setup_kwargs = {
     'name': 'inducoapi',
-    'version': '2.1.0',
+    'version': '2.1.1',
     'description': 'A simple python program to generate OpenApi documentation by supplying request/response bodies.',
     'long_description': "# InducOapi\n\n[![ci](https://github.com/TheWall89/inducoapi/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/TheWall89/inducoapi/actions/workflows/ci.yml)\n[![PyPI version](https://badge.fury.io/py/inducoapi.svg)](https://badge.fury.io/py/inducoapi)\n\nA simple python module to generate OpenAPI Description Documents by supplying request/response bodies.\n\n*Contributions for new features, fixes or improvements are welcome. Feel free to send a pull request.*\n\n## Motivation\n\nSometimes you have a fully functioning HTTP service without OpenAPI documentation. At some point in time, others may\nneed to use your service. Writing the documentation by hand is a pain and can feel like an overwhelming job for complex\nservices.\n*inducoapi* helps you generate your OpenAPI Description Documents by taking as input request/response examples plus some\nother information.\n\nThe generated OpenAPI documentation is validated\nwith [openapi-spec-validator](https://github.com/p1c2u/openapi-spec-validator).\n\n*Warning*: This program also generates the `example` fields in OpenAPI schemas by default. If you have sensitive data in\nyour request/response files, disable this feature with `--no-example`.\n\n## Installation\n\n### With `pip`\n\n```shell script\npip install inducoapi\n```\n\n### With [poetry](https://python-poetry.org/)\n\n```shell script\ngit clone git@github.com:TheWall89/inducoapi.git\ncd inducoapi\npoetry install\n```\n\nTo run unit-tests:\n\n```shell script\npoetry run pytest\n```\n\n## Usage\n\n### From CLI\n\n`inducoapi` provides its own command. You can simply execute it with\n\n```shell script\ninducoapi\n```\n\nIf you get a `command not found` error, try to activate your virtualenv or run `poetry shell` first.\n\nYou can also run `inducoapi` in the classic way:\n\n```shell script\npython -m inducoapi\n```\n\n#### Help\n\n`inducoapi` provides its own help. Check it out with:\n\n```shell script\npython -m inducoapi -h\n```\n\n#### Examples\n\nLet's consider a simple case: you have an HTTP service managing employees. We want to generate the OpenAPI Description\nDocument for a GET on all the employees, returning a 200 status code:\n\n```shell script\npython -m inducoapi GET /employees 200\n```\n\n<details><summary>output</summary>\n\n```yaml\nopenapi: 3.0.0\ninfo:\n  title: Generated by InducOapi\n  version: v1\npaths:\n  /employees:\n    get:\n      responses:\n        200:\n          description: ''\n```\n\n</details>\n\nNow, a GET request with an empty response is not quite useful. Let's add an argument with a JSON file containing a\nresponse example. Input examples can be found in [examples](examples).\n\n```shell script\npython -m inducoapi GET /employees 200 --response examples/employees.json\n```\n\n<details><summary>output</summary>\n\n```yaml\nopenapi: 3.0.0\ninfo:\n  title: Generated by InducOapi\n  version: v1\npaths:\n  /employees:\n    get:\n      responses:\n        200:\n          description: ''\n          content:\n            application/json:\n              schema:\n                type: array\n                items:\n                  type: object\n                  properties:\n                    id:\n                      type: integer\n                      example: 1\n                    name:\n                      type: string\n                      example: Dwight Schrute\n                    role:\n                      type: string\n                      example: salesman\n```\n\n</details>\n\nLet's add a parameter to filter the employees by name.\n\n```shell script\npython -m inducoapi GET /employees 200 --response examples/employees.json --parameter name,query \n```\n\n<details><summary>output</summary>\n\n```yaml\nopenapi: 3.0.0\ninfo:\n  title: Generated by InducOapi\n  version: v1\npaths:\n  /employees:\n    get:\n      responses:\n        '200':\n          description: ''\n          content:\n            application/json:\n              schema:\n                type: array\n                items:\n                  type: object\n                  properties:\n                    id:\n                      type: integer\n                      example: 1\n                    name:\n                      type: string\n                      example: Dwight Schrute\n                    role:\n                      type: string\n                      example: salesman\n      parameters:\n        - name: name\n          in: query\n          required: false\n          description: ''\n          schema: { }\n```\n\n</details>\n\nFinally, let's try a POST request with both request and response examples.\n\n```shell script\npython -m inducoapi POST /employees 201 --request examples/new_employee_req.json --response examples/new_employee_resp.json\n```\n\n<details><summary>output</summary>\n\n```yaml\nopenapi: 3.0.0\ninfo:\n  title: Generated by InducOapi\n  version: v1\npaths:\n  /employees:\n    post:\n      requestBody:\n        content:\n          application/json:\n            schema:\n              type: object\n              properties:\n                name:\n                  type: string\n                  example: Michael Scott\n                role:\n                  type: string\n                  example: manager\n      responses:\n        201:\n          description: ''\n          content:\n            application/json:\n              schema:\n                type: object\n                properties:\n                  id:\n                    type: integer\n                    example: 4\n                  name:\n                    type: string\n                    example: Michael Scott\n                  role:\n                    type: string\n                    example: manager\n```\n\n</details>\n\nIf you want to directly write the generated OpenAPI Description Documents to a YAML file, just\nadd `--output openapi.yaml`\n\n### From python\n\n[test_inducoapi.py](tests/test_inducoapi.py) provides usage examples of the module from python.\n\n## TODO list\n\n- [x] Add support for request/response files in YAML\n- [x] Add support for `application/yaml` content\n- [x] Customize title and version in info\n- [x] Package module\n- [x] Support for `$ref` in response schemas\n- [x] Add support for `parameters`\n- [ ] ~~Add support for `links`~~ (I don't think it is very useful)\n- [ ] ~~Add support for `format`~~ (hard to infer)\n",
     'author': 'Matteo Pergolesi',
     'author_email': 'matpergo@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/TheWall89/inducoapi',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'entry_points': entry_points,
-    'python_requires': '>=3.7.0,<4.0.0',
+    'python_requires': '>=3.8.0,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `inducoapi-2.1.0/PKG-INFO` & `inducoapi-2.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: inducoapi
-Version: 2.1.0
+Version: 2.1.1
 Summary: A simple python program to generate OpenApi documentation by supplying request/response bodies.
 Home-page: https://github.com/TheWall89/inducoapi
 License: Apache-2.0
 Keywords: openapi,rest
 Author: Matteo Pergolesi
 Author-email: matpergo@gmail.com
-Requires-Python: >=3.7.0,<4.0.0
+Requires-Python: >=3.8.0,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openapi-spec-validator (>=0.5,<0.6)
+Requires-Dist: openapi-spec-validator (>=0.6,<0.7)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Project-URL: Repository, https://github.com/TheWall89/inducoapi
 Description-Content-Type: text/markdown
 
 # InducOapi
 
 [![ci](https://github.com/TheWall89/inducoapi/actions/workflows/ci.yml/badge.svg?branch=master)](https://github.com/TheWall89/inducoapi/actions/workflows/ci.yml)
```

