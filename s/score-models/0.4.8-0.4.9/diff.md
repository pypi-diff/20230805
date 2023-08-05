# Comparing `tmp/score_models-0.4.8.tar.gz` & `tmp/score_models-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_models-0.4.8.tar", last modified: Tue Aug  1 05:47:21 2023, max compression
+gzip compressed data, was "score_models-0.4.9.tar", last modified: Sat Aug  5 18:21:08 2023, max compression
```

## Comparing `score_models-0.4.8.tar` & `score_models-0.4.9.tar`

### file list

```diff
@@ -1,63 +1,66 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.8/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 05:47:21.482461 score_models-0.4.8/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.8/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.8/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.474461 score_models-0.4.8/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.474461 score_models-0.4.8/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.8/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20889 2023-08-01 05:40:23.000000 score_models-0.4.8/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/definitions.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      517 2023-08-01 05:47:04.000000 score_models-0.4.8/score_models/dsm.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      688 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2874 2023-08-01 03:24:14.000000 score_models-0.4.8/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-08-01 03:24:14.000000 score_models-0.4.8/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3141 2023-08-01 03:24:14.000000 score_models-0.4.8/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.8/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2713 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.8/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1520 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2184 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1641 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3102 2023-07-31 23:38:29.000000 score_models-0.4.8/score_models/sliced_score_matching.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-08-01 03:00:20.000000 score_models-0.4.8/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.474461 score_models-0.4.8/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1784 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-08-01 05:47:21.000000 score_models-0.4.8/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-01 05:47:21.486461 score_models-0.4.8/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-08-01 05:45:39.000000 score_models-0.4.8/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-01 05:47:21.482461 score_models-0.4.8/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-22 02:58:16.000000 score_models-0.4.8/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7729 2023-07-31 23:38:29.000000 score_models-0.4.8/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.8/tests/test_score_models.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.8/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.355948 score_models-0.4.9/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.9/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-05 18:21:08.355948 score_models-0.4.9/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6070 2023-08-05 18:16:55.000000 score_models-0.4.9/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.9/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.351948 score_models-0.4.9/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.351948 score_models-0.4.9/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5963 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4391 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    16277 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20442 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/definitions.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      536 2023-08-05 18:13:51.000000 score_models-0.4.9/score_models/dsm.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.355948 score_models-0.4.9/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      688 2023-07-31 23:38:29.000000 score_models-0.4.9/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2874 2023-08-01 03:24:14.000000 score_models-0.4.9/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3090 2023-08-01 03:24:14.000000 score_models-0.4.9/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3141 2023-08-01 03:24:14.000000 score_models-0.4.9/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3389 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3201 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.9/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7488 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-08-05 17:19:10.000000 score_models-0.4.9/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/layers/upsample.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.355948 score_models-0.4.9/score_models/ode/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/ode/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      864 2023-08-05 18:16:55.000000 score_models-0.4.9/score_models/ode/euler.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2713 2023-07-31 23:38:29.000000 score_models-0.4.9/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.355948 score_models-0.4.9/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.9/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1520 2023-07-31 23:38:29.000000 score_models-0.4.9/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2184 2023-07-31 23:38:29.000000 score_models-0.4.9/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1641 2023-07-31 23:38:29.000000 score_models-0.4.9/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3102 2023-07-31 23:38:29.000000 score_models-0.4.9/score_models/sliced_score_matching.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4128 2023-08-05 15:21:18.000000 score_models-0.4.9/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.351948 score_models-0.4.9/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-08-05 18:21:08.000000 score_models-0.4.9/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1839 2023-08-05 18:21:08.000000 score_models-0.4.9/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-08-05 18:21:08.000000 score_models-0.4.9/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-08-05 18:21:08.000000 score_models-0.4.9/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-08-05 18:21:08.000000 score_models-0.4.9/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-08-05 18:21:08.355948 score_models-0.4.9/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-08-05 18:21:00.000000 score_models-0.4.9/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-08-05 18:21:08.355948 score_models-0.4.9/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1413 2023-08-05 18:16:55.000000 score_models-0.4.9/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7729 2023-07-31 23:38:29.000000 score_models-0.4.9/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2448 2023-08-05 18:16:55.000000 score_models-0.4.9/tests/test_score_models.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6703 2023-08-05 18:16:55.000000 score_models-0.4.9/tests/test_training.py
```

### Comparing `score_models-0.4.8/LICENSE.txt` & `score_models-0.4.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/PKG-INFO` & `score_models-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score_models
-Version: 0.4.8
+Version: 0.4.9
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `score_models-0.4.8/README.md` & `score_models-0.4.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -35,40 +35,50 @@
 of an SDE and $f_\theta : [0, 1] \times\mathbb{R}^d \to \mathbb{R}^d$ is a neural network for $\mathbf{x} \in \mathbb{R}^d$. 
 
 The `ScoreModel` class extends the `torch.nn.Module` class. Example usage:
 
 ```python
 from score_models import ScoreModel, EnergyModel, NCSNpp, MLP, DDPM
 
