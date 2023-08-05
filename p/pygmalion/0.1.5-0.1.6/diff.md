# Comparing `tmp/pygmalion-0.1.5.tar.gz` & `tmp/pygmalion-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmalion-0.1.5.tar", last modified: Thu May 11 00:52:19 2023, max compression
+gzip compressed data, was "pygmalion-0.1.6.tar", last modified: Sat Aug  5 18:15:22 2023, max compression
```

## Comparing `pygmalion-0.1.5.tar` & `pygmalion-0.1.6.tar`

### file list

```diff
@@ -1,90 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.081575 pygmalion-0.1.5/
--rw-rw-rw-   0        0        0     1085 2023-02-19 10:00:21.000000 pygmalion-0.1.5/LICENSE
--rw-rw-rw-   0        0        0     7481 2023-05-11 00:52:19.081575 pygmalion-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     6942 2023-03-27 11:47:38.000000 pygmalion-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.001438 pygmalion-0.1.5/pygmalion/
--rw-rw-rw-   0        0        0      179 2023-02-26 08:55:42.000000 pygmalion-0.1.5/pygmalion/__init__.py
--rw-rw-rw-   0        0        0       53 2023-05-11 00:51:54.000000 pygmalion-0.1.5/pygmalion/_info.py
--rw-rw-rw-   0        0        0     1858 2023-04-08 20:30:29.000000 pygmalion-0.1.5/pygmalion/_model.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.021431 pygmalion-0.1.5/pygmalion/datasets/
--rw-rw-rw-   0        0        0      369 2023-04-17 09:37:44.000000 pygmalion-0.1.5/pygmalion/datasets/__init__.py
--rw-rw-rw-   0        0        0      416 2023-04-08 21:42:37.000000 pygmalion-0.1.5/pygmalion/datasets/_airline_tweets.py
--rw-rw-rw-   0        0        0      334 2023-04-08 21:42:48.000000 pygmalion-0.1.5/pygmalion/datasets/_aquarium.py
--rw-rw-rw-   0        0        0      353 2023-04-08 21:42:46.000000 pygmalion-0.1.5/pygmalion/datasets/_boston_housing.py
--rw-rw-rw-   0        0        0      342 2023-04-08 21:42:51.000000 pygmalion-0.1.5/pygmalion/datasets/_cityscapes.py
--rw-rw-rw-   0        0        0      341 2023-04-08 21:43:00.000000 pygmalion-0.1.5/pygmalion/datasets/_fashion_mnist.py
--rw-rw-rw-   0        0        0      323 2023-04-08 21:43:03.000000 pygmalion-0.1.5/pygmalion/datasets/_iris.py
--rw-rw-rw-   0        0        0      385 2023-04-08 21:43:06.000000 pygmalion-0.1.5/pygmalion/datasets/_sentence_pairs.py
--rw-rw-rw-   0        0        0      332 2023-04-08 21:43:09.000000 pygmalion-0.1.5/pygmalion/datasets/_titanic.py
--rw-rw-rw-   0        0        0      330 2023-04-17 09:37:25.000000 pygmalion-0.1.5/pygmalion/datasets/_usa_economy.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.040742 pygmalion-0.1.5/pygmalion/datasets/generators/
--rw-rw-rw-   0        0        0      159 2023-04-08 20:29:21.000000 pygmalion-0.1.5/pygmalion/datasets/generators/__init__.py
--rw-rw-rw-   0        0        0     3698 2023-02-26 08:07:23.000000 pygmalion-0.1.5/pygmalion/datasets/generators/_circles_generator.py
--rw-rw-rw-   0        0        0     2335 2023-03-18 11:53:06.000000 pygmalion-0.1.5/pygmalion/datasets/generators/_roman_numerals_generator.py
--rw-rw-rw-   0        0        0     4063 2023-04-11 18:11:29.000000 pygmalion-0.1.5/pygmalion/datasets/generators/_shapes_generator.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.041749 pygmalion-0.1.5/pygmalion/neural_networks/
--rw-rw-rw-   0        0        0      383 2023-04-09 11:47:43.000000 pygmalion-0.1.5/pygmalion/neural_networks/__init__.py
--rw-rw-rw-   0        0        0     9292 2023-04-09 13:28:07.000000 pygmalion-0.1.5/pygmalion/neural_networks/_conversions.py
--rw-rw-rw-   0        0        0     3159 2023-05-08 18:56:45.000000 pygmalion-0.1.5/pygmalion/neural_networks/_dense_classifier.py
--rw-rw-rw-   0        0        0     3925 2023-05-08 19:14:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/_dense_regressor.py
--rw-rw-rw-   0        0        0     2618 2023-05-01 13:40:52.000000 pygmalion-0.1.5/pygmalion/neural_networks/_image_classifier.py
--rw-rw-rw-   0        0        0    15671 2023-05-01 13:37:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/_image_object_detector.py
--rw-rw-rw-   0        0        0     3917 2023-05-10 06:32:14.000000 pygmalion-0.1.5/pygmalion/neural_networks/_image_segmenter.py
--rw-rw-rw-   0        0        0     4627 2023-04-28 08:55:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/_loss_functions.py
--rw-rw-rw-   0        0        0    12897 2023-05-01 14:08:12.000000 pygmalion-0.1.5/pygmalion/neural_networks/_neural_network.py
--rw-rw-rw-   0        0        0     6341 2023-04-24 21:23:40.000000 pygmalion-0.1.5/pygmalion/neural_networks/_text_classifier.py
--rw-rw-rw-   0        0        0     6484 2023-04-26 18:21:07.000000 pygmalion-0.1.5/pygmalion/neural_networks/_text_segmenter.py
--rw-rw-rw-   0        0        0    18204 2023-04-24 21:24:15.000000 pygmalion-0.1.5/pygmalion/neural_networks/_text_translator.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.052365 pygmalion-0.1.5/pygmalion/neural_networks/layers/
--rw-rw-rw-   0        0        0      235 2023-05-08 18:36:43.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/__init__.py
--rw-rw-rw-   0        0        0     1218 2023-04-08 21:26:11.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_activation.py
--rw-rw-rw-   0        0        0     1698 2023-05-08 19:15:35.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_dropout.py
--rw-rw-rw-   0        0        0     6262 2023-05-08 19:14:00.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_normalization.py
--rw-rw-rw-   0        0        0     2375 2023-05-01 13:38:55.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/_positional_encoding.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.052365 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/
--rw-rw-rw-   0        0        0      285 2023-05-01 12:29:29.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/__init__.py
--rw-rw-rw-   0        0        0     2614 2023-05-08 18:29:06.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_conv_block.py
--rw-rw-rw-   0        0        0     3090 2023-05-01 12:53:43.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_padded_conv.py
--rw-rw-rw-   0        0        0     4082 2023-05-01 14:00:12.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_stack.py
--rw-rw-rw-   0        0        0     3319 2023-05-01 13:58:21.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_stages.py
--rw-rw-rw-   0        0        0     1791 2023-02-24 15:48:47.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_upsampling.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.060871 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/
--rw-rw-rw-   0        0        0      108 2023-05-01 13:38:49.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/__init__.py
--rw-rw-rw-   0        0        0    11373 2023-03-18 18:53:35.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_attention.py
--rw-rw-rw-   0        0        0     4689 2023-03-18 18:52:48.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_multihead_attention.py
--rw-rw-rw-   0        0        0     4887 2023-03-14 08:58:05.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stack.py
--rw-rw-rw-   0        0        0     6543 2023-04-24 21:25:22.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stages.py
--rw-rw-rw-   0        0        0     1333 2023-03-13 14:05:17.000000 pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_utilities.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.061881 pygmalion-0.1.5/pygmalion/tokenizers/
--rw-rw-rw-   0        0        0      188 2023-03-11 22:05:58.000000 pygmalion-0.1.5/pygmalion/tokenizers/__init__.py
--rw-rw-rw-   0        0        0     1452 2023-03-27 11:23:04.000000 pygmalion-0.1.5/pygmalion/tokenizers/_ascii_char_tokenizer.py
--rw-rw-rw-   0        0        0     9881 2023-04-08 22:43:59.000000 pygmalion-0.1.5/pygmalion/tokenizers/_byte_pair_encoder.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.061881 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/
--rw-rw-rw-   0        0        0      176 2023-04-08 21:17:04.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/__init__.py
--rw-rw-rw-   0        0        0     2736 2023-03-03 15:19:46.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_bytes_tree.py
--rw-rw-rw-   0        0        0     1334 2023-02-26 17:57:11.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_functions.py
--rw-rw-rw-   0        0        0      483 2023-02-26 09:01:48.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_special_token.py
--rw-rw-rw-   0        0        0     3709 2023-04-08 21:17:06.000000 pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_tokenizer.py
--rw-rw-rw-   0        0        0     3004 2023-03-10 17:17:36.000000 pygmalion-0.1.5/pygmalion/tokenizers/_words_tokenizer.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.061881 pygmalion-0.1.5/pygmalion/unsupervised/
--rw-rw-rw-   0        0        0       22 2023-02-26 08:42:10.000000 pygmalion-0.1.5/pygmalion/unsupervised/__init__.py
--rw-rw-rw-   0        0        0     3469 2023-04-08 20:31:17.000000 pygmalion-0.1.5/pygmalion/unsupervised/pca.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.081575 pygmalion-0.1.5/pygmalion/utilities/
--rw-rw-rw-   0        0        0      277 2023-04-08 21:44:23.000000 pygmalion-0.1.5/pygmalion/utilities/__init__.py
--rw-rw-rw-   0        0        0     2677 2023-02-19 10:02:35.000000 pygmalion-0.1.5/pygmalion/utilities/_cross_validation.py
--rw-rw-rw-   0        0        0     3775 2023-02-19 10:00:21.000000 pygmalion-0.1.5/pygmalion/utilities/_decorators.py
--rw-rw-rw-   0        0        0     2215 2023-04-09 11:51:21.000000 pygmalion-0.1.5/pygmalion/utilities/_download.py
--rw-rw-rw-   0        0        0     1774 2023-04-11 20:17:18.000000 pygmalion-0.1.5/pygmalion/utilities/_load_model.py
--rw-rw-rw-   0        0        0     6453 2023-02-19 10:02:35.000000 pygmalion-0.1.5/pygmalion/utilities/_metrics.py
--rw-rw-rw-   0        0        0     6916 2023-04-10 18:08:54.000000 pygmalion-0.1.5/pygmalion/utilities/_ploting.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.021431 pygmalion-0.1.5/pygmalion.egg-info/
--rw-rw-rw-   0        0        0     7481 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3066 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-11 00:52:18.000000 pygmalion-0.1.5/pygmalion.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-11 00:52:19.081575 pygmalion-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1262 2023-03-31 19:08:49.000000 pygmalion-0.1.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-11 00:52:19.081575 pygmalion-0.1.5/test/
--rw-rw-rw-   0        0        0      596 2023-03-14 13:51:25.000000 pygmalion-0.1.5/test/test_decoder_stage.py
--rw-rw-rw-   0        0        0     5062 2023-03-12 12:47:08.000000 pygmalion-0.1.5/test/test_kernelized_attention.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.301005 pygmalion-0.1.6/
+-rw-rw-rw-   0        0        0     1085 2023-02-19 10:00:21.000000 pygmalion-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0     8318 2023-08-05 18:15:22.300004 pygmalion-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     7770 2023-08-05 18:09:26.000000 pygmalion-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.209012 pygmalion-0.1.6/pygmalion/
+-rw-rw-rw-   0        0        0      208 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/__init__.py
+-rw-rw-rw-   0        0        0       53 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/_info.py
+-rw-rw-rw-   0        0        0     1858 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/_model.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.240177 pygmalion-0.1.6/pygmalion/datasets/
+-rw-rw-rw-   0        0        0      369 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/__init__.py
+-rw-rw-rw-   0        0        0      399 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_airline_tweets.py
+-rw-rw-rw-   0        0        0      334 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_aquarium.py
+-rw-rw-rw-   0        0        0      336 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_boston_housing.py
+-rw-rw-rw-   0        0        0      342 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_cityscapes.py
+-rw-rw-rw-   0        0        0      341 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_fashion_mnist.py
+-rw-rw-rw-   0        0        0      306 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_iris.py
+-rw-rw-rw-   0        0        0      385 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_sentence_pairs.py
+-rw-rw-rw-   0        0        0      315 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_titanic.py
+-rw-rw-rw-   0        0        0      330 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/_usa_economy.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.244181 pygmalion-0.1.6/pygmalion/datasets/generators/
+-rw-rw-rw-   0        0        0      230 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/generators/__init__.py
+-rw-rw-rw-   0        0        0     3698 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/generators/_circles_generator.py
+-rw-rw-rw-   0        0        0     5703 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/generators/_orbital_trajectory_generator.py
+-rw-rw-rw-   0        0        0     2335 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/generators/_roman_numerals_generator.py
+-rw-rw-rw-   0        0        0     4063 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/datasets/generators/_shapes_generator.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.248185 pygmalion-0.1.6/pygmalion/decision_trees/
+-rw-rw-rw-   0        0        0      254 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/decision_trees/__init__.py
+-rw-rw-rw-   0        0        0     7918 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/decision_trees/_branch.py
+-rw-rw-rw-   0        0        0    11868 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/decision_trees/_decision_tree.py
+-rw-rw-rw-   0        0        0     5569 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/decision_trees/_gradient_boosting_classifier.py
+-rw-rw-rw-   0        0        0     3264 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/decision_trees/_gradient_boosting_regressor.py
+-rw-rw-rw-   0        0        0      413 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/decision_trees/_monotonicity.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.257192 pygmalion-0.1.6/pygmalion/neural_networks/
+-rw-rw-rw-   0        0        0      438 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/__init__.py
+-rw-rw-rw-   0        0        0     9340 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_conversions.py
+-rw-rw-rw-   0        0        0     3145 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_dense_classifier.py
+-rw-rw-rw-   0        0        0     3879 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_dense_regressor.py
+-rw-rw-rw-   0        0        0     2642 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_image_classifier.py
+-rw-rw-rw-   0        0        0    16227 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_image_object_detector.py
+-rw-rw-rw-   0        0        0     3953 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_image_segmenter.py
+-rw-rw-rw-   0        0        0     4627 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_loss_functions.py
+-rw-rw-rw-   0        0        0    13155 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_neural_network.py
+-rw-rw-rw-   0        0        0     6045 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_text_classifier.py
+-rw-rw-rw-   0        0        0     6161 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_text_segmenter.py
+-rw-rw-rw-   0        0        0    16953 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_text_translator.py
+-rw-rw-rw-   0        0        0     9103 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/_time_series_regressor.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.260938 pygmalion-0.1.6/pygmalion/neural_networks/layers/
+-rw-rw-rw-   0        0        0      142 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/__init__.py
+-rw-rw-rw-   0        0        0     1218 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/_activation.py
+-rw-rw-rw-   0        0        0     1698 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/_dropout.py
+-rw-rw-rw-   0        0        0     5655 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/_normalization.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.264421 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/
+-rw-rw-rw-   0        0        0      285 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/__init__.py
+-rw-rw-rw-   0        0        0     2614 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_conv_block.py
+-rw-rw-rw-   0        0        0     3090 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_padded_conv.py
+-rw-rw-rw-   0        0        0     4178 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_stack.py
+-rw-rw-rw-   0        0        0     3319 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_stages.py
+-rw-rw-rw-   0        0        0     1791 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_upsampling.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.267423 pygmalion-0.1.6/pygmalion/neural_networks/layers/positional_encoding/
+-rw-rw-rw-   0        0        0      322 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/positional_encoding/__init__.py
+-rw-rw-rw-   0        0        0     1523 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/positional_encoding/_learned_positional_encoding.py
+-rw-rw-rw-   0        0        0     1284 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/positional_encoding/_sinusoidal_positional_encoding.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.270426 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/
+-rw-rw-rw-   0        0        0      180 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/__init__.py
+-rw-rw-rw-   0        0        0     5024 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/_stack.py
+-rw-rw-rw-   0        0        0     6040 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/_stages.py
+-rw-rw-rw-   0        0        0     1325 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.283990 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/
+-rw-rw-rw-   0        0        0      369 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/__init__.py
+-rw-rw-rw-   0        0        0     9323 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/_fourier_kernel_attention.py
+-rw-rw-rw-   0        0        0    11635 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/_kernelized_attention.py
+-rw-rw-rw-   0        0        0     7110 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/_scaled_dot_product.py
+-rw-rw-rw-   0        0        0     1325 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/_utilities.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.287994 pygmalion-0.1.6/pygmalion/tokenizers/
+-rw-rw-rw-   0        0        0      188 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/__init__.py
+-rw-rw-rw-   0        0        0     1452 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_ascii_char_tokenizer.py
+-rw-rw-rw-   0        0        0     9881 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_byte_pair_encoder.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.290996 pygmalion-0.1.6/pygmalion/tokenizers/_utilities/
+-rw-rw-rw-   0        0        0      176 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_utilities/__init__.py
+-rw-rw-rw-   0        0        0     2736 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_bytes_tree.py
+-rw-rw-rw-   0        0        0     1334 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_functions.py
+-rw-rw-rw-   0        0        0      483 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_special_token.py
+-rw-rw-rw-   0        0        0     3709 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_tokenizer.py
+-rw-rw-rw-   0        0        0     3004 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/tokenizers/_words_tokenizer.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.292998 pygmalion-0.1.6/pygmalion/unsupervised/
+-rw-rw-rw-   0        0        0       23 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/unsupervised/__init__.py
+-rw-rw-rw-   0        0        0     3469 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/unsupervised/_pca.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.298003 pygmalion-0.1.6/pygmalion/utilities/
+-rw-rw-rw-   0        0        0      305 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/__init__.py
+-rw-rw-rw-   0        0        0     2677 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/_cross_validation.py
+-rw-rw-rw-   0        0        0     3544 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/_data_processing.py
+-rw-rw-rw-   0        0        0     3775 2023-02-19 10:00:21.000000 pygmalion-0.1.6/pygmalion/utilities/_decorators.py
+-rw-rw-rw-   0        0        0     2215 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/_download.py
+-rw-rw-rw-   0        0        0     1814 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/_load_model.py
+-rw-rw-rw-   0        0        0     6453 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/_metrics.py
+-rw-rw-rw-   0        0        0     6916 2023-08-05 18:09:26.000000 pygmalion-0.1.6/pygmalion/utilities/_ploting.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.233171 pygmalion-0.1.6/pygmalion.egg-info/
+-rw-rw-rw-   0        0        0     8318 2023-08-05 18:15:21.000000 pygmalion-0.1.6/pygmalion.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3979 2023-08-05 18:15:22.000000 pygmalion-0.1.6/pygmalion.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:15:21.000000 pygmalion-0.1.6/pygmalion.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2023-08-05 18:15:21.000000 pygmalion-0.1.6/pygmalion.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-05 18:15:22.000000 pygmalion-0.1.6/pygmalion.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:15:22.301571 pygmalion-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1262 2023-08-05 18:09:26.000000 pygmalion-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:15:22.299003 pygmalion-0.1.6/test/
+-rw-rw-rw-   0        0        0      596 2023-08-05 18:09:26.000000 pygmalion-0.1.6/test/test_decoder_stage.py
+-rw-rw-rw-   0        0        0     5062 2023-08-05 18:09:26.000000 pygmalion-0.1.6/test/test_kernelized_attention.py
```

### Comparing `pygmalion-0.1.5/LICENSE` & `pygmalion-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/PKG-INFO` & `pygmalion-0.1.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,189 @@
 Metadata-Version: 2.1
 Name: pygmalion
