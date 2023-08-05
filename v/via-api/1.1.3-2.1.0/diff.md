# Comparing `tmp/via-api-1.1.3.tar.gz` & `tmp/via-api-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-api-1.1.3.tar", last modified: Fri Mar 17 15:01:19 2023, max compression
+gzip compressed data, was "via-api-2.1.0.tar", last modified: Sat Aug  5 10:43:22 2023, max compression
```

## Comparing `via-api-1.1.3.tar` & `via-api-2.1.0.tar`

### file list

```diff
@@ -1,49 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.762000 via-api-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-17 15:01:19.762000 via-api-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-17 15:00:35.000000 via-api-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 15:01:19.762000 via-api-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-03-17 15:00:35.000000 via-api-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.758000 via-api-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.758000 via-api-1.1.3/src/via/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6876 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/bounding_graph_gdfs_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/edge_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.758000 via-api-1.1.3/src/via/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/geojson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/geojson/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/geojson/retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/geojson/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.758000 via-api-1.1.3/src/via/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3613 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18503 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/journey.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/journey_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/journeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    20276 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     5328 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/nearest_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/nearest_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    15880 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/network_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2304 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/place_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/pull_journeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)    12244 2023-03-17 15:00:35.000000 via-api-1.1.3/src/via/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.762000 via-api-1.1.3/src/via_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-03-17 15:01:19.000000 via-api-1.1.3/src/via_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-03-17 15:01:19.000000 via-api-1.1.3/src/via_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 15:01:19.000000 via-api-1.1.3/src/via_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-17 15:01:19.000000 via-api-1.1.3/src/via_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-03-17 15:01:19.000000 via-api-1.1.3/src/via_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-03-17 15:01:19.000000 via-api-1.1.3/src/via_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 15:01:19.762000 via-api-1.1.3/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_base_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_edge_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_nearest_edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1953 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_nearest_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_network_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_place_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     5844 2023-03-17 15:00:35.000000 via-api-1.1.3/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.063264 via-api-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 10:43:22.063264 via-api-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-05 10:42:15.000000 via-api-2.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 10:43:22.063264 via-api-2.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 10:42:15.000000 via-api-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.055264 via-api-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.059265 via-api-2.1.0/src/via/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.059265 via-api-2.1.0/src/via/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/bounding_graph_gdfs_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/edge_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.059265 via-api-2.1.0/src/via/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/geojson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/geojson/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/geojson/retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/geojson/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.063264 via-api-2.1.0/src/via/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18747 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/journey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/journey_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/journeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/network_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/place_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-05 10:42:15.000000 via-api-2.1.0/src/via/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.063264 via-api-2.1.0/src/via_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 10:43:22.000000 via-api-2.1.0/src/via_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 10:43:22.000000 via-api-2.1.0/src/via_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 10:43:22.000000 via-api-2.1.0/src/via_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-05 10:43:22.000000 via-api-2.1.0/src/via_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-05 10:43:22.000000 via-api-2.1.0/src/via_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 10:43:22.000000 via-api-2.1.0/src/via_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 10:43:22.063264 via-api-2.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-05 10:42:16.000000 via-api-2.1.0/test/test_edge_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-05 10:42:16.000000 via-api-2.1.0/test/test_network_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-05 10:42:16.000000 via-api-2.1.0/test/test_place_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-05 10:42:16.000000 via-api-2.1.0/test/test_utils.py
```

### Comparing `via-api-1.1.3/README.md` & `via-api-2.1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,11 @@
 # Via
 
+## Install:
+  - Ensure you have python3.10 installed locally along with python3.10-venv
+
+
 <img src="/assets/logo.png" alt="via logo" style="height: 100px; width:100px;"/>
 
 Road quality assessment from cycling / driving / bussing around, tools to analyse data collected from the android app https://github.com/RobertLucey/road-quality-aggregator
 
 All uploaded data is public and no accounts required. Neat privacy to make it very difficult / impossible (depending on your settings and how many trips have been taken in the area) to find the route of an individual journey as well as its origin / destination
