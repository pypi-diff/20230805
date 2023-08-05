# Comparing `tmp/vaimm-0.1.0.tar.gz` & `tmp/vaimm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vaimm-0.1.0.tar", last modified: Fri Aug  4 19:33:21 2023, max compression
+gzip compressed data, was "vaimm-0.2.0.tar", last modified: Fri Aug  4 21:08:58 2023, max compression
```

## Comparing `vaimm-0.1.0.tar` & `vaimm-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:33:21.854784 vaimm-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:33:21.842784 vaimm-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:33:21.846784 vaimm-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 19:33:06.000000 vaimm-0.1.0/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 19:33:06.000000 vaimm-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-04 19:33:06.000000 vaimm-0.1.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-08-04 19:33:21.854784 vaimm-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10159 2023-08-04 19:33:06.000000 vaimm-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-04 19:33:06.000000 vaimm-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:33:21.854784 vaimm-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:33:21.846784 vaimm-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 19:33:06.000000 vaimm-0.1.0/tests/test_example.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:33:21.850784 vaimm-0.1.0/vaimm/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-04 19:33:06.000000 vaimm-0.1.0/vaimm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6197 2023-08-04 19:33:06.000000 vaimm-0.1.0/vaimm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-08-04 19:33:06.000000 vaimm-0.1.0/vaimm/net.py
--rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-04 19:33:06.000000 vaimm-0.1.0/vaimm/vai.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 19:33:06.000000 vaimm-0.1.0/vaimm/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 19:33:21.854784 vaimm-0.1.0/vaimm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 19:33:21.000000 vaimm-0.1.0/vaimm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:08:58.355181 vaimm-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:08:58.351180 vaimm-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:08:58.351180 vaimm-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-08-04 21:08:44.000000 vaimm-0.2.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-04 21:08:44.000000 vaimm-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-08-04 21:08:44.000000 vaimm-0.2.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-08-04 21:08:58.355181 vaimm-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10221 2023-08-04 21:08:44.000000 vaimm-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-08-04 21:08:44.000000 vaimm-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:08:58.355181 vaimm-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:08:58.351180 vaimm-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 21:08:44.000000 vaimm-0.2.0/tests/test_example.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:08:58.351180 vaimm-0.2.0/vaimm/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-08-04 21:08:44.000000 vaimm-0.2.0/vaimm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6581 2023-08-04 21:08:44.000000 vaimm-0.2.0/vaimm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4481 2023-08-04 21:08:44.000000 vaimm-0.2.0/vaimm/net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3642 2023-08-04 21:08:44.000000 vaimm-0.2.0/vaimm/vai.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 21:08:44.000000 vaimm-0.2.0/vaimm/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 21:08:58.355181 vaimm-0.2.0/vaimm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10595 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-04 21:08:58.000000 vaimm-0.2.0/vaimm.egg-info/top_level.txt
```

### Comparing `vaimm-0.1.0/.github/workflows/release.yml` & `vaimm-0.2.0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `vaimm-0.1.0/PKG-INFO` & `vaimm-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: vaimm
-Version: 0.1.0
-Summary: Quickly download models for Topaz Video AI
-Author-email: jojje <tinjon+pypi@gmail.com>
-License: GPLv2
-Keywords: vai,video,ai,models
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 
 # vaimm
 
 VAI model manager
 
 Quickly download models for Topaz Video AI.
 
@@ -28,49 +16,49 @@
 ```text
 usage: vaimm [-h] [--json-dir path]  ...
 
 VAI Models Manager (<version>): Download missing models for TopazLabs Video AI
 
 options:
   -h, --help       show this help message and exit
-  --json-dir path  Directory where the VAI model json files reside. E.g. alq-13.json.
-                   Defaults to the value of the environment variable TVAI_MODEL_DIR if
-                   set, else the windows default if running on windows, else you have to
-                   specify it yourself. (default: C:\ProgramData\Topaz Labs LLC\Topaz
-                   Video AI\models)
+  --json-dir path  Directory where the VAI model json files reside. E.g.
+                   alq-13.json. Defaults to the value of the environment variable
+                   TVAI_MODEL_DIR if set, else checks if any of the default folders
+                   exist, otherwise you just have to specify it yourself. (default:
+                   C:\ProgramData\Topaz Labs LLC\Topaz Video AI\models)
 
 commands:
-    backends       Lists the available backends that VAI supports
+    list-backends  Lists the available backends that VAI supports
     list-models    Lists available models for a given backend
     list-files     Lists model files for a backend
     download       Download VAI models missing from your model data directory
 ```
 
 Each command takes options and arguments. List which ones are available,
 optional and required by providing `--help` after the command name. 
 
-Example: `vaimm backends --help`
+Example: `vaimm list-backends --help`
 
 To use any of the commands, you have to specify where the VAI model JSON files
 are. For windows users, the default (shown above) should be the correct location
 for most folks. For Mac and Linux users, you'll have to specify the path
 explicitly.
 
-Example: `vaimm --json-dir /opt/TopazVideoAIBETA/models backends`
+Example: `vaimm --json-dir /opt/TopazVideoAIBETA/models list-backends`
 
 The list commands are there to give you some information about the models and
 versions available, and what model files are required for each. If you are only
 interested in a subset of the models, you can tell the program to filter only on
 those.
 
 For example, to only show the latest version of the model files for Artemis Medium and
 Prometheus, applicable to the ONNX (32-bit) backend:
 
 ```
-$ vaimm list-files onnx --include prob-3,amq-13
+$ vaimm list-files --backend onnx --include prob-3,amq-13
 
 amq-v13-fgnet-fp32-256x352-1x-ox.tz
 amq-v13-fgnet-fp32-256x352-2x-ox.tz
 ...
 prob-v3-fgnet-fp32-576x672-2x-ox.tz
 prob-v3-fgnet-fp32-576x672-4x-ox.tz
 
@@ -94,48 +82,49 @@
 subset of models to download. You _really_ want to do this, since the complete
 set of models are hundred(s) of gigabyte in size.
 
 Let's say you want to download the same two model files ("onnx networks") listed
 above, for a RTX 3080 card which uses 16-bit floating point.
 
 ```
-$ vaimm download onnx16 --include prob-3,amq-13 --dir . --cookie "$COOKIE"
+$ vaimm download --backend onnx16 --include prob-3,amq-13 --dir . --cookie "$COOKIE"
 
 Downloading: 100%|████████████████| 54/54 [00:26<00:00,  2.07 files /s, speed=64.04 MiB/s]
 Download completed successfully with 1.63 GiB of data fetched.
 ```
 
 * `--dir` is the directory the files should be saved to. You'd likely want to
   specify the `TVAI_MODEL_DATA_DIR` directory. I.e. where you already have some
   model files that VAI downloaded on-the-fly as you used that program.
 * `--cookie` is a cloudflare authentication string which Topaz has configured
   their CDN to require. This value is likely unique per user, so you have to
   discover what yours is before you can download any models. How to find this
   value is in the help description for the command. See below.
 
 ```
-usage: vaimm download [-h] [--backend name] [--include ids] -d path -c str [-t n]
+usage: vaimm download [-h] --backend name [--include ids] -d path -c str [-t n]
 
 options:
   -h, --help            show this help message and exit
-  --backend name        Name of the backend to fetch models for (env: TVAI_BACKEND
-                        (default: onnx)
-  --include ids         Commma separated list of specific model(s) to include (default:
-                        None)
-  -d path, --dir path   Path to your model data directory. Defaults to env-var
-                        TVAI_MODEL_DATA_DIR if set. (default: None)
-  -c str, --cookie str  The value of the cf_clearance cookie, required to download files
-                        from topaz Cloudflare CDN. You can find this when logged into
-                        the topaz website, by opening "developer tools" in firefox (or
-                        inspector in chrome), then the network tab. Once that is done,
-                        download a test model from the browser. E.g: https://veai-
-                        models.topazlabs.com/prap-v3-fp32-ov.tz . Finally look at the
-                        request headers for the associated request, and the Cookie
-                        header. That header has the value required. It looks like
-                        "cf_clearance: <the-string-you-need-here>". (default: None)
+  --backend name        Name of the backend to fetch models for (env: TVAI_BACKEND)
+                        (default: None)
+  --include ids         Commma separated list of specific model(s) to include
+                        (default: None)
+  -d path, --dir path   Path to your model data directory (env:
+                        TVAI_MODEL_DATA_DIR). (default: None)
+  -c str, --cookie str  The value of the cf_clearance cookie, required to download
+                        files from topaz Cloudflare CDN. You can find this when
+                        logged into the topaz website, by opening "developer tools"
+                        in firefox (or inspector in chrome), then the network tab.
+                        Once that is done, download a test model from the browser.
+                        E.g: https://veai-models.topazlabs.com/prap-v3-fp32-ov.tz .
+                        Finally look at the request headers for the associated
+                        request, and the Cookie header. That header has the value
+                        required. It looks like "cf_clearance: <the-string-you-need-
+                        here>" (env: TVAI_COOKIE). (default: None)
   -t n, --threads n     Number of concurrent downloads to use (default: 4)
 ```
 
 One note on the `--include` option. It says default is None. What that _really_
 means is that there is no filtering for specific model IDs done by default. So
 _all_ models for the backend will be downloaded if you don't limit the scope to
 just a few chosen, as was been done in the examples up until now.
