# Comparing `tmp/slack-logger-python-0.4.0.tar.gz` & `tmp/slack-logger-python-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slack-logger-python-0.4.0.tar", last modified: Wed Aug  2 00:51:27 2023, max compression
+gzip compressed data, was "slack-logger-python-0.5.0.tar", last modified: Sat Aug  5 00:50:30 2023, max compression
```

## Comparing `slack-logger-python-0.4.0.tar` & `slack-logger-python-0.5.0.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.envrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.279563 slack-logger-python-0.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.github/workflows/format.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.github/workflows/tagging.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8242 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-02 00:51:19.000000 slack-logger-python-0.4.0/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/shell.nix
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/slack_logger/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/slack_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/slack_logger/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/slack_logger_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9337 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-02 00:51:27.000000 slack-logger-python-0.4.0/slack_logger_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:27.283563 slack-logger-python-0.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-02 00:51:16.000000 slack-logger-python-0.4.0/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.959026 slack-logger-python-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.envrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.951026 slack-logger-python-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.955026 slack-logger-python-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.github/workflows/format.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.github/workflows/tagging.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.955026 slack-logger-python-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-08-05 00:50:30.959026 slack-logger-python-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8361 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 00:50:21.000000 slack-logger-python-0.5.0/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:50:30.959026 slack-logger-python-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/shell.nix
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.959026 slack-logger-python-0.5.0/slack_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/slack_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/slack_logger/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.959026 slack-logger-python-0.5.0/slack_logger_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9456 2023-08-05 00:50:30.000000 slack-logger-python-0.5.0/slack_logger_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-08-05 00:50:30.000000 slack-logger-python-0.5.0/slack_logger_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:50:30.000000 slack-logger-python-0.5.0/slack_logger_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-05 00:50:30.000000 slack-logger-python-0.5.0/slack_logger_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 00:50:30.000000 slack-logger-python-0.5.0/slack_logger_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:30.959026 slack-logger-python-0.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/tests/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-05 00:50:16.000000 slack-logger-python-0.5.0/tests/utils.py
```

### Comparing `slack-logger-python-0.4.0/.github/workflows/deploy.yml` & `slack-logger-python-0.5.0/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/.github/workflows/format.yml` & `slack-logger-python-0.5.0/.github/workflows/format.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/.github/workflows/tagging.yml` & `slack-logger-python-0.5.0/.github/workflows/tagging.yml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/.gitignore` & `slack-logger-python-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/LICENSE` & `slack-logger-python-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/PKG-INFO` & `slack-logger-python-0.5.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -68,20 +68,20 @@
 
 You can use the `SlackFormatter.minimal()` and `SlackFormatter.default()` formatter for more visually appealing log messages.
 For now, those require a configuration to show e.g. the header.
 Extra fields are shown in blocks at the bottom of the message and can be dynamically added at runtime.
 Everything else stays the same:
 
 ```python
-from slack_logger import Configuration, SlackFormatter, SlackHandler
+from slack_logger import FormatConfig, SlackFormatter, SlackHandler
 
 logger = logging.getLogger(__name__)
 
-config = Configuration(service="testrunner", environment="test", extra_fields={"foo": "bar"})
-formatter = SlackFormatter.default(config)
+format_config = FormatConfig(service="testrunner", environment="test", extra_fields={"foo": "bar"})
+formatter = SlackFormatter.default(format_config)
 handler = SlackHandler.from_webhook(os.environ["SLACK_WEBHOOK"])
 handler.setFormatter(formatter)
 handler.setLevel(logging.WARN)
 
 logger.addHandler(handler)
 
 logger.info("I won't appear.")
@@ -107,20 +107,20 @@
 ```
 
 Let's look at an example error log from a division by zero error.
 Given the following code snippet with a configuration and the default formatter:
 
 ```python
 import os
-from slack_logger import Configuration, SlackFormatter, SlackHandler
-service_config = Configuration(
+from slack_logger import FormatConfig, SlackFormatter, SlackHandler
+format_config = FormatConfig(
     service="testrunner", environment="test", extra_fields={"foo": "bar", "raven": "caw"}
 )
 slack_handler = SlackHandler.from_webhook(os.environ["SLACK_WEBHOOK"])
-formatter = SlackFormatter.default(service_config)
+formatter = SlackFormatter.default(format_config)
 slack_handler.setFormatter(formatter)
 log.addHandler(slack_handler)
 try:
     1/0
 except Exception:
     log.exception("Something terrible happened!")
 ```
