# Comparing `tmp/audiostream2py-0.1.8.tar.gz` & `tmp/audiostream2py-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audiostream2py-0.1.8.tar", last modified: Fri Dec 10 01:41:42 2021, max compression
+gzip compressed data, was "audiostream2py-0.1.9.tar", last modified: Mon Dec 20 22:02:53 2021, max compression
```

## Comparing `audiostream2py-0.1.8.tar` & `audiostream2py-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 01:41:42.475212 audiostream2py-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-10 01:41:19.000000 audiostream2py-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      397 2021-12-10 01:41:42.475212 audiostream2py-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)       95 2021-12-10 01:41:19.000000 audiostream2py-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 01:41:42.475212 audiostream2py-0.1.8/audiostream2py/
--rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-10 01:41:19.000000 audiostream2py-0.1.8/audiostream2py/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    28688 2021-12-10 01:41:19.000000 audiostream2py-0.1.8/audiostream2py/audio.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 01:41:42.475212 audiostream2py-0.1.8/audiostream2py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2021-12-10 01:41:42.000000 audiostream2py-0.1.8/audiostream2py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      313 2021-12-10 01:41:42.000000 audiostream2py-0.1.8/audiostream2py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 01:41:42.000000 audiostream2py-0.1.8/audiostream2py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 01:41:42.000000 audiostream2py-0.1.8/audiostream2py.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-10 01:41:42.000000 audiostream2py-0.1.8/audiostream2py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-10 01:41:42.000000 audiostream2py-0.1.8/audiostream2py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      536 2021-12-10 01:41:42.479212 audiostream2py-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-10 01:41:19.000000 audiostream2py-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 22:02:53.572411 audiostream2py-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2021-12-20 22:02:30.000000 audiostream2py-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2021-12-20 22:02:53.572411 audiostream2py-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       95 2021-12-20 22:02:30.000000 audiostream2py-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 22:02:53.572411 audiostream2py-0.1.9/audiostream2py/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2021-12-20 22:02:30.000000 audiostream2py-0.1.9/audiostream2py/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28755 2021-12-20 22:02:30.000000 audiostream2py-0.1.9/audiostream2py/audio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-20 22:02:53.572411 audiostream2py-0.1.9/audiostream2py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2021-12-20 22:02:53.000000 audiostream2py-0.1.9/audiostream2py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      313 2021-12-20 22:02:53.000000 audiostream2py-0.1.9/audiostream2py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 22:02:53.000000 audiostream2py-0.1.9/audiostream2py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-20 22:02:53.000000 audiostream2py-0.1.9/audiostream2py.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-12-20 22:02:53.000000 audiostream2py-0.1.9/audiostream2py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-12-20 22:02:53.000000 audiostream2py-0.1.9/audiostream2py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2021-12-20 22:02:53.572411 audiostream2py-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-12-20 22:02:30.000000 audiostream2py-0.1.9/setup.py
```

### Comparing `audiostream2py-0.1.8/LICENSE` & `audiostream2py-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `audiostream2py-0.1.8/audiostream2py/audio.py` & `audiostream2py-0.1.9/audiostream2py/audio.py`

 * *Files 0% similar despite different names*

```diff
@@ -128,16 +128,19 @@
         )
     # If no information on the device is given, ask pyaudio to find a default
     elif input_device is None and input_device_index is None:
         info = PyAudioSourceReader.get_default_input_device_info()
         if verbose:
             import json
 
-            print(f"Will use {info['name']} (index={info['index']}) as an input device")
-            print(f"It's info:\n{json.dumps(info, indent=2)}")
+            print(
+                f"Will use {info['name']} (index={info['index']}) as an input device",
+                end='\r',
+            )
+            print(f"It's info:\n{json.dumps(info, indent=2)}", end='\r')
     else:
         input_device = input_device or input_device_index
         if isinstance(input_device, int):
             info = {'index': input_device}
         elif isinstance(input_device, Callable):
             info = match_device_info(filt=input_device)
         else:  # should be string or re.compile instance
```

### Comparing `audiostream2py-0.1.8/setup.cfg` & `audiostream2py-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = audiostream2py
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/i2mint/audiostream2py
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = apache-2.0
 author = OtoSense
 description = stream2py interface for audio
```