```

### Comparing `via-api-1.1.3/setup.py` & `via-api-2.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,28 +3,31 @@
     setup
 )
 
 INSTALL_REQUIRES = (
     'cached_property',
     'packaging',
     'reverse_geocoder',
-    'fast_json',
-    'boto3',
     'haversine',
     'osmnx',
     'scikit-learn',
     'requests',
     'geopandas',
     'python-logging-loki',
-    'rtree'
+    'rtree',
+    'fastapi[all]',
+    'pydantic',
+    'pymongo',
+    'cachetools',
+    'mappymatch'
 )
 
 setup(
     name='via-api',
-    version='1.1.3',
+    version='2.1.0',
     python_requires='>=3.6',
     description='Analysing and serving crowdsourced road quality data',
     long_description='Analysing and serving crowdsourced road quality data',
     author='Robert Lucey',
     url='https://github.com/RobertLucey/via',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `via-api-1.1.3/src/via/__init__.py` & `via-api-2.1.0/src/via/__init__.py`

 * *Files identical despite different names*

### Comparing `via-api-1.1.3/src/via/edge_cache.py` & `via-api-2.1.0/src/via/edge_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-1.1.3/src/via/geojson/retrieve.py` & `via-api-2.1.0/src/via/geojson/retrieve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-import os
-import time
-import stat
-
-from via.constants import GEOJSON_DIR
-from via.settings import MAX_GEOJSON_AGE
-from via.utils import read_json
-from via.geojson.utils import generate_basename
+import datetime
+
+from via.settings import MAX_GEOJSON_AGE, MONGO_PARSED_JOURNEYS_COLLECTION
+from via.utils import get_mongo_interface
 
 
 def get_geojson(
-    journey_type,
-    earliest_time=None,
-    latest_time=None,
-    place=None,
-    version=None,
-    version_op=None,
-    max_age=None,
-):
+    journey_type: str,
+    earliest_time: int = None,
+    latest_time: int = None,
+    place: str = None,
+    version: str = None,
+    version_op: str = None,
+) -> dict:
+    # TODO: react to version/version_op/earliest_time/latest_time
+
     if journey_type is None:
         journey_type = "all"
 
