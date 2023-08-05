# Comparing `tmp/plot2vid-1.0.1.tar.gz` & `tmp/plot2vid-1.0.2.tar.gz`

## Comparing `plot2vid-1.0.1.tar` & `plot2vid-1.0.2.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 plot2vid-1.0.1/src/plot2vid/__init__.py
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 plot2vid-1.0.1/src/plot2vid/recorder.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 plot2vid-1.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plot2vid-1.0.1/LICENSE
--rw-r--r--   0        0        0      799 2020-02-02 00:00:00.000000 plot2vid-1.0.1/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 plot2vid-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1348 2020-02-02 00:00:00.000000 plot2vid-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1419 2020-02-02 00:00:00.000000 plot2vid-1.0.2/src/plot2vid/__init__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 plot2vid-1.0.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plot2vid-1.0.2/LICENSE
+-rw-r--r--   0        0        0      831 2020-02-02 00:00:00.000000 plot2vid-1.0.2/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 plot2vid-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1380 2020-02-02 00:00:00.000000 plot2vid-1.0.2/PKG-INFO
```

### Comparing `plot2vid-1.0.1/src/plot2vid/recorder.py` & `plot2vid-1.0.2/src/plot2vid/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.backends.backend_agg import FigureCanvasAgg
 import cv2
 import numpy as np
 import math
 
+__version__ = "1.0.2"
+
 
 class PlotRecorder():
     def __init__(self, destination: str, fps=30):
         self.destination = destination
         self.fps = fps
 
         self.writer = None
```

### Comparing `plot2vid-1.0.1/README.md` & `plot2vid-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 pip install plot2vid
 ```
 
 ## Basic Usage
 
 ```python
 from plot2vid import plot2vid
+import matplotlib.pyplot as plt
 
 # Setup
 recorder = plot2vid.PlotRecorder("out.mp4")
 fig = plt.figure()
 
 for i in range(90):
     # Setting the plot limits
```

### Comparing `plot2vid-1.0.1/pyproject.toml` & `plot2vid-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "plot2vid"
-version = "1.0.1"
+version = "1.0.2"
 description = "The easiest way to create animations using plots."
 readme = "README.md"
 authors = [{ name = "Franciszek Szewczyk", email = "szewczyk.franciszek02@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
```

### Comparing `plot2vid-1.0.1/PKG-INFO` & `plot2vid-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plot2vid
-Version: 1.0.1
+Version: 1.0.2
 Summary: The easiest way to create animations using plots.
 Project-URL: Homepage, https://github.com/fszewczyk/plot2vid
 Author-email: Franciszek Szewczyk <szewczyk.franciszek02@gmail.com>
 License-File: LICENSE
 Keywords: animation,plot,video
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -26,14 +26,15 @@
 pip install plot2vid
 ```
 
 ## Basic Usage
 
 ```python
 from plot2vid import plot2vid
+import matplotlib.pyplot as plt
 
 # Setup
 recorder = plot2vid.PlotRecorder("out.mp4")
 fig = plt.figure()
 
 for i in range(90):
     # Setting the plot limits
```

