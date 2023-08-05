# Comparing `tmp/via-api-2.2.0.tar.gz` & `tmp/via-api-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "via-api-2.2.0.tar", last modified: Sat Aug  5 11:18:40 2023, max compression
+gzip compressed data, was "via-api-2.3.0.tar", last modified: Sat Aug  5 13:02:37 2023, max compression
```

## Comparing `via-api-2.2.0.tar` & `via-api-2.3.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.976475 via-api-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 11:18:40.976475 via-api-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-05 11:17:34.000000 via-api-2.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 11:18:40.976475 via-api-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 11:17:34.000000 via-api-2.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.964475 via-api-2.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.964475 via-api-2.2.0/src/via/
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.968475 via-api-2.2.0/src/via/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/api/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/bounding_graph_gdfs_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/edge_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.968475 via-api-2.2.0/src/via/geojson/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/geojson/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/geojson/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/geojson/retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/geojson/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.972475 via-api-2.2.0/src/via/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/gps.py
--rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/journey.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/journey_mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/journeys.py
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/models/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/network_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2326 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/place_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-05 11:17:34.000000 via-api-2.2.0/src/via/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.972475 via-api-2.2.0/src/via_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 11:18:40.000000 via-api-2.2.0/src/via_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 11:18:40.000000 via-api-2.2.0/src/via_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:18:40.000000 via-api-2.2.0/src/via_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-05 11:18:40.000000 via-api-2.2.0/src/via_api.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-05 11:18:40.000000 via-api-2.2.0/src/via_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 11:18:40.000000 via-api-2.2.0/src/via_api.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:18:40.976475 via-api-2.2.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-05 11:17:35.000000 via-api-2.2.0/test/test_edge_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-05 11:17:35.000000 via-api-2.2.0/test/test_network_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-05 11:17:35.000000 via-api-2.2.0/test/test_place_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-05 11:17:35.000000 via-api-2.2.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.773734 via-api-2.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 13:02:37.773734 via-api-2.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-08-05 13:01:24.000000 via-api-2.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 13:02:37.773734 via-api-2.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-08-05 13:01:24.000000 via-api-2.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.765734 via-api-2.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.765734 via-api-2.3.0/src/via/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.769734 via-api-2.3.0/src/via/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/api/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/bounding_graph_gdfs_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/edge_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.769734 via-api-2.3.0/src/via/geojson/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/geojson/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/geojson/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/geojson/retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/geojson/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.769734 via-api-2.3.0/src/via/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3977 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/journey.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/journey_mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3928 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/journeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/models/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/network_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/place_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8867 2023-08-05 13:01:24.000000 via-api-2.3.0/src/via/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.769734 via-api-2.3.0/src/via_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-08-05 13:02:37.000000 via-api-2.3.0/src/via_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-08-05 13:02:37.000000 via-api-2.3.0/src/via_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 13:02:37.000000 via-api-2.3.0/src/via_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-05 13:02:37.000000 via-api-2.3.0/src/via_api.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-08-05 13:02:37.000000 via-api-2.3.0/src/via_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-05 13:02:37.000000 via-api-2.3.0/src/via_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 13:02:37.773734 via-api-2.3.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-08-05 13:01:25.000000 via-api-2.3.0/test/test_edge_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-08-05 13:01:25.000000 via-api-2.3.0/test/test_network_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-08-05 13:01:25.000000 via-api-2.3.0/test/test_place_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8865 2023-08-05 13:01:25.000000 via-api-2.3.0/test/test_utils.py
```

### Comparing `via-api-2.2.0/README.md` & `via-api-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/setup.py` & `via-api-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     'pymongo',
     'cachetools',
     'mappymatch'
 )
 
 setup(
     name='via-api',
-    version='2.2.0',
+    version='2.3.0',
     python_requires='>=3.6',
     description='Analysing and serving crowdsourced road quality data',
     long_description='Analysing and serving crowdsourced road quality data',
     author='Robert Lucey',
     url='https://github.com/RobertLucey/via',
     packages=find_packages('src'),
     package_dir={'': 'src'},
```

### Comparing `via-api-2.2.0/src/via/__init__.py` & `via-api-2.3.0/src/via/__init__.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/api/main.py` & `via-api-2.3.0/src/via/api/main.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/bounding_graph_gdfs_cache.py` & `via-api-2.3.0/src/via/bounding_graph_gdfs_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/constants.py` & `via-api-2.3.0/src/via/constants.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/edge_cache.py` & `via-api-2.3.0/src/via/edge_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/geojson/generate.py` & `via-api-2.3.0/src/via/geojson/generate.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/geojson/retrieve.py` & `via-api-2.3.0/src/via/geojson/retrieve.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/geojson/utils.py` & `via-api-2.3.0/src/via/geojson/utils.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/log.py` & `via-api-2.3.0/src/via/log.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/models/frame.py` & `via-api-2.3.0/src/via/models/frame.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/models/generic.py` & `via-api-2.3.0/src/via/models/generic.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/models/gps.py` & `via-api-2.3.0/src/via/models/gps.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/models/journey.py` & `via-api-2.3.0/src/via/models/journey.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/models/journey_mixins.py` & `via-api-2.3.0/src/via/models/journey_mixins.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/models/journeys.py` & `via-api-2.3.0/src/via/models/journeys.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,19 +28,15 @@
 class Journeys(
     GenericObjects, SnappedRouteGraphMixin, GeoJsonMixin, BoundingGraphMixin
 ):
     def __init__(self, *args, **kwargs):
         kwargs.setdefault("child_class", Journey)
         super().__init__(*args, **kwargs)
 
-        network_types = [journey.network_type for journey in self]
-        if len(set(network_types)) == 0 or len(set(network_types)) > 1:
-            self.network_type = "all"
-        elif len(set(network_types)) == 1:
-            self.network_type = network_types[0]
+        self.network_type = "bike"
 
     @property
     def edge_quality_map(self):
         """
         Get a map between edge_hash and road quality of the road. edge_map
         being edge id and road quality being something that hasn't been
         defined yet TODO
```

### Comparing `via-api-2.2.0/src/via/models/point.py` & `via-api-2.3.0/src/via/models/point.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/network_cache.py` & `via-api-2.3.0/src/via/network_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/place_cache.py` & `via-api-2.3.0/src/via/place_cache.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         :return: A dict of north, south, east, and west
             lats and lngs
         """
         place_name = place_name.lower().replace(",", "")
         try:
             return self.data[place_name]
         except KeyError:
-            place_graph = ox.graph_from_place(place_name, network_type="all")
+            place_graph = ox.graph_from_place(place_name, network_type="bike")
 
             lats = []
             lngs = []
             for _, node_data in place_graph._node.items():
                 lats.append(node_data["y"])
                 lngs.append(node_data["x"])
```

### Comparing `via-api-2.2.0/src/via/settings.py` & `via-api-2.3.0/src/via/settings.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via/utils.py` & `via-api-2.3.0/src/via/utils.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/src/via_api.egg-info/SOURCES.txt` & `via-api-2.3.0/src/via_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/test/test_edge_cache.py` & `via-api-2.3.0/test/test_edge_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/test/test_network_cache.py` & `via-api-2.3.0/test/test_network_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/test/test_place_cache.py` & `via-api-2.3.0/test/test_place_cache.py`

 * *Files identical despite different names*

### Comparing `via-api-2.2.0/test/test_utils.py` & `via-api-2.3.0/test/test_utils.py`

 * *Files identical despite different names*