-# Create a ScoreModelBase instance with Yang Song's NCSN++ architecture and the VESDE
-net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
-model = ScoreModelBase(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
+# B is the batch size
+# C is the input channels
+# dimensions are the spatial dimensions (e.g. [28, 28] for MNIST)
+
+# Create a ScoreModel instance with Yang Song's NCSN++ architecture and the VESDE
+net = NCSNpp(channels=C, dimensions=len(dimensions), nf=128, ch_mult=[2, 2, 2, 2])
+model = ScoreModel(model=net, sigma_min=1e-2, sigma_max=50, device="cuda")
 # ... or the VPSDE
-model = ScoreModelBase(model=net, beta_min=1e-2, beta_max=20, device="cuda")
+model = ScoreModel(model=net, beta_min=1e-2, beta_max=20, device="cuda")
 
 # NN Architectures support a Unet with 1D convolutions for time series input data
-net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
+net = NCSNpp(channels=C, nf=128, ch_mult=[2, 2, 2, 2], dimensions=1)
 # ... or 3D convolutions for videos/voxels
 net = NCSNpp(channels=1, nf=128, ch_mult=[2, 2, 2, 2], attention=False, dimensions=3)
-# You can also use a simpler MLP architecture 
-net = MLP(dimensions=dim, layers=4, units=100)
+# You can also use a simpler MLP architecture (dimensions=0)
+net = MLP(dimensions=C, layers=4, units=100)
 # ... or Jonathan Ho's DDPM architecture
-net = DDPM(channels=1, dimensions=2, nf=128, ch_mult=[2, 2, 2, 2])
+net = DDPM(channels=1, nf=128, ch_mult=[2, 2, 2, 2])
 
 # Train the model
 model.fit(dataset=your_dataset, epochs=100, learning_rate=1e-4)
 
-# Generate samples from the trained model
-samples = model.sample(size=[batch_size, *dimensions], N=1000)
+# Generate samples from the trained model (N is the number of Euler-Maruyam steps)
+samples = model.sample(shape=[B, *dimensions], N=N)
+
+# Generate posterior samples given a likelihood score function (with a specified guidance factor, defaults to 1.)
+samples = model.sample([B, *dimensions], N, likelihood_score_fn, guidance_factor)
 
 # Compute the score for a given input
 score = model.score(t, x)
 
+# Compute the likelihood for a given input
+score = model.likelihood(t, x)
+
 # Initialise the score model and its neural network from a path to a checkpoint directory 
-score = ScoreModel(checkpoint_directory)
+score = ScoreModel(checkpoints_directory=checkpoint_directory)
 ```
 
 ### EnergyModel
 
 The `EnergyModel` class works in pretty much the same way as `ScoreModel`, but implements the score via the 
 automatic differentation of an energy model
 ```math
```

### Comparing `score_models-0.4.8/score_models/architectures/mlp.py` & `score_models-0.4.9/score_models/architectures/mlp.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,37 +3,50 @@
 from score_models.layers import GaussianFourierProjection, ScaledAttentionLayer
 from score_models.utils import get_activation
 
 
 class MLP(nn.Module):
     def __init__(
             self, 
-            dimensions, 
-            units=100, 
-            layers=2, 
-            time_embedding_dimensions=32, 
-            embedding_scale=30,
-            activation="swish",
-            time_branch_layers=1,
-            bottleneck=None,
-            attention=False,
-            nn_is_energy=False,
-            output_activation=None,
+            dimensions:int, 
+            units:int=100, 
+            layers:int=2, 
+            time_embedding_dimensions:int =32, 
+            embedding_scale:int=30,
+            activation:int="swish",
+            time_branch_layers:int=1,
+            bottleneck:int=None,
+            attention:bool=False,
+            nn_is_energy:bool=False,
+            output_activation:str=None,
+            conditioning:list[str,...]=["none"],
+            conditioning_channels:list[int,...]=None,
             **kwargs
             ):
         super().__init__()
+        self.conditioned = False
+        for c in conditioning:
+            if c.lower() not in ["none", "input"]:
+                raise ValueError(f"Conditioning must be in ['None', 'Input'], received {c}")
+            if c.lower() != "none":
+                self.conditioned = True
+                if conditioning_channels is not None:
+                    raise ValueError("conditioning_channels must be provided when the network is conditioned")
+            elif c.lower() == "none" and self.conditioned:
+                raise ValueError(f"Cannot have a mix of 'None' and other type of conditioning, received the list {conditioning}")
         self.hyperparameters = {
                 "dimensions": dimensions,
                 "units": units,
                 "layers": layers,
                 "time_embedding_dimensions": time_embedding_dimensions,
                 "embedding_scale": embedding_scale,
                 "activation": activation,
                 "time_branch_layers": time_branch_layers,
-                "nn_is_energy": nn_is_energy
+                "nn_is_energy": nn_is_energy,
+                "conditioning": conditioning
                 }
         if nn_is_energy:
             self.hyperparameters.update({"output_activation": output_activation})
         self.time_branch_layers = time_branch_layers
         self.layers = layers
         self.nn_is_energy = nn_is_energy
         t_dim = time_embedding_dimensions
```

### Comparing `score_models-0.4.8/score_models/architectures/ncsnpp.py` & `score_models-0.4.9/score_models/architectures/ncsnpp.py`

 * *Files 7% similar despite different names*

```diff
@@ -49,18 +49,31 @@
             progressive="output_skip",
             progressive_input="input_skip",
             init_scale=1e-2,
             fourier_scale=16.,
             resblock_type="biggan",
             combine_method="sum",
             attention=True,
+            conditioning:list[str,...]=["None"],
+            conditioning_channels:list[int,...]=None,
             **kwargs
           ):
         super().__init__()
