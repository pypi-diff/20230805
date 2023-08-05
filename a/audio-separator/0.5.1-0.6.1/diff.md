# Comparing `tmp/audio_separator-0.5.1.tar.gz` & `tmp/audio_separator-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "audio_separator-0.5.1.tar", max compression
+gzip compressed data, was "audio_separator-0.6.1.tar", max compression
```

## Comparing `audio_separator-0.5.1.tar` & `audio_separator-0.6.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-09 20:53:03.831268 audio_separator-0.5.1/LICENSE
--rw-r--r--   0        0        0     7479 2023-07-09 20:53:03.831268 audio_separator-0.5.1/README.md
--rw-r--r--   0        0        0       33 2023-07-09 20:53:03.831268 audio_separator-0.5.1/audio_separator/__init__.py
--rw-r--r--   0        0        0    12879 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/separator.py
--rw-r--r--   0        0        0        0 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/utils/__init__.py
--rwxr-xr-x   0        0        0     2520 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/utils/cli.py
--rw-r--r--   0        0        0    21906 2023-07-09 20:53:03.835268 audio_separator-0.5.1/audio_separator/utils/spec_utils.py
--rw-r--r--   0        0        0      985 2023-07-09 20:53:03.835268 audio_separator-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     8539 1970-01-01 00:00:00.000000 audio_separator-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-06-30 05:57:58.913442 audio_separator-0.6.1/LICENSE
+-rw-r--r--   0        0        0     8757 2023-08-05 18:54:39.190288 audio_separator-0.6.1/README.md
+-rw-r--r--   0        0        0       33 2023-06-30 18:38:54.200542 audio_separator-0.6.1/audio_separator/__init__.py
+-rw-r--r--   0        0        0    13550 2023-08-05 19:04:39.431017 audio_separator-0.6.1/audio_separator/separator.py
+-rw-r--r--   0        0        0        0 2023-06-30 05:58:37.414385 audio_separator-0.6.1/audio_separator/utils/__init__.py
+-rwxr-xr-x   0        0        0     3459 2023-08-05 19:17:36.849760 audio_separator-0.6.1/audio_separator/utils/cli.py
+-rw-r--r--   0        0        0    21906 2023-08-05 18:58:36.032370 audio_separator-0.6.1/audio_separator/utils/spec_utils.py
+-rw-r--r--   0        0        0      985 2023-08-05 18:04:46.296326 audio_separator-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     9817 1970-01-01 00:00:00.000000 audio_separator-0.6.1/PKG-INFO
```

### Comparing `audio_separator-0.5.1/LICENSE` & `audio_separator-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `audio_separator-0.5.1/README.md` & `audio_separator-0.6.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -18,14 +18,27 @@
 
 ## Installation 🛠️
 
 You can install Audio Separator using pip:
 
 `pip install audio-separator`
 
+### Extra installation steps for use with a GPU
+
+Unfortunately the way Torch and ONNX Runtime are published means the correct platform-specific dependencies for CUDA use don't get installed by the package published to PyPI with Poetry.
+
+As such, if you want to use audio-separator with a CUDA-capable Nvidia GPU, you need to reinstall them directly, allowing pip to calculate the right versions for your platform:
+
+- `pip uninstall torch onnxruntime`
+- `pip cache purge`
+- `pip install -r requirements-gpu.txt`
+
+This should get you set up to run audio-separator with CUDA acceleration, using the `--use_cuda` argument.
+
+> Note: if anyone has a way to make this cleaner so we can support both CPU and CUDA transcodes without separate installation processes, please let me know or submit a PR!
 
 ## Usage 🚀
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
@@ -35,14 +48,16 @@
     audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
     log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
     log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
     model_name: (Optional) The name of the model to use for separation. Default: UVR_MDXNET_KARA_2
     model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
     output_dir: (Optional) The directory where the separated files will be saved. If not specified, outputs to current dir.
     use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+    denoise_enabled: (Optional) Flag to enable or disable denoising as part of the separation process. Default: True
+    normalization_enabled: (Optional) Flag to enable or disable normalization as part of the separation process. Default: False
     output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 ```
 
 Example:
 
 ```
 audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
@@ -72,14 +87,16 @@
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
 - log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
 - log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
 - use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+- denoise_enabled: (Optional) Flag to enable or disable denoising as part of the separation process. Default: True
+- normalization_enabled: (Optional) Flag to enable or disable normalization as part of the separation process. Default: False
 - output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 
 ## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
```

