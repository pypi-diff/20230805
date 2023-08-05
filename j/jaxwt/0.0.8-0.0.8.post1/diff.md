# Comparing `tmp/jaxwt-0.0.8.tar.gz` & `tmp/jaxwt-0.0.8.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jaxwt-0.0.8.tar", last modified: Mon Mar 20 13:47:37 2023, max compression
+gzip compressed data, was "jaxwt-0.0.8.post1.tar", last modified: Mon Mar 20 14:55:36 2023, max compression
```

## Comparing `jaxwt-0.0.8.tar` & `jaxwt-0.0.8.post1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 13:47:37.464663 jaxwt-0.0.8/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)    14014 2022-05-25 09:26:29.000000 jaxwt-0.0.8/LICENSE
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     5351 2023-03-20 13:47:37.464663 jaxwt-0.0.8/PKG-INFO
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     4235 2023-03-20 13:46:55.000000 jaxwt-0.0.8/README.rst
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1353 2023-03-20 13:47:37.464663 jaxwt-0.0.8/setup.cfg
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      115 2022-05-25 09:26:29.000000 jaxwt-0.0.8/setup.py
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 13:47:37.464663 jaxwt-0.0.8/src/
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 13:47:37.464663 jaxwt-0.0.8/src/jaxwt/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      267 2022-06-15 12:48:43.000000 jaxwt-0.0.8/src/jaxwt/__init__.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     5015 2022-10-26 15:29:13.000000 jaxwt-0.0.8/src/jaxwt/continuous_transform.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8392 2023-03-20 13:46:55.000000 jaxwt-0.0.8/src/jaxwt/conv_fwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     8486 2023-03-20 13:46:55.000000 jaxwt-0.0.8/src/jaxwt/conv_fwt_2d.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     7891 2023-03-20 13:46:55.000000 jaxwt-0.0.8/src/jaxwt/packets.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1784 2022-10-26 15:39:29.000000 jaxwt-0.0.8/src/jaxwt/utils.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      963 2023-03-20 13:47:35.000000 jaxwt-0.0.8/src/jaxwt/version.py
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 13:47:37.464663 jaxwt-0.0.8/src/jaxwt.egg-info/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     5351 2023-03-20 13:47:37.000000 jaxwt-0.0.8/src/jaxwt.egg-info/PKG-INFO
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      489 2023-03-20 13:47:37.000000 jaxwt-0.0.8/src/jaxwt.egg-info/SOURCES.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)        1 2023-03-20 13:47:37.000000 jaxwt-0.0.8/src/jaxwt.egg-info/dependency_links.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)       84 2023-03-20 13:47:37.000000 jaxwt-0.0.8/src/jaxwt.egg-info/requires.txt
--rw-rw-r--   0 wolter    (1000) wolter    (1000)        6 2023-03-20 13:47:37.000000 jaxwt-0.0.8/src/jaxwt.egg-info/top_level.txt
-drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 13:47:37.464663 jaxwt-0.0.8/tests/
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     2964 2023-03-20 13:46:55.000000 jaxwt-0.0.8/tests/test_conv_fwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1569 2023-03-20 13:46:55.000000 jaxwt-0.0.8/tests/test_conv_fwt2d.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1567 2022-06-10 16:59:25.000000 jaxwt-0.0.8/tests/test_cwt.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)      543 2022-05-25 09:26:29.000000 jaxwt-0.0.8/tests/test_jax.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     1970 2023-03-20 13:46:55.000000 jaxwt-0.0.8/tests/test_jit.py
--rw-rw-r--   0 wolter    (1000) wolter    (1000)     3934 2023-03-20 13:46:55.000000 jaxwt-0.0.8/tests/test_packets.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 14:55:36.803444 jaxwt-0.0.8.post1/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)    14014 2022-05-25 09:26:29.000000 jaxwt-0.0.8.post1/LICENSE
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     5353 2023-03-20 14:55:36.803444 jaxwt-0.0.8.post1/PKG-INFO
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     4231 2023-03-20 14:55:09.000000 jaxwt-0.0.8.post1/README.rst
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1359 2023-03-20 14:55:36.803444 jaxwt-0.0.8.post1/setup.cfg
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      115 2022-05-25 09:26:29.000000 jaxwt-0.0.8.post1/setup.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 14:55:36.799444 jaxwt-0.0.8.post1/src/
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 14:55:36.803444 jaxwt-0.0.8.post1/src/jaxwt/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      267 2022-06-15 12:48:43.000000 jaxwt-0.0.8.post1/src/jaxwt/__init__.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     5015 2022-10-26 15:29:13.000000 jaxwt-0.0.8.post1/src/jaxwt/continuous_transform.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8392 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/src/jaxwt/conv_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     8486 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/src/jaxwt/conv_fwt_2d.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     7891 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/src/jaxwt/packets.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1784 2022-10-26 15:39:29.000000 jaxwt-0.0.8.post1/src/jaxwt/utils.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      967 2023-03-20 13:48:01.000000 jaxwt-0.0.8.post1/src/jaxwt/version.py
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 14:55:36.803444 jaxwt-0.0.8.post1/src/jaxwt.egg-info/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     5353 2023-03-20 14:55:36.000000 jaxwt-0.0.8.post1/src/jaxwt.egg-info/PKG-INFO
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      489 2023-03-20 14:55:36.000000 jaxwt-0.0.8.post1/src/jaxwt.egg-info/SOURCES.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)        1 2023-03-20 14:55:36.000000 jaxwt-0.0.8.post1/src/jaxwt.egg-info/dependency_links.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)       84 2023-03-20 14:55:36.000000 jaxwt-0.0.8.post1/src/jaxwt.egg-info/requires.txt
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)        6 2023-03-20 14:55:36.000000 jaxwt-0.0.8.post1/src/jaxwt.egg-info/top_level.txt
+drwxrwxr-x   0 wolter    (1000) wolter    (1000)        0 2023-03-20 14:55:36.803444 jaxwt-0.0.8.post1/tests/
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     2964 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/tests/test_conv_fwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1569 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/tests/test_conv_fwt2d.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1567 2022-06-10 16:59:25.000000 jaxwt-0.0.8.post1/tests/test_cwt.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)      543 2022-05-25 09:26:29.000000 jaxwt-0.0.8.post1/tests/test_jax.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     1970 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/tests/test_jit.py
+-rw-rw-r--   0 wolter    (1000) wolter    (1000)     3934 2023-03-20 13:46:55.000000 jaxwt-0.0.8.post1/tests/test_packets.py
```

### Comparing `jaxwt-0.0.8/LICENSE` & `jaxwt-0.0.8.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/PKG-INFO` & `jaxwt-0.0.8.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxwt
-Version: 0.0.8
+Version: 0.0.8.post1
 Summary: Differentiable and gpu enabled fast wavelet transforms in JAX
 Home-page: https://github.com/v0lta/Jax-Wavelet-Toolbox
 Download-URL: https://github.com/v0lta/Jax-Wavelet-Toolbox/releases
 Author: Moritz Wolter
 Author-email: moritz@wolter.tech
 Maintainer: Moritz Wolter
 Maintainer-email: moritz@wolter.tech
