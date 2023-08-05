# Comparing `tmp/iman-0.0.95.tar.gz` & `tmp/iman-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\iman-0.0.95.tar", last modified: Sat Aug  5 09:37:32 2023, max compression
+gzip compressed data, was "dist\iman-0.0.96.tar", last modified: Sat Aug  5 09:42:08 2023, max compression
```

## Comparing `iman-0.0.95.tar` & `iman-0.0.96.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/
--rw-rw-rw-   0        0        0     6983 2023-08-05 09:37:32.000000 iman-0.0.95/PKG-INFO
--rw-rw-rw-   0        0        0     6609 2023-08-05 09:37:11.000000 iman-0.0.95/README.rst
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:31.000000 iman-0.0.95/iman/
--rw-rw-rw-   0        0        0     2070 2022-12-25 10:45:05.000000 iman-0.0.95/iman/AUG.py
--rw-rw-rw-   0        0        0    18503 2023-08-05 08:31:04.000000 iman-0.0.95/iman/Audio.py
--rw-rw-rw-   0        0        0      124 2023-01-29 08:15:58.000000 iman-0.0.95/iman/Boors.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:31.000000 iman-0.0.95/iman/Features/
--rw-rw-rw-   0        0        0       42 2022-11-13 07:01:23.000000 iman-0.0.95/iman/Features/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/Features/mfcc/
--rw-rw-rw-   0        0        0     2836 2022-11-13 07:05:02.000000 iman-0.0.95/iman/Features/mfcc/LS.py
--rw-rw-rw-   0        0        0      604 2022-12-12 11:32:38.000000 iman-0.0.95/iman/Features/mfcc/SB.py
--rw-rw-rw-   0        0        0        0 2022-11-13 06:42:54.000000 iman-0.0.95/iman/Features/mfcc/__init__.py
--rw-rw-rw-   0        0        0    11080 2021-12-01 10:31:39.000000 iman-0.0.95/iman/Features/mfcc/getmfcc_from_librosa.py
--rw-rw-rw-   0        0        0    41655 2022-12-12 11:33:13.000000 iman-0.0.95/iman/Features/mfcc/sb_mfcc_class.py
--rw-rw-rw-   0        0        0     1057 2022-12-25 10:05:56.000000 iman-0.0.95/iman/Image.py
--rw-rw-rw-   0        0        0      815 2022-12-20 06:25:42.000000 iman-0.0.95/iman/Report.py
--rw-rw-rw-   0        0        0     2640 2023-02-20 05:13:55.000000 iman-0.0.95/iman/Text.py
--rw-rw-rw-   0        0        0     4478 2023-07-22 04:52:36.000000 iman-0.0.95/iman/__init__.py
--rw-rw-rw-   0        0        0      686 2022-12-17 11:18:42.000000 iman-0.0.95/iman/examples.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/examples_folder/
--rw-rw-rw-   0        0        0        0 2022-12-17 11:24:05.000000 iman-0.0.95/iman/examples_folder/__init__.py
--rw-rw-rw-   0        0        0      539 2023-01-01 11:18:41.000000 iman-0.0.95/iman/examples_folder/age.py
--rw-rw-rw-   0        0        0      100 2023-01-01 05:01:21.000000 iman-0.0.95/iman/examples_folder/ffmpeg.py
--rw-rw-rw-   0        0        0      490 2022-12-17 09:55:52.000000 iman-0.0.95/iman/examples_folder/flask.py
--rw-rw-rw-   0        0        0      262 2021-01-05 11:07:03.000000 iman-0.0.95/iman/examples_folder/gpu_allocate_tf.py
--rw-rw-rw-   0        0        0      299 2022-12-31 09:42:30.000000 iman-0.0.95/iman/examples_folder/graphviz_chart.py
--rw-rw-rw-   0        0        0      345 2022-12-17 11:09:10.000000 iman-0.0.95/iman/examples_folder/parallel.py
--rw-rw-rw-   0        0        0      217 2022-12-17 11:12:20.000000 iman-0.0.95/iman/examples_folder/post_by_python.py
--rw-rw-rw-   0        0        0      775 2019-12-03 03:31:26.000000 iman-0.0.95/iman/examples_folder/pyworldd.py
--rw-rw-rw-   0        0        0      406 2022-12-05 05:24:04.000000 iman-0.0.95/iman/examples_folder/queue_worker.py
--rw-rw-rw-   0        0        0     1607 2021-11-28 10:10:27.000000 iman-0.0.95/iman/examples_folder/save_docx.py
--rw-rw-rw-   0        0        0      478 2019-05-05 06:27:38.000000 iman-0.0.95/iman/examples_folder/stft_test.py
--rw-rw-rw-   0        0        0      276 2019-11-19 00:37:16.000000 iman-0.0.95/iman/examples_folder/threading_example.py
--rw-rw-rw-   0        0        0      454 2021-05-25 08:55:10.000000 iman-0.0.95/iman/examples_folder/wikipedia.py
--rw-rw-rw-   0        0        0    15323 2022-11-06 10:39:16.000000 iman-0.0.95/iman/gpu_info.py
--rw-rw-rw-   0        0        0     1862 2022-11-12 05:34:50.000000 iman-0.0.95/iman/info.py
--rw-rw-rw-   0        0        0      318 2022-11-08 10:24:41.000000 iman-0.0.95/iman/matlab.py
--rw-rw-rw-   0        0        0     3422 2022-12-26 10:35:15.000000 iman-0.0.95/iman/metrics.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/num2fa/
--rw-rw-rw-   0        0        0     8938 2023-01-28 05:46:54.000000 iman-0.0.95/iman/num2fa/__init__.py
--rw-rw-rw-   0        0        0      506 2023-01-28 05:46:54.000000 iman-0.0.95/iman/num2fa/__main__.py
--rw-rw-rw-   0        0        0      237 2022-12-19 06:23:20.000000 iman-0.0.95/iman/par.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/pyctcdecode/
--rw-rw-rw-   0        0        0      265 2023-07-11 05:28:53.000000 iman-0.0.95/iman/pyctcdecode/__init__.py
--rw-rw-rw-   0        0        0     6186 2023-07-11 05:28:53.000000 iman-0.0.95/iman/pyctcdecode/alphabet.py
--rw-rw-rw-   0        0        0      617 2023-07-11 05:28:53.000000 iman-0.0.95/iman/pyctcdecode/constants.py
--rw-rw-rw-   0        0        0    29784 2023-07-19 12:40:28.000000 iman-0.0.95/iman/pyctcdecode/decoder.py
--rw-rw-rw-   0        0        0    11420 2023-07-11 05:28:53.000000 iman-0.0.95/iman/pyctcdecode/language_model.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/sad_tf/
--rw-rw-rw-   0        0        0      101 2023-07-23 07:12:34.000000 iman-0.0.95/iman/sad_tf/__init__.py
--rw-rw-rw-   0        0        0     5963 2023-08-05 08:55:48.000000 iman-0.0.95/iman/sad_tf/export_funcs.py
--rw-rw-rw-   0        0        0     2221 2023-07-05 11:06:11.000000 iman-0.0.95/iman/sad_tf/features.py
--rw-rw-rw-   0        0        0    19052 2023-08-05 09:25:39.000000 iman-0.0.95/iman/sad_tf/segmenter.py
--rw-rw-rw-   0        0        0    20025 2023-07-23 08:03:31.000000 iman-0.0.95/iman/sad_tf/segmentero.py
--rw-rw-rw-   0        0        0    13783 2022-11-30 10:00:38.000000 iman-0.0.95/iman/sad_tf/sidekit_mfcc.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.95/iman/sad_tf/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.95/iman/sad_tf/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.95/iman/sad_tf/viterbi_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/sad_torch_mfcc/
--rw-rw-rw-   0        0        0      107 2022-12-26 10:21:43.000000 iman-0.0.95/iman/sad_torch_mfcc/__init__.py
--rw-rw-rw-   0        0        0     4645 2022-12-11 08:33:44.000000 iman-0.0.95/iman/sad_torch_mfcc/export_funcs.py
--rw-rw-rw-   0        0        0     2002 2023-07-05 11:08:54.000000 iman-0.0.95/iman/sad_torch_mfcc/features.py
--rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.95/iman/sad_torch_mfcc/sad_model.py
--rw-rw-rw-   0        0        0    19324 2023-07-22 04:57:05.000000 iman-0.0.95/iman/sad_torch_mfcc/segmenter.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.95/iman/sad_torch_mfcc/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.95/iman/sad_torch_mfcc/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.95/iman/sad_torch_mfcc/viterbi_utils.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:32.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/
--rw-rw-rw-   0        0        0       36 2023-07-26 06:11:13.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/__init__.py
--rw-rw-rw-   0        0        0      631 2023-07-26 06:41:32.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/features.py
--rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/sad_model.py
--rw-rw-rw-   0        0        0    10232 2023-07-26 07:10:07.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/segmenter.py
--rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/thread_returning.py
--rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/viterbi.py
--rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.95/iman/sad_torch_mfcc_speaker/viterbi_utils.py
--rw-rw-rw-   0        0        0      422 2022-11-22 05:36:39.000000 iman-0.0.95/iman/tsne.py
--rw-rw-rw-   0        0        0     2234 2023-06-10 12:42:19.000000 iman-0.0.95/iman/web.py
--rw-rw-rw-   0        0        0     7159 2022-10-26 09:16:54.000000 iman-0.0.95/iman/xvector.py
-drwxrwxrwx   0        0        0        0 2023-08-05 09:37:31.000000 iman-0.0.95/iman.egg-info/
--rw-rw-rw-   0        0        0     6983 2023-08-05 09:37:31.000000 iman-0.0.95/iman.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2067 2023-08-05 09:37:31.000000 iman-0.0.95/iman.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 09:37:31.000000 iman-0.0.95/iman.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-08-05 09:37:31.000000 iman-0.0.95/iman.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-08-05 09:37:31.000000 iman-0.0.95/iman.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 09:37:32.000000 iman-0.0.95/setup.cfg
--rw-rw-rw-   0        0        0      903 2023-08-05 09:33:16.000000 iman-0.0.95/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:08.000000 iman-0.0.96/
+-rw-rw-rw-   0        0        0     6983 2023-08-05 09:42:08.000000 iman-0.0.96/PKG-INFO
+-rw-rw-rw-   0        0        0     6609 2023-08-05 09:37:11.000000 iman-0.0.96/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/
+-rw-rw-rw-   0        0        0     2070 2022-12-25 10:45:05.000000 iman-0.0.96/iman/AUG.py
+-rw-rw-rw-   0        0        0    18503 2023-08-05 08:31:04.000000 iman-0.0.96/iman/Audio.py
+-rw-rw-rw-   0        0        0      124 2023-01-29 08:15:58.000000 iman-0.0.96/iman/Boors.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/Features/
+-rw-rw-rw-   0        0        0       42 2022-11-13 07:01:23.000000 iman-0.0.96/iman/Features/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/Features/mfcc/
+-rw-rw-rw-   0        0        0     2836 2022-11-13 07:05:02.000000 iman-0.0.96/iman/Features/mfcc/LS.py
+-rw-rw-rw-   0        0        0      604 2022-12-12 11:32:38.000000 iman-0.0.96/iman/Features/mfcc/SB.py
+-rw-rw-rw-   0        0        0        0 2022-11-13 06:42:54.000000 iman-0.0.96/iman/Features/mfcc/__init__.py
+-rw-rw-rw-   0        0        0    11080 2021-12-01 10:31:39.000000 iman-0.0.96/iman/Features/mfcc/getmfcc_from_librosa.py
+-rw-rw-rw-   0        0        0    41655 2022-12-12 11:33:13.000000 iman-0.0.96/iman/Features/mfcc/sb_mfcc_class.py
+-rw-rw-rw-   0        0        0     1057 2022-12-25 10:05:56.000000 iman-0.0.96/iman/Image.py
+-rw-rw-rw-   0        0        0      815 2022-12-20 06:25:42.000000 iman-0.0.96/iman/Report.py
+-rw-rw-rw-   0        0        0     2640 2023-02-20 05:13:55.000000 iman-0.0.96/iman/Text.py
+-rw-rw-rw-   0        0        0     4478 2023-07-22 04:52:36.000000 iman-0.0.96/iman/__init__.py
+-rw-rw-rw-   0        0        0      686 2022-12-17 11:18:42.000000 iman-0.0.96/iman/examples.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/examples_folder/
+-rw-rw-rw-   0        0        0        0 2022-12-17 11:24:05.000000 iman-0.0.96/iman/examples_folder/__init__.py
+-rw-rw-rw-   0        0        0      539 2023-01-01 11:18:41.000000 iman-0.0.96/iman/examples_folder/age.py
+-rw-rw-rw-   0        0        0      100 2023-01-01 05:01:21.000000 iman-0.0.96/iman/examples_folder/ffmpeg.py
+-rw-rw-rw-   0        0        0      490 2022-12-17 09:55:52.000000 iman-0.0.96/iman/examples_folder/flask.py
+-rw-rw-rw-   0        0        0      262 2021-01-05 11:07:03.000000 iman-0.0.96/iman/examples_folder/gpu_allocate_tf.py
+-rw-rw-rw-   0        0        0      299 2022-12-31 09:42:30.000000 iman-0.0.96/iman/examples_folder/graphviz_chart.py
+-rw-rw-rw-   0        0        0      345 2022-12-17 11:09:10.000000 iman-0.0.96/iman/examples_folder/parallel.py
+-rw-rw-rw-   0        0        0      217 2022-12-17 11:12:20.000000 iman-0.0.96/iman/examples_folder/post_by_python.py
+-rw-rw-rw-   0        0        0      775 2019-12-03 03:31:26.000000 iman-0.0.96/iman/examples_folder/pyworldd.py
+-rw-rw-rw-   0        0        0      406 2022-12-05 05:24:04.000000 iman-0.0.96/iman/examples_folder/queue_worker.py
+-rw-rw-rw-   0        0        0     1607 2021-11-28 10:10:27.000000 iman-0.0.96/iman/examples_folder/save_docx.py
+-rw-rw-rw-   0        0        0      478 2019-05-05 06:27:38.000000 iman-0.0.96/iman/examples_folder/stft_test.py
+-rw-rw-rw-   0        0        0      276 2019-11-19 00:37:16.000000 iman-0.0.96/iman/examples_folder/threading_example.py
+-rw-rw-rw-   0        0        0      454 2021-05-25 08:55:10.000000 iman-0.0.96/iman/examples_folder/wikipedia.py
+-rw-rw-rw-   0        0        0    15323 2022-11-06 10:39:16.000000 iman-0.0.96/iman/gpu_info.py
+-rw-rw-rw-   0        0        0     1862 2022-11-12 05:34:50.000000 iman-0.0.96/iman/info.py
+-rw-rw-rw-   0        0        0      318 2022-11-08 10:24:41.000000 iman-0.0.96/iman/matlab.py
+-rw-rw-rw-   0        0        0     3422 2022-12-26 10:35:15.000000 iman-0.0.96/iman/metrics.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/num2fa/
+-rw-rw-rw-   0        0        0     8938 2023-01-28 05:46:54.000000 iman-0.0.96/iman/num2fa/__init__.py
+-rw-rw-rw-   0        0        0      506 2023-01-28 05:46:54.000000 iman-0.0.96/iman/num2fa/__main__.py
+-rw-rw-rw-   0        0        0      237 2022-12-19 06:23:20.000000 iman-0.0.96/iman/par.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/pyctcdecode/
+-rw-rw-rw-   0        0        0      265 2023-07-11 05:28:53.000000 iman-0.0.96/iman/pyctcdecode/__init__.py
+-rw-rw-rw-   0        0        0     6186 2023-07-11 05:28:53.000000 iman-0.0.96/iman/pyctcdecode/alphabet.py
+-rw-rw-rw-   0        0        0      617 2023-07-11 05:28:53.000000 iman-0.0.96/iman/pyctcdecode/constants.py
+-rw-rw-rw-   0        0        0    29784 2023-07-19 12:40:28.000000 iman-0.0.96/iman/pyctcdecode/decoder.py
+-rw-rw-rw-   0        0        0    11420 2023-07-11 05:28:53.000000 iman-0.0.96/iman/pyctcdecode/language_model.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman/sad_tf/
+-rw-rw-rw-   0        0        0      101 2023-07-23 07:12:34.000000 iman-0.0.96/iman/sad_tf/__init__.py
+-rw-rw-rw-   0        0        0     5963 2023-08-05 08:55:48.000000 iman-0.0.96/iman/sad_tf/export_funcs.py
+-rw-rw-rw-   0        0        0     2221 2023-07-05 11:06:11.000000 iman-0.0.96/iman/sad_tf/features.py
+-rw-rw-rw-   0        0        0    19052 2023-08-05 09:41:47.000000 iman-0.0.96/iman/sad_tf/segmenter.py
+-rw-rw-rw-   0        0        0    20025 2023-07-23 08:03:31.000000 iman-0.0.96/iman/sad_tf/segmentero.py
+-rw-rw-rw-   0        0        0    13783 2022-11-30 10:00:38.000000 iman-0.0.96/iman/sad_tf/sidekit_mfcc.py
+-rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.96/iman/sad_tf/thread_returning.py
+-rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.96/iman/sad_tf/viterbi.py
+-rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.96/iman/sad_tf/viterbi_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:08.000000 iman-0.0.96/iman/sad_torch_mfcc/
+-rw-rw-rw-   0        0        0      107 2022-12-26 10:21:43.000000 iman-0.0.96/iman/sad_torch_mfcc/__init__.py
+-rw-rw-rw-   0        0        0     4645 2022-12-11 08:33:44.000000 iman-0.0.96/iman/sad_torch_mfcc/export_funcs.py
+-rw-rw-rw-   0        0        0     2002 2023-07-05 11:08:54.000000 iman-0.0.96/iman/sad_torch_mfcc/features.py
+-rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.96/iman/sad_torch_mfcc/sad_model.py
+-rw-rw-rw-   0        0        0    19324 2023-07-22 04:57:05.000000 iman-0.0.96/iman/sad_torch_mfcc/segmenter.py
+-rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.96/iman/sad_torch_mfcc/thread_returning.py
+-rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.96/iman/sad_torch_mfcc/viterbi.py
+-rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.96/iman/sad_torch_mfcc/viterbi_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:08.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/
+-rw-rw-rw-   0        0        0       36 2023-07-26 06:11:13.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/__init__.py
+-rw-rw-rw-   0        0        0      631 2023-07-26 06:41:32.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/features.py
+-rw-rw-rw-   0        0        0     3098 2022-12-11 08:39:59.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/sad_model.py
+-rw-rw-rw-   0        0        0    10232 2023-07-26 07:10:07.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/segmenter.py
+-rw-rw-rw-   0        0        0      553 2022-01-12 05:39:10.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/thread_returning.py
+-rw-rw-rw-   0        0        0     7808 2022-01-12 05:39:09.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/viterbi.py
+-rw-rw-rw-   0        0        0     1755 2022-01-12 05:39:10.000000 iman-0.0.96/iman/sad_torch_mfcc_speaker/viterbi_utils.py
+-rw-rw-rw-   0        0        0      422 2022-11-22 05:36:39.000000 iman-0.0.96/iman/tsne.py
+-rw-rw-rw-   0        0        0     2234 2023-06-10 12:42:19.000000 iman-0.0.96/iman/web.py
+-rw-rw-rw-   0        0        0     7159 2022-10-26 09:16:54.000000 iman-0.0.96/iman/xvector.py
+drwxrwxrwx   0        0        0        0 2023-08-05 09:42:07.000000 iman-0.0.96/iman.egg-info/
+-rw-rw-rw-   0        0        0     6983 2023-08-05 09:42:07.000000 iman-0.0.96/iman.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2067 2023-08-05 09:42:07.000000 iman-0.0.96/iman.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 09:42:07.000000 iman-0.0.96/iman.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-08-05 09:42:07.000000 iman-0.0.96/iman.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-05 09:42:07.000000 iman-0.0.96/iman.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 09:42:08.000000 iman-0.0.96/setup.cfg
+-rw-rw-rw-   0        0        0      903 2023-08-05 09:42:00.000000 iman-0.0.96/setup.py
```

### Comparing `iman-0.0.95/PKG-INFO` & `iman-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iman
-Version: 0.0.95
+Version: 0.0.96
 Summary: Python package for daily Tasks
 Home-page: UNKNOWN
 Author: Iman Sarraf
 Author-email: imansarraf@gmail.com
 License: UNKNOWN
 Keywords: python,iman
 Platform: UNKNOWN
