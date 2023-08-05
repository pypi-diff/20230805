# Comparing `tmp/audio_separator-0.6.2.tar.gz` & `tmp/audio_separator-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.6.2.tar", max compression
+gzip compressed data, was "audio_separator-0.6.3.tar", max compression
```

## Comparing `audio_separator-0.6.2.tar` & `audio_separator-0.6.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.6.2/LICENSE
--rw-r--r--   0        0        0     8757 2023-08-05 18:54:39.190288 audio_separator-0.6.2/README.md
--rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.6.2/audio_separator/__init__.py
--rw-r--r--   0        0        0    14146 2023-08-05 19:59:44.637012 audio_separator-0.6.2/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.6.2/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     3834 2023-08-05 19:57:04.949515 audio_separator-0.6.2/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-08-05 18:58:36.032370 audio_separator-0.6.2/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      985 2023-08-05 19:35:29.038158 audio_separator-0.6.2/pyproject.toml
--rw-r--r--   0        0        0     9817 1970-01-01 00:00:00.000000 audio_separator-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-05 20:23:27.543104 audio_separator-0.6.3/LICENSE
+-rw-r--r--   0        0        0     8757 2023-08-05 20:23:27.543104 audio_separator-0.6.3/README.md
+-rw-r--r--   0        0        0       33 2023-08-05 20:23:27.543104 audio_separator-0.6.3/audio_separator/__init__.py
+-rw-r--r--   0        0        0    14430 2023-08-05 20:23:27.543104 audio_separator-0.6.3/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-08-05 20:23:27.543104 audio_separator-0.6.3/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3795 2023-08-05 20:23:27.543104 audio_separator-0.6.3/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-08-05 20:23:27.543104 audio_separator-0.6.3/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      985 2023-08-05 20:23:27.543104 audio_separator-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0     9817 1970-01-01 00:00:00.000000 audio_separator-0.6.3/PKG-INFO
```

### Comparing `audio_separator-0.6.2/LICENSE` & `audio_separator-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.6.2/README.md` & `audio_separator-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `audio_separator-0.6.2/audio_separator/separator.py` & `audio_separator-0.6.3/audio_separator/separator.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,17 @@
         else:
             self.logger.debug(
                 f"Denoising disabled, model will only be run once. This is twice as fast, but may result in noisier output audio."
             )
 
         self.output_single_stem = output_single_stem
         if output_single_stem is not None:
-            self.logger.debug(f"Single stem output requested, only one output file will be written: {output_single_stem}")
+            if output_single_stem.lower() not in {"instrumental", "vocals"}:
+                raise Exception("output_single_stem must be either 'instrumental' or 'vocals'")
+            self.logger.debug(f"Single stem output requested, only one output file ({output_single_stem}) will be written")
 
         self.chunks = 0
         self.margin = 44100
         self.adjust = 1
         self.dim_c = 4
         self.hop = 1024
 
@@ -166,23 +168,23 @@
         mdx_net_cut = True
         mix, raw_mix, samplerate = prepare_mix(self.audio_file_path, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
         self.logger.info("Demixing...")
         source = self.demix_base(mix)[0]
 
         output_files = []
 
-        if self.output_single_stem != "secondary":
+        if not self.output_single_stem or self.output_single_stem.lower() == self.primary_stem.lower():
             self.logger.info(f"Saving {self.primary_stem} stem...")
             primary_stem_path = os.path.join(f"{self.audio_file_base}_({self.primary_stem})_{self.model_name}.{self.output_format.lower()}")
             if not isinstance(self.primary_source, np.ndarray):
                 self.primary_source = spec_utils.normalize(self.logger, source, self.normalization_enabled).T
             self.write_audio(primary_stem_path, self.primary_source, samplerate)
             output_files.append(primary_stem_path)
 
-        if self.output_single_stem != "primary":
+        if not self.output_single_stem or self.output_single_stem.lower() == self.secondary_stem.lower():
             self.logger.info(f"Saving {self.secondary_stem} stem...")
             secondary_stem_path = os.path.join(
                 f"{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.{self.output_format.lower()}"
             )
             if not isinstance(self.secondary_source, np.ndarray):
                 raw_mix = self.demix_base(raw_mix, is_match_mix=True)[0] if mdx_net_cut else raw_mix
                 self.secondary_source, raw_mix = spec_utils.normalize_two_stem(
```

### Comparing `audio_separator-0.6.2/audio_separator/utils/cli.py` & `audio_separator-0.6.3/audio_separator/utils/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         default=True,
         help="Optional: enable or disable normalization during separation (default: %(default)s). Example: --normalize=False",
     )
 
     parser.add_argument(
         "--single_stem",
         default=None,
-        help="Optional: output only single stem, primary or secondary. With the default model, primary is the instrumental. Example: --single_stem=primary",
+        help="Optional: output only single stem, either instrumental or vocals. Example: --single_stem=instrumental",
     )
 
     args = parser.parse_args()
 
     log_level = getattr(logging, args.log_level.upper())
     logger.setLevel(log_level)
```

### Comparing `audio_separator-0.6.2/audio_separator/utils/spec_utils.py` & `audio_separator-0.6.3/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.6.2/pyproject.toml` & `audio_separator-0.6.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.6.2"
+version = "0.6.3"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 homepage = "https://github.com/karaokenerds/python-audio-separator"
 repository = "https://github.com/karaokenerds/python-audio-separator"
```

### Comparing `audio_separator-0.6.2/PKG-INFO` & `audio_separator-0.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.6.2
+Version: 0.6.3
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
```