@@ -196,45 +196,45 @@
 }
 ```
 
 You can import and overwrite it partially, or define a complete new set of emoji.
 The following example demonstrates how you can add the emoji set to the `SlackFormatter`:
 
 ```python
-from slack_logger import Configuration, SlackFormatter
+from slack_logger import FormatConfig, SlackFormatter
 
 my_emojis = {
     logging.CRITICAL: ":x:",    # ❌
     logging.ERROR: ":x:",       # ❌
     logging.FATAL: ":x:",       # ❌
     logging.WARNING: ":bell:",  # 🔔
     logging.WARN: ":bell:",     # 🔔
     logging.INFO: ":mega:",     # 📣
     logging.DEBUG: ":mega:",    # 📣
     logging.NOTSET: ":mega:",   # 📣
 }
 
-config = Configuration(service="testrunner", environment="test", emojis=my_emojis)
+config = FormatConfig(service="testrunner", environment="test", emojis=my_emojis)
 formatter = SlackFormatter.default(config)
 ```
 
 
 ### Filter Message
 
 Filters implement the logging interface of `Filters`.
 Design goal (4) and (5) are partially demonstrated.
 
 ```python
-from slack_logger import Configuration, SlackFilter, SlackHandler
+from slack_logger import FilterConfig, SlackFilter, SlackHandler
 import os
 import logging 
 
 logger = logging.getLogger("ProdFilter")
 # Allow only logs from `prod` environment
-filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyAllowList)
+filter = SlackFilter(config=FilterConfig(environment="prod"), filterType=FilterType.AnyAllowList)
 slack_handler.addFilter(filter)
 logger.addHandler(slack_handler)
 
 
 # When the ENV enviroment variable is set to prod, the message will be send.
 # Otherwise, the message is filtered out and not send (e.g. if ENV is `dev`)
 logger.warning(f"{log_msg} in some environment and allow listed prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
@@ -243,7 +243,9 @@
 logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "dev"}})
 
 # Will be send
 logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "prod"}})
 ```
 
 The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
+
+More examples can be found it the [tests folder](https://github.com/GRBurst/slack-logger-python/tree/main/tests).
```

### Comparing `slack-logger-python-0.4.0/README.md` & `slack-logger-python-0.5.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,20 +46,20 @@
 
 You can use the `SlackFormatter.minimal()` and `SlackFormatter.default()` formatter for more visually appealing log messages.
 For now, those require a configuration to show e.g. the header.
 Extra fields are shown in blocks at the bottom of the message and can be dynamically added at runtime.
 Everything else stays the same:
 
 ```python
-from slack_logger import Configuration, SlackFormatter, SlackHandler
+from slack_logger import FormatConfig, SlackFormatter, SlackHandler
 
 logger = logging.getLogger(__name__)
 
-config = Configuration(service="testrunner", environment="test", extra_fields={"foo": "bar"})
-formatter = SlackFormatter.default(config)
+format_config = FormatConfig(service="testrunner", environment="test", extra_fields={"foo": "bar"})
+formatter = SlackFormatter.default(format_config)
 handler = SlackHandler.from_webhook(os.environ["SLACK_WEBHOOK"])
 handler.setFormatter(formatter)
 handler.setLevel(logging.WARN)
 
 logger.addHandler(handler)
 
 logger.info("I won't appear.")
@@ -85,20 +85,20 @@
 ```
 
 Let's look at an example error log from a division by zero error.
 Given the following code snippet with a configuration and the default formatter:
 
 ```python
 import os
-from slack_logger import Configuration, SlackFormatter, SlackHandler
-service_config = Configuration(
+from slack_logger import FormatConfig, SlackFormatter, SlackHandler
+format_config = FormatConfig(
     service="testrunner", environment="test", extra_fields={"foo": "bar", "raven": "caw"}
 )
 slack_handler = SlackHandler.from_webhook(os.environ["SLACK_WEBHOOK"])
-formatter = SlackFormatter.default(service_config)
+formatter = SlackFormatter.default(format_config)
 slack_handler.setFormatter(formatter)
 log.addHandler(slack_handler)
 try:
     1/0
 except Exception:
     log.exception("Something terrible happened!")
 ```
