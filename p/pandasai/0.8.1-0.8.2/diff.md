# Comparing `tmp/pandasai-0.8.1.tar.gz` & `tmp/pandasai-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pandasai-0.8.1.tar", max compression
+gzip compressed data, was "pandasai-0.8.2.tar", max compression
```

## Comparing `pandasai-0.8.1.tar` & `pandasai-0.8.2.tar`

### file list

```diff
@@ -1,40 +1,40 @@
--rw-r--r--   0        0        0     1055 2023-07-28 23:36:48.651563 pandasai-0.8.1/LICENSE
--rw-r--r--   0        0        0     7986 2023-07-28 23:36:48.651563 pandasai-0.8.1/README.md
--rw-r--r--   0        0        0    28810 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/__init__.py
--rw-r--r--   0        0        0      155 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/callbacks/__init__.py
--rw-r--r--   0        0        0      519 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/callbacks/base.py
--rw-r--r--   0        0        0      583 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/callbacks/file.py
--rw-r--r--   0        0        0     1438 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/constants.py
--rw-r--r--   0        0        0     1509 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3814 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     6404 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1742 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      566 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     3631 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/from_google_sheets.py
--rw-r--r--   0        0        0     1493 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3070 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/openai_info.py
--rw-r--r--   0        0        0     2454 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0     9911 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4289 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    13023 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/base.py
--rw-r--r--   0        0        0      542 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/fake.py
--rw-r--r--   0        0        0      735 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4440 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      585 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     3130 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/openai.py
--rw-r--r--   0        0        0      739 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      663 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      948 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      653 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0     1230 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1578 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1261 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1380 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      460 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1256 2023-07-28 23:36:48.659563 pandasai-0.8.1/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     2003 2023-07-28 23:36:48.663563 pandasai-0.8.1/pyproject.toml
--rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 pandasai-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-08-05 00:39:25.135716 pandasai-0.8.2/LICENSE
+-rw-r--r--   0        0        0     7986 2023-08-05 00:39:25.135716 pandasai-0.8.2/README.md
+-rw-r--r--   0        0        0    28832 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/__init__.py
+-rw-r--r--   0        0        0      155 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/callbacks/__init__.py
+-rw-r--r--   0        0        0      519 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/callbacks/base.py
+-rw-r--r--   0        0        0      583 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/callbacks/file.py
+-rw-r--r--   0        0        0     1438 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/constants.py
+-rw-r--r--   0        0        0     1509 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/exceptions.py
+-rw-r--r--   0        0        0      316 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3814 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     6404 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1742 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      566 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     3631 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/from_google_sheets.py
+-rw-r--r--   0        0        0     1493 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3070 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/openai_info.py
+-rw-r--r--   0        0        0     2454 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0     9911 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0      423 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4289 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    13023 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/base.py
+-rw-r--r--   0        0        0      542 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/fake.py
+-rw-r--r--   0        0        0      735 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4440 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      585 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     3130 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/openai.py
+-rw-r--r--   0        0        0      739 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0      192 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      663 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      948 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      653 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0      517 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0     1230 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1578 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1261 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1380 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      460 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1204 2023-08-05 00:39:25.143716 pandasai-0.8.2/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     2003 2023-08-05 00:39:25.143716 pandasai-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0     9285 1970-01-01 00:00:00.000000 pandasai-0.8.2/PKG-INFO
```

### Comparing `pandasai-0.8.1/LICENSE` & `pandasai-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/README.md` & `pandasai-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/__init__.py` & `pandasai-0.8.2/pandasai/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -380,15 +380,15 @@
             else:
                 rows_to_display = 0 if self._enforce_privacy else 5
 
                 multiple: bool = isinstance(data_frame, list)
 
                 if multiple:
                     heads = [
-                        anonymize_dataframe_head(dataframe)
+                        anonymize_dataframe_head(dataframe.head(rows_to_display))
                         if anonymize_df
                         else dataframe.head(rows_to_display)
                         for dataframe in data_frame
                     ]
 
                     multiple_dataframes_default_values = {"dataframes": heads}
                     (
```

### Comparing `pandasai-0.8.1/pandasai/callbacks/base.py` & `pandasai-0.8.2/pandasai/callbacks/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/callbacks/file.py` & `pandasai-0.8.2/pandasai/callbacks/file.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/constants.py` & `pandasai-0.8.2/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/exceptions.py` & `pandasai-0.8.2/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/_optional.py` & `pandasai-0.8.2/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/anonymizer.py` & `pandasai-0.8.2/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/cache.py` & `pandasai-0.8.2/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/from_excel.py` & `pandasai-0.8.2/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/from_google_sheets.py` & `pandasai-0.8.2/pandasai/helpers/from_google_sheets.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/notebook.py` & `pandasai-0.8.2/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/openai_info.py` & `pandasai-0.8.2/pandasai/helpers/openai_info.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/save_chart.py` & `pandasai-0.8.2/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/helpers/shortcuts.py` & `pandasai-0.8.2/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/azure_openai.py` & `pandasai-0.8.2/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/base.py` & `pandasai-0.8.2/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/fake.py` & `pandasai-0.8.2/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/falcon.py` & `pandasai-0.8.2/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/google_palm.py` & `pandasai-0.8.2/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/langchain.py` & `pandasai-0.8.2/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/openai.py` & `pandasai-0.8.2/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/llm/starcoder.py` & `pandasai-0.8.2/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/middlewares/base.py` & `pandasai-0.8.2/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/middlewares/charts.py` & `pandasai-0.8.2/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/middlewares/streamlit.py` & `pandasai-0.8.2/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/prompts/base.py` & `pandasai-0.8.2/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/prompts/correct_error_prompt.py` & `pandasai-0.8.2/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/prompts/correct_multiples_prompt.py` & `pandasai-0.8.2/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/prompts/generate_python_code.py` & `pandasai-0.8.2/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `pandasai-0.8.1/pandasai/prompts/multiple_dataframes.py` & `pandasai-0.8.2/pandasai/prompts/multiple_dataframes.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 """  # noqa: E501
 
     def __init__(self, dataframes: list[pd.DataFrame]):
         for i, dataframe in enumerate(dataframes, start=1):
             row, col = dataframe.shape
 
             self.text += f"""
-Dataframe df{i}, with {row} rows and {col} columns.
 This is the metadata of the dataframe df{i}:
 {dataframe}"""
 
         self.text += self.instruction
         self.text = self.text.format(
             START_CODE_TAG=START_CODE_TAG,
             END_CODE_TAG=END_CODE_TAG,
```

### Comparing `pandasai-0.8.1/pyproject.toml` & `pandasai-0.8.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pandasai"
-version = "0.8.1"
+version = "0.8.2"
 description = "Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational."
 authors = ["Gabriele Venturi"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `pandasai-0.8.1/PKG-INFO` & `pandasai-0.8.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pandasai
-Version: 0.8.1
+Version: 0.8.2
 Summary: Pandas AI is a Python library that integrates generative artificial intelligence capabilities into Pandas, making dataframes conversational.
 License: MIT
 Author: Gabriele Venturi
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

