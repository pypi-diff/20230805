# Comparing `tmp/stable-ts-2.7.2.tar.gz` & `tmp/stable-ts-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stable-ts-2.7.2.tar", last modified: Fri Jul 28 23:47:54 2023, max compression
+gzip compressed data, was "stable-ts-2.8.0.tar", last modified: Fri Aug  4 23:53:52 2023, max compression
```

## Comparing `stable-ts-2.7.2.tar` & `stable-ts-2.8.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 23:47:54.101724 stable-ts-2.7.2/
--rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.7.2/LICENSE
--rw-rw-rw-   0        0        0    11472 2023-07-28 23:47:54.101724 stable-ts-2.7.2/PKG-INFO
--rw-rw-rw-   0        0        0    11176 2023-07-20 19:47:30.000000 stable-ts-2.7.2/README.md
--rw-rw-rw-   0        0        0       42 2023-07-28 23:47:54.102725 stable-ts-2.7.2/setup.cfg
--rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.7.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 23:47:54.033451 stable-ts-2.7.2/stable_ts.egg-info/
--rw-rw-rw-   0        0        0    11472 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      627 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      110 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-07-28 23:47:53.000000 stable-ts-2.7.2/stable_ts.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-28 23:47:54.098722 stable-ts-2.7.2/stable_whisper/
--rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.7.2/stable_whisper/__init__.py
--rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.7.2/stable_whisper/__main__.py
--rw-rw-rw-   0        0        0       23 2023-07-28 23:15:11.000000 stable-ts-2.7.2/stable_whisper/_version.py
--rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.7.2/stable_whisper/audio.py
--rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.7.2/stable_whisper/decode.py
--rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.7.2/stable_whisper/enhancement.py
--rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.7.2/stable_whisper/non_whisper.py
--rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.7.2/stable_whisper/quantization.py
--rw-rw-rw-   0        0        0    43529 2023-07-28 23:22:16.000000 stable-ts-2.7.2/stable_whisper/result.py
--rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.7.2/stable_whisper/stabilization.py
--rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.7.2/stable_whisper/text_output.py
--rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.7.2/stable_whisper/timing.py
--rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.7.2/stable_whisper/video_output.py
--rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.7.2/stable_whisper/whisper_word_level.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:53:52.779855 stable-ts-2.8.0/
+-rw-rw-rw-   0        0        0     1082 2022-11-20 18:10:26.000000 stable-ts-2.8.0/LICENSE
+-rw-rw-rw-   0        0        0    11471 2023-08-04 23:53:52.778854 stable-ts-2.8.0/PKG-INFO
+-rw-rw-rw-   0        0        0    11175 2023-08-04 23:35:49.000000 stable-ts-2.8.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-08-04 23:53:52.779855 stable-ts-2.8.0/setup.cfg
+-rw-rw-rw-   0        0        0     1100 2023-03-25 19:12:43.000000 stable-ts-2.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 23:53:52.701853 stable-ts-2.8.0/stable_ts.egg-info/
+-rw-rw-rw-   0        0        0    11471 2023-08-04 23:53:52.000000 stable-ts-2.8.0/stable_ts.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      627 2023-08-04 23:53:52.000000 stable-ts-2.8.0/stable_ts.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 23:53:52.000000 stable-ts-2.8.0/stable_ts.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2023-08-04 23:53:52.000000 stable-ts-2.8.0/stable_ts.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      110 2023-08-04 23:53:52.000000 stable-ts-2.8.0/stable_ts.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-08-04 23:53:52.000000 stable-ts-2.8.0/stable_ts.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-04 23:53:52.776854 stable-ts-2.8.0/stable_whisper/
+-rw-rw-rw-   0        0        0      241 2023-07-13 00:23:52.000000 stable-ts-2.8.0/stable_whisper/__init__.py
+-rw-rw-rw-   0        0        0       44 2023-02-15 00:11:21.000000 stable-ts-2.8.0/stable_whisper/__main__.py
+-rw-rw-rw-   0        0        0       23 2023-08-04 23:35:49.000000 stable-ts-2.8.0/stable_whisper/_version.py
+-rw-rw-rw-   0        0        0     8360 2023-07-13 00:08:53.000000 stable-ts-2.8.0/stable_whisper/audio.py
+-rw-rw-rw-   0        0        0     4373 2023-04-24 04:50:11.000000 stable-ts-2.8.0/stable_whisper/decode.py
+-rw-rw-rw-   0        0        0    15934 2023-04-28 16:52:08.000000 stable-ts-2.8.0/stable_whisper/enhancement.py
+-rw-rw-rw-   0        0        0    12947 2023-07-13 00:22:18.000000 stable-ts-2.8.0/stable_whisper/non_whisper.py
+-rw-rw-rw-   0        0        0     1645 2023-05-03 19:33:54.000000 stable-ts-2.8.0/stable_whisper/quantization.py
+-rw-rw-rw-   0        0        0    45144 2023-08-04 23:46:16.000000 stable-ts-2.8.0/stable_whisper/result.py
+-rw-rw-rw-   0        0        0    14128 2023-07-12 23:15:05.000000 stable-ts-2.8.0/stable_whisper/stabilization.py
+-rw-rw-rw-   0        0        0    20528 2023-05-08 02:53:22.000000 stable-ts-2.8.0/stable_whisper/text_output.py
+-rw-rw-rw-   0        0        0    10370 2023-04-24 04:57:46.000000 stable-ts-2.8.0/stable_whisper/timing.py
+-rw-rw-rw-   0        0        0     2265 2023-03-17 01:46:33.000000 stable-ts-2.8.0/stable_whisper/video_output.py
+-rw-rw-rw-   0        0        0    53252 2023-07-13 00:20:47.000000 stable-ts-2.8.0/stable_whisper/whisper_word_level.py
```

### Comparing `stable-ts-2.7.2/LICENSE` & `stable-ts-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/PKG-INFO` & `stable-ts-2.8.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.7.2
+Version: 2.8.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -133,32 +133,32 @@
 # The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