-        assert dimensions in [1, 2, 3]
+        if dimensions not in [1, 2, 3]:
+            raise ValueError("Input must have 1, 2, or 3 spatial dimensions to use this architecture")
+        self.conditioned = False
+        for c in conditioning:
+            if c.lower() not in ["none", "time", "input"]:
+                raise ValueError(f"Conditioning must be in ['None', 'Time', 'Input'], received {c}")
+            if c.lower() != "none":
+                self.conditioned = True
+                if conditioning_channels is not None:
+                    raise ValueError("conditioning_channels must be provided when the network is conditioned")
+            elif c.lower() == "none" and self.conditioned:
+                raise ValueError(f"Cannot have a mix of 'None' and other type of conditioning, received the list {conditioning}")
         self.dimensions = dimensions
         self.channels = channels
         self.hyperparameters = {
             "channels": channels,
             "nf": nf,
             "activation_type": activation_type,
             "ch_mult": ch_mult,
@@ -73,15 +86,16 @@
             "progressive": progressive,
             "progressive_input": progressive_input,
             "init_scale": init_scale,
             "fourier_scale": fourier_scale,
             "resblock_type": resblock_type,
             "combine_method": combine_method,
             "attention": attention,
-            "dimensions": dimensions
+            "dimensions": dimensions,
+            "conditioning": conditioning
         }
         self.act = act = get_activation(activation_type)
         self.attention = attention
 
         self.nf = nf
         self.num_res_blocks = num_res_blocks
         self.num_resolutions = num_resolutions = len(ch_mult)
@@ -141,27 +155,24 @@
                                             )
 
         else:
             raise ValueError(f'resblock type {resblock_type} unrecognized.')
 
         # Downsampling block
         input_pyramid_ch = channels
-
         modules.append(conv3x3(channels, nf, dimensions=dimensions))
         hs_c = [nf]
-
         in_ch = nf
         for i_level in range(num_resolutions):
             # Residual blocks for this resolution
             for i_block in range(num_res_blocks):
                 out_ch = nf * ch_mult[i_level]
                 modules.append(ResnetBlock(in_ch=in_ch, out_ch=out_ch))
                 in_ch = out_ch
                 hs_c.append(in_ch)
-
             if i_level != num_resolutions - 1:
                 if resblock_type == 'ddpm':
                     modules.append(Downsample(in_ch=in_ch))
                 else:
                     modules.append(ResnetBlock(down=True, in_ch=in_ch))
 
                 if progressive_input == 'input_skip':