@@ -174,45 +174,45 @@
 }
 ```
 
 You can import and overwrite it partially, or define a complete new set of emoji.
 The following example demonstrates how you can add the emoji set to the `SlackFormatter`:
 
 ```python
-from slack_logger import Configuration, SlackFormatter
+from slack_logger import FormatConfig, SlackFormatter
 
 my_emojis = {
     logging.CRITICAL: ":x:",    # ❌
     logging.ERROR: ":x:",       # ❌
     logging.FATAL: ":x:",       # ❌
     logging.WARNING: ":bell:",  # 🔔
     logging.WARN: ":bell:",     # 🔔
     logging.INFO: ":mega:",     # 📣
     logging.DEBUG: ":mega:",    # 📣
     logging.NOTSET: ":mega:",   # 📣
 }
 
-config = Configuration(service="testrunner", environment="test", emojis=my_emojis)
+config = FormatConfig(service="testrunner", environment="test", emojis=my_emojis)
 formatter = SlackFormatter.default(config)
 ```
 
 
 ### Filter Message
 
 Filters implement the logging interface of `Filters`.
 Design goal (4) and (5) are partially demonstrated.
 
 ```python
-from slack_logger import Configuration, SlackFilter, SlackHandler
+from slack_logger import FilterConfig, SlackFilter, SlackHandler
 import os
 import logging 
 
 logger = logging.getLogger("ProdFilter")
 # Allow only logs from `prod` environment
-filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyAllowList)
+filter = SlackFilter(config=FilterConfig(environment="prod"), filterType=FilterType.AnyAllowList)
 slack_handler.addFilter(filter)
 logger.addHandler(slack_handler)
 
 
 # When the ENV enviroment variable is set to prod, the message will be send.
 # Otherwise, the message is filtered out and not send (e.g. if ENV is `dev`)
 logger.warning(f"{log_msg} in some environment and allow listed prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
@@ -220,8 +220,10 @@
 # Will be filtered
 logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "dev"}})
 
 # Will be send
 logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "prod"}})
 ```
 
-The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
+The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
+
+More examples can be found it the [tests folder](https://github.com/GRBurst/slack-logger-python/tree/main/tests).
```

### Comparing `slack-logger-python-0.4.0/pyproject.toml` & `slack-logger-python-0.5.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/shell.nix` & `slack-logger-python-0.5.0/shell.nix`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/slack_logger/__init__.py` & `slack-logger-python-0.5.0/slack_logger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 import json
 import logging
 from abc import ABC, abstractmethod
 from enum import Enum
 from logging import LogRecord
 from typing import Any, Dict, List, Optional, Sequence, Union
 
-from attrs import define
+from attrs import asdict, define
+from cattrs import structure
 from slack_sdk.models.attachments import Attachment
 from slack_sdk.models.blocks import Block, ContextBlock, DividerBlock, HeaderBlock, SectionBlock
 from slack_sdk.models.blocks.basic_components import MarkdownTextObject, PlainTextObject
 from slack_sdk.webhook.async_client import AsyncWebhookClient
 from slack_sdk.webhook.webhook_response import WebhookResponse
 
 log = logging.getLogger("slack_logger")
@@ -204,15 +205,15 @@
         super().format(record)
         return self.design.format(record)
 
 
 class SlackFilter(logging.Filter):
     config: FilterConfig
 
