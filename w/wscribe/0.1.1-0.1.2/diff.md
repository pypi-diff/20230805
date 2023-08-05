# Comparing `tmp/wscribe-0.1.1.tar.gz` & `tmp/wscribe-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wscribe-0.1.1.tar", max compression
+gzip compressed data, was "wscribe-0.1.2.tar", max compression
```

## Comparing `wscribe-0.1.1.tar` & `wscribe-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1074 2023-07-21 09:28:16.650987 wscribe-0.1.1/LICENSE
--rw-r--r--   0        0        0     4960 2023-08-05 15:47:09.725778 wscribe-0.1.1/README.org
--rw-r--r--   0        0        0     1128 2023-08-05 15:57:26.271659 wscribe-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1786 2023-07-25 13:58:47.564422 wscribe-0.1.1/src/wscribe/__init__.py
--rw-r--r--   0        0        0     2576 2023-08-05 07:06:03.013196 wscribe-0.1.1/src/wscribe/backends/fasterwhisper.py
--rw-r--r--   0        0        0     2253 2023-08-05 15:47:09.721778 wscribe-0.1.1/src/wscribe/cli/main.py
--rw-r--r--   0        0        0     2157 2023-08-05 07:10:37.672683 wscribe-0.1.1/src/wscribe/core.py
--rw-r--r--   0        0        0      378 2023-07-25 13:58:47.514422 wscribe-0.1.1/src/wscribe/sources/local.py
--rw-r--r--   0        0        0     3298 2023-08-05 07:17:56.081761 wscribe-0.1.1/src/wscribe/writers.py
--rw-r--r--   0        0        0     5618 1970-01-01 00:00:00.000000 wscribe-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-21 09:28:16.650987 wscribe-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5908 2023-08-05 16:00:55.334063 wscribe-0.1.2/docs/README.md
+-rw-r--r--   0        0        0     1132 2023-08-05 16:02:05.787534 wscribe-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1786 2023-07-25 13:58:47.564422 wscribe-0.1.2/src/wscribe/__init__.py
+-rw-r--r--   0        0        0     2576 2023-08-05 07:06:03.013196 wscribe-0.1.2/src/wscribe/backends/fasterwhisper.py
+-rw-r--r--   0        0        0     2253 2023-08-05 15:47:09.721778 wscribe-0.1.2/src/wscribe/cli/main.py
+-rw-r--r--   0        0        0     2157 2023-08-05 07:10:37.672683 wscribe-0.1.2/src/wscribe/core.py
+-rw-r--r--   0        0        0      378 2023-07-25 13:58:47.514422 wscribe-0.1.2/src/wscribe/sources/local.py
+-rw-r--r--   0        0        0     3298 2023-08-05 07:17:56.081761 wscribe-0.1.2/src/wscribe/writers.py
+-rw-r--r--   0        0        0     6569 1970-01-01 00:00:00.000000 wscribe-0.1.2/PKG-INFO
```

### Comparing `wscribe-0.1.1/LICENSE` & `wscribe-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.1/pyproject.toml` & `wscribe-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
 name = "wscribe"
-version = "0.1.1"
+version = "0.1.2"
 description = "ez audio transcription tool with flexible processing and post-processing options"
 authors = ["Hrishikesh Barman <oss@geekodour.org>"]
 homepage = "https://github.com/geekodour/wscribe"
 license = "MIT"
-readme = "README.org"
+readme = "docs/README.md"
 packages = [{include = "wscribe", from = "src"}]
 
 [tool.poetry.scripts]
 wscribe = "wscribe.cli.main:cli"
 
 [tool.poetry.dependencies]
 # tool.*.group.*.dependencies$ : These can only be installed via poetry
```

### Comparing `wscribe-0.1.1/src/wscribe/__init__.py` & `wscribe-0.1.2/src/wscribe/__init__.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.1/src/wscribe/backends/fasterwhisper.py` & `wscribe-0.1.2/src/wscribe/backends/fasterwhisper.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.1/src/wscribe/cli/main.py` & `wscribe-0.1.2/src/wscribe/cli/main.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.1/src/wscribe/core.py` & `wscribe-0.1.2/src/wscribe/core.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.1/src/wscribe/writers.py` & `wscribe-0.1.2/src/wscribe/writers.py`

 * *Files identical despite different names*

### Comparing `wscribe-0.1.1/PKG-INFO` & `wscribe-0.1.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,97 +1,176 @@
 Metadata-Version: 2.1
 Name: wscribe