-Version: 0.1.5
+Version: 0.1.6
 Summary: A machine learning package
 Home-page: https://github.com/BFavier/Pygmalion
 Author: Benoit Favier
 Author-email: benoitfamillefavier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Pygmalion in the greek mythologie is a sculptor that fell in love with one of his creations.
-In the myth, Aphrodite gives life to Galatea, the sculpture he fell in love with. This package is a machine learning library. It contains the tools to give a mind of their own to inanimate objects.
+Pygmalion in the greek mythologie is a sculptor that fell in love with one of his creations. In the myth, Aphrodite gives life to Galatea, the sculpture he fell in love with. This package is a python machine learning library that implements models for some common machine learning tasks. Everything that you need to give a mind of their own to inanimate objects.
 
 # Installing pygmalion
 
 pygmalion can be installed through pip.
 
 ~~~
-pip install pygmalion
+python -m pip install pygmalion
 ~~~
 
 # Fast prototyping of models with pygmalion
 
-Architectures for several common machine learning tasks (regression, image classification, ...) are implemented in this package.
+Architectures for several common machine learning tasks (regression, image classification, machine translation ...) are implemented in this package.
 
-The inputs and outputs of the models are common python objects (such as numpy array and pandas dataframes) so there are few new things you need to learn to use this package.
+The inputs and outputs of the models are common python objects (such as numpy array and pandas dataframes).
 
-In this part we are going to see how to load a dataset, train a model, and display some metrics. As a first step you can import the following packages.
+In this section we are going to see how to load a dataset, train a model, display some metrics, and save a model.
 
 ~~~python
 >>> import pygmalion as ml
 >>> import pygmalion.neural_networks as nn
 >>> import pandas as pd
 >>> import numpy as np
 >>> import matplotlib.pyplot as plt
 ~~~
 
 You can download a dataset and split it with the **split** function.
 
 ~~~python
 >>> ml.datasets.boston_housing("./")
 >>> df = pd.read_csv("./boston_housing.csv")
->>> x, y = df[[c for c in d_Fcolumns if c != "medv"]], df["medv"]
->>> train_data, val_data, test_data = ml.split(x, y, frac=(0.1, 0.1))
+>>> df_train, df_val, df_test = ml.utilities.split(df, weights=(0.8, 0.1, 0.1))
 ~~~
 
-Creating and training a model is done in a few lines of code.
+Creating and training a model takes few lines of code.
 
 ~~~python
