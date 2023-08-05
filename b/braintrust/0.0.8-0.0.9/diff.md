# Comparing `tmp/braintrust-0.0.8.tar.gz` & `tmp/braintrust-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "braintrust-0.0.8.tar", last modified: Fri Jun 30 23:32:32 2023, max compression
+gzip compressed data, was "braintrust-0.0.9.tar", last modified: Fri Jun 30 23:45:16 2023, max compression
```

## Comparing `braintrust-0.0.8.tar` & `braintrust-0.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.074586 braintrust-0.0.8/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:32:32.074450 braintrust-0.0.8/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.8/README.md
--rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-30 23:32:32.074628 braintrust-0.0.8/setup.cfg
--rw-r--r--   0 ankur      (501) staff       (20)     1640 2023-06-30 23:03:25.000000 braintrust-0.0.8/setup.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.070388 braintrust-0.0.8/src/
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.072667 braintrust-0.0.8/src/braintrust/
--rw-r--r--   0 ankur      (501) staff       (20)    35426 2023-06-30 23:31:00.000000 braintrust-0.0.8/src/braintrust/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/aws.py
--rw-r--r--   0 ankur      (501) staff       (20)      171 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/cache.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.073600 braintrust-0.0.8/src/braintrust/cli/
--rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/__main__.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.074196 braintrust-0.0.8/src/braintrust/cli/install/
--rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/install/__init__.py
--rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/install/api.py
--rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-22 23:54:28.000000 braintrust-0.0.8/src/braintrust/cli/install/redshift.py
--rw-r--r--   0 ankur      (501) staff       (20)      399 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/duckutil.py
--rw-r--r--   0 ankur      (501) staff       (20)     2878 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/gitutil.py
--rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.8/src/braintrust/oai.py
--rw-r--r--   0 ankur      (501) staff       (20)      307 2023-06-30 23:03:25.000000 braintrust-0.0.8/src/braintrust/util.py
--rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-30 23:31:25.000000 braintrust-0.0.8/src/braintrust/version.py
-drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:32:32.073375 braintrust-0.0.8/src/braintrust.egg-info/
--rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/PKG-INFO
--rw-r--r--   0 ankur      (501) staff       (20)      619 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/SOURCES.txt
--rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/dependency_links.txt
--rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/entry_points.txt
--rw-r--r--   0 ankur      (501) staff       (20)      316 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/requires.txt
--rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-30 23:32:32.000000 braintrust-0.0.8/src/braintrust.egg-info/top_level.txt
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:45:16.680352 braintrust-0.0.9/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:45:16.680191 braintrust-0.0.9/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)       49 2023-04-02 02:49:19.000000 braintrust-0.0.9/README.md
+-rw-r--r--   0 ankur      (501) staff       (20)       38 2023-06-30 23:45:16.680397 braintrust-0.0.9/setup.cfg
+-rw-r--r--   0 ankur      (501) staff       (20)     1640 2023-06-30 23:03:25.000000 braintrust-0.0.9/setup.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:45:16.676213 braintrust-0.0.9/src/
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:45:16.678069 braintrust-0.0.9/src/braintrust/
+-rw-r--r--   0 ankur      (501) staff       (20)    35345 2023-06-30 23:45:01.000000 braintrust-0.0.9/src/braintrust/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)      427 2023-06-22 23:54:28.000000 braintrust-0.0.9/src/braintrust/aws.py
+-rw-r--r--   0 ankur      (501) staff       (20)      171 2023-06-30 23:03:25.000000 braintrust-0.0.9/src/braintrust/cache.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:45:16.679081 braintrust-0.0.9/src/braintrust/cli/
+-rw-r--r--   0 ankur      (501) staff       (20)        0 2023-06-22 23:54:28.000000 braintrust-0.0.9/src/braintrust/cli/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     1406 2023-06-22 23:54:28.000000 braintrust-0.0.9/src/braintrust/cli/__main__.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:45:16.679900 braintrust-0.0.9/src/braintrust/cli/install/
+-rw-r--r--   0 ankur      (501) staff       (20)      472 2023-06-22 23:54:28.000000 braintrust-0.0.9/src/braintrust/cli/install/__init__.py
+-rw-r--r--   0 ankur      (501) staff       (20)     8207 2023-06-22 23:54:28.000000 braintrust-0.0.9/src/braintrust/cli/install/api.py
+-rw-r--r--   0 ankur      (501) staff       (20)     6421 2023-06-22 23:54:28.000000 braintrust-0.0.9/src/braintrust/cli/install/redshift.py
+-rw-r--r--   0 ankur      (501) staff       (20)      399 2023-06-30 23:03:25.000000 braintrust-0.0.9/src/braintrust/duckutil.py
+-rw-r--r--   0 ankur      (501) staff       (20)     2878 2023-06-30 23:03:25.000000 braintrust-0.0.9/src/braintrust/gitutil.py
+-rw-r--r--   0 ankur      (501) staff       (20)      811 2023-04-15 21:46:41.000000 braintrust-0.0.9/src/braintrust/oai.py
+-rw-r--r--   0 ankur      (501) staff       (20)      307 2023-06-30 23:03:25.000000 braintrust-0.0.9/src/braintrust/util.py
+-rw-r--r--   0 ankur      (501) staff       (20)       18 2023-06-30 23:44:56.000000 braintrust-0.0.9/src/braintrust/version.py
+drwxr-xr-x   0 ankur      (501) staff       (20)        0 2023-06-30 23:45:16.678858 braintrust-0.0.9/src/braintrust.egg-info/
+-rw-r--r--   0 ankur      (501) staff       (20)      483 2023-06-30 23:45:16.000000 braintrust-0.0.9/src/braintrust.egg-info/PKG-INFO
+-rw-r--r--   0 ankur      (501) staff       (20)      619 2023-06-30 23:45:16.000000 braintrust-0.0.9/src/braintrust.egg-info/SOURCES.txt
+-rw-r--r--   0 ankur      (501) staff       (20)        1 2023-06-30 23:45:16.000000 braintrust-0.0.9/src/braintrust.egg-info/dependency_links.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       60 2023-06-30 23:45:16.000000 braintrust-0.0.9/src/braintrust.egg-info/entry_points.txt
+-rw-r--r--   0 ankur      (501) staff       (20)      316 2023-06-30 23:45:16.000000 braintrust-0.0.9/src/braintrust.egg-info/requires.txt
+-rw-r--r--   0 ankur      (501) staff       (20)       11 2023-06-30 23:45:16.000000 braintrust-0.0.9/src/braintrust.egg-info/top_level.txt
```

### Comparing `braintrust-0.0.8/setup.py` & `braintrust-0.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.8/src/braintrust/__init__.py` & `braintrust-0.0.9/src/braintrust/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 import traceback
 import urllib.parse
 import uuid
 from functools import cache as _cache
 from getpass import getpass
 from typing import Any, Dict, Optional
 