-    basename = generate_basename(
-        name=journey_type,
-        version=version,
-        version_op=version_op,
-        earliest_time=earliest_time,
-        latest_time=latest_time,
-        place=place,
+    mongo_interface = get_mongo_interface()
+    data = getattr(mongo_interface, MONGO_PARSED_JOURNEYS_COLLECTION).find_one(
+        {
+            "journey_type": journey_type,
+            "save_time": {
+                "$gt": (
+                    datetime.datetime.utcnow()
+                    - datetime.timedelta(seconds=MAX_GEOJSON_AGE)
+                ).timestamp()
+            },
+            "place": place,
+        }
     )
-    geojson_file = os.path.join(GEOJSON_DIR, f"{basename}.geojson")
-
-    if not os.path.exists(geojson_file):
-        raise FileNotFoundError()
-
-    if max_age is None:
-        max_age = MAX_GEOJSON_AGE
+    if not data:
+        raise FileNotFoundError()  # Quick hack
 
-    if time.time() - os.stat(geojson_file)[stat.ST_MTIME] > max_age:
-        raise FileNotFoundError()
+    data["_id"] = str(data["_id"])
 
-    return read_json(geojson_file)
+    return data
```

### Comparing `via-api-1.1.3/src/via/log.py` & `via-api-2.1.0/src/via/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from via.constants import LOG_LOCATION
 
 
 FORMAT = "%(asctime)s|%(levelname)s| %(message)s"
 
 
 class ColourfulFormatter(logging.Formatter):
-
     cyan = "\x1b[36;21m"
     grey = "\x1b[38;21m"
     yellow = "\x1b[33;21m"
     red = "\x1b[31;21m"
     bold_red = "\x1b[31;1m"
     reset = "\x1b[0m"
     format = FORMAT
@@ -36,15 +35,15 @@
         return formatter.format(record)
 
 
 logger = logging.Logger("via", logging.DEBUG)
 
 os.makedirs(os.path.dirname(LOG_LOCATION), exist_ok=True)
 
-if os.getenv("LOKI_ENDPOINT"):
+if os.getenv("LOKI_ENDPOINT"):  # pragma: nocover
     handler = logging_loki.LokiHandler(
         url=os.getenv("LOKI_ENDPOINT"),
         tags={"application": "via"},
         auth=(os.getenv("LOKI_USERNAME"), os.getenv("LOKI_PASSWORD")),
         version="1",
     )
     logger.addHandler(handler)
```

### Comparing `via-api-1.1.3/src/via/models/frame.py` & `via-api-2.1.0/src/via/models/frame.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,18 +46,14 @@
         """
         return (
             isinstance(self.time, float)
             and self.gps.is_populated
             and self.acceleration != []
         )
 
-    @property
-    def road_quality(self) -> int:
-        return int(self.acceleration.quality * 100)
-
     def serialize(self, **kwargs) -> dict:
         data = {"gps": self.gps.serialize(), "acc": self.acceleration}
         if kwargs.get("include_time", True):
             data["time"] = round(self.time, 2)
         return data
```

### Comparing `via-api-1.1.3/src/via/models/gps.py` & `via-api-2.1.0/src/via/models/gps.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,48 +66,42 @@
 
         key = hash((self.point, point))
         if key not in HAVERSINE_CACHE:
             HAVERSINE_CACHE[key] = haversine(self.point, point, unit=Unit.METERS)
 
         return HAVERSINE_CACHE[key]
 
-    def slope_between(self, dst) -> float:
-        from via.models.point import FramePoint
-
-        if isinstance(dst, FramePoint):
-            dst = dst.gps
-        try:
-            return (self.lng - dst.lng) / (self.lat - dst.lat)
-        except ZeroDivisionError:
-            return 0
-
     def serialize(self) -> dict:
         return {"lat": self.lat, "lng": self.lng, "elevation": self.elevation}
 
     @cached_property
     def reverse_geo(self):
         # TODO: make a cache for this for "close enough" positions if we end
         # up using this frequently
-        data = dict(rg.search((self.lat, self.lng))[0])
+        data = dict(rg.search((self.lat, self.lng), mode=1)[0])
         del data["lat"]
         del data["lon"]
         data["place_1"] = data.pop("name", None)
         data["place_2"] = data.pop("admin1", None)
         data["place_3"] = data.pop("admin2", None)
         return data
 
     @cached_property
     def content_hash(self) -> int:
         """
         A content hash that will act as an id for the data, handy for caching
         """
-        return (
-            int.from_bytes(f"{self.lat} {self.lng} {self.elevation}".encode(), "little")
-            % 2**100
-        )
+        input_string = f"{self.lat} {self.lng} {self.elevation}"
+        encoded_int = 0
+
+        for char in input_string:
+            encoded_int = (encoded_int << 8) + ord(char)
+            encoded_int %= 1000000000
+
+        return encoded_int
 
     @property
     def point(self) -> Tuple[float, float]:
         """
 
         :rtype: tuple
         :return: tuple of (lat, lng)
@@ -121,12 +115,12 @@
         or starting up this will not be populated.
 
         Does not consider elevation since it's not important
 
         :rtype: bool
         """
         return (
-            self.lat != 0
-            and self.lng != 0
+            self.lat
+            and self.lng
             and isinstance(self.lat, (int, float))
             and isinstance(self.lng, (int, float))
         )
```

### Comparing `via-api-1.1.3/src/via/models/journey.py` & `via-api-2.1.0/src/via/models/journey.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,42 @@
 import datetime
 import statistics
+from pathlib import Path
 
+from functools import cache
 from collections import defaultdict
-from functools import lru_cache
 from packaging import version
 
 from dateutil.parser import parse
 
 from cached_property import cached_property
 import geopandas as gpd
-import fast_json
 
 from shapely.ops import cascaded_union
 
 import networkx as nx
 import osmnx as ox
 
+from mappymatch.maps.nx.readers.osm_readers import (
+    NetworkType,
+    nx_graph_from_osmnx,
+    parse_osmnx_graph,
+)
+from mappymatch import package_root
+from mappymatch.constructs.geofence import Geofence
+from mappymatch.constructs.trace import Trace
+from mappymatch.maps.nx.nx_map import NxMap
+from mappymatch.matchers.lcss.lcss import LCSSMatcher
+from mappymatch.utils.plot import plot_matches
+
+import pandas
+
 from via import settings
 from via import logger
 from via.utils import window, get_combined_id
-from via.nearest_edge import nearest_edge
 from via.constants import (
     POLY_POINT_BUFFER,
     VALID_JOURNEY_MIN_DISTANCE,
     VALID_JOURNEY_MIN_POINTS,
     VALID_JOURNEY_MIN_DURATION,
 )
 
@@ -34,14 +47,31 @@
 from via.models.journey_mixins import (
     SnappedRouteGraphMixin,
     GeoJsonMixin,
     BoundingGraphMixin,
 )
 
 
+@cache
+def get_nxmap(bounding_graph):
+    return NxMap(parse_osmnx_graph(bounding_graph, NetworkType.BIKE))
+
+
+@cache
+def get_matcher_by_graph(bounding_graph):
+    return LCSSMatcher(
+        get_nxmap(bounding_graph),
+        distance_epsilon=50.0,
+        similarity_cutoff=0.5,
+        cutting_threshold=5.0,  # not too sure what this does
+        random_cuts=0,
+        distance_threshold=100,  # default 10000
+    )
+
+
 class Journey(FramePoints, SnappedRouteGraphMixin, GeoJsonMixin, BoundingGraphMixin):
     """
     A single journey (or patial journey)
 
     Relates to one raw file downloaded through pull_journeys
     """
 
@@ -74,26 +104,26 @@
 
         self.is_culled = kwargs.get("is_culled", False)
         self.is_sent = kwargs.get("is_sent", False)
 
         self.transport_type = str(kwargs.get("transport_type", "unknown")).lower()
         self.suspension = kwargs.get("suspension", None)
 
-        self.network_type = kwargs.get("network_type", "all")
+        self.network_type = kwargs.get("network_type", "bike")
         self._timestamp = kwargs.get("timestamp", None)
 
         self.last_gps = None
 
     def __del__(self):
         attrs_to_del = ["edge_quality_map", "route_graph"]
 
         for attr in attrs_to_del:
             try:
                 delattr(self, attr)
-            except:
+            except Exception:
                 pass
 
     @staticmethod
     def parse(objs):
         """
         Given a dict representation of a Journey (or a Journey object)
         return with a Journey object
@@ -102,33 +132,14 @@
             return objs
 
         if isinstance(objs, dict):
             return Journey(**objs)
 
         raise NotImplementedError(f"Can't parse journey from type {type(objs)}")
 
-    @staticmethod
-    @lru_cache(maxsize=500)
-    def from_file(filepath: str):
-        """
-        Given a file get a Journey object
-
-        :param filepath: Path to a saved journey file
-        :rtype: via.models.journey.Journey
-        """
-        logger.debug("Loading journey from %s", filepath)
-
-        # TODO: should cache stages of processed files from raw (currently,
-        # which uses frames instead of frame points) to processed (which
-        # it will use frame points) so we can skip the building up of context
-        # when we should be able to find from a raw file path
-
-        with open(filepath, "r") as journey_file:
-            return Journey(**fast_json.loads(journey_file.read()))
-
     def set_contexts(self):
         """
         For each of the FramePoints in the journey give each of them
         context of their surrounding points
         """
 
         if len(self._data) < 7:
@@ -143,15 +154,15 @@
             pre=[self._data[0], self._data[1]], post=[self._data[3], self._data[4]]
         )
         self._data[-3].set_context(
             pre=[self._data[-5], self._data[-4]], post=[self._data[-2], self._data[-1]]
         )
 
         # then do normal loop which will skip the ones already set because they'll be on the edge