-    .merge_by_gap(.15, max_words=3)
+    .merge_by_gap(.3, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
+result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L877-L924)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L685-L697)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L738-L749)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L799-L815)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L709-L727)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L761-L779)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L786-L788)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L827-L844)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L908-L956)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L705-L717)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L758-L769)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L820-L839)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L729-L747)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L781-L799)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L806-L808)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L858-L875)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -173,15 +173,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L969-L985)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L999-L1015)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.7.2/README.md` & `stable-ts-2.8.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -122,32 +122,32 @@
 # The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
-    .merge_by_gap(.15, max_words=3)
+    .merge_by_gap(.3, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
+result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L877-L924)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L685-L697)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L738-L749)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L799-L815)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L709-L727)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L761-L779)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L786-L788)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L827-L844)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L908-L956)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L705-L717)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L758-L769)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L820-L839)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L729-L747)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L781-L799)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L806-L808)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L858-L875)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -162,15 +162,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L969-L985)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L999-L1015)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.7.2/setup.py` & `stable-ts-2.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_ts.egg-info/PKG-INFO` & `stable-ts-2.8.0/stable_ts.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stable-ts
-Version: 2.7.2
+Version: 2.8.0
 Summary: Modifies OpenAI's Whisper to produce more reliable timestamps.
 Home-page: https://github.com/jianfch/stable-ts
 Author: Jian
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -133,32 +133,32 @@
 # The following all functionally equivalent:
 result0 = model.transcribe('audio.mp3', regroup=True) # regroup is True by default
 result1 = model.transcribe('audio.mp3', regroup=False)
 (
     result1
     .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
     .split_by_gap(.5)
-    .merge_by_gap(.15, max_words=3)
+    .merge_by_gap(.3, max_words=3)
     .split_by_punctuation([('.', ' '), '。', '?', '？'])
 )