```

### Comparing `iman-0.0.95/README.rst` & `iman-0.0.96/README.rst`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/AUG.py` & `iman-0.0.96/iman/AUG.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Audio.py` & `iman-0.0.96/iman/Audio.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Features/mfcc/LS.py` & `iman-0.0.96/iman/Features/mfcc/LS.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Features/mfcc/SB.py` & `iman-0.0.96/iman/Features/mfcc/SB.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Features/mfcc/getmfcc_from_librosa.py` & `iman-0.0.96/iman/Features/mfcc/getmfcc_from_librosa.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Features/mfcc/sb_mfcc_class.py` & `iman-0.0.96/iman/Features/mfcc/sb_mfcc_class.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Image.py` & `iman-0.0.96/iman/Image.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Report.py` & `iman-0.0.96/iman/Report.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/Text.py` & `iman-0.0.96/iman/Text.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/__init__.py` & `iman-0.0.96/iman/__init__.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/examples.py` & `iman-0.0.96/iman/examples.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/examples_folder/age.py` & `iman-0.0.96/iman/examples_folder/age.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/examples_folder/pyworldd.py` & `iman-0.0.96/iman/examples_folder/pyworldd.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/examples_folder/save_docx.py` & `iman-0.0.96/iman/examples_folder/save_docx.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/gpu_info.py` & `iman-0.0.96/iman/gpu_info.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/info.py` & `iman-0.0.96/iman/info.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/metrics.py` & `iman-0.0.96/iman/metrics.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/num2fa/__init__.py` & `iman-0.0.96/iman/num2fa/__init__.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/pyctcdecode/alphabet.py` & `iman-0.0.96/iman/pyctcdecode/alphabet.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/pyctcdecode/constants.py` & `iman-0.0.96/iman/pyctcdecode/constants.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/pyctcdecode/decoder.py` & `iman-0.0.96/iman/pyctcdecode/decoder.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/pyctcdecode/language_model.py` & `iman-0.0.96/iman/pyctcdecode/language_model.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/export_funcs.py` & `iman-0.0.96/iman/sad_tf/export_funcs.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/features.py` & `iman-0.0.96/iman/sad_tf/features.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/segmenter.py` & `iman-0.0.96/iman/sad_tf/segmenter.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,28 +408,28 @@
             if lab == 0:
                 lab = 'noEnergy'
             else:
                 lab = 'energy'
                 vadseg.append(('speech', start, stop))
             lseg.append((lab, start, stop))
         if (self.vad_type == 'vad'):
-           return [(lab, start_sec + start * .04, start_sec + stop * .04 , stop-start) for lab, start, stop in vadseg]
+           return [(lab, start_sec + start * .02, start_sec + stop * .02 , stop-start) for lab, start, stop in vadseg]
         # perform voice activity detection
         lseg = self.vad(mspec, lseg, difflen)
         
         
         
 
         # perform gender segmentation on speech segments
         if self.detect_gender:
             lseg = self.gender(mspec, lseg, difflen)
         if (self.complete_output):
-           return   [(lab, start_sec + start * .04, start_sec + stop * .04 , (stop-start) * .04) for lab, start, stop in lseg ]
+           return   [(lab, start_sec + start * .02, start_sec + stop * .02 , (stop-start) * .02) for lab, start, stop in lseg ]
         else:
-           return   [[lab, start_sec + start * .04, start_sec + stop * .04 , (stop-start) * .04] for lab, start, stop in lseg if (lab=='male' or lab=="female" or lab=="speech")]   
+           return   [[lab, start_sec + start * .02, start_sec + stop * .02 , (stop-start) * .02] for lab, start, stop in lseg if (lab=='male' or lab=="female" or lab=="speech")]   
 
 
     def __call__(self, medianame,start_sec=None, stop_sec=None):
         """
         Return segmentation of a given file
                 * convert file to wav 16k mono with ffmpeg
                 * call NN segmentation procedures
```