@@ -61,15 +61,15 @@
 """"""""
 - 1d analysis and synthesis transforms are implemented in ``src/jaxwt/conv_fwt.py``.
 - 2d analysis and synthesis transform are part of the ``src/jaxwt/conv_fwt_2d.py`` module.
 - ``cwt``-function supports 1d continuous wavelet transforms.
 - The ``WaveletPacket`` object supports 1d wavelet packet transforms.
 - ``WaveletPacket2d`` implements two-dimensional wavelet packet transforms.
 
-This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a Jax backend.
 
 Installation
 """"""""""""
 To install Jax, head over to https://github.com/google/jax#installation and follow the procedure described there.
 Afterward, type ``pip install jaxwt`` to install the Jax-Wavelet-Toolbox. You can uninstall it later by typing ``pip uninstall jaxwt``.
 
 Documentation
```

### Comparing `jaxwt-0.0.8/README.rst` & `jaxwt-0.0.8.post1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 """"""""
 - 1d analysis and synthesis transforms are implemented in ``src/jaxwt/conv_fwt.py``.
 - 2d analysis and synthesis transform are part of the ``src/jaxwt/conv_fwt_2d.py`` module.
 - ``cwt``-function supports 1d continuous wavelet transforms.
 - The ``WaveletPacket`` object supports 1d wavelet packet transforms.
 - ``WaveletPacket2d`` implements two-dimensional wavelet packet transforms.
 