-result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.15+3_sp=.* /。/?/？')
+result2 = model.transcribe('audio.mp3', regroup='sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？')
 
 # To undo all regrouping operations:
 result0.reset()
 ```
 Any regrouping algorithm can be expressed as a string. Please feel free share your strings [here](https://github.com/jianfch/stable-ts/discussions/162)
 #### Regrouping Methods
-- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L877-L924)
-- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L685-L697)
-- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L738-L749)
-- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L799-L815)
-- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L709-L727)
-- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L761-L779)
-- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L786-L788)
-- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L827-L844)
+- [regroup()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L908-L956)
+- [split_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L705-L717)
+- [split_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L758-L769)
+- [split_by_length()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L820-L839)
+- [merge_by_gap()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L729-L747)
+- [merge_by_punctuation()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L781-L799)
+- [merge_all_segments()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L806-L808)
+- [clamp_max()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L858-L875)
 
 ### Locating Words
 You can locate words with regular expression.
 ```python
 # Find every sentence that contains "and"
 matches = result.find(r'[^.]+and[^.]+\.')
 # print the all matches if there are any
@@ -173,15 +173,15 @@
 for match in matches:
   print(f'match: {match.text_match}\n'
         f'text: {match.text}\n'
         f'start: {match.start}\n'
         f'end: {match.end}\n')
 ```
 Parameters: 
-[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L969-L985)
+[find()](https://github.com/jianfch/stable-ts/blob/main/stable_whisper/result.py#L999-L1015)
 
 ### Boosting Performance
 * One of the methods that Stable-ts uses to increase timestamp accuracy 
 and reduce hallucinations is silence suppression, enabled with `suppress_silence=True` (default).
 This method essentially suppresses the timestamps where the audio is silent or contain no speech
 by suppressing the corresponding tokens during inference and also readjusting the timestamps after inference. 
 To figure out which parts of the audio track are silent or contain no speech, Stable-ts supports non-VAD and VAD methods.
```

### Comparing `stable-ts-2.7.2/stable_ts.egg-info/SOURCES.txt` & `stable-ts-2.8.0/stable_ts.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/audio.py` & `stable-ts-2.8.0/stable_whisper/audio.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/decode.py` & `stable-ts-2.8.0/stable_whisper/decode.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/enhancement.py` & `stable-ts-2.8.0/stable_whisper/enhancement.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/non_whisper.py` & `stable-ts-2.8.0/stable_whisper/non_whisper.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/quantization.py` & `stable-ts-2.8.0/stable_whisper/quantization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/result.py` & `stable-ts-2.8.0/stable_whisper/result.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,34 +396,54 @@
             else:
                 ending, beginning = p
                 indices.extend([i for i, (w0, w1) in enumerate(zip(self.words[:-1], self.words[1:]))
                                 if w0.word.endswith(ending) and w1.word.startswith(beginning)])
 
         return sorted(set(indices) - set(self.get_locked_indices()))
 
-    def get_length_indices(self, max_chars: int = None, max_words: int = None):  # for splitting
+    def get_length_indices(self, max_chars: int = None, max_words: int = None, even_split: bool = True):
+        # for splitting
         if max_chars is None and max_words is None:
             return []
         assert max_chars != 0 and max_words != 0, \
             f'max_chars and max_words must be greater 0, but got {max_chars} and {max_words}'
         indices = []