```

### Comparing `vaimm-0.1.0/README.md` & `vaimm-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: vaimm
+Version: 0.2.0
+Summary: Quickly download models for Topaz Video AI
+Author-email: jojje <tinjon+pypi@gmail.com>
+License: GPLv2
+Keywords: vai,video,ai,models
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 
 # vaimm
 
 VAI model manager
 
 Quickly download models for Topaz Video AI.
 
@@ -16,49 +28,49 @@
 ```text
 usage: vaimm [-h] [--json-dir path]  ...
 
 VAI Models Manager (<version>): Download missing models for TopazLabs Video AI
 
 options:
   -h, --help       show this help message and exit
-  --json-dir path  Directory where the VAI model json files reside. E.g. alq-13.json.
-                   Defaults to the value of the environment variable TVAI_MODEL_DIR if
-                   set, else the windows default if running on windows, else you have to
-                   specify it yourself. (default: C:\ProgramData\Topaz Labs LLC\Topaz
-                   Video AI\models)
+  --json-dir path  Directory where the VAI model json files reside. E.g.
+                   alq-13.json. Defaults to the value of the environment variable
+                   TVAI_MODEL_DIR if set, else checks if any of the default folders
+                   exist, otherwise you just have to specify it yourself. (default:
+                   C:\ProgramData\Topaz Labs LLC\Topaz Video AI\models)
 
 commands:
-    backends       Lists the available backends that VAI supports
+    list-backends  Lists the available backends that VAI supports
     list-models    Lists available models for a given backend
     list-files     Lists model files for a backend
     download       Download VAI models missing from your model data directory
 ```
 
 Each command takes options and arguments. List which ones are available,
 optional and required by providing `--help` after the command name. 
 
-Example: `vaimm backends --help`
+Example: `vaimm list-backends --help`
 
 To use any of the commands, you have to specify where the VAI model JSON files
 are. For windows users, the default (shown above) should be the correct location
 for most folks. For Mac and Linux users, you'll have to specify the path
 explicitly.
 
-Example: `vaimm --json-dir /opt/TopazVideoAIBETA/models backends`
+Example: `vaimm --json-dir /opt/TopazVideoAIBETA/models list-backends`
 
 The list commands are there to give you some information about the models and
 versions available, and what model files are required for each. If you are only
 interested in a subset of the models, you can tell the program to filter only on
 those.
 
 For example, to only show the latest version of the model files for Artemis Medium and
 Prometheus, applicable to the ONNX (32-bit) backend:
 
 ```
-$ vaimm list-files onnx --include prob-3,amq-13
+$ vaimm list-files --backend onnx --include prob-3,amq-13
 
 amq-v13-fgnet-fp32-256x352-1x-ox.tz
 amq-v13-fgnet-fp32-256x352-2x-ox.tz
 ...
 prob-v3-fgnet-fp32-576x672-2x-ox.tz
 prob-v3-fgnet-fp32-576x672-4x-ox.tz
 
@@ -82,48 +94,49 @@
 subset of models to download. You _really_ want to do this, since the complete
 set of models are hundred(s) of gigabyte in size.
 
 Let's say you want to download the same two model files ("onnx networks") listed
 above, for a RTX 3080 card which uses 16-bit floating point.
 
 ```
