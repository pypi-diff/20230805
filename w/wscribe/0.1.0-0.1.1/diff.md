# Comparing `tmp/wscribe-0.1.0.tar.gz` & `tmp/wscribe-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wscribe-0.1.0.tar", max compression
+gzip compressed data, was "wscribe-0.1.1.tar", max compression
```

## Comparing `wscribe-0.1.0.tar` & `wscribe-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-07-21 09:28:16.650987 wscribe-0.1.0/LICENSE
--rw-r--r--   0        0        0     2986 2023-07-25 13:58:47.678420 wscribe-0.1.0/README.org
--rw-r--r--   0        0        0     1043 2023-07-25 13:58:47.575421 wscribe-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1786 2023-07-25 13:58:47.564422 wscribe-0.1.0/src/wscribe/__init__.py
--rw-r--r--   0        0        0     2555 2023-07-25 14:05:14.337538 wscribe-0.1.0/src/wscribe/backends/fasterwhisper.py
--rw-r--r--   0        0        0     2186 2023-07-25 14:05:14.337538 wscribe-0.1.0/src/wscribe/cli/main.py
--rw-r--r--   0        0        0     1801 2023-07-25 13:58:47.516422 wscribe-0.1.0/src/wscribe/core.py
--rw-r--r--   0        0        0      378 2023-07-25 13:58:47.514422 wscribe-0.1.0/src/wscribe/sources/local.py
--rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 wscribe-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-21 09:28:16.650987 wscribe-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4960 2023-08-05 15:47:09.725778 wscribe-0.1.1/README.org
+-rw-r--r--   0        0        0     1128 2023-08-05 15:57:26.271659 wscribe-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1786 2023-07-25 13:58:47.564422 wscribe-0.1.1/src/wscribe/__init__.py
+-rw-r--r--   0        0        0     2576 2023-08-05 07:06:03.013196 wscribe-0.1.1/src/wscribe/backends/fasterwhisper.py
+-rw-r--r--   0        0        0     2253 2023-08-05 15:47:09.721778 wscribe-0.1.1/src/wscribe/cli/main.py
+-rw-r--r--   0        0        0     2157 2023-08-05 07:10:37.672683 wscribe-0.1.1/src/wscribe/core.py
+-rw-r--r--   0        0        0      378 2023-07-25 13:58:47.514422 wscribe-0.1.1/src/wscribe/sources/local.py
+-rw-r--r--   0        0        0     3298 2023-08-05 07:17:56.081761 wscribe-0.1.1/src/wscribe/writers.py
+-rw-r--r--   0        0        0     5618 1970-01-01 00:00:00.000000 wscribe-0.1.1/PKG-INFO
```

### Comparing `wscribe-0.1.0/LICENSE` & `wscribe-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.0/pyproject.toml` & `wscribe-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 [tool.poetry]
 name = "wscribe"
-version = "0.1.0"
-description = "Simple audio transcription tool using Whisper"
+version = "0.1.1"
+description = "ez audio transcription tool with flexible processing and post-processing options"
 authors = ["Hrishikesh Barman <oss@geekodour.org>"]
+homepage = "https://github.com/geekodour/wscribe"
 license = "MIT"
 readme = "README.org"
 packages = [{include = "wscribe", from = "src"}]
 
 [tool.poetry.scripts]
 wscribe = "wscribe.cli.main:cli"
```

### Comparing `wscribe-0.1.0/src/wscribe/__init__.py` & `wscribe-0.1.1/src/wscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.0/src/wscribe/backends/fasterwhisper.py` & `wscribe-0.1.1/src/wscribe/backends/fasterwhisper.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 from typing import Any, Mapping, MutableMapping
 
 import numpy as np
 import structlog
 from faster_whisper import WhisperModel  # type: ignore
 from tqdm import tqdm  # type: ignore
 
-from ..core import Backend
+from ..core import Backend, TranscribedData
+from ..writers import format_timestamp
 
 DEFAULT_BEAM = 5
 LOGGER = structlog.get_logger()
-SUPPORTED_MODELS = ["small", "medium", "large-v2"]
+SUPPORTED_MODELS = ["tiny", "small", "medium", "large-v2"]
 
 
 @dataclass(kw_only=True)
 class FasterWhisperBackend(Backend):
     device: str = "cpu"  # cpu, cuda
     quantization: str = "int8"  # int8, float16
     model: WhisperModel | None = None
@@ -35,42 +36,41 @@
             raise RuntimeError(f"model not found in {local_model_path}")
 
     def load(self) -> None:
         self.model = WhisperModel(
             self.model_path(), device=self.device, compute_type=self.quantization
         )
 
