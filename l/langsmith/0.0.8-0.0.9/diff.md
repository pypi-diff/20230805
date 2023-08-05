# Comparing `tmp/langsmith-0.0.8.tar.gz` & `tmp/langsmith-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langsmith-0.0.8.tar", max compression
+gzip compressed data, was "langsmith-0.0.9.tar", max compression
```

## Comparing `langsmith-0.0.8.tar` & `langsmith-0.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     8107 2023-07-17 14:32:27.346477 langsmith-0.0.8/README.md
--rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.8/langsmith/__init__.py
--rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.8/langsmith/cli/__init__.py
--rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.8/langsmith/cli/conf/nginx.conf
--rw-r--r--   0        0        0      143 2023-07-12 06:25:39.153595 langsmith-0.0.8/langsmith/cli/docker-compose.dev.yaml
--rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.8/langsmith/cli/docker-compose.ngrok.yaml
--rw-r--r--   0        0        0     1186 2023-07-12 00:52:45.305623 langsmith-0.0.8/langsmith/cli/docker-compose.yaml
--rw-r--r--   0        0        0    14420 2023-07-15 15:32:37.213445 langsmith-0.0.8/langsmith/cli/main.py
--rw-r--r--   0        0        0    45457 2023-07-17 14:32:27.347012 langsmith-0.0.8/langsmith/client.py
--rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.8/langsmith/evaluation/__init__.py
--rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.8/langsmith/evaluation/evaluator.py
--rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.8/langsmith/evaluation/string_evaluator.py
--rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.8/langsmith/run_helpers.py
--rw-r--r--   0        0        0     6116 2023-07-12 00:52:45.306853 langsmith-0.0.8/langsmith/run_trees.py
--rw-r--r--   0        0        0     6499 2023-07-13 17:24:35.594023 langsmith-0.0.8/langsmith/schemas.py
--rw-r--r--   0        0        0     4180 2023-07-15 15:34:27.624819 langsmith-0.0.8/langsmith/utils.py
--rw-r--r--   0        0        0      858 2023-07-17 15:17:02.918787 langsmith-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     8669 1970-01-01 00:00:00.000000 langsmith-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     8107 2023-07-17 14:32:27.346477 langsmith-0.0.9/README.md
+-rw-r--r--   0        0        0      478 2023-07-10 20:55:19.191988 langsmith-0.0.9/langsmith/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-05 17:54:45.352774 langsmith-0.0.9/langsmith/cli/__init__.py
+-rw-r--r--   0        0        0      363 2023-07-05 17:54:45.353156 langsmith-0.0.9/langsmith/cli/conf/nginx.conf
+-rw-r--r--   0        0        0      143 2023-07-12 06:25:39.153595 langsmith-0.0.9/langsmith/cli/docker-compose.dev.yaml
+-rw-r--r--   0        0        0      315 2023-07-05 17:54:45.353418 langsmith-0.0.9/langsmith/cli/docker-compose.ngrok.yaml
+-rw-r--r--   0        0        0     1186 2023-07-12 00:52:45.305623 langsmith-0.0.9/langsmith/cli/docker-compose.yaml
+-rw-r--r--   0        0        0    14420 2023-07-15 15:32:37.213445 langsmith-0.0.9/langsmith/cli/main.py
+-rw-r--r--   0        0        0    45488 2023-07-17 16:22:58.799855 langsmith-0.0.9/langsmith/client.py
+-rw-r--r--   0        0        0      234 2023-07-05 17:54:45.355050 langsmith-0.0.9/langsmith/evaluation/__init__.py
+-rw-r--r--   0        0        0     1411 2023-07-05 17:54:45.355316 langsmith-0.0.9/langsmith/evaluation/evaluator.py
+-rw-r--r--   0        0        0     1529 2023-07-05 17:54:45.355546 langsmith-0.0.9/langsmith/evaluation/string_evaluator.py
+-rw-r--r--   0        0        0     9462 2023-07-05 17:54:45.355760 langsmith-0.0.9/langsmith/run_helpers.py
+-rw-r--r--   0        0        0     6116 2023-07-12 00:52:45.306853 langsmith-0.0.9/langsmith/run_trees.py
+-rw-r--r--   0        0        0     6523 2023-07-17 16:22:58.800152 langsmith-0.0.9/langsmith/schemas.py
+-rw-r--r--   0        0        0     4180 2023-07-15 15:34:27.624819 langsmith-0.0.9/langsmith/utils.py
+-rw-r--r--   0        0        0      858 2023-07-17 17:47:21.642153 langsmith-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     8669 1970-01-01 00:00:00.000000 langsmith-0.0.9/PKG-INFO
```

### Comparing `langsmith-0.0.8/README.md` & `langsmith-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/cli/docker-compose.yaml` & `langsmith-0.0.9/langsmith/cli/docker-compose.yaml`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/cli/main.py` & `langsmith-0.0.9/langsmith/cli/main.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/client.py` & `langsmith-0.0.9/langsmith/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Optional,
     Sequence,
     Tuple,
     Union,
     cast,
 )
 from urllib.parse import urlsplit
-from uuid import UUID
+from uuid import UUID, uuid4
 
 from requests import ConnectionError, HTTPError, Response, Session
 from requests.adapters import HTTPAdapter
 from urllib3.util import Retry
 
 from langsmith.evaluation.evaluator import RunEvaluator
 from langsmith.schemas import (
@@ -1368,14 +1368,15 @@
                 metadata=source_info
             )
         elif feedback_source_type == FeedbackSourceType.MODEL:
             feedback_source = ModelFeedbackSource(metadata=source_info)
         else:
             raise ValueError(f"Unknown feedback source type {feedback_source_type}")
         feedback = FeedbackCreate(
+            id=uuid4(),
             run_id=run_id,
             key=key,
             score=score,
             value=value,
             correction=correction,
             comment=comment,
             feedback_source=feedback_source,
```