-        curr_words = 0
-        curr_chars = 0
-        for i, word in enumerate(self.words):
-            curr_words += 1
-            curr_chars += len(word)
-            if i != 0:
-                if (
-                        max_chars is not None and curr_chars > max_chars
-                        or
-                        max_words is not None and curr_words > max_words
-                ):
-                    indices.append(i-1)
-                    curr_words = 1
-                    curr_chars = len(word)
+        if even_split:
+            char_count = -1 if max_chars is None else sum(map(len, self.words))
+            word_count = -1 if max_words is None else len(self.words)
+            exceed_chars = max_chars is not None and char_count > max_chars
+            exceed_words = max_words is not None and word_count > max_words
+            if exceed_chars:
+                splits = np.ceil(char_count / max_chars)
+                chars_per_split = char_count / splits
+                char_indices = list(chain.from_iterable([i]*len(word) for i, word in enumerate(self.words)))
+                indices = [char_indices[round(i * chars_per_split)] - 1 for i in range(1, int(splits))]
+                if max_words is not None:
+                    exceed_words = any(j-i+1 > max_words for i, j in zip([0]+indices, indices+[len(self.words)]))
+
+            if exceed_words:
+                splits = np.ceil(word_count / max_words)
+                words_per_split = word_count / splits
+                indices = [round(i*words_per_split)-1 for i in range(1, int(splits))]
+
+        else:
+            curr_words = 0
+            curr_chars = 0
+            for i, word in enumerate(self.words):
+                curr_words += 1
+                curr_chars += len(word)
+                if i != 0:
+                    if (
+                            max_chars is not None and curr_chars > max_chars
+                            or
+                            max_words is not None and curr_words > max_words
+                    ):
+                        indices.append(i-1)
+                        curr_words = 1
+                        curr_chars = len(word)
         return indices
 
     def split(self, indices: List[int]):
         if len(indices) == 0:
             return []
         if indices[-1] != len(self.words) - 1:
             indices.append(len(self.words) - 1)
@@ -789,45 +809,56 @@
         self._merge_segments(list(range(len(self.segments) - 1)))
         return self
 
     def split_by_length(
             self,
             max_chars: int = None,
             max_words: int = None,
+            even_split: bool = True,
             force_len: bool = False,
             lock: bool = False
     ):
         """
 
         Split (in-place) any segment in segments that do not exceed the specified length
 
         Parameters
         ----------
         max_chars: int
             Maximum number of character allowed in each segment.
         max_words: int
             Maximum number of words allowed in each segment.
+        even_split: bool
+            Whether to evenly split a segment in length if it exceeds [max_chars] or [max_words]. (Default: True)
+            Note that some segments might still slightly exceed [max_chars] to avoid uneven splits.
         force_len: bool
-            Maintain a relatively constant length for each segment. (Default: False)
+            Whether to force a constant length for each segment except the last segment. (Default: False)
             This will ignore all previous non-locked segment boundaries (e.g. boundaries set by `regroup()`).
         lock: bool
             Whether to prevent future splits/merges from altering changes made by this method. (Default: False)
 
         """
         if force_len:
             self.merge_all_segments()
-        self._split_segments(lambda x: x.get_length_indices(max_chars=max_chars, max_words=max_words), lock=lock)
+        self._split_segments(
+            lambda x: x.get_length_indices(
+                max_chars=max_chars,
+                max_words=max_words,
+                even_split=even_split
+            ),
+            lock=lock
+        )
         return self
 
     def clamp_max(
             self,
             medium_factor: float = 2.5,
             max_dur: float = None,
             clip_start: bool = None,
-            verbose: bool = True):
+            verbose: bool = False):
         """
 
         Clamp all word durations above certain value.
 
         Parameters
         ----------
         medium_factor: float
@@ -877,24 +908,25 @@
         """
 
         Regroup (in-place) all words into segments with more natural boundaries without locking.
 
         Parameters
         ----------
         regroup_algo: str
-            string for customizing the regrouping algorithm
+            string for customizing the regrouping algorithm (default: 'da')
 
                 Method keys:
                     sg: split_by_gap
                     sp: split_by_punctuation
                     sl: split_by_length
                     mg: merge_by_gap
                     mp: merge_by_punctuation
                     ms: merge_all_segment
                     cm: clamp_max
+                    da: default algorithm (sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？)
 
                 Metacharacters:
                     = separates a method key and its arguments (not used if no argument)
                     _ separates method keys (after arguments if there are any)
                     + separates arguments for a method key
                     / separates an argument into list of strings
                     * separates an item in list of strings into a nested list of strings