-Version: 0.1.1
+Version: 0.1.2
 Summary: ez audio transcription tool with flexible processing and post-processing options
 Home-page: https://github.com/geekodour/wscribe
 License: MIT
 Author: Hrishikesh Barman
 Author-email: oss@geekodour.org
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.6,<9.0.0)
 Requires-Dist: faster-whisper (>=0.7.0,<0.8.0)
 Requires-Dist: structlog (>=23.1.0,<24.0.0)
-Description-Content-Type: text/plain
+Description-Content-Type: text/markdown
+
+
+# Table of Contents
+
+1.  [wscribe](#orgb3cb7b6)
+    1.  [Getting started](#org4bfa46d)
+        1.  [Installation](#org32caff3)
+        2.  [Usage](#org7f7ca72)
+    2.  [Roadmap](#org7e84ad8)
+        1.  [Processing Backends](#orgb5339b4)
+        2.  [Transcription Features](#orga02a040)
+        3.  [Inference interfaces](#org5455504)
+        4.  [Audio sources](#org3caa573)
+        5.  [Distribution](#orgd2b3566)
+    3.  [Contributing](#org9388e9b)
+        1.  [Testing](#org949fef2)
+
+
+<a id="orgb3cb7b6"></a>
+
+# wscribe
+
+
+<a id="org4bfa46d"></a>
+
+## Getting started
+
+`wscribe` is yet another easy to use front-end for [whisper](https://github.com/openai/whisper) specifically for transcription. It aims to be modular so that it can support multiple audio sources, processing backends and inference interfaces. It can run both on CPU and GPU based on the processing backend. Once transcript is generated, editing/correction/visualization of the transcript can be done manually with the [wscribe-editor](https://github.com/geekodour/wscribe-editor).
+
+It was created at [sochara](https://www.sochara.org/) because we have a large volume of audio recordings that need to be transcribed and eventually archived. Another important need was that we needed to verify and manually edit the generated transcript, I could not find any open-source tool that checked all the boxes. Suggested workflow is generating word-level transcript(only supported in `json` export) and then editing the transcript with the [wscribe-editor](https://github.com/geekodour/wscribe-editor).
+
+Currently, it supports the following. Check [roadmap](#org7e84ad8) for upcoming support.
+
+-   Processing backend: [faster-whisper](https://github.com/guillaumekln/faster-whisper)
+-   Audio sources: Local files (Audio/Video)
+-   Inference interfaces: Python CLI
+-   File exports: JSON, SRT, WebVTT
+
+
+<a id="org32caff3"></a>
+
+### Installation
+
+These instructions were tested on `NixOS:Python3.10` and `ArchLinux:Python3.10` but should work for any other OS, if you face any installation issues please feel free to [create issues](https://github.com/geekodour/wscribe/issues). I&rsquo;ll try to put out a docker image sometime.
+
+1.  1. Set required env var
+
+    -   `WSCRIBE_MODELS_DIR` : Path to the directory where whisper models should be downloaded to.
+    
+        export WSCRIBE_MODELS_DIR=$XDG_DATA_HOME/whisper-models # example
+
+2.  2. Download the models
+
+    1.  Recommended
+    
+        -   Recommended way for downloading the models is to use the [helper script](https://github.com/geekodour/wscribe/blob/main/scripts/fw_dw_hf_wo_lfs.sh), it&rsquo;ll download the models to `WSCRIBE_MODELS_DIR`.
+            
+                cd /tmp # temporary script, only needed to download the models
+                curl https://raw.githubusercontent.com/geekodour/wscribe/main/scripts/fw_dw_hf_wo_lfs.sh
+                chmod u+x fw_dw_hf_wo_lfs.sh
+                ./fw_dw_hf_wo_lfs.sh tiny # other models: tiny, small, medium and large-v2
+    
+    2.  Manual
+    
+        You can download the models directly [from here](https://huggingface.co/guillaumekln) using `git lfs`, make sure you download/copy them to `WSCRIBE_MODELS_DIR`
+
+3.  3. Install wscribe
+
+    Assuming you already have a working `python>=3.10` setup
+    
+        pip install wscribe
+
+
+<a id="org7f7ca72"></a>
+
+### Usage
+
+    # wscribe transcribe [OPTIONS] SOURCE DESTINATION
+    
+    # cpu
+    wscribe transcribe audio.mp3 transcription.json
+    # use gpu
+    wscribe transcribe video.mp4 transcription.json --gpu
+    # use gpu, srt format
+    wscribe transcribe video.mp4 transcription.srt -g -f srt
+    # use gpu, srt format, tiny model
+    wscribe transcribe video.mp4 transcription.vtt -g -f vtt -m tiny
+    wscribe transcribe --help # all help info
+
+
+<a id="org7e84ad8"></a>
+
+## Roadmap
+
+
+<a id="orgb5339b4"></a>
+
+### Processing Backends
+
+-   [X] [faster-whisper](https://github.com/guillaumekln/faster-whisper)
+-   [ ] [whisper.cpp](https://github.com/ggerganov/whisper.cpp), also see [this explanation about the speed difference](https://github.com/ggerganov/whisper.cpp/issues/1127).
+-   [ ] [WhisperX](https://github.com/m-bain/whisperX), diarization is something to look forward to
+
+
+<a id="orga02a040"></a>
+
+### Transcription Features
+
+-   [ ] Add support for [diarization](https://github.com/guillaumekln/faster-whisper/issues/303)
+-   [ ] Add VAD/other de-noising stuff etc.
+-   [ ] Add local llm integration with [llama.cpp](https://github.com/ggerganov/llama.cpp/pull/1773) or something similar for summary and [othe possible things](https://news.ycombinator.com/item?id=36900294). It can be also used to generate more accurate transcript. Whisper mostly generates sort of a subtitle, for converting subtitle into transcription we need to group the subtitle. This can be done in various ways. Eg. By speaker if diarization is supported, by time chunks etc. By using LLMs or maybe other NLP techniques we&rsquo;ll also be able to do this with things like break in dialogue etc. Have to explore.
+
+
+<a id="org5455504"></a>
+
+### Inference interfaces
+
+-   [-] Python CLI
+    -   [X] Basic CLI
+    -   [ ] Improve summary statistics
+-   [ ] REST endpoint
+    -   [ ] Basic server to run wscribe via an API.
+    -   [ ] Possibly add glue code to expose it via CFtunnels or something similar
+
+
+<a id="org3caa573"></a>
+
+### Audio sources
+
+-   [X] Local files
+-   [ ] Youtube
+-   [ ] Google drive
+
+
+<a id="orgd2b3566"></a>
+
+### Distribution
+
+-   [X] Python packaging
+-   [ ] Docker/Podman
+-   [ ] Package for Nix
+-   [ ] Package for Arch(AUR)
+
+
+<a id="org9388e9b"></a>
+
+## Contributing
 
-* wscribe
-** Getting started
-~wscribe~ is yet another easy to use front-end for [[https://github.com/openai/whisper][whisper]] specifically for transcription. It aims to be modular so that it can support multiple audio sources, processing backends and inference interfaces. It can run both on CPU and GPU based on the processing backend. Once transcript is generated, editing/correction/visualization of the transcript can be done manually with the [[https://github.com/geekodour/wscribe-editor][wscribe-editor]].
-
-It was created at [[https://www.sochara.org/][sochara]] because we have a large volume of audio recordings that need to be transcribed and eventually archived. Another important need was that we needed to verify and manually edit the generated transcript, I could not find any open-source tool that checked all the boxes. Suggested workflow is generating word-level transcript(only supported in ~json~ export) and then editing the transcript with the [[https://github.com/geekodour/wscribe-editor][wscribe-editor]].
-
-Currently, it supports the following. Check [[*Roadmap][roadmap]] for upcoming support.
-- Processing backend: [[https://github.com/guillaumekln/faster-whisper][faster-whisper]]
-- Audio sources: Local files (Audio/Video)
-- Inference interfaces: Python CLI
-- File exports: JSON, SRT, WebVTT
-*** Installation
-These instructions were tested on ~NixOS:Python3.10~ and ~ArchLinux:Python3.10~ but should work for any other OS, if you face any installation issues please feel free to [[https://github.com/geekodour/wscribe/issues][create issues]]. I'll try to put out a docker image sometime.
-**** 1. Set required env var
-- ~WSCRIBE_MODELS_DIR~ : Path to the directory where whisper models should be downloaded to.
-#+begin_src bash
-export WSCRIBE_MODELS_DIR=$XDG_DATA_HOME/whisper-models # example
-#+end_src
-**** 2. Download the models
-***** Recommended
-- Recommended way for downloading the models is to use the [[https://github.com/geekodour/wscribe/blob/main/scripts/fw_dw_hf_wo_lfs.sh][helper script]], it'll download the models to ~WSCRIBE_MODELS_DIR~.
-  #+begin_src shell
-cd /tmp # temporary script, only needed to download the models
-curl https://raw.githubusercontent.com/geekodour/wscribe/main/scripts/fw_dw_hf_wo_lfs.sh
-chmod u+x fw_dw_hf_wo_lfs.sh
-./fw_dw_hf_wo_lfs.sh tiny # other models: tiny, small, medium and large-v2
-  #+end_src
-***** Manual
-You can download the models directly [[https://huggingface.co/guillaumekln][from here]] using ~git lfs~, make sure you download/copy them to ~WSCRIBE_MODELS_DIR~
-**** 3. Install wscribe
-Assuming you already have a working ~python>=3.10~ setup
-#+begin_src shell
-pip install wscribe
-#+end_src
-*** Usage
-#+begin_src shell
-# wscribe transcribe [OPTIONS] SOURCE DESTINATION
-
-# cpu
-wscribe transcribe audio.mp3 transcription.json
-# use gpu
-wscribe transcribe video.mp4 transcription.json --gpu
-# use gpu, srt format
-wscribe transcribe video.mp4 transcription.srt -g -f srt
-# use gpu, srt format, tiny model
-wscribe transcribe video.mp4 transcription.vtt -g -f vtt -m tiny
-wscribe transcribe --help # all help info
-#+end_src
-** Roadmap
-*** Processing Backends
-- [X] [[https://github.com/guillaumekln/faster-whisper][faster-whisper]]
-- [ ] [[https://github.com/ggerganov/whisper.cpp][whisper.cpp]], also see [[https://github.com/ggerganov/whisper.cpp/issues/1127][this explanation about the speed difference]].
-- [ ] [[https://github.com/m-bain/whisperX][WhisperX]], diarization is something to look forward to
-*** Transcription Features
-  - [ ] Add support for [[https://github.com/guillaumekln/faster-whisper/issues/303][diarization]]
-  - [ ] Add VAD/other de-noising stuff etc.
-  - [ ] Add local llm integration with [[https://github.com/ggerganov/llama.cpp/pull/1773][llama.cpp]] or something similar for summary and [[https://news.ycombinator.com/item?id=36900294][othe possible things]]. It can be also used to generate more accurate transcript. Whisper mostly generates sort of a subtitle, for converting subtitle into transcription we need to group the subtitle. This can be done in various ways. Eg. By speaker if diarization is supported, by time chunks etc. By using LLMs or maybe other NLP techniques we'll also be able to do this with things like break in dialogue etc. Have to explore.
-*** Inference interfaces
-- [-] Python CLI
-  - [X] Basic CLI
-  - [ ] Improve summary statistics
-- [ ] REST endpoint
-  - [ ] Basic server to run wscribe via an API.
-  - [ ] Possibly add glue code to expose it via CFtunnels or something similar
-*** Audio sources
-- [X] Local files
-- [ ] Youtube
-- [ ] Google drive
-*** Distribution
-- [X] Python packaging
-- [ ] Docker/Podman
-- [ ] Package for Nix
-- [ ] Package for Arch(AUR)
-** Contributing
 All contribution happens through PRs, any contributions is greatly appreciated, bugfixes are welcome, features are welcome, tests are welcome, suggestions & criticism are welcome.
-*** Testing
-- ~make test~
-- See other helper commands in ~Makefile~
+
+
+<a id="org949fef2"></a>
+
+### Testing
+
+-   `make test`
+-   See other helper commands in `Makefile`
+
```