->>> hidden_layers = [{"features": 8}, {"features": 8}]
->>> model = nn.DenseRegressor(x.columns, hidden_layers)
->>> model.train(train_data, val_data, n_epochs=1000, patience=100, learning_rate=1.0E-3)
+>>> inputs, target = [c for c in df.columns if c != "medv"], "medv"
+>>> model = nn.DenseRegressor(inputs, target, hidden_layers=[32, 32])
+>>> x_train, y_train = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> x_val, y_val = model.data_to_tensor(df_val[inputs], df_val[target])
+>>> history = model.fit((x_train, y_train), (x_val, y_val), n_steps=1000, patience=100, learning_rate=1.0E-3)
 ~~~
 
 Some usefull metrics can easily be evaluated.
 
 For a regressor model, the available metrics are [**MSE**](https://en.wikipedia.org/wiki/Mean_squared_error), [**RMSE**](https://en.wikipedia.org/wiki/Root-mean-square_deviation), [**R2**](https://en.wikipedia.org/wiki/Coefficient_of_determination), and the correlation between target and prediction can be visualized with the **plot_fitting** function.
 
 ~~~python
 >>> f, ax = plt.subplots()
->>> x_train, y_train = train_data
->>> ml.plot_fitting(model(x_train), y_train, ax=ax, label="training")
->>> x_val, y_val = val_data
->>> ml.plot_fitting(model(x_val), y_val, ax=ax, label="validation")
->>> x_test, y_test = test_data
->>> ml.plot_fitting(model(x_test), y_test, ax=ax, label="testing", color="C3")
->>> R2 = ml.R2(model(x_test), y_test)
+>>> ml.utilities.plot_fitting(df_train[target], model.predict(df_train), ax=ax, label="training")
+>>> ml.utilities.plot_fitting(df_val[target], model.predict(df_val), ax=ax, label="validation")
+>>> ml.utilities.plot_fitting(df_test[target], model.predict(df_test), ax=ax, label="testing", color="C3")
+>>> R2 = ml.utilities.R2(model.predict(df_test), df_test[target])
 >>> ax.set_title(f"RÂ²={R2:.3g}")
+>>> ax.set_xlabel("target")
+>>> ax.set_ylabel("predicted")
 >>> plt.show()
 ~~~
 
 ![pairplot](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/boston_housing_pairplot.png)
 
 
 For a classifier model you can evaluate the [**accuracy**](https://en.wikipedia.org/wiki/Accuracy_and_precision#In_binary_classification), and display the confusion matrix.
 
 ~~~python
 >>> ml.datasets.iris("./")
 >>> df = pd.read_csv("./iris.csv")
->>> x, y = df[[c for c in d_Fcolumns if c != "variety"]], df["variety"]
->>> inputs, classes = x.columns(), y.unique()
->>> hidden_layers = [{"features": 5},
->>>                  {"features": 5},
->>>                  {"features": 5}]
->>> model = nn.DenseClassifier(inputs, classes,
->>>                            hidden_layers=hidden_layers,
->>>                            activation="elu")
->>> train_data, val_data, test_data = ml.split(x, y, frac=(0.2, 0.1))
->>> model.train(train_data, val_data, n_epochs=1000, patience=100)
+>>> df_train, df_val, df_test = ml.utilities.split(df, weights=(0.7, 0.2, 0.1))
+>>> inputs, target = [c for c in df.columns if c != "variety"], "variety"
+>>> classes = df[target].unique()
+>>> model = nn.DenseClassifier(inputs, target, classes, hidden_layers=[8, 8, 8])
+>>> train_data = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> val_data = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> model.fit(train_data, val_data, n_steps=1000, patience=100)
 >>> f, ax = plt.subplots()
->>> x_test, y_test = test_data
->>> ml.plot_matrix(ml.confusion_matrix(y_test, y_pred, classes=classes),
-...                ax=ax, cmap="Greens", write_values=True, format=".2%")
->>> acc = ml.accuracy(y_pred, y)*100
->>> ax.set_title(f"Accuracy: {acc:.2f}%")
+>>> y_test, y_pred = df_test[target], model.predict(df_test)
+>>> ml.utilities.plot_matrix(ml.utilities.confusion_matrix(y_test, y_pred, classes=classes), ax=ax, cmap="Greens", write_values=True, format=".2%")
+>>> acc = ml.utilities.accuracy(y_pred, y_test)
+>>> ax.set_title(f"Accuracy: {acc:.2%}")
 >>> plt.tight_layout()
 >>> plt.show()
 ~~~
 
 ![confusion matrix](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/iris_confusion_matrix.png)
 
-All the models can be dumped as a dictionnary through the **dump** property. A copy of the model can be loaded with the **from_dump** class method.
+All the models can be saved directly to the disk with the **save** method.
+A model saved on the disk can then be loaded back with the **load_model** function.
 
 ~~~python
->>> dump = model.dump
->>> model = nn.DenseRegressor.from_dump(dump)
-~~~
-
-The models can also be be saved directly to the disk in json/hdf5 format with the **save** method.
-A model saved on the disk can then be loaded back with the **load** function.
-
-~~~python
->>> model.save("./model.json")
->>> model = ml.load("./model.json")
+>>> model.save("./model.pth")
+>>> model = ml.utilities.load_model("./model.pth")
 ~~~
 
 # Implemented models
 
 For examples of model training see the **samples** folder in the [github page](https://github.com/BFavier/Pygmalion).
 
 ## Neural networks
 
 The neural networks are implemented in pytorch under the hood.
-The underlying pytorch Module and Optimizer can be accessed as the **model** and **optimizer** attributes of the model.
+Each model is a pytorch **Module**. The fit method of neural networks returns a train loss, validation loss, gradient scale history that can be ploted with the **plot_loss** functions.
 
-### **DenseRegressor**
+~~~python
+>>> train_losses, val_losses, grad, best_step = model.fit(...)
+>>> ml.utilities.plot_losses(train_losses, val_losses, grad, best_step)
+~~~
 
-A dense regressor (or multi layer perceptron regressor) predicts a scalar value given an input of several variables.
+![loss history](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/Fashion_MNIST_residuals.png)
 
-This implementation takes in input **x** a pandas.DataFrame of numerical observations, and returns **y** a numpy.ndarray of floats of the same length. The optional **weights** weighting of the observations during training are numpy.ndarray of floats.
+### **DenseRegressor**
 
-It is implemented as a sucession of hidden **Activated0d** layers (linear weighting/non linear activation/batch normalization) and a final linear weighting to reduces the number of features to one scalar prediction.
+A DenseRegressor (or multi layer perceptron regressor) predicts a scalar value given an input of several variables. An example of DenseRegressor training was demonstrated in a previous section.
 
 ### **DenseClassifier**
 
-A dense classifier (or multi layer perceptron classifier) predicts a str class value given an input of several variables.
-
-This implementation takes in input **x** a pandas.DataFrame of numerical observations, and returns **y** list of str of the same length. The optional **weights** weighting of the observations during training are numpy.ndarray of floats.
-
-Similarly to the DenseRegressor it is a succession of hidden **Activated0d** layers, and a final linear layer with as much output as there are classes to predict.
+A DenseClassifier (or multi layer perceptron classifier) predicts a str class value given an input of several variables. An example of DenseClassifier training was presented in a previous section.
 
 ### **ImageClassifier**
 
 An ImageClassifier predicts a str class given as input an image. Here below the predictions of a model trained on the fashion-MNIST dataset.
 
 ![fashion-MNIST predictions](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/Fashion_MNIST_illustration.png)
 
-It is implemented as a Convolutional Neural Network similar to LeNet.
+It is implemented as a Convolutional Neural Network similar to ResNet.
+
+### **ImageSegmenter**
 
-### **SemanticSegmenter**
+An ImageSegmenter predicts a class for each pixel of the input image (semantic segmentation). Here below the predictions of a model trained on the cityscape dataset.
 
-A SemanticSegmenter predicts a class for each pixel of the input image. Here below the predictions of a model trained on the cityscape dataset.
+![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/segmented_cityscape.png)
 
-![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/segmented_cityscape_2.png)
+It is implemented as a Convolutional Neural Network similar to U-Net.
 
-It is implemented as a Convolutional Neural Network similar to U-Net. It is a succession of convolutions/pooling followed by a succession of upsampling/convolutions, leading to a convergent/divergent feature map structure. The feature map before each downsampling stage is concatenated to the upsampling of the same size to preserve features.
+### **ImageObjectDetector**
 
+An ImageObjectDetector predict the presence and box coordinates of objects in an image. This model is an implementation of the YOLO convolutional neural network. Here below the prediction of a model trained to detect circles and squares in images generated on the fly:
 
+![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/ImageObjectDetector.png)
 
+### **TextClassifier**
+
+A TextClassifier classifies text inputs. It is implemented as a transformer encoder. Here below some prediction of the model on a sentiment analysis task where tweets were to be classified as positive, neutral or negative.
+
+~~~
+@JetBlue Thanks! Her flight leaves at 2 but she's arriving to the airport early. Wedding is in VT in Sept. Grateful you fly to BTV!! :)
+>>> positive
+
+@united how are conditions in BOS today? I'm in UA994. Everything appears to be in time but I wanted to check.
+>>> neutral
+
+@AmericanAir it's been almost 3 days and it's still frozen. Thanks doll ðŸ˜˜ðŸ˜‘
+>>> negative
+~~~
+
+### **TextTranslator**
+
+A TextTranslator model predicts a string outputs for a string inputs. It is implemented as an encoder/decoder transformer. Here below some predictions of a model trained to translate arabic numerals to roman numerals.
+
+~~~
+402 >>> ['CDII']
+863 >>> ['DCCCLXIII']
+1275 >>> ['MCCLXXV']
+798 >>> ['DCCXCVIII']
+1532 >>> ['MDXXXII']
+223 >>> ['CCXXIII']
+90 >>> ['XC']
+1261 >>> ['MCCLXI']
+1032 >>> ['MXXXII']
+432 >>> ['CDXXXII']
+~~~
```

### Comparing `pygmalion-0.1.5/README.md` & `pygmalion-0.1.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,148 +1,171 @@
-Pygmalion in the greek mythologie is a sculptor that fell in love with one of his creations.
-In the myth, Aphrodite gives life to Galatea, the sculpture he fell in love with. This package is a machine learning library. It contains the tools to give a mind of their own to inanimate objects.
+Pygmalion in the greek mythologie is a sculptor that fell in love with one of his creations. In the myth, Aphrodite gives life to Galatea, the sculpture he fell in love with. This package is a python machine learning library that implements models for some common machine learning tasks. Everything that you need to give a mind of their own to inanimate objects.
 
 # Installing pygmalion
 
 pygmalion can be installed through pip.
 
 ~~~
-pip install pygmalion
+python -m pip install pygmalion
 ~~~
 
 # Fast prototyping of models with pygmalion
 
-Architectures for several common machine learning tasks (regression, image classification, ...) are implemented in this package.
+Architectures for several common machine learning tasks (regression, image classification, machine translation ...) are implemented in this package.
 
-The inputs and outputs of the models are common python objects (such as numpy array and pandas dataframes) so there are few new things you need to learn to use this package.
+The inputs and outputs of the models are common python objects (such as numpy array and pandas dataframes).
 
-In this part we are going to see how to load a dataset, train a model, and display some metrics. As a first step you can import the following packages.
+In this section we are going to see how to load a dataset, train a model, display some metrics, and save a model.
 
 ~~~python
 >>> import pygmalion as ml
 >>> import pygmalion.neural_networks as nn
 >>> import pandas as pd
 >>> import numpy as np
 >>> import matplotlib.pyplot as plt
 ~~~
 
 You can download a dataset and split it with the **split** function.
 
 ~~~python
 >>> ml.datasets.boston_housing("./")
 >>> df = pd.read_csv("./boston_housing.csv")
->>> x, y = df[[c for c in d_Fcolumns if c != "medv"]], df["medv"]
->>> train_data, val_data, test_data = ml.split(x, y, frac=(0.1, 0.1))
+>>> df_train, df_val, df_test = ml.utilities.split(df, weights=(0.8, 0.1, 0.1))
 ~~~
 
-Creating and training a model is done in a few lines of code.
+Creating and training a model takes few lines of code.
 
 ~~~python
->>> hidden_layers = [{"features": 8}, {"features": 8}]
->>> model = nn.DenseRegressor(x.columns, hidden_layers)
->>> model.train(train_data, val_data, n_epochs=1000, patience=100, learning_rate=1.0E-3)
+>>> inputs, target = [c for c in df.columns if c != "medv"], "medv"
+>>> model = nn.DenseRegressor(inputs, target, hidden_layers=[32, 32])
+>>> x_train, y_train = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> x_val, y_val = model.data_to_tensor(df_val[inputs], df_val[target])
+>>> history = model.fit((x_train, y_train), (x_val, y_val), n_steps=1000, patience=100, learning_rate=1.0E-3)
 ~~~
 
 Some usefull metrics can easily be evaluated.
 
 For a regressor model, the available metrics are [**MSE**](https://en.wikipedia.org/wiki/Mean_squared_error), [**RMSE**](https://en.wikipedia.org/wiki/Root-mean-square_deviation), [**R2**](https://en.wikipedia.org/wiki/Coefficient_of_determination), and the correlation between target and prediction can be visualized with the **plot_fitting** function.
 
 ~~~python
 >>> f, ax = plt.subplots()
->>> x_train, y_train = train_data
->>> ml.plot_fitting(model(x_train), y_train, ax=ax, label="training")
->>> x_val, y_val = val_data
->>> ml.plot_fitting(model(x_val), y_val, ax=ax, label="validation")
->>> x_test, y_test = test_data
->>> ml.plot_fitting(model(x_test), y_test, ax=ax, label="testing", color="C3")
->>> R2 = ml.R2(model(x_test), y_test)
+>>> ml.utilities.plot_fitting(df_train[target], model.predict(df_train), ax=ax, label="training")
+>>> ml.utilities.plot_fitting(df_val[target], model.predict(df_val), ax=ax, label="validation")
+>>> ml.utilities.plot_fitting(df_test[target], model.predict(df_test), ax=ax, label="testing", color="C3")
+>>> R2 = ml.utilities.R2(model.predict(df_test), df_test[target])
 >>> ax.set_title(f"R²={R2:.3g}")
+>>> ax.set_xlabel("target")
+>>> ax.set_ylabel("predicted")
 >>> plt.show()
 ~~~
 
 ![pairplot](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/boston_housing_pairplot.png)
 
 
 For a classifier model you can evaluate the [**accuracy**](https://en.wikipedia.org/wiki/Accuracy_and_precision#In_binary_classification), and display the confusion matrix.
 
 ~~~python
 >>> ml.datasets.iris("./")
 >>> df = pd.read_csv("./iris.csv")
->>> x, y = df[[c for c in d_Fcolumns if c != "variety"]], df["variety"]
->>> inputs, classes = x.columns(), y.unique()
->>> hidden_layers = [{"features": 5},
->>>                  {"features": 5},
->>>                  {"features": 5}]
->>> model = nn.DenseClassifier(inputs, classes,
->>>                            hidden_layers=hidden_layers,
->>>                            activation="elu")
->>> train_data, val_data, test_data = ml.split(x, y, frac=(0.2, 0.1))
->>> model.train(train_data, val_data, n_epochs=1000, patience=100)
+>>> df_train, df_val, df_test = ml.utilities.split(df, weights=(0.7, 0.2, 0.1))
+>>> inputs, target = [c for c in df.columns if c != "variety"], "variety"
+>>> classes = df[target].unique()
+>>> model = nn.DenseClassifier(inputs, target, classes, hidden_layers=[8, 8, 8])
+>>> train_data = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> val_data = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> model.fit(train_data, val_data, n_steps=1000, patience=100)
 >>> f, ax = plt.subplots()
->>> x_test, y_test = test_data
->>> ml.plot_matrix(ml.confusion_matrix(y_test, y_pred, classes=classes),
-...                ax=ax, cmap="Greens", write_values=True, format=".2%")
->>> acc = ml.accuracy(y_pred, y)*100
->>> ax.set_title(f"Accuracy: {acc:.2f}%")
+>>> y_test, y_pred = df_test[target], model.predict(df_test)
+>>> ml.utilities.plot_matrix(ml.utilities.confusion_matrix(y_test, y_pred, classes=classes), ax=ax, cmap="Greens", write_values=True, format=".2%")
+>>> acc = ml.utilities.accuracy(y_pred, y_test)
+>>> ax.set_title(f"Accuracy: {acc:.2%}")
 >>> plt.tight_layout()
 >>> plt.show()
 ~~~
 
 ![confusion matrix](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/iris_confusion_matrix.png)
 
-All the models can be dumped as a dictionnary through the **dump** property. A copy of the model can be loaded with the **from_dump** class method.
+All the models can be saved directly to the disk with the **save** method.
+A model saved on the disk can then be loaded back with the **load_model** function.
 
 ~~~python
->>> dump = model.dump
->>> model = nn.DenseRegressor.from_dump(dump)
-~~~
-
-The models can also be be saved directly to the disk in json/hdf5 format with the **save** method.
-A model saved on the disk can then be loaded back with the **load** function.
-
-~~~python
->>> model.save("./model.json")
->>> model = ml.load("./model.json")
+>>> model.save("./model.pth")
+>>> model = ml.utilities.load_model("./model.pth")
 ~~~
 
 # Implemented models
 
 For examples of model training see the **samples** folder in the [github page](https://github.com/BFavier/Pygmalion).
 
 ## Neural networks
 
 The neural networks are implemented in pytorch under the hood.
-The underlying pytorch Module and Optimizer can be accessed as the **model** and **optimizer** attributes of the model.
+Each model is a pytorch **Module**. The fit method of neural networks returns a train loss, validation loss, gradient scale history that can be ploted with the **plot_loss** functions.
 
-### **DenseRegressor**
+~~~python
+>>> train_losses, val_losses, grad, best_step = model.fit(...)
+>>> ml.utilities.plot_losses(train_losses, val_losses, grad, best_step)
+~~~
 
-A dense regressor (or multi layer perceptron regressor) predicts a scalar value given an input of several variables.
+![loss history](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/Fashion_MNIST_residuals.png)
 
-This implementation takes in input **x** a pandas.DataFrame of numerical observations, and returns **y** a numpy.ndarray of floats of the same length. The optional **weights** weighting of the observations during training are numpy.ndarray of floats.
+### **DenseRegressor**
 
-It is implemented as a sucession of hidden **Activated0d** layers (linear weighting/non linear activation/batch normalization) and a final linear weighting to reduces the number of features to one scalar prediction.
+A DenseRegressor (or multi layer perceptron regressor) predicts a scalar value given an input of several variables. An example of DenseRegressor training was demonstrated in a previous section.
 
 ### **DenseClassifier**
 
-A dense classifier (or multi layer perceptron classifier) predicts a str class value given an input of several variables.
-
-This implementation takes in input **x** a pandas.DataFrame of numerical observations, and returns **y** list of str of the same length. The optional **weights** weighting of the observations during training are numpy.ndarray of floats.
-
-Similarly to the DenseRegressor it is a succession of hidden **Activated0d** layers, and a final linear layer with as much output as there are classes to predict.
+A DenseClassifier (or multi layer perceptron classifier) predicts a str class value given an input of several variables. An example of DenseClassifier training was presented in a previous section.
 
 ### **ImageClassifier**
 
 An ImageClassifier predicts a str class given as input an image. Here below the predictions of a model trained on the fashion-MNIST dataset.
 
 ![fashion-MNIST predictions](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/Fashion_MNIST_illustration.png)
 
-It is implemented as a Convolutional Neural Network similar to LeNet.
+It is implemented as a Convolutional Neural Network similar to ResNet.
+
+### **ImageSegmenter**
 
-### **SemanticSegmenter**
+An ImageSegmenter predicts a class for each pixel of the input image (semantic segmentation). Here below the predictions of a model trained on the cityscape dataset.
 
-A SemanticSegmenter predicts a class for each pixel of the input image. Here below the predictions of a model trained on the cityscape dataset.
+![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/segmented_cityscape.png)
 
-![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/segmented_cityscape_2.png)
+It is implemented as a Convolutional Neural Network similar to U-Net.
 
-It is implemented as a Convolutional Neural Network similar to U-Net. It is a succession of convolutions/pooling followed by a succession of upsampling/convolutions, leading to a convergent/divergent feature map structure. The feature map before each downsampling stage is concatenated to the upsampling of the same size to preserve features.
+### **ImageObjectDetector**
 
+An ImageObjectDetector predict the presence and box coordinates of objects in an image. This model is an implementation of the YOLO convolutional neural network. Here below the prediction of a model trained to detect circles and squares in images generated on the fly:
 
+![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/ImageObjectDetector.png)
+
+### **TextClassifier**
+
+A TextClassifier classifies text inputs. It is implemented as a transformer encoder. Here below some prediction of the model on a sentiment analysis task where tweets were to be classified as positive, neutral or negative.
+
+~~~
+@JetBlue Thanks! Her flight leaves at 2 but she's arriving to the airport early. Wedding is in VT in Sept. Grateful you fly to BTV!! :)
+>>> positive
+
+@united how are conditions in BOS today? I'm in UA994. Everything appears to be in time but I wanted to check.
+>>> neutral
+
+@AmericanAir it's been almost 3 days and it's still frozen. Thanks doll 😘😑
+>>> negative
+~~~
+
+### **TextTranslator**
+
+A TextTranslator model predicts a string outputs for a string inputs. It is implemented as an encoder/decoder transformer. Here below some predictions of a model trained to translate arabic numerals to roman numerals.
+
+~~~
+402 >>> ['CDII']
+863 >>> ['DCCCLXIII']
+1275 >>> ['MCCLXXV']
+798 >>> ['DCCXCVIII']
+1532 >>> ['MDXXXII']
+223 >>> ['CCXXIII']
+90 >>> ['XC']
+1261 >>> ['MCCLXI']
+1032 >>> ['MXXXII']
+432 >>> ['CDXXXII']
+~~~
```

### Comparing `pygmalion-0.1.5/pygmalion/_model.py` & `pygmalion-0.1.6/pygmalion/_model.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/datasets/generators/_circles_generator.py` & `pygmalion-0.1.6/pygmalion/datasets/generators/_circles_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/datasets/generators/_roman_numerals_generator.py` & `pygmalion-0.1.6/pygmalion/datasets/generators/_roman_numerals_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/datasets/generators/_shapes_generator.py` & `pygmalion-0.1.6/pygmalion/datasets/generators/_shapes_generator.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_conversions.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_conversions.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,40 +11,40 @@
                     names: List[str], device: Optional[torch.device]=None
                     ) -> torch.Tensor:
     """converts named variables to tensors"""
     if isinstance(data, dict):
         data = {k: v if hasattr(v, "__iter__") else [v] for k, v in zip(names, (data[n] for n in names))}
         data = pd.DataFrame.from_dict(data)
     if isinstance(data, pd.DataFrame):
-        data = data[names].to_numpy()
+        data = data[names].to_numpy(dtype=np.float32)
     data = floats_to_tensor(data, device=device)
     if len(data.shape) == 1:
         data = data.unsqueeze(-1)
     return data
 
 
 def floats_to_tensor(arr: Iterable, device: Optional[torch.device] = None) -> torch.Tensor:
     """converts an array of numerical values to a tensor of floats"""
     if isinstance(arr, pd.Series):
-        arr = arr.to_numpy()
+        arr = arr.to_numpy(dtype=np.float32)
     t = torch.tensor(arr, dtype=torch.float, device=device,
                      requires_grad=False)
     return t
 
 
 def tensor_to_floats(tensor: torch.Tensor) -> np.ndarray:
     """converts a torch.Tensor to a numpy.ndarray of doubles"""
     assert tensor.dtype == torch.float
     return tensor.detach().cpu().numpy()
 
 
 def longs_to_tensor(arr: Iterable, device: Optional[torch.device] = None) -> torch.Tensor:
     """converts an array of numerical values to a tensor of longs"""
     if isinstance(arr, pd.Series):
-        arr = arr.to_numpy()
+        arr = arr.to_numpy(dtype=np.float32)
     t = torch.tensor(arr, dtype=torch.long, device=device,
                      requires_grad=False)
     return t
 
 
 def tensor_to_longs(tensor: torch.Tensor) -> list:
     """converts a tensor of longs to numpy"""
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_dense_classifier.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_dense_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
         """
         super().__init__(classes)
         self.inputs = tuple(inputs)
         self.target = str(target)
         self.layers = torch.nn.ModuleList()
         in_features = len(inputs)
-        self.input_normalizer = Normalizer(1, in_features, affine=False)
+        self.input_normalizer = Normalizer(1, in_features)
         for out_features in hidden_layers:
             self.layers.append(torch.nn.Linear(in_features, out_features))
             if normalize:
                 self.layers.append(FeaturesNorm(1, out_features))
             self.layers.append(Activation(activation))
             if dropout is not None:
                 self.layers.append(Dropout(dropout))
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_dense_regressor.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_dense_regressor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import torch
 import pandas as pd
 import numpy as np
 from typing import Union, Iterable, Optional
-from ._conversions import floats_to_tensor, tensor_to_floats
+from ._conversions import tensor_to_floats
 from ._conversions import named_to_tensor, tensor_to_dataframe
 from ._neural_network import NeuralNetwork
 from ._loss_functions import MSE
 from .layers import Activation, Normalizer, FeaturesNorm, Dropout
 
 
 class DenseRegressor(NeuralNetwork):
@@ -42,25 +42,25 @@
             the dropout after each hidden layer if provided
         """
         super().__init__()
         self.inputs = tuple(inputs)
         self.target = target if isinstance(target, str) else tuple(target)
         self.layers = torch.nn.ModuleList()
         in_features = len(inputs)
-        self.input_normalizer = Normalizer(1, in_features, affine=False)
+        self.input_normalizer = Normalizer(1, in_features)
         for out_features in hidden_layers:
             self.layers.append(torch.nn.Linear(in_features, out_features))
             if normalize:
                 self.layers.append(FeaturesNorm(1, out_features))
             self.layers.append(Activation(activation))
             self.layers.append(Dropout(dropout))
             in_features = out_features
         out_features = 1 if isinstance(target, str) else len(self.target)
         self.output = torch.nn.Linear(in_features, out_features)
-        self.target_normalizer = Normalizer(1, out_features, affine=False)
+        self.target_normalizer = Normalizer(1, out_features)
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
         X = self.input_normalizer(X)
         for layer in self.layers:
             X = layer(X)
         return self.output(X)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_image_classifier.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_image_classifier.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,24 +19,24 @@
                  pooling_size: Tuple[int, int] = (2, 2),
                  stride: Tuple[int, int] = (1, 1),
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
                  dropout: Optional[float] = None,
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True):
         """
         Parameters
         ----------
         ...
         """
         super().__init__(classes)
         self.encoder = ConvolutionalEncoder(
             in_channels, features, kernel_size, pooling_size, stride, activation,
-            n_convs_per_block, normalize, residuals, dropout, low_memory)
+            n_convs_per_block, normalize, residuals, dropout, gradient_checkpointing)
         self.output = torch.nn.Linear(features[-1], len(self.classes))
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
         X = self.encoder(X)
         N, C, H, W = X.shape
         X = X.reshape(N, C, -1).mean(dim=-1)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_image_object_detector.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_image_object_detector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import torch
 import pandas as pd
 import numpy as np
 import torch.nn.functional as F
 from typing import List, Sequence, Iterable, Tuple, Optional
+from itertools import count
 from .layers.convolutions import ConvolutionalEncoder, PaddedConv2d
 from ._conversions import tensor_to_classes
 from ._conversions import classes_to_tensor, images_to_tensor, floats_to_tensor
 from ._conversions import tensor_to_probabilities
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy, RMSE
 
@@ -21,27 +22,28 @@
                  pooling_size: Tuple[int, int] = (2, 2),
                  stride: Tuple[int, int] = (1, 1),
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
                  dropout: Optional[float] = None,
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True):
         """
         Parameters
         ----------
         ...
         """
         super().__init__(classes)
-        self.cells_dimensions = tuple((s*mp) ** len(features) for s, mp in zip(stride, pooling_size or (1, 1)))
+        self.downsampling_window = tuple((s*mp) for s, mp in zip(stride or (1, 1), pooling_size or (1, 1)))
+        self.cells_dimensions = tuple(dw ** len(features) for dw in self.downsampling_window)
         self.layers = torch.nn.ModuleList()
         self.bboxes_per_cell = bboxes_per_cell
         self.encoder = ConvolutionalEncoder(
             in_channels, features, kernel_size, pooling_size, stride, activation,
-            n_convs_per_block, normalize, residuals, dropout, low_memory)
+            n_convs_per_block, normalize, residuals, dropout, gradient_checkpointing)
         self.confidence = PaddedConv2d(features[-1], self.bboxes_per_cell, kernel_size)
         self.positions = PaddedConv2d(features[-1], self.bboxes_per_cell*2, kernel_size)
         self.dimensions = PaddedConv2d(features[-1], self.bboxes_per_cell*2, kernel_size)
         self.objects_class = PaddedConv2d(features[-1], self.bboxes_per_cell*len(self.classes), kernel_size)
 
     def forward(self, X: torch.Tensor):
         """
@@ -123,38 +125,41 @@
                                     weights=weights[presence],
                                     class_weights=class_weights))
         else:
             return absence_loss
 
     def predict(self, images: np.ndarray, detection_treshold: float=0.5,
                 threshold_intersect: Optional[float] = 0.6,
-                downscaling_factors: List[int] = [1]) -> List[dict]:
+                multi_scale: bool = False) -> List[dict]:
         """
         """
-        n = len(images)
+        n, h_image, w_image = images.shape[:3]
         predictions = [{"x": [], "y": [], "w": [], "h": [], "class": [],
                         "bboxe confidence": [], "class confidence": []}
                        for _ in range(n)]
         self.eval()
         X = self._x_to_tensor(images, self.device)
-        for df in downscaling_factors:
+        for i in count():
+            h_down, w_down = tuple(s**i for s in self.downsampling_window)
+            if any(s // (d*g) == 0 for s, d, g in zip((h_image, w_image), (h_down, w_down), self.cells_dimensions)):
+                break
             with torch.no_grad():
-                confidence, position, dimension, object_class = self(F.avg_pool2d(X, kernel_size=(df, df)))
-            h_image, w_image = images.shape[1:3]
+                confidence, position, dimension, object_class = self(F.avg_pool2d(X, kernel_size=(h_down, w_down)))
             h_cell, w_cell = self.cells_dimensions
             N, _, h_grid, w_grid = confidence.shape
             # select most confident bboxe for each cell
             confidence, bboxe_index = confidence.max(dim=1)
             position, dimension, object_class = (
                 torch.gather(tensor, 1, bboxe_index.reshape(N, 1, 1, h_grid, w_grid).expand(-1, -1, tensor.shape[2], -1, -1)).squeeze(1)
                 for tensor in (position, dimension, object_class))
             # converting from grid coordinates to pixel coordinates
-            grid_pos = torch.stack(torch.meshgrid(torch.arange(0, w_image, w_cell, dtype=position.dtype, device=self.device),
-                                torch.arange(0, h_image, h_cell, dtype=position.dtype, device=self.device),
-                                indexing="xy"), dim=0)
+            grid_pos = torch.stack(torch.meshgrid(torch.arange(0, w_image, w_cell*w_down, dtype=position.dtype, device=self.device),
+                                                  torch.arange(0, h_image, h_cell*h_down, dtype=position.dtype, device=self.device),
+                                                  indexing="xy"),
+                                   dim=0)
             cell_dimension = torch.tensor([w_cell, h_cell], dtype=torch.float, device=self.device).reshape(1, 2, 1, 1)
             pixel_position = grid_pos.unsqueeze(0) + position * cell_dimension
             pixel_dimension = dimension * cell_dimension
             # selecting cells with detected objects
             subset = confidence > detection_treshold
             probabilities, classes = torch.softmax(object_class, dim=1).max(dim=1)
             for i, (sub, conf, pos, dim, prob, cls) in enumerate(zip(subset, confidence, pixel_position, pixel_dimension, probabilities, classes)):
@@ -166,14 +171,16 @@
                 predictions[i]["x"].extend(pos[:, 0].cpu().tolist())
                 predictions[i]["y"].extend(pos[:, 1].cpu().tolist())
                 predictions[i]["w"].extend(dim[:, 0].cpu().tolist())
                 predictions[i]["h"].extend(dim[:, 1].cpu().tolist())
                 predictions[i]["class"].extend([self.classes[i] for i in cls.cpu().tolist()])
                 predictions[i]["bboxe confidence"].extend(conf.cpu().tolist())
                 predictions[i]["class confidence"].extend(prob.cpu().tolist())
+            if not multi_scale:
+                break
         # applying non max suppression
         if threshold_intersect is not None:
             predictions = [self._non_max_suppression(bboxes, threshold_intersect) for bboxes in predictions]
         return predictions
 
     @staticmethod
     def _non_max_suppression(bboxes: dict, threshold_intersect: float) -> dict:
@@ -251,41 +258,42 @@
     def device(self) -> torch.device:
         return self.confidence.conv.weight.device
 
     def _x_to_tensor(self, x: np.ndarray,
                      device: Optional[torch.device] = None):
         return images_to_tensor(x, device=device)
 
-    def _y_to_tensor(self, x: np.ndarray, y: Iterable[dict],
+    def _y_to_tensor(self, y: Iterable[dict], image_h: int, image_w: int,
                      device: Optional[torch.device] = None) -> torch.Tensor:
-        grid_h, grid_w = self.cells_dimensions
-        n, h, w = x.shape[:3]
-        h, w = (h//grid_h, w//grid_w)
-        presence = torch.zeros((n, h, w), dtype=torch.bool)
-        positions = torch.zeros((n, 2, h, w), dtype=torch.float)
-        dimensions = torch.zeros((n, 2, h, w), dtype=torch.float)
-        classes = torch.zeros((n, h, w), dtype=torch.long)
+        n = len(y)
+        cell_h, cell_w = self.cells_dimensions
+        grid_h, grid_w = (image_h//cell_h, image_w//cell_w)
+        presence = torch.zeros((n, grid_h, grid_w), dtype=torch.bool)
+        positions = torch.zeros((n, 2, grid_h, grid_w), dtype=torch.float)
+        dimensions = torch.zeros((n, 2, grid_h, grid_w), dtype=torch.float)
+        classes = torch.zeros((n, grid_h, grid_w), dtype=torch.long)
         for n, bboxes in enumerate(y):
             X, Y, W, H = (floats_to_tensor(bboxes[v]) for v in ("x", "y", "w", "h"))
             C = classes_to_tensor(bboxes["class"], self.classes, device=device)
-            i, j = (torch.div(Y, grid_h, rounding_mode="floor").long(), torch.div(X, grid_w, rounding_mode="floor").long())
-            py, px = ((Y % grid_h) / grid_h, (X % grid_w) / grid_w)
+            i, j = (torch.div(Y, cell_h, rounding_mode="floor").long(), torch.div(X, cell_w, rounding_mode="floor").long())
+            py, px = ((Y % cell_h) / cell_h, (X % cell_w) / cell_w)
             presence[n, i, j] = 1
             positions[n, :, i, j] = torch.stack([px, py], dim=0)
-            dimensions[n, :, i, j] = torch.stack([W / grid_w, H / grid_h], dim=0)
+            dimensions[n, :, i, j] = torch.stack([W / cell_w, H / cell_h], dim=0)
             classes[n, i, j] = C
         return presence, positions, dimensions, classes
 
     def data_to_tensor(self, x: np.ndarray, y: List[dict],
                        class_weights: Optional[Sequence[float]] = None,
                        device: Optional[torch.device] = None, **kwargs) -> tuple:
         """
         """
         images = self._x_to_tensor(x, device, **kwargs)
-        presence, positions, dimensions, classes = self._y_to_tensor(x, y, device, **kwargs)
+        h, w = x.shape[1:3]
+        presence, positions, dimensions, classes = self._y_to_tensor(y, h, w, device, **kwargs)
         return images, presence, positions, dimensions, classes
 
     def _tensor_to_y(self, tensor: torch.Tensor) -> List[str]:
         return tensor_to_classes(tensor, self.classes)
 
     def _tensor_to_proba(self, tensor: torch.Tensor) -> pd.DataFrame:
         return tensor_to_probabilities(tensor, self.classes)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_image_segmenter.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_image_segmenter.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,34 +22,34 @@
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
                  upsampling_method: UPSAMPLING_METHOD = "nearest",
                  dropout: Optional[float] = None,
                  entropy_dice_mixture: float = 0.9,
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True):
         """
         Parameters
         ----------
         ...
         """
         super().__init__(classes)
         self.entropy_dice_mixture = entropy_dice_mixture
         scale_factor = tuple(a*b for a, b in zip(stride, pooling_size or (1, 1)))
         self.encoder = ConvolutionalEncoder(in_channels, features, kernel_size,
                                             pooling_size, stride, activation,
                                             n_convs_per_block, normalize,
-                                            residuals, dropout, low_memory)
+                                            residuals, dropout, gradient_checkpointing)
         self.intermediate = ConvBlock(
             features[-1], features[-1], kernel_size, stride, activation,
             normalize, residuals, n_convs_per_block, dropout)
         self.decoder = ConvolutionalDecoder(features[-1], features[::-1], features[::-1],
                                             kernel_size, scale_factor, upsampling_method,
                                             activation, n_convs_per_block, normalize,
-                                            residuals, dropout, low_memory)
+                                            residuals, dropout, gradient_checkpointing)
         self.output = torch.nn.Conv2d(features[0], len(self.classes), (1, 1))
 
     def forward(self, X: torch.Tensor):
         X = X.to(self.device)
         encoded = []
         X = self.encoder(X, encoded)
         X = self.intermediate(X)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_loss_functions.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_loss_functions.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_neural_network.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_neural_network.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import io
 import copy
 import pathlib
 import math
 import torch
-from typing import Union, Sequence, Optional, Callable, Iterable, List
+from typing import Union, Sequence, Optional, Callable, Iterable
 from ._conversions import floats_to_tensor
 from .layers import Dropout
 from pygmalion._model import Model
 from datetime import datetime
 
 
 class NeuralNetwork(torch.nn.Module, Model):
@@ -50,39 +50,38 @@
             if not(overwrite) and file_path.exists():
                 raise FileExistsError(
                     f"The file '{file_path}' already exists, set 'overwrite=True' to overwrite.")
             torch.save(self, file_path)
         else:
             torch.save(self, file_path)
 
-    def fit(self, training_data: Iterable,
-            validation_data: Optional[Iterable] = None,
+    def fit(self, training_data: Union[Iterable, tuple],
+            validation_data: Optional[Union[Iterable, tuple]] = None,
             optimizer: Optional[torch.optim.Optimizer] = None,
             n_steps: int = 1000,
             learning_rate: Union[float, Callable[[int], float]] = 1.0E-3,
-            patience: Optional[int] = None,
+            patience: int = math.inf,
             keep_best: bool = True,
             L1: Optional[float] = None,
             L2: Optional[float] = None,
             gradient_cliping: Optional[float] = None,
             backup_path: Optional[str] = None,
             backup_prefix: str = "model",
             backup_frequency: int = 10000,
             verbose: bool = True):
         """
         Trains a neural network model.
 
         Parameters
         ----------
-        training_data : Iterable of (x, y) or (x, y, weights) data
-            The data used to fit the model on.
-            A tuple of (x, y[, weights]) or a callable that yields them.
-            The type of each element depends on the model kind.
-        validation_data : None or Iterable of (x, y) or (x, y, weights) data
-            The data used to test for early stoping.
+        training_data : tuple or Iterable of tuples
+            The *args passed to the model's loss.
+            If an iterable instead, the number of batches yielded makes the number of gradient accumulation steps.
+        validation_data : None, or same as training data
+            The data used for early stoping.
             Similar to training_data or None
         optimizer : torch.optim.Optimizer or None
             optimizer to use for training
         n_steps : int
             The maximum number of optimization steps
         learning_rate : float or Callable
             The learning rate used to update the parameters,
@@ -105,21 +104,25 @@
         backup_path : str or path like or None
             if provided, path where to backup the model (and optimizer) on disk
         backup_prefix : str
             prefix of the backup filename (the suffix is the current number step)
         backup_frequency : int
             number of steps before each on-disk backup
         verbose : bool
-            If True the loss are displayed at each epoch
+            If True the loss are displayed at each optimization step
         
         Returns
         -------
         tuple :
             (train_losses, val_losses, grad_norms, best_step)
         """
+        if isinstance(training_data, tuple):
+            training_data = [training_data]
+        if isinstance(validation_data, tuple):
+            validation_data = [validation_data]
         if backup_path is not None:
             backup_path = pathlib.Path(backup_path)
             if not backup_path.is_dir():
                 raise NotADirectoryError(f"Backup path is not a valid directory: '{backup_path}'")
         best_step = 0
         best_state = copy.deepcopy(self.state_dict())
         best_metric = None
@@ -182,19 +185,21 @@
                 metric = val_loss if val_loss is not None else train_loss
                 if best_metric is None or metric < best_metric:
                     best_step = step
                     best_metric = metric
                     if keep_best:
                         best_state = copy.deepcopy(self.state_dict())
                 # early stoping
-                if patience is not None and (step - best_step) > patience:
+                if (step - best_step) > patience:
+                    if verbose:
+                        print(f"Early stoping because preformed {patience:,} steps without improvement".replace(",", " "))
                     break
                 # message printing
                 if verbose:
-                    time = datetime.now().strftime("[%Y/%m/%d-%H:%M:%S]")
+                    time = datetime.now().strftime("[%Y-%m-%d %H:%M:%S]")
                     if val_loss is not None:
                         print(f"{time} Step {step}: train loss = {train_loss:.3g}, val loss = {val_loss:.3g}, grad = {grad_norms[-1]:.3e}")
                     else:
                         print(f"{time} Step {step}: train loss = {train_loss:.3g}, grad = {grad_norms[-1]:.3e}")
                 # backup on disk
                 if (backup_path is not None) and (step % backup_frequency == 0) and (step > 0):
                     dec = math.floor(math.log10(n_steps)) + 1
@@ -228,15 +233,15 @@
     def predict(self, *args):
         self.eval()
         x = self._x_to_tensor(*args)
         with torch.no_grad():
             y_pred = self(x)
         return self._tensor_to_y(y_pred)
     
-    def loss(x: torch.Tensor, y: torch.Tensor) -> torch.Tensor:
+    def loss(*args) -> torch.Tensor:
         raise NotImplementedError()
     
     @property
     def dropout(self) -> Optional[float]:
         for m in self.modules():
             if isinstance(m, Dropout):
                 return m.p
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_text_classifier.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_text_segmenter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import torch
 import pandas as pd
-from typing import Union, List, Optional, Literal
-from .layers.transformers import TransformerEncoder, ATTENTION_TYPE
-from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding, Dropout
+from typing import Union, List, Optional, Iterable
+from .layers.transformers import TransformerEncoder, ATTENTION_TYPE, ScaledDotProductAttention
+from .layers.positional_encoding import SinusoidalPositionalEncoding, POSITIONAL_ENCODING_TYPE
+from .layers import Dropout
 from ._conversions import strings_to_tensor, tensor_to_classes, tensor_to_probabilities
 from ._conversions import classes_to_tensor
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy
 from pygmalion.tokenizers._utilities import Tokenizer
 
 
-class TextClassifier(NeuralNetworkClassifier):
+class TextSegmenter(NeuralNetworkClassifier):
 
-    def __init__(self, classes: List[str],
+    def __init__(self, classes: Iterable[str],
                  tokenizer: Tokenizer,
                  n_stages: int, projection_dim: int, n_heads: int,
                  activation: str = "relu",
                  dropout: Union[float, None] = None,
-                 positional_encoding_type: Literal["sinusoidal", "learned", None] = "sinusoidal",
                  mask_padding: bool = True,
-                 attention_type: ATTENTION_TYPE = "scaled dot product",
-                 RPE_radius: Optional[int] = None,
-                 sequence_length: Optional[int] = None,
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True,
+                 positional_encoding_type: Optional[POSITIONAL_ENCODING_TYPE] = SinusoidalPositionalEncoding,
+                 positional_encoding_kwargs: dict={},
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
+                 attention_kwargs: dict = {}):
         """
         Parameters
         ----------
         classes : list of str
             the class names
         tokenizer : Tokenizer
             tokenizer of the input sentences
@@ -36,102 +37,96 @@
             dimension of a single attention head
         n_heads : int
             number of heads for the multi-head attention mechanism
         activation : str
             activation function
         dropout : float or None
             dropout probability if any
-        positional_encoding_type : str or None
-            type of absolute positional encoding
         mask_padding : bool
             If True, PAD tokens are masked in attention
-        attention_type : ATTENTION_TYPE
-            type of attention for multi head attention
-        RPE_radius : int or None
-            radius of the relative positional encoding, or None if not used
-        sequence_length : int or None
-            Fixed size of the input sequence after padding.
-            Usefull if 'mask_padding' is False,
-            or if 'positional_encoding_type' is not None.
-        low_memory : bool
+        gradient_checkpointing : bool
             If True, uses gradient checkpointing to reduce memory usage during
             training at the expense of computation time.
+        positional_encoding_type : POSITIONAL_ENCODING_TYPE or None
+            type of absolute positional encoding
+        positional_encoding_kwargs : dict
+            additional kwargs passed to positional_encoding_type initializer
+        attention_type : ATTENTION_TYPE
+            type of attention for multi head attention
+        attention_kwargs : dict
+            additional kwargs passed to attention_type initializer
         """
         super().__init__(classes)
         self.mask_padding = mask_padding
-        self.sequence_length = sequence_length
         embedding_dim = projection_dim*n_heads
         self.tokenizer = tokenizer
-        self.embedding = torch.nn.Embedding(self.tokenizer.n_tokens,
-                                                  embedding_dim)
+        self.embedding = torch.nn.Embedding(self.tokenizer.n_tokens, embedding_dim)
         self.dropout_input = Dropout(dropout)
-        if positional_encoding_type == "sinusoidal":
-            self.positional_encoding = SinusoidalPositionalEncoding()
-        elif positional_encoding_type == "learned":
-            assert sequence_length is not None
-            self.positional_encoding = LearnedPositionalEncoding(sequence_length, embedding_dim)
-        elif positional_encoding_type is None:
+        if positional_encoding_type is None:
             self.positional_encoding = None
         else:
-            raise ValueError(f"Unexpected positional encoding type '{positional_encoding_type}'")
+            self.positional_encoding = positional_encoding_type(embedding_dim, **positional_encoding_kwargs)
         self.transformer_encoder = TransformerEncoder(n_stages, projection_dim, n_heads,
                                                       dropout=dropout, activation=activation,
-                                                      RPE_radius=RPE_radius, attention_type=attention_type,
-                                                      low_memory=low_memory)
+                                                      attention_type=attention_type,
+                                                      gradient_checkpointing=gradient_checkpointing,
+                                                      **attention_kwargs)
         self.head = torch.nn.Linear(embedding_dim, len(self.classes))
 
-    def forward(self, X: torch.Tensor):
+    def forward(self, X: torch.Tensor, padding_mask: Optional[torch.Tensor]):
         """
         performs the encoding part of the network
 
         Parameters
         ----------
         X : torch.Tensor
             tensor of longs of shape (N, L) with:
             * N : number of sentences
             * L : words per sentence
+        padding_mask : torch.Tensor or None
+            tensor of booleans of shape (N, L)
 
         Returns
         -------
         torch.Tensor :
-            tensor of floats of shape (N, C) with C the number of classes
+            tensor of floats of shape (N, L, C) with C the number of classes
         """
         X = X.to(self.device)
         padding_mask = (X == self.tokenizer.PAD) if self.mask_padding else None
         N, L = X.shape
         X = self.embedding(X)
         if self.positional_encoding is not None:
             X = self.positional_encoding(X)
         X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
         X = self.transformer_encoder(X, padding_mask)
-        return self.head(X.mean(dim=1))
+        return self.head(X)
 
     def loss(self, x, y_target, weights=None, class_weights=None):
         """
         Parameters
         ----------
         x : torch.Tensor
             tensor of long of shape (N, L)
         y_target : torch.Tensor
-            tensor of long of shape (N,)
+            tensor of long of shape (N, L)
         """
         x, y_target = x.to(self.device), y_target.to(self.device)
         y_pred = self(x)
         return cross_entropy(y_pred, y_target, weights, class_weights)
 
     @property
     def device(self) -> torch.device:
         return self.head.weight.device
 
     def _x_to_tensor(self, x: List[str],
                      device: Optional[torch.device] = None,
                      max_input_sequence_length: Optional[int] = None,
                      raise_on_longer_sequences: bool = False):
         return strings_to_tensor(x, self.tokenizer, device,
-                                 max_sequence_length=self.sequence_length or max_input_sequence_length,
+                                 max_sequence_length=self.input_sequence_length or max_input_sequence_length,
                                  raise_on_longer_sequences=raise_on_longer_sequences,
                                  add_start_end_tokens=False)
 
     def _y_to_tensor(self, y: List[str],
                      device: Optional[torch.device] = None) -> torch.Tensor:
         return classes_to_tensor(y, self.classes, device=device)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_text_segmenter.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_text_classifier.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 import torch
 import pandas as pd
-from typing import Union, List, Optional, Literal, Iterable
-from .layers.transformers import TransformerEncoder, ATTENTION_TYPE
-from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding, Dropout
+from typing import Union, List, Optional
+from .layers.transformers import TransformerEncoder, ATTENTION_TYPE, ScaledDotProductAttention
+from .layers.positional_encoding import SinusoidalPositionalEncoding, POSITIONAL_ENCODING_TYPE
+from .layers import Dropout
 from ._conversions import strings_to_tensor, tensor_to_classes, tensor_to_probabilities
 from ._conversions import classes_to_tensor
 from ._neural_network import NeuralNetworkClassifier
 from ._loss_functions import cross_entropy
 from pygmalion.tokenizers._utilities import Tokenizer
 
 
-class TextSegmenter(NeuralNetworkClassifier):
+class TextClassifier(NeuralNetworkClassifier):
 
-    def __init__(self, tokenizer: Tokenizer,
-                 classes: Iterable[str],
+    def __init__(self, classes: List[str],
+                 tokenizer: Tokenizer,
                  n_stages: int, projection_dim: int, n_heads: int,
                  activation: str = "relu",
                  dropout: Union[float, None] = None,
-                 positional_encoding_type: Literal["sinusoidal", "learned", None] = "sinusoidal",
                  mask_padding: bool = True,
-                 attention_type: ATTENTION_TYPE = "scaled dot product",
-                 RPE_radius: Optional[int] = None,
-                 sequence_length: Optional[int] = None,
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True,
+                 positional_encoding_type: Optional[POSITIONAL_ENCODING_TYPE] = SinusoidalPositionalEncoding,
+                 positional_encoding_kwargs: dict={},
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
+                 attention_kwargs: dict = {}):
         """
         Parameters
         ----------
         classes : list of str
             the class names
         tokenizer : Tokenizer
             tokenizer of the input sentences
@@ -36,104 +37,95 @@
             dimension of a single attention head
         n_heads : int
             number of heads for the multi-head attention mechanism
         activation : str
             activation function
         dropout : float or None
             dropout probability if any
-        positional_encoding_type : str or None
-            type of absolute positional encoding
         mask_padding : bool
             If True, PAD tokens are masked in attention
-        attention_type : ATTENTION_TYPE
-            type of attention for multi head attention
-        RPE_radius : int or None
-            radius of the relative positional encoding, or None if not used
-        sequence_length : int or None
-            Fixed size of the input sequence after padding.
-            Usefull if 'mask_padding' is False,
-            or if 'positional_encoding_type' is not None.
-        low_memory : bool
+        gradient_checkpointing : bool
             If True, uses gradient checkpointing to reduce memory usage during
             training at the expense of computation time.
+        positional_encoding_type : POSITIONAL_ENCODING_TYPE or None
+            type of absolute positional encoding
+        positional_encoding_kwargs : dict
+            additional kwargs passed to positional_encoding_type initializer
+        attention_type : ATTENTION_TYPE
+            type of attention for multi head attention
+        attention_kwargs : dict
+            additional kwargs passed to attention_type initializer
         """
         super().__init__(classes)
         self.mask_padding = mask_padding
-        self.sequence_length = sequence_length
         embedding_dim = projection_dim*n_heads
         self.tokenizer = tokenizer
         self.embedding = torch.nn.Embedding(self.tokenizer.n_tokens,
                                                   embedding_dim)
         self.dropout_input = Dropout(dropout)
-        if positional_encoding_type == "sinusoidal":
-            self.positional_encoding = SinusoidalPositionalEncoding()
-        elif positional_encoding_type == "learned":
-            assert sequence_length is not None
-            self.positional_encoding = LearnedPositionalEncoding(sequence_length, embedding_dim)
-        elif positional_encoding_type is None:
+        if positional_encoding_type is None:
             self.positional_encoding = None
         else:
-            raise ValueError(f"Unexpected positional encoding type '{positional_encoding_type}'")
+            self.positional_encoding = positional_encoding_type(embedding_dim, **positional_encoding_kwargs)
         self.transformer_encoder = TransformerEncoder(n_stages, projection_dim, n_heads,
                                                       dropout=dropout, activation=activation,
-                                                      RPE_radius=RPE_radius, attention_type=attention_type,
-                                                      low_memory=low_memory)
+                                                      attention_type=attention_type,
+                                                      gradient_checkpointing=gradient_checkpointing,
+                                                      **attention_kwargs)
         self.head = torch.nn.Linear(embedding_dim, len(self.classes))
 
-    def forward(self, X: torch.Tensor, padding_mask: Optional[torch.Tensor]):
+    def forward(self, X: torch.Tensor):
         """
         performs the encoding part of the network
 
         Parameters
         ----------
         X : torch.Tensor
             tensor of longs of shape (N, L) with:
             * N : number of sentences
             * L : words per sentence
-        padding_mask : torch.Tensor or None
-            tensor of booleans of shape (N, L)
 
         Returns
         -------
         torch.Tensor :
-            tensor of floats of shape (N, L, C) with C the number of classes
+            tensor of floats of shape (N, C) with C the number of classes
         """
         X = X.to(self.device)
         padding_mask = (X == self.tokenizer.PAD) if self.mask_padding else None
         N, L = X.shape
         X = self.embedding(X)
         if self.positional_encoding is not None:
             X = self.positional_encoding(X)
         X = self.dropout_input(X.reshape(N*L, -1)).reshape(N, L, -1)
         X = self.transformer_encoder(X, padding_mask)
-        return self.head(X)
+        return self.head(X.mean(dim=1))
 
     def loss(self, x, y_target, weights=None, class_weights=None):
         """
         Parameters
         ----------
         x : torch.Tensor
             tensor of long of shape (N, L)
         y_target : torch.Tensor
-            tensor of long of shape (N, L)
+            tensor of long of shape (N,)
         """
         x, y_target = x.to(self.device), y_target.to(self.device)
         y_pred = self(x)
         return cross_entropy(y_pred, y_target, weights, class_weights)
 
     @property
     def device(self) -> torch.device:
         return self.head.weight.device
 
     def _x_to_tensor(self, x: List[str],
                      device: Optional[torch.device] = None,
                      max_input_sequence_length: Optional[int] = None,
                      raise_on_longer_sequences: bool = False):
         return strings_to_tensor(x, self.tokenizer, device,
-                                 max_sequence_length=self.input_sequence_length or max_input_sequence_length,
+                                 max_sequence_length=max_input_sequence_length,
                                  raise_on_longer_sequences=raise_on_longer_sequences,
                                  add_start_end_tokens=False)
 
     def _y_to_tensor(self, y: List[str],
                      device: Optional[torch.device] = None) -> torch.Tensor:
         return classes_to_tensor(y, self.classes, device=device)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/_text_translator.py` & `pygmalion-0.1.6/pygmalion/neural_networks/_text_translator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import torch
 import numpy as np
-from typing import Union, List, Sequence, Optional, Literal
+from typing import Union, List, Sequence, Optional
 from itertools import count
 from warnings import warn
-from .layers.transformers import TransformerEncoder, TransformerDecoder, ATTENTION_TYPE
-from .layers import LearnedPositionalEncoding, SinusoidalPositionalEncoding, Dropout
+from .layers.transformers import TransformerEncoder, TransformerDecoder, ATTENTION_TYPE, ScaledDotProductAttention
+from .layers.positional_encoding import SinusoidalPositionalEncoding, POSITIONAL_ENCODING_TYPE
+from .layers import Dropout
 from ._conversions import strings_to_tensor, tensor_to_strings
 from ._conversions import floats_to_tensor
 from ._neural_network import NeuralNetwork
 from ._loss_functions import cross_entropy
-from pygmalion.tokenizers._utilities import Tokenizer, SpecialToken
+from pygmalion.tokenizers._utilities import Tokenizer
 
 
 class TextTranslator(NeuralNetwork):
 
-    def __init__(self, tokenizer_input: Tokenizer,
-                 tokenizer_output: Tokenizer,
+    def __init__(self, tokenizer_input: Tokenizer, tokenizer_output: Tokenizer,
                  n_stages: int, projection_dim: int, n_heads: int,
                  activation: str = "relu",
                  dropout: Union[float, None] = None,
-                 positional_encoding_type: Literal["sinusoidal", "learned", None] = "sinusoidal",
                  mask_padding: bool = True,
-                 attention_type: ATTENTION_TYPE = "scaled dot product",
-                 RPE_radius: Optional[int] = None,
-                 input_sequence_length: Optional[int] = None,
-                 output_sequence_length: Optional[int] = None,
-                 low_memory: bool = True,
-                 label_smoothing: float = 0.):
+                 gradient_checkpointing: bool = True,
+                 label_smoothing: float = 0.,
+                 positional_encoding_type: Optional[POSITIONAL_ENCODING_TYPE] = SinusoidalPositionalEncoding,
+                 input_positional_encoding_kwargs: dict={},
+                 output_positional_encoding_kwargs: dict={},
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
+                 attention_kwargs: dict = {}):
         """
         Parameters
         ----------
         
         tokenizer_input : Tokenizer
             tokenizer of the input sentences
         tokenizer_output : Tokenizer
@@ -41,68 +41,60 @@
             dimension of a single attention head
         n_heads : int
             number of heads for the multi-head attention mechanism
         activation : str
             activation function
         dropout : float or None
             dropout probability if any
-        positional_encoding_type : str or None
-            type of absolute positional encoding
         mask_padding : bool
             If True, PAD tokens are masked in attention
-        attention_type : ATTENTION_TYPE
-            type of attention for multi head attention
-        RPE_radius : int or None
-            radius of the relative positional encoding, or None if not used
-        input_sequence_length : int or None
-            Fixed size of the input sequence after padding.
-            Usefull if 'mask_padding' is False,
-            or if 'positional_encoding_type' is not None.
-        output_sequence_length : int or None
-            Same as input_sequence_length but for output sequences.
-        low_memory : bool
+        gradient_checkpointing : bool
             If True, uses gradient checkpointing to reduce memory usage during
             training at the expense of computation time.
         label_smoothing : float
             label smoothing level used in cross entropy loss
+        positional_encoding_type : POSITIONAL_ENCODING_TYPE or None
+            type of absolute positional encoding
+        input_positional_encoding_kwargs : dict
+            additional kwargs passed to positional_encoding_type initializer
+        output_positional_encoding_kwargs : dict
+            additional kwargs passed to positional_encoding_type initializer
+        attention_type : ATTENTION_TYPE
+            type of attention for multi head attention
+        attention_kwargs : dict
+            additional kwargs passed to attention_type initializer
         """
         super().__init__()
         self.mask_padding = mask_padding
-        self.input_sequence_length = input_sequence_length
-        self.output_sequence_length = output_sequence_length
         self.label_smoothing = label_smoothing
         embedding_dim = projection_dim*n_heads
         self.tokenizer_input = tokenizer_input
         self.tokenizer_output = tokenizer_output
         self.embedding_input = torch.nn.Embedding(self.tokenizer_input.n_tokens,
                                                   embedding_dim)
         self.embedding_output = torch.nn.Embedding(self.tokenizer_output.n_tokens,
                                                 embedding_dim)
         self.dropout_input = Dropout(dropout)
         self.dropout_output = Dropout(dropout)
-        if positional_encoding_type == "sinusoidal":
-            self.positional_encoding_input = SinusoidalPositionalEncoding()
-            self.positional_encoding_output = SinusoidalPositionalEncoding()
-        elif positional_encoding_type == "learned":
-            assert input_sequence_length is not None and output_sequence_length is not None
-            self.positional_encoding_input = LearnedPositionalEncoding(input_sequence_length, embedding_dim)
-            self.positional_encoding_output = LearnedPositionalEncoding(output_sequence_length, embedding_dim)
-        elif positional_encoding_type is None:
+        if positional_encoding_type is None:
             self.positional_encoding_input = None
             self.positional_encoding_output = None
         else:
-            raise ValueError(f"Unexpected positional encoding type '{positional_encoding_type}'")
+            self.positional_encoding_input = positional_encoding_type(embedding_dim, **input_positional_encoding_kwargs)
+            self.positional_encoding_output = positional_encoding_type(embedding_dim, **output_positional_encoding_kwargs)
         self.transformer_encoder = TransformerEncoder(n_stages, projection_dim, n_heads,
                                                       dropout=dropout, activation=activation,
-                                                      RPE_radius=RPE_radius, attention_type=attention_type,
-                                                      low_memory=low_memory)
+                                                      attention_type=attention_type,
+                                                      gradient_checkpointing=gradient_checkpointing,
+                                                      **attention_kwargs)
         self.transformer_decoder = TransformerDecoder(n_stages, projection_dim, n_heads,
                                                       dropout=dropout, activation=activation,
-                                                      RPE_radius=RPE_radius, attention_type=attention_type,
-                                                      low_memory=low_memory)
+                                                      attention_type=attention_type,
+                                                      gradient_checkpointing=gradient_checkpointing,
+                                                      **attention_kwargs)
         self.head = torch.nn.Linear(embedding_dim, self.tokenizer_output.n_tokens)
 
     def forward(self, X: torch.Tensor, padding_mask: Optional[torch.Tensor]):
         return self.encode(X, padding_mask)
 
     def encode(self, X: torch.Tensor, padding_mask: Optional[torch.Tensor]) -> torch.Tensor:
         """
@@ -188,19 +180,14 @@
         Predict a translation for the given sequences using beam search,
         outputing at most 'max_tokens' tokens.
         If 'n_beams' is 1, this is equivalent to predicting the single token
         with the highest likelyhood at each step.
         """
         if isinstance(sequences, str):
             sequences = [sequences]
-        if max_tokens is not None and self.output_sequence_length is not None:
-            if max_tokens > self.output_sequence_length:
-                warn(f"Tried predicting up to {max_tokens} tokens but 'output_sequence_length' is {self.output_sequence_length}")
-                max_tokens = self.output_sequence_length
-        max_tokens = max_tokens or self.output_sequence_length
         self.eval()
         with torch.no_grad():
             X = self._x_to_tensor(sequences, self.device, raise_on_longer_sequences=True)
             START = self.tokenizer_output.START
             END = self.tokenizer_output.END
             PAD = self.tokenizer_input.PAD
             n_classes = self.tokenizer_output.n_tokens
@@ -257,19 +244,14 @@
     
     def _predict_naive(self, sequences: List[str], max_tokens: Optional[int] = None) -> List[str]:
         """
         For comparison sake, this should output the same result as predict with n_beams=1
         """
         if isinstance(sequences, str):
             sequences = [sequences]
-        if max_tokens is not None and self.output_sequence_length is not None:
-            if max_tokens > self.output_sequence_length:
-                warn(f"Tried predicting up to {max_tokens} tokens but 'output_sequence_length' is {self.output_sequence_length}")
-                max_tokens = self.output_sequence_length
-        max_tokens = max_tokens or self.output_sequence_length
         self.eval()
         with torch.no_grad():
             X = self._x_to_tensor(sequences, self.device, raise_on_longer_sequences=True)
             START = self.tokenizer_output.START
             END = self.tokenizer_output.END
             PAD = self.tokenizer_input.PAD
             encoded_padding_mask = (X == PAD) if self.mask_padding else None
@@ -318,25 +300,25 @@
 
     def _x_to_tensor(self, x: List[str],
                      device: Optional[torch.device] = None,
                      max_input_sequence_length: Optional[int] = None,
                      raise_on_longer_sequences: bool = False,
                      progress_bar: bool = False):
         return strings_to_tensor(x, self.tokenizer_input, device,
-                                 max_sequence_length=self.input_sequence_length or max_input_sequence_length,
+                                 max_sequence_length=max_input_sequence_length,
                                  raise_on_longer_sequences=raise_on_longer_sequences,
                                  add_start_end_tokens=False,
                                  progress_bar=progress_bar)
 
     def _y_to_tensor(self, y: List[str],
                      device: Optional[torch.device] = None,
                      max_output_sequence_length: Optional[int] = None,
                      raise_on_longer_sequences: bool = False,
                      progress_bar: bool = False) -> torch.Tensor:
         return strings_to_tensor(y, self.tokenizer_output, device,
-                                 max_sequence_length=self.output_sequence_length or max_output_sequence_length,
+                                 max_sequence_length=max_output_sequence_length,
                                  raise_on_longer_sequences=raise_on_longer_sequences,
                                  add_start_end_tokens=True,
                                  progress_bar=progress_bar)
 
     def _tensor_to_y(self, tensor: torch.Tensor) -> np.ndarray:
         return tensor_to_strings(tensor, self.tokenizer_output)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/_activation.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/_activation.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/_dropout.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/_dropout.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/_normalization.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/_normalization.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,76 +6,63 @@
     """
     Normalize a tensor along the given dimension based on a running average
     of all training observations. Suitable only to normalize input or target data,
     as normalization parameters will change less and less as more batches are seen.
     """
 
     def __init__(self, dim: int, num_features: int, eps: float=1e-05,
-                 affine: bool=True, device: Optional[torch.device]=None,
+                 device: Optional[torch.device]=None,
                  dtype: Optional[torch.dtype]=None):
         """
         Parameters
         ----------
         dim : int
             dimension along which data are normalised
         num_features : int
             size of the given dimension along which data are normalized
         eps : float
             epsilon factor to avoid division by zero
-        momentum : float
-            update factor used for the running stats
-        affine: bool
-            if True, apply a linear transformation with bias after normalization
         device : torch.device or None
             device to store the parameters and tensors on
         dtype : torch.dtype
             dtype of the tensors and parameters
         """
         super().__init__()
         self.dim = dim
         self.num_features = num_features
         self.eps = eps
         self.n_observations = 0
         self.running_mean = torch.zeros(num_features, device=device, dtype=dtype)
         self.running_var = torch.ones(num_features, device=device, dtype=dtype)
-        if affine:
-            self.weight = torch.nn.parameter.Parameter(torch.ones(num_features, device=device, dtype=dtype))
-            self.bias = torch.nn.parameter.Parameter(torch.zeros(num_features, device=device, dtype=dtype))
-        else:
-            self.weight, self.bias = (None, None)
-    
-    def forward(self, X: torch.Tensor) -> torch.Tensor:
+
+    def forward(self, X: torch.Tensor, track_running_stats: bool=True) -> torch.Tensor:
         """
         Parameters
         ----------
         X : torch.Tensor
             tensor of floats of shape (N, ..., num_features, ...)
         
         Returns
         -------
         torch.Tensor :
             tensor of floats of shape (N, ..., num_features, ...) normalized along the given dimension
         """
         if X.shape[self.dim] != self.num_features:
             raise ValueError(f"Expected tensor of shape (N, *, {self.num_features}, *) but got {tuple(X.shape)}")
-        if self.training:
+        if self.training and track_running_stats:
             with torch.no_grad():
                 self.running_mean, self.running_var = self.running_mean.to(X.device), self.running_var.to(X.device)
                 n = X.numel() // self.num_features
                 var = X.moveaxis(self.dim, 0).reshape(self.num_features, -1).var(dim=-1, unbiased=False)
                 mean = X.moveaxis(self.dim, 0).reshape(self.num_features, -1).mean(dim=self.dim)
                 self.running_var = (self.n_observations/(self.n_observations+n)) * self.running_var + (n/(self.n_observations+n)) * var + self.n_observations*n/(self.n_observations+n)**2 * (mean - self.running_mean)**2
                 self.running_mean = mean * (self.n_observations / (self.n_observations + n)) + self.running_mean * (n / (self.n_observations + n))
                 self.n_observations += n
-        shape = [self.num_features if i == self.dim else 1 for i, _ in enumerate(X.shape)]
+        shape = [self.num_features if i == self.dim % len(X.shape) else 1 for i, _ in enumerate(X.shape)]
         X = (X - self.running_mean.reshape(shape)) / (self.running_var.reshape(shape) + self.eps)**0.5
-        if self.weight is not None:
-            X = X * self.weight.reshape(shape)
-        if self.bias is not None:
-            X = X + self.bias.reshape(shape)
         return X
 
     def unscale(self, Y: torch.Tensor) -> torch.Tensor:
         """
         Unapply normalization
         """
         shape = [self.num_features if i == self.dim else 1 for i, _ in enumerate(Y.shape)]
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/_positional_encoding.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/positional_encoding/_learned_positional_encoding.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,26 +2,26 @@
 
 
 class LearnedPositionalEncoding(torch.nn.Module):
     """
     Learned positional encoding for sequences
     """
 
-    def __init__(self, n_positions: int, embedding_dimension: int):
+    def __init__(self, embedding_dimension: int, sequence_length: int):
         """
         Parameters
         ----------
-        n_positions : int
-            maximum length of the sequence to encode position in
-            There won't be a learned embedding vector for tokens beyond 'n_positions'
         embedding_dimension : int
             Embedding vector dimension
+        sequence_length : int
+            Maximum length of the sequence to encode position in.
+            There won't be a learned embedding vector for tokens beyond 'sequence_length'.
         """
         super().__init__()
-        self.embedding = torch.nn.Embedding(n_positions, embedding_dimension)
+        self.embedding = torch.nn.Embedding(sequence_length, embedding_dimension)
 
     def forward(self, X: torch.Tensor, offset: int=0) -> torch.Tensor:
         """
         Parameters
         ----------
         X : torch.Tensor
             tensor of floats of shape (..., L, D)
@@ -30,46 +30,13 @@
         
         Returns
         -------
         torch.Tensor :
             tensor of floats of shape (..., L, D)
         """
         L, D = X.shape[-2:]
+        sequence_length = self.embedding.weight.shape[0]
+        if (L+offset >= sequence_length):
+            raise ValueError(f"Tried applying {type(self).__name__} with {sequence_length} learned positions to longer sequence of length {L}. (Tensor of shape {tuple(X.shape)})")
         P = torch.arange(L, device=X.device)
         shape = tuple(1 for _ in range(len(X.shape) - 2)) + (L, D)
-        return X + self.embedding(P+offset).reshape(shape)
-
-
-class SinusoidalPositionalEncoding(torch.nn.Module):
-    """
-    Parameterless positional encoding for sequences
-    Performs positional encoding on the input, in the
-    "Attention is all you need" paper fashion.
-    """
-
-    def __init__(self):
-        super().__init__()
-    
-    def forward(self, X: torch.Tensor, offset: int=0) -> torch.Tensor:
-        """
-        Parameters
-        ----------
-        X : torch.Tensor
-            tensor of shape (..., D), with D the embedding dimension
-        offset : int
-            a position offset
-
-        Returns
-        -------
-        torch.Tensor:
-            tensor of shape (..., D)
-        """
-        shape = X.shape
-        X = X.reshape(-1, shape[-1])
-        N, D = X.shape
-        pe = torch.zeros(N, D, dtype=torch.float, device=X.device)
-        position = torch.arange(0, D, dtype=torch.float).unsqueeze(0) + offset
-        angle = position / 10000**(2*torch.div(position, 2, rounding_mode='floor')/D)
-        pe[:, 0::2] = torch.cos(angle[:, 0::2])
-        pe[:, 1::2] = torch.sin(angle[:, 1::2])
-        X = (X + pe).reshape(shape)
-        return X
+        return X + self.embedding(P+offset).reshape(shape)
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_conv_block.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_conv_block.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_padded_conv.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_padded_conv.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_stack.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_stack.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,17 +14,17 @@
                  pooling_size: Tuple[int, int] = (2, 2),
                  stride: Tuple[int, int] = (1, 1),
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
                  dropout: Optional[float] = None,
-                 low_memory: bool = False):
+                 gradient_checkpointing: bool = False):
         super().__init__()
-        self.low_memory = low_memory
+        self.gradient_checkpointing = gradient_checkpointing
         self.stages = torch.nn.ModuleList()
         for out_features in features:
             self.stages.append(ConvolutionalEncoderStage(
                 in_features, out_features, kernel_size, pooling_size, stride,
                 activation, n_convs_per_block, normalize, residuals, dropout))
             in_features = out_features
 
@@ -40,15 +40,15 @@
         
         Returns
         -------
         torch.Tensor :
             tensor of shape (N, Cout, Hout, Wout)
         """
         for stage in self.stages:
-            if self.low_memory and self.training:
+            if self.gradient_checkpointing and self.training:
                 X.requires_grad_(True)  # To ensure that the gradient is backpropagated in the convolution parameters
                 X, map = checkpoint(stage, X)
             else:
                 X, map = stage(X)
             if maps is not None:
                 maps.append(map)
         return X
@@ -63,17 +63,17 @@
                  upsampling_factor: Tuple[int, int] = (2, 2),
                  upsampling_method : UPSAMPLING_METHOD = "nearest",
                  activation: str = "relu",
                  n_convs_per_block: int = 1,
                  normalize: bool = True,
                  residuals: bool = True,
                  dropout: Optional[float] = None,
-                 low_memory: bool = False):
+                 gradient_checkpointing: bool = False):
         super().__init__()