-    def __init__(self, config: FilterConfig):
+    def __init__(self, config: FilterConfig = FilterConfig()):
         super(SlackFilter, self).__init__()
         self.config = config
 
     @classmethod
     def filter_by_fields(
         cls, fields: Dict[str, str], filter_type: FilterType = FilterType.AnyAllowList, use_regex: bool = False
     ) -> "SlackFilter":
@@ -324,18 +325,20 @@
 
         log.debug(t)
         return WebhookResponse(url="", status_code=200, body="ok", headers={})
 
 
 class SlackHandler(logging.Handler):
     client: AsyncWebhookClient
+    config: LogConfig
 
-    def __init__(self, client: AsyncWebhookClient):
+    def __init__(self, client: AsyncWebhookClient, config: LogConfig = LogConfig()):
         super(SlackHandler, self).__init__()
         self.client = client
+        self.config = config
 
     @classmethod
     def from_webhook(cls, webhook_url: str) -> "SlackHandler":
         return cls(
             client=AsyncWebhookClient(webhook_url),
         )
 
@@ -366,15 +369,27 @@
 
         except Exception:
             self.handleError(record)
 
     def handle(self, record: LogRecord) -> bool:
         # This pre-filters the messages with the Slack Filters
         if isinstance(self.formatter, SlackFormatter) and self.formatter.config is not None:
-            format_config: LogConfig = self.formatter.config
+            combined_config: LogConfig = structure(
+                {
+                    **asdict(self.formatter.config),
+                    **{k: v for k, v in asdict(self.config).items() if v is not None},  # overwrite non None values
+                },
+                LogConfig,
+            )
+            log.debug(f"handler config: {self.config}")
+            log.debug(f"formatter config: {self.formatter.config}")
+            log.debug(f"combined config: {combined_config}")
             for sf in self.filters:
                 if isinstance(sf, SlackFilter):
-                    res = sf.filterConfig(serviceConfig=format_config, record=record)
-                    if not res:
+                    if sf.config.use_regex is True:
+                        res = sf.regexFilterConfig(serviceConfig=combined_config, record=record)
+                    else:
+                        res = sf.filterConfig(serviceConfig=combined_config, record=record)
+                    if res is False:
                         return False
 
         return super().handle(record)
```

### Comparing `slack-logger-python-0.4.0/slack_logger_python.egg-info/PKG-INFO` & `slack-logger-python-0.5.0/slack_logger_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slack-logger-python
-Version: 0.4.0
+Version: 0.5.0
 Summary: Slack logger utilizing python logging interface.
 Author-email: GRBurst <GRBurst@protonmail.com>
 Project-URL: Homepage, https://github.com/GRBurst/slack-python-logging
 Project-URL: Bug Tracker, https://github.com/GRBurst/slack-python-logging/issues
 Keywords: slack,python,logging,logger,log,python-logging,Handler,Formatter,logging.Handler,logging.Formatter,monitoring,alerting,slack-api,webhook,slack-logger,messaging,health-check,notification-service,notification
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -68,20 +68,20 @@
 
 You can use the `SlackFormatter.minimal()` and `SlackFormatter.default()` formatter for more visually appealing log messages.
 For now, those require a configuration to show e.g. the header.
 Extra fields are shown in blocks at the bottom of the message and can be dynamically added at runtime.
 Everything else stays the same:
 
 ```python
-from slack_logger import Configuration, SlackFormatter, SlackHandler
+from slack_logger import FormatConfig, SlackFormatter, SlackHandler
 
 logger = logging.getLogger(__name__)
 
-config = Configuration(service="testrunner", environment="test", extra_fields={"foo": "bar"})
-formatter = SlackFormatter.default(config)
+format_config = FormatConfig(service="testrunner", environment="test", extra_fields={"foo": "bar"})
+formatter = SlackFormatter.default(format_config)
 handler = SlackHandler.from_webhook(os.environ["SLACK_WEBHOOK"])
 handler.setFormatter(formatter)
 handler.setLevel(logging.WARN)
 
 logger.addHandler(handler)
 
 logger.info("I won't appear.")
@@ -107,20 +107,20 @@
 ```
 
 Let's look at an example error log from a division by zero error.
 Given the following code snippet with a configuration and the default formatter:
 
 ```python
 import os
-from slack_logger import Configuration, SlackFormatter, SlackHandler
-service_config = Configuration(
+from slack_logger import FormatConfig, SlackFormatter, SlackHandler
+format_config = FormatConfig(
     service="testrunner", environment="test", extra_fields={"foo": "bar", "raven": "caw"}
 )
 slack_handler = SlackHandler.from_webhook(os.environ["SLACK_WEBHOOK"])
-formatter = SlackFormatter.default(service_config)
+formatter = SlackFormatter.default(format_config)
 slack_handler.setFormatter(formatter)
 log.addHandler(slack_handler)
 try:
     1/0
 except Exception:
     log.exception("Something terrible happened!")
 ```