-$ vaimm download onnx16 --include prob-3,amq-13 --dir . --cookie "$COOKIE"
+$ vaimm download --backend onnx16 --include prob-3,amq-13 --dir . --cookie "$COOKIE"
 
 Downloading: 100%|████████████████| 54/54 [00:26<00:00,  2.07 files /s, speed=64.04 MiB/s]
 Download completed successfully with 1.63 GiB of data fetched.
 ```
 
 * `--dir` is the directory the files should be saved to. You'd likely want to
   specify the `TVAI_MODEL_DATA_DIR` directory. I.e. where you already have some
   model files that VAI downloaded on-the-fly as you used that program.
 * `--cookie` is a cloudflare authentication string which Topaz has configured
   their CDN to require. This value is likely unique per user, so you have to
   discover what yours is before you can download any models. How to find this
   value is in the help description for the command. See below.
 
 ```
-usage: vaimm download [-h] [--backend name] [--include ids] -d path -c str [-t n]
+usage: vaimm download [-h] --backend name [--include ids] -d path -c str [-t n]
 
 options:
   -h, --help            show this help message and exit
-  --backend name        Name of the backend to fetch models for (env: TVAI_BACKEND
-                        (default: onnx)
-  --include ids         Commma separated list of specific model(s) to include (default:
-                        None)
-  -d path, --dir path   Path to your model data directory. Defaults to env-var
-                        TVAI_MODEL_DATA_DIR if set. (default: None)
-  -c str, --cookie str  The value of the cf_clearance cookie, required to download files
-                        from topaz Cloudflare CDN. You can find this when logged into
-                        the topaz website, by opening "developer tools" in firefox (or
-                        inspector in chrome), then the network tab. Once that is done,
-                        download a test model from the browser. E.g: https://veai-
-                        models.topazlabs.com/prap-v3-fp32-ov.tz . Finally look at the
-                        request headers for the associated request, and the Cookie
-                        header. That header has the value required. It looks like
-                        "cf_clearance: <the-string-you-need-here>". (default: None)
+  --backend name        Name of the backend to fetch models for (env: TVAI_BACKEND)
+                        (default: None)
+  --include ids         Commma separated list of specific model(s) to include
+                        (default: None)
+  -d path, --dir path   Path to your model data directory (env:
+                        TVAI_MODEL_DATA_DIR). (default: None)
+  -c str, --cookie str  The value of the cf_clearance cookie, required to download
+                        files from topaz Cloudflare CDN. You can find this when
+                        logged into the topaz website, by opening "developer tools"
+                        in firefox (or inspector in chrome), then the network tab.
+                        Once that is done, download a test model from the browser.
+                        E.g: https://veai-models.topazlabs.com/prap-v3-fp32-ov.tz .
+                        Finally look at the request headers for the associated
+                        request, and the Cookie header. That header has the value
+                        required. It looks like "cf_clearance: <the-string-you-need-
+                        here>" (env: TVAI_COOKIE). (default: None)
   -t n, --threads n     Number of concurrent downloads to use (default: 4)
 ```
 
 One note on the `--include` option. It says default is None. What that _really_
 means is that there is no filtering for specific model IDs done by default. So
 _all_ models for the backend will be downloaded if you don't limit the scope to
 just a few chosen, as was been done in the examples up until now.
```

### Comparing `vaimm-0.1.0/pyproject.toml` & `vaimm-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `vaimm-0.1.0/vaimm/cli.py` & `vaimm-0.2.0/vaimm/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,47 +17,46 @@
 ENV_BACKEND = 'TVAI_BACKEND'
 ENV_COOKIE = 'TVAI_COOKIE'
 AVG_MODEL_SIZE_MB = 91
 
 def main():
     opts = parser_args()
     metas = find_models_metadata(opts.json_dir)
-    if opts.cmd == 'backends':
+    if opts.cmd == 'list-backends':
         list_backends(metas)
     elif opts.cmd == 'list-models':
         list_models(metas, opts.backend)
     elif opts.cmd == 'list-files':
         list_backend_files(metas, opts.backend, opts.include)
     elif opts.cmd == 'download':
         download_missing_files(metas, opts.backend, opts.include, opts.dir, opts.threads, opts.cookie)
     else:
         print(f'command {opts.cmd} not implemented (this is a bug)', file=sys.stderr)
         sys.exit(-1)
 
 
 def parser_args() -> argparse.Namespace:
-    win = platform.system() == 'Windows'
-    json_dir = os.getenv(ENV_JSON_DIR, WINDOWS_DEFAULT_JSON_DIR if win else None)
+    json_dir = find_models_json_dir()
     model_dir = os.getenv(ENV_MODEL_DIR)
     backend = os.getenv(ENV_BACKEND)
     cookie = os.getenv(ENV_COOKIE)
 
     helper = argparse.ArgumentDefaultsHelpFormatter
 
     parser = argparse.ArgumentParser(
         formatter_class=helper,
         description=f'VAI Models Manager (v{__version__}): Download missing models for TopazLabs Video AI'
     )
     parser.add_argument('--json-dir', metavar='path', default=json_dir, required=not json_dir,
                         help='Directory where the VAI model json files reside. E.g. alq-13.json. Defaults to the '
-                             f'value of the environment variable {ENV_JSON_DIR} if set, else the windows default if '
-                             'running on windows, else you have to specify it yourself.')
+                             f'value of the environment variable {ENV_JSON_DIR} if set, else checks if any of the '
+                              'default folders exist, otherwise you just have to specify it yourself.')
 
     commands = parser.add_subparsers(dest='cmd', title='commands', metavar='')