+import duckdb
 import git
 import openai
 import requests
 from requests.adapters import HTTPAdapter
 from urllib3.util.retry import Retry
 
 from .cache import CACHE_PATH, EXPERIMENTS_PATH, LOGIN_INFO_PATH
@@ -322,19 +323,22 @@
         with open(experiment_path, "wb") as f:
             f.write(resp.content)
 
     return experiment_path
 
 
 def _parse_scores(duck_cursor, experiment_parquet_file):
-    return set(
-        duck_cursor.query(
-            f"SELECT scores.* FROM parquet_scan({quote_sql_string(experiment_parquet_file)}) LIMIT 0"
-        ).columns
-    )
+    try:
+        return set(
+            duck_cursor.query(
+                f"SELECT scores.* FROM parquet_scan({quote_sql_string(experiment_parquet_file)}) LIMIT 0"
+            ).columns
+        )
+    except duckdb.BinderException:
+        return set()
 
 
 def init(
     project,
     experiment=None,
     description=None,
     base_experiment=None,
@@ -730,14 +734,67 @@
 
         if metadata:
             args["metadata"] = metadata
 
         self.logger.log(args)
         return args["id"]
 
+    def _compute_summary(self, comparison_experiment_id):
+        comparison_experiment_file = _ensure_experiment(comparison_experiment_id)
+
+        self.logger.flush()
+        cursor = duckdb_cursor()
+        cursor.execute(
+            f"COPY (SELECT * FROM {quote_sql_string(self.local_json_path)}) TO {quote_sql_string(self.local_parquet_path)} (FORMAT PARQUET, COMPRESSION 'ZSTD')"
+        )
+
+        overlapping_scores = _parse_scores(cursor, self.local_parquet_path).intersection(
+            _parse_scores(cursor, comparison_experiment_file)
+        )
+
+        if len(overlapping_scores) == 0:
+            return {}
+
+        projections = ", ".join(
+            [
+                textwrap.dedent(
+                    f"""\
+                    struct_pack(
+                        "name" := {quote_sql_string(n)},
+                        "diff" := AVG(e1.scores.{quote_sql_ident(n)})-AVG(e2.scores.{quote_sql_ident(n)}),
+                        "improvements" := SUM(IF(e1.scores.{quote_sql_ident(n)} > e2.scores.{quote_sql_ident(n)}, 1, 0))::bigint,
+                        "regressions" := SUM(IF(e1.scores.{quote_sql_ident(n)} < e2.scores.{quote_sql_ident(n)}, 1, 0))::bigint
+                    ) AS {quote_sql_ident(n)}"""
+                )
+                for n in overlapping_scores
+            ]
+        )
+        query = textwrap.dedent(
+            f"""
+            SELECT {projections}
+            FROM (
+                SELECT e1, e2
+                FROM
+                (
+                    SELECT e1, (SELECT e2 FROM parquet_scan({quote_sql_string(comparison_experiment_file)}) AS e2 WHERE e1.inputs = e2.inputs) e2
+                    FROM parquet_scan({quote_sql_string(self.local_parquet_path)}) AS e1
+                )
+            )
+            """
+        )
+        resp = cursor.query(query)
+        longest_score_name = max(len(n) for n in overlapping_scores)
+        return {
+            k: v
+            for (k, v) in zip(
+                overlapping_scores,
+                [ScoreSummary(_longest_score_name=longest_score_name, **d) for d in resp.fetchone()],
+            )
+        }
+
     def summarize(self, summarize_scores=True, comparison_experiment_id=None):
         """
         Summarize the experiment, including the scores (compared to the closest reference experiment) and metadata.
 
         :param summarize_scores: Whether to summarize the scores. If False, only the metadata will be returned.
         :param comparison_experiment_id: The experiment to compare against. If None, the most recent experiment on the origin's main branch will be used.
         :returns: `ExperimentSummary`
@@ -749,71 +806,21 @@
         comparison_experiment_name = None
         if summarize_scores:
             # Get the comparison experiment
             if comparison_experiment_id is None:
                 conn = api_conn()
                 resp = conn.get("/crud/base_experiments", params={"id": self.id})
                 resp.raise_for_status()
-                comparison_experiment_id = resp.json()[0]["base_exp_id"]
-                comparison_experiment_name = resp.json()[0]["base_exp_name"]
-
-            if comparison_experiment_id is None:
-                raise ValueError(
-                    "No comparison experiment found. Please specify a comparison experiment id or run with summarize_experiment=False"
-                )
-
-            comparison_experiment_file = _ensure_experiment(comparison_experiment_id)
+                base_experiments = resp.json()
+                if base_experiments:
+                    comparison_experiment_id = base_experiments[0]["base_exp_id"]
+                    comparison_experiment_name = base_experiments[0]["base_exp_name"]
 
-            self.logger.flush()
-            cursor = duckdb_cursor()
-            cursor.execute(
-                f"COPY (SELECT * FROM {quote_sql_string(self.local_json_path)}) TO {quote_sql_string(self.local_parquet_path)} (FORMAT PARQUET, COMPRESSION 'ZSTD')"
-            )
-
-            overlapping_scores = _parse_scores(cursor, self.local_parquet_path).intersection(
-                _parse_scores(cursor, comparison_experiment_file)
-            )
-
-            if len(overlapping_scores) > 0:
-                projections = ", ".join(
-                    [
-                        textwrap.dedent(
-                            f"""\
-                            struct_pack(
-                                "name" := {quote_sql_string(n)},
-                                "diff" := AVG(e1.scores.{quote_sql_ident(n)})-AVG(e2.scores.{quote_sql_ident(n)}),
-                                "improvements" := SUM(IF(e1.scores.{quote_sql_ident(n)} > e2.scores.{quote_sql_ident(n)}, 1, 0))::bigint,
-                                "regressions" := SUM(IF(e1.scores.{quote_sql_ident(n)} < e2.scores.{quote_sql_ident(n)}, 1, 0))::bigint
-                            ) AS {quote_sql_ident(n)}"""
-                        )
-                        for n in overlapping_scores
-                    ]
-                )
-                query = textwrap.dedent(
-                    f"""
-                    SELECT {projections}
-                    FROM (
-                        SELECT e1, e2
-                        FROM
-                        (
-                            SELECT e1, (SELECT e2 FROM parquet_scan({quote_sql_string(comparison_experiment_file)}) AS e2 WHERE e1.inputs = e2.inputs) e2
-                            FROM parquet_scan({quote_sql_string(self.local_parquet_path)}) AS e1
-                        )
-                    )
-                    """
-                )
-                resp = cursor.query(query)
-                longest_score_name = max(len(n) for n in overlapping_scores)
-                score_summary = {
-                    k: v
-                    for (k, v) in zip(
-                        overlapping_scores,
-                        [ScoreSummary(_longest_score_name=longest_score_name, **d) for d in resp.fetchone()],
-                    )
-                }
+            if comparison_experiment_id is not None:
+                score_summary = self._compute_summary(comparison_experiment_id)
 
         return ExperimentSummary(
             project_name=self.project.name,
             experiment_name=self.name,
             project_url=project_url,
             experiment_url=experiment_url,
             comparison_experiment_name=comparison_experiment_name,
@@ -867,20 +874,23 @@
     experiment_url: str
     """The experiment scores are baselined against."""
     comparison_experiment_name: Optional[str]
     """Summary of the experiment's scores."""
     scores: Dict[str, ScoreSummary]
 
     def __str__(self):
+        comparison_line = ""
         if self.comparison_experiment_name:
             comparison_line = f"""{self.experiment_name} compared to {self.comparison_experiment_name}:\n"""
         return (
             f"""\n=========================SUMMARY=========================\n{comparison_line}"""
             + "\n".join([str(score) for score in self.scores.values()])
             + "\n\n"
+            if self.scores
+            else ""
             + textwrap.dedent(
                 f"""\
         See results for all experiments in {self.project_name} at {self.project_url}
         See results for {self.experiment_name} at {self.experiment_url}"""
             )
         )
```

### Comparing `braintrust-0.0.8/src/braintrust/cli/__main__.py` & `braintrust-0.0.9/src/braintrust/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.8/src/braintrust/cli/install/api.py` & `braintrust-0.0.9/src/braintrust/cli/install/api.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.8/src/braintrust/cli/install/redshift.py` & `braintrust-0.0.9/src/braintrust/cli/install/redshift.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.8/src/braintrust/gitutil.py` & `braintrust-0.0.9/src/braintrust/gitutil.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.8/src/braintrust/oai.py` & `braintrust-0.0.9/src/braintrust/oai.py`

 * *Files identical despite different names*

### Comparing `braintrust-0.0.8/src/braintrust.egg-info/SOURCES.txt` & `braintrust-0.0.9/src/braintrust.egg-info/SOURCES.txt`

 * *Files identical despite different names*

