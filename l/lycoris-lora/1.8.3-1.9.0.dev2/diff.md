# Comparing `tmp/lycoris_lora-1.8.3.tar.gz` & `tmp/lycoris_lora-1.9.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lycoris_lora-1.8.3.tar", last modified: Fri Jul 28 15:13:06 2023, max compression
+gzip compressed data, was "lycoris_lora-1.9.0.dev2.tar", last modified: Sat Aug  5 02:40:39 2023, max compression
```

## Comparing `lycoris_lora-1.8.3.tar` & `lycoris_lora-1.9.0.dev2.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.405975 lycoris_lora-1.8.3/
--rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/.gitignore
--rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.8.3/Algo.md
--rw-rw-rw-   0        0        0     1277 2023-07-27 09:31:21.000000 lycoris_lora-1.8.3/Change.md
--rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.8.3/Demo.md
--rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.8.3/LICENSE.md
--rw-rw-rw-   0        0        0      348 2023-07-28 15:13:06.405975 lycoris_lora-1.8.3/PKG-INFO
--rw-rw-rw-   0        0        0     7531 2023-07-27 09:30:40.000000 lycoris_lora-1.8.3/README.md
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.382475 lycoris_lora-1.8.3/experiments/
--rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.8.3/experiments/better_conv.py
--rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.8.3/experiments/better_conv_extract.py
--rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/experiments/compare_norm.py
--rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.8.3/experiments/concept_neuron.py
--rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.8.3/experiments/locon_extract_test.py
--rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.8.3/experiments/locon_merge_test.py
--rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/experiments/loha_svd.py
--rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.8.3/experiments/singular_value_test.py
--rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.8.3/experiments/sparse_bias_test.py
--rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.8.3/experiments/time_test.py
--rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.8.3/experiments/weakre_speed.py
--rw-rw-rw-   0        0        0     4110 2023-07-27 02:15:19.000000 lycoris_lora-1.8.3/hyperdream_gen_weight.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.383476 lycoris_lora-1.8.3/lycoris/
--rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/__init__.py
--rw-rw-rw-   0        0        0     2672 2023-07-27 02:52:33.000000 lycoris_lora-1.8.3/lycoris/config.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.385976 lycoris_lora-1.8.3/lycoris/kohya/
--rw-rw-rw-   0        0        0    42384 2023-07-28 15:12:31.000000 lycoris_lora-1.8.3/lycoris/kohya/__init__.py
--rw-rw-rw-   0        0        0    56362 2023-07-27 09:26:55.000000 lycoris_lora-1.8.3/lycoris/kohya/model_utils.py
--rw-rw-rw-   0        0        0    58870 2023-07-27 09:27:06.000000 lycoris_lora-1.8.3/lycoris/kohya/original_unet.py
--rw-rw-rw-   0        0        0    20779 2023-07-27 09:28:08.000000 lycoris_lora-1.8.3/lycoris/kohya/sdxl_model_util.py
--rw-rw-rw-   0        0        0    41085 2023-07-27 03:12:49.000000 lycoris_lora-1.8.3/lycoris/kohya/sdxl_original_unet.py
--rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/kohya/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.389475 lycoris_lora-1.8.3/lycoris/modules/
--rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/__init__.py
--rw-rw-rw-   0        0        0     7334 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/attention.py
--rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/dylora.py
--rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/glokr.py
--rw-rw-rw-   0        0        0     4117 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/glora.py
--rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/hyperlycoris.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.390475 lycoris_lora-1.8.3/lycoris/modules/hypernet/
--rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/hypernet/__init__.py
--rw-rw-rw-   0        0        0     8228 2023-07-25 10:04:24.000000 lycoris_lora-1.8.3/lycoris/modules/hypernet/generater.py
--rw-rw-rw-   0        0        0     8111 2023-07-25 10:04:17.000000 lycoris_lora-1.8.3/lycoris/modules/hypernet/text_encoder.py
--rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/modules/ia3.py
--rw-rw-rw-   0        0        0    10342 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/locon.py
--rw-rw-rw-   0        0        0    10065 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/loha.py
--rw-rw-rw-   0        0        0    12654 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/modules/lokr.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.391976 lycoris_lora-1.8.3/lycoris/utils/
--rw-rw-rw-   0        0        0    21031 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/utils/__init__.py
--rw-rw-rw-   0        0        0       41 2023-07-25 09:54:09.000000 lycoris_lora-1.8.3/lycoris/utils/preset.py
--rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/lycoris/utils/xformers_utils.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.404477 lycoris_lora-1.8.3/lycoris_lora.egg-info/
--rw-rw-rw-   0        0        0      348 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1385 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-07-28 15:13:06.000000 lycoris_lora-1.8.3/lycoris_lora.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.8.3/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-07-28 15:13:06.405975 lycoris_lora-1.8.3/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-07-28 15:12:43.000000 lycoris_lora-1.8.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-28 15:13:06.404976 lycoris_lora-1.8.3/tools/
--rw-rw-rw-   0        0        0     4087 2023-07-27 02:15:19.000000 lycoris_lora-1.8.3/tools/extract_locon.py
--rw-rw-rw-   0        0        0     2293 2023-07-27 02:15:19.000000 lycoris_lora-1.8.3/tools/merge.py
--rw-rw-rw-   0        0        0    55484 2023-07-25 09:54:11.000000 lycoris_lora-1.8.3/train_hyperdream.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.768440 lycoris_lora-1.9.0.dev2/
+-rw-rw-rw-   0        0        0     1682 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/.gitignore
+-rw-rw-rw-   0        0        0     4436 2023-04-09 13:45:45.000000 lycoris_lora-1.9.0.dev2/Algo.md
+-rw-rw-rw-   0        0        0     1277 2023-07-27 09:31:21.000000 lycoris_lora-1.9.0.dev2/Change.md
+-rw-rw-rw-   0        0        0     2828 2023-03-09 12:01:15.000000 lycoris_lora-1.9.0.dev2/Demo.md
+-rw-rw-rw-   0        0        0    11545 2023-03-09 05:37:07.000000 lycoris_lora-1.9.0.dev2/LICENSE.md
+-rw-rw-rw-   0        0        0      353 2023-08-05 02:40:39.767941 lycoris_lora-1.9.0.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     7737 2023-07-30 11:18:57.000000 lycoris_lora-1.9.0.dev2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.743440 lycoris_lora-1.9.0.dev2/experiments/
+-rw-rw-rw-   0        0        0     3579 2023-03-12 01:46:48.000000 lycoris_lora-1.9.0.dev2/experiments/better_conv.py
+-rw-rw-rw-   0        0        0     1967 2023-03-12 01:46:43.000000 lycoris_lora-1.9.0.dev2/experiments/better_conv_extract.py
+-rw-rw-rw-   0        0        0      651 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/experiments/compare_norm.py
+-rw-rw-rw-   0        0        0     8783 2023-03-12 03:21:33.000000 lycoris_lora-1.9.0.dev2/experiments/concept_neuron.py
+-rw-rw-rw-   0        0        0      894 2023-03-09 14:26:54.000000 lycoris_lora-1.9.0.dev2/experiments/locon_extract_test.py
+-rw-rw-rw-   0        0        0      755 2023-03-10 15:36:09.000000 lycoris_lora-1.9.0.dev2/experiments/locon_merge_test.py
+-rw-rw-rw-   0        0        0     1028 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/experiments/loha_svd.py
+-rw-rw-rw-   0        0        0     3411 2023-03-09 05:37:07.000000 lycoris_lora-1.9.0.dev2/experiments/singular_value_test.py
+-rw-rw-rw-   0        0        0     2334 2023-03-11 09:28:26.000000 lycoris_lora-1.9.0.dev2/experiments/sparse_bias_test.py
+-rw-rw-rw-   0        0        0     2791 2023-03-12 01:46:48.000000 lycoris_lora-1.9.0.dev2/experiments/time_test.py
+-rw-rw-rw-   0        0        0      255 2023-06-25 07:25:35.000000 lycoris_lora-1.9.0.dev2/experiments/weakre_speed.py
+-rw-rw-rw-   0        0        0     4110 2023-07-27 02:15:19.000000 lycoris_lora-1.9.0.dev2/hyperdream_gen_weight.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.744442 lycoris_lora-1.9.0.dev2/lycoris/
+-rw-rw-rw-   0        0        0       55 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/__init__.py
+-rw-rw-rw-   0        0        0     2672 2023-07-27 02:52:33.000000 lycoris_lora-1.9.0.dev2/lycoris/config.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.746941 lycoris_lora-1.9.0.dev2/lycoris/kohya/
+-rw-rw-rw-   0        0        0    42580 2023-08-05 02:40:24.000000 lycoris_lora-1.9.0.dev2/lycoris/kohya/__init__.py
+-rw-rw-rw-   0        0        0    56362 2023-07-27 09:26:55.000000 lycoris_lora-1.9.0.dev2/lycoris/kohya/model_utils.py
+-rw-rw-rw-   0        0        0    58870 2023-07-27 09:27:06.000000 lycoris_lora-1.9.0.dev2/lycoris/kohya/original_unet.py
+-rw-rw-rw-   0        0        0    20779 2023-07-27 09:28:08.000000 lycoris_lora-1.9.0.dev2/lycoris/kohya/sdxl_model_util.py
+-rw-rw-rw-   0        0        0    41085 2023-07-27 03:12:49.000000 lycoris_lora-1.9.0.dev2/lycoris/kohya/sdxl_original_unet.py
+-rw-rw-rw-   0        0        0     1512 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/kohya/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.750942 lycoris_lora-1.9.0.dev2/lycoris/modules/
+-rw-rw-rw-   0        0        0        0 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/__init__.py
+-rw-rw-rw-   0        0        0     7334 2023-07-25 09:54:09.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/attention.py
+-rw-rw-rw-   0        0        0     4762 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/dylora.py
+-rw-rw-rw-   0        0        0    10763 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/glokr.py
+-rw-rw-rw-   0        0        0     4139 2023-07-31 09:36:13.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/glora.py
+-rw-rw-rw-   0        0        0       64 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/hyperlycoris.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.751940 lycoris_lora-1.9.0.dev2/lycoris/modules/hypernet/
+-rw-rw-rw-   0        0        0       97 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/hypernet/__init__.py
+-rw-rw-rw-   0        0        0     8236 2023-08-05 02:39:54.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/hypernet/generater.py
+-rw-rw-rw-   0        0        0     8111 2023-07-25 10:04:17.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/hypernet/text_encoder.py
+-rw-rw-rw-   0        0        0     2103 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/ia3.py
+-rw-rw-rw-   0        0        0    10434 2023-08-05 02:06:29.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/locon.py
+-rw-rw-rw-   0        0        0    10166 2023-08-05 02:05:44.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/loha.py
+-rw-rw-rw-   0        0        0    12779 2023-08-05 02:05:16.000000 lycoris_lora-1.9.0.dev2/lycoris/modules/lokr.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.752940 lycoris_lora-1.9.0.dev2/lycoris/utils/
+-rw-rw-rw-   0        0        0    21290 2023-07-31 15:37:50.000000 lycoris_lora-1.9.0.dev2/lycoris/utils/__init__.py
+-rw-rw-rw-   0        0        0       41 2023-07-25 09:54:09.000000 lycoris_lora-1.9.0.dev2/lycoris/utils/preset.py
+-rw-rw-rw-   0        0        0      249 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/lycoris/utils/xformers_utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.766939 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/
+-rw-rw-rw-   0        0        0      353 2023-08-05 02:40:39.000000 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1385 2023-08-05 02:40:39.000000 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 02:40:39.000000 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-03-09 13:25:15.000000 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-08-05 02:40:39.000000 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-08-05 02:40:39.000000 lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-19 08:00:19.000000 lycoris_lora-1.9.0.dev2/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 02:40:39.768440 lycoris_lora-1.9.0.dev2/setup.cfg
+-rw-rw-rw-   0        0        0      566 2023-08-05 02:39:09.000000 lycoris_lora-1.9.0.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 02:40:39.767439 lycoris_lora-1.9.0.dev2/tools/
+-rw-rw-rw-   0        0        0     4087 2023-07-27 02:15:19.000000 lycoris_lora-1.9.0.dev2/tools/extract_locon.py
+-rw-rw-rw-   0        0        0     2323 2023-07-31 15:29:19.000000 lycoris_lora-1.9.0.dev2/tools/merge.py
+-rw-rw-rw-   0        0        0    55484 2023-07-25 09:54:11.000000 lycoris_lora-1.9.0.dev2/train_hyperdream.py
```

### Comparing `lycoris_lora-1.8.3/.gitignore` & `lycoris_lora-1.9.0.dev2/.gitignore`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/Algo.md` & `lycoris_lora-1.9.0.dev2/Algo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/Change.md` & `lycoris_lora-1.9.0.dev2/Change.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/Demo.md` & `lycoris_lora-1.9.0.dev2/Demo.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/LICENSE.md` & `lycoris_lora-1.9.0.dev2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/README.md` & `lycoris_lora-1.9.0.dev2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # LyCORIS - Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion.
 
-![image](https://user-images.githubusercontent.com/59680068/224026402-7b779d58-5164-4ecd-a807-f98badae589e.png)
+![image](https://user-images.githubusercontent.com/59680068/224026402-7b779d58-5164-4ecd-a807-f98badae589e.png)  
 (This image is generated by the model trained in Hadamard product representation)
 
 A project for implementing different algorithm to do parameter-efficient finetuning on stable diffusion or more.
 
 This project is started from LoCon(see archive branch).
 
+**If you are interested in discussing more details, you can join [our Discord server](https://discord.gg/VtTFKrj9gJ).**
+
+[![Discord!](https://i.imgur.com/A8tOvFS.jpg)](https://discord.gg/VtTFKrj9gJ)
+
 
 ## What we have now
 See [Algo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Algo.md) or [Demo.md](https://github.com/KohakuBlueleaf/LyCORIS/blob/main/Demo.md) for more example and explanation
 
 ### Conventional LoRA
 * Include Conv layer implementation from LoCon
 * recommended settings
```