-    commands.add_parser('backends', help='Lists the available backends that VAI supports')
+    commands.add_parser('list-backends', help='Lists the available backends that VAI supports')
 
     mlist = commands.add_parser('list-models', help='Lists available models for a given backend')
     mlist.add_argument('--backend', metavar='name', default=backend, required=not backend,
                        help=f'Name of the backend to list models for (env: {ENV_BACKEND})')
 
     files = commands.add_parser('list-files', help='Lists model files for a backend')
     files.add_argument('--backend', metavar='name', default=backend, required=not backend,
@@ -66,23 +65,24 @@
 
     download = commands.add_parser('download', formatter_class=helper,
                                    help='Download VAI models missing from your model data directory')
     download.add_argument('--backend', metavar='name', default=backend, required=not backend,
                           help=f'Name of the backend to fetch models for (env: {ENV_BACKEND})')
     download.add_argument('--include', metavar='ids', help='Commma separated list of specific model(s) to include')
     download.add_argument('-d', '--dir', metavar='path', default=model_dir, required=not model_dir,
-                          help='Path to your model data directory. Defaults to env-var TVAI_MODEL_DATA_DIR if set.')
+                          help=f'Path to your model data directory (env: {ENV_MODEL_DIR}).')
     download.add_argument('-c', '--cookie', metavar='str', default=cookie, required=not cookie,
                           help='The value of the cf_clearance cookie, required to download files from topaz '
                                'Cloudflare CDN. You can find this when logged into the topaz website, by opening '
                                '"developer tools" in firefox (or inspector in chrome), then the network tab. Once '
                                'that is done, download a test model from the browser. E.g: '
                                'https://veai-models.topazlabs.com/prap-v3-fp32-ov.tz . Finally look at the request '
                                'headers for the associated request, and the Cookie header. That header has the value '
-                               'required. It looks like "cf_clearance: <the-string-you-need-here>".')
+                               'required. It looks like "cf_clearance: <the-string-you-need-here>" '
+                               f'(env: {ENV_COOKIE}).')
     download.add_argument('-t', '--threads', metavar='n', default=4, type=int,
                           help='Number of concurrent downloads to use')
 
     if len(sys.argv) < 2:
         sys.argv.append('-h')
     return parser.parse_args()
 