-        self.low_memory = low_memory
+        self.gradient_checkpointing = gradient_checkpointing
         self.stages = torch.nn.ModuleList()
         for out_features, add in zip(features, add_features or repeat(None)):
             self.stages.append(ConvolutionalDecoderStage(
                 in_features, out_features, add, kernel_size, upsampling_factor, upsampling_method,
                 activation, n_convs_per_block, normalize, residuals, dropout))
             in_features = out_features
 
@@ -90,13 +90,13 @@
         
         Returns
         -------
         torch.Tensor :
             tensor of shape (N, Cout, Hout, Wout)
         """
         for stage, add in zip(self.stages, add_maps or repeat(None)):
-            if self.low_memory and self.training:
+            if self.gradient_checkpointing and self.training:
                 X.requires_grad_(True)  # To ensure that the gradient is backpropagated in the convolution parameters
                 X = checkpoint(stage, X, add)
             else:
                 X = stage(X, add)
         return X
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_stages.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_stages.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/convolutions/_upsampling.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/convolutions/_upsampling.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_attention.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/multihead_attention/_kernelized_attention.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,238 +1,238 @@
 import torch
 from typing import Optional, Callable
 from ._utilities import _align, _mask_chronological, _log_exp_kernel
 
-
-class ScaledDotProductAttention(torch.nn.Module):
-
-    def __init__(self):
-        super().__init__()
-    
-    def forward(self, q: torch.Tensor, k: torch.Tensor, v: torch.Tensor, mask_future: bool,
-                padding_mask: Optional[torch.Tensor], RPE: Optional[torch.nn.Embedding],
-                mask_index_offset: int = 0):
-        return self._scaled_dot_product_attention(q, k, v, mask_future, padding_mask, RPE, mask_index_offset)
-
-    @staticmethod
-    def _scaled_dot_product_attention(q: torch.Tensor, k: torch.Tensor,
-                                      v: torch.Tensor, mask_future: bool,
-                                      padding_mask: Optional[torch.Tensor],
-                                      RPE: Optional[torch.nn.Embedding],
-                                      mask_index_offset: int = 0
-                                      ) -> torch.Tensor:
-        """
-        Apply scaled dot product attention to a batch of 'N' sentences pairs,
-        with 'H' the number of heads, and 'D' the projection dimension.
-        The query is a sequence of length 'Lq', and the key is
-        a sequence of length 'Lk'.
-        This is the original attention mechanism described in the 2017 paper:
-            'Attention is all you need'
-            https://arxiv.org/pdf/1706.03762.pdf
-
-        Parameters
-        ----------
-        q : torch.Tensor
-            query tensor of shape (N, H, Lq, D)
-        k : torch.Tensor
-            key tensor of shape (N, H, Lk, D)
-        v : torch.Tensor
-            value tensor of shape (N, H, Lk, D)
-        mask_future : bool
-            whether or not a query at index i can't attend to keys at index j > i
-            in the sequence 
-        padding_mask : torch.Tensor or None
-            tensor of booleans of shape (N, Lk)
-        RPE : torch.nn.Embedding or None
-            if provided, the the relative positional embedding
-        mask_index_offset : int
-            Add the given offset to the query positions for future masking.
-            This is intended for evaluation mode, where representation of
-            previously generated tokens must not be generated several times.
-
-        Returns
-        -------
-        torch.Tensor:
-            attention, a tensor of shape (N, H, Lq, D)
-        """
-        N, H, Lq, d = q.shape
-        N, H, Lk, d = k.shape
-        scaling = Lk**0.5 if padding_mask is None else (~padding_mask).float().sum(dim=-1).reshape(N, 1, 1, 1)**0.5
-        score = torch.einsum("nhqd, nhkd -> nhqk", q, k) / scaling
-        if RPE is not None:
-            r = RPE.weight.shape[0] // 2
-            P = torch.clip(r + torch.arange(Lk, device=score.device).reshape(1, Lk)
-                           - torch.arange(Lq, device=score.device).reshape(Lq, 1)
-                           - mask_index_offset, 0, 2*r)
-            P = RPE(P).reshape(Lq, Lk, H, d)
-            score = score + torch.einsum("qkhd, nhkd -> nhqk", P, k) / scaling
-        if mask_future:
-            score = score.masked_fill(_mask_chronological(Lq, Lk, score.device, mask_index_offset).reshape(1, 1, Lq, Lk), -float("inf"))
-        if padding_mask is not None:
-            score = score.masked_fill(padding_mask.reshape(N, 1, 1, Lk), -float("inf"))
-        score = torch.softmax(score, dim=-1)
-        attention = torch.matmul(score, v)
-        return attention
-
-
 class KernelizedAttention(torch.nn.Module):
 
-    def __init__(self, kernel_function: Callable = _log_exp_kernel,
-                 linear_compelxity: bool = True,
+    def __init__(self, projection_dim: int, n_heads: int,
+                 mask_future: bool, RPE_radius: Optional[int] = None,
+                 kernel_function: Callable = _log_exp_kernel,
+                 linear_complexity: bool = True,
                  scaled: bool = True):
         """
         Parameters
         ----------