### Comparing `lycoris_lora-1.8.3/experiments/better_conv.py` & `lycoris_lora-1.9.0.dev2/experiments/better_conv.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/better_conv_extract.py` & `lycoris_lora-1.9.0.dev2/experiments/better_conv_extract.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/compare_norm.py` & `lycoris_lora-1.9.0.dev2/experiments/compare_norm.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/concept_neuron.py` & `lycoris_lora-1.9.0.dev2/experiments/concept_neuron.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/locon_extract_test.py` & `lycoris_lora-1.9.0.dev2/experiments/locon_extract_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/locon_merge_test.py` & `lycoris_lora-1.9.0.dev2/experiments/locon_merge_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/loha_svd.py` & `lycoris_lora-1.9.0.dev2/experiments/loha_svd.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/singular_value_test.py` & `lycoris_lora-1.9.0.dev2/experiments/singular_value_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/sparse_bias_test.py` & `lycoris_lora-1.9.0.dev2/experiments/sparse_bias_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/experiments/time_test.py` & `lycoris_lora-1.9.0.dev2/experiments/time_test.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/hyperdream_gen_weight.py` & `lycoris_lora-1.9.0.dev2/hyperdream_gen_weight.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/config.py` & `lycoris_lora-1.9.0.dev2/lycoris/config.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/kohya/__init__.py` & `lycoris_lora-1.9.0.dev2/lycoris/kohya/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 from .utils import *
 from ..modules.locon import LoConModule
 from ..modules.loha import LohaModule
 from ..modules.ia3 import IA3Module
 from ..modules.lokr import LokrModule
 from ..modules.dylora import DyLoraModule
 from ..modules.glora import GLoRAModule