@@ -918,57 +950,55 @@
 
         verbose: bool
             whether to show all the methods and arguments parsed from [regroup_algo]
         only_show: bool
             show the all methods and arguments parsed from [regroup_algo] without running the methods
 
         """
-        if isinstance(regroup_algo, str):
-            methods = dict(
-                sg=self.split_by_gap,
-                sp=self.split_by_punctuation,
-                sl=self.split_by_length,
-                mg=self.merge_by_gap,
-                mp=self.merge_by_punctuation,
-                ms=self.merge_all_segments,
-                cm=self.clamp_max
-            )
-
-            def _to_arg(x: str):
-                if len(x) == 0:
-                    return None
-                if '/' in x:
-                    return [a.split('*') if '*' in a else a for a in x.split('/')]
-                try:
-                    x = float(x) if '.' in x else int(x)
-                except ValueError:
-                    pass
-                finally:
-                    return x
-
-            for method in regroup_algo.split('_'):
-                method, args = method.split('=', maxsplit=1) if '=' in method else (method, '')
-                if method not in methods:
-                    raise NotImplementedError(f'{method} is not one of the available methods: {tuple(methods.keys())}')
-                args = [] if len(args) == 0 else list(map(_to_arg, args.split('+')))
-                if verbose or only_show:
-                    print(f'{methods[method].__name__}({", ".join(map(str, args))})')
-                if not only_show:
-                    methods[method](*args)
-
-            return self
+        if regroup_algo is None:
+            regroup_algo = 'da'
 
-        return (
-            self
-            .split_by_punctuation([('.', ' '), '。', '?', '？', ',', '，'])
-            .split_by_gap(.5)
-            .merge_by_gap(.3, max_words=3)
-            .split_by_punctuation([('.', ' '), '。', '?', '？'])
+        methods = dict(
+            sg=self.split_by_gap,
+            sp=self.split_by_punctuation,
+            sl=self.split_by_length,
+            mg=self.merge_by_gap,
+            mp=self.merge_by_punctuation,
+            ms=self.merge_all_segments,
+            cm=self.clamp_max
         )
 
+        def _to_arg(x: str):
+            if len(x) == 0:
+                return None
+            if '/' in x:
+                return [a.split('*') if '*' in a else a for a in x.split('/')]
+            try:
+                x = float(x) if '.' in x else int(x)
+            except ValueError:
+                pass
+            finally:
+                return x
+
+        calls = regroup_algo.split('_')
+        if 'da' in calls:
+            default_calls = 'sp=.* /。/?/？/,/，_sg=.5_mg=.3+3_sp=.* /。/?/？'.split('_')
+            calls = chain.from_iterable(default_calls if method == 'da' else [method] for method in calls)
+        for method in calls:
+            method, args = method.split('=', maxsplit=1) if '=' in method else (method, '')
+            if method not in methods:
+                raise NotImplementedError(f'{method} is not one of the available methods: {tuple(methods.keys())}')
+            args = [] if len(args) == 0 else list(map(_to_arg, args.split('+')))
+            if verbose or only_show:
+                print(f'{methods[method].__name__}({", ".join(map(str, args))})')
+            if not only_show:
+                methods[method](*args)
+
+        return self
+
     def find(self, pattern: str, word_level=True, flags=None) -> "WhisperResultMatches":
         """
 
         Find segments/words and timestamps with regular expression.
 
         Parameters
         ----------
```

### Comparing `stable-ts-2.7.2/stable_whisper/stabilization.py` & `stable-ts-2.8.0/stable_whisper/stabilization.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/text_output.py` & `stable-ts-2.8.0/stable_whisper/text_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/timing.py` & `stable-ts-2.8.0/stable_whisper/timing.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/video_output.py` & `stable-ts-2.8.0/stable_whisper/video_output.py`

 * *Files identical despite different names*

### Comparing `stable-ts-2.7.2/stable_whisper/whisper_word_level.py` & `stable-ts-2.8.0/stable_whisper/whisper_word_level.py`

 * *Files identical despite different names*

