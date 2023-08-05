# Comparing `tmp/sliderule-3.6.0.tar.gz` & `tmp/sliderule-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliderule-3.6.0.tar", last modified: Mon Jul 10 20:01:50 2023, max compression
+gzip compressed data, was "sliderule-3.7.0.tar", last modified: Sat Aug  5 15:17:19 2023, max compression
```

## Comparing `sliderule-3.6.0.tar` & `sliderule-3.7.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.114854 sliderule-3.6.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-07-10 20:01:35.000000 sliderule-3.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      149 2023-07-10 20:01:35.000000 sliderule-3.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-10 20:01:50.114854 sliderule-3.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-07-10 20:01:35.000000 sliderule-3.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       59 2023-07-10 20:01:35.000000 sliderule-3.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-10 20:01:50.114854 sliderule-3.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-07-10 20:01:35.000000 sliderule-3.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.110854 sliderule-3.6.0/sliderule/
--rw-r--r--   0 runner    (1001) docker     (122)      221 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30636 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/earthdata.py
--rw-r--r--   0 runner    (1001) docker     (122)    17363 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/gedi.py
--rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/h5.py
--rw-r--r--   0 runner    (1001) docker     (122)    34802 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/icesat2.py
--rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/io.py
--rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/ipxapi.py
--rw-r--r--   0 runner    (1001) docker     (122)    85029 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/ipysliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)     6578 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/raster.py
--rw-r--r--   0 runner    (1001) docker     (122)    45770 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/sliderule.py
--rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/swot.py
--rw-r--r--   0 runner    (1001) docker     (122)      322 2023-07-10 20:01:35.000000 sliderule-3.6.0/sliderule/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.114854 sliderule-3.6.0/sliderule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      584 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-07-10 20:01:50.000000 sliderule-3.6.0/sliderule.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-10 20:01:50.114854 sliderule-3.6.0/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/big_query.py
--rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_3dep_DEM_geojson.py
--rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_arctic_dem_mosaics_index.py
--rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_arctic_dem_mosaics_vrt_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/build_arctic_dem_strips_vrt.py
--rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/extract_h5_dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/icepyx_region.py
--rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/lpdaac_download.py
--rw-r--r--   0 runner    (1001) docker     (122)      256 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/lpdaac_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     6618 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (122)      922 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_cmr.py
--rw-r--r--   0 runner    (1001) docker     (122)      677 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_elevations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_photons.py
--rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_stac.py
--rw-r--r--   0 runner    (1001) docker     (122)      612 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/query_version.py
--rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/region_of_interest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/results_to_s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/stac.py
--rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/stream_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/tail_events.py
--rw-r--r--   0 runner    (1001) docker     (122)     6260 2023-07-10 20:01:35.000000 sliderule-3.6.0/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-07-10 20:01:35.000000 sliderule-3.6.0/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 15:17:19.228341 sliderule-3.7.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1524 2023-08-05 15:17:11.000000 sliderule-3.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      149 2023-08-05 15:17:11.000000 sliderule-3.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-08-05 15:17:19.228341 sliderule-3.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-08-05 15:17:11.000000 sliderule-3.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       59 2023-08-05 15:17:11.000000 sliderule-3.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-05 15:17:19.228341 sliderule-3.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1202 2023-08-05 15:17:11.000000 sliderule-3.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 15:17:19.224341 sliderule-3.7.0/sliderule/
+-rw-r--r--   0 runner    (1001) docker     (122)      221 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32195 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/earthdata.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17363 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/gedi.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9808 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/h5.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34802 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/icesat2.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38844 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/io.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5523 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/ipxapi.py
+-rw-r--r--   0 runner    (1001) docker     (122)    85515 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/ipysliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6578 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/raster.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45781 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/sliderule.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12772 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/swot.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-05 15:17:11.000000 sliderule-3.7.0/sliderule/version.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 15:17:19.224341 sliderule-3.7.0/sliderule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      584 2023-08-05 15:17:19.000000 sliderule-3.7.0/sliderule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1042 2023-08-05 15:17:19.000000 sliderule-3.7.0/sliderule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-05 15:17:19.000000 sliderule-3.7.0/sliderule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-08-05 15:17:19.000000 sliderule-3.7.0/sliderule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-08-05 15:17:19.000000 sliderule-3.7.0/sliderule.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-05 15:17:19.228341 sliderule-3.7.0/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/big_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3640 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/build_3dep_DEM_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1581 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/build_arctic_dem_mosaics_index.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1690 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/build_arctic_dem_mosaics_vrt_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2341 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/build_arctic_dem_strips_vrt.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/create_geojson.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1140 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/extract_h5_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2126 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/icepyx_region.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4055 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/lpdaac_download.py
+-rw-r--r--   0 runner    (1001) docker     (122)      322 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/lpdaac_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6468 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)      924 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/query_cmr.py
+-rw-r--r--   0 runner    (1001) docker     (122)      677 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/query_elevations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1405 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/query_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/query_photons.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1034 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/query_stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/query_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3175 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/region_of_interest.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1087 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/results_to_s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1828 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/stac.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1305 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/stream_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/tail_events.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6260 2023-08-05 15:17:11.000000 sliderule-3.7.0/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-05 15:17:11.000000 sliderule-3.7.0/version.txt
```

### Comparing `sliderule-3.6.0/LICENSE` & `sliderule-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/PKG-INFO` & `sliderule-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.6.0
+Version: 3.7.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.6.0/README.md` & `sliderule-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/setup.py` & `sliderule-3.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule/earthdata.py` & `sliderule-3.7.0/sliderule/earthdata.py`

 * *Files 3% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
 # default maximum number of resources to process in one request
 DEFAULT_MAX_REQUESTED_RESOURCES = 300
 max_requested_resources = DEFAULT_MAX_REQUESTED_RESOURCES
 
 # best effort match of datasets to providers and versions for earthdata
 DATASETS = {
-    "ATL03":                                               {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "formats": [".h5"],    "collections": [] },
-    "ATL06":                                               {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "formats": [".h5"],    "collections": []},
-    "ATL08":                                               {"provider": "NSIDC_ECS",   "version": "005",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "ATL03":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": [] },
+    "ATL06":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": []},
+    "ATL08":                                               {"provider": "NSIDC_ECS",   "version": "006",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI01_B":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI02_A":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI02_B":                                            {"provider": "LPDAAC_ECS",  "version": "002",  "api": "cmr",   "formats": [".tiff"],  "collections": []},
     "GEDI_L3_LandSurface_Metrics_V2_1952":                 {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI_L4A_AGB_Density_V2_1_2056":                      {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".h5"],    "collections": []},
     "GEDI_L4B_Gridded_Biomass_2017":                       {"provider": "ORNL_CLOUD",  "version": None,   "api": "cmr",   "formats": [".tiff"],  "collections": []},
     "HLS":                                                 {"provider": "LPCLOUD",     "version": None,   "api": "stac",  "formats": [".tiff"],  "collections": ["HLSS30.v2.0", "HLSL30.v2.0"]},
@@ -174,14 +174,43 @@
     # return granule metadata
     # - time start and time end
     # - time granule was updated
     # - granule size in bits
     # - polygons as geodataframe geometry
     return granule_metadata
 
+def __cmr_collection_query(provider, short_name):
+    """Perform a CMR query for collection metadata."""
+    # build params
+    cmr_query_type = 'collections'
+    cmr_format = 'json'
+    CMR_URL = 'https://cmr.earthdata.nasa.gov'
+    cmr_query_url = '/'.join([CMR_URL, 'search', f'{cmr_query_type}.{cmr_format}'])
+    # build list of CMR query parameters
+    params = []
+    params.append(f'?provider={provider}')
+    params.append(f'&short_name={short_name}')
+    # full CMR query url
+    cmr_query_url += "".join(params)
+    logger.debug(f'cmr request={cmr_query_url}\n')
+    # ssl context
+    ctx = ssl.create_default_context()
+    ctx.check_hostname = False
+    ctx.verify_mode = ssl.CERT_NONE
+    # query CMR for collection metadata
+    req = urllib.request.Request(cmr_query_url)
+    response = urllib.request.urlopen(req, context=ctx)
+    # read the CMR search as JSON
+    search_results = json.loads(response.read().decode('utf8'))
+    # return only valid collection entries
+    if 'feed' not in search_results or 'entry' not in search_results['feed']:
+        return []
+    else:
+        return search_results['feed']['entry']
+
 def __cmr_query(provider, short_name, version, time_start, time_end, **kwargs):
     """Perform a scrolling CMR query for files matching input criteria."""
     kwargs.setdefault('polygon',None)
     kwargs.setdefault('name_filter',None)
     kwargs.setdefault('return_metadata',False)
     # build params
     params = '&short_name={0}'.format(short_name)
@@ -307,14 +336,27 @@
 
     if return_metadata:
         return (url_list,meta_list)
     else:
         return url_list
 
 #
+# Get the maximum available version for a dataset from CMR
+#
+def __cmr_max_version(provider, short_name):
+    """Get the maximum version of a dataset from CMR."""
+    entries = __cmr_collection_query(provider, short_name)
+    version_ids = [e['version_id'] for e in entries]
+    # return only when there was valid collection entries
+    if not version_ids:
+        return None
+    else:
+        return max(version_ids)
+
+#
 # Build a GeoJSON Response from STAC Query Response
 #
 def __build_geojson(rsps):
     geojson = rsps.json()
     del geojson["links"]
     if 'numberMatched' in geojson:
         del geojson['numberMatched']
```