-from ..modules.hypernet import ImgWeightGenerator, TextWeightGenerator
 
 from ..config import PRESET
 from ..utils.preset import read_preset
 
 
 def create_network(multiplier, network_dim, network_alpha, vae, text_encoder, unet, **kwargs):
     if network_dim is None:
@@ -31,25 +30,30 @@
     conv_alpha = float(kwargs.get('conv_alpha', network_alpha) or network_alpha)
     dropout = float(kwargs.get('dropout', 0.) or 0.)
     rank_dropout = float(kwargs.get("rank_dropout", 0.) or 0.)
     module_dropout = float(kwargs.get("module_dropout", 0.) or 0.)
     algo = (kwargs.get('algo', 'lora') or 'lora').lower()
     use_cp = (not kwargs.get('disable_conv_cp', True)
               or kwargs.get('use_conv_cp', False))
+    use_scalar = kwargs.get('use_scalar', False)
     block_size = int(kwargs.get('block_size', 4) or 4)
     network_module = {
         'lora': LoConModule,
         'locon': LoConModule,
         'loha': LohaModule,
         'ia3':  IA3Module,
         'lokr': LokrModule,
         'dylora': DyLoraModule,
         'glora': GLoRAModule,
     }[algo]
     
+    if algo == 'glora' and conv_dim>0:
+        conv_dim = 0
+        print('Disable conv layer for GLoRA')
+    
     preset = kwargs.get('preset', 'full')
     if preset not in PRESET:
         preset = read_preset(preset)
     else:
         preset = PRESET[preset]
     assert preset is not None
     LycorisNetwork.apply_preset(preset)
