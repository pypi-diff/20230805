# Comparing `tmp/wordview-1.0.0.tar.gz` & `tmp/wordview-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wordview-1.0.0.tar", max compression
+gzip compressed data, was "wordview-1.1.0.tar", max compression
```

## Comparing `wordview-1.0.0.tar` & `wordview-1.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     2705 2023-08-03 11:22:29.022213 wordview-1.0.0/CHANGES.rst
--rw-r--r--   0        0        0     1074 2023-08-03 11:22:29.022213 wordview-1.0.0/LICENSE
--rw-r--r--   0        0        0     4047 2023-08-03 11:22:29.022213 wordview-1.0.0/README.rst
--rw-r--r--   0        0        0      937 2023-08-03 11:22:29.130264 wordview-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      163 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/__init__.py
--rw-r--r--   0        0        0       60 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/anomaly/__init__.py
--rw-r--r--   0        0        0     7343 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/anomaly/gaussianize.py
--rw-r--r--   0        0        0     4789 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/anomaly/normaldist.py
--rw-r--r--   0        0        0       48 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/clustering/__init__.py
--rw-r--r--   0        0        0     3027 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/clustering/cluster.py
--rw-r--r--   0        0        0     1340 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/io/dataframe_reader.py
--rw-r--r--   0        0        0       85 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/__init__.py
--rw-r--r--   0        0        0     2900 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/am.py
--rw-r--r--   0        0        0     1499 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/association_measures.py
--rw-r--r--   0        0        0     1438 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/chunker.py
--rw-r--r--   0        0        0     9431 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/mwe.py
--rw-r--r--   0        0        0     3962 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/mwe_utils.py
--rw-r--r--   0        0        0     1967 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/mwes/patterns.py
--rw-r--r--   0        0        0      111 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/preprocessing/__init__.py
--rw-r--r--   0        0        0     3078 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/preprocessing/cleaning.py
--rw-r--r--   0        0        0     3718 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/preprocessing/count.py
--rw-r--r--   0        0        0       75 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/text_analysis/__init__.py
--rw-r--r--   0        0        0    12315 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/text_analysis/core.py
--rw-r--r--   0        0        0     8763 2023-08-03 11:22:29.130264 wordview-1.0.0/wordview/text_analysis/wrapper.py
--rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 wordview-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     3034 2023-08-05 14:14:11.767025 wordview-1.1.0/CHANGES.rst
+-rw-r--r--   0        0        0     1074 2023-08-05 14:14:11.767025 wordview-1.1.0/LICENSE
+-rw-r--r--   0        0        0     4047 2023-08-05 14:14:11.767025 wordview-1.1.0/README.rst
+-rw-r--r--   0        0        0      936 2023-08-05 14:14:11.859026 wordview-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      163 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/__init__.py
+-rw-r--r--   0        0        0       60 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/anomaly/__init__.py
+-rw-r--r--   0        0        0     7343 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/anomaly/gaussianize.py
+-rw-r--r--   0        0        0     4789 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/anomaly/normaldist.py
+-rw-r--r--   0        0        0       53 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/bias_analysis/__init__.py
+-rw-r--r--   0        0        0     7130 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/bias_analysis/bias.py
+-rw-r--r--   0        0        0     4131 2023-08-05 14:14:11.859026 wordview-1.1.0/wordview/bias_analysis/bias_terms.py
+-rw-r--r--   0        0        0       48 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/clustering/__init__.py
+-rw-r--r--   0        0        0     3027 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/clustering/cluster.py
+-rw-r--r--   0        0        0     1340 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/io/dataframe_reader.py
+-rw-r--r--   0        0        0       34 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/__init__.py
+-rw-r--r--   0        0        0     1499 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/association_measures.py
+-rw-r--r--   0        0        0     9848 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/mwe.py
+-rw-r--r--   0        0        0     1967 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/mwes/patterns.py
+-rw-r--r--   0        0        0      111 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/preprocessing/__init__.py
+-rw-r--r--   0        0        0     3078 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/preprocessing/cleaning.py
+-rw-r--r--   0        0        0     3718 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/preprocessing/count.py
+-rw-r--r--   0        0        0       75 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/text_analysis/__init__.py
+-rw-r--r--   0        0        0    12315 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/text_analysis/core.py
+-rw-r--r--   0        0        0     8753 2023-08-05 14:14:11.863026 wordview-1.1.0/wordview/text_analysis/wrapper.py
+-rw-r--r--   0        0        0     4886 1970-01-01 00:00:00.000000 wordview-1.1.0/PKG-INFO
```

### Comparing `wordview-1.0.0/CHANGES.rst` & `wordview-1.1.0/CHANGES.rst`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Version 1.1.0
+-------------
+- Add bias detection and analysis feature (based on sentiment analysis)
+- Include 3 bias categories: race, religion, and gender.
+- Include an initial set of key terms for each bias category.
+- Add function to visualize bias analysis in a plot.
+- Add function to visualize bias analysis in a tables.
+
+
 Version 1.0.0
 -------------
 - Complete refactoring and upgrading of the MWE module.
 - Support for extracting variable length MWEs given a custom user syntactic patterns of POS tags.
 - Predefined patterns for extracting Light Verb Constructions (LVCs), 2-3 word Noun Compounds, 2-3 Adjective Noun Compounds, and 2-3 Verb Noun Compounds, and Verb Particle Constructions (VPCs).
 - Refactoring of the Association Measure module.
 - Move DataFrame reader to a separate preprocessing module so that it can support all modules easier.
```