-        for (one, two, three, four, five, six, seven) in window(self, window_size=7):
+        for one, two, three, four, five, six, seven in window(self, window_size=7):
             if not four.is_context_populated:
                 four.set_context(pre=[one, two, three], post=[five, six, seven])
 
     def extend(self, objs):
         # Possibly shouldn't set contexts here and should be done explicitly
         for obj in objs:
             self.append(obj)
@@ -165,15 +176,15 @@
 
         Though journey data may not have time it will (should) always be
         chronological
         """
         # TODO: warn if not chronological
         if isinstance(obj, FramePoint):
             self._data.append(obj)
-        else:
+        elif isinstance(obj, (dict, Frame)):
             # Most datapoints are only accelerometer so we need to find the
             # closest point with gps in the past to add the accelerometer
             # data to
 
             frame = Frame.parse(obj)
 
             frame_gps_populated = frame.gps.is_populated
@@ -181,17 +192,15 @@
             if frame_gps_populated:
                 if self.gps_inclusion_iter % settings.GPS_INCLUDE_RATIO == 0:
                     self.last_gps = frame.gps
                 else:
                     frame.gps = self.last_gps
                 self.gps_inclusion_iter += 1
             else:
-                if not hasattr(self, "last_gps"):
-                    return
-                if self.last_gps is None:
+                if not self.last_gps:
                     return
                 frame.gps = self.last_gps
 
             if len(self._data) == 0:
                 self._data.append(FramePoint(frame.time, frame.gps, frame.acceleration))
                 return
 
@@ -223,14 +232,16 @@
             else:
                 if self._data[-1].gps == frame.gps:
                     self._data[-1].append_acceleration(frame.acceleration)
                 else:
                     self._data.append(
                         FramePoint(frame.time, frame.gps, frame.acceleration)
                     )
+        else:
+            raise NotImplementedError("Cannot append to journey of type: {type(obj)}")
 
     def get_indirect_distance(self, n_seconds: int = 0) -> float:
         """
         NB: Data must be chronological
 
         :param n_seconds: use the location every n seconds as if the
             location is calculated too frequently the distance