+        projection_dim : int
+            the dimension of the projection space for the feature vectors
+        n_heads : int
+            the number of different projection at each stage of the transformer
+        mask_future: bool
+            whether or not a query at index i can't attend to keys
+            at index j > i in the sequence
+        RPE_radius : int or None
+            The radius of the relative positional encoding
+            or None if no relative positional encoding should be applied
         kernel_function : Callable
             the kernel function applied to query and keys
         linear_complexity : bool
             whether to use linear or quadratic complexity algorithm
-        scaled: bool
-            if True, the scores sum up to 1
+        scaled : bool
+            if True, the attention scores of any query to all keys sums up to 1
         """
         super().__init__()
+        self.n_heads = n_heads
+        self.projection_dim = projection_dim
+        dim = projection_dim * n_heads
+        self.mask_future = mask_future
+        self.relative_positional_encoding = torch.nn.Embedding(2*RPE_radius+1, dim) if RPE_radius else None
+        self.query = torch.nn.Linear(dim, dim, bias=False)
+        self.key = torch.nn.Linear(dim, dim, bias=False)
+        self.value = torch.nn.Linear(dim, dim, bias=False)
         self.kernel_function = kernel_function
-        self.linear_complexity = linear_compelxity
+        self.linear_complexity = linear_complexity
         self.scaled = scaled
-    
-    def forward(self, q: torch.Tensor, k: torch.Tensor,
-                v: torch.Tensor, mask_future: bool,
-                padding_mask: Optional[torch.Tensor],
-                RPE: Optional[torch.nn.Embedding],
-                mask_index_offset: int = 0):
+
+    def forward(self, query: torch.Tensor, key: torch.Tensor,
+                query_mask: Optional[torch.Tensor] = None,
+                key_mask: Optional[torch.Tensor] = None,
+                future_offset: int=0):
         """
