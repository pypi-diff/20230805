# Comparing `tmp/opennsfw2-0.9.1.tar.gz` & `tmp/opennsfw2-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opennsfw2-0.9.1.tar", last modified: Sat May 21 01:54:32 2022, max compression
+gzip compressed data, was "opennsfw2-0.9.2.tar", last modified: Sat May 21 02:04:54 2022, max compression
```

## Comparing `opennsfw2-0.9.1.tar` & `opennsfw2-0.9.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 byung     (1000) byung     (1000)        0 2022-05-21 01:54:32.869765 opennsfw2-0.9.1/
--rw-rw-r--   0 byung     (1000) byung     (1000)     1067 2021-11-01 10:54:10.000000 opennsfw2-0.9.1/LICENSE
--rw-rw-r--   0 byung     (1000) byung     (1000)    11675 2022-05-21 01:54:32.869765 opennsfw2-0.9.1/PKG-INFO
--rw-r--r--   0 byung     (1000) byung     (1000)    11210 2022-05-21 01:53:38.000000 opennsfw2-0.9.1/README.md
-drwxrwxr-x   0 byung     (1000) byung     (1000)        0 2022-05-21 01:54:32.868765 opennsfw2-0.9.1/opennsfw2/
--rw-r--r--   0 byung     (1000) byung     (1000)      558 2022-05-21 01:54:18.000000 opennsfw2-0.9.1/opennsfw2/__init__.py
--rw-r--r--   0 byung     (1000) byung     (1000)      727 2022-05-04 13:08:25.000000 opennsfw2-0.9.1/opennsfw2/_download.py
--rw-r--r--   0 byung     (1000) byung     (1000)     1660 2022-05-04 13:08:25.000000 opennsfw2-0.9.1/opennsfw2/_image.py
--rw-r--r--   0 byung     (1000) byung     (1000)     6370 2022-05-21 01:53:38.000000 opennsfw2-0.9.1/opennsfw2/_inference.py
--rw-r--r--   0 byung     (1000) byung     (1000)     3757 2022-05-04 13:08:36.000000 opennsfw2-0.9.1/opennsfw2/_inspection.py
--rw-r--r--   0 byung     (1000) byung     (1000)     6687 2022-05-04 13:08:25.000000 opennsfw2-0.9.1/opennsfw2/_model.py
--rw-r--r--   0 byung     (1000) byung     (1000)      156 2022-05-04 13:08:25.000000 opennsfw2-0.9.1/opennsfw2/_typing.py
--rw-r--r--   0 byung     (1000) byung     (1000)        0 2021-06-17 08:22:19.000000 opennsfw2-0.9.1/opennsfw2/py.typed
-drwxrwxr-x   0 byung     (1000) byung     (1000)        0 2022-05-21 01:54:32.869765 opennsfw2-0.9.1/opennsfw2.egg-info/
--rw-rw-r--   0 byung     (1000) byung     (1000)    11675 2022-05-21 01:54:32.000000 opennsfw2-0.9.1/opennsfw2.egg-info/PKG-INFO
--rw-rw-r--   0 byung     (1000) byung     (1000)      380 2022-05-21 01:54:32.000000 opennsfw2-0.9.1/opennsfw2.egg-info/SOURCES.txt
--rw-rw-r--   0 byung     (1000) byung     (1000)        1 2022-05-21 01:54:32.000000 opennsfw2-0.9.1/opennsfw2.egg-info/dependency_links.txt
--rw-rw-r--   0 byung     (1000) byung     (1000)      132 2022-05-21 01:54:32.000000 opennsfw2-0.9.1/opennsfw2.egg-info/requires.txt
--rw-rw-r--   0 byung     (1000) byung     (1000)       10 2022-05-21 01:54:32.000000 opennsfw2-0.9.1/opennsfw2.egg-info/top_level.txt
--rw-r--r--   0 byung     (1000) byung     (1000)      103 2021-07-17 01:19:59.000000 opennsfw2-0.9.1/pyproject.toml
--rw-r--r--   0 byung     (1000) byung     (1000)      753 2022-05-21 01:54:32.869765 opennsfw2-0.9.1/setup.cfg
+drwxrwxr-x   0 byung     (1000) byung     (1000)        0 2022-05-21 02:04:54.342318 opennsfw2-0.9.2/
+-rw-rw-r--   0 byung     (1000) byung     (1000)     1067 2021-11-01 10:54:10.000000 opennsfw2-0.9.2/LICENSE
+-rw-rw-r--   0 byung     (1000) byung     (1000)    11675 2022-05-21 02:04:54.342318 opennsfw2-0.9.2/PKG-INFO
+-rw-r--r--   0 byung     (1000) byung     (1000)    11210 2022-05-21 01:53:38.000000 opennsfw2-0.9.2/README.md
+drwxrwxr-x   0 byung     (1000) byung     (1000)        0 2022-05-21 02:04:54.342318 opennsfw2-0.9.2/opennsfw2/
+-rw-r--r--   0 byung     (1000) byung     (1000)      558 2022-05-21 02:04:00.000000 opennsfw2-0.9.2/opennsfw2/__init__.py
+-rw-r--r--   0 byung     (1000) byung     (1000)      727 2022-05-04 13:08:25.000000 opennsfw2-0.9.2/opennsfw2/_download.py
+-rw-r--r--   0 byung     (1000) byung     (1000)     1660 2022-05-04 13:08:25.000000 opennsfw2-0.9.2/opennsfw2/_image.py
+-rw-r--r--   0 byung     (1000) byung     (1000)     6415 2022-05-21 02:01:44.000000 opennsfw2-0.9.2/opennsfw2/_inference.py
+-rw-r--r--   0 byung     (1000) byung     (1000)     3757 2022-05-04 13:08:36.000000 opennsfw2-0.9.2/opennsfw2/_inspection.py
+-rw-r--r--   0 byung     (1000) byung     (1000)     6687 2022-05-04 13:08:25.000000 opennsfw2-0.9.2/opennsfw2/_model.py
+-rw-r--r--   0 byung     (1000) byung     (1000)      156 2022-05-04 13:08:25.000000 opennsfw2-0.9.2/opennsfw2/_typing.py
+-rw-r--r--   0 byung     (1000) byung     (1000)        0 2021-06-17 08:22:19.000000 opennsfw2-0.9.2/opennsfw2/py.typed
+drwxrwxr-x   0 byung     (1000) byung     (1000)        0 2022-05-21 02:04:54.342318 opennsfw2-0.9.2/opennsfw2.egg-info/
+-rw-rw-r--   0 byung     (1000) byung     (1000)    11675 2022-05-21 02:04:53.000000 opennsfw2-0.9.2/opennsfw2.egg-info/PKG-INFO
+-rw-rw-r--   0 byung     (1000) byung     (1000)      380 2022-05-21 02:04:54.000000 opennsfw2-0.9.2/opennsfw2.egg-info/SOURCES.txt
+-rw-rw-r--   0 byung     (1000) byung     (1000)        1 2022-05-21 02:04:54.000000 opennsfw2-0.9.2/opennsfw2.egg-info/dependency_links.txt
+-rw-rw-r--   0 byung     (1000) byung     (1000)      132 2022-05-21 02:04:54.000000 opennsfw2-0.9.2/opennsfw2.egg-info/requires.txt
+-rw-rw-r--   0 byung     (1000) byung     (1000)       10 2022-05-21 02:04:54.000000 opennsfw2-0.9.2/opennsfw2.egg-info/top_level.txt
+-rw-r--r--   0 byung     (1000) byung     (1000)      103 2021-07-17 01:19:59.000000 opennsfw2-0.9.2/pyproject.toml
+-rw-r--r--   0 byung     (1000) byung     (1000)      753 2022-05-21 02:04:54.343319 opennsfw2-0.9.2/setup.cfg
```

### Comparing `opennsfw2-0.9.1/LICENSE` & `opennsfw2-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opennsfw2-0.9.1/PKG-INFO` & `opennsfw2-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opennsfw2
-Version: 0.9.1
+Version: 0.9.2
 Summary: TensorFlow 2 implementation of the Yahoo Open-NSFW model
 Home-page: https://github.com/bhky/opennsfw2
 Author: attr: opennsfw2.__author__
 Author-email: xtorch501@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opennsfw2-0.9.1/README.md` & `opennsfw2-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `opennsfw2-0.9.1/opennsfw2/__init__.py` & `opennsfw2-0.9.2/opennsfw2/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,10 +3,10 @@
 from ._image import preprocess_image as preprocess_image
 from ._inference import Aggregation
 from ._inference import predict_image as predict_image
 from ._inference import predict_images as predict_images
 from ._inference import predict_video_frames as predict_video_frames
 from ._model import make_open_nsfw_model as make_open_nsfw_model
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __author__ = "Bosco Yung"
 __license__ = "MIT"
```