@@ -302,15 +313,15 @@
 
         return data
 
     @property
     def timestamp(self):
         if self._timestamp is None:
             # FIXME: We shouldn't need to do this but the ui always includes earliest / latest as a filter
-            return datetime.datetime(2021, 1, 1)
+            return datetime.datetime(1970, 1, 1)
         return parse(self._timestamp)
 
     @cached_property
     def edge_quality_map(self):
         """
         Get a map between edge_hash and road quality of the road. edge_map
         being edge_id and road quality being something that hasn't been
@@ -338,68 +349,72 @@
 
         return {
             edge_id: d
             for edge_id, d in data.items()
             if d["count"] >= settings.MIN_PER_JOURNEY_USAGE
         }
 
-    @property
+    @cached_property
     def edge_data(self):
         """
-        Get all the edges with their associated data for this journey
+        Get all the edges with their associated data for this journey.
+
+        TODO: replace with a conventional algo for matching
 
         :rtype: dict
         :return: {edge_id: [{edge_data}, {edge_data}]}
         """
+
+        trace = [(p.gps.lat, p.gps.lng) for p in self.all_points]
+        trace = Trace.from_dataframe(pandas.DataFrame(trace), True, 0, 1)
+
+        # This takes a long time, cache it more
+        matcher = get_matcher_by_graph(self.bounding_graph)
+
+        match_result = matcher.match_trace(trace)
+
         data = defaultdict(list)
-        bounding_graph = self.graph
-        route_graph = self.route_graph
 
-        nearest_edge.get(bounding_graph, self._data)
+        for (our_origin, our_destination), match_point in zip(
+            window(self, window_size=2), match_result.matches
+        ):
+            if not match_point or not match_point.road:
+                continue
 
-        raw_edges_list = []
-        for (our_origin, our_destination) in window(self, window_size=2):
-            nearest_edges = nearest_edge.get(bounding_graph, [our_origin])[0]
-
-            edge = our_origin.get_best_edge(
-                nearest_edges,
-                mode=settings.NEAREST_EDGE_METHOD,
-                graph=bounding_graph,
-                include_slow=True,
+            edge = (
+                (match_point.road.road_id.start, match_point.road.road_id.end, 0),
+                0,
             )
 
             our_edge_data = get_edge_data(
-                our_origin.uuid, our_destination.uuid, graph=route_graph
-            )
-
-            raw_edges_list.append(
-                [get_combined_id(edge[0][0], edge[0][1]), our_edge_data]
+                our_origin.uuid, our_destination.uuid, graph=self.route_graph
             )
 
-        edges_list = []
-        for (pre, current, post) in window(raw_edges_list, window_size=3):
-            if pre[0] == post[0] and current[0] != pre[0]:
-                current[0] = pre[0]
-            edges_list.append(current)
+            data[get_combined_id(edge[0][0], edge[0][1])].append(our_edge_data)
 
-        for edge in edges_list:
-            data[edge[0]].append(edge[1])
+        if len(data) < 5:  # TODO: to config
+            return defaultdict(list)
 
         return data
 
+    def write_mappy_path(self):
+        mmap_file = Path(f"/tmp/{self.uuid}_matches_map.html")
+        mmap = plot_matches(match_result.matches)
+        mmap.save(str(mmap_file))
+
     @cached_property
     def route_graph(self):
         """
         Get a graph of the journey without snapping to closest node / edge
         """
         graph = nx.Graph()
 
         combined_edge_data = defaultdict(list)
 
-        for (origin, destination) in window(self, window_size=2):
+        for origin, destination in window(self, window_size=2):
             edge_id = get_combined_id(origin.uuid, destination.uuid)
 
             graph.add_node(origin.uuid, **{"x": origin.gps.lng, "y": origin.gps.lat})
             graph.add_node(
                 destination.uuid, **{"x": destination.gps.lng, "y": destination.gps.lat}
             )
 
@@ -417,15 +432,14 @@
                     else None
                     # TODO: other bits, speed / elevation maybe?
                 }
             )
 
         merged_edge_data = {}
         for shared_id, values in combined_edge_data.items():
-
             merged_edge_data[shared_id] = {
                 "origin": values[0]["origin"],
                 "destination": values[0]["destination"],
                 "distance": values[0]["distance"],
                 "avg_road_quality": statistics.mean(
                     [val["road_quality"] for val in values]
                 ),
@@ -510,18 +524,18 @@
     @property
     def version(self):
         """
         Get the version of the app used to generate this data
 
         :rtype: version.Version
         """
+        if not self._version:
+            return version.parse("0.0.0")
         if isinstance(self._version, version.Version):
             return self._version
-        if isinstance(self._version, type(None)):
-            return version.parse("0.0.0")
         return version.parse(self._version)
 
     @property
     def region(self):
         """
         Get the region name in which this journey started
         """
```

### Comparing `via-api-1.1.3/src/via/models/journey_mixins.py` & `via-api-2.1.0/src/via/models/journey_mixins.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,106 +1,82 @@
-import os
 from collections import defaultdict
 
 import osmnx as ox
+from networkx.classes.multidigraph import MultiDiGraph
 
 from via import settings
 from via import logger
 from via.utils import (
     filter_nodes_from_geodataframe,
     filter_edges_from_geodataframe,
     update_edge_data,
     get_graph_id,
     area_from_coords,
-    write_json,
+    get_combined_id,
 )
-from via.nearest_edge import nearest_edge
 from via.network_cache import network_cache
-from via.constants import GEOJSON_DIR
-
 from via.bounding_graph_gdfs_cache import bounding_graph_gdfs_cache
-
 from via.geojson.utils import geojson_from_graph
 
 
 class SnappedRouteGraphMixin:
     @property
-    def snapped_route_graph(self):
-        """
-        Get the route graph, snapping to the nearest edge
-        """
-        bounding_graph = self.graph
-
-        nearest_edge.get(bounding_graph, self.all_points)
+    def snapped_route_graph(self) -> MultiDiGraph:
+        """ """
+        used_combined_edges = []
+        for journey in self:
+            used_combined_edges.extend(list(journey.edge_data.keys()))
 
-        edges = []
+        bounding_graph = self.graph
+        used_edges = []
         used_node_ids = []
 
-        all_nearest_edges = nearest_edge.get(bounding_graph, self.all_points)
-
-        for our_origin, nearest_edges in list(zip(self.all_points, all_nearest_edges)):
-            edge = our_origin.get_best_edge(
-                nearest_edges, mode=settings.NEAREST_EDGE_METHOD, graph=bounding_graph
-            )
-            if not edge:
-                continue
-
-            edges.append(tuple(edge[0]))
-            used_node_ids.extend([edge[0][0], edge[0][1]])
+        for start, end, _ in bounding_graph.edges:
+            graph_edge_id = get_combined_id(start, end)
+            if graph_edge_id in used_combined_edges:
+                used_node_ids.extend([start, end])
+                used_edges.append(tuple([start, end, 0]))
 
         if bounding_graph_gdfs_cache.get(get_graph_id(bounding_graph)) is None:
             bounding_graph_gdfs_cache.set(
                 get_graph_id(bounding_graph),
                 ox.graph_to_gdfs(bounding_graph, fill_edge_geometry=True),
             )
 
         graph_nodes, graph_edges = bounding_graph_gdfs_cache.get(
             get_graph_id(bounding_graph)
         )
 
-        # Filter only the nodes and edges on the route and ignore the
-        # buffer used to get context
         graph = ox.graph_from_gdfs(
             filter_nodes_from_geodataframe(graph_nodes, used_node_ids),
-            filter_edges_from_geodataframe(graph_edges, edges),
+            filter_edges_from_geodataframe(graph_edges, used_edges),
         )
 
         return update_edge_data(graph, self.edge_quality_map)
 
 
 class GeoJsonMixin:
-    def save_geojson(self):
-        geojson_file = os.path.join(GEOJSON_DIR, self.content_hash + ".geojson")
-
-        if not os.path.exists(geojson_file):
-            logger.debug("%s not found, generating...", geojson_file)
-
-            write_json(geojson_file, self.geojson)
-
     @property
-    def geojson(self):
+    def geojson(self) -> dict:
         """
         Write and return a GeoJSON object string of the graph.
         """
 
-        geojson_file = os.path.join(GEOJSON_DIR, self.content_hash + ".geojson")
-
-        logger.debug("%s generating...", geojson_file)
-
         from via.models.journeys import Journeys
 
         if isinstance(self, Journeys):
             region_map = defaultdict(Journeys)
 
             for journey in self:
                 # use place_2 as place_1 is too specific and a journey that
                 # starts in a place_1 could share roads with a journey that
                 # starts in a different area nearby
                 # This is also a possible issue with place_2 but will happen
                 # much less, still a FIXME
+                # {'cc': 'IE', 'place_1': 'Rathgar', 'place_2': 'Leinster', 'place_3': 'Dublin City'}
                 region_name = journey.origin.gps.reverse_geo["place_2"]
                 region_map[region_name].append(journey)
 
             if len(region_map) > 1:
                 geo_features = []
                 for region_name, journeys in region_map.items():
                     logger.debug(
@@ -112,42 +88,48 @@
                 geo_features = {"type": "FeatureCollection", "features": geo_features}
                 return geo_features
 
             return geojson_from_graph(
                 self.snapped_route_graph, must_include_props=["count", "avg", "edge_id"]
             )
 
+        # TODO: Does this *need* to return edge_id (or any other props)?
+        # edge_id not used in front end seemingly and other nullables can be
+        # handled wherever... edge_id wasn't being returned for any data I
+        # tried so this is a hack for now.
         return geojson_from_graph(
-            self.snapped_route_graph, must_include_props=["count", "avg", "edge_id"]
+            # self.snapped_route_graph, must_include_props=["count", "avg", "edge_id"]
+            self.snapped_route_graph,
+            must_include_props=None,
         )
 
 
 class BoundingGraphMixin:
-    def get_bounding_graph(self, use_graph_cache: bool = True):
+    def get_bounding_graph(self, use_graph_cache: bool = True) -> MultiDiGraph:
         logger.debug(
             "Plotting bounding graph (n,s,e,w) (%s, %s, %s, %s)",
             self.most_northern,
             self.most_southern,
             self.most_eastern,
             self.most_western,
         )
 
-        if use_graph_cache is False or network_cache.get("bbox", self) is None:
+        if use_graph_cache is False or network_cache.get(self) is None:
             logger.debug("bbox > %s not found in cache, generating...", self.gps_hash)
             network = ox.graph_from_bbox(
                 self.most_northern,
                 self.most_southern,
                 self.most_eastern,
                 self.most_western,
                 network_type=self.network_type,
                 simplify=True,
             )
-            network_cache.set("bbox", self, network)
+            network_cache.set(network, self.bbox)
 
-        return network_cache.get("bbox", self)
+        return network_cache.get(self)
 
     @property
     def bounding_graph(self):
         """
         Get a rectangular graph which contains the journey
         """
         return self.get_bounding_graph(use_graph_cache=True)
```

### Comparing `via-api-1.1.3/src/via/models/journeys.py` & `via-api-2.1.0/src/via/models/journeys.py`

 * *Files 13% similar despite different names*

```diff
@@ -104,20 +104,14 @@
     def get_graph(self, use_graph_cache=True):
         return self.get_bounding_graph(use_graph_cache=use_graph_cache)
 
     @property
     def graph(self) -> MultiDiGraph:
         return self.get_graph(use_graph_cache=True)
 
-    @staticmethod
-    def from_files(filepaths):
-        with closing(multiprocessing.Pool(multiprocessing.cpu_count() - 1)) as pool:
-            journeys = list(pool.imap_unordered(Journey.from_file, filepaths))
-        return Journeys(data=journeys)
-
     @property
     def gps_hash(self) -> str:
         """
         Get the hash of all the GPSs of the points in all the journeys
         """
         return hashlib.md5(
             str([journey.gps_hash for journey in self]).encode()
@@ -129,25 +123,14 @@
         Get the hash of the contents of all the journeys
         """
         return hashlib.md5(
             str([journey.content_hash for journey in self]).encode()
         ).hexdigest()
 
     @property