@@ -79,15 +83,15 @@
     else:
         network = LycorisNetwork(
             text_encoder, unet, 
             multiplier=multiplier, 
             lora_dim=network_dim, conv_lora_dim=conv_dim, 
             alpha=network_alpha, conv_alpha=conv_alpha,
             dropout=dropout, rank_dropout=rank_dropout, module_dropout=module_dropout,
-            use_cp=use_cp,
+            use_cp=use_cp, use_scalar=use_scalar,
             network_module=network_module,
             decompose_both=kwargs.get('decompose_both', False),
             factor=kwargs.get('factor', -1),
             block_size = block_size
         )
     
     if algo=='dylora':
@@ -513,14 +517,15 @@
         lora_dim=4, alpha=1,
         use_cp = False,
         dropout = 0, rank_dropout = 0, module_dropout = 0,
         network_module = LoConModule,
         down_dim = 100, up_dim = 50, delta_iters = 5, decoder_blocks = 4, vocab_size = 49408,
         **kwargs,
     ) -> None:
+        from ..modules.hypernet import ImgWeightGenerator, TextWeightGenerator
         super().__init__()
         self.gradient_ckpt = False
         self.multiplier = multiplier
         self.lora_dim = lora_dim
         self.alpha = alpha
         
         if 1 >= dropout >= 0:
```

### Comparing `lycoris_lora-1.8.3/lycoris/kohya/model_utils.py` & `lycoris_lora-1.9.0.dev2/lycoris/kohya/model_utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/kohya/original_unet.py` & `lycoris_lora-1.9.0.dev2/lycoris/kohya/original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/kohya/sdxl_model_util.py` & `lycoris_lora-1.9.0.dev2/lycoris/kohya/sdxl_model_util.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/kohya/sdxl_original_unet.py` & `lycoris_lora-1.9.0.dev2/lycoris/kohya/sdxl_original_unet.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/kohya/utils.py` & `lycoris_lora-1.9.0.dev2/lycoris/kohya/utils.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/modules/attention.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/attention.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/modules/dylora.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/dylora.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/modules/glokr.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/glokr.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/modules/glora.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/glora.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,8 +96,8 @@
                 drop_b = drop_b.view(1, -1, 1, 1)
             else:
                 drop_a = drop_a.view(*[1]*(dims-1), -1)
                 drop_b = drop_b.view(*[1]*(dims-1), -1)
             ax_mid = ax_mid * drop_a
             bx_mid = bx_mid * drop_b
         
-        return self.org_forward(x + self.dropout(self.a2(ax_mid))) + self.dropout(self.b2(bx_mid))
+        return self.org_forward(x + self.dropout(self.a2(ax_mid))*self.scale) + self.dropout(self.b2(bx_mid))*self.scale
```

### Comparing `lycoris_lora-1.8.3/lycoris/modules/hypernet/generater.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/hypernet/generater.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 from torchvision.transforms.functional import resize
 
 from timm import create_model
 from einops import rearrange
 
 from lycoris.modules.attention import TransformerBlock