### Comparing `langsmith-0.0.8/langsmith/evaluation/evaluator.py` & `langsmith-0.0.9/langsmith/evaluation/evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/evaluation/string_evaluator.py` & `langsmith-0.0.9/langsmith/evaluation/string_evaluator.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/run_helpers.py` & `langsmith-0.0.9/langsmith/run_helpers.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/run_trees.py` & `langsmith-0.0.9/langsmith/run_trees.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/langsmith/schemas.py` & `langsmith-0.0.9/langsmith/schemas.py`

 * *Files 2% similar despite different names*

```diff
@@ -152,15 +152,16 @@
     MODEL = "model"
     """Model-assisted feedback."""
 
 
 class FeedbackBase(BaseModel):
     """Feedback schema."""
 
-    id: Optional[UUID] = None
+    id: UUID
+    """The unique ID of the feedback."""
     created_at: Optional[datetime] = None
     """The time the feedback was created."""
     modified_at: Optional[datetime] = None
     """The time the feedback was last modified."""
     run_id: UUID
     """The associated run ID this feedback is logged for."""
     key: str
```

### Comparing `langsmith-0.0.8/langsmith/utils.py` & `langsmith-0.0.9/langsmith/utils.py`

 * *Files identical despite different names*

### Comparing `langsmith-0.0.8/pyproject.toml` & `langsmith-0.0.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langsmith"
-version = "0.0.8"
+version = "0.0.9"
 description = "Client library to connect to the LangSmith LLM Tracing and Evaluation Platform."
 authors = ["LangChain"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "langsmith"}]
 
 [tool.poetry.scripts]
```

### Comparing `langsmith-0.0.8/PKG-INFO` & `langsmith-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langsmith
-Version: 0.0.8
+Version: 0.0.9
 Summary: Client library to connect to the LangSmith LLM Tracing and Evaluation Platform.
 License: MIT
 Author: LangChain
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