-    def all_points(self) -> List:
-        """
-        Return all the points in this journeys obj
-        """
-        return flatten([journey.all_points for journey in self._data])
-
-    @property
     def bbox(self):
         return {
             "north": self.most_northern,
             "south": self.most_southern,
             "east": self.most_eastern,
             "west": self.most_western,
         }
-
-    @property
-    def regions(self):
-        return [journey.region for journey in self]
```

### Comparing `via-api-1.1.3/src/via/place_cache.py` & `via-api-2.1.0/src/via/place_cache.py`

 * *Files 7% similar despite different names*

```diff
@@ -20,27 +20,27 @@
                 "north": 53.626487,
                 "south": 53.3018049,
                 "east": -6.1366563,
                 "west": -6.433500,
             }
         }
 
-    def get_by_bbox(self, cmp_bbox):
+    def get_by_bbox(self, cmp_bbox: dict) -> dict:
         """
         Given a bbox, return a dict of the place name and bbox of the
         place it is within
 
         :param cmp_bbox:
         """
         for name, bbox in self.data.items():
             if is_within(cmp_bbox, bbox):
                 return {"name": name, "bbox": bbox}
         return None
 
-    def is_in_place(self, bbox: dict, place_name: str):
+    def is_in_place(self, bbox: dict, place_name: str) -> bool:
         """
         Return if a box is within the confines of a 'place'
 
         :param bbox: dict representing a lat/lng bbox
         :param place_name: the name of a place
         """
         place_name = place_name.lower().replace(",", "")
