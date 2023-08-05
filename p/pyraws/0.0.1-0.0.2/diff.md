# Comparing `tmp/pyraws-0.0.1-py3-none-any.whl.zip` & `tmp/pyraws-0.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 50649 bytes, number of entries: 20
+Zip file size: 50646 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     2237 b- defN 23-Jul-04 17:51 pyraws/__init__.py
 -rw-r--r--  2.0 unx      116 b- defN 23-Aug-02 08:45 pyraws/sys_cfg.py
 -rw-r--r--  2.0 unx    19727 b- defN 23-Jul-04 17:51 pyraws/l1/l1_event.py
 -rw-r--r--  2.0 unx    15879 b- defN 23-Jul-04 17:51 pyraws/l1/l1_tile.py
 -rw-r--r--  2.0 unx    21386 b- defN 23-Jul-04 17:51 pyraws/raw/raw_event.py
 -rw-r--r--  2.0 unx    66121 b- defN 23-Aug-05 18:33 pyraws/raw/raw_granule.py
 -rw-r--r--  2.0 unx     5073 b- defN 23-Jul-04 17:51 pyraws/utils/band_shape_utils.py
@@ -10,13 +10,13 @@
 -rw-r--r--  2.0 unx    19025 b- defN 23-Jul-04 17:51 pyraws/utils/database_utils.py
 -rw-r--r--  2.0 unx      927 b- defN 23-Jul-04 17:51 pyraws/utils/date_utils.py
 -rw-r--r--  2.0 unx    21747 b- defN 23-Jul-04 17:51 pyraws/utils/l1_utils.py
 -rw-r--r--  2.0 unx      486 b- defN 23-Jul-04 17:51 pyraws/utils/parse_csv_utils.py
 -rw-r--r--  2.0 unx    15891 b- defN 23-Jul-04 17:51 pyraws/utils/raw_utils.py
 -rw-r--r--  2.0 unx     4140 b- defN 23-Jul-04 17:51 pyraws/utils/shape_utils.py
 -rw-r--r--  2.0 unx     4704 b- defN 23-Aug-05 18:33 pyraws/utils/visualization_utils.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Aug-05 21:18 pyraws-0.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     5405 b- defN 23-Aug-05 21:18 pyraws-0.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 21:18 pyraws-0.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Aug-05 21:18 pyraws-0.0.1.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1619 b- defN 23-Aug-05 21:18 pyraws-0.0.1.dist-info/RECORD
-20 files, 218693 bytes uncompressed, 48041 bytes compressed:  78.0%
+-rw-r--r--  2.0 unx    11357 b- defN 23-Aug-05 21:21 pyraws-0.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     5399 b- defN 23-Aug-05 21:21 pyraws-0.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-05 21:21 pyraws-0.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-Aug-05 21:21 pyraws-0.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1619 b- defN 23-Aug-05 21:21 pyraws-0.0.2.dist-info/RECORD
+20 files, 218687 bytes uncompressed, 48038 bytes compressed:  78.0%
```

## zipnote {}

```diff
@@ -39,23 +39,23 @@
 
 Filename: pyraws/utils/shape_utils.py
 Comment: 
 
 Filename: pyraws/utils/visualization_utils.py
 Comment: 
 
-Filename: pyraws-0.0.1.dist-info/LICENSE
+Filename: pyraws-0.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: pyraws-0.0.1.dist-info/METADATA
+Filename: pyraws-0.0.2.dist-info/METADATA
 Comment: 
 
-Filename: pyraws-0.0.1.dist-info/WHEEL
+Filename: pyraws-0.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: pyraws-0.0.1.dist-info/top_level.txt
+Filename: pyraws-0.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: pyraws-0.0.1.dist-info/RECORD
+Filename: pyraws-0.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pyraws-0.0.1.dist-info/LICENSE` & `pyraws-0.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pyraws-0.0.1.dist-info/METADATA` & `pyraws-0.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyraws
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python for RAW Sentinel2 data (PyRawS) is a powerful open-source Python package that provides a comprehensive set of tools for working with Sentinel-2 Raw data. It provides utilities for coarse spatial bands coregistration, geo-referencing, data visualization, and image processing.
 Home-page: https://github.com/ESA-PhiLab/PyRawS
 Author: ESA Philab
 Author-email: gabriele.meoni@esa.int
 License: UNKNOWN
 Project-URL: Source, https://github.com/ESA-PhiLab/PyRawS
 Platform: UNKNOWN
