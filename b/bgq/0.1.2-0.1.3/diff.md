# Comparing `tmp/bgq-0.1.2.tar.gz` & `tmp/bgq-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bgq-0.1.2.tar", max compression
+gzip compressed data, was "bgq-0.1.3.tar", max compression
```

## Comparing `bgq-0.1.2.tar` & `bgq-0.1.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     5458 2023-02-20 21:26:17.931828 bgq-0.1.2/bgq.py
--rw-r--r--   0        0        0     1174 2023-02-20 21:27:09.476555 bgq-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     5152 2023-01-27 00:43:31.635971 bgq-0.1.2/webint_jobs/__init__.py
--rw-r--r--   0        0        0      354 2023-01-27 00:43:31.639971 bgq-0.1.2/webint_jobs/templates/__init__.py
--rw-r--r--   0        0        0      139 2023-01-27 00:43:31.639971 bgq-0.1.2/webint_jobs/templates/by_module.html
--rw-r--r--   0        0        0      620 2023-01-27 00:43:31.647971 bgq-0.1.2/webint_jobs/templates/by_object.html
--rw-r--r--   0        0        0     1064 2023-01-27 00:43:31.643971 bgq-0.1.2/webint_jobs/templates/index.html
--rw-r--r--   0        0        0     1086 2023-01-27 00:43:31.643971 bgq-0.1.2/webint_jobs/templates/job.html
--rw-r--r--   0        0        0     1217 2023-01-27 00:43:31.647971 bgq-0.1.2/webint_jobs/templates/run.html
--rw-r--r--   0        0        0     1040 2023-01-27 00:43:31.639971 bgq-0.1.2/webint_jobs/templates/schedules.html
--rw-r--r--   0        0        0      612 2023-01-27 00:43:31.635971 bgq-0.1.2/webint_jobs/templates/slow.html
--rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 bgq-0.1.2/setup.py
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 bgq-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     5511 2023-02-20 22:11:58.266189 bgq-0.1.3/bgq.py
+-rw-r--r--   0        0        0     1174 2023-02-20 22:14:58.032658 bgq-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5152 2023-01-27 00:43:31.635971 bgq-0.1.3/webint_jobs/__init__.py
+-rw-r--r--   0        0        0      354 2023-01-27 00:43:31.639971 bgq-0.1.3/webint_jobs/templates/__init__.py
+-rw-r--r--   0        0        0      139 2023-01-27 00:43:31.639971 bgq-0.1.3/webint_jobs/templates/by_module.html
+-rw-r--r--   0        0        0      620 2023-01-27 00:43:31.647971 bgq-0.1.3/webint_jobs/templates/by_object.html
+-rw-r--r--   0        0        0     1064 2023-01-27 00:43:31.643971 bgq-0.1.3/webint_jobs/templates/index.html
+-rw-r--r--   0        0        0     1086 2023-01-27 00:43:31.643971 bgq-0.1.3/webint_jobs/templates/job.html
+-rw-r--r--   0        0        0     1217 2023-01-27 00:43:31.647971 bgq-0.1.3/webint_jobs/templates/run.html
+-rw-r--r--   0        0        0     1040 2023-01-27 00:43:31.639971 bgq-0.1.3/webint_jobs/templates/schedules.html
+-rw-r--r--   0        0        0      612 2023-01-27 00:43:31.635971 bgq-0.1.3/webint_jobs/templates/slow.html
+-rw-r--r--   0        0        0      967 1970-01-01 00:00:00.000000 bgq-0.1.3/setup.py
+-rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 bgq-0.1.3/PKG-INFO
```

### Comparing `bgq-0.1.2/bgq.py` & `bgq-0.1.3/bgq.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,22 +149,24 @@
 
         def run_worker(domain, db, cache_db, browser):
             while True:
                 for job in db.select("job_runs", where="started is null"):
                     handle_job(domain, job["job_id"], db, cache_db, browser)
                 time.sleep(0.5)
 
-        for db_filename in pathlib.Path().glob("site.db"):
-            domain = "TODO"  # XXX db_filename.stem.removeprefix("site-")
-            log.info(f"Watching for jobs at: {domain}")
-            # XXX sqldb = sqlyte.db(f"site-{domain}.db")
-            # XXX cache_db = sqlyte.db(f"cache-{domain}.db")
-            sqldb = sqlyte.db("site.db")
-            cache_db = sqlyte.db("cache.db")
-            for _ in range(worker_count):
-                gevent.spawn(run_worker, domain, sqldb, cache_db, browser)
+        while not pathlib.Path("site.db").exists():
+            time.sleep(1)
+        # for db_filename in pathlib.Path().glob("site.db"):
+        domain = "localhost"  # XXX db_filename.stem.removeprefix("site-")
+        log.info(f"Watching for jobs at: {domain}")
+        # XXX sqldb = sqlyte.db(f"site-{domain}.db")
+        # XXX cache_db = sqlyte.db(f"cache-{domain}.db")
+        sqldb = sqlyte.db("site.db")
+        cache_db = sqlyte.db("cache.db")
+        for _ in range(worker_count):
+            gevent.spawn(run_worker, domain, sqldb, cache_db, browser)
         try:
             while True:
                 time.sleep(1)
         except KeyboardInterrupt:  # TODO capture supervisord's kill signal
             if self.browser:
                 browser.quit()
```

### Comparing `bgq-0.1.2/pyproject.toml` & `bgq-0.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bgq"
-version = "0.1.2"
+version = "0.1.3"
 description = "a simple asynchronous background job queue"
 homepage = "https://ragt.ag/code/projects/bgq"
 repository = "https://ragt.ag/code/projects/bgq.git"
 documentation = "https://ragt.ag/code/projects/bgq/api"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-2-Clause"
 packages = [{include="bgq.py"}, {include="webint_jobs"}]
```

### Comparing `bgq-0.1.2/webint_jobs/__init__.py` & `bgq-0.1.3/webint_jobs/__init__.py`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/webint_jobs/templates/by_object.html` & `bgq-0.1.3/webint_jobs/templates/by_object.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/webint_jobs/templates/index.html` & `bgq-0.1.3/webint_jobs/templates/index.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/webint_jobs/templates/job.html` & `bgq-0.1.3/webint_jobs/templates/job.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/webint_jobs/templates/run.html` & `bgq-0.1.3/webint_jobs/templates/run.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/webint_jobs/templates/schedules.html` & `bgq-0.1.3/webint_jobs/templates/schedules.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/webint_jobs/templates/slow.html` & `bgq-0.1.3/webint_jobs/templates/slow.html`

 * *Files identical despite different names*

### Comparing `bgq-0.1.2/setup.py` & `bgq-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
  'webint>0.0.569']
 
 entry_points = \
 {'console_scripts': ['bgq = bgq:main'], 'webapps': ['jobs = webint_jobs:app']}
 
 setup_kwargs = {
     'name': 'bgq',
-    'version': '0.1.2',
+    'version': '0.1.3',
     'description': 'a simple asynchronous background job queue',
     'long_description': 'None',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/projects/bgq',
```

### Comparing `bgq-0.1.2/PKG-INFO` & `bgq-0.1.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bgq
-Version: 0.1.2
+Version: 0.1.3
 Summary: a simple asynchronous background job queue
 Home-page: https://ragt.ag/code/projects/bgq
 License: BSD-2-Clause
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.10,<3.11
 Classifier: License :: OSI Approved :: BSD License
```