+        Apply scaled dot product attention to a batch of 'N' sentences pairs,
+        with 'H' the number of heads, and 'D' the projection dimension.
+        The query is a sequence of length 'Lq', and the key is
+        a sequence of length 'Lk'.
+        This is the original attention mechanism described in the 2017 paper:
+            'Attention is all you need'
+            https://arxiv.org/abs/1706.03762
+        In addition, relative positional encoding is implemented as well:
+            'Self-Attention with Relative Position Representations'
+            https://arxiv.org/abs/1803.02155
+
         Parameters
         ----------
-        q : torch.Tensor
-            query tensor of shape (N, H, Lq, D)
-        k : torch.Tensor
-            key tensor of shape (N, H, Lk, D)
-        v : torch.Tensor
-            value tensor of shape (N, H, Lk, D)
-        mask_future : bool
-            whether or not a query at index i can't attend to keys at index j > i
-            in the sequence 
-        padding_mask : torch.Tensor or None
-            tensor of booleans of shape (N, Lk)
-        RPE : torch.nn.Embedding or None
-            if provided, the relative positional embedding
-        mask_index_offset : int
+        query : torch.Tensor
+            tensor of shape (N, Lq, D)
+        key : torch.Tensor
+            tensor of shape (N, Lk, D)
+        query_mask : torch.Tensor or None
+            Tensor of booleans of shape (N, Lq)
+            or None if padding tokens should not be masked.
+            Masked queries are set to null vector after transformation.
+        key_mask : torch.Tensor or None
+            Tensor of booleans of shape (N, Lk)
+            or None if padding tokens should not be masked.
+            Attention scores to masked keys is set to 0
+        future_offset : int
             Add the given offset to the query positions for future masking.
             This is intended for evaluation mode, where representation of
             previously generated tokens must not be generated several times.
-            If different from 0, the squared complexity algorithm is used
-            (because this is intended for use with a sequence of queries of length 1).
 
         Returns
         -------
-        torch.Tensor:
-            attention, a tensor of shape (N, H, Lq, D)
+        torch.Tensor :
+            tensor of shape (N, Lq, D)
         """
-        if self.linear_complexity and (mask_index_offset == 0):
-            return self._kernelized_attention_linear(
-                self.kernel_function, q, k, v, mask_future, padding_mask, RPE, self.scaled)
+        query, key = query.to(self.device), key.to(self.device)
+        N, Lq, _ = query.shape
+        N, Lk, _ = key.shape
+        # project into 'n_heads' different subspaces
+        q = self.kernel_function(self.query(query).reshape(N, Lq, self.n_heads, self.projection_dim))
+        k = self.kernel_function(self.key(key).reshape(N, Lk, self.n_heads, self.projection_dim))
+        v = self.value(key).reshape(N, Lk, self.n_heads, self.projection_dim)
+        # compute attention
+        q, k, v = q.transpose(1, 2), k.transpose(1, 2), v.transpose(1, 2)
+        if self.linear_complexity:
+            attention = self._attention_linear(
+                self.kernel_function, q, k, v, self.mask_future, key_mask, self.relative_positional_encoding, self.scaled, future_offset)
         else:
-            return self._kernelized_attention_naive(
-                self.kernel_function, q, k, v, mask_future, padding_mask, RPE, self.scaled,
-                mask_index_offset)
+            attention = self._attention_naive(
+                self.kernel_function, q, k, v, self.mask_future, key_mask, self.relative_positional_encoding, self.scaled, future_offset)
+        attention = attention.transpose(2, 1).reshape(N, Lq, -1)
+        # mask queries if needed
+        if query_mask is not None:
+            query_mask = query_mask.to(attention.device).unsqueeze(-1)
+            attention = torch.masked_fill(attention, query_mask, 0.)
+        return attention
+
+    @property
+    def device(self) -> torch.device:
+        return self.query.weight.device
 
     @staticmethod
-    def _kernelized_attention_linear(kernel: Callable, q: torch.Tensor, k: torch.Tensor,
-                                     v: torch.Tensor, mask_future: bool,
-                                     padding_mask: Optional[torch.Tensor],
-                                     RPE: Optional[torch.nn.Embedding],
-                                     scaled: bool) -> torch.Tensor:
-        """
-        see forward doc
-        """
-        pq, pk = kernel(q), kernel(k)
-        N, H, Lq, _ = pq.shape
-        N, H, Lk, _ = pk.shape
+    def _attention_linear(kernel: Callable, q: torch.Tensor, k: torch.Tensor,
+                          v: torch.Tensor, mask_future: bool,
+                          key_mask: Optional[torch.Tensor],
+                          RPE: Optional[torch.nn.Embedding],
+                          scaled: bool, future_offset: int = 0) -> torch.Tensor:
+        """
+        see self._attention_naive doc
+        """
+        if future_offset != 0:
+            raise ValueError("Linear complexity not implemented for 'future_offset' != 0")
+        q, k = kernel(q), kernel(k)
+        N, H, Lq, _ = q.shape
+        N, H, Lk, _ = k.shape
         D = v.shape[-1]
-        if padding_mask is not None:
-            v = torch.masked_fill(v, padding_mask.reshape(N, 1, Lk, 1), 0.)
+        if key_mask is not None:
+            v = torch.masked_fill(v, key_mask.reshape(N, 1, Lk, 1), 0.)
         if mask_future:
-            expanded = torch.einsum("nhkd, nhkD -> nhkdD", pk, v)
+            expanded = torch.einsum("nhkd, nhkD -> nhkdD", k, v)
             summed = _align(torch.cumsum(expanded, dim=2), Lq, 2)
-            attention = torch.einsum("nhqd, nhqdD -> nhqD", pq, summed)
+            attention = torch.einsum("nhqd, nhqdD -> nhqD", q, summed)
         else:
-            right = torch.einsum("nhkd, nhkD -> nhdD", pk, v)
-            attention = torch.einsum("nhqd, nhdD -> nhqD", pq, right)
+            right = torch.einsum("nhkd, nhkD -> nhdD", k, v)
+            attention = torch.einsum("nhqd, nhdD -> nhqD", q, right)
         if RPE is not None:
             rpe = kernel(RPE.weight)
             r = rpe.shape[0] // 2
             if mask_future:
                 rpe = torch.masked_fill(rpe, torch.arange(2*r+1).unsqueeze(-1) > r, 0.)
-            W = torch.einsum("nhqd, Rd -> nhqR", pq, rpe)
+            W = torch.einsum("nhqd, Rd -> nhqR", q, rpe)
             # before horizon
             p_before, n_before = min(r, Lq), min(max(0, Lq-r), Lk)
             W_before = W[..., 0]  # (N, H, Lq)
             padding_before = tuple(p_before if i == 2 else s for i, s in enumerate(v.shape))
             V_before = _align(torch.cat([torch.zeros(padding_before), v[..., :n_before, :].cumsum(dim=2)], dim=2), Lq, 2)
             attention = attention + torch.einsum("nhq, nhqd -> nhqd", W_before, V_before)
             # horizon
             W_horizon = W[..., 1:-1]  # (N, H, Lq, 2r-1)
             V_horizon = torch.cat([torch.zeros((N, H, max(0, r-1), D),
-                                            device=pq.device),
+                                            device=q.device),
                                 v,
                                 torch.zeros((N, H, max(0, Lq-(Lk-r)), D),
-                                            device=pq.device)],
+                                            device=q.device)],
                                 dim=-2)
             L = V_horizon.shape[-2]
             V_horizon = V_horizon.as_strided(size=(N, H, Lq, 2*r-1, D),
                                             stride=(H*L*D, L*D, D, D, 1))
             attention = attention + torch.einsum("nhqr, nhqrd -> nhqd", W_horizon, V_horizon)
             # after horizon
             if not mask_future:
                 n_after = min(Lq+r, Lk)
                 p_after = max(0, Lq-max(0, Lk-r))
                 W_after = W[..., -1]  # (N, H, Lq)
-                padding_after = torch.zeros((N, H, p_after, D), device=pq.device)
+                padding_after = torch.zeros((N, H, p_after, D), device=q.device)
                 Rcum = (v[..., r-1:n_after, :].sum(dim=-2).unsqueeze(-2)
                         - v[..., r-1:n_after-1, :].cumsum(dim=-2))
                 V_after = torch.cat([Rcum, padding_after], dim=-2)
                 attention = attention + torch.einsum("nhq, nhqd -> nhqd", W_after, V_after)
         if scaled:
             v_scaling = torch.ones(N, H, Lk, 1)
-            if padding_mask is not None:
-                v_scaling = torch.masked_fill(v_scaling, padding_mask.reshape(N, 1, Lk, 1), 0.)
+            if key_mask is not None:
+                v_scaling = torch.masked_fill(v_scaling, key_mask.reshape(N, 1, Lk, 1), 0.)
             scale = KernelizedAttention._kernelized_attention_linear(
-                kernel, q, k, v_scaling, mask_future, padding_mask, RPE, scaled=False)
+                kernel, q, k, v_scaling, mask_future, key_mask, RPE, scaled=False)
             attention = attention / scale
         return attention
 
     @staticmethod
-    def _kernelized_attention_naive(kernel: Callable, q: torch.Tensor, k: torch.Tensor,
-                                    v: torch.Tensor, mask_future: bool,
-                                    padding_mask: Optional[torch.Tensor],
-                                    RPE: Optional[torch.nn.Embedding],
-                                    scaled: bool,
-                                    mask_index_offset: int = 0,
-                                    ) -> torch.Tensor:
+    def _attention_naive(kernel: Callable, q: torch.Tensor, k: torch.Tensor,
+                         v: torch.Tensor, mask_future: bool,
+                         key_mask: Optional[torch.Tensor],
+                         RPE: Optional[torch.nn.Embedding],
+                         scaled: bool, future_offset: int = 0) -> torch.Tensor:
         """