-This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a Jax backend.
 
 Installation
 """"""""""""
 To install Jax, head over to https://github.com/google/jax#installation and follow the procedure described there.
 Afterward, type ``pip install jaxwt`` to install the Jax-Wavelet-Toolbox. You can uninstall it later by typing ``pip uninstall jaxwt``.
 
 Documentation
```

### Comparing `jaxwt-0.0.8/setup.cfg` & `jaxwt-0.0.8.post1/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jaxwt
-version = 0.0.8
+version = 0.0.8.post1
 description = Differentiable and gpu enabled fast wavelet transforms in JAX
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/v0lta/Jax-Wavelet-Toolbox
 download_url = https://github.com/v0lta/Jax-Wavelet-Toolbox/releases
 project_urls = 
 	Bug Tracker = https://github.com/v0lta/Jax-Wavelet-Toolbox/issues
```

### Comparing `jaxwt-0.0.8/src/jaxwt/continuous_transform.py` & `jaxwt-0.0.8.post1/src/jaxwt/continuous_transform.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/src/jaxwt/conv_fwt.py` & `jaxwt-0.0.8.post1/src/jaxwt/conv_fwt.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/src/jaxwt/conv_fwt_2d.py` & `jaxwt-0.0.8.post1/src/jaxwt/conv_fwt_2d.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/src/jaxwt/packets.py` & `jaxwt-0.0.8.post1/src/jaxwt/packets.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/src/jaxwt/utils.py` & `jaxwt-0.0.8.post1/src/jaxwt/utils.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/src/jaxwt/version.py` & `jaxwt-0.0.8.post1/src/jaxwt/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 __all__ = [
     "VERSION",
     "get_version",
     "get_git_hash",
 ]
 
-VERSION = "0.0.8"
+VERSION = "0.0.9-dev"
 
 
 def get_git_hash() -> str:
     """Get the :mod:`jaxwt` git hash."""
     with open(os.devnull, "w") as devnull:
         try:
             ret = check_output(  # noqa: S603,S607
```

### Comparing `jaxwt-0.0.8/src/jaxwt.egg-info/PKG-INFO` & `jaxwt-0.0.8.post1/src/jaxwt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jaxwt
-Version: 0.0.8
+Version: 0.0.8.post1
 Summary: Differentiable and gpu enabled fast wavelet transforms in JAX
 Home-page: https://github.com/v0lta/Jax-Wavelet-Toolbox
 Download-URL: https://github.com/v0lta/Jax-Wavelet-Toolbox/releases
 Author: Moritz Wolter
 Author-email: moritz@wolter.tech
 Maintainer: Moritz Wolter
 Maintainer-email: moritz@wolter.tech
@@ -61,15 +61,15 @@
 """"""""
 - 1d analysis and synthesis transforms are implemented in ``src/jaxwt/conv_fwt.py``.
 - 2d analysis and synthesis transform are part of the ``src/jaxwt/conv_fwt_2d.py`` module.
 - ``cwt``-function supports 1d continuous wavelet transforms.
 - The ``WaveletPacket`` object supports 1d wavelet packet transforms.
 - ``WaveletPacket2d`` implements two-dimensional wavelet packet transforms.
 
-This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a PyTorch backend.
+This toolbox extends `PyWavelets <https://pywavelets.readthedocs.io/en/latest/>`_ . We additionally provide GPU and gradient support via a Jax backend.
 
 Installation
 """"""""""""
 To install Jax, head over to https://github.com/google/jax#installation and follow the procedure described there.
 Afterward, type ``pip install jaxwt`` to install the Jax-Wavelet-Toolbox. You can uninstall it later by typing ``pip uninstall jaxwt``.
 
 Documentation
```

### Comparing `jaxwt-0.0.8/tests/test_conv_fwt.py` & `jaxwt-0.0.8.post1/tests/test_conv_fwt.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/tests/test_conv_fwt2d.py` & `jaxwt-0.0.8.post1/tests/test_conv_fwt2d.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/tests/test_cwt.py` & `jaxwt-0.0.8.post1/tests/test_cwt.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/tests/test_jax.py` & `jaxwt-0.0.8.post1/tests/test_jax.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/tests/test_jit.py` & `jaxwt-0.0.8.post1/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `jaxwt-0.0.8/tests/test_packets.py` & `jaxwt-0.0.8.post1/tests/test_packets.py`

 * *Files identical despite different names*

