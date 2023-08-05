# Comparing `tmp/assess_acceptability_judgments-0.0.8.tar.gz` & `tmp/assess_acceptability_judgments-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assess_acceptability_judgments-0.0.8.tar", last modified: Mon Jul 31 21:42:09 2023, max compression
+gzip compressed data, was "assess_acceptability_judgments-0.0.9.tar", last modified: Wed Aug  2 00:23:49 2023, max compression
```

## Comparing `assess_acceptability_judgments-0.0.8.tar` & `assess_acceptability_judgments-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.568709 assess_acceptability_judgments-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-31 21:42:09.568709 assess_acceptability_judgments-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/constituency_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5242 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/dependency_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/fluency_score_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/glue.py
--rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/nce.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/ppl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.548707 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-31 21:41:58.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.568709 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/
--rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/treebank.json
--rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
--rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
--rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/slor.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-31 21:42:09.552708 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-31 21:42:09.000000 assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-31 21:42:09.572709 assess_acceptability_judgments-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-07-31 21:41:59.000000 assess_acceptability_judgments-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.036988 assess_acceptability_judgments-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-02 00:23:49.036988 assess_acceptability_judgments-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.016987 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6742 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/constituency_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/dependency_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/fluency_score_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4017 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/nce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/ppl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.012986 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.020987 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/nce_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.020987 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/slor_scores_distribution/wordpiece_roberta_base.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.036988 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/
+-rw-r--r--   0 runner    (1001) docker     (123)  4196866 2023-08-02 00:23:37.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/treebank.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4236193 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   885888 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   834521 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json
+-rw-r--r--   0 runner    (1001) docker     (123)   917643 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/slor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-02 00:23:48.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-02 00:23:49.016987 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-08-02 00:23:48.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-08-02 00:23:48.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-02 00:23:48.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-02 00:23:48.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-08-02 00:23:48.000000 assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-08-02 00:23:49.040988 assess_acceptability_judgments-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-08-02 00:23:38.000000 assess_acceptability_judgments-0.0.9/setup.py
```

### Comparing `assess_acceptability_judgments-0.0.8/LICENSE` & `assess_acceptability_judgments-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/PKG-INFO` & `assess_acceptability_judgments-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess_acceptability_judgments
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.8.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.9.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/constituency_parser.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/constituency_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
-from typing import List, Union, Generator
+from typing import List, Union
 
 import benepar
 import spacy
 import stanza
 import supar
 from stanza.models.constituency.tree_reader import read_trees
 from supar import Parser
 
 
-# Todo: add encoding of the parse tree using Tree-LSTM: https://github.com/dmlc/dgl/blob/master/examples/pytorch/tree_lstm/README.md
+# Add encoding of the parse tree using Tree-LSTM:
+#  https://github.com/dmlc/dgl/blob/master/examples/pytorch/tree_lstm/README.md
 # similar to https://www.hindawi.com/journals/cin/2022/4096383/
 
 
 class ConstituencyParserCoreNLP:
     def __init__(self) -> None:
         """
          Create a dependency parsing model that use Stanza constituency parser.
@@ -61,15 +62,15 @@
                 parsed_trees.append(doc_parsed_trees)
             else:
                 parsed_trees.append([""])
 
         return parsed_trees
 
 
-class ConstituencyParsingSuPar:
+class ConstituencyParserSuPar:
     def __init__(self, model: str) -> None:
         """
         Create a dependency parsing model that use SuPar constituency parser.
 
         Base on the SuPar documentation https://github.com/yzhangcs/parser#usage.
 
         :param model: (str) The parsing model to use. Choices are
@@ -113,15 +114,15 @@
                 process_documents = self.process_sentences(sentence)
                 parsed_trees.append(self.get_tree(process_documents))
             else:
                 parsed_trees.append([""])
         return parsed_trees
 
 