### Comparing `audio_separator-0.5.1/audio_separator/separator.py` & `audio_separator-0.6.1/audio_separator/separator.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,14 +21,16 @@
         log_formatter=None,
         model_name="UVR_MDXNET_KARA_2",
         model_file_dir="/tmp/audio-separator-models/",
         output_dir=None,
         use_cuda=False,
         output_format="WAV",
         output_subtype=None,
+        normalization_enabled=True,
+        denoise_enabled=True,
     ):
         self.logger = logging.getLogger(__name__)
         self.logger.setLevel(log_level)
         self.log_level = log_level
         self.log_formatter = log_formatter
 
         self.log_handler = logging.StreamHandler()
@@ -63,16 +65,25 @@
 
         if self.output_format is None:
             self.output_format = "WAV"
 
         if self.output_subtype is None and output_format == "WAV":
             self.output_subtype = "PCM_16"
 
-        self.is_normalization = False
-        self.is_denoise = False
+        self.normalization_enabled = normalization_enabled
+        if self.normalization_enabled:
+            self.logger.debug(f"Normalization enabled, waveform will be normalized to max amplitude of 1.0 to avoid clipping.")
+        else:
+            self.logger.debug(f"Normalization disabled, waveform will not be normalized.")
+
+        self.denoise_enabled = denoise_enabled
+        if self.denoise_enabled:
+            self.logger.debug(f"Denoising enabled, model will be run twice to reduce noise in output audio.")
+        else:
+            self.logger.debug(f"Denoising disabled, model will only be run once. This may result in noisier output audio.")
 
         self.chunks = 0
         self.margin = 44100
         self.adjust = 1
         self.dim_c = 4
         self.hop = 1024
 
@@ -149,23 +160,23 @@
         mix, raw_mix, samplerate = prepare_mix(self.audio_file_path, self.chunks, self.margin, mdx_net_cut=mdx_net_cut)
         self.logger.info("Demixing...")
         source = self.demix_base(mix)[0]
 
         self.logger.info(f"Saving {self.primary_stem} stem...")
         primary_stem_path = os.path.join(f"{self.audio_file_base}_({self.primary_stem})_{self.model_name}.{self.output_format.lower()}")
         if not isinstance(self.primary_source, np.ndarray):
-            self.primary_source = spec_utils.normalize(self.logger, source, self.is_normalization).T
+            self.primary_source = spec_utils.normalize(self.logger, source, self.normalization_enabled).T
         self.write_audio(primary_stem_path, self.primary_source, samplerate)
 
         self.logger.info(f"Saving {self.secondary_stem} stem...")
         secondary_stem_path = os.path.join(f"{self.audio_file_base}_({self.secondary_stem})_{self.model_name}.{self.output_format.lower()}")
         if not isinstance(self.secondary_source, np.ndarray):
             raw_mix = self.demix_base(raw_mix, is_match_mix=True)[0] if mdx_net_cut else raw_mix
             self.secondary_source, raw_mix = spec_utils.normalize_two_stem(
-                self.logger, source * self.compensate, raw_mix, self.is_normalization
+                self.logger, source * self.compensate, raw_mix, self.normalization_enabled
             )
             self.secondary_source = -self.secondary_source.T + raw_mix.T
         self.write_audio(secondary_stem_path, self.secondary_source, samplerate)
 
         torch.cuda.empty_cache()
         return primary_stem_path, secondary_stem_path
 
@@ -233,15 +244,15 @@
     def run_model(self, mix, is_ckpt=False, is_match_mix=False):
         spek = self.stft(mix.to(self.device)) * self.adjust
         spek[:, :, :3, :] *= 0
 
         if is_match_mix:
             spec_pred = spek.cpu().numpy()
         else:
-            spec_pred = -self.model_run(-spek) * 0.5 + self.model_run(spek) * 0.5 if self.is_denoise else self.model_run(spek)
+            spec_pred = -self.model_run(-spek) * 0.5 + self.model_run(spek) * 0.5 if self.denoise_enabled else self.model_run(spek)
 
         if is_ckpt:
             return self.istft(spec_pred).cpu().detach().numpy()
         else:
             return (
                 self.istft(torch.tensor(spec_pred).to(self.device))
                 .to(self.cpu)[:, :, self.trim : -self.trim]
```

### Comparing `audio_separator-0.5.1/audio_separator/utils/cli.py` & `audio_separator-0.6.1/audio_separator/utils/cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,21 +17,58 @@
         formatter_class=lambda prog: argparse.HelpFormatter(prog, max_help_position=35),
     )
 
     parser.add_argument("audio_file", nargs="?", help="The audio file path to separate, in any common format.", default=argparse.SUPPRESS)
 
     package_version = pkg_resources.get_distribution("audio-separator").version
     parser.add_argument("-v", "--version", action="version", version=f"%(prog)s {package_version}")
-    parser.add_argument("--log_level", default="INFO", help="Optional: Logging level, e.g. info, debug, warning. Default: INFO")
 
-    parser.add_argument("--model_name", default="UVR_MDXNET_KARA_2", help="Optional: model name to be used for separation.")
-    parser.add_argument("--model_file_dir", default="/tmp/audio-separator-models/", help="Optional: model files directory.")
-    parser.add_argument("--output_dir", default=None, help="Optional: directory to write output files. Default: current dir.")
-    parser.add_argument("--use_cuda", action="store_true", help="Optional: use Nvidia GPU with CUDA for separation.")
-    parser.add_argument("--output_format", default="FLAC", help="Optional: output format for separated files, any common format. Default: FLAC")
+    parser.add_argument(
+        "--log_level", default="info", help="Optional: logging level, e.g. info, debug, warning (default: info). Ex: --log_level=debug"
+    )
+
+    parser.add_argument(
+        "--model_name",
+        default="UVR_MDXNET_KARA_2",
+        help="Optional: model name to be used for separation (default: UVR_MDXNET_KARA_2). Ex: --model_name=UVR-MDX-NET-Inst_HQ_3",
+    )
+
+    parser.add_argument(
+        "--model_file_dir",
+        default="/tmp/audio-separator-models/",
+        help="Optional: model files directory (default: /tmp/audio-separator-models/). Ex: --model_file_dir=/app/models",
+    )
+
+    parser.add_argument(
+        "--output_dir",
+        default=None,
+        help="Optional: directory to write output files (default: <current dir>). Ex: --output_dir=/app/separated",
+    )
+
+    parser.add_argument(
+        "--use_cuda", action="store_true", help="Optional: use Nvidia GPU with CUDA for separation (default: false). Ex: --use_cuda=true"
+    )
+
+    parser.add_argument(
+        "--output_format", default="FLAC", help="Optional: output format for separated files, any common format. Default: FLAC"
+    )
+
+    parser.add_argument(
+        "--denoise",
+        type=lambda x: (str(x).lower() == "true"),
+        default=True,
+        help="Optional: enable or disable denoising during separation (default: True). Ex: --denoise=False",
+    )
+
+    parser.add_argument(
+        "--normalize",
+        type=lambda x: (str(x).lower() == "true"),
+        default=True,
+        help="Optional: enable or disable normalization during separation (default: True). Ex: --normalize=False",
+    )
 
     args = parser.parse_args()
 
     log_level = getattr(logging, args.log_level.upper())
     logger.setLevel(log_level)
 
     if not hasattr(args, "audio_file"):
@@ -45,14 +82,16 @@
         log_formatter=log_formatter,
         log_level=log_level,
         model_name=args.model_name,
         model_file_dir=args.model_file_dir,
         output_dir=args.output_dir,
         use_cuda=args.use_cuda,
         output_format=args.output_format,
+        denoise_enabled=args.denoise,
+        normalization_enabled=args.normalize,
     )
     primary_stem_path, secondary_stem_path = separator.separate()
 
     logger.info(f"Separation complete! Output files: {primary_stem_path} {secondary_stem_path}")
 
 
 if __name__ == "__main__":
