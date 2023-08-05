# Comparing `tmp/pystv-0.8.1.tar.gz` & `tmp/pystv-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystv-0.8.1.tar", last modified: Fri Mar 10 05:55:29 2023, max compression
+gzip compressed data, was "pystv-0.9.0.tar", last modified: Tue Apr  4 03:54:18 2023, max compression
```

## Comparing `pystv-0.8.1.tar` & `pystv-0.9.0.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:55:29.943486 pystv-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-03-10 05:55:13.000000 pystv-0.8.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-10 05:55:13.000000 pystv-0.8.1/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-03-10 05:55:13.000000 pystv-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-03-10 05:55:13.000000 pystv-0.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-10 05:55:29.943486 pystv-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-03-10 05:55:13.000000 pystv-0.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:55:29.943486 pystv-0.8.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/Makefile
--rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/pystv.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-03-10 05:55:13.000000 pystv-0.8.1/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-10 05:55:13.000000 pystv-0.8.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:55:29.943486 pystv-0.8.1/pystv/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-03-10 05:55:13.000000 pystv-0.8.1/pystv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-03-10 05:55:13.000000 pystv-0.8.1/pystv/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4682 2023-03-10 05:55:13.000000 pystv-0.8.1/pystv/pystv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3067 2023-03-10 05:55:13.000000 pystv-0.8.1/pystv/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-03-10 05:55:13.000000 pystv-0.8.1/pystv/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3119 2023-03-10 05:55:13.000000 pystv-0.8.1/pystv/viz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:55:29.943486 pystv-0.8.1/pystv.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-10 05:55:29.000000 pystv-0.8.1/pystv.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-03-10 05:55:29.943486 pystv-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-10 05:55:13.000000 pystv-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-10 05:55:29.943486 pystv-0.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/test_pystv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/test_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/test_viz.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/transform_testdata.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-03-10 05:55:13.000000 pystv-0.8.1/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 03:54:18.375747 pystv-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-04 03:53:56.000000 pystv-0.9.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-04 03:53:56.000000 pystv-0.9.0/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-04-04 03:53:56.000000 pystv-0.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-04 03:53:56.000000 pystv-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-04 03:54:18.375747 pystv-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-04 03:53:56.000000 pystv-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 03:54:18.371747 pystv-0.9.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/Makefile
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4884 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/pystv.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-04-04 03:53:56.000000 pystv-0.9.0/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-04 03:53:56.000000 pystv-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 03:54:18.371747 pystv-0.9.0/pystv/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-04-04 03:53:56.000000 pystv-0.9.0/pystv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-04-04 03:53:56.000000 pystv-0.9.0/pystv/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-04 03:53:56.000000 pystv-0.9.0/pystv/pystv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-04-04 03:53:56.000000 pystv-0.9.0/pystv/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-04-04 03:53:56.000000 pystv-0.9.0/pystv/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3125 2023-04-04 03:53:56.000000 pystv-0.9.0/pystv/viz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 03:54:18.371747 pystv-0.9.0/pystv.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 03:54:18.000000 pystv-0.9.0/pystv.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-04 03:54:18.375747 pystv-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-04 03:53:56.000000 pystv-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 03:54:18.375747 pystv-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6323 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/test_pystv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/test_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/test_viz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/transform_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/transform_weighted_testdata.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-04-04 03:53:56.000000 pystv-0.9.0/tests/utils.py
```

### Comparing `pystv-0.8.1/CONTRIBUTING.rst` & `pystv-0.9.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/LICENSE` & `pystv-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/PKG-INFO` & `pystv-0.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystv
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python API for adjudicating single transferable vote elections.  Also contains basic web server to adjudicate results in CSV format.
 Home-page: https://github.com/chrisroat/pystv
 Author: Chris Roat
 Author-email: chris.roat@gmail.com
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/chrisroat/pystv/issues
 Platform: UNKNOWN
```

### Comparing `pystv-0.8.1/README.rst` & `pystv-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/docs/Makefile` & `pystv-0.9.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/docs/conf.py` & `pystv-0.9.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/docs/installation.rst` & `pystv-0.9.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/docs/make.bat` & `pystv-0.9.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/pystv/pystv.py` & `pystv-0.9.0/pystv/pystv.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
     # TODO: Need to add 1 if it evenly divides
     votes_needed = int(np.ceil(np.sum(votes) / (race_info.metadata.num_seats + 1)))
 
     status = np.zeros(num_slots, int)
     status[0] = -2
     valid = np.ones_like(ballots, bool)