### Comparing `opennsfw2-0.9.1/opennsfw2/_download.py` & `opennsfw2-0.9.2/opennsfw2/_download.py`

 * *Files identical despite different names*

### Comparing `opennsfw2-0.9.1/opennsfw2/_image.py` & `opennsfw2-0.9.2/opennsfw2/_image.py`

 * *Files identical despite different names*

### Comparing `opennsfw2-0.9.1/opennsfw2/_inference.py` & `opennsfw2-0.9.2/opennsfw2/_inference.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 from enum import auto, Enum
 from typing import Any, Callable, List, Optional, Sequence, Tuple
 
 import cv2  # type: ignore
 import numpy as np
 from PIL import Image  # type: ignore
-from tqdm import tqdm
+from tqdm import tqdm  # type: ignore
 
 from ._download import get_default_weights_path
 from ._image import preprocess_image, Preprocessing
 from ._inspection import make_and_save_nsfw_grad_cam
 from ._model import make_open_nsfw_model
 from ._typing import NDFloat32Array
 
@@ -122,15 +122,15 @@
     video_writer: Optional[cv2.VideoWriter] = None  # pylint: disable=no-member
     input_frames: List[NDFloat32Array] = []
     nsfw_probability = 0.0
     nsfw_probabilities: List[float] = []
     frame_count = 0
 
     if progress_bar:
-        pbar = tqdm(total=int(cap.get(cv2.CAP_PROP_FRAME_COUNT)))
+        pbar = tqdm(total=int(cap.get(cv2.CAP_PROP_FRAME_COUNT)))  # pylint: disable=no-member
     else:
         pbar = None
 
     while cap.isOpened():
         ret, bgr_frame = cap.read()  # Get next video frame.
         if not ret:
             break  # End of given video.
```

### Comparing `opennsfw2-0.9.1/opennsfw2/_inspection.py` & `opennsfw2-0.9.2/opennsfw2/_inspection.py`

 * *Files identical despite different names*

### Comparing `opennsfw2-0.9.1/opennsfw2/_model.py` & `opennsfw2-0.9.2/opennsfw2/_model.py`

 * *Files identical despite different names*

### Comparing `opennsfw2-0.9.1/opennsfw2.egg-info/PKG-INFO` & `opennsfw2-0.9.2/opennsfw2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opennsfw2
-Version: 0.9.1
+Version: 0.9.2
 Summary: TensorFlow 2 implementation of the Yahoo Open-NSFW model
 Home-page: https://github.com/bhky/opennsfw2
 Author: attr: opennsfw2.__author__
 Author-email: xtorch501@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `opennsfw2-0.9.1/setup.cfg` & `opennsfw2-0.9.2/setup.cfg`

 * *Files identical despite different names*