```

### Comparing `via-api-1.1.3/src/via_api.egg-info/SOURCES.txt` & `via-api-2.1.0/src/via_api.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 README.md
 setup.py
 src/via/__init__.py
-src/via/base_cache.py
 src/via/bounding_graph_gdfs_cache.py
 src/via/constants.py
 src/via/edge_cache.py
 src/via/log.py
-src/via/nearest_edge.py
-src/via/nearest_node.py
 src/via/network_cache.py
 src/via/place_cache.py
-src/via/pull_journeys.py
 src/via/settings.py
 src/via/utils.py
+src/via/api/__init__.py
+src/via/api/main.py
 src/via/geojson/__init__.py
 src/via/geojson/generate.py
 src/via/geojson/retrieve.py
 src/via/geojson/utils.py
 src/via/models/__init__.py
 src/via/models/frame.py
 src/via/models/generic.py
@@ -27,14 +25,11 @@
 src/via/models/point.py
 src/via_api.egg-info/PKG-INFO
 src/via_api.egg-info/SOURCES.txt
 src/via_api.egg-info/dependency_links.txt
 src/via_api.egg-info/entry_points.txt
 src/via_api.egg-info/requires.txt
 src/via_api.egg-info/top_level.txt
-test/test_base_cache.py
 test/test_edge_cache.py