-        see forward doc
         Parameters
         ----------
+        kernel : callable
+            kernel function
+        q : torch.Tensor
+            query tensor of shape (N, H, Lq, d)
+        k : torch.Tensor
+            key tensor of shape (N, H, Lk, d)
+        v : torch.Tensor
+            value tensor of shape (N, H, Lk, d)
+        mask_future : bool
+            whether or not a query at index i can't attend to keys at index j > i
+            in the sequence 
+        key_mask : torch.Tensor or None
+            tensor of booleans of shape (N, Lk)
+        RPE : torch.nn.Embedding or None
+            if provided, the relative positional embedding
+            tensor of shape (2*R+1, D) or None
+        scaled : bool
+            if True, the attention scores of any query to all keys sums up to 1
+        future_offset : int
+            Add the given offset to the query positions for future masking.
+            This is intended for evaluation mode, where representation of
+            previously generated tokens must not be generated several times.
+            If different from 0, the squared complexity algorithm is used
+            (because this is intended for use with a sequence of queries of length 1).
 
+        Returns
+        -------
+        torch.Tensor:
+            attention, a tensor of shape (N, H, Lq, D)
         """
-        pq, pk = kernel(q), kernel(k)
-        N, H, Lq, d = pq.shape
-        N, H, Lk, d = pk.shape
-        score = torch.einsum("nhqd, nhkd -> nhqk", pq, pk)
+        q, k = kernel(q), kernel(k)
+        N, H, Lq, d = q.shape
+        N, H, Lk, d = k.shape
+        score = torch.einsum("nhqd, nhkd -> nhqk", q, k)
         if RPE is not None:
             r = RPE.weight.shape[0] // 2
             P = torch.clip(r + torch.arange(Lk, device=score.device).reshape(1, Lk)
                            - torch.arange(Lq, device=score.device).reshape(Lq, 1)
-                           - mask_index_offset,
+                           - future_offset,
                            0, 2*r)
-            score = score + torch.einsum("qkd, nhqd -> nhqk", kernel(RPE(P)), pq)
+            score = score + torch.einsum("qkd, nhqd -> nhqk", kernel(RPE(P)), q)
         if mask_future:
-            mask = _mask_chronological(Lq, Lk, score.device, mask_index_offset).reshape(1, 1, Lq, Lk)
+            mask = _mask_chronological(Lq, Lk, score.device, future_offset).reshape(1, 1, Lq, Lk)
             score = torch.masked_fill(score, mask, 0)
-        if padding_mask is not None:
-            score = torch.masked_fill(score, padding_mask.reshape(N, 1, 1, Lk), 0)
+        if key_mask is not None:
+            score = torch.masked_fill(score, key_mask.reshape(N, 1, 1, Lk), 0)
         if scaled:
             score = score / score.sum(dim=-1).unsqueeze(-1)
-        if padding_mask is not None:
-            score = torch.masked_fill(score, padding_mask.reshape(N, 1, 1, Lk), 0.)
+        if key_mask is not None:
+            score = torch.masked_fill(score, key_mask.reshape(N, 1, 1, Lk), 0.)
         attention = torch.matmul(score, v)
-        return attention
+        return attention
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stack.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/_stack.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 import torch
 from typing import Optional, List, Tuple, Sequence
-from ._multihead_attention import ATTENTION_TYPE
+from .multihead_attention import ATTENTION_TYPE, ScaledDotProductAttention
 from ._stages import TransformerEncoderStage, TransformerDecoderStage
 from torch.utils.checkpoint import checkpoint
 
 
 class TransformerEncoder(torch.nn.Module):
     """
     A transformer encoder is a sequence of TransformerEncoderStage
     """
 
     def __init__(self, n_stages: int, projection_dim: int, n_heads: int,
                  dropout: Optional[float] = None, activation: str = "relu",
-                 RPE_radius: Optional[int] = None, attention_type: ATTENTION_TYPE = "scaled dot product",
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True,
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
+                 **kwargs):
         super().__init__()
         self.stages: Sequence[TransformerEncoderStage] = torch.nn.ModuleList()
-        self.low_memory = low_memory
+        self.gradient_checkpointing = gradient_checkpointing
         for stage in range(n_stages):
             self.stages.append(TransformerEncoderStage(projection_dim, n_heads,
                                                        dropout=dropout, activation=activation,
-                                                       RPE_radius=RPE_radius,
-                                                       attention_type=attention_type))
+                                                       attention_type=attention_type, **kwargs))
 
-    def forward(self, X: torch.Tensor, padding_mask: Optional[torch.Tensor] = None):
+    def forward(self, X: torch.Tensor, padding_mask: Optional[torch.Tensor] = None, attention_kwargs: dict = {}):
         """
         Parameter
         ---------
         X : torch.Tensor
             Tensor of shape (N, L, D) with
             * N sentences count
             * L sequence length
             * D number of features
         padding_mask : torch.tensor or None
             tensor of booleans of shape (N, L) of tokens to ignore
+        attention_kwargs : dict
+            additional kwargs passed to self attention
 
         Returns
         -------
         torch.Tensor
             tensor of shape (N, L, D)
         """
         for stage in self.stages:
-            if self.low_memory and self.training:
-                X = checkpoint(stage, X, padding_mask)
+            if self.gradient_checkpointing and self.training:
+                X = checkpoint(stage, X, padding_mask, attention_kwargs)
             else:
-                X = stage(X, padding_mask)
+                X = stage(X, padding_mask, attention_kwargs)
         return X
 
 
 class TransformerDecoder(torch.nn.Module):
     """
     A transformer decoder is a sequence of TransformerDecoderStage
     """
 
     def __init__(self, n_stages: int, projection_dim: int, n_heads: int,
                  dropout: Optional[float] = None, activation: str = "relu",
-                 RPE_radius: Optional[int] = None, attention_type: ATTENTION_TYPE = "scaled dot product",
-                 low_memory: bool = True):
+                 gradient_checkpointing: bool = True, 
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
+                 **kwargs):
         super().__init__()
         self.stages: Sequence[TransformerDecoderStage] = torch.nn.ModuleList()
-        self.low_memory = low_memory
+        self.gradient_checkpointing = gradient_checkpointing
         for stage in range(n_stages):
             self.stages.append(TransformerDecoderStage(projection_dim, n_heads,
                                                        dropout=dropout, activation=activation,
-                                                       RPE_radius=RPE_radius,
-                                                       attention_type=attention_type))
+                                                       attention_type=attention_type, **kwargs))
 
     def forward(self, Y: torch.Tensor, encoded: torch.Tensor,
                 encoded_padding_mask: Optional[torch.Tensor] = None):
         """
         Parameter
         ---------
         Y : torch.Tensor
@@ -80,15 +82,15 @@
 
         Returns
         -------
         torch.Tensor
             tensor of shape (N, L, D)
         """
         for stage in self.stages:
-            if self.low_memory and self.training:
+            if self.gradient_checkpointing and self.training:
                 Y = checkpoint(stage, Y, encoded, encoded_padding_mask)
             else:
                 Y = stage(Y, encoded, encoded_padding_mask)
         return Y
 
     def predict(self, intermediate: List[torch.Tensor],
                 Q: torch.Tensor, encoded: torch.Tensor,
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_stages.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/_stages.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,58 +1,57 @@
 import torch
 from typing import Optional
-from ._multihead_attention import MultiHeadAttention, ATTENTION_TYPE
+from .multihead_attention import ATTENTION_TYPE, ScaledDotProductAttention
 from pygmalion.neural_networks.layers._dropout import Dropout
-from torch.utils.checkpoint import checkpoint
 
 
 class TransformerEncoderStage(torch.nn.Module):
 
     def __init__(self, projection_dim: int, n_heads: int,
                  dropout: Optional[float] = None,
-                 activation: str = "relu", RPE_radius: Optional[int] = None,
-                 attention_type: ATTENTION_TYPE = "scaled dot product",
+                 activation: str = "relu",
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
+                 mask_future: bool = False,
                  **kwargs):
         super().__init__()
         dim = projection_dim * n_heads
         self.activation = getattr(torch, activation)
-        self.self_attention = MultiHeadAttention(projection_dim, n_heads, False,
-                                                 RPE_radius=RPE_radius,
-                                                 attention_type=attention_type,
-                                                 **kwargs)
+        self.self_attention = attention_type(projection_dim, n_heads, mask_future=mask_future, **kwargs)
         self.intermediate_norm = torch.nn.LayerNorm(dim)
         self.intermediate_dropout = Dropout(dropout)
         self.expand = torch.nn.Linear(dim, dim * 4)
         self.contract = torch.nn.Linear(dim * 4, dim)
         self.out_dropout = Dropout(dropout)
         self.out_norm = torch.nn.LayerNorm(dim)
 
     def forward(self, X: torch.Tensor,
-                padding_mask: Optional[torch.Tensor] = None):
+                padding_mask: Optional[torch.Tensor] = None,
+                attention_kwargs: dict = {}):
         """
         Parameter
         ---------
         X : torch.Tensor
             Tensor of shape (N, L, D) with
             * N sentences count
             * L sequence length
             * D number of features
-
         padding_mask : torch.tensor or None
             tensor of booleans of shape (N, L) of tokens to ignore
+        attention_kwargs : dict
+            kwargs passed to self_attention
 
         Returns
         -------
         torch.Tensor
             tensor of shape (N, L, D)
         """
         X = X.to(self.device)
         N, L, _ = X.shape
         input = X.reshape(N * L, -1)
-        X = self.self_attention(X, X, padding_mask, padding_mask).reshape(N * L, -1)
+        X = self.self_attention(X, X, padding_mask, padding_mask, **attention_kwargs).reshape(N * L, -1)
         X = self.intermediate_dropout(X) + input
         X = self.intermediate_norm(X)
         input = X
         X = self.contract(self.activation(self.expand(X)))
         X = self.out_dropout(X)
         X = self.out_norm(X + input)
         return X.reshape(N, L, -1)
@@ -62,29 +61,23 @@
         return self.self_attention.key.weight.device
 
 
 class TransformerDecoderStage(torch.nn.Module):
 
     def __init__(self, projection_dim: int, n_heads: int,
                  dropout: Optional[float] = None, activation: str = "relu",
-                 RPE_radius: Optional[int] = None,
-                 attention_type: ATTENTION_TYPE = "scaled dot product",
+                 attention_type: ATTENTION_TYPE = ScaledDotProductAttention,
                  **kwargs):
         super().__init__()
         dim = projection_dim * n_heads
         self.activation = getattr(torch, activation)
-        self.masked_self_attention = MultiHeadAttention(projection_dim, n_heads, True,
-                                                        RPE_radius=RPE_radius,
-                                                        attention_type=attention_type,
-                                                        **kwargs)
+        self.masked_self_attention = attention_type(projection_dim, n_heads, mask_future=True, **kwargs)
         self.first_dropout = Dropout(dropout)
         self.first_norm = torch.nn.LayerNorm(dim)
-        self.attention = MultiHeadAttention(projection_dim, n_heads, False,
-                                            RPE_radius=RPE_radius,
-                                            attention_type=attention_type)
+        self.attention = attention_type(projection_dim, n_heads, mask_future=False, **kwargs)
         self.second_dropout = Dropout(dropout)
         self.second_norm = torch.nn.LayerNorm(dim)
         self.expand = torch.nn.Linear(dim, 4 * dim)
         self.contract = torch.nn.Linear(4 * dim, dim)
         self.out_dropout = Dropout(dropout)
         self.out_norm = torch.nn.LayerNorm(dim)
 
@@ -109,16 +102,16 @@
         Y = Y.to(self.device)
         N, L, _ = Y.shape
         input = Y.reshape(N * L, -1)
         Y = self.masked_self_attention(Y, Y).reshape(N * L, -1)
         Y = self.first_dropout(Y)
         Y = self.first_norm(Y + input).reshape(N, L, -1)
         input = Y.reshape(N * L, -1)
-        Y = self.attention(Y, encoded, query_padding_mask=None,
-                           key_padding_mask=encoded_padding_mask).reshape(N * L, -1)
+        Y = self.attention(Y, encoded, query_mask=None,
+                           key_mask=encoded_padding_mask).reshape(N * L, -1)
         Y = self.second_dropout(Y)
         Y = self.second_norm(Y + input)
         input = Y
         Y = self.contract(self.activation(self.expand(Y)))
         Y = self.out_dropout(Y)
         Y = self.out_norm(Y + input)
         return Y.reshape(N, L, -1)
@@ -145,20 +138,20 @@
         """
         assert not self.training
         encoded = encoded.to(self.device)
         Y = Y.to(self.device)
         N, L, _ = Y.shape
         Q = Y[:, -1:, :]
         input = Q.reshape(N, -1)
-        Q = self.masked_self_attention(Q, Y, mask_index_offset=L-1).reshape(N, -1)
+        Q = self.masked_self_attention(Q, Y, future_offset=L-1).reshape(N, -1)
         Q = self.first_norm(Q + input).reshape(N, 1, -1)
         input = Q.reshape(N, -1)
-        Q = self.attention(Q, encoded, query_padding_mask=None,
-                           key_padding_mask=encoded_padding_mask,
-                           mask_index_offset=L-1).reshape(N, -1)
+        Q = self.attention(Q, encoded, query_mask=None,
+                           key_mask=encoded_padding_mask,
+                           future_offset=L-1).reshape(N, -1)
         Q = self.second_norm(Q + input)
         input = Q
         Q = self.contract(self.activation(self.expand(Q)))
         Q = self.out_norm(Q + input)
         return Q.reshape(N, 1, -1)
 
     @property
```

### Comparing `pygmalion-0.1.5/pygmalion/neural_networks/layers/transformers/_utilities.py` & `pygmalion-0.1.6/pygmalion/neural_networks/layers/transformers/_utilities.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         rep = rep.expand(*(n-L if i == dim else -1 for i, _ in enumerate(rep.shape)))
         tensor = torch.cat([tensor, rep], dim=dim)
     elif L > n:
         tensor = (tensor.moveaxis(dim, 0)[:n]).moveaxis(0, dim)
     return tensor
 
 
-def _mask_chronological(Lq: int, Lk: int, device: torch.device, mask_index_offset: int=0) -> torch.Tensor:
+def _mask_chronological(Lq: int, Lk: int, device: torch.device, future_offset: int=0) -> torch.Tensor:
     """
     A mask for transformers attention
 
     Parameters
     ----------
     Lq : int
         the sequence length of queries
@@ -31,15 +31,15 @@
 
     Returns
     -------
     torch.Tensor :
         tensor of booleans of shape (Lq, Lk)
     """
     mask = torch.ones(Lq, Lk, dtype=torch.bool, device=device)
-    mask = torch.triu(mask, diagonal=1+mask_index_offset)
+    mask = torch.triu(mask, diagonal=1+future_offset)
     return mask
 
 
 def _log_exp_kernel(x: torch.Tensor) -> torch.Tensor:
     """
     a default kernel function for kernelized attention
     """
```

### Comparing `pygmalion-0.1.5/pygmalion/tokenizers/_ascii_char_tokenizer.py` & `pygmalion-0.1.6/pygmalion/tokenizers/_ascii_char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/tokenizers/_byte_pair_encoder.py` & `pygmalion-0.1.6/pygmalion/tokenizers/_byte_pair_encoder.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_bytes_tree.py` & `pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_bytes_tree.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_functions.py` & `pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_functions.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/tokenizers/_utilities/_tokenizer.py` & `pygmalion-0.1.6/pygmalion/tokenizers/_utilities/_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/tokenizers/_words_tokenizer.py` & `pygmalion-0.1.6/pygmalion/tokenizers/_words_tokenizer.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/unsupervised/pca.py` & `pygmalion-0.1.6/pygmalion/unsupervised/_pca.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/utilities/_cross_validation.py` & `pygmalion-0.1.6/pygmalion/utilities/_cross_validation.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/utilities/_decorators.py` & `pygmalion-0.1.6/pygmalion/utilities/_decorators.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/utilities/_download.py` & `pygmalion-0.1.6/pygmalion/utilities/_download.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/utilities/_load_model.py` & `pygmalion-0.1.6/pygmalion/utilities/_load_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import torch
 from typing import Union, Type
 from io import IOBase
 from pygmalion._model import Model
 from ._download import download_bytes
 from pygmalion.unsupervised import *
 from pygmalion.neural_networks import *
