# Comparing `tmp/mereja-0.0.6.tar.gz` & `tmp/mereja-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mereja-0.0.6.tar", last modified: Fri Aug  4 20:45:20 2023, max compression
+gzip compressed data, was "mereja-0.0.7.tar", last modified: Sat Aug  5 07:09:18 2023, max compression
```

## Comparing `mereja-0.0.6.tar` & `mereja-0.0.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:45:20.269714 mereja-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-08-04 20:45:20.269714 mereja-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4832 2023-08-04 20:45:10.000000 mereja-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:45:20.269714 mereja-0.0.6/mereja/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:45:20.269714 mereja-0.0.6/mereja/functions/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/functions/forex.py
--rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/functions/jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/functions/market.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/functions/news.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/functions/telebirr.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:45:20.269714 mereja-0.0.6/mereja/ui/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/forex_table_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/job_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/marketpalce_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/news_view_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/transaction_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:45:20.269714 mereja-0.0.6/mereja/ui/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/ui/widgets/header.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-08-04 20:45:10.000000 mereja-0.0.6/mereja/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 20:45:20.269714 mereja-0.0.6/mereja.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5196 2023-08-04 20:45:20.000000 mereja-0.0.6/mereja.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-04 20:45:20.000000 mereja-0.0.6/mereja.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 20:45:20.000000 mereja-0.0.6/mereja.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-04 20:45:20.000000 mereja-0.0.6/mereja.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 20:45:20.000000 mereja-0.0.6/mereja.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-04 20:45:20.000000 mereja-0.0.6/mereja.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-04 20:45:20.273714 mereja-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-04 20:45:10.000000 mereja-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-05 07:09:18.265019 mereja-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4810 2023-08-05 07:09:09.000000 mereja-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.261019 mereja-0.0.7/mereja/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/mereja/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/forex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2597 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2913 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/news.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/functions/telebirr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/mereja/ui/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/forex_table_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/job_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4149 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/marketpalce_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/news_view_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/transaction_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.265019 mereja-0.0.7/mereja/ui/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/ui/widgets/header.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-08-05 07:09:09.000000 mereja-0.0.7/mereja/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:09:18.261019 mereja-0.0.7/mereja.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-08-05 07:09:18.000000 mereja-0.0.7/mereja.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-08-05 07:09:18.265019 mereja-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-08-05 07:09:09.000000 mereja-0.0.7/setup.py
```

### Comparing `mereja-0.0.6/PKG-INFO` & `mereja-0.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Mereja
 