-test/test_nearest_edge.py
-test/test_nearest_node.py
 test/test_network_cache.py
 test/test_place_cache.py
 test/test_utils.py
```

### Comparing `via-api-1.1.3/test/test_edge_cache.py` & `via-api-2.1.0/test/test_edge_cache.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import json
+import os
 
-from unittest import TestCase, skip
+from unittest import TestCase, skip, skipUnless
 
 from via.models.journey import Journey
 from via.models.frame import Frame
 
 from via.edge_cache import get_edge_data
 
 
+IS_ACTION = os.environ.get("IS_ACTION", "False") == "True"
+
+
 class EdgeCacheTest(TestCase):
     def setUp(self):
-
         with open("test/resources/just_route.json") as json_file:
             self.test_data = json.load(json_file)
 
         self.test_journey = Journey()
         for d in self.test_data:
             self.test_journey.append(
                 Frame(
                     d["time"],
                     {"lat": d["lat"], "lng": d["lng"]},
                     1,  # acceleration, don't really care at the mo
                 )
             )
 
+    @skipUnless(not IS_ACTION, "action_mongo")
     def test_get(self):
         self.assertEqual(
             get_edge_data(389281, 135109553, graph=self.test_journey.graph)[0]["osmid"],
             14039949,
         )
         self.assertEqual(
             get_edge_data(389281, 135109553, graph=self.test_journey.graph)[0]["name"],
             "York Street",
         )
 
     def test_get_no_graph(self):
         self.assertEqual(get_edge_data(1, 2, graph=None), None)
 
+    @skipUnless(not IS_ACTION, "action_mongo")
     def test_caching(self):
         self.assertEqual(
             get_edge_data(389281, 135109553, graph=self.test_journey.graph)[0]["osmid"],
             14039949,
         )
         self.assertEqual(
             get_edge_data(389281, 135109553, graph=self.test_journey.graph)[0]["name"],
```

### Comparing `via-api-1.1.3/test/test_place_cache.py` & `via-api-2.1.0/test/test_place_cache.py`

 * *Files identical despite different names*