+    orig = first_nonzero(valid, axis=1)  # Original candidate on each ballot
 
     round_info = []
     while np.count_nonzero(status > 0) < race_info.metadata.num_seats:
         counts = np.bincount(ballots.ravel(), (weights * votes).ravel(), num_slots)
         counts_masked = np.ma.array(counts, mask=(status != 0))
         elected_mask = counts_masked >= votes_needed
 
@@ -51,15 +52,14 @@
             status[to_remove] = -1
 
         # Distribute votes from elected/eliminated candidates to the next active
         # lower ranked candidate.  Elected candidates transfer excess votes, while
         # eliminated candidates transfer all votes.
         transfers = {}
         for cand, mult in zip(to_remove, multipliers):
-            orig = first_nonzero(valid, axis=1)  # Original candidate on each ballot
             valid[ballots == cand] = False
             next = first_nonzero(valid, axis=1)  # Next active candidate on each ballot
 
             # Ballots where the candidate changed
             o_rows = orig != next
             # Ballots the candidate changed, but where no active candidate remains
             n_rows = o_rows & (next != -1)
@@ -73,14 +73,15 @@
             slicer = n_rows, next[n_rows]
             for c, v in zip(ballots[slicer], (weights * votes)[slicer]):
                 if v:
                     transfers_cand[c] += v
 
             if transfers_cand:
                 transfers[cand] = dict(transfers_cand)
+            orig = next
 
         if not np.isclose(counts.sum(), votes.sum()):
             raise PyStvError("Final round count total does not equal original votes")
 
         round_info.append(
             RoundResult(counts.tolist(), list(elected), list(eliminated), transfers)
         )