-from .text_encoder import FrozenOpenCLIPEmbedder
 
 
 def _get_sinusoid_encoding_table(n_position, d_hid):
     ''' Sinusoid position encoding table '''
     # TODO: make it with torch instead of numpy
 
     def get_position_angle_vec(position):
@@ -147,14 +146,15 @@
         train_encoder: bool = False,
         reference_size: Tuple[int] = (224, 224), 
         weight_dim: int = 150,                      # 100+50 in paper
         weight_num: int = 54,                       # 21*2 in SD UNet + 12 in CLIP-L TE
         decoder_blocks: int = 4,
         sample_iters: int = 1,
     ):
+        from .text_encoder import FrozenOpenCLIPEmbedder
         super(TextWeightGenerator, self).__init__()
         self.ref_size = reference_size
         self.weight_num = weight_num
         self.weight_dim = weight_dim
         self.sample_iters = sample_iters
         self.train_encoder = train_encoder
```

### Comparing `lycoris_lora-1.8.3/lycoris/modules/hypernet/text_encoder.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/hypernet/text_encoder.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/modules/ia3.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/ia3.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/lycoris/modules/locon.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/locon.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,24 +14,23 @@
 
     def __init__(
         self, 
         lora_name, org_module: nn.Module, 
         multiplier=1.0, 
         lora_dim=4, alpha=1, 
         dropout=0., rank_dropout=0., module_dropout=0.,
-        use_cp=False,
+        use_cp=False, use_scalar=False,
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
         self.lora_dim = lora_dim
         self.cp = False
 
-        self.scalar = nn.Parameter(torch.tensor(0.0))
         if isinstance(org_module, nn.Conv2d):
             self.isconv = True
             # For general LoCon
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
             stride = org_module.stride
             padding = org_module.padding
@@ -66,14 +65,18 @@
         
         if type(alpha) == torch.Tensor:
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
+        else:
+            self.scalar = 1.0
         # same as microsoft's
         torch.nn.init.kaiming_uniform_(self.lora_down.weight, a=math.sqrt(5))
         torch.nn.init.kaiming_uniform_(self.lora_up.weight)
         if self.cp:
             torch.nn.init.kaiming_uniform_(self.lora_mid.weight, a=math.sqrt(5))
 
         self.multiplier = multiplier
```

### Comparing `lycoris_lora-1.8.3/lycoris/modules/loha.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/loha.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,24 +90,24 @@
     def __init__(
         self, 
         lora_name, 
         org_module: nn.Module, 
         multiplier=1.0, lora_dim=4, alpha=1, 
         dropout=0., rank_dropout=0., module_dropout=0.,
         use_cp=False,
+        use_scalar=False,
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         self.lora_name = lora_name
         self.lora_dim = lora_dim
         self.cp=False
         
         self.shape = org_module.weight.shape
-        self.scalar = nn.Parameter(torch.tensor(0.0))
         if org_module.__class__.__name__ == 'Conv2d':
             in_dim = org_module.in_channels
             k_size = org_module.kernel_size
             out_dim = org_module.out_channels
             self.cp = use_cp and k_size!=(1, 1)
             if self.cp:
                 shape = (out_dim, in_dim, *k_size)
@@ -150,14 +150,18 @@
         
         if type(alpha) == torch.Tensor:
             alpha = alpha.detach().float().numpy()  # without casting, bf16 causes error
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
+        else:
+            self.scalar = 1.0
         # Need more experiments on init method
         if self.cp:
             torch.nn.init.normal_(self.hada_t1, std=0.1)
             torch.nn.init.normal_(self.hada_t2, std=0.1)
         torch.nn.init.normal_(self.hada_w1_b, std=1)
         torch.nn.init.normal_(self.hada_w1_a, std=0.1)
         torch.nn.init.normal_(self.hada_w2_b, std=1)
```

### Comparing `lycoris_lora-1.8.3/lycoris/modules/lokr.py` & `lycoris_lora-1.9.0.dev2/lycoris/modules/lokr.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,14 +76,15 @@
     def __init__(
         self, 
         lora_name, org_module: nn.Module, 
         multiplier=1.0, 
         lora_dim=4, alpha=1, 
         dropout=0., rank_dropout=0., module_dropout=0.,
         use_cp=False,
+        use_scalar=False,
         decompose_both = False,
         factor:int=-1, # factorization factor
         **kwargs,
     ):
         """ if alpha == 0 or None, alpha is rank (no scaling). """
         super().__init__()
         factor = int(factor)
@@ -171,15 +172,19 @@
         alpha = lora_dim if alpha is None or alpha == 0 else alpha
         if self.use_w2 and self.use_w1:
             #use scale = 1
             alpha = lora_dim
         self.scale = alpha / self.lora_dim
         self.register_buffer('alpha', torch.tensor(alpha)) # 定数として扱える
 
-        self.scalar = nn.Parameter(torch.tensor(0.0))
+        if use_scalar:
+            self.scalar = nn.Parameter(torch.tensor(0.0))
+        else:
+            self.scalar = 1.0
+        
         if self.use_w2:
             torch.nn.init.kaiming_uniform_(self.lokr_w2, 0)
         else:
             if self.cp:
                 torch.nn.init.kaiming_uniform_(self.lokr_t2, a=math.sqrt(5))
             torch.nn.init.kaiming_uniform_(self.lokr_w2_a, a=math.sqrt(5))
             torch.nn.init.kaiming_uniform_(self.lokr_w2_b, a=math.sqrt(5))
@@ -292,15 +297,15 @@
                 return self.op(
                     x,
                     self.org_module[0].weight.data,
                     None if self.org_module[0].bias is None else self.org_module[0].bias.data
                 )
         weight = (
             self.org_module[0].weight.data 
-            + self.get_weight(self.org_module[0].weight.data) * self.scalar * self.multiplier
+            + self.get_weight(self.org_module[0].weight.data) * self.vector * self.scalar * self.multiplier
         )
         bias = None if self.org_module[0].bias is None else self.org_module[0].bias.data
         return self.op(
             x, 
             weight.view(self.shape),
             bias,
             **self.extra_args
```

### Comparing `lycoris_lora-1.8.3/lycoris/utils/__init__.py` & `lycoris_lora-1.9.0.dev2/lycoris/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -414,14 +414,17 @@
             else:
                 w1 = w1a @ w1b
         if w2a is not None and w2b is not None:
             if t2:
                 w2 = cp_weight(w2a, w2b, t2)
             else:
                 w2 = w2a @ w2b
+        if len(w2.shape) == 4:
+            w1 = w1.unsqueeze(2).unsqueeze(2)
+        w2 = w2.contiguous()
         rebuild = torch.kron(w1, w2).reshape(orig_weight.shape) 
         merged = orig_weight + rebuild* scale
         del w1, w1a, w1b, w2, w2a, w2b, t1, t2, alpha, params, rebuild
     elif module_type == 'full':
         rebuild = params.reshape(orig_weight.shape) 
         merged = orig_weight + rebuild * scale
         del params, rebuild
@@ -483,26 +486,28 @@
                     lyco_state_dict, lora_name
                 ), getattr(module, 'weight'), scale)
                 if result is not None:
                     merged += 1
                     module.requires_grad_(False)
                     module.weight.copy_(result)
     
-    if device == 'cpu':
-        for k, v in tqdm(list(lyco_state_dict.items()), desc='Converting Dtype'):
-            lyco_state_dict[k] = v.float()
+    for k, v in tqdm(list(lyco_state_dict.items()), desc='Converting Dtype and Device'):
+        if device=='cpu':
+            lyco_state_dict[k] = v.float().cpu()
+        else:
+            lyco_state_dict[k] = v.to(device, dtype=base_model[0].parameters().__next__().dtype)
     
     merge_state_dict(
         LORA_PREFIX_TEXT_ENCODER,
-        base_model[0],
+        base_model[0].to(device),
         lyco_state_dict,
         TEXT_ENCODER_TARGET_REPLACE_MODULE,
         UNET_TARGET_REPLACE_NAME
     )
     merge_state_dict(
         LORA_PREFIX_UNET,
-        base_model[2],
+        base_model[2].to(device),
         lyco_state_dict,
         UNET_TARGET_REPLACE_MODULE,
         UNET_TARGET_REPLACE_NAME
     )
     print(f'{merged} Modules been merged')
```

### Comparing `lycoris_lora-1.8.3/lycoris_lora.egg-info/SOURCES.txt` & `lycoris_lora-1.9.0.dev2/lycoris_lora.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/setup.py` & `lycoris_lora-1.9.0.dev2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='lycoris_lora',
     packages=find_packages(),
-    version='1.8.3',
+    version='1.9.0.dev2',
     url='https://github.com/KohakuBlueleaf/LyCORIS',
     description='Lora beYond Conventional methods, Other Rank adaptation Implementations for Stable diffusion',
     author='Shih-Ying Yeh(KohakuBlueLeaf), Yu-Guan Hsieh, Zhidong Gao',
     author_email='apolloyeh0123@gmail.com',
     zip_safe=False,
     install_requires=[
         'torch',
```

### Comparing `lycoris_lora-1.8.3/tools/extract_locon.py` & `lycoris_lora-1.9.0.dev2/tools/extract_locon.py`

 * *Files identical despite different names*

### Comparing `lycoris_lora-1.8.3/tools/merge.py` & `lycoris_lora-1.9.0.dev2/tools/merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     save_stable_diffusion_checkpoint,
     load_file
 )
 
 import torch
 
 
+@torch.no_grad()
 def main():
     base = load_models_from_stable_diffusion_checkpoint(ARGS.is_v2, ARGS.base_model)
     if ARGS.lycoris_model.rsplit('.', 1)[-1] == 'safetensors':
         lyco = load_file(ARGS.lycoris_model)
     else:
         lyco = torch.load(ARGS.lycoris_model)
     
@@ -71,15 +72,15 @@
         lyco,
         ARGS.weight,
         ARGS.device
     )
     
     save_stable_diffusion_checkpoint(
         ARGS.is_v2, ARGS.output_name, 
-        base[0], base[2], 
+        base[0].cpu(), base[2].cpu(), 
         None, 0, 0, dtype, 
         base[1]
     )
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `lycoris_lora-1.8.3/train_hyperdream.py` & `lycoris_lora-1.9.0.dev2/train_hyperdream.py`

 * *Files identical despite different names*