@@ -117,7 +117,19 @@
 
 
 def find_missing_files(model_dicts:Iterable[dict], backend:str, includes:str, data_dir:str):
     backend_files = find_backend_files(model_dicts, backend, includes)
     target_files = (os.path.join(data_dir, file) for file in backend_files)
     missing_files = (file for file in target_files if not os.path.exists(file))
     return missing_files
+
+
+def find_models_json_dir() -> str:
+    candidates = [
+        os.getenv('ENV_JSON_DIR', ''),
+        os.path.join(os.getenv('PROGRAMDATA', ''), 'Topaz Labs LLC\\Topaz Video AI\\models'),
+        '/Applications/Topaz Video AI.app/Contents/Resources/models',
+        '/opt/TopazVideoAIBETA/models',
+    ]
+    for path in candidates:
+        if path and os.path.exists(f'{path}/alq-13.json'):
+            return path
```

### Comparing `vaimm-0.1.0/vaimm/net.py` & `vaimm-0.2.0/vaimm/net.py`

 * *Files identical despite different names*

### Comparing `vaimm-0.1.0/vaimm/vai.py` & `vaimm-0.2.0/vaimm/vai.py`

 * *Files identical despite different names*

### Comparing `vaimm-0.1.0/vaimm.egg-info/PKG-INFO` & `vaimm-0.2.0/vaimm.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vaimm
-Version: 0.1.0
+Version: 0.2.0
 Summary: Quickly download models for Topaz Video AI
 Author-email: jojje <tinjon+pypi@gmail.com>
 License: GPLv2
 Keywords: vai,video,ai,models
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
 Classifier: Development Status :: 4 - Beta
 Requires-Python: >=3.7
@@ -28,49 +28,49 @@
 ```text
 usage: vaimm [-h] [--json-dir path]  ...
 
 VAI Models Manager (<version>): Download missing models for TopazLabs Video AI
 
 options:
   -h, --help       show this help message and exit
-  --json-dir path  Directory where the VAI model json files reside. E.g. alq-13.json.
-                   Defaults to the value of the environment variable TVAI_MODEL_DIR if
-                   set, else the windows default if running on windows, else you have to
-                   specify it yourself. (default: C:\ProgramData\Topaz Labs LLC\Topaz
-                   Video AI\models)
+  --json-dir path  Directory where the VAI model json files reside. E.g.
+                   alq-13.json. Defaults to the value of the environment variable
+                   TVAI_MODEL_DIR if set, else checks if any of the default folders
+                   exist, otherwise you just have to specify it yourself. (default:
+                   C:\ProgramData\Topaz Labs LLC\Topaz Video AI\models)
 
 commands:
-    backends       Lists the available backends that VAI supports
+    list-backends  Lists the available backends that VAI supports
     list-models    Lists available models for a given backend
     list-files     Lists model files for a backend
     download       Download VAI models missing from your model data directory
 ```
 
 Each command takes options and arguments. List which ones are available,
 optional and required by providing `--help` after the command name. 
 
-Example: `vaimm backends --help`
+Example: `vaimm list-backends --help`
 
 To use any of the commands, you have to specify where the VAI model JSON files
 are. For windows users, the default (shown above) should be the correct location
 for most folks. For Mac and Linux users, you'll have to specify the path
 explicitly.
 