```

### Comparing `pystv-0.8.1/pystv/transform.py` & `pystv-0.9.0/pystv/transform.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Utilities to convert ballot formats into pystv standard format."""
 import re
 
 import numpy as np
 import pandas as pd
 
 from .types import PyStvError, RaceInfo, RaceMetadata
 
@@ -19,22 +20,28 @@
     r"\[(?P<option>.*)\]$"
 )
 
 
 def parse_google_form_csv(buffer):
     df = pd.read_csv(buffer)
     race_infos = []
+
+    weights = df["weight"].values if "weight" in df else None
+
     for metadata, slice_ in parse_header(df.columns):
         goog = df.iloc[:, slice_].applymap(coerce).values
         goog = np.ma.array(goog, mask=(goog == 0))
 
         argsort = goog.argsort(axis=1)
         mask = np.take_along_axis(goog.mask, argsort, axis=1)
         ballots = np.ma.array(argsort, mask=mask) + 1
         ballots = ballots.filled(0)
+        if weights is not None:
+            ballots = np.repeat(ballots, weights, axis=0)
+
         ballots, votes = np.unique(ballots, axis=0, return_counts=True)
         race_infos.append(RaceInfo(metadata, ballots.tolist(), votes.tolist()))
     return race_infos
 
 
 def parse_header(header):
     current_question = None
```

### Comparing `pystv-0.8.1/pystv/types.py` & `pystv-0.9.0/pystv/types.py`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/pystv/viz.py` & `pystv-0.9.0/pystv/viz.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 
     labels = ["<exhausted>"] + race_result.metadata.names
     num_cands = len(labels)
 
     node_color = [node_palette[idx % len(node_palette)] for idx in range(num_cands)]
     df_nodes = pd.DataFrame({"label": labels, "color": node_color})
     df_nodes = pd.concat(
-        [df_nodes] * num_rounds, keys=range(num_rounds), names=["round", "id"]
+        [df_nodes] * (num_rounds + 1), keys=range(num_rounds + 1), names=["round", "id"]
     )
     df_nodes = df_nodes.reset_index()
 
     data_links = []
-    for rnd in range(num_rounds - 1):
+    for rnd in range(num_rounds):
         round_result = race_result.rounds[rnd]
         for src in range(num_cands):
             color = link_palette[src % len(link_palette)]
             src_left = round_result.count[src]
             if src in round_result.transfers:
                 for tgt, diff in round_result.transfers[src].items():
                     data_links.append((rnd, src, tgt, diff, color))
@@ -60,29 +60,29 @@
         node=dict(
             thickness=10,
             line={"width": 0},
             label=df_nodes["label"],
             color=df_nodes["color"],
             customdata=df_nodes["round"],
             hovertemplate=(
-                "%{label} has %{value:.0d} votes "
+                "%{label} has %{value:.0f} votes "
                 "in round %{customdata}<extra></extra>"
             ),
         ),
         link=dict(
             source=df_links["source"],
             target=df_links["target"],
             value=df_links["value"],
             color=df_links["color"],
             # For display, add 2 to round:
             # - add 1 because it is the next round that the transfers are counted
             # - add 1 to start indexing from 1 (real people do not like 0-indexing)
             customdata=df_links["round"] + 2,
             hovertemplate=(
-                "%{value:.0d} votes transferred<br />"
+                "%{value:.0f} votes transferred<br />"
                 "from %{source.label} to %{target.label}<br />"
                 "in round %{customdata}<extra></extra>"
             ),
         ),
         visible=True,
     )
```

### Comparing `pystv-0.8.1/pystv.egg-info/PKG-INFO` & `pystv-0.9.0/pystv.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystv
-Version: 0.8.1
+Version: 0.9.0
 Summary: Python API for adjudicating single transferable vote elections.  Also contains basic web server to adjudicate results in CSV format.
 Home-page: https://github.com/chrisroat/pystv
 Author: Chris Roat
 Author-email: chris.roat@gmail.com
 License: GNU General Public License v3
 Project-URL: Bug Tracker, https://github.com/chrisroat/pystv/issues
 Platform: UNKNOWN
```

### Comparing `pystv-0.8.1/pystv.egg-info/SOURCES.txt` & `pystv-0.9.0/pystv.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -32,8 +32,9 @@
 pystv.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/test_pystv.py
 tests/test_transform.py
 tests/test_viz.py
 tests/transform_testdata.csv
+tests/transform_weighted_testdata.csv
 tests/utils.py
```

### Comparing `pystv-0.8.1/setup.cfg` & `pystv-0.9.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pystv
-version = 0.8.1
+version = 0.9.0
 author = Chris Roat
 author_email = chris.roat@gmail.com
 description = Python API for adjudicating single transferable vote elections.  Also contains basic web server to adjudicate results in CSV format.
 license = GNU General Public License v3
 license_files = LICENSE
 long_description = file: README.rst
 long_description_content_type = text/x-rst
```

### Comparing `pystv-0.8.1/tests/test_pystv.py` & `pystv-0.9.0/tests/test_pystv.py`

 * *Files identical despite different names*

### Comparing `pystv-0.8.1/tests/test_viz.py` & `pystv-0.9.0/tests/test_viz.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,33 @@
             RR([0, 2, 5, 3], [2], [], {2: {1: 1}}),
             RR([0, 3, 4, 3], [], [1], {1: {3: 3}}),
             RR([0, 0, 4, 6], [3], [], {}),
         ],
     )
     df_nodes, df_links = pystv.result_to_sankey_data(race_result)
 
-    node_colors = (["rgba(0,0,0,0)"] + pystv.NODE_PALETTE[1:4]) * 3
+    node_colors = ["rgba(0,0,0,0)"] + pystv.NODE_PALETTE[1:4]
     df_nodes_desired = pd.DataFrame(
         {
-            "round": [0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2],
-            "id": [0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3],
-            "label": ([""] + names) * 3,
-            "color": node_colors,
+            "round": [0, 0, 0, 0, 1, 1, 1, 1, 2, 2, 2, 2, 3, 3, 3, 3],
+            "id": [0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3, 0, 1, 2, 3],
+            "label": ([""] + names) * 4,
+            "color": node_colors * 4,
         }
     )
     df_links_desired = pd.DataFrame(
         {
-            "round": [0, 0, 0, 0, 1, 1, 1],
-            "source": [1, 2, 2, 3, 5, 6, 7],
-            "target": [5, 5, 6, 7, 11, 10, 11],
-            "value": [2, 1, 4, 3, 3, 4, 3],
-            "color": [pystv.LINK_PALETTE[i] for i in [1, 2, 2, 3, 1, 2, 3]],
+            "round": [0, 0, 0, 0, 1, 1, 1, 2, 2],
+            "source": [1, 2, 2, 3, 5, 6, 7, 10, 11],
+            "target": [5, 5, 6, 7, 11, 10, 11, 14, 15],
+            "value": [2, 1, 4, 3, 3, 4, 3, 4, 6],
+            "color": [pystv.LINK_PALETTE[i] for i in [1, 2, 2, 3, 1, 2, 3, 2, 3]],
         }
     )
 
+    print(df_links)
     pd.testing.assert_frame_equal(df_nodes, df_nodes_desired, check_like=True)
     pd.testing.assert_frame_equal(df_links, df_links_desired, check_like=True)
 
     # Just make sure this executes (not sure how to test figure generation)
     fig = pystv.create_sankey_fig(df_nodes, df_links)
     assert fig is not None
```

### Comparing `pystv-0.8.1/tests/utils.py` & `pystv-0.9.0/tests/utils.py`

 * *Files identical despite different names*