### Comparing `sliderule-3.6.0/sliderule/gedi.py` & `sliderule-3.7.0/sliderule/gedi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule/h5.py` & `sliderule-3.7.0/sliderule/h5.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule/icesat2.py` & `sliderule-3.7.0/sliderule/icesat2.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 # profiling times for each major function
 profiles = {}
 
 # default asset
 DEFAULT_ASSET="icesat2"
 
 # default standard data product version
-DEFAULT_ICESAT2_SDP_VERSION='005'
+DEFAULT_ICESAT2_SDP_VERSION='006'
 
 # icesat2 parameters
 CNF_POSSIBLE_TEP = -2
 CNF_NOT_CONSIDERED = -1
 CNF_BACKGROUND = 0
 CNF_WITHIN_10M = 1
 CNF_SURFACE_LOW = 2
```

### Comparing `sliderule-3.6.0/sliderule/io.py` & `sliderule-3.7.0/sliderule/io.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule/ipxapi.py` & `sliderule-3.7.0/sliderule/ipxapi.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule/ipysliderule.py` & `sliderule-3.7.0/sliderule/ipysliderule.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,16 +100,16 @@
                 "\n\tATL08: Land and Vegetation Height"),
             disabled=False,
             style=self.style,
         )
 
         # dropdown menu for setting data release
         self.release = ipywidgets.Dropdown(
-            options=['003', '004', '005'],
-            value='005',
+            options=['003', '004', '005', '006'],
+            value='006',
             description='Release:',
             description_tooltip="Release: ICESat-2 data release",
             disabled=False,
             style=self.style,
         )
 
         self.start_date = ipywidgets.DatePicker(
@@ -347,15 +347,15 @@
             readout_format='d',
             style=self.style,
         )
 
         # slider for setting maximum number of iterations
         # (not including initial least-squares-fit selection)
         self.iteration = ipywidgets.IntSlider(
-            value=1,
+            value=6,
             min=0,
             max=20,
             step=1,
             description='Iterations:',
             description_tooltip=("Iterations: maximum number of iterations, "
                 "not including initial least-squares-fit selection"),
             disabled=False,
@@ -428,14 +428,17 @@
             continuous_update=False,
             orientation='horizontal',
             readout=True,
             readout_format='0.1f',
             style=self.style,
         )
 