@@ -226,26 +237,32 @@
         if progressive != 'output_skip':
             modules.append(nn.GroupNorm(num_groups=min(in_ch // 4, 32),
                                         num_channels=in_ch, eps=1e-6))
             modules.append(conv3x3(in_ch, channels, init_scale=1., dimensions=dimensions))
 
         self.all_modules = nn.ModuleList(modules)
 
-    def forward(self, t, x):
+    def forward(self, t, x, *args):
         # timestep/noise_level embedding; only for continuous training
         modules = self.all_modules
         m_idx = 0
         # Gaussian Fourier features embeddings.
         temb = modules[m_idx](t)
         m_idx += 1
+        # if self.conditioned:
+            # if self.conditioning.lower() == "time":
+                # temb = torch.cat([temb, *args], dim=1)
         temb = modules[m_idx](temb)
         m_idx += 1
         temb = modules[m_idx](self.act(temb))
         m_idx += 1
-
+        
+        # if self.conditioning.lower() == "input":
+            # x = torch.cat([x, *args], dim=1)
+        
         # Downsampling block
         input_pyramid = None
         if self.progressive_input != 'none':
             input_pyramid = x
 
         hs = [modules[m_idx](x)]
         m_idx += 1
```

### Comparing `score_models-0.4.8/score_models/base.py` & `score_models-0.4.9/score_models/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 from typing import Callable
 
 import torch
 from torch import Tensor
 from torch.nn import Module
 from torch.func import vjp
-from .utils import DEVICE, DTYPE
+from .utils import DEVICE
 from score_models.sde import VESDE, VPSDE, SDE
 from typing import Union
 from .utils import load_architecture
 from abc import ABC, abstractmethod
 from torch_ema import ExponentialMovingAverage
 from tqdm import tqdm
-import h5py
 import time
 import os, glob, re, json
 import numpy as np
 from datetime import datetime
 from torch.utils.data import DataLoader, Dataset
 
 
-# TODO support data parallel
 class ScoreModelBase(Module, ABC):
     def __init__(self, model: Union[str, Module]=None, sde:SDE=None, checkpoints_directory=None, device=DEVICE, **hyperparameters):
         super().__init__()
         if model is None and checkpoints_directory is None:
-            raise ValueError("Must provide one of 'model'i or 'checkpoints_directory'")
+            raise ValueError("Must provide one of 'model' or 'checkpoints_directory'")
         if model is None or isinstance(model, str):
             model, hyperparams = load_architecture(checkpoints_directory, model=model, device=device, hyperparameters=hyperparameters)
             hyperparameters.update(hyperparams)
         elif hasattr(model, "hyperparameters"):
             hyperparameters.update(model.hyperparameters)
         if sde is None:
             if "sigma_min" in hyperparameters.keys():
@@ -47,14 +45,15 @@
                     hyperparameters["epsilon"] = 1e-5
                 sde = VPSDE(
                         beta_min=hyperparameters["beta_min"], 
                         beta_max=hyperparameters["beta_max"], 
                         T=hyperparameters["T"],
                         epsilon=hyperparameters["epsilon"]
                         )
+        hyperparameters["model_architecture"] = model.__class__.__name__
         self.hyperparameters = hyperparameters
         self.checkpoints_directory = checkpoints_directory
         self.model = model
         self.model.to(device)
         self.sde = sde
         self.device = device
 
@@ -87,19 +86,19 @@
         f = lambda x: drift_fn(t, x)
         _, vjp_func = vjp(f, samples)
         divergence = (vectors * vjp_func(vectors)[0]).flatten(1).sum(dim=1)
         return divergence
     
     def log_likelihood(
             self, 
+            t,
             x,
             ode_steps: int, 
             n_cotangent_vectors: int = 1, 
             noise_type="rademacher", 
-            epsilon=0.,
             verbose=0
             ) -> Tensor:
         """
         A basic implementation of Euler discretisation method of the ODE associated 
         with the marginales of the learned SDE.
         
         ode_steps: Number of steps to perform in the ODE
@@ -114,19 +113,19 @@
         (Chen et al. 2018,https://arxiv.org/abs/1806.07366)
         See also Song et al. 2020, https://arxiv.org/abs/2011.13456)
         """
         kwargs = {"n_cotangent_vectors": n_cotangent_vectors, "noise_type": noise_type}
         disable = False if verbose else True  
         B, *D = x.shape
         log_p = 0.
-        dt = 1 / ode_steps
-        t = torch.zeros(B).to(x.device) + epsilon
+        dt = t / ode_steps
         for _ in tqdm(range(ode_steps), disable=disable):
-            x = x + self.ode_drift(t, x) * dt
+            x = x + self.ode_drift(t, x) * dt.view(-1, *[1]*len(D))
             log_p += self.divergence(self.ode_drift, t, x, **kwargs) * dt
+            t = t + dt
         log_p = self.sde.prior(D).log_prob(x)
         return log_p
     
     def score_at_zero_temperature(
             self, 
             x,
             ode_steps: int, 
@@ -152,34 +151,33 @@
         if return_ll:
             return score, ll
         return score
     
     @torch.no_grad()
     def sample(
             self, 
-            n, 
             shape, 
             steps, 
             likelihood_score_fn:Callable=None,
             guidance_factor=1.
             ):
         """
-        n: Number of samples to draw
-        shape: Shape of the tensor to sample, except batch dimension.
+        shape: Shape of the tensor to sample (including batch size)
         steps: Number of Euler-Maruyam steps to perform
         likelihood_score_fn: Add an additional drift to the sampling for posterior sampling. Must have the signature f(t, x)
         guidance_factor: Multiplicative factor for the likelihood drift
         """
+        B, *D = shape
         sampling_from = "prior" if likelihood_score_fn is None else "posterior"
         if likelihood_score_fn is None:
             likelihood_score_fn = lambda t, x: 0.
         # A simple Euler-Maruyama integration of the model SDE
-        x = self.sde.prior(shape).sample([n]).to(self.device)
+        x = self.sde.prior(D).sample([B]).to(self.device)
         dt = -self.sde.T / steps
-        t = torch.ones(n).to(self.device) * self.sde.T
+        t = torch.ones(B).to(self.device) * self.sde.T
         for _ in (pbar := tqdm(range(steps))):
             pbar.set_description(f"Sampling from the {sampling_from} | t = {t[0].item():.1f} | sigma = {self.sde.sigma(t)[0].item():.1e}"
                                  f"| scale ~ {x.max().item():.1e}")
             g = self.sde.diffusion(t, x)
             f = self.sde.drift(t, x) - g**2 * (self.score(t, x) + guidance_factor * likelihood_score_fn(t, x))
             dw = torch.randn_like(x) * (-dt)**(1/2)
             x_mean = x + f * dt
@@ -263,39 +261,30 @@
             checkpoints_directory = self.checkpoints_directory
         
         if preprocessing_fn is not None:
             preprocessing_name = preprocessing_fn.__name__
         else:
             preprocessing_name = None
             preprocessing_fn = lambda x: x
-        
-        hyperparameters = self.model.hyperparameters
-        if isinstance(self.sde, VPSDE):
-            hyperparameters["sde"] = "vpsde"
-            hyperparameters["beta_min"] = self.sde.beta_min
-            hyperparameters["beta_max"] = self.sde.beta_max
-        elif isinstance(self.sde, VESDE):
-            hyperparameters["sde"] = "vesde"
-            hyperparameters["sigma_min"] = self.sde.sigma_min
-            hyperparameters["sigma_max"] = self.sde.sigma_max
-        hyperparameters["epsilon"] = self.sde.epsilon
-        hyperparameters["T"] = self.sde.T
-
+         
        # ==== Take care of where to write checkpoints and stuff =================================================================
         if checkpoints_directory is not None:
             if os.path.isdir(checkpoints_directory):
                 logname = os.path.split(checkpoints_directory)[-1]
         elif logname is None:
             logname = logname_prefix + "_" + datetime.now().strftime("%y%m%d%H%M%S")
 
         save_checkpoint = False
+        latest_checkpoint = 0
         if checkpoints_directory is not None or logdir is not None:
             save_checkpoint = True
-            if checkpoints_directory is None: # the way to create a new directory is using logdir
+            if checkpoints_directory is None:
                 checkpoints_directory = os.path.join(logdir, logname)
+            if not os.path.isdir(checkpoints_directory):
+                os.mkdir(checkpoints_directory)
                 with open(os.path.join(checkpoints_directory, "script_params.json"), "w") as f:
                     json.dump(
                         {
                             "preprocessing": preprocessing_name,
                             "learning_rate": learning_rate,
                             "ema_decay": ema_decay,
                             "batch_size": batch_size,
@@ -314,15 +303,15 @@
                             "logname": logname,
                             "logname_prefix": logname_prefix,
                         },
                         f,
                         indent=4
                     )
                 with open(os.path.join(checkpoints_directory, "model_hparams.json"), "w") as f:
-                    json.dump(hyperparameters, f, indent=4)
+                    json.dump(self.hyperparameters, f, indent=4)
 
             # ======= Load model if model_id is provided ===============================================================
             paths = glob.glob(os.path.join(checkpoints_directory, "checkpoint*.pt"))
             opt_paths = glob.glob(os.path.join(checkpoints_directory, "optimizer*.pt"))
             checkpoint_indices = [int(re.findall('[0-9]+', os.path.split(path)[-1])[-1]) for path in paths]
             scores = [float(re.findall('([0-9]{1}.[0-9]+e[+-][0-9]{2})', os.path.split(path)[-1])[-1]) for path in paths]
             if checkpoint_indices:
@@ -336,20 +325,17 @@
                     max_checkpoint_index = np.argmax(checkpoint_indices)
                     checkpoint_path = paths[max_checkpoint_index]
                     opt_path = opt_paths[max_checkpoint_index]
                     self.model.load_state_dict(torch.load(checkpoint_path, map_location=self.device))
                     optimizer.load_state_dict(torch.load(opt_path, map_location=self.device))
                     print(f"Loaded checkpoint {checkpoint_indices[max_checkpoint_index]} of {logname}")
                     latest_checkpoint = checkpoint_indices[max_checkpoint_index]
-                latest_checkpoint = 0
 
         if seed is not None:
             torch.manual_seed(seed)
-
-
         best_loss = float('inf')
         losses = []
         step = 0
         global_start = time.time()
         estimated_time_for_epoch = 0
         out_of_time = False
 
@@ -359,19 +345,23 @@
             epoch_start = time.time()
             time_per_step_epoch_mean = 0
             cost = 0
             data_iter = iter(dataloader)
             for _ in range(n_iterations_in_epoch):
                 start = time.time()
                 try:
-                    x = next(data_iter)
-                    x, *args = next(data_iter)
+                    X = next(data_iter)
                 except StopIteration:
                     data_iter = iter(dataloader)
-                    x, *args = next(data_iter)
+                    X = next(data_iter)
+                if isinstance(X, list):
+                    x, *args = X
+                else:
+                    x = X
+                    args = []
                 if preprocessing_fn is not None:
                     x = preprocessing_fn(x)
                 optimizer.zero_grad()
                 loss = self.loss_fn(x, *args)
                 loss.backward()
 
                 if step < warmup:
```

### Comparing `score_models-0.4.8/score_models/definitions.py` & `score_models-0.4.9/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/dsm.py` & `score_models-0.4.9/score_models/dsm.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,12 +3,12 @@
 import torch
 from torch import Tensor
 from .score_model import ScoreModel, EnergyModel
 
 def denoising_score_matching(score_model: Union[ScoreModel, EnergyModel], samples: Tensor):
     B, *D = samples.shape
     sde = score_model.sde
-    z = torch.randn_like(x)
+    z = torch.randn_like(samples)
     t = torch.rand(B).to(score_model.device) * (sde.T - sde.epsilon) + sde.epsilon
-    mean, sigma = sde.marginal_prob(t, x)
-    return torch.sum((z + sigma * self(t, mean + sigma * z)) ** 2) / B
+    mean, sigma = sde.marginal_prob(t, samples)
+    return torch.sum((z + sigma * score_model(t, mean + sigma * z)) ** 2) / B
```

### Comparing `score_models-0.4.8/score_models/layers/__init__.py` & `score_models-0.4.9/score_models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/attention_block.py` & `score_models-0.4.9/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/combine.py` & `score_models-0.4.9/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.4.9/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.4.9/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.4.9/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conv1dsame.py` & `score_models-0.4.9/score_models/layers/conv1dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conv2dsame.py` & `score_models-0.4.9/score_models/layers/conv2dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conv3dsame.py` & `score_models-0.4.9/score_models/layers/conv3dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/conv_layers.py` & `score_models-0.4.9/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/ddpm_resnet_block.py` & `score_models-0.4.9/score_models/layers/ddpm_resnet_block.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,23 +43,23 @@
 
 class DDPMResnetBlock(nn.Module):
     """The ResNet Blocks used in DDPM."""
     def __init__(self, act, in_ch, out_ch=None, temb_dim=None, conv_shortcut=False, dropout=0.1, dimensions=2):
         super().__init__()
         if out_ch is None:
             out_ch = in_ch
-        self.GroupNorm_0 = nn.GroupNorm(num_groups=32, num_channels=in_ch, eps=1e-6)
+        self.GroupNorm_0 = nn.GroupNorm(num_groups=min(in_ch // 4, 32), num_channels=in_ch, eps=1e-6)
         self.act = act
         self.Conv_0 = conv3x3(in_ch, out_ch, dimensions=dimensions)
         if temb_dim is not None:
             self.Dense_0 = nn.Linear(temb_dim, out_ch)
             self.Dense_0.weight.data = default_init()(self.Dense_0.weight.data.shape)
             nn.init.zeros_(self.Dense_0.bias)
 
-        self.GroupNorm_1 = nn.GroupNorm(num_groups=32, num_channels=out_ch, eps=1e-6)
+        self.GroupNorm_1 = nn.GroupNorm(num_groups=min(out_ch // 4, 32), num_channels=out_ch, eps=1e-6)
         self.Dropout_0 = nn.Dropout(dropout)
         self.Conv_1 = conv3x3(out_ch, out_ch, dimensions=dimensions)
         if in_ch != out_ch:
             if conv_shortcut:
                 self.Conv_2 = conv3x3(in_ch, out_ch, dimensions=dimensions)
             else:
                 self.NIN_0 = NIN(in_ch, out_ch)
```

### Comparing `score_models-0.4.8/score_models/layers/downsample.py` & `score_models-0.4.9/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/ncsn_resnet_block.py` & `score_models-0.4.9/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/projection_embedding.py` & `score_models-0.4.9/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/resnet_block_biggan.py` & `score_models-0.4.9/score_models/layers/resnet_block_biggan.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         h = self.act(self.GroupNorm_0(x))
 
         if self.up:
             if self.fir:
                 h = upsample(h, self.fir_kernel, factor=2, dimensions=self.dimensions)
                 x = upsample(x, self.fir_kernel, factor=2, dimensions=self.dimensions)
             else:
-                print("hello")
                 h = naive_upsample(h, factor=2, dimensions=self.dimensions)
                 x = naive_upsample(x, factor=2, dimensions=self.dimensions)
         elif self.down:
             if self.fir:
                 h = downsample(h, self.fir_kernel, factor=2, dimensions=self.dimensions)
                 x = downsample(x, self.fir_kernel, factor=2, dimensions=self.dimensions)
             else:
```

### Comparing `score_models-0.4.8/score_models/layers/spectral_normalization.py` & `score_models-0.4.9/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/squeeze_and_excitation.py` & `score_models-0.4.9/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/style_gan_conv.py` & `score_models-0.4.9/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/up_or_downsampling.py` & `score_models-0.4.9/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/up_or_downsampling1d.py` & `score_models-0.4.9/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/up_or_downsampling2d.py` & `score_models-0.4.9/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/up_or_downsampling3d.py` & `score_models-0.4.9/score_models/layers/up_or_downsampling3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 __all__ = ["naive_upsample_3d", "naive_downsample_3d", 
            "upsample_3d", "downsample_3d",
            "conv_downsample_3d", "upsample_conv_3d"
            ]
 
 
 def naive_upsample_3d(x, factor=2):
-    print("hello")
     _N, C, H, W, D = x.shape
     x = torch.reshape(x, (-1, C, H, 1, W, 1, D, 1))
     x = x.repeat(1, 1, 1, factor, 1, factor, 1, factor)
     return torch.reshape(x, (-1, C, H * factor, W * factor, D * factor))
 
 
 def naive_downsample_3d(x, factor=2):
```

### Comparing `score_models-0.4.8/score_models/layers/upfirdn1d.py` & `score_models-0.4.9/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/upfirdn2d.py` & `score_models-0.4.9/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/upfirdn3d.py` & `score_models-0.4.9/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/layers/upsample.py` & `score_models-0.4.9/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/score_model.py` & `score_models-0.4.9/score_models/score_model.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/sde/sde.py` & `score_models-0.4.9/score_models/sde/sde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/sde/vesde.py` & `score_models-0.4.9/score_models/sde/vesde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/sde/vpsde.py` & `score_models-0.4.9/score_models/sde/vpsde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/sliced_score_matching.py` & `score_models-0.4.9/score_models/sliced_score_matching.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models/utils.py` & `score_models-0.4.9/score_models/utils.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/score_models.egg-info/PKG-INFO` & `score_models-0.4.9/score_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-models
-Version: 0.4.8
+Version: 0.4.9
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `score_models-0.4.8/score_models.egg-info/SOURCES.txt` & `score_models-0.4.9/score_models.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,16 @@
 score_models/layers/up_or_downsampling1d.py
 score_models/layers/up_or_downsampling2d.py
 score_models/layers/up_or_downsampling3d.py
 score_models/layers/upfirdn1d.py
 score_models/layers/upfirdn2d.py
 score_models/layers/upfirdn3d.py
 score_models/layers/upsample.py
+score_models/ode/__init__.py
+score_models/ode/euler.py
 score_models/sde/__init__.py
 score_models/sde/sde.py
 score_models/sde/vesde.py
 score_models/sde/vpsde.py
 tests/test_architectures.py
 tests/test_layers.py
 tests/test_score_models.py
```

### Comparing `score_models-0.4.8/setup.py` & `score_models-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name="score_models",
-	version="0.4.8",
+	version="0.4.9",
     description="A simple pytorch interface for score model and basic diffusion.",
     long_description=long_description,
     author="Alexandre Adam",
     author_email="alexandre.adam@umontreal.ca",
     url="https://github.com/AlexandreAdam/torch_score_models",
     packages=find_packages(),
     install_requires=[
```

### Comparing `score_models-0.4.8/tests/test_architectures.py` & `score_models-0.4.9/tests/test_architectures.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 
 def test_ddpm():
     x = torch.randn(size=[1, 1, 32, 32]) * 230
     t = torch.randn([1])
     model = DDPM(1, nf=64, ch_mult=(1, 1, 2, 2))
     model(x=x, t=t)
 
+def test_ddpm_smallnf():
+    x = torch.randn(size=[1, 1, 32, 32]) * 230
+    t = torch.randn([1])
+    model = DDPM(1, nf=8, ch_mult=(1, 1, 2, 2))
+    model(x=x, t=t)
 
 def test_ncsnpp():
     x = torch.randn(size=[1, 1, 32, 32]) * 500
     t = torch.randn([1])
-    model = NCSNpp(1, dimensions=2, nf=8, ch_mult=(1, 1, 2, 2))
+    model = NCSNpp(1, dimensions=2, nf=8, ch_mult=(2, 2, 2, 2), num_res_blocks=3)
     model(x=x, t=t)
 
-
 def test_ncsnpp1d():
     x = torch.randn(size=[1, 1, 256]) * 500
     t = torch.randn([1])
     model = NCSNpp(1, dimensions=1, nf=8, ch_mult=(1, 1, 2, 2), attention=True)
     model(x=x, t=t)
```

### Comparing `score_models-0.4.8/tests/test_layers.py` & `score_models-0.4.9/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.8/tests/test_score_models.py` & `score_models-0.4.9/tests/test_score_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,32 +52,34 @@
         score = ScoreModel(net)
 
 def test_log_likelihood():
     net = MLP(dimensions=2)
     score = ScoreModel(net, beta_min=1e-2, beta_max=10)
     print(score.sde)
     x = torch.randn(3, 2)
-    ll = score.log_likelihood(x, ode_steps=10, verbose=1, epsilon=1e-5)
+    t = torch.rand(3)
+    ll = score.log_likelihood(t, x, ode_steps=10, verbose=1)
     print(ll)
     assert ll.shape == torch.Size([3])
 
 def test_score_at_zero_t():
     net = MLP(dimensions=2)
     score = ScoreModel(net, beta_min=1e-2, beta_max=10)
     print(score.sde)
     x = torch.randn(3, 2)
-    ll, vjp_func = torch.func.vjp(lambda x: score.log_likelihood(x, ode_steps=10, epsilon=1e-5), x)
+    t = torch.rand(3)
+    ll, vjp_func = torch.func.vjp(lambda x: score.log_likelihood(t, x, ode_steps=10), x)
     grad = vjp_func(torch.ones_like(ll))
     print(grad)
 
 def test_sample_fn():
     net = NCSNpp(1, nf=8, ch_mult=(2, 2))
     score = ScoreModel(net, sigma_min=1e-2, sigma_max=10)
-    score.sample(5, shape=[1, 16, 16], steps=10)
+    score.sample(shape=[5, 1, 16, 16], steps=10)
 
     net = DDPM(1, nf=32, ch_mult=(2, 2))
     score = ScoreModel(net, beta_min=1e-2, beta_max=10)
-    score.sample(5, shape=[1, 16, 16], steps=10)
-
-    
+    score.sample(shape=[5, 1, 16, 16], steps=10)
 
     
+if __name__ == "__main__":
+    local_test_loading_model_and_score_fn()
```