### Comparing `wordview-1.0.0/LICENSE` & `wordview-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/README.rst` & `wordview-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/pyproject.toml` & `wordview-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "wordview"
-version = "1.0.0"
+version = "1.1.0"
 description = "Wordview is a Python package for text analysis."
 authors = ["meghdadFar <meghdad.farahmand@gmail.com>"]
 readme = "README.rst"
 include = ["CHANGES.rst"]
 exclude = ["notebooks/", "tests/", "data/"]
 license = "MIT"
 keywords = ["nlp", "text analysis", "statistics"]
@@ -27,14 +27,13 @@
 pytest = ">=7.1"
 pytest-cov = ">=3.0.0"
 ipython = ">=8.4.0"
 sphinx = ">=v6.1.3"
 sphinx-rtd-theme = "1.2.1"
 jupyter = "1.0.0"
 
-
 [tool.poetry.scripts]
 nltk_download_script = "bin.downloads:download_nltk_req"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `wordview-1.0.0/wordview/anomaly/gaussianize.py` & `wordview-1.1.0/wordview/anomaly/gaussianize.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/anomaly/normaldist.py` & `wordview-1.1.0/wordview/anomaly/normaldist.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/clustering/cluster.py` & `wordview-1.1.0/wordview/clustering/cluster.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/io/dataframe_reader.py` & `wordview-1.1.0/wordview/io/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/mwes/association_measures.py` & `wordview-1.1.0/wordview/mwes/association_measures.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/mwes/mwe.py` & `wordview-1.1.0/wordview/mwes/mwe.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,30 @@
+import re
 import string
+from re import Match
 from typing import Dict, Optional
 
+import nltk
 import pandas
 from nltk import RegexpParser, word_tokenize
 from tabulate import tabulate  # type: ignore
 from tqdm import tqdm
 
 from wordview import logger
 from wordview.io.dataframe_reader import DataFrameReader
 from wordview.mwes.association_measures import PMICalculator
-from wordview.mwes.mwe_utils import get_pos_tags
 from wordview.mwes.patterns import DeMWEPatterns, EnMWEPatterns
 
 
+# TODO use this function to ensure that the tokens are alphanumeric
+def is_alphanumeric_latinscript_multigram(word: str) -> Optional[Match[str]]:
+    match: Optional[Match] = re.match("[a-zA-Z0-9]{2,}", word)
+    return match
+
+
 class MWEPatternAssociation:
     """Extract MWE candidates from a list of tokens based on a given pattern."""
 
     def __init__(self, association_measure: PMICalculator, pattern: str) -> None:
         """Initializes a new instance of MWEExtractor class.
 
         Args:
@@ -50,15 +58,20 @@
             tokens (list[str]): A list of tokens from which mwe candidates are to be extracted.
 
         Returns:
             match_counter (dict[str, dict[str, int]]): A counter dictionary with count of matched strings, grouped by pattern label.
                                                     An empty list if none were found.
         """
 
+        def get_pos_tags(tokens: list[str]) -> list[tuple[str, str]]:
+            pos_tags = nltk.pos_tag(tokens)
+            return pos_tags
+
         def validate_input() -> None:
+            """Validate input argument `tokens`."""
             if not isinstance(tokens, list):
                 raise TypeError(
                     f'Input argument "tokens" must be a list of string. Currently it is of type {type(self.tokens)} \
                     with a value of: {self.tokens}.'
                 )
             if len(tokens) == 0:
                 raise ValueError(
```

### Comparing `wordview-1.0.0/wordview/mwes/patterns.py` & `wordview-1.1.0/wordview/mwes/patterns.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/preprocessing/cleaning.py` & `wordview-1.1.0/wordview/preprocessing/cleaning.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/preprocessing/count.py` & `wordview-1.1.0/wordview/preprocessing/count.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/text_analysis/core.py` & `wordview-1.1.0/wordview/text_analysis/core.py`

 * *Files identical despite different names*

### Comparing `wordview-1.0.0/wordview/text_analysis/wrapper.py` & `wordview-1.1.0/wordview/text_analysis/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -155,17 +155,17 @@
 
     def show_word_clouds(self, pos: str, **kwargs) -> None:
         """Shows POS word clouds.
 
         Args:
             pos (str): Type of POS. Can be any of: [NN, JJ, VB].
             **kwargs: Keyword arguments to be passed to self._create_pos_plots() and wordview.text_analysis.core.plotly_wordcloud().
-              This includes:
-                - plot_settings: Dictionary of form: for self._create_pos_plots(). For available settings see: https://plotly.com/python/reference/layout/.
-                - wc_settings: Dictionary of form: {"color": "<color>", "max_words": int} for core.plotly_wordcloud(). Accepted values are color strings as usable by PIL/Pillow.
+            This includes:
+            - plot_settings: Dictionary of form: for self._create_pos_plots(). For available settings see: https://plotly.com/python/reference/layout/.
+            - wc_settings: Dictionary of form: {"color": "<color>", "max_words": int} for core.plotly_wordcloud(). Accepted values are color strings as usable by PIL/Pillow.
 
         Returns:
             None
         """
         self._create_pos_plots(pos=pos, **kwargs).show()
 
     def show_stats(self) -> None:
```

### Comparing `wordview-1.0.0/PKG-INFO` & `wordview-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wordview
-Version: 1.0.0
+Version: 1.1.0
 Summary: Wordview is a Python package for text analysis.
 License: MIT
 Keywords: nlp,text analysis,statistics
 Author: meghdadFar
 Author-email: meghdad.farahmand@gmail.com
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