```

### Comparing `audio_separator-0.5.1/audio_separator/utils/spec_utils.py` & `audio_separator-0.6.1/audio_separator/utils/spec_utils.py`

 * *Files identical despite different names*

### Comparing `audio_separator-0.5.1/pyproject.toml` & `audio_separator-0.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "audio-separator"
-version = "0.5.1"
+version = "0.6.1"
 description = "Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07"
 authors = ["Andrew Beveridge <andrew@beveridge.uk>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "audio_separator"}]
 homepage = "https://github.com/karaokenerds/python-audio-separator"
 repository = "https://github.com/karaokenerds/python-audio-separator"
```

### Comparing `audio_separator-0.5.1/PKG-INFO` & `audio_separator-0.6.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: audio-separator
-Version: 0.5.1
+Version: 0.6.1
 Summary: Easy to use vocal separation on CLI or as a python package, using the amazing MDX-Net models from UVR trained by @Anjok07
 Home-page: https://github.com/karaokenerds/python-audio-separator
 License: MIT
 Author: Andrew Beveridge
 Author-email: andrew@beveridge.uk
 Requires-Python: >=3.9,<3.11
 Classifier: License :: OSI Approved :: MIT License
@@ -43,14 +43,27 @@
 
 ## Installation 🛠️
 
 You can install Audio Separator using pip:
 
 `pip install audio-separator`
 
+### Extra installation steps for use with a GPU
+
+Unfortunately the way Torch and ONNX Runtime are published means the correct platform-specific dependencies for CUDA use don't get installed by the package published to PyPI with Poetry.
+
+As such, if you want to use audio-separator with a CUDA-capable Nvidia GPU, you need to reinstall them directly, allowing pip to calculate the right versions for your platform:
+
+- `pip uninstall torch onnxruntime`
+- `pip cache purge`
+- `pip install -r requirements-gpu.txt`
+
+This should get you set up to run audio-separator with CUDA acceleration, using the `--use_cuda` argument.
+
+> Note: if anyone has a way to make this cleaner so we can support both CPU and CUDA transcodes without separate installation processes, please let me know or submit a PR!
 
 ## Usage 🚀
 
 ### Command Line Interface (CLI)
 
 You can use Audio Separator via the command line:
 
@@ -60,14 +73,16 @@
     audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
     log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
     log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
     model_name: (Optional) The name of the model to use for separation. Default: UVR_MDXNET_KARA_2
     model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
     output_dir: (Optional) The directory where the separated files will be saved. If not specified, outputs to current dir.
     use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+    denoise_enabled: (Optional) Flag to enable or disable denoising as part of the separation process. Default: True
+    normalization_enabled: (Optional) Flag to enable or disable normalization as part of the separation process. Default: False
     output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 ```
 
 Example:
 
 ```
 audio-separator /path/to/your/audio.wav --model_name UVR_MDXNET_KARA_2
@@ -97,14 +112,16 @@
 - audio_file: The path to the audio file to be separated. Supports all common formats (WAV, MP3, FLAC, M4A, etc.)
 - log_level: (Optional) Logging level, e.g. info, debug, warning. Default: INFO
 - log_formatter: (Optional) The log format. Default: '%(asctime)s - %(name)s - %(levelname)s - %(message)s'
 - model_name: (Optional) The name of the model to use for separation. Defaults to 'UVR_MDXNET_KARA_2', a very powerful model for Karaoke instrumental tracks.
 - model_file_dir: (Optional) Directory to cache model files in. Default: /tmp/audio-separator-models/
 - output_dir: (Optional) Directory where the separated files will be saved. If not specified, outputs to current dir.
 - use_cuda: (Optional) Flag to use Nvidia GPU via CUDA for separation if available. Default: False
+- denoise_enabled: (Optional) Flag to enable or disable denoising as part of the separation process. Default: True
+- normalization_enabled: (Optional) Flag to enable or disable normalization as part of the separation process. Default: False
 - output_format: (Optional) Format to encode output files, any common format (WAV, MP3, FLAC, M4A, etc.). Default: WAV
 
 ## Requirements 📋
 
 Python <= 3.10 (one of the dependencies doesn't like 3.11 yet)
 
 Libraries: onnx, onnxruntime, numpy, soundfile, librosa, torch, wget, six
```