@@ -196,45 +196,45 @@
 }
 ```
 
 You can import and overwrite it partially, or define a complete new set of emoji.
 The following example demonstrates how you can add the emoji set to the `SlackFormatter`:
 
 ```python
-from slack_logger import Configuration, SlackFormatter
+from slack_logger import FormatConfig, SlackFormatter
 
 my_emojis = {
     logging.CRITICAL: ":x:",    # ❌
     logging.ERROR: ":x:",       # ❌
     logging.FATAL: ":x:",       # ❌
     logging.WARNING: ":bell:",  # 🔔
     logging.WARN: ":bell:",     # 🔔
     logging.INFO: ":mega:",     # 📣
     logging.DEBUG: ":mega:",    # 📣
     logging.NOTSET: ":mega:",   # 📣
 }
 
-config = Configuration(service="testrunner", environment="test", emojis=my_emojis)
+config = FormatConfig(service="testrunner", environment="test", emojis=my_emojis)
 formatter = SlackFormatter.default(config)
 ```
 
 
 ### Filter Message
 
 Filters implement the logging interface of `Filters`.
 Design goal (4) and (5) are partially demonstrated.
 
 ```python
-from slack_logger import Configuration, SlackFilter, SlackHandler
+from slack_logger import FilterConfig, SlackFilter, SlackHandler
 import os
 import logging 
 
 logger = logging.getLogger("ProdFilter")
 # Allow only logs from `prod` environment
-filter = SlackFilter(config=Configuration(environment="prod"), filterType=FilterType.AnyAllowList)
+filter = SlackFilter(config=FilterConfig(environment="prod"), filterType=FilterType.AnyAllowList)
 slack_handler.addFilter(filter)
 logger.addHandler(slack_handler)
 
 
 # When the ENV enviroment variable is set to prod, the message will be send.
 # Otherwise, the message is filtered out and not send (e.g. if ENV is `dev`)
 logger.warning(f"{log_msg} in some environment and allow listed prod", extra={"filter": {"environment": os.getenv("ENV", "dev")}})
@@ -243,7 +243,9 @@
 logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "dev"}})
 
 # Will be send
 logger.warning(f"{log_msg} in dev environment and allow listed prod", extra={"filter": {"environment": "prod"}})
 ```
 
 The composition of configurations, filters and dynamic extra fields allow for a flexible way of specifying your message content and filter unwanted messages.
+
+More examples can be found it the [tests folder](https://github.com/GRBurst/slack-logger-python/tree/main/tests).
```

### Comparing `slack-logger-python-0.4.0/slack_logger_python.egg-info/SOURCES.txt` & `slack-logger-python-0.5.0/slack_logger_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/tests/test_basic.py` & `slack-logger-python-0.5.0/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/tests/test_filter.py` & `slack-logger-python-0.5.0/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `slack-logger-python-0.4.0/tests/utils.py` & `slack-logger-python-0.5.0/tests/utils.py`

 * *Files identical despite different names*

