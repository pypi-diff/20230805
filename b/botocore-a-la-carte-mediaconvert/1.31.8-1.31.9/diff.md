# Comparing `tmp/botocore-a-la-carte-mediaconvert-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-mediaconvert-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-mediaconvert-1.31.8.tar", last modified: Fri Jul 21 01:21:44 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-mediaconvert-1.31.9.tar", last modified: Sat Jul 22 01:20:46 2023, max compression
```

## Comparing `botocore-a-la-carte-mediaconvert-1.31.8.tar` & `botocore-a-la-carte-mediaconvert-1.31.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:44.000000 botocore-a-la-carte-mediaconvert-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/
--rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-07-21 01:21:06.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-21 01:21:06.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   938183 2023-07-21 01:21:06.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/botocore_a_la_carte_mediaconvert.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-21 01:21:44.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore_a_la_carte_mediaconvert.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-21 01:21:44.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore_a_la_carte_mediaconvert.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:44.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore_a_la_carte_mediaconvert.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:44.000000 botocore-a-la-carte-mediaconvert-1.31.8/botocore_a_la_carte_mediaconvert.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:44.747362 botocore-a-la-carte-mediaconvert-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-21 01:21:44.000000 botocore-a-la-carte-mediaconvert-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:45.000000 botocore-a-la-carte-mediaconvert-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/
+-rw-r--r--   0 runner    (1001) docker     (123)    20785 2023-07-22 01:20:09.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-22 01:20:09.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   937533 2023-07-22 01:20:09.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/botocore_a_la_carte_mediaconvert.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-07-22 01:20:46.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore_a_la_carte_mediaconvert.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-22 01:20:46.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore_a_la_carte_mediaconvert.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:46.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore_a_la_carte_mediaconvert.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:46.000000 botocore-a-la-carte-mediaconvert-1.31.9/botocore_a_la_carte_mediaconvert.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:46.177245 botocore-a-la-carte-mediaconvert-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-22 01:20:45.000000 botocore-a-la-carte-mediaconvert-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/LICENSE.txt` & `botocore-a-la-carte-mediaconvert-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/PKG-INFO` & `botocore-a-la-carte-mediaconvert-1.31.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-mediaconvert
-Version: 1.31.8
+Version: 1.31.9
 Summary: mediaconvert data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/endpoint-rule-set-1.json` & `botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/paginators-1.json` & `botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/botocore/data/mediaconvert/2017-08-29/service-2.json` & `botocore-a-la-carte-mediaconvert-1.31.9/botocore/data/mediaconvert/2017-08-29/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999875201593513%*

 * *Differences: {"'shapes'": "{'HlsGroupSettings': {'members': {'SegmentsPerSubdirectory': {'documentation': "*

 * *             "'Specify the number of segments to write to a subdirectory before starting a new "*

 * *             'one. You  must also set Directory structure to Subdirectory per stream for this '*

 * *             "setting to have an effect.'}}}, 'ProresChromaSampling': {'documentation': 'This "*

 * *             'setting applies only to ProRes 4444 and ProRes 4444 XQ outputs that you create from '*

 * *             'inputs that us […]*

```diff
@@ -6905,15 +6905,15 @@
                 },
                 "SegmentLengthControl": {
                     "documentation": "Specify how you want MediaConvert to determine the segment length. Choose Exact (EXACT) to have the encoder use the exact length that you specify with the setting Segment length (SegmentLength). This might result in extra I-frames. Choose Multiple of GOP (GOP_MULTIPLE) to have the encoder round up the segment lengths to match the next GOP boundary.",
                     "locationName": "segmentLengthControl",
                     "shape": "HlsSegmentLengthControl"
                 },
                 "SegmentsPerSubdirectory": {
-                    "documentation": "Specify the number of segments to write to a subdirectory before starting a new one. You must also set Directory structure to Subdirectory per stream for this setting to have an effect.",
+                    "documentation": "Specify the number of segments to write to a subdirectory before starting a new one. You  must also set Directory structure to Subdirectory per stream for this setting to have an effect.",
                     "locationName": "segmentsPerSubdirectory",
                     "shape": "__integerMin1Max2147483647"
                 },
                 "StreamInfResolution": {
                     "documentation": "Include or exclude RESOLUTION attribute for video in EXT-X-STREAM-INF tag of variant manifest.",
                     "locationName": "streamInfResolution",
                     "shape": "HlsStreamInfResolution"
@@ -10601,15 +10601,15 @@
             "enum": [
                 "ON_DEMAND",
                 "RESERVED"
             ],
             "type": "string"
         },
         "ProresChromaSampling": {
-            "documentation": "This setting applies only to ProRes 4444 and ProRes 4444 XQ outputs that you create from inputs that use 4:4:4 chroma sampling. Set Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING) to allow outputs to also use 4:4:4 chroma sampling. You must specify a value for this setting when your output codec profile supports 4:4:4 chroma sampling. Related Settings: When you set Chroma sampling to Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING), you must choose an output codec profile that supports 4:4:4 chroma sampling. These values for Profile (CodecProfile) support 4:4:4 chroma sampling: Apple ProRes 4444 (APPLE_PRORES_4444) or Apple ProRes 4444 XQ (APPLE_PRORES_4444_XQ). When you set Chroma sampling to Preserve 4:4:4 sampling, you must disable all video preprocessors except for Nexguard file marker (PartnerWatermarking). When you set Chroma sampling to Preserve 4:4:4 sampling and use framerate conversion, you must set Frame rate conversion algorithm (FramerateConversionAlgorithm) to Drop duplicate (DUPLICATE_DROP).",
+            "documentation": "This setting applies only to ProRes 4444 and ProRes 4444 XQ outputs that you create from inputs that use 4:4:4 chroma sampling. Set Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING) to allow outputs to also use 4:4:4 chroma sampling. You must specify a value for this setting when your output codec profile supports 4:4:4 chroma sampling. Related Settings: For Apple ProRes outputs with 4:4:4 chroma sampling: Choose Preserve 4:4:4 sampling. Use when your input has 4:4:4 chroma sampling and your output codec Profile is Apple ProRes 4444 or 4444 XQ. Note that when you choose Preserve 4:4:4 sampling, you cannot include any of the following Preprocessors: Dolby Vision, HDR10+, or Noise reducer.",
             "enum": [
                 "PRESERVE_444_SAMPLING",
                 "SUBSAMPLE_TO_422"
             ],
             "type": "string"
         },
         "ProresCodecProfile": {
@@ -10668,15 +10668,15 @@
             ],
             "type": "string"
         },
         "ProresSettings": {
             "documentation": "Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value PRORES.",
             "members": {
                 "ChromaSampling": {
-                    "documentation": "This setting applies only to ProRes 4444 and ProRes 4444 XQ outputs that you create from inputs that use 4:4:4 chroma sampling. Set Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING) to allow outputs to also use 4:4:4 chroma sampling. You must specify a value for this setting when your output codec profile supports 4:4:4 chroma sampling. Related Settings: When you set Chroma sampling to Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING), you must choose an output codec profile that supports 4:4:4 chroma sampling. These values for Profile (CodecProfile) support 4:4:4 chroma sampling: Apple ProRes 4444 (APPLE_PRORES_4444) or Apple ProRes 4444 XQ (APPLE_PRORES_4444_XQ). When you set Chroma sampling to Preserve 4:4:4 sampling, you must disable all video preprocessors except for Nexguard file marker (PartnerWatermarking). When you set Chroma sampling to Preserve 4:4:4 sampling and use framerate conversion, you must set Frame rate conversion algorithm (FramerateConversionAlgorithm) to Drop duplicate (DUPLICATE_DROP).",
+                    "documentation": "This setting applies only to ProRes 4444 and ProRes 4444 XQ outputs that you create from inputs that use 4:4:4 chroma sampling. Set Preserve 4:4:4 sampling (PRESERVE_444_SAMPLING) to allow outputs to also use 4:4:4 chroma sampling. You must specify a value for this setting when your output codec profile supports 4:4:4 chroma sampling. Related Settings: For Apple ProRes outputs with 4:4:4 chroma sampling: Choose Preserve 4:4:4 sampling. Use when your input has 4:4:4 chroma sampling and your output codec Profile is Apple ProRes 4444 or 4444 XQ. Note that when you choose Preserve 4:4:4 sampling, you cannot include any of the following Preprocessors: Dolby Vision, HDR10+, or Noise reducer.",
                     "locationName": "chromaSampling",
                     "shape": "ProresChromaSampling"
                 },
                 "CodecProfile": {
                     "documentation": "Use Profile (ProResCodecProfile) to specify the type of Apple ProRes codec to use for this output.",
                     "locationName": "codecProfile",
                     "shape": "ProresCodecProfile"
@@ -11816,15 +11816,15 @@
                 },
                 "AvcIntraSettings": {
                     "documentation": "Required when you choose AVC-Intra for your output video codec. For more information about the AVC-Intra settings, see the relevant specification. For detailed information about SD and HD in AVC-Intra, see https://ieeexplore.ieee.org/document/7290936. For information about 4K/2K in AVC-Intra, see https://pro-av.panasonic.net/en/avc-ultra/AVC-ULTRAoverview.pdf.",
                     "locationName": "avcIntraSettings",
                     "shape": "AvcIntraSettings"
                 },
                 "Codec": {
-                    "documentation": "Specifies the video codec. This must be equal to one of the enum values defined by the object VideoCodec. To passthrough the video stream of your input JPEG2000, VC-3, AVC-INTRA or Apple ProRes video without any video encoding: Choose Passthrough. If you have multiple input videos, note that they must have identical encoding attributes. When you choose Passthrough, your output container must be MXF or QuickTime MOV.",
+                    "documentation": "Specifies the video codec. This must be equal to one of the enum values defined by the object VideoCodec. To passthrough the video stream of your input JPEG2000, VC-3, AVC-INTRA or Apple ProRes  video without any video encoding: Choose Passthrough. If you have multiple input videos, note that they must have identical encoding attributes. When you choose Passthrough, your output container must be MXF or QuickTime MOV.",
                     "locationName": "codec",
                     "shape": "VideoCodec"
                 },
                 "FrameCaptureSettings": {
                     "documentation": "Required when you set (Codec) under (VideoDescription)>(CodecSettings) to the value FRAME_CAPTURE.",
                     "locationName": "frameCaptureSettings",
                     "shape": "FrameCaptureSettings"
```

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/botocore_a_la_carte_mediaconvert.egg-info/PKG-INFO` & `botocore-a-la-carte-mediaconvert-1.31.9/botocore_a_la_carte_mediaconvert.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-mediaconvert
-Version: 1.31.8
+Version: 1.31.9
 Summary: mediaconvert data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-mediaconvert-1.31.8/setup.py` & `botocore-a-la-carte-mediaconvert-1.31.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-mediaconvert',
-    version="1.31.8",
+    version="1.31.9",
     description='mediaconvert data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/mediaconvert/*/*.json'],
```