+from pygmalion.decision_trees import *
 from pygmalion.tokenizers import *
 
 
 def load_model(file_path: Union[str, pathlib.Path, IOBase]) -> Model:
     """
     loads a model from the disk, or download from google drive.
```

### Comparing `pygmalion-0.1.5/pygmalion/utilities/_metrics.py` & `pygmalion-0.1.6/pygmalion/utilities/_metrics.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion/utilities/_ploting.py` & `pygmalion-0.1.6/pygmalion/utilities/_ploting.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/pygmalion.egg-info/PKG-INFO` & `pygmalion-0.1.6/pygmalion.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,167 +1,189 @@
 Metadata-Version: 2.1
 Name: pygmalion
-Version: 0.1.5
+Version: 0.1.6
 Summary: A machine learning package
 Home-page: https://github.com/BFavier/Pygmalion
 Author: Benoit Favier
 Author-email: benoitfamillefavier@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: GPU :: NVIDIA CUDA
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-Pygmalion in the greek mythologie is a sculptor that fell in love with one of his creations.
-In the myth, Aphrodite gives life to Galatea, the sculpture he fell in love with. This package is a machine learning library. It contains the tools to give a mind of their own to inanimate objects.
+Pygmalion in the greek mythologie is a sculptor that fell in love with one of his creations. In the myth, Aphrodite gives life to Galatea, the sculpture he fell in love with. This package is a python machine learning library that implements models for some common machine learning tasks. Everything that you need to give a mind of their own to inanimate objects.
 
 # Installing pygmalion
 
 pygmalion can be installed through pip.
 
 ~~~
-pip install pygmalion
+python -m pip install pygmalion
 ~~~
 
 # Fast prototyping of models with pygmalion
 
-Architectures for several common machine learning tasks (regression, image classification, ...) are implemented in this package.
+Architectures for several common machine learning tasks (regression, image classification, machine translation ...) are implemented in this package.
 
-The inputs and outputs of the models are common python objects (such as numpy array and pandas dataframes) so there are few new things you need to learn to use this package.
+The inputs and outputs of the models are common python objects (such as numpy array and pandas dataframes).
 
-In this part we are going to see how to load a dataset, train a model, and display some metrics. As a first step you can import the following packages.
+In this section we are going to see how to load a dataset, train a model, display some metrics, and save a model.
 
 ~~~python
 >>> import pygmalion as ml
 >>> import pygmalion.neural_networks as nn
 >>> import pandas as pd
 >>> import numpy as np
 >>> import matplotlib.pyplot as plt
 ~~~
 
 You can download a dataset and split it with the **split** function.
 
 ~~~python
 >>> ml.datasets.boston_housing("./")
 >>> df = pd.read_csv("./boston_housing.csv")
->>> x, y = df[[c for c in d_Fcolumns if c != "medv"]], df["medv"]
->>> train_data, val_data, test_data = ml.split(x, y, frac=(0.1, 0.1))
+>>> df_train, df_val, df_test = ml.utilities.split(df, weights=(0.8, 0.1, 0.1))
 ~~~
 
-Creating and training a model is done in a few lines of code.
+Creating and training a model takes few lines of code.
 
 ~~~python
->>> hidden_layers = [{"features": 8}, {"features": 8}]
->>> model = nn.DenseRegressor(x.columns, hidden_layers)
->>> model.train(train_data, val_data, n_epochs=1000, patience=100, learning_rate=1.0E-3)
+>>> inputs, target = [c for c in df.columns if c != "medv"], "medv"
+>>> model = nn.DenseRegressor(inputs, target, hidden_layers=[32, 32])
+>>> x_train, y_train = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> x_val, y_val = model.data_to_tensor(df_val[inputs], df_val[target])
+>>> history = model.fit((x_train, y_train), (x_val, y_val), n_steps=1000, patience=100, learning_rate=1.0E-3)
 ~~~
 
 Some usefull metrics can easily be evaluated.
 
 For a regressor model, the available metrics are [**MSE**](https://en.wikipedia.org/wiki/Mean_squared_error), [**RMSE**](https://en.wikipedia.org/wiki/Root-mean-square_deviation), [**R2**](https://en.wikipedia.org/wiki/Coefficient_of_determination), and the correlation between target and prediction can be visualized with the **plot_fitting** function.
 
 ~~~python
 >>> f, ax = plt.subplots()
->>> x_train, y_train = train_data
->>> ml.plot_fitting(model(x_train), y_train, ax=ax, label="training")
->>> x_val, y_val = val_data
->>> ml.plot_fitting(model(x_val), y_val, ax=ax, label="validation")
->>> x_test, y_test = test_data
->>> ml.plot_fitting(model(x_test), y_test, ax=ax, label="testing", color="C3")
->>> R2 = ml.R2(model(x_test), y_test)
+>>> ml.utilities.plot_fitting(df_train[target], model.predict(df_train), ax=ax, label="training")
+>>> ml.utilities.plot_fitting(df_val[target], model.predict(df_val), ax=ax, label="validation")
+>>> ml.utilities.plot_fitting(df_test[target], model.predict(df_test), ax=ax, label="testing", color="C3")
+>>> R2 = ml.utilities.R2(model.predict(df_test), df_test[target])
 >>> ax.set_title(f"RÂ²={R2:.3g}")
+>>> ax.set_xlabel("target")
+>>> ax.set_ylabel("predicted")
 >>> plt.show()
 ~~~
 
 ![pairplot](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/boston_housing_pairplot.png)
 
 
 For a classifier model you can evaluate the [**accuracy**](https://en.wikipedia.org/wiki/Accuracy_and_precision#In_binary_classification), and display the confusion matrix.
 
 ~~~python
 >>> ml.datasets.iris("./")
 >>> df = pd.read_csv("./iris.csv")
->>> x, y = df[[c for c in d_Fcolumns if c != "variety"]], df["variety"]
->>> inputs, classes = x.columns(), y.unique()
->>> hidden_layers = [{"features": 5},
->>>                  {"features": 5},
->>>                  {"features": 5}]
->>> model = nn.DenseClassifier(inputs, classes,
->>>                            hidden_layers=hidden_layers,
->>>                            activation="elu")
->>> train_data, val_data, test_data = ml.split(x, y, frac=(0.2, 0.1))
->>> model.train(train_data, val_data, n_epochs=1000, patience=100)
+>>> df_train, df_val, df_test = ml.utilities.split(df, weights=(0.7, 0.2, 0.1))
+>>> inputs, target = [c for c in df.columns if c != "variety"], "variety"
+>>> classes = df[target].unique()
+>>> model = nn.DenseClassifier(inputs, target, classes, hidden_layers=[8, 8, 8])
+>>> train_data = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> val_data = model.data_to_tensor(df_train[inputs], df_train[target])
+>>> model.fit(train_data, val_data, n_steps=1000, patience=100)
 >>> f, ax = plt.subplots()
->>> x_test, y_test = test_data
->>> ml.plot_matrix(ml.confusion_matrix(y_test, y_pred, classes=classes),
-...                ax=ax, cmap="Greens", write_values=True, format=".2%")
->>> acc = ml.accuracy(y_pred, y)*100
->>> ax.set_title(f"Accuracy: {acc:.2f}%")
+>>> y_test, y_pred = df_test[target], model.predict(df_test)
+>>> ml.utilities.plot_matrix(ml.utilities.confusion_matrix(y_test, y_pred, classes=classes), ax=ax, cmap="Greens", write_values=True, format=".2%")
+>>> acc = ml.utilities.accuracy(y_pred, y_test)
+>>> ax.set_title(f"Accuracy: {acc:.2%}")
 >>> plt.tight_layout()
 >>> plt.show()
 ~~~
 
 ![confusion matrix](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/iris_confusion_matrix.png)
 
-All the models can be dumped as a dictionnary through the **dump** property. A copy of the model can be loaded with the **from_dump** class method.
+All the models can be saved directly to the disk with the **save** method.
+A model saved on the disk can then be loaded back with the **load_model** function.
 
 ~~~python
->>> dump = model.dump
->>> model = nn.DenseRegressor.from_dump(dump)
-~~~
-
-The models can also be be saved directly to the disk in json/hdf5 format with the **save** method.
-A model saved on the disk can then be loaded back with the **load** function.
-
-~~~python
->>> model.save("./model.json")
->>> model = ml.load("./model.json")
+>>> model.save("./model.pth")
+>>> model = ml.utilities.load_model("./model.pth")
 ~~~
 
 # Implemented models
 
 For examples of model training see the **samples** folder in the [github page](https://github.com/BFavier/Pygmalion).
 
 ## Neural networks
 
 The neural networks are implemented in pytorch under the hood.
-The underlying pytorch Module and Optimizer can be accessed as the **model** and **optimizer** attributes of the model.
+Each model is a pytorch **Module**. The fit method of neural networks returns a train loss, validation loss, gradient scale history that can be ploted with the **plot_loss** functions.
 
-### **DenseRegressor**
+~~~python
+>>> train_losses, val_losses, grad, best_step = model.fit(...)
+>>> ml.utilities.plot_losses(train_losses, val_losses, grad, best_step)
+~~~
 
-A dense regressor (or multi layer perceptron regressor) predicts a scalar value given an input of several variables.
+![loss history](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/Fashion_MNIST_residuals.png)
 
-This implementation takes in input **x** a pandas.DataFrame of numerical observations, and returns **y** a numpy.ndarray of floats of the same length. The optional **weights** weighting of the observations during training are numpy.ndarray of floats.
+### **DenseRegressor**
 
-It is implemented as a sucession of hidden **Activated0d** layers (linear weighting/non linear activation/batch normalization) and a final linear weighting to reduces the number of features to one scalar prediction.
+A DenseRegressor (or multi layer perceptron regressor) predicts a scalar value given an input of several variables. An example of DenseRegressor training was demonstrated in a previous section.
 
 ### **DenseClassifier**
 
-A dense classifier (or multi layer perceptron classifier) predicts a str class value given an input of several variables.
-
-This implementation takes in input **x** a pandas.DataFrame of numerical observations, and returns **y** list of str of the same length. The optional **weights** weighting of the observations during training are numpy.ndarray of floats.
-
-Similarly to the DenseRegressor it is a succession of hidden **Activated0d** layers, and a final linear layer with as much output as there are classes to predict.
+A DenseClassifier (or multi layer perceptron classifier) predicts a str class value given an input of several variables. An example of DenseClassifier training was presented in a previous section.
 
 ### **ImageClassifier**
 
 An ImageClassifier predicts a str class given as input an image. Here below the predictions of a model trained on the fashion-MNIST dataset.
 
 ![fashion-MNIST predictions](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/Fashion_MNIST_illustration.png)
 
-It is implemented as a Convolutional Neural Network similar to LeNet.
+It is implemented as a Convolutional Neural Network similar to ResNet.
+
+### **ImageSegmenter**
 
-### **SemanticSegmenter**
+An ImageSegmenter predicts a class for each pixel of the input image (semantic segmentation). Here below the predictions of a model trained on the cityscape dataset.
 
-A SemanticSegmenter predicts a class for each pixel of the input image. Here below the predictions of a model trained on the cityscape dataset.
+![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/segmented_cityscape.png)
 
-![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/segmented_cityscape_2.png)
+It is implemented as a Convolutional Neural Network similar to U-Net.
 
-It is implemented as a Convolutional Neural Network similar to U-Net. It is a succession of convolutions/pooling followed by a succession of upsampling/convolutions, leading to a convergent/divergent feature map structure. The feature map before each downsampling stage is concatenated to the upsampling of the same size to preserve features.
+### **ImageObjectDetector**
 
+An ImageObjectDetector predict the presence and box coordinates of objects in an image. This model is an implementation of the YOLO convolutional neural network. Here below the prediction of a model trained to detect circles and squares in images generated on the fly:
 
+![segmented_cityscapes](https://raw.githubusercontent.com/BFavier/Pygmalion/main/images/ImageObjectDetector.png)
 
+### **TextClassifier**
+
+A TextClassifier classifies text inputs. It is implemented as a transformer encoder. Here below some prediction of the model on a sentiment analysis task where tweets were to be classified as positive, neutral or negative.
+
+~~~
+@JetBlue Thanks! Her flight leaves at 2 but she's arriving to the airport early. Wedding is in VT in Sept. Grateful you fly to BTV!! :)
+>>> positive
+
+@united how are conditions in BOS today? I'm in UA994. Everything appears to be in time but I wanted to check.
+>>> neutral
+
+@AmericanAir it's been almost 3 days and it's still frozen. Thanks doll ðŸ˜˜ðŸ˜‘
+>>> negative
+~~~
+
+### **TextTranslator**
+
+A TextTranslator model predicts a string outputs for a string inputs. It is implemented as an encoder/decoder transformer. Here below some predictions of a model trained to translate arabic numerals to roman numerals.
+
+~~~
+402 >>> ['CDII']
+863 >>> ['DCCCLXIII']
+1275 >>> ['MCCLXXV']
+798 >>> ['DCCXCVIII']
+1532 >>> ['MDXXXII']
+223 >>> ['CCXXIII']
+90 >>> ['XC']
+1261 >>> ['MCCLXI']
+1032 >>> ['MXXXII']
+432 >>> ['CDXXXII']
+~~~
```

### Comparing `pygmalion-0.1.5/pygmalion.egg-info/SOURCES.txt` & `pygmalion-0.1.6/pygmalion.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -17,58 +17,72 @@
 pygmalion/datasets/_fashion_mnist.py
 pygmalion/datasets/_iris.py
 pygmalion/datasets/_sentence_pairs.py
 pygmalion/datasets/_titanic.py
 pygmalion/datasets/_usa_economy.py
 pygmalion/datasets/generators/__init__.py
 pygmalion/datasets/generators/_circles_generator.py
+pygmalion/datasets/generators/_orbital_trajectory_generator.py
 pygmalion/datasets/generators/_roman_numerals_generator.py
 pygmalion/datasets/generators/_shapes_generator.py
+pygmalion/decision_trees/__init__.py
+pygmalion/decision_trees/_branch.py
+pygmalion/decision_trees/_decision_tree.py
+pygmalion/decision_trees/_gradient_boosting_classifier.py
+pygmalion/decision_trees/_gradient_boosting_regressor.py
+pygmalion/decision_trees/_monotonicity.py
 pygmalion/neural_networks/__init__.py
 pygmalion/neural_networks/_conversions.py
 pygmalion/neural_networks/_dense_classifier.py
 pygmalion/neural_networks/_dense_regressor.py
 pygmalion/neural_networks/_image_classifier.py
 pygmalion/neural_networks/_image_object_detector.py
 pygmalion/neural_networks/_image_segmenter.py
 pygmalion/neural_networks/_loss_functions.py
 pygmalion/neural_networks/_neural_network.py
 pygmalion/neural_networks/_text_classifier.py
 pygmalion/neural_networks/_text_segmenter.py
 pygmalion/neural_networks/_text_translator.py
+pygmalion/neural_networks/_time_series_regressor.py
 pygmalion/neural_networks/layers/__init__.py
 pygmalion/neural_networks/layers/_activation.py
 pygmalion/neural_networks/layers/_dropout.py
 pygmalion/neural_networks/layers/_normalization.py
-pygmalion/neural_networks/layers/_positional_encoding.py
 pygmalion/neural_networks/layers/convolutions/__init__.py
 pygmalion/neural_networks/layers/convolutions/_conv_block.py
 pygmalion/neural_networks/layers/convolutions/_padded_conv.py
 pygmalion/neural_networks/layers/convolutions/_stack.py
 pygmalion/neural_networks/layers/convolutions/_stages.py
 pygmalion/neural_networks/layers/convolutions/_upsampling.py
+pygmalion/neural_networks/layers/positional_encoding/__init__.py
+pygmalion/neural_networks/layers/positional_encoding/_learned_positional_encoding.py
+pygmalion/neural_networks/layers/positional_encoding/_sinusoidal_positional_encoding.py
 pygmalion/neural_networks/layers/transformers/__init__.py
-pygmalion/neural_networks/layers/transformers/_attention.py
-pygmalion/neural_networks/layers/transformers/_multihead_attention.py
 pygmalion/neural_networks/layers/transformers/_stack.py
 pygmalion/neural_networks/layers/transformers/_stages.py
 pygmalion/neural_networks/layers/transformers/_utilities.py
+pygmalion/neural_networks/layers/transformers/multihead_attention/__init__.py
+pygmalion/neural_networks/layers/transformers/multihead_attention/_fourier_kernel_attention.py
+pygmalion/neural_networks/layers/transformers/multihead_attention/_kernelized_attention.py
+pygmalion/neural_networks/layers/transformers/multihead_attention/_scaled_dot_product.py
+pygmalion/neural_networks/layers/transformers/multihead_attention/_utilities.py
 pygmalion/tokenizers/__init__.py
 pygmalion/tokenizers/_ascii_char_tokenizer.py
 pygmalion/tokenizers/_byte_pair_encoder.py
 pygmalion/tokenizers/_words_tokenizer.py
 pygmalion/tokenizers/_utilities/__init__.py
 pygmalion/tokenizers/_utilities/_bytes_tree.py
 pygmalion/tokenizers/_utilities/_functions.py
 pygmalion/tokenizers/_utilities/_special_token.py
 pygmalion/tokenizers/_utilities/_tokenizer.py
 pygmalion/unsupervised/__init__.py
-pygmalion/unsupervised/pca.py
+pygmalion/unsupervised/_pca.py
 pygmalion/utilities/__init__.py
 pygmalion/utilities/_cross_validation.py
+pygmalion/utilities/_data_processing.py
 pygmalion/utilities/_decorators.py
 pygmalion/utilities/_download.py
 pygmalion/utilities/_load_model.py
 pygmalion/utilities/_metrics.py
 pygmalion/utilities/_ploting.py
 test/test_decoder_stage.py
 test/test_kernelized_attention.py
```

### Comparing `pygmalion-0.1.5/setup.py` & `pygmalion-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/test/test_decoder_stage.py` & `pygmalion-0.1.6/test/test_decoder_stage.py`

 * *Files identical despite different names*

### Comparing `pygmalion-0.1.5/test/test_kernelized_attention.py` & `pygmalion-0.1.6/test/test_kernelized_attention.py`

 * *Files identical despite different names*