-class ConstituencyParsingBeNePar:
+class ConstituencyParserBeNePar:
     def __init__(self, use_larger_model: bool = False) -> None:
         """
         Create a dependency parsing model that use BeNePar constituency parser.
 
         Base on the BeNePar documentation
         https://github.com/nikitakit/self-attentive-parser#usage-with-spacy-recommended.
```

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/dependency_parser.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/dependency_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 
 import conllu
 import nltk
 import supar
 from nltk.parse.corenlp import CoreNLPServer, CoreNLPParser
 from supar import Parser
 
-from assess_acceptability_judgments import CACHE_PATH
-from assess_acceptability_judgments.util import DownloadProgressBar
+from . import CACHE_PATH
+from .util import DownloadProgressBar
 
 CORENLP_URL = "http://nlp.stanford.edu/software/stanford-corenlp-full-2018-02-27.zip"
 
 
-class DependencyParsingCoreNLP:
+class DependencyParserCoreNLP:
     # Path to the corenlp JAR models to use for parsing and create Tree
     # As of july 2023, Stanza does not return a Tree by a dictionary. Thus, we use NLTK API
     # that parse and return a dependency parse tree.
     CORENLP_DIRECTORY = "stanford-corenlp-full-2018-02-27"
     JAR_FILE_NAME = os.path.join(CORENLP_DIRECTORY, "stanford-corenlp-3.9.1.jar")
     JAR_MODEL_FILE_NAME = os.path.join(CORENLP_DIRECTORY, "stanford-corenlp-3.9.1-models.jar")
 
@@ -71,15 +71,15 @@
                 if len(sentence) > 0:
                     parsed_trees.append(list(parser.raw_parse(sentence)))
                 else:
                     parsed_trees.append([""])
             return parsed_trees
 
 
-class DependencyParsingSuPar:
+class DependencyParserSuPar:
     def __init__(self, model: str):
         """
         Create a dependency parsing model that use SuPar constituency parser.
 
         Base on the SuPar documentation https://github.com/yzhangcs/parser#usage.
 
         :param model: (str) The parsing model to use. Choices are
```

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/fluency_score_interface.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/fluency_score_interface.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/nce.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/nce.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/ppl.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/ppl.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/treebank.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/treebank.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace_llm_bert_large_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/whitespace_llm_roberta_base.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_base_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/wordpiece_bert_large_uncased.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/resources/words_probability/wordpiece_roberta_base.json`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/slor.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/slor.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments/util.py` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments/util.py`

 * *Files identical despite different names*

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/PKG-INFO` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: assess-acceptability-judgments
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for assessing acceptability judgments
 Home-page: https://github.com/davebulaval/assess_acceptability_judgments
-Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.8.zip
+Download-URL: https://github.com/GRAAL-Research/assess_acceptability_judgments/archive/v0.0.9.zip
 Author: David Beauchemin
 Author-email: david.beauchemin.5@ulaval.ca
 License: LGPLv3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
```

### Comparing `assess_acceptability_judgments-0.0.8/assess_acceptability_judgments.egg-info/SOURCES.txt` & `assess_acceptability_judgments-0.0.9/assess_acceptability_judgments.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 pyproject.toml
 setup.cfg
 setup.py
 assess_acceptability_judgments/__init__.py
 assess_acceptability_judgments/constituency_parser.py
 assess_acceptability_judgments/dependency_parser.py
 assess_acceptability_judgments/fluency_score_interface.py
-assess_acceptability_judgments/glue.py
 assess_acceptability_judgments/nce.py
 assess_acceptability_judgments/ppl.py
 assess_acceptability_judgments/slor.py
 assess_acceptability_judgments/util.py
 assess_acceptability_judgments/version.py
 assess_acceptability_judgments.egg-info/PKG-INFO
 assess_acceptability_judgments.egg-info/SOURCES.txt
```

### Comparing `assess_acceptability_judgments-0.0.8/setup.py` & `assess_acceptability_judgments-0.0.9/setup.py`

 * *Files identical despite different names*