@@ -40,15 +40,15 @@
 ![GitHub contributors](https://img.shields.io/github/contributors/ESA-PhiLab/PyRawS?style=flat-square)
 ![GitHub issues](https://img.shields.io/github/issues/ESA-PhiLab/PyRawS?style=flat-square)
 ![GitHub pull requests](https://img.shields.io/github/issues-pr/ESA-PhiLab/PyRawS?style=flat-square)
 [![Tests](https://github.com/ESA-PhiLab/PyRawS/actions/workflows/run_tests.yml/badge.svg)](https://github.com/ESA-PhiLab/PyRawS/actions/workflows/run_tests.yml)
 ![Python 3.8](https://img.shields.io/badge/python-3.8-blue.svg)
 ![Python 3.9](https://img.shields.io/badge/python-3.9-blue.svg)
 ![Python 3.10](https://img.shields.io/badge/python-3.10-blue.svg)
-[![PyPI](https://img.shields.io/pypi/v/pyraws.svg)](https://pypi.org/project/pyraws/0.0.0/)
+[![PyPI](https://img.shields.io/pypi/v/pyraws.svg)](https://pypi.org/project/pyraws/)
 # PyRawS
 [![Py-Raw-S-logo.png](https://i.postimg.cc/7Yptgf5y/Py-Raw-S-logo.png)](https://postimg.cc/vctvy87P)
 ## About the project
 `Python for RAW Sentinel2 data (PyRawS)` is a powerful open-source Python package that provides a comprehensive set of tools for working with [Sentinel-2 Raw data](#sentinel-2-raw-data).
 <sup id="fnref:1"><a href="#fn:1" class="footnote">1</a></sup>
 It provides utilities for coarse spatial bands coregistration, geo-referencing, data visualization, and image processing.
 The software is demonstrated on the first Sentinel-2 Raw database for warm temperature hotspots detection/classification, making it an ideal tool for a wide range of applications in remote sensing and earth observation.
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyraws Version: 0.0.1 Summary: Python for RAW
+Metadata-Version: 2.1 Name: pyraws Version: 0.0.2 Summary: Python for RAW
 Sentinel2 data (PyRawS) is a powerful open-source Python package that provides
 a comprehensive set of tools for working with Sentinel-2 Raw data. It provides
 utilities for coarse spatial bands coregistration, geo-referencing, data
 visualization, and image processing. Home-page: https://github.com/ESA-PhiLab/
 PyRawS Author: ESA Philab Author-email: gabriele.meoni@esa.int License: UNKNOWN
 Project-URL: Source, https://github.com/ESA-PhiLab/PyRawS Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
@@ -25,36 +25,36 @@
 PyRawS?style=flat-square) ![GitHub pull requests](https://img.shields.io/
 github/issues-pr/ESA-PhiLab/PyRawS?style=flat-square) [![Tests](https://
 github.com/ESA-PhiLab/PyRawS/actions/workflows/run_tests.yml/badge.svg)](https:
 //github.com/ESA-PhiLab/PyRawS/actions/workflows/run_tests.yml) ![Python 3.8]
 (https://img.shields.io/badge/python-3.8-blue.svg) ![Python 3.9](https://
 img.shields.io/badge/python-3.9-blue.svg) ![Python 3.10](https://
 img.shields.io/badge/python-3.10-blue.svg) [![PyPI](https://img.shields.io/
-pypi/v/pyraws.svg)](https://pypi.org/project/pyraws/0.0.0/) # PyRawS [![Py-Raw-
-S-logo.png](https://i.postimg.cc/7Yptgf5y/Py-Raw-S-logo.png)](https://
-postimg.cc/vctvy87P) ## About the project `Python for RAW Sentinel2 data
-(PyRawS)` is a powerful open-source Python package that provides a
-comprehensive set of tools for working with [Sentinel-2 Raw data](#sentinel-2-
-raw-data). 1 It provides utilities for coarse spatial bands coregistration,
-geo-referencing, data visualization, and image processing. The software is
-demonstrated on the first Sentinel-2 Raw database for warm temperature hotspots
-detection/classification, making it an ideal tool for a wide range of
-applications in remote sensing and earth observation. The package is written in
-Python and is open source, making it easy to use and modify for your specific
-needs. The systme is based on [pytorch]("https://pytorch.org/"), which be
-installed with `CUDA 11` support, to enable GPU acceleation. TEST 2 NB: What we
-call raw data in this project are Sentinel-2 data generated by the
-decompression and metadata addition of Sentinel-2 L0 data. Because of that,
-with the exception of the effects due to onboard equalization and lossy
-compression, they are the most similar version of the rawest form of data
-acquired by the satellite's sensors. Both the compression and equalization are
-applied onboard the satellite to reduce the amount of data transmitted to the
-ground station. For easy naming convention, this repo refer to the term "Raw"
-as the products decompressed with ancillary information appended. For further
-information browse our paper at https://arxiv.org/abs/2305.11891 ↩
+pypi/v/pyraws.svg)](https://pypi.org/project/pyraws/) # PyRawS [![Py-Raw-S-
+logo.png](https://i.postimg.cc/7Yptgf5y/Py-Raw-S-logo.png)](https://postimg.cc/
+vctvy87P) ## About the project `Python for RAW Sentinel2 data (PyRawS)` is a
+powerful open-source Python package that provides a comprehensive set of tools
+for working with [Sentinel-2 Raw data](#sentinel-2-raw-data). 1 It provides
+utilities for coarse spatial bands coregistration, geo-referencing, data
+visualization, and image processing. The software is demonstrated on the first
+Sentinel-2 Raw database for warm temperature hotspots detection/classification,
+making it an ideal tool for a wide range of applications in remote sensing and
+earth observation. The package is written in Python and is open source, making
+it easy to use and modify for your specific needs. The systme is based on
+[pytorch]("https://pytorch.org/"), which be installed with `CUDA 11` support,
+to enable GPU acceleation. TEST 2 NB: What we call raw data in this project are
+Sentinel-2 data generated by the decompression and metadata addition of
+Sentinel-2 L0 data. Because of that, with the exception of the effects due to
+onboard equalization and lossy compression, they are the most similar version
+of the rawest form of data acquired by the satellite's sensors. Both the
+compression and equalization are applied onboard the satellite to reduce the
+amount of data transmitted to the ground station. For easy naming convention,
+this repo refer to the term "Raw" as the products decompressed with ancillary
+information appended. For further information browse our paper at https://
+arxiv.org/abs/2305.11891 ↩
 *(Disclaimer: This project is currently under development.)* ## Contributing
 The ```PyRawS``` project is open to contributions. To discuss new ideas and
 applications, please, reach us via email (please, refer to [Contacts]
 (#contacts)). To report a bug or request a new feature, please, open an [issue]
 (https://github.com/ESA-PhiLab/PyRawS/issues) to report a bug or to request a
 new feature. If you want to contribute, please proceed as follow: 1. Fork the
 Project 2. Create your Feature Branch (`git checkout -b feature/NewFeature`) 3.
```

## Comparing `pyraws-0.0.1.dist-info/RECORD` & `pyraws-0.0.2.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -9,12 +9,12 @@
 pyraws/utils/database_utils.py,sha256=QveN0yq5cMptofvqXhVIcFCM3UbcC5e_GganJ3rqLR0,19025
 pyraws/utils/date_utils.py,sha256=UmLH7rqALIJZ-W440SwetZpmj5iRb0RaRrxHUTUg8os,927
 pyraws/utils/l1_utils.py,sha256=5JRYvmphvN4AzDhA8piZw1-iZBYyTbw8771bx9B4p0o,21747
 pyraws/utils/parse_csv_utils.py,sha256=T7zefx1a-bLUruWdQFYZZ0bMgNKV5i6DVHelCgE3Nkg,486
 pyraws/utils/raw_utils.py,sha256=GERJRrFEFpPHL54i2dVsbtxlZhFanTCHVEmHYc9KRvA,15891
 pyraws/utils/shape_utils.py,sha256=4_SD30AtWsimoSOvKM_ajHIYSKynxLnmohBvyXP-KAI,4140
 pyraws/utils/visualization_utils.py,sha256=cm-oLsJoiIHWngSnGuYr29gG9YqspABy80C9LOOJsYY,4704
-pyraws-0.0.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-pyraws-0.0.1.dist-info/METADATA,sha256=kpHmwwYWhVkfHff2tILT-P75Lr7ho5zICySK0iTIF7U,5405
-pyraws-0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pyraws-0.0.1.dist-info/top_level.txt,sha256=vfx_AOvbbRQoNagNFpsLhwWxZM5_exBOzuNBFJSTPiE,7
-pyraws-0.0.1.dist-info/RECORD,,
+pyraws-0.0.2.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+pyraws-0.0.2.dist-info/METADATA,sha256=SqBtfVR9TmVreJmBbidTEPbB31dTbfjY0AQlKLx5yTk,5399
+pyraws-0.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pyraws-0.0.2.dist-info/top_level.txt,sha256=vfx_AOvbbRQoNagNFpsLhwWxZM5_exBOzuNBFJSTPiE,7
+pyraws-0.0.2.dist-info/RECORD,,
```