-[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
-# Currently working on python3.11
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
 ## Features
 
 - Scrape and display the latest news articles.
```

### Comparing `mereja-0.0.6/README.md` & `mereja-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Mereja
 
-[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
-# Currently working on python3.11
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
 ## Features
 
 - Scrape and display the latest news articles.
```

### Comparing `mereja-0.0.6/mereja/functions/forex.py` & `mereja-0.0.7/mereja/functions/forex.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/functions/jobs.py` & `mereja-0.0.7/mereja/functions/jobs.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/functions/market.py` & `mereja-0.0.7/mereja/functions/market.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/functions/news.py` & `mereja-0.0.7/mereja/functions/news.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/functions/telebirr.py` & `mereja-0.0.7/mereja/functions/telebirr.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/main.py` & `mereja-0.0.7/mereja/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,126 +2,21 @@
 import asyncio
 import sys
 
 import questionary
 
 from mereja import constants
 from mereja.functions import forex, telebirr, market, news, jobs
-from mereja.utils import awaitable, Back
-
-questions = [
-    {
-        "type": "select",
-        "name": "answer",
-        "message": "What do you want to do?",
-        "choices": [
-            "📈 Forex",
-            "📝 News",
-            "💼 Jobs",
-            "🛍 Marketplace",
-            "💳 Telebirr",
-            "🛑 Exit",
-        ],
-    },
-    {
-        "type": "select",
-        "name": "forex_choice",
-        "message": "What do you want to do?",
-        "choices": [
-            "📈 Get forex",
-            "📈 🚦 Get forex Live",
-            "📂 Export forex data",
-            "🔙 Back",
-        ],
-        "qmark": "📈",
-        "when": lambda answers: answers.get("answer") == "📈 Forex",
-    },
-    {
-        "type": "select",
-        "name": "choice",
-        "message": "What do you want to do with news?",
-        "choices": ["📝 Get latest news", "🔍 Search for news", "🔙 Back"],
-        "qmark": "📝",
-        "when": lambda answers: answers.get("answer") == "📝 News",
-    },
-    {
-        "type": "select",
-        "name": "choice",
-        "message": "What do you want to do with jobs?",
-        "choices": ["Get latest jobs", "🔍 Search for jobs", "🔙 Back"],
-        "qmark": "💼",
-        "when": lambda answers: answers.get("answer") == "💼 Jobs",
-    },
-    {
-        "type": "select",
-        "name": "choice",
-        "message": "What do you want to do with marketplace?",
-        "choices": ["📈 Get trending products", "🔍 Search for products", "🔙 Back"],
-        "qmark": "🛍",
-        "when": lambda answers: answers.get("answer") == "🛍 Marketplace",
-    },
-    {
-        "type": "select",
-        "name": "telebirr_choice",
-        "message": "What do you want to do with telebirr?",
-        "choices": ["💳 Transaction Details", "📂 Export transaction data", "🔙 Back"],
-        "qmark": "💳",
-        "when": lambda answers: answers.get("answer") == "💳 Telebirr",
-    },
-    {
-        "type": "text",
-        "name": "transaction_id",
-        "message": "💳 Enter your transaction ID:",
-        "when": lambda answers: answers.get("telebirr_choice")
-        in ["💳 Transaction Details", "📂 Export transaction data"],
-    },
-    {
-        "type": "confirm",
-        "name": "exit",
-        "message": "Are you sure you want to exit?",
-        "default": True,
-        "when": lambda answers: answers.get("answer") == "🛑 Exit",
-    },
-    {
-        "type": "text",
-        "name": "search",
-        "message": "Enter your search query:",
-        "when": lambda answers: "Search" in answers.get("choice", ""),
-    },
-    {
-        "type": "text",
-        "name": "path",
-        "message": "Enter the path to save the file:",
-        "when": lambda answers: answers.get("forex_choice") in ["📂 Export forex data"]
-        or answers.get("telebirr_choice") in ["📂 Export transaction data"],
-        "validate": lambda val: (val and val.endswith(".json"))
-        or "Path must end with .json",
-    },
-    {
-        "type": "text",
-        "name": "page",
-        "message": "Enter the page number:",
-        "when": lambda answers: answers.get("choice")
-        in [
-            "Get latest jobs",
-            "📝 Get latest news",
-            "📈 Get trending products",
-            "🔍 Search for products",
-        ],
-        "validate": lambda val: val.isdigit() or "Page number must be a number",
-        "filter": lambda val: int(val),
-        "default": "1",
-    },
-]
+from mereja.utils import awaitable
 
 
 @awaitable
 def show_menu():
     ans = questionary.prompt(
-        questions,
+        constants.QUESTIONS,
         style=constants.STYLE,
         qmark="📡",
     )
     return ans
 
 
 async def parse_answers(answers):
@@ -198,99 +93,93 @@
         except KeyboardInterrupt:
             print("Exiting...")
             sys.exit(0)
 
 
 def runner(args):
     loop = asyncio.get_event_loop()
-    try:
-        if args.job:
-            if args.search:
-                loop.run_until_complete(jobs.search_for_job(query=args.search))
-            # elif args.gov:
-            #     loop.run_until_complete(jobs.get_government_jobs())
-            elif args.latest:
-                if args.export:
-                    loop.run_until_complete(
-                        jobs.export_latest_jobs(path=args.path, limit=args.limit)
-                    )
-                    return
-                loop.run_until_complete(jobs.get_latest_jobs())
-
-        elif args.news:
+    if args.job:
+        if args.search:
+            loop.run_until_complete(jobs.search_for_job(query=args.search))
+        # elif args.gov:
+        #     loop.run_until_complete(jobs.get_government_jobs())
+        elif args.latest:
             if args.export:
                 loop.run_until_complete(
-                    news.export_news(
-                        path=args.path,
-                        limit=args.limit,
-                        page=args.page + 1 if not args.page else args.page,
-                    )
+                    jobs.export_latest_jobs(path=args.path, limit=args.limit)
                 )
                 return
-            if args.search:
-                if args.export:
-                    loop.run_until_complete(
-                        news.export_news(
-                            query=args.search, path=args.path, limit=args.limit
-                        )
-                    )
+            loop.run_until_complete(jobs.get_latest_jobs())
+
+    elif args.news:
+        if args.export:
+            loop.run_until_complete(
+                news.export_news(
+                    path=args.path,
+                    limit=args.limit,
+                    page=args.page + 1 if not args.page else args.page,
+                )
+            )
+            return
+        if args.search:
+            if args.export:
                 loop.run_until_complete(
-                    news.search_news(
-                        query=args.search, page=args.page, limit=args.limit
+                    news.export_news(
+                        query=args.search, path=args.path, limit=args.limit
                     )
                 )
-                return
-            loop.run_until_complete(news.get_news(page=args.page))
+            loop.run_until_complete(
+                news.search_news(query=args.search, page=args.page, limit=args.limit)
+            )
+            return
+        loop.run_until_complete(news.get_news(page=args.page))
 
-        elif args.marketplace:
-            if args.trending:
-                if args.export:
-                    loop.run_until_complete(
-                        market.export_products(path=args.path, limit=args.limit)
-                    )
-                    return
+    elif args.marketplace:
+        if args.trending:
+            if args.export:
                 loop.run_until_complete(
-                    market.get_trending_products(
-                        page=args.page + 1 if not args.page else args.page,
-                        limit=args.limit,
-                    )
+                    market.export_products(path=args.path, limit=args.limit)
                 )
-            if args.search:
-                loop.run_until_complete(
-                    market.search_for_product(
-                        query=args.search,
-                        page=args.page + 1 if not args.page else args.page,
-                        limit=args.limit,
-                    )
+                return
+            loop.run_until_complete(
+                market.get_trending_products(
+                    page=args.page + 1 if not args.page else args.page,
+                    limit=args.limit,
                 )
+            )
+        if args.search:
+            loop.run_until_complete(
+                market.search_for_product(
+                    query=args.search,
+                    page=args.page + 1 if not args.page else args.page,
+                    limit=args.limit,
+                )
+            )
 
-        elif args.telebirr:
-            if args.transaction:
-                if args.export:
-                    loop.run_until_complete(
-                        telebirr.export_transaction(args.transaction, args.path)
-                    )
-                    return
-                loop.run_until_complete(telebirr.check_transaction(args.transaction))
-
-        elif args.forex:
+    elif args.telebirr:
+        if args.transaction:
             if args.export:
-                loop.run_until_complete(forex.export_forex_data(args.path))
+                loop.run_until_complete(
+                    telebirr.export_transaction(args.transaction, args.path)
+                )
                 return
-            loop.run_until_complete(forex.get_forex(args.live))
+            loop.run_until_complete(telebirr.check_transaction(args.transaction))
 
-        elif args.export:
-            loop.run_until_complete(
-                telebirr.export_transaction(args.transaction, args.path)
-            )
-        else:
-            loop.run_until_complete(ask_questions())
-    except KeyboardInterrupt:
-        print("Bye!")
-        sys.exit()
+    elif args.forex:
+        if args.export:
+            loop.run_until_complete(forex.export_forex_data(args.path))
+            return
+        loop.run_until_complete(forex.get_forex(args.live))
+
+    elif args.export:
+        loop.run_until_complete(
+            telebirr.export_transaction(args.transaction, args.path)
+        )
+    else:
+        loop.run_until_complete(ask_questions())
 
 
 def main():
     parser = argparse.ArgumentParser(
         description=(
             "Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a "
             "Text-based User Interface (TUI). The app allows users to access and display various data, including the "
```

### Comparing `mereja-0.0.6/mereja/ui/forex_table_ui.py` & `mereja-0.0.7/mereja/ui/forex_table_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/ui/job_view_ui.py` & `mereja-0.0.7/mereja/ui/job_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/ui/marketpalce_ui.py` & `mereja-0.0.7/mereja/ui/marketpalce_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/ui/news_view_ui.py` & `mereja-0.0.7/mereja/ui/news_view_ui.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/ui/transaction_table.py` & `mereja-0.0.7/mereja/ui/transaction_table.py`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/mereja/ui/widgets/header.py` & `mereja-0.0.7/mereja/ui/widgets/header.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from datetime import datetime
+from typing import Union
 
 from rich.text import Text
 from textual import events
 from textual.app import RenderResult
 from textual.events import Mount
 from textual.reactive import Reactive
 from textual.widget import Widget
@@ -92,16 +93,16 @@
     tall: Reactive[bool] = Reactive(False)
 
     def __init__(
         self,
         show_clock: bool = False,
         title: str = "</> with ❤️ by @wizkiye",
         *,
-        classes: str | None = None,
-        id: str | None = None,
+        classes: Union[str, None] = None,
+        id: Union[str, None] = None,
     ):
         super().__init__(classes=classes, id=id)
         self._show_clock = show_clock
         self.title = title
 
     def compose(self):
         yield HeaderIcon()
```

### Comparing `mereja-0.0.6/mereja/utils.py` & `mereja-0.0.7/mereja/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from mereja import constants
 
 
 class Back(Exception):
     pass
 
 
+# utility functions
 def random_spinner():
     return random.choice(constants.SPINNERS)
 
 
 def rmv_etb(text: str) -> float:
     if isinstance(text, str):
         return round(float(re.search(r"(\d+\.\d+)", text).group(1)), 4)
@@ -59,34 +60,28 @@
                 "buy": f.find("td", attrs={"width": "94"}).get_text(strip=True),
                 "sell": f.find("td", attrs={"width": "102"}).get_text(strip=True),
             }
             for f in table
         ]
 
 
+# table functions
 def loop_colum(table: Table, columns: List):
     for column in columns:
         with beat(5):
             table.add_column(column)
 
 
 def loop_row(table: Table, rows: List[tuple]):
     for row in rows:
         with beat(5):
             table.add_row(*row)
 
 
 async def ask(message: str, choice: List[Choice]):
-    # choice.append(
-    #     Choice(
-    #         title="🔙 Back",
-    #         value="back",
-    #     )
-    # )
-
     return await questionary.select(
         message=message,
         choices=choice,
         qmark="📝",
         style=constants.STYLE,
         use_arrow_keys=True,
         use_jk_keys=True,
@@ -95,15 +90,14 @@
 
 
 def make_qr(data: str):
     qr = qrcode.QRCode(
         version=1,
         error_correction=qrcode.constants.ERROR_CORRECT_L,
         box_size=1,
-        border=4,
     )
     qr.add_data(data)
     f = io.StringIO()
     qr.print_ascii(out=f)
     f.seek(0)
     return f.read()
 
@@ -118,16 +112,14 @@
             ) as status:
                 try:
                     await func(*args, **kwargs, status=status)
                 except ConnectError:
                     console.print("[bold red]No internet connection.")
                     exit(1)
                 except KeyboardInterrupt:
-                    # print("Exiting...")
-                    # exit(0)
                     return
                 except ConnectTimeout:
                     console.print("[bold red]Connection timeout.")
                     exit(1)
                 except Exception as e:
                     print(e)
                     exit(1)
@@ -160,13 +152,10 @@
 def no_ans_or_back(ans: str):
     if not ans:
         raise KeyboardInterrupt
 
 
 def clean_emoji(text: str) -> str:
     return re.compile(
-        "[^\U00000000-\U0000d7ff\U0000e000-\U0000ffff]", flags=re.UNICODE
+        "[^\U00000000-\U0000d7ff\U0000e000-\U0000ffff]",
+        flags=re.UNICODE,
     ).sub("", text)
-
-
-if __name__ == "__main__":
-    print(clean_emoji("hello 🔙"))
```

### Comparing `mereja-0.0.6/mereja.egg-info/PKG-INFO` & `mereja-0.0.7/mereja.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: mereja
-Version: 0.0.6
+Version: 0.0.7
 Home-page: https://github.com/wizkiye/mereja
 Author: Kidus
 Author-email: wizkiye@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # Mereja
 
-[![Python](https://img.shields.io/badge/python-3.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
+[![Python](https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C%203.10%20%7C%203.11-blue)](https://www.python.org/)
 
-# Currently working on python3.11
 
 ## Description
 Mereja is a versatile Python application that provides both a Command-Line Interface (CLI) and a Text-based User Interface (TUI). The app allows users to access and display various data, including the latest news, jobs, forex data, trending products for marketplaces, and telebirr transaction details. Additionally, it provides a search functionality for finding jobs, news articles, and marketplace products, making it a one-stop solution for information retrieval.
 
 ## Features
 
 - Scrape and display the latest news articles.
```

### Comparing `mereja-0.0.6/mereja.egg-info/SOURCES.txt` & `mereja-0.0.7/mereja.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mereja-0.0.6/setup.py` & `mereja-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def read_file(filename: str):
     with open(filename, encoding="utf-8") as f:
         return f.read()
 
 
 setup(
     name="mereja",
-    version="0.0.6",
+    version="0.0.7",
     packages=find_packages(),
     url="https://github.com/wizkiye/mereja",
     license="MIT",
     author="Kidus",
     author_email="wizkiye@gmail.com",
     description="",
     install_requires=[
@@ -30,9 +30,9 @@
         "console_scripts": [
             "mereja = mereja.main:main",
         ],
     },
     long_description=read_file("README.md"),
     long_description_content_type="text/markdown",
     include_package_data=True,
-    python_requires=">=3.9",
+    python_requires=">=3.8",
 )
```