-    def transcribe(self, input: np.ndarray) -> Mapping[str, Any]:
+    def transcribe(self, input: np.ndarray) -> list[TranscribedData]:
         """
         Return word level transcription data.
         World level probabities are calculated by ctranslate2.models.Whisper.align
         """
-        result: MutableMapping[str, Any] = {"data": []}
+        result: list[TranscribedData] = []
         assert self.model is not None
         segments, info = self.model.transcribe(
             input,
             beam_size=DEFAULT_BEAM,
             word_timestamps=True,
         )
-        result["language"] = info.language
         with tqdm(total=info.duration, unit_scale=True, unit="playback") as pbar:
             for segment in segments:
                 if segment.words is None:
                     continue
-                segment_extract = {
+                segment_extract: TranscribedData = {
                     "text": segment.text,
                     "start": segment.start,
                     "end": segment.end,
                     "score": round(math.exp(segment.avg_logprob), 2),
                     "words": [
                         {
                             "start": w.start,
                             "end": w.end,
                             "text": w.word,
                             "score": round(w.probability, 2),
                         }
                         for w in segment.words
                     ],
                 }
-                result["data"].append(segment_extract)
+                result.append(segment_extract)
                 pbar.update(segment.end - pbar.last_print_n)
         return result
```

### Comparing `wscribe-0.1.0/src/wscribe/cli/main.py` & `wscribe-0.1.1/src/wscribe/cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 import click
 import structlog
 
 from wscribe.backends.fasterwhisper import FasterWhisperBackend
 from wscribe.sources.local import LocalAudio
 
+from ..writers import WRITERS
+
 LOGGER = structlog.get_logger(ui="cli")
 
 
 @click.group()
 def cli():
     """CLI for audio transcription using faster-whisper"""
     pass
@@ -28,15 +30,15 @@
     nargs=1,
     type=click.Path(exists=False, resolve_path=True),
 )
 @click.option(
     "-f",
     "--format",
     help="destication file format, currently only json is supported",
-    type=click.Choice(["json"], case_sensitive=True),
+    type=click.Choice(list(WRITERS.keys()), case_sensitive=True),
     default="json",
     show_default=True,
 )
 @click.option(
     "-m",
     "--model",
     help="model should already be downloaded",
@@ -61,19 +63,19 @@
 
     device, quantization = ("cuda", "float16") if gpu else ("cpu", "int8")
     m = FasterWhisperBackend(model_size=model, device=device, quantization=quantization)
     m.load()
     log.debug(f"model loaded with {device}-{quantization}")
     audio = LocalAudio(source=source).convert_audio()
     result = m.transcribe(input=audio)
-    with open(destination, "w") as f:
-        json.dump(result, f)
+    writer = WRITERS[format](result=result, destination=destination)
+    writer.write()
 
 
 @cli.command()
 def info():
     """Information about related files and directories"""
-    click.echo(f"Model directory: {os.environ['WSCRIBE_MODELS_DIR']}")
+    click.echo(f"WSCRIBE_MODELS_DIR: {os.environ['WSCRIBE_MODELS_DIR']}")
 
 
 if __name__ == "__main__":
     cli()
```

### Comparing `wscribe-0.1.0/src/wscribe/core.py` & `wscribe-0.1.1/src/wscribe/core.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,31 @@
+from ctypes import Union
 from dataclasses import dataclass
-from typing import Any, Mapping
+from typing import Any, Mapping, TypedDict
 
 import numpy as np
 import structlog
 from faster_whisper.audio import decode_audio  # type: ignore
 
 LOGGER = structlog.get_logger()
 
+WordData = TypedDict(
+    "WordData", {"text": str, "start": float | str, "end": float | str, "score": float}
+)
+TranscribedData = TypedDict(
+    "TranscribedData",
+    {
+        "text": str,
+        "start": float | str,
+        "end": float | str,
+        "score": float,
+        "words": list[WordData],
+    },
+)
+
 
 @dataclass(kw_only=True)
 class Backend:
     name: str = "faster-whisper"
     model_size: str
 
     def __post_init__(self):
@@ -32,15 +47,15 @@
 
     def supported_model_sizes(self) -> list[str]:
         raise NotImplementedError()
 
     def load(self):
         raise NotImplementedError()
 
-    def transcribe(self, input: np.ndarray) -> Mapping[str, Any]:
+    def transcribe(self, input: np.ndarray) -> list[TranscribedData]:
         """
         This should return word level transcription data.
         """
         raise NotImplementedError()
 
 
 @dataclass(kw_only=True)
```