+        # watch widgets for changes
+        self.length.observe(self.set_default_values_from_length)
+
         # dropdown menu for setting map projection
         # Global: Web Mercator (EPSG:3857)
         # North: Alaska Polar Stereographic (EPSG:5936)
         # South: Polar Stereographic South (EPSG:3031)
         projection_list = ['Global','North','South']
         self.projection = ipywidgets.Dropdown(
             options=projection_list,
@@ -728,14 +731,22 @@
 
     @property
     def time_end(self):
         """end time in ISO format
         """
         return self.end_date.value.isoformat()
 
+    # function for setting default values when segment length changes
+    def set_default_values_from_length(self, sender):
+        """function for setting default values when segment length changes
+        """
+        self.step.value = int(self.length.value//2)
+        self.spread.value = self.length.value/2.0
+        self.count.value = np.maximum(5, self.length.value//4)
+
     # function for setting available map layers
     def set_layers(self, sender):
         """function for updating available map layers
         """
         if (self.projection.value == 'Global'):
             layer_options = ['3DEP','ASTER GDEM','ESRI imagery','GLIMS','RGI']
         elif (self.projection.value == 'North'):
```

### Comparing `sliderule-3.6.0/sliderule/raster.py` & `sliderule-3.7.0/sliderule/raster.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule/sliderule.py` & `sliderule-3.7.0/sliderule/sliderule.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 logger = logging.getLogger(__name__)
 
 clustering_enabled = False
 try:
     from sklearn.cluster import KMeans
     clustering_enabled = True
 except:
-    logger.warning("Unable to import sklearn... clustering support disabled")
+    logger.info("Unable to import sklearn... clustering support disabled")
 
 recdef_table = {}
 
 arrow_file_table = {}
 
 profiles = {}
 
@@ -1028,15 +1028,15 @@
 #
 def gps2utc (gps_time, as_str=True):
     '''
     Convert a GPS based time returned from SlideRule into a UTC time.
 
     Parameters
     ----------
-        gps_time:   int
+        gps_time:   float
                     number of seconds since GPS epoch (January 6, 1980)
         as_str:     bool
                     if True, returns the time as a string; if False, returns the time as datatime object
 
     Returns
     -------
     datetime
@@ -1044,15 +1044,15 @@
 
     Examples
     --------
         >>> import sliderule
         >>> sliderule.gps2utc(1235331234)
         '2019-02-27 19:34:03'
     '''
-    rsps = source("time", {"time": gps_time, "input": "GPS", "output": "DATE"})
+    rsps = source("time", {"time": int(gps_time * 1000), "input": "GPS", "output": "DATE"})
     if as_str:
         return rsps["time"]
     else:
         return datetime.strptime(rsps["time"], '%Y-%m-%dT%H:%M:%SZ')
 #
 # get_definition
 #
```

### Comparing `sliderule-3.6.0/sliderule/swot.py` & `sliderule-3.7.0/sliderule/swot.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/sliderule.egg-info/PKG-INFO` & `sliderule-3.7.0/sliderule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sliderule
-Version: 3.6.0
+Version: 3.7.0
 Summary: Python client for interacting with sliderule server
 Home-page: https://github.com/ICESat2-SlideRule/sliderule/
 Author: SlideRule Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sliderule-3.6.0/sliderule.egg-info/SOURCES.txt` & `sliderule-3.7.0/sliderule.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 sliderule.egg-info/requires.txt
 sliderule.egg-info/top_level.txt
 utils/big_query.py
 utils/build_3dep_DEM_geojson.py
 utils/build_arctic_dem_mosaics_index.py
 utils/build_arctic_dem_mosaics_vrt_list.py
 utils/build_arctic_dem_strips_vrt.py
+utils/create_geojson.py
 utils/extract_h5_dataset.py
 utils/icepyx_region.py
 utils/lpdaac_download.py
 utils/lpdaac_list.py
 utils/monitor.py
 utils/query_cmr.py
 utils/query_elevations.py
```

### Comparing `sliderule-3.6.0/utils/big_query.py` & `sliderule-3.7.0/utils/big_query.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/build_3dep_DEM_geojson.py` & `sliderule-3.7.0/utils/build_3dep_DEM_geojson.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/build_arctic_dem_mosaics_index.py` & `sliderule-3.7.0/utils/build_arctic_dem_mosaics_index.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/build_arctic_dem_mosaics_vrt_list.py` & `sliderule-3.7.0/utils/build_arctic_dem_mosaics_vrt_list.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/build_arctic_dem_strips_vrt.py` & `sliderule-3.7.0/utils/build_arctic_dem_strips_vrt.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/extract_h5_dataset.py` & `sliderule-3.7.0/utils/extract_h5_dataset.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/icepyx_region.py` & `sliderule-3.7.0/utils/icepyx_region.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/lpdaac_download.py` & `sliderule-3.7.0/utils/lpdaac_download.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/monitor.py` & `sliderule-3.7.0/utils/monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -33,21 +33,21 @@
     if trace["stop"] == None:
         trace["stop"] = trace["start"]
     # Get values of trace
     trace_id        = trace["start"]['id']
     thread_id       = trace["start"]['tid']
     start_time      = trace["start"]['time']
     stop_time       = trace["stop"]['time']
-    sec_from_origin = start_time / 1e3
-    sec_duration    = (stop_time - start_time) / 1e3
-    dt              = sliderule.gps2utc(sec_from_origin)
+    sec_from_origin = start_time / 1e6
+    sec_duration    = (stop_time - start_time) / 1e6
+    dt              = sec_from_origin
     name            = trace["start"]['name']
     attributes      = trace["start"]['attr']
     # Print trace
-    print('{} ({:7.3f} sec):{:{indent}}{:{width}} <{}> {} [{}]'.format(dt, sec_duration, "", str(name), thread_id, attributes, trace_id, indent=depth, width=30-depth))
+    print('{:.3f} ({:7.3f} sec):{:{indent}}{:{width}} <{}> {} [{}]'.format(dt, sec_duration, "", str(name), thread_id, attributes, trace_id, indent=depth, width=30-depth))
     # Recurse on children
     for child in trace["children"]:
         display_trace(child, depth + 2)
 
 def write_sta_events(filename, df):
     f = open(filename, "w")
     for index,row in df.iterrows():
@@ -75,46 +75,45 @@
         f.write("Calc CPU=True\n")
         f.write("Color=%d\n" % (COLOR_MAP[depth - 1]))
         f.write("Hide=False\n")
         f.write("DuplicateEdgeWarningsDisabled=False\n")
         index += 1
     f.close()
 
-def build_event_list(trace, depth, max_depth, names, events, perf_ids):
-    # Get Perf ID
+def build_event_list(trace, depth, max_depth, names, events, perf_ids, filter_list):
     name = trace["name"]
+    # Filter
+    if name.split(".")[0] in filter_list:
+        return
+    # Get Perf ID
     perf_id = names.index(name)
     perf_ids[name] = {"id": perf_id, "depth": depth}
     # Append Events
     try:
         events.append({"id": perf_id, "time": trace["start"]["time"], "edge": 0})
         events.append({"id": perf_id, "time": trace["stop"]["time"], "edge": 1})
     except:
         pass
     # Recurse on Children
     if (depth < max_depth) or (max_depth == 0):
         for child in trace["children"]:
-            build_event_list(child, depth + 1, max_depth, names, events, perf_ids)
+            build_event_list(child, depth + 1, max_depth, names, events, perf_ids, filter_list)
 
 def console_output(origins):
     # Output traces to console
     for trace in origins:
         display_trace(trace, 1)
 
-def sta_output(idlist, depth, names, traces):
+def sta_output(filter_list, depth, names, traces):
     global origins
     # Build list of events and names
     events = []
     perf_ids = {}
-    if len(idlist) > 0:
-        for trace_id in idlist:
-            build_event_list(traces[trace_id], 1, depth, names, events, perf_ids)
-    else:
-        for trace in origins:
-            build_event_list(trace, 1, depth, names, events, perf_ids)
+    for trace in origins:
+        build_event_list(trace, 1, depth, names, events, perf_ids, filter_list)
     # Build and sort data frame
     df = pandas.DataFrame(events)
     df = df.sort_values("time")
     # Build delta times
     df["delta"] = df["time"].diff()
     df.at[0, "delta"] = 0.0
     # Write out data frame as sta events
@@ -158,38 +157,36 @@
 
     # Default Parameters
     parms = {
         "url": "localhost",
         "organization": None,
         "fmt": "console",
         "depth": 0,
-        "ids": []
+        "filter": []
     }
 
     # Override Parameters
-    parms = parse_command_line(sys.argv, parms)
+    parse_command_line(sys.argv, parms)
 
     # Default Request
     rqst = {
         "type": LOG | TRACE,
         "level" : "INFO",
         "duration": 30
     }
 
     # Override Request
-    rqst = parse_command_line(sys.argv, rqst)
+    parse_command_line(sys.argv, rqst)
 
     # Set URL and Organization
     sliderule.set_url(parms["url"])
     sliderule.authenticate(parms["organization"])
 
     # Connect to SlideRule
     rsps = sliderule.source("event", rqst, stream=True, callbacks={'eventrec': process_event})
 
-    # Flatten names to get indexes
+    # Flatten Names to Get Indexes
     names = list(names)
 
-    # Run commanded operation
-    if parms["fmt"] == "console":
-        console_output(origins)
-    elif parms["fmt"] == "sta":
-        sta_output(parms["ids"], parms["depth"], names, traces)
+    # Output Traces
+    console_output(origins)
+    sta_output(parms["filter"], parms["depth"], names, traces)
```

### Comparing `sliderule-3.6.0/utils/query_cmr.py` & `sliderule-3.7.0/utils/query_cmr.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 # MAIN
 ###############################################################################
 
 if __name__ == '__main__':
 
     # Defaults
     cfg = {
-        "region": "examples/grandmesa.geojson",
+        "region": "tests/data/grandmesa.geojson",
         "tolerance": 0.0,
         "dataset": "ATL03",
-        "version": "005",
+        "version": "006",
     }
 
     # Command line parameters
     parse_command_line(sys.argv, cfg)
 
     # Override region of interest
     region = sliderule.toregion(cfg["region"], cfg["tolerance"])
```

### Comparing `sliderule-3.6.0/utils/query_elevations.py` & `sliderule-3.7.0/utils/query_elevations.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/query_metrics.py` & `sliderule-3.7.0/utils/query_metrics.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/query_photons.py` & `sliderule-3.7.0/utils/query_photons.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/query_stac.py` & `sliderule-3.7.0/utils/query_stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/query_version.py` & `sliderule-3.7.0/utils/query_version.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/region_of_interest.py` & `sliderule-3.7.0/utils/region_of_interest.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/results_to_s3.py` & `sliderule-3.7.0/utils/results_to_s3.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/stac.py` & `sliderule-3.7.0/utils/stac.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/stream_events.py` & `sliderule-3.7.0/utils/stream_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/tail_events.py` & `sliderule-3.7.0/utils/tail_events.py`

 * *Files identical despite different names*

### Comparing `sliderule-3.6.0/utils/utils.py` & `sliderule-3.7.0/utils/utils.py`

 * *Files identical despite different names*