-Example: `vaimm --json-dir /opt/TopazVideoAIBETA/models backends`
+Example: `vaimm --json-dir /opt/TopazVideoAIBETA/models list-backends`
 
 The list commands are there to give you some information about the models and
 versions available, and what model files are required for each. If you are only
 interested in a subset of the models, you can tell the program to filter only on
 those.
 
 For example, to only show the latest version of the model files for Artemis Medium and
 Prometheus, applicable to the ONNX (32-bit) backend:
 
 ```
-$ vaimm list-files onnx --include prob-3,amq-13
+$ vaimm list-files --backend onnx --include prob-3,amq-13
 
 amq-v13-fgnet-fp32-256x352-1x-ox.tz
 amq-v13-fgnet-fp32-256x352-2x-ox.tz
 ...
 prob-v3-fgnet-fp32-576x672-2x-ox.tz
 prob-v3-fgnet-fp32-576x672-4x-ox.tz
 
@@ -94,48 +94,49 @@
 subset of models to download. You _really_ want to do this, since the complete
 set of models are hundred(s) of gigabyte in size.
 
 Let's say you want to download the same two model files ("onnx networks") listed
 above, for a RTX 3080 card which uses 16-bit floating point.
 
 ```
-$ vaimm download onnx16 --include prob-3,amq-13 --dir . --cookie "$COOKIE"
+$ vaimm download --backend onnx16 --include prob-3,amq-13 --dir . --cookie "$COOKIE"
 
 Downloading: 100%|████████████████| 54/54 [00:26<00:00,  2.07 files /s, speed=64.04 MiB/s]
 Download completed successfully with 1.63 GiB of data fetched.
 ```
 
 * `--dir` is the directory the files should be saved to. You'd likely want to
   specify the `TVAI_MODEL_DATA_DIR` directory. I.e. where you already have some
   model files that VAI downloaded on-the-fly as you used that program.
 * `--cookie` is a cloudflare authentication string which Topaz has configured
   their CDN to require. This value is likely unique per user, so you have to
   discover what yours is before you can download any models. How to find this
   value is in the help description for the command. See below.
 
 ```
-usage: vaimm download [-h] [--backend name] [--include ids] -d path -c str [-t n]
+usage: vaimm download [-h] --backend name [--include ids] -d path -c str [-t n]
 
 options:
   -h, --help            show this help message and exit
-  --backend name        Name of the backend to fetch models for (env: TVAI_BACKEND
-                        (default: onnx)
-  --include ids         Commma separated list of specific model(s) to include (default:
-                        None)
-  -d path, --dir path   Path to your model data directory. Defaults to env-var
-                        TVAI_MODEL_DATA_DIR if set. (default: None)
-  -c str, --cookie str  The value of the cf_clearance cookie, required to download files
-                        from topaz Cloudflare CDN. You can find this when logged into
-                        the topaz website, by opening "developer tools" in firefox (or
-                        inspector in chrome), then the network tab. Once that is done,
-                        download a test model from the browser. E.g: https://veai-
-                        models.topazlabs.com/prap-v3-fp32-ov.tz . Finally look at the
-                        request headers for the associated request, and the Cookie
-                        header. That header has the value required. It looks like
-                        "cf_clearance: <the-string-you-need-here>". (default: None)
+  --backend name        Name of the backend to fetch models for (env: TVAI_BACKEND)
+                        (default: None)
+  --include ids         Commma separated list of specific model(s) to include
+                        (default: None)
+  -d path, --dir path   Path to your model data directory (env:
+                        TVAI_MODEL_DATA_DIR). (default: None)
+  -c str, --cookie str  The value of the cf_clearance cookie, required to download
+                        files from topaz Cloudflare CDN. You can find this when
+                        logged into the topaz website, by opening "developer tools"
+                        in firefox (or inspector in chrome), then the network tab.
+                        Once that is done, download a test model from the browser.
+                        E.g: https://veai-models.topazlabs.com/prap-v3-fp32-ov.tz .
+                        Finally look at the request headers for the associated
+                        request, and the Cookie header. That header has the value
+                        required. It looks like "cf_clearance: <the-string-you-need-
+                        here>" (env: TVAI_COOKIE). (default: None)
   -t n, --threads n     Number of concurrent downloads to use (default: 4)
 ```
 
 One note on the `--include` option. It says default is None. What that _really_
 means is that there is no filtering for specific model IDs done by default. So
 _all_ models for the backend will be downloaded if you don't limit the scope to
 just a few chosen, as was been done in the examples up until now.
```