### Comparing `iman-0.0.95/iman/sad_tf/segmentero.py` & `iman-0.0.96/iman/sad_tf/segmentero.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/sidekit_mfcc.py` & `iman-0.0.96/iman/sad_tf/sidekit_mfcc.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/thread_returning.py` & `iman-0.0.96/iman/sad_tf/thread_returning.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/viterbi.py` & `iman-0.0.96/iman/sad_tf/viterbi.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_tf/viterbi_utils.py` & `iman-0.0.96/iman/sad_tf/viterbi_utils.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/export_funcs.py` & `iman-0.0.96/iman/sad_torch_mfcc/export_funcs.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/features.py` & `iman-0.0.96/iman/sad_torch_mfcc/features.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/sad_model.py` & `iman-0.0.96/iman/sad_torch_mfcc/sad_model.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/segmenter.py` & `iman-0.0.96/iman/sad_torch_mfcc/segmenter.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/thread_returning.py` & `iman-0.0.96/iman/sad_torch_mfcc/thread_returning.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/viterbi.py` & `iman-0.0.96/iman/sad_torch_mfcc/viterbi.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc/viterbi_utils.py` & `iman-0.0.96/iman/sad_torch_mfcc/viterbi_utils.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc_speaker/features.py` & `iman-0.0.96/iman/sad_torch_mfcc_speaker/features.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc_speaker/sad_model.py` & `iman-0.0.96/iman/sad_torch_mfcc_speaker/sad_model.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc_speaker/segmenter.py` & `iman-0.0.96/iman/sad_torch_mfcc_speaker/segmenter.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc_speaker/thread_returning.py` & `iman-0.0.96/iman/sad_torch_mfcc_speaker/thread_returning.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc_speaker/viterbi.py` & `iman-0.0.96/iman/sad_torch_mfcc_speaker/viterbi.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/sad_torch_mfcc_speaker/viterbi_utils.py` & `iman-0.0.96/iman/sad_torch_mfcc_speaker/viterbi_utils.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/web.py` & `iman-0.0.96/iman/web.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman/xvector.py` & `iman-0.0.96/iman/xvector.py`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/iman.egg-info/PKG-INFO` & `iman-0.0.96/iman.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iman
-Version: 0.0.95
+Version: 0.0.96
 Summary: Python package for daily Tasks
 Home-page: UNKNOWN
 Author: Iman Sarraf
 Author-email: imansarraf@gmail.com
 License: UNKNOWN
 Keywords: python,iman
 Platform: UNKNOWN
```

### Comparing `iman-0.0.95/iman.egg-info/SOURCES.txt` & `iman-0.0.96/iman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iman-0.0.95/setup.py` & `iman-0.0.96/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 setup(
         # the name must match the folder name 'verysimplemodule'
         name="iman", 
-        version='0.0.95',
+        version='0.0.96',
         author="Iman Sarraf",
         author_email="imansarraf@gmail.com",
         description='Python package for daily Tasks',
         long_description=read('README.rst'),
         packages=find_packages(),
         
         # add any additional packages that
```

