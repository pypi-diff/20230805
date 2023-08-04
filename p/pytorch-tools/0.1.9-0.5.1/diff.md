# Comparing `tmp/pytorch_tools-0.1.9.tar.gz` & `tmp/pytorch_tools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytorch_tools-0.1.9.tar", last modified: Fri Jan 22 15:00:52 2021, max compression
+gzip compressed data, was "pytorch_tools-0.5.1.tar", last modified: Fri Aug  4 22:06:32 2023, max compression
```

## Comparing `pytorch_tools-0.1.9.tar` & `pytorch_tools-0.5.1.tar`

### file list

```diff
@@ -1,139 +1,153 @@
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1084 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/LICENSE
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       87 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/requirements.txt
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      841 2020-01-31 16:26:45.000000 pytorch_tools-0.1.9/.gitignore
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       38 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/setup.cfg
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      942 2020-07-08 12:35:37.000000 pytorch_tools-0.1.9/setup.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1503 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/PKG-INFO
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:51.000000 pytorch_tools-0.1.9/tests/
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/modules/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5698 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/tests/modules/test_modules.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/models/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3530 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/models/test_models.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2213 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/models/test_weights.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/utils/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    10537 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/tests/utils/test_box_utils.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      544 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/tests/utils/test_misc_utils.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/losses/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    22815 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/tests/losses/test_losses.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/fit_wrapper/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5506 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/tests/fit_wrapper/test_runner.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/tta_wrapper/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3487 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/tests/tta_wrapper/test_tta.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/detection_models/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2165 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/detection_models/test_det_models.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/imgs/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    49918 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/imgs/cityscapes_sample.jpg
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    85657 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/imgs/helmet.jpeg
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    76081 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/imgs/dog.jpg
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)   428014 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/imgs/cityscapes_sample2.jpg
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/benchmarking/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    12359 2021-01-22 14:51:14.000000 pytorch_tools-0.1.9/tests/benchmarking/memory_test.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1382 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/tests/benchmarking/benchmarking_example.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     4027 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/tests/benchmarking/README.md
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/metrics/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3961 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/tests/metrics/test_metric.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/tests/segmentation_models/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3346 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/tests/segmentation_models/test_segm_models.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:51.000000 pytorch_tools-0.1.9/pytorch_tools/
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/modules/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5062 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/modules/spatial_ocr_block.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1790 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/modules/weight_standartization.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     6092 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/modules/activated_batch_norm.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     8966 2020-07-20 17:54:27.000000 pytorch_tools-0.1.9/pytorch_tools/modules/bifpn.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2252 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/modules/fpn.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3447 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/modules/pooling.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    48473 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/modules/residual.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1385 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/modules/activated_no_norm.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5221 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/modules/activated_batch_channel_norm.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2425 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/modules/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2408 2021-01-22 14:51:10.000000 pytorch_tools-0.1.9/pytorch_tools/modules/activated_group_norm.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     6749 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/modules/decoder.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5223 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/pytorch_tools/modules/activations.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3531 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/modules/tf_same_ops.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/optim/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     6481 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/optim/radam.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2585 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/optim/rmsprop.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    10890 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/optim/lr_finder.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2274 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/optim/lookahead.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2181 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/optim/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5431 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/optim/adamw.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     4261 2020-04-27 10:15:56.000000 pytorch_tools-0.1.9/pytorch_tools/optim/sgdw.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1895 2020-05-08 12:48:56.000000 pytorch_tools-0.1.9/pytorch_tools/optim/schedulers.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       47 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/optim/README.md
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      266 2021-01-22 14:57:58.000000 pytorch_tools-0.1.9/pytorch_tools/__init__.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/models/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    18196 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/models/hrnet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      832 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/models/preprocessing.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    21665 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/models/b_model.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    19663 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/pytorch_tools/models/efficientnet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    30188 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/models/resnet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    11879 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/models/bit_resnet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     8333 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/models/vgg.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1578 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/models/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    10053 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/models/tresnet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    13867 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/models/densenet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2274 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/models/README.md
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/utils/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      832 2020-04-18 12:55:17.000000 pytorch_tools-0.1.9/pytorch_tools/utils/preprocessing.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1824 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/utils/rle.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    17580 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/utils/box.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)        0 2020-01-31 16:26:45.000000 pytorch_tools-0.1.9/pytorch_tools/utils/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     8403 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/utils/misc.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      825 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/pytorch_tools/utils/tensorboard.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2367 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/utils/visualization.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/losses/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3198 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/kld.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     4868 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/losses/vgg_loss.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      392 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/losses/wing_loss.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1135 2020-07-20 17:25:52.000000 pytorch_tools-0.1.9/pytorch_tools/losses/huber.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     7762 2020-04-29 16:59:34.000000 pytorch_tools-0.1.9/pytorch_tools/losses/lovasz.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     4315 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/focal.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      781 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     4124 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/smooth.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2914 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/angular.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1603 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/base.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3113 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/pytorch_tools/losses/detection.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3338 2020-04-29 16:59:34.000000 pytorch_tools-0.1.9/pytorch_tools/losses/dice_jaccard.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     6293 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/losses/functional.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      290 2020-04-02 08:13:52.000000 pytorch_tools-0.1.9/pytorch_tools/losses/README.md
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      520 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/losses/hinge.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5170 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/wrapper.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       28 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    31157 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/callbacks.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2257 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/README.md
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2075 2021-01-22 14:51:09.000000 pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/state.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5370 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/wrapper.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       25 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2787 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/functional.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      957 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/README.md
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/detection_models/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    14280 2020-07-20 17:56:38.000000 pytorch_tools-0.1.9/pytorch_tools/detection_models/efficientdet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      450 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/detection_models/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     8597 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/detection_models/retinanet.py
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/metrics/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      233 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/metrics/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2361 2020-07-20 17:58:55.000000 pytorch_tools-0.1.9/pytorch_tools/metrics/accuracy.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2056 2020-04-02 08:14:56.000000 pytorch_tools-0.1.9/pytorch_tools/metrics/psnr.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      720 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/metrics/dice_jaccard.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      272 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/metrics/README.md
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:52.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)    10053 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/hrnet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3997 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/linknet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3149 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/segm_bifpn.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      195 2020-07-20 17:56:38.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/__init__.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      393 2020-04-02 09:03:30.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/base.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     2429 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/encoders.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5392 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/segm_fpn.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3118 2021-01-22 14:51:11.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/deeplabv3_plus.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     5567 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/unet.py
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1421 2020-07-20 17:10:17.000000 pytorch_tools-0.1.9/pytorch_tools/segmentation_models/README.md
-drwxrwxr-x   0 zakirov   (1005) zakirov   (1005)        0 2021-01-22 15:00:51.000000 pytorch_tools-0.1.9/pytorch_tools.egg-info/
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     3815 2021-01-22 15:00:51.000000 pytorch_tools-0.1.9/pytorch_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)     1503 2021-01-22 15:00:47.000000 pytorch_tools-0.1.9/pytorch_tools.egg-info/PKG-INFO
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       14 2021-01-22 15:00:47.000000 pytorch_tools-0.1.9/pytorch_tools.egg-info/top_level.txt
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)       88 2021-01-22 15:00:47.000000 pytorch_tools-0.1.9/pytorch_tools.egg-info/requires.txt
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)        1 2021-01-22 15:00:47.000000 pytorch_tools-0.1.9/pytorch_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 zakirov   (1005) zakirov   (1005)      930 2020-09-04 13:42:55.000000 pytorch_tools-0.1.9/README.md
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.909974 pytorch_tools-0.5.1/
+-rw-r--r--   0 zakirove   (501) staff       (20)      841 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/.gitignore
+-rw-r--r--   0 zakirove   (501) staff       (20)      488 2022-09-27 11:07:55.000000 pytorch_tools-0.5.1/.pre-commit-config.yaml
+-rw-r--r--   0 zakirove   (501) staff       (20)     1084 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/LICENSE
+-rw-r--r--   0 zakirove   (501) staff       (20)     1414 2023-08-04 22:06:32.909809 pytorch_tools-0.5.1/PKG-INFO
+-rw-r--r--   0 zakirove   (501) staff       (20)     1010 2023-08-04 21:29:06.000000 pytorch_tools-0.5.1/README.md
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.892330 pytorch_tools-0.5.1/pytorch_tools/
+-rw-r--r--   0 zakirove   (501) staff       (20)      266 2023-08-04 22:06:04.000000 pytorch_tools-0.5.1/pytorch_tools/__init__.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.893287 pytorch_tools-0.5.1/pytorch_tools/detection_models/
+-rw-r--r--   0 zakirove   (501) staff       (20)      450 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/detection_models/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    14227 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/detection_models/efficientdet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     8567 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/detection_models/retinanet.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.894001 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/
+-rw-r--r--   0 zakirove   (501) staff       (20)     2350 2023-08-04 21:58:29.000000 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)       28 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    34337 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/callbacks.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2751 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/state.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3669 2022-09-27 11:05:42.000000 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/utils.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5144 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/wrapper.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.895900 pytorch_tools-0.5.1/pytorch_tools/losses/
+-rw-r--r--   0 zakirove   (501) staff       (20)      289 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/losses/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)      781 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/losses/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2914 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/losses/angular.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2251 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/losses/base.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3113 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/losses/detection.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3410 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/losses/dice_jaccard.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4189 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/losses/focal.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     6293 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/losses/functional.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      516 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/losses/hinge.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     1131 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/losses/huber.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3198 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/losses/kld.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     7729 2022-01-18 16:46:39.000000 pytorch_tools-0.5.1/pytorch_tools/losses/lovasz.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4631 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/losses/smooth.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4846 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/losses/vgg_loss.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      392 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/losses/wing_loss.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.896590 pytorch_tools-0.5.1/pytorch_tools/metrics/
+-rw-r--r--   0 zakirove   (501) staff       (20)      266 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/metrics/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)      233 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/metrics/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2357 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/metrics/accuracy.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      720 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/metrics/dice_jaccard.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2026 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/metrics/psnr.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.898042 pytorch_tools-0.5.1/pytorch_tools/models/
+-rw-r--r--   0 zakirove   (501) staff       (20)     2718 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/models/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)     1606 2022-01-18 18:37:04.000000 pytorch_tools-0.5.1/pytorch_tools/models/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    21700 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/models/b_model.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    11875 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/models/bit_resnet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5144 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/models/cmodel.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    13958 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/models/densenet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    19374 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/models/efficientnet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    18314 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/models/hrnet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      818 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/models/preprocessing.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    30118 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/models/resnet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     9966 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/models/tresnet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     8291 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/models/vgg.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.899856 pytorch_tools-0.5.1/pytorch_tools/modules/
+-rw-r--r--   0 zakirove   (501) staff       (20)     2259 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/pytorch_tools/modules/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5301 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/activated_batch_channel_norm.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     6172 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/activated_batch_norm.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2452 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/activated_group_norm.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     1388 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/activated_no_norm.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3057 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/activations.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     8968 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/bifpn.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2370 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/modules/conv.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     6759 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/decoder.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2222 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/fpn.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4799 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/modules/mlp.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3539 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/modules/pooling.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    58024 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/modules/residual.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5095 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/modules/spatial_ocr_block.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3555 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/modules/tf_same_ops.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     1790 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/modules/weight_standartization.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.900964 pytorch_tools-0.5.1/pytorch_tools/optim/
+-rw-r--r--   0 zakirove   (501) staff       (20)       48 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/optim/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)     2181 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/optim/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3716 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/optim/adamp.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     7472 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/optim/adamw.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2274 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/optim/lookahead.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    10890 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/optim/lr_finder.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     6481 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/optim/radam.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2587 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/optim/rmsprop.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     1895 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/optim/schedulers.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4309 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/optim/sgdw.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.902550 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/
+-rw-r--r--   0 zakirove   (501) staff       (20)     1413 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)      195 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      393 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/base.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3118 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/deeplabv3_plus.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2429 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/encoders.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     9856 2022-01-18 16:46:18.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/hrnet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3997 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/linknet.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3147 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/segm_bifpn.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5348 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/segm_fpn.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5782 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/segmentation_models/unet.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.903047 pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/
+-rw-r--r--   0 zakirove   (501) staff       (20)      956 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)       25 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2787 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/functional.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5350 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/wrapper.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.904404 pytorch_tools-0.5.1/pytorch_tools/utils/
+-rw-r--r--   0 zakirove   (501) staff       (20)      156 2022-09-08 12:22:10.000000 pytorch_tools-0.5.1/pytorch_tools/utils/__init__.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    17546 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/pytorch_tools/utils/box.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     5179 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/pytorch_tools/utils/fuse.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3032 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/pytorch_tools/utils/guided_filter.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     6201 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/pytorch_tools/utils/misc.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      818 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/utils/preprocessing.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     1823 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/pytorch_tools/utils/rle.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     1156 2023-08-04 21:58:30.000000 pytorch_tools-0.5.1/pytorch_tools/utils/tensorboard.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     7437 2023-08-04 21:58:21.000000 pytorch_tools-0.5.1/pytorch_tools/utils/tiles.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2367 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/pytorch_tools/utils/visualization.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.892949 pytorch_tools-0.5.1/pytorch_tools.egg-info/
+-rw-r--r--   0 zakirove   (501) staff       (20)     1414 2023-08-04 22:06:32.000000 pytorch_tools-0.5.1/pytorch_tools.egg-info/PKG-INFO
+-rw-r--r--   0 zakirove   (501) staff       (20)     4228 2023-08-04 22:06:32.000000 pytorch_tools-0.5.1/pytorch_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 zakirove   (501) staff       (20)        1 2023-08-04 22:06:32.000000 pytorch_tools-0.5.1/pytorch_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 zakirove   (501) staff       (20)       55 2023-08-04 22:06:32.000000 pytorch_tools-0.5.1/pytorch_tools.egg-info/requires.txt
+-rw-r--r--   0 zakirove   (501) staff       (20)       14 2023-08-04 22:06:32.000000 pytorch_tools-0.5.1/pytorch_tools.egg-info/top_level.txt
+-rw-r--r--   0 zakirove   (501) staff       (20)       55 2023-08-04 21:39:22.000000 pytorch_tools-0.5.1/requirements.txt
+-rw-r--r--   0 zakirove   (501) staff       (20)       38 2023-08-04 22:06:32.910013 pytorch_tools-0.5.1/setup.cfg
+-rw-r--r--   0 zakirove   (501) staff       (20)      942 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/setup.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.891423 pytorch_tools-0.5.1/tests/
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.904935 pytorch_tools-0.5.1/tests/benchmarking/
+-rw-r--r--   0 zakirove   (501) staff       (20)     3939 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/tests/benchmarking/README.md
+-rw-r--r--   0 zakirove   (501) staff       (20)     1364 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/tests/benchmarking/benchmarking_example.py
+-rw-r--r--   0 zakirove   (501) staff       (20)    12136 2022-09-27 11:07:58.000000 pytorch_tools-0.5.1/tests/benchmarking/memory_test.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.905274 pytorch_tools-0.5.1/tests/detection_models/
+-rw-r--r--   0 zakirove   (501) staff       (20)     2165 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/detection_models/test_det_models.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.905635 pytorch_tools-0.5.1/tests/fit_wrapper/
+-rw-r--r--   0 zakirove   (501) staff       (20)    10634 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/tests/fit_wrapper/test_runner.py
+-rw-r--r--   0 zakirove   (501) staff       (20)      499 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/tests/fit_wrapper/test_utils.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.907851 pytorch_tools-0.5.1/tests/imgs/
+-rw-r--r--   0 zakirove   (501) staff       (20)    49918 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/imgs/cityscapes_sample.jpg
+-rw-r--r--   0 zakirove   (501) staff       (20)   428014 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/imgs/cityscapes_sample2.jpg
+-rw-r--r--   0 zakirove   (501) staff       (20)    76081 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/imgs/dog.jpg
+-rw-r--r--   0 zakirove   (501) staff       (20)    85657 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/imgs/helmet.jpeg
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.908220 pytorch_tools-0.5.1/tests/losses/
+-rw-r--r--   0 zakirove   (501) staff       (20)    24464 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/tests/losses/test_losses.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.908364 pytorch_tools-0.5.1/tests/metrics/
+-rw-r--r--   0 zakirove   (501) staff       (20)     3961 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/metrics/test_metric.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.908843 pytorch_tools-0.5.1/tests/models/
+-rw-r--r--   0 zakirove   (501) staff       (20)      213 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/tests/models/modules.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     6559 2022-03-31 12:08:27.000000 pytorch_tools-0.5.1/tests/models/test_cmodel.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3502 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/tests/models/test_models.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     2205 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/tests/models/test_weights.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.908957 pytorch_tools-0.5.1/tests/modules/
+-rw-r--r--   0 zakirove   (501) staff       (20)     7691 2022-09-27 11:07:59.000000 pytorch_tools-0.5.1/tests/modules/test_modules.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.909072 pytorch_tools-0.5.1/tests/segmentation_models/
+-rw-r--r--   0 zakirove   (501) staff       (20)     3346 2021-06-26 05:29:44.000000 pytorch_tools-0.5.1/tests/segmentation_models/test_segm_models.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.909190 pytorch_tools-0.5.1/tests/tta_wrapper/
+-rw-r--r--   0 zakirove   (501) staff       (20)     3557 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/tests/tta_wrapper/test_tta.py
+drwxr-xr-x   0 zakirove   (501) staff       (20)        0 2023-08-04 22:06:32.909624 pytorch_tools-0.5.1/tests/utils/
+-rw-r--r--   0 zakirove   (501) staff       (20)    10631 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/tests/utils/test_box_utils.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4454 2021-09-30 12:54:08.000000 pytorch_tools-0.5.1/tests/utils/test_misc_utils.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     4570 2022-09-08 12:20:26.000000 pytorch_tools-0.5.1/tests/utils/test_model_fuse.py
+-rw-r--r--   0 zakirove   (501) staff       (20)     3924 2023-08-04 21:58:21.000000 pytorch_tools-0.5.1/tests/utils/test_tiles.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pytorch_tools-0.1.9/LICENSE` & `pytorch_tools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/.gitignore` & `pytorch_tools-0.5.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/setup.py` & `pytorch_tools-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/modules/test_modules.py` & `pytorch_tools-0.5.1/tests/modules/test_modules.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import torch
 import pytest
 import pytorch_tools as pt
 import pytorch_tools.modules as modules
 
-activations_name = ["Swish", "Swish_Naive", "Mish", "Mish_naive"]
-INP = torch.ones(1, 10, 16, 16)
+activations_name = ["Mish", "Mish_naive"]
+INP = torch.ones(2, 10, 16, 16)
 
 
 @pytest.mark.parametrize("activation", activations_name)
 def test_activations_init(activation):
     act = modules.activation_from_name(activation)
     res = act(INP)
     assert res.mean()
@@ -54,15 +54,18 @@
 
 
 def test_abcn():
     """Check that abcn init and forward works"""
     l = modules.bn_from_name("abcn")(10, num_groups=2)
 
 
-# bcn runs
+def test_no_norm():
+    """check that can init without params"""
+    modules.bn_from_name("none")(10)
+    modules.bn_from_name("none")()
 
 
 def test_drop_connect_repr():
     """Check that keep_prob is shown correctly in DropConnect repr"""
     l = modules.residual.DropConnect(0.123)
     assert repr(l) == "DropConnect(keep_prob=0.12)"
 
@@ -83,58 +86,58 @@
     ws_m = modules.weight_standartization.conv_to_ws_conv(m)
     assert type(ws_m.blocks[1][0].conv_dw) == torch.nn.Conv2d
 
 
 def test_fpn_block():
     """Check that it works for different number of input feature maps"""
     inp_channels = [15, 16, 17, 18]
-    inp = [torch.rand(1, in_ch, 2 * 2 ** idx, 2 * 2 ** idx) for idx, in_ch in enumerate(inp_channels)]
+    inp = [torch.rand(1, in_ch, 2 * 2**idx, 2 * 2**idx) for idx, in_ch in enumerate(inp_channels)]
     # test for 4 features maps
     fpn4 = modules.fpn.FPN(inp_channels, pyramid_channels=55)
     res4 = fpn4(inp)
     for idx, r in enumerate(res4):
-        assert r.shape == torch.Size([1, 55, 2 * 2 ** idx, 2 * 2 ** idx])
+        assert r.shape == torch.Size([1, 55, 2 * 2**idx, 2 * 2**idx])
 
     # test that is also works for 3 feature maps
     fpn3 = modules.fpn.FPN(inp_channels[:3], pyramid_channels=55)
     res3 = fpn3(inp[:3])
     for idx, r in enumerate(res3):
-        assert r.shape == torch.Size([1, 55, 2 * 2 ** idx, 2 * 2 ** idx])
+        assert r.shape == torch.Size([1, 55, 2 * 2**idx, 2 * 2**idx])
 
 
 def test_fpn_num_layers():
     # FPN should only support one layer
     with pytest.raises(AssertionError):
         modules.fpn.FPN([1, 2, 3, 4], num_layers=2)
 
 
 def test_bifpn_block():
     """Check that it works for different number of input feature maps"""
     inp_channels = [15, 16, 17, 18, 19]
-    inp = [torch.rand(1, in_ch, 2 * 2 ** idx, 2 * 2 ** idx) for idx, in_ch in enumerate(inp_channels)]
+    inp = [torch.rand(1, in_ch, 2 * 2**idx, 2 * 2**idx) for idx, in_ch in enumerate(inp_channels)]
     # test for 5 features maps
     bifpn5 = modules.bifpn.BiFPN(inp_channels, pyramid_channels=55)
     res5 = bifpn5(inp)
     for idx, r in enumerate(res5):
-        assert r.shape == torch.Size([1, 55, 2 * 2 ** idx, 2 * 2 ** idx])
+        assert r.shape == torch.Size([1, 55, 2 * 2**idx, 2 * 2**idx])
 
     # test that is also works for 3 feature maps
     bifpn3 = modules.bifpn.BiFPN(inp_channels[:3], pyramid_channels=55)
     res3 = bifpn3(inp[:3])
     for idx, r in enumerate(res3):
-        assert r.shape == torch.Size([1, 55, 2 * 2 ** idx, 2 * 2 ** idx])
+        assert r.shape == torch.Size([1, 55, 2 * 2**idx, 2 * 2**idx])
 
 
 def test_first_bifpn_layer():
     inp_channels = [15, 16, 17, 18, 19]
-    inp = [torch.rand(1, in_ch, 2 * 2 ** idx, 2 * 2 ** idx) for idx, in_ch in enumerate(inp_channels)]
+    inp = [torch.rand(1, in_ch, 2 * 2**idx, 2 * 2**idx) for idx, in_ch in enumerate(inp_channels)]
     layer = modules.bifpn.FirstBiFPNLayer(inp_channels, 55)
     res = layer(inp)
     for idx, r in enumerate(res):
-        assert r.shape == torch.Size([1, 55, 2 * 2 ** idx, 2 * 2 ** idx])
+        assert r.shape == torch.Size([1, 55, 2 * 2**idx, 2 * 2**idx])
 
 
 def test_bifpn_num_layers():
     """Test different number of layers"""
     modules.bifpn.BiFPN([55, 55, 32, 30, 28], pyramid_channels=55, num_layers=2)
     modules.bifpn.BiFPN([1, 2, 3, 4], pyramid_channels=55, num_layers=2)
 
@@ -146,7 +149,57 @@
     out = s2d_4(inp)
     expected = torch.arange(16).view(1, -1, 1, 1)
     assert torch.allclose(out, expected)
     s2d_2 = modules.SpaceToDepth(block_size=2)
     out2 = s2d_2(inp)
     expected2 = torch.tensor([[[[0, 2], [8, 10]], [[1, 3], [9, 11]], [[4, 6], [12, 14]], [[5, 7], [13, 15]]]])
     assert torch.allclose(out2, expected2)
+
+
+def test_drop_connect():
+    """ "Tests that dropconnect works correctly for any number of dimensions"""
+    drop_connect = modules.residual.DropConnect(0.5)
+    inp1d = torch.rand(2, 10, 16)
+    inp3d = torch.rand(2, 10, 16, 16, 16)
+    assert drop_connect(INP).shape == INP.shape
+    assert drop_connect(inp1d).shape == inp1d.shape
+    assert drop_connect(inp3d).shape == inp3d.shape
+
+
+def test_fused_vgg():
+    """Test that Fused and not Fused version of VGG block are equal"""
+    orig = modules.residual.RepVGGBlock(4, 6, act=torch.nn.SELU, alpha=0.1, n_heads=3)
+    fused = modules.residual.FusedRepVGGBlock(4, 6, act=torch.nn.SELU)
+    fused.load_state_dict(orig.state_dict())
+    inp = torch.randn(1, 4, 3, 3)
+    orig_out = orig(inp)
+    fused_out = fused(inp)
+    assert torch.allclose(orig_out, fused_out, atol=1e-6)
+
+
+@pytest.mark.skip  # currently not working for some reason
+def test_xca_module():
+    """make sure that version that works on images and version that works on token are identical"""
+    BS = 2
+    DIM = 128
+    SIZE = 7
+    inp = torch.rand(BS, SIZE**2, DIM)
+    inp_img = inp.transpose(1, 2).reshape(BS, DIM, SIZE, SIZE)
+    xca_timm = modules.residual.XCA_Token(DIM, num_heads=4)
+    xca_my = modules.residual.XCA(DIM, num_heads=4, qkv_bias=False)
+
+    # load weights from Linear layer to conv1x1 layer
+    xca_my.load_state_dict(xca_timm.state_dict())
+
+    # make sure results are identical
+    out_timm = xca_timm(inp)
+    out_my = xca_my(inp_img)
+    out_timm_reshaped = out_timm.transpose(1, 2).reshape(BS, DIM, SIZE, SIZE)
+    assert torch.allclose(out_timm_reshaped, out_my, atol=1e-5)
+
+
+def test_sesr_convs():
+    expansion = 5
+    sesr_e = pt.modules.conv.SESRBlockExpanded(INP.size(1), expansion)
+    sesr_c = pt.modules.conv.SESRBlockCollapsed(INP.size(1), expansion)
+    sesr_c.load_state_dict(sesr_e.state_dict())
+    assert torch.allclose(sesr_e(INP), sesr_c(INP), atol=1e-6)
```

### Comparing `pytorch_tools-0.1.9/tests/models/test_models.py` & `pytorch_tools-0.5.1/tests/models/test_models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import torch
 import pytest
 import numpy as np
 import pytorch_tools as pt
 import pytorch_tools.models as models
 
 ALL_MODEL_NAMES = sorted(
-    name
-    for name in models.__dict__
-    if name.islower() and not name.startswith("_") and callable(models.__dict__[name])
+    name for name in models.__dict__ if name.islower() and not name.startswith("_") and callable(models.__dict__[name])
 )
 
 DENSENET_NAMES = [name for name in ALL_MODEL_NAMES if "dense" in name]
 
 EFFNET_NAMES = [name for name in ALL_MODEL_NAMES if "efficient" in name]
 
 VGG_NAMES = [name for name in ALL_MODEL_NAMES if "vgg" in name]
@@ -20,20 +18,15 @@
 
 TRESNET_NAMES = [name for name in ALL_MODEL_NAMES if "tresne" in name]
 
 HRNET_NAMES = [name for name in ALL_MODEL_NAMES if "hrnet" in name]
 
 # test only part of the models
 TEST_MODEL_NAMES = (
-    DENSENET_NAMES[:1]
-    + EFFNET_NAMES[:1]
-    + VGG_NAMES[:1]
-    + RESNET_NAMES[:1]
-    + TRESNET_NAMES[:1]
-    + HRNET_NAMES[:1]
+    DENSENET_NAMES[:1] + EFFNET_NAMES[:1] + VGG_NAMES[:1] + RESNET_NAMES[:1] + TRESNET_NAMES[:1] + HRNET_NAMES[:1]
 )
 # TEST_MODEL_NAMES = HRNET_NAMES[:1]
 INP = torch.ones(2, 3, 128, 128)
 
 
 def _test_forward(model):
     with torch.no_grad():
```

### Comparing `pytorch_tools-0.1.9/tests/models/test_weights.py` & `pytorch_tools-0.5.1/tests/models/test_weights.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,15 @@
 from PIL import Image
 
 from pytorch_tools.utils.preprocessing import get_preprocessing_fn
 from pytorch_tools.utils.visualization import tensor_from_rgb_image
 import pytorch_tools.models as models
 
 MODEL_NAMES = sorted(
-    name
-    for name in models.__dict__
-    if name.islower() and not name.startswith("__") and callable(models.__dict__[name])
+    name for name in models.__dict__ if name.islower() and not name.startswith("__") and callable(models.__dict__[name])
 )
 
 # tests are made to be run from root project directory
 # format "imagenet_image_class: PIL Image"
 IMGS = {
     560: Image.open("tests/imgs/helmet.jpeg"),
     207: Image.open("tests/imgs/dog.jpg"),
```

### Comparing `pytorch_tools-0.1.9/tests/utils/test_box_utils.py` & `pytorch_tools-0.5.1/tests/utils/test_box_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,23 +161,33 @@
             [ -4,  -4, 28, 28],
             [  4, -20, 20, 44],
             [-20,   4, 44, 20],
         ]
     ).float()
     # fmt: on
     generated, num_anchors = pt.utils.box.generate_anchors_boxes(
-        16, num_scales=1, aspect_ratios=(1, 0.25, 4), pyramid_levels=[3,]
+        16,
+        num_scales=1,
+        aspect_ratios=(1, 0.25, 4),
+        pyramid_levels=[
+            3,
+        ],
     )
     assert torch.allclose(expected, generated)
     assert num_anchors == 3
 
     # check that it is scriptable
     jit_generate = torch.jit.script(pt.utils.box.generate_anchors_boxes)
     generated, num_anchors = jit_generate(
-        (16, 16), num_scales=1, aspect_ratios=(1, 0.25, 4), pyramid_levels=[3,]
+        (16, 16),
+        num_scales=1,
+        aspect_ratios=(1, 0.25, 4),
+        pyramid_levels=[
+            3,
+        ],
     )
     assert torch.allclose(expected, generated)
     assert num_anchors == 3
 
 
 def test_box_iou():
     """Make sure IoU is calculated correctly"""
```

### Comparing `pytorch_tools-0.1.9/tests/losses/test_losses.py` & `pytorch_tools-0.5.1/tests/losses/test_losses.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 https://github.com/BloodAxe/pytorch-toolbelt/
 """
 
 set_random_seed(42)
 
 EPS = 1e-3
 BS = 16
-N_CLASSES = 10
+N_CLASSES = 7
 IM_SIZE = 10
 INP = torch.randn(BS, N_CLASSES)
 INP_BINARY = torch.randn(BS).float()
 INP_IMG = torch.rand(BS, N_CLASSES, IM_SIZE, IM_SIZE)
 INP_IMG_BINARY = torch.rand(BS, 1, IM_SIZE, IM_SIZE)
 
 TARGET = torch.randint(0, N_CLASSES, (BS,)).long()
@@ -36,14 +36,15 @@
 TARGET_IMG_MULTILABEL.scatter_(1, TARGET_IMG_MULTICLASS.unsqueeze(1), 1.0)
 
 LOSSES_NAMES = sorted(name for name in losses.__dict__ if not name.islower())
 
 # this tests are slow. it's usefull to sometimes remove them.
 LOSSES_NAMES.pop(LOSSES_NAMES.index("ContentLoss"))
 LOSSES_NAMES.pop(LOSSES_NAMES.index("StyleLoss"))
+LOSSES_NAMES.pop(LOSSES_NAMES.index("AdaCos"))
 
 ## Tests for Focal loss
 def test_focal_loss_fn_basic():
     """explicit tests for values in two corner cases"""
     input_good = torch.Tensor([10, -10, 10]).float()
     input_bad = torch.Tensor([-1, 2, 0]).float()
     target = torch.Tensor([1, 0, 1])
@@ -112,29 +113,32 @@
 
 
 def test_focal_incorrect_mode():
     with pytest.raises(ValueError):
         losses.FocalLoss(mode="some_mode")
 
 
-def test_focal_incorrect_reduction():
-    with pytest.raises(ValueError):
-        losses.FocalLoss(reduction="some_reduction")
+# as of 12.11.21 reduction is validated only during forward, so this test doesn't work
+# def test_focal_incorrect_reduction():
+#     with pytest.raises(ValueError):
+#         losses.FocalLoss(reduction="some_reduction")
 
 
+@pytest.mark.skip(reason="no time to fix enum in class on 06.10.21")
 def test_focal_fn_is_scribtable():
     """check that script gives the same results"""
     input_bad = torch.Tensor([-1, 2, 0]).float()
     target = torch.Tensor([1, 0, 1])
     loss = pt_F.focal_loss_with_logits(input_bad, target)
     jit_func = torch.jit.script(pt_F.focal_loss_with_logits)
     loss_jit = jit_func(input_bad, target)
     assert torch.allclose(loss, loss_jit)
 
 
+@pytest.mark.skip(reason="no time to fix enum in class on 06.10.21")
 def test_focal_class_is_scribtable():
     """check that script gives the same results"""
     input_bad = torch.Tensor([-1, 2, 0]).float()
     target = torch.Tensor([1, 0, 1])
     loss = losses.FocalLoss()(input_bad, target)
     jit_class = torch.jit.script(losses.FocalLoss())
     loss_jit = jit_class(input_bad, target)
@@ -180,14 +184,15 @@
 def test_soft_jaccard_score_2(y_true, y_pred, expected):
     y_true = torch.tensor(y_true, dtype=torch.float32)
     y_pred = torch.tensor(y_pred, dtype=torch.float32)
     actual = pt_F.soft_jaccard_score(y_pred, y_true, dims=[1])
     actual = actual.mean()
     assert float(actual) == pytest.approx(expected, abs=EPS)
 
+
 # fmt: off
 @pytest.mark.parametrize(
     ["y_true", "y_pred", "expected"],
     [
         [[1, 1, 1, 1], [1, 1, 1, 1], 1.0],
         [[0, 1, 1, 0], [0, 1, 1, 0], 1.0],
         [[1, 1, 1, 1], [1, 1, 0, 0], 2.0 / 3.0],
@@ -324,14 +329,25 @@
     y_pred = torch.tensor([[[0.0, 1.0, 1.0, 0.0], [0.0, 1.0, 1.0, 0.0]]])
     y_true = torch.tensor([[[1.0, 1.0, 0.0, 0.0], [1.0, 1.0, 0.0, 0.0]]])
 
     loss = criterion(y_pred, y_true)
     assert float(loss) == pytest.approx(1.0 - 1.0 / 3.0, abs=EPS)
 
 
+@torch.no_grad()
+def test_multilabel_jaccard_loss_reduction():
+    criterion = losses.JaccardLoss(mode="multilabel", reduction="none", from_logits=False, eps=1e-4)
+
+    y_pred = torch.tensor([[[0.0, 1.0, 0.0, 0.0], [0.0, 1.0, 1.0, 0.0]]])
+    y_true = torch.tensor([[[1.0, 1.0, 0.0, 0.0], [1.0, 1.0, 0.0, 0.0]]])
+
+    loss = criterion(y_pred, y_true)
+    assert torch.allclose(loss, torch.tensor([1 / 2, 2 / 3]), atol=EPS)
+
+
 @pytest.mark.parametrize("loss_name", LOSSES_NAMES)
 def test_correct_inheritance(loss_name):
     """test that all models are inherited from our custom loss"""
     assert issubclass(losses.__dict__[loss_name], losses.base.Loss)
 
 
 @pytest.mark.parametrize("loss_name", LOSSES_NAMES)
@@ -383,14 +399,18 @@
 def test_binary_cross_entropy(reduction):
     # classification test
     torch_ce = F.binary_cross_entropy_with_logits(INP_BINARY, TARGET_BINARY, reduction=reduction)
     my_ce_loss = losses.CrossEntropyLoss(mode="binary", reduction=reduction)
     my_ce = my_ce_loss(INP_BINARY, TARGET_BINARY)
     assert torch.allclose(torch_ce, my_ce)
 
+    # test than long targets would also work
+    my_ce = my_ce_loss(INP_BINARY, TARGET_BINARY.long())
+    assert torch.allclose(torch_ce, my_ce)
+
     # test for images
     torch_ce = F.binary_cross_entropy_with_logits(INP_IMG_BINARY, TARGET_IMG_BINARY, reduction=reduction)
     my_ce = my_ce_loss(INP_IMG_BINARY, TARGET_IMG_BINARY)
     assert torch.allclose(torch_ce, my_ce)
 
     my_ce = my_ce_loss(INP_IMG_BINARY.squeeze(), TARGET_IMG_BINARY.squeeze())
     assert torch.allclose(torch_ce.squeeze(), my_ce.squeeze())
@@ -439,14 +459,29 @@
 
     my_ce_w = losses.CrossEntropyLoss(weight=weight_2)(INP, TARGET)
     assert torch.allclose(torch_ce_w, my_ce_w)
 
     my_ce_w = losses.CrossEntropyLoss(weight=weight_3)(INP, TARGET)
     assert torch.allclose(torch_ce_w, my_ce_w)
 
+    # test 2d case
+    torch2d_ce_w = torch.nn.CrossEntropyLoss(weight=weight_1)(INP_IMG, TARGET_IMG_MULTICLASS)
+    my2d_ce_w = losses.CrossEntropyLoss(weight=weight_1)(INP_IMG, TARGET_IMG_MULTILABEL)
+    assert torch.allclose(torch2d_ce_w, my2d_ce_w)
+
+
+@torch.no_grad()
+@pytest.mark.parametrize("reduction", ["mean", "none"])
+def test_cross_entropy_reduction(reduction):
+    torch_ce = F.cross_entropy(INP_IMG, TARGET_IMG_MULTICLASS, reduction=reduction)
+    my_ce_loss = losses.CrossEntropyLoss(mode="multiclass", reduction=reduction)
+    # using multilabel in our loss because in current implementation it wouldn't perform OHE
+    my_ce = my_ce_loss(INP_IMG, TARGET_IMG_MULTILABEL)
+    assert torch.allclose(torch_ce, my_ce)
+
 
 # For lovasz tests only check that it doesn't fail, not that results are right
 
 
 def test_binary_lovasz():
     loss = losses.LovaszLoss(mode="binary")(INP_IMG_BINARY, TARGET_IMG_BINARY)
     # try other target shape
@@ -459,45 +494,48 @@
     loss = losses.LovaszLoss(mode="multiclass")(INP_IMG, TARGET_IMG_MULTICLASS)
     loss2 = losses.LovaszLoss(mode="multilabel")(INP_IMG, TARGET_IMG_MULTILABEL)
     assert torch.allclose(loss, loss2)
 
 
 def test_binary_hinge():
     from sklearn.metrics import hinge_loss
+
     my_l = losses.BinaryHinge()(INP_IMG_BINARY, TARGET_IMG_BINARY)
     sk_l = hinge_loss(TARGET_IMG_BINARY.flatten() * 2 - 1, INP_IMG_BINARY.flatten())
     assert torch.allclose(my_l, torch.tensor(sk_l, dtype=torch.float32))
 
+
 @pytest.mark.parametrize("reduction", ["sum", "mean", "none"])
 def test_smoothl1(reduction):
     loss_my = losses.SmoothL1Loss(delta=1, reduction=reduction)(INP, TARGET_MULTILABEL)
     loss_torch = F.smooth_l1_loss(INP, TARGET_MULTILABEL, reduction=reduction)
     assert torch.allclose(loss_my, loss_torch)
     # check that delta = 0 turns it into l1
     loss_my = losses.SmoothL1Loss(delta=0, reduction=reduction)(INP, TARGET_MULTILABEL)
     loss_torch = F.l1_loss(INP, TARGET_MULTILABEL, reduction=reduction)
     assert torch.allclose(loss_my, loss_torch)
 
 
+@pytest.mark.skip(reason="no time to fix enum in class on 06.10.21")
 def test_detection_loss_is_scriptabble():
     # this is a piece of real target and box/cls outputs for COCO images
     # fmt:off
     target = torch.tensor([
         [[190., 114., 209., 170.,  0.], [  6., 134., 125., 210.,  0.]],
         [[  1.,  55., 469., 506.,  1.], [ -1.,  -1.,  -1.,  -1., -1.]],
         [[  3., 213., 324., 380.,  1.], [147., 109., 195., 183.,  1.]],
         [[123.,  74., 261., 230.,  1.], [126., 286., 149., 317.,  1.]],
         [[  1.,  45., 276., 422.,  0.], [  2., 223., 256., 506.,  0.]]
     ])
     anchors = torch.tensor([
-        [-12.0000, -12.0000,  20.0000,  20.0000], 
+        [-12.0000, -12.0000,  20.0000,  20.0000],
         [-18.6274,  -7.3137,  26.6274,  15.3137]
     ])
     cls_out = torch.tensor([
-        [[-3.4645, -4.9549], [-6.3456, -7.3695]], 
+        [[-3.4645, -4.9549], [-6.3456, -7.3695]],
         [[-4.7375, -5.5270], [-5.4755, -6.7083]],
         [[-3.7339, -4.7242], [-6.2671, -6.8925]],
         [[-3.6217, -4.7811], [-5.6993, -6.7674]],
         [[-5.2376, -6.1608], [-6.1039, -7.0789]]
     ])
     box_out = torch.tensor([
         [[-0.0600,  6.1500, -21.8200,   0.2200], [ 0.0800,  0.0400,  -1.1300,  -1.4700]],
@@ -511,33 +549,34 @@
     loss = losses.DetectionLoss(anchors=anchors)
     loss_jit = torch.jit.script(loss)
     res = loss((cls_out, box_out), target)
     res_jit = loss_jit((cls_out, box_out), target)
     assert torch.allclose(res, res_jit)
     assert torch.allclose(res, torch.tensor(5e-07))
 
+
 # tests for KLD are from @alexeykarnachev
 # https://gist.github.com/alexeykarnachev/6829d8b208585582bc9c79ad1ed8bb45
 def test_binary_kld_loss():
     # ==================================================================================================================
     # [1] Test an ordinal KLD loss:
     x_logits = torch.tensor([[2.28, 4.20]])
     x_softmax = torch.softmax(x_logits, 1)  # => [[0.1279, 0.8721]]
     x_log_softmax = torch.log_softmax(x_logits, 1)
 
     y_p_0 = torch.tensor([[0.1279, 0.8721]])
-    kld_loss_0 = nn.KLDivLoss(reduction='batchmean')(x_log_softmax, y_p_0)
+    kld_loss_0 = nn.KLDivLoss(reduction="batchmean")(x_log_softmax, y_p_0)
     assert torch.allclose(kld_loss_0, torch.tensor([0.0]), atol=1e-3)
 
     y_p_1 = torch.tensor([[0.0, 1.0]])
-    kld_loss_1 = nn.KLDivLoss(reduction='batchmean')(x_log_softmax, y_p_1)
+    kld_loss_1 = nn.KLDivLoss(reduction="batchmean")(x_log_softmax, y_p_1)
     assert torch.allclose(kld_loss_1, torch.tensor([0.1368]), atol=1e-3)
 
     y_p_2 = torch.tensor([[0.1, 0.9]])
-    kld_loss_2 = nn.KLDivLoss(reduction='batchmean')(x_log_softmax, y_p_2)
+    kld_loss_2 = nn.KLDivLoss(reduction="batchmean")(x_log_softmax, y_p_2)
     assert torch.allclose(kld_loss_2, torch.tensor([0.0037]), atol=1e-3)
 
     # ==================================================================================================================
     # [2] Compare with BCESoftLoss (with Bernoulli inputs):
     x_p_bernoulli = x_softmax[:, 1:]
     y_p_0_bernoulli = y_p_0[:, 1:]
     bce_soft_loss_0 = losses.BinaryKLDivLoss(from_logits=False)(x_p_bernoulli, y_p_0_bernoulli)
@@ -556,9 +595,9 @@
     y_p_1_bernoulli = y_p_1[:, 1:]
     bce_soft_loss_1 = losses.BinaryKLDivLoss(from_logits=False)(x_p_bernoulli, y_p_1_bernoulli)
     bce_loss_1 = nn.BCELoss()(x_p_bernoulli, y_p_1_bernoulli)
     assert torch.allclose(bce_soft_loss_1, bce_loss_1, atol=1e-3)
 
     # ==================================================================================================================
     # [4] Check, that torch KLDivLoss for log-bernoulli input is the WRONG approach:
-    kld_loss_2_bernoulli = nn.KLDivLoss(reduction='batchmean')(torch.log(x_p_bernoulli), y_p_2_bernoulli)
+    kld_loss_2_bernoulli = nn.KLDivLoss(reduction="batchmean")(torch.log(x_p_bernoulli), y_p_2_bernoulli)
     assert not torch.allclose(kld_loss_2, kld_loss_2_bernoulli, atol=1e-3)
```

### Comparing `pytorch_tools-0.1.9/tests/tta_wrapper/test_tta.py` & `pytorch_tools-0.5.1/tests/tta_wrapper/test_tta.py`

 * *Files 9% similar despite different names*

```diff
@@ -104,9 +104,18 @@
     assert (inp - tta_m(inp)).mean() < 1e-6
 
 
 @pytest.mark.parametrize("merge", ["mean", "max", "gmean"])
 def test_wrapper_cls(merge):
     m = SumAll()
     inp = INPUT / 15.0  # make sure max is less that 1 to avoid overflow
-    tta_m = TTA(m, segm=False, h_flip=True, v_flip=True, h_shift=1, v_shift=-1, rotation=90, merge=merge,)
+    tta_m = TTA(
+        m,
+        segm=False,
+        h_flip=True,
+        v_flip=True,
+        h_shift=1,
+        v_shift=-1,
+        rotation=90,
+        merge=merge,
+    )
     assert tta_m(inp).allclose(torch.Tensor([8.0]))
```

### Comparing `pytorch_tools-0.1.9/tests/detection_models/test_det_models.py` & `pytorch_tools-0.5.1/tests/detection_models/test_det_models.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/imgs/cityscapes_sample.jpg` & `pytorch_tools-0.5.1/tests/imgs/cityscapes_sample.jpg`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/imgs/helmet.jpeg` & `pytorch_tools-0.5.1/tests/imgs/helmet.jpeg`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/imgs/dog.jpg` & `pytorch_tools-0.5.1/tests/imgs/dog.jpg`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/imgs/cityscapes_sample2.jpg` & `pytorch_tools-0.5.1/tests/imgs/cityscapes_sample2.jpg`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/benchmarking/memory_test.py` & `pytorch_tools-0.5.1/tests/benchmarking/memory_test.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import time
 import torch
 import pytest
 import argparse
 import numpy as np
-from apex import amp
+
+# from apex import amp
 import torchvision as tv
 import torch.backends.cudnn as cudnn
 
 import pytorch_tools as pt
 from pytorch_tools import models
 import pytorch_tools.segmentation_models as pt_sm
 
@@ -88,15 +89,15 @@
             RUN_ITERS,
             BS,
             SZ,
             f_times.mean(),
             f_times.std(),
             (fb_times - f_times).mean(),
             (fb_times - f_times).std(),
-            torch.cuda.max_memory_allocated(0) / 2 ** 20,
+            torch.cuda.max_memory_allocated(0) / 2**20,
             BS * 1000 / fb_times.mean(),
         )
     )
     del optimizer
     del model
 
 
@@ -125,36 +126,37 @@
     parser = argparse.ArgumentParser("Model Benchmarking")
     parser.add_argument("--forward", "-f", action="store_true", help="Flag to only run forward. Disables grads")
     parser.add_argument("--amp", action="store_true", help="Measure speed using apex mixed precision")
     parser.add_argument("--print", action="store_true", help="Print model")
     parser.add_argument("--torch_amp", action="store_true", help="Measure speed using torch native mixed precision")
     parser.add_argument("--channels_last", action="store_true", help="Use channels last memory format")
     parser.add_argument(
-        "--bs", default=64, type=int, help="BS for benchmarking",
+        "--bs",
+        default=64,
+        type=int,
+        help="BS for benchmarking",
     )
     parser.add_argument(
-        "--sz", default=224, type=int, help="Size of images for benchmarking",
+        "--sz",
+        default=224,
+        type=int,
+        help="Size of images for benchmarking",
     )
     args = parser.parse_args()
     # all models are first init to cpu memory to find errors earlier
     # fmt: off
     models_dict = {
-        # "EffDet0 My": pt.detection_models.efficientdet_d0(match_tf_same_padding=False, pretrained=None),
-        "RetinaNet My": pt.detection_models.retinanet_r50_fpn(),
-
-        # "EffDet0 My Wrapped": DetectionTrainWrapper(
-        #     modell=pt.detection_models.efficientdet_d0(match_tf_same_padding=False, pretrained=None),
-        #     size=args.sz,
-        # ),
-        # "R50": pt.models.resnet50(),
+        "EffDet0 My": pt.detection_models.efficientdet_d0(match_tf_same_padding=False, pretrained=None),
+        "EffDet0 My Wrapped": DetectionTrainWrapper(
+            modell=pt.detection_models.efficientdet_d0(match_tf_same_padding=False, pretrained=None),
+            size=args.sz,
+        ),
+        "R50": pt.models.resnet50(),
         # "Simp_R50": pt.models.simpl_resnet50(),
-        # "R34": pt.models.resnet34(),
-        # "EfficientNet B0": pt.models.efficientnet_b0(norm_act="swish_naive"),
-        # "EfficientNet B3": pt.models.efficientnet_b3(norm_act="swish_naive"),
-        # "EfficientNet B5": pt.models.efficientnet_b5(norm_act="swish_naive"),
+        "R34": pt.models.resnet34(),
         # "R34 est": pt.models.resnet34(norm_layer="estimated_abn"),
         # "R34 abcn": pt.models.resnet34(norm_layer="abcn"),
         # "R34 est abcn": pt.models.resnet34(norm_layer="abcn_micro"),
         # "R34 agn": pt.models.resnet34(norm_layer="agn"),
         # "R34 SE 0.5": pt.models.resnet34(attn_type="se"),
         # "R34 ECA": pt.models.resnet34(attn_type="eca"),
         # "Simp_R34": pt.models.simpl_resnet34(),
@@ -237,15 +239,15 @@
         #         # "head_width": [1536, 2560],
         #         # "head_type": "mlp_2",
         #         # "head_width": [1024, 1536, 2560],
         #         # "head_type": "mlp_3",
         #         "head_norm_act": "swish_hard",
         #     }
         # )
-
+        # "Eff B0": pt.models.efficientnet_b0(),
         # "TR50": pt.models.tresnetm(norm_layer="abn"),
         # "D53 timm": timm.models.darknet53(),
         # "CSPD53 timm": timm.models.cspdarknet53(),
         # "CSPR50 timm": timm.models.cspresnet50(),
         # "CSPR50d timm": timm.models.cspresnet50d(),
         # "CSPX50 timm": timm.models.cspresnext50(),
         # "TRes ": pt.models.tresnetm(),
```

### Comparing `pytorch_tools-0.1.9/tests/benchmarking/benchmarking_example.py` & `pytorch_tools-0.5.1/tests/benchmarking/benchmarking_example.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,30 +5,30 @@
 
 # #### MEMORY ####
 def consume_gpu_ram(n):
     return torch.ones((n, n)).cuda(0)
 
 
 def consume_gpu_ram_256mb():
-    return consume_gpu_ram(2 ** 13)
+    return consume_gpu_ram(2**13)
 
 
 # should be 1024 peak, 0 used
 z = [consume_gpu_ram_256mb() for i in range(4)]  # 1GB
 del z
-print("Peak memory: {}Mb".format(torch.cuda.max_memory_allocated(0) / 2 ** 10 / 2 ** 10))
-print("Current memory: {}Mb".format(torch.cuda.memory_allocated(0) / 2 ** 10 / 2 ** 10))
+print("Peak memory: {}Mb".format(torch.cuda.max_memory_allocated(0) / 2**10 / 2**10))
+print("Current memory: {}Mb".format(torch.cuda.memory_allocated(0) / 2**10 / 2**10))
 torch.cuda.reset_max_memory_allocated()
 
 # should be: 512 peaked, 256 used
 c1 = consume_gpu_ram_256mb()
 c2 = consume_gpu_ram_256mb()
 del c1
-print("Peak memory: {}Mb".format(torch.cuda.max_memory_allocated(0) / 2 ** 10 / 2 ** 10))
-print("Current memory: {}Mb".format(torch.cuda.memory_allocated(0) / 2 ** 10 / 2 ** 10))
+print("Peak memory: {}Mb".format(torch.cuda.max_memory_allocated(0) / 2**10 / 2**10))
+print("Current memory: {}Mb".format(torch.cuda.memory_allocated(0) / 2**10 / 2**10))
 torch.backends.cudnn.benchmark = False
 #### SPEED ####
 x = torch.ones((8, 3, 32, 32), requires_grad=True).cuda(0)
 conv = torch.nn.Conv2d(3, 64, 5).cuda(0)
 start = torch.cuda.Event(enable_timing=True)
 end = torch.cuda.Event(enable_timing=True)
 start.record()
```

### Comparing `pytorch_tools-0.1.9/tests/benchmarking/README.md` & `pytorch_tools-0.5.1/tests/benchmarking/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,72 +1,72 @@
 # Speed comparison of different models and their memory usage
 
-**VGG 16 ABN:**  
-Mean of 10 runs 50 iters each BS=128: 719.29+-1.45 msecs gpu. Max memory: 17732.86Mb  
-**VGG 16 InplaceABN:**  
+**VGG 16 ABN:**
+Mean of 10 runs 50 iters each BS=128: 719.29+-1.45 msecs gpu. Max memory: 17732.86Mb
+**VGG 16 InplaceABN:**
 Mean of 10 runs 50 iters each BS=128: 727.05+-0.73 msecs gpu. Max memory: 11857.39Mb
 
-**VGG 16 Naive PostAct:**  
-Mean of 10 runs 10 iters each BS=128: 652.89+-0.98 msecs gpu. Max memory: 17585.80Mb  
-**VGG 16 Chpnt PostAct:**  
+**VGG 16 Naive PostAct:**
+Mean of 10 runs 10 iters each BS=128: 652.89+-0.98 msecs gpu. Max memory: 17585.80Mb
+**VGG 16 Chpnt PostAct:**
 Mean of 10 runs 10 iters each BS=128: 847.33+-10.08 msecs gpu. Max memory: 13423.22Mb
 
-**VGG 16 Naive PreAct:**  
-Mean of 10 runs 10 iters each BS=128: 641.53+-1.29 msecs gpu. Max memory: 17585.80Mb  
-**VGG 16 Chpnt PreAct:**  
+**VGG 16 Naive PreAct:**
+Mean of 10 runs 10 iters each BS=128: 641.53+-1.29 msecs gpu. Max memory: 17585.80Mb
+**VGG 16 Chpnt PreAct:**
 Mean of 10 runs 10 iters each BS=128: 841.74+-12.48 msecs gpu. Max memory: 13423.22Mb
 
-**Resnet50 ABN:**  
-Mean of 10 runs 50 iters each BS=128: 447.21+-0.61 msecs gpu. Max memory: 10884.15Mb  
-**Resnet50 InplaceABN:**  
+**Resnet50 ABN:**
+Mean of 10 runs 50 iters each BS=128: 447.21+-0.61 msecs gpu. Max memory: 10884.15Mb
+**Resnet50 InplaceABN:**
 Mean of 10 runs 50 iters each BS=128: 479.64+-1.32 msecs gpu. Max memory: 8888.33Mb
 
-**SE Resnext50_32x4 ABN:**  
-Mean of 10 runs 50 iters each BS=128: 700.99+-0.67 msecs gpu. Max memory: 16826.77Mb  
-**SE Resnext50_32x4 InplaceABN:**  
+**SE Resnext50_32x4 ABN:**
+Mean of 10 runs 50 iters each BS=128: 700.99+-0.67 msecs gpu. Max memory: 16826.77Mb
+**SE Resnext50_32x4 InplaceABN:**
 Mean of 10 runs 50 iters each BS=128: 718.09+-2.18 msecs gpu. Max memory: 10575.54Mb
 
-**SE Resnext50_32x4 ABN:**  
-Mean of 10 runs 10 iters each BS=64: 394.58+-0.41 msecs gpu. Max memory: 8607.16Mb  
-**SE Resnext50_32x4 InplaceABN:**  
+**SE Resnext50_32x4 ABN:**
+Mean of 10 runs 10 iters each BS=64: 394.58+-0.41 msecs gpu. Max memory: 8607.16Mb
+**SE Resnext50_32x4 InplaceABN:**
 Mean of 10 runs 10 iters each BS=64: 410.02+-3.24 msecs gpu. Max memory: 5470.71Mb
 
-**EffNet B0 rwightman 5.29M params**  
-Mean of 10 runs 10 iters each BS=64: 27.15+-0.03 msecs Forward. 117.22+-3.62 msecs Backward. Max memory: 5491.36Mb  
-**EffNet B1 rwightman 7.79M params**  
-Mean of 10 runs 10 iters each BS=64: 39.05+-0.02 msecs Forward. 151.09+-3.33 msecs Backward. Max memory: 7680.92Mb  
-**EffNet B2 rwightman 9.11M params**  
-Mean of 10 runs 10 iters each BS=64: 41.30+-0.05 msecs Forward. 148.15+-2.87 msecs Backward. Max memory: 8064.01Mb  
-**EffNet B3 rwightman 12.23M params**  
-Mean of 10 runs 10 iters each BS=64: 53.73+-0.02 msecs Forward. 192.05+-2.13 msecs Backward. Max memory: 10675.62Mb  
-
-
-**EffNet B1 rwightman CUDA Swish 7.79M params**  
-Mean of 10 runs 10 iters each BS=64: 38.65+-0.01 msecs Forward. 145.76+-3.77 msecs Backward. Max memory: 7741.70Mb  
-**EffNet B1 rwightman RELU 7.79M params**  
-Mean of 10 runs 10 iters each BS=64: 38.50+-0.01 msecs Forward. 150.01+-4.07 msecs Backward. Max memory: 5767.71Mb  
-
-
-**EffNet B0 lukemelas 5.29M params**  
-Mean of 10 runs 10 iters each BS=64: 38.59+-0.01 msecs Forward. 141.19+-4.33 msecs Backward. Max memory: 5980.59Mb  
-**EffNet B1 lukemelas 7.79M params**  
-Mean of 10 runs 10 iters each BS=64: 54.97+-0.01 msecs Forward. 185.83+-5.13 msecs Backward. Max memory: 8254.66Mb  
+**EffNet B0 rwightman 5.29M params**
+Mean of 10 runs 10 iters each BS=64: 27.15+-0.03 msecs Forward. 117.22+-3.62 msecs Backward. Max memory: 5491.36Mb
+**EffNet B1 rwightman 7.79M params**
+Mean of 10 runs 10 iters each BS=64: 39.05+-0.02 msecs Forward. 151.09+-3.33 msecs Backward. Max memory: 7680.92Mb
+**EffNet B2 rwightman 9.11M params**
+Mean of 10 runs 10 iters each BS=64: 41.30+-0.05 msecs Forward. 148.15+-2.87 msecs Backward. Max memory: 8064.01Mb
+**EffNet B3 rwightman 12.23M params**
+Mean of 10 runs 10 iters each BS=64: 53.73+-0.02 msecs Forward. 192.05+-2.13 msecs Backward. Max memory: 10675.62Mb
+
+
+**EffNet B1 rwightman CUDA Swish 7.79M params**
+Mean of 10 runs 10 iters each BS=64: 38.65+-0.01 msecs Forward. 145.76+-3.77 msecs Backward. Max memory: 7741.70Mb
+**EffNet B1 rwightman RELU 7.79M params**
+Mean of 10 runs 10 iters each BS=64: 38.50+-0.01 msecs Forward. 150.01+-4.07 msecs Backward. Max memory: 5767.71Mb
+
+
+**EffNet B0 lukemelas 5.29M params**
+Mean of 10 runs 10 iters each BS=64: 38.59+-0.01 msecs Forward. 141.19+-4.33 msecs Backward. Max memory: 5980.59Mb
+**EffNet B1 lukemelas 7.79M params**
+Mean of 10 runs 10 iters each BS=64: 54.97+-0.01 msecs Forward. 185.83+-5.13 msecs Backward. Max memory: 8254.66Mb
 
-**Resnet50 Baseline: 25.56M params**  
-Mean of 10 runs 10 iters each BS=64: 59.65+-0.07 msecs Forward. 164.39+-2.58 msecs Backward. Max memory: 5935.15Mb  
+**Resnet50 Baseline: 25.56M params**
+Mean of 10 runs 10 iters each BS=64: 59.65+-0.07 msecs Forward. 164.39+-2.58 msecs Backward. Max memory: 5935.15Mb
 
 **Resnet50 AMP** 25.56M params
 Mean of 10 runs 10 iters each BS=256: 111.44+-0.03 msecs Forward. 357.80+-1.61 msecs Backward. Max memory: 11226.14Mb. 545.56 imgs/sec
 
-**Resnet34 Leaky ReLU 21.82M params**  
-Mean of 10 runs 10 iters each BS=64: 30.81+-0.18 msecs Forward. 103.95+-1.05 msecs Backward. Max memory: 2766.59Mb  
-**Resnet34 ReLU 21.82M params**  
-Mean of 10 runs 10 iters each BS=64: 30.76+-0.01 msecs Forward. 103.90+-1.10 msecs Backward. Max memory: 2932.52Mb  
-**Resnet34 Mish 21.82M params**  
-Mean of 10 runs 10 iters each BS=64: 35.07+-0.02 msecs Forward. 112.40+-4.26 msecs Backward. Max memory: 3739.84Mb  
-**Resnet34 Mish Naive 21.82M params**  
-Mean of 10 runs 10 iters each BS=64: 37.73+-0.01 msecs Forward. 125.56+-5.10 msecs Backward. Max memory: 5846.58Mb  
+**Resnet34 Leaky ReLU 21.82M params**
+Mean of 10 runs 10 iters each BS=64: 30.81+-0.18 msecs Forward. 103.95+-1.05 msecs Backward. Max memory: 2766.59Mb
+**Resnet34 ReLU 21.82M params**
+Mean of 10 runs 10 iters each BS=64: 30.76+-0.01 msecs Forward. 103.90+-1.10 msecs Backward. Max memory: 2932.52Mb
+**Resnet34 Mish 21.82M params**
+Mean of 10 runs 10 iters each BS=64: 35.07+-0.02 msecs Forward. 112.40+-4.26 msecs Backward. Max memory: 3739.84Mb
+**Resnet34 Mish Naive 21.82M params**
+Mean of 10 runs 10 iters each BS=64: 37.73+-0.01 msecs Forward. 125.56+-5.10 msecs Backward. Max memory: 5846.58Mb
 
 
 ## Methodology
 
 Check `benchmarking_example.py` for an example of how to measure speed and memory usage. NOTE: Memory usage reported by pytorch doesn't include memory used by internal CUDA libraries which also has to be loaded to device. It means that more memory is actually used than reported by this tests. But the number of additional memory is always constant for the same device.
```

### Comparing `pytorch_tools-0.1.9/tests/metrics/test_metric.py` & `pytorch_tools-0.5.1/tests/metrics/test_metric.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/tests/segmentation_models/test_segm_models.py` & `pytorch_tools-0.5.1/tests/segmentation_models/test_segm_models.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/spatial_ocr_block.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/spatial_ocr_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from pytorch_tools.modules import ABN
 from pytorch_tools.modules.residual import conv1x1
 
 
 class SpatialOCR_Gather(nn.Module):
     """Aggregate the context features according to the initial predicted probability distribution.
        Employ the soft-weighted method to aggregate the context.
-    Input: 
+    Input:
         torch.Tensor (B x C_2 x H x W), torch.Tensor (B x C_1 x H x W)
     Returns:
         torch.Tensor (B x C_2 x C_1 x 1)
     """
 
     def forward(self, feats, probs):
         # C_1 is number of final classes. C_2 in number of features in `feats`
@@ -76,22 +76,25 @@
         self.f_object = nn.Sequential(
             conv1x1(in_channels, key_channels, bias=True),
             norm_layer(key_channels, activation=norm_act),
             conv1x1(key_channels, key_channels, bias=True),
             norm_layer(key_channels, activation=norm_act),
         )
         self.f_down = nn.Sequential(
-            conv1x1(in_channels, key_channels, bias=True), norm_layer(key_channels, activation=norm_act),
+            conv1x1(in_channels, key_channels, bias=True),
+            norm_layer(key_channels, activation=norm_act),
         )
         self.f_up = nn.Sequential(
-            conv1x1(key_channels, in_channels, bias=True), norm_layer(in_channels, activation=norm_act),
+            conv1x1(key_channels, in_channels, bias=True),
+            norm_layer(in_channels, activation=norm_act),
         )
 
         self.conv_bn = nn.Sequential(
-            conv1x1(2 * in_channels, out_channels, bias=True), norm_layer(out_channels, activation=norm_act),
+            conv1x1(2 * in_channels, out_channels, bias=True),
+            norm_layer(out_channels, activation=norm_act),
         )
 
     def forward(self, feats, proxy_feats):
         # feats B x 512 x H //4 x W//4
         # proxy feats B x 512 x num_classes (19) x 1
         batch_size = feats.size(0)
         # C = num classes; 512 = in_channels; 256 = key_channels
@@ -102,15 +105,15 @@
         key = self.f_object(proxy_feats).view(batch_size, self.key_channels, -1)
         # value.shape = B x 512 x C x 1 => B x 256 x C x 1 => B x C x 256
         value = self.f_down(proxy_feats).view(batch_size, self.key_channels, -1)
         value = value.permute(0, 2, 1)
 
         # sim_map.shape = B x H*W//16 x 256 @ B x 256 x C => B x H*W//16 x C
         sim_map = torch.matmul(query, key)
-        sim_map = (self.key_channels ** -0.5) * sim_map
+        sim_map = (self.key_channels**-0.5) * sim_map
         sim_map = sim_map.softmax(dim=-1)
 
         # add bg context ...
         # context.shape = B x H*W//16 x C @ B x C x 256 => B x H*W//16 x 256
         context = torch.matmul(sim_map, value)
         # B x H*W//16 x 256 => B x 256 x H*W//16 => ... => B x 256 x H//4 x W//4
         context = context.permute(0, 2, 1).contiguous()
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/weight_standartization.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/weight_standartization.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/activated_batch_norm.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/activated_batch_norm.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
         momentum (float): Momentum factor applied to compute running statistics.
         affine (bool): If `True` apply learned scale and shift transformation after normalization.
         activation (str): Name of the activation functions, one of: `relu`, `leaky_relu`, `elu` or `identity`.
         activation_param (float): Negative slope for the `leaky_relu` activation.
         frozen (bool): if True turns `weight` and `bias` into untrainable buffers.
         estimated_stats (bool): Flag to use running stats for normalization instead of batch stats. Useful for
             micro-batch training. See Ref.
-    
+
     Reference:
         https://arxiv.org/abs/1911.09738 - Rethinking Normalization and Elimination Singularity in Neural Networks
     """
 
     def __init__(
         self,
         num_features,
@@ -70,15 +70,22 @@
             nn.init.constant_(self.bias, 0)
 
     def forward(self, x):
         # in F.batch_norm `training` regulates whether to use batch stats of buffer stats
         # if `training` is True and buffers are given, they always would be updated!
         use_batch_stats = self.training and not self.estimated_stats and not self.frozen
         x = F.batch_norm(
-            x, self.running_mean, self.running_var, self.weight, self.bias, use_batch_stats, self.momentum, self.eps,
+            x,
+            self.running_mean,
+            self.running_var,
+            self.weight,
+            self.bias,
+            use_batch_stats,
+            self.momentum,
+            self.eps,
         )
         if self.training and self.estimated_stats:
             with torch.no_grad():  # not sure if needed but just in case
                 # PyTorch BN uses biased var by default
                 var, mean = torch.var_mean(x, dim=(0, 2, 3), unbiased=False)
                 self.running_mean = self.running_mean.mul(1 - self.momentum).add(mean, alpha=self.momentum)
                 self.running_var = self.running_var.mul(1 - self.momentum).add(var, alpha=self.momentum)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/bifpn.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/bifpn.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
         return self.act(sum(features))
 
 
 class BiFPNLayer(nn.Module):
     """Builds one layer of Bi-directional Feature Pyramid Network
     Args:
         channels (int): Number of channels in each feature map after BiFPN. Defaults to 64.
-        
+
     Input:
         features (List): 5 feature maps from encoder with resolution from 1/128 to 1/8
 
     Returns:
         p_out: features processed by 1 layer of BiFPN
     """
 
@@ -61,17 +61,15 @@
         self.num_features = num_features
 
         # disable attention for large models. This is a very dirty way to check that it's B6 & B7. But i don't care
         Fusion = SumFusion if channels > 288 else FastNormalizedFusion
 
         # There is no activation in SeparableConvs, instead activation is in fusion layer
         # fusions for p6, p5, p4, p3. (no fusion for first feature map)
-        self.fuse_up = nn.ModuleList(
-            [Fusion(in_nodes=2, activation=norm_act) for _ in range(num_features - 1)]
-        )
+        self.fuse_up = nn.ModuleList([Fusion(in_nodes=2, activation=norm_act) for _ in range(num_features - 1)])
 
         # fusions for p4, p5, p6, p7. last is different because there is no bottop up tensor for it
         self.fuse_out = nn.ModuleList(
             [
                 *(Fusion(in_nodes=3, activation=norm_act) for _ in range(num_features - 2)),
                 Fusion(in_nodes=2, activation=norm_act),
             ]
@@ -129,30 +127,32 @@
         # pretrained weights for them were ~1e-5 which additionally shows that they are not needed
         self.downsample_1 = nn.ModuleList()
         self.downsample_2 = []
         for enc_in_channel in encoder_channels:
             layer, layer2 = nn.Identity(), nn.Identity()
             if enc_in_channel != channels:
                 layer = nn.Sequential(
-                    conv1x1(enc_in_channel, channels), norm_layer(channels, activation="identity"),
+                    conv1x1(enc_in_channel, channels),
+                    norm_layer(channels, activation="identity"),
                 )
                 layer2 = nn.Sequential(
-                    conv1x1(enc_in_channel, channels), norm_layer(channels, activation="identity"),
+                    conv1x1(enc_in_channel, channels),
+                    norm_layer(channels, activation="identity"),
                 )
             self.downsample_1.append(layer)
             self.downsample_2.append(layer2)
         # no second downsample for last feature map (highest res)
         self.downsample_2[-1] = nn.Identity()
         # [::-1] for proper weight order.
         self.downsample_2 = nn.ModuleList(self.downsample_2[::-1])
 
     def forward(self, features):
         # type: List[Tensor] -> List[Tensor]
         """Args:
-            features (List[Tensor]): number of input features should match number of encoder_channels passed during init
+        features (List[Tensor]): number of input features should match number of encoder_channels passed during init
         """
         features_in_1 = [down(feat) for down, feat in zip(self.downsample_1, features)]
         features_in_2 = [down(feat) for down, feat in zip(self.downsample_2[::-1], features)]
 
         # below is copy from BiFPNLayer with features changed to features_in_1 / features_in_2
 
         # p7_in, p6_in, p5_in, p4_in, p3_in = features
@@ -185,15 +185,15 @@
     """
     Implementation of Bi-directional Feature Pyramid Network
 
     Args:
         encoder_channels (List[int]): Number of channels for each feature map from low res to high res.
         pyramid_channels (int): Number of channels in each feature map after BiFPN. Defaults to 64.
         num_layers (int): Number or repeats for BiFPN block. Default is 2
-    
+
     Input:
         features (List): 5 feature maps from encoder [low_res, ... , high_res]
 
     https://arxiv.org/pdf/1911.09070.pdf
     """
 
     def __init__(self, encoder_channels, pyramid_channels=64, num_layers=1, **bn_args):
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/fpn.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/fpn.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         return x
 
 
 class FPN(nn.Module):
     """Feature Pyramid Network for enhancing high-resolution feature maps with semantic
     meaning from low resolution maps
     Ref: https://arxiv.org/abs/1612.03144
-        
+
     Args:
         encoder_channels (List[int]): Number of channels for each input feature map
         pyramid_channels (int): Number of channels in each feature map after FPN. Defaults to 256.
         num_layers (int): Number of FPN layers.
     Input:
         features (List): this module expects list of feature maps of different resolution
     """
@@ -33,17 +33,15 @@
         num_layers=1,
         **bn_args,  # for compatability only. Not used
     ):
         super().__init__()
         assert num_layers == 1, "More that 1 layer is not supported in FPN"
 
         # we DO use bias in this convs
-        self.lateral_convs = nn.ModuleList(
-            [conv1x1(in_ch, pyramid_channels, bias=True) for in_ch in encoder_channels]
-        )
+        self.lateral_convs = nn.ModuleList([conv1x1(in_ch, pyramid_channels, bias=True) for in_ch in encoder_channels])
         self.smooth_convs = nn.ModuleList(
             [conv3x3(pyramid_channels, pyramid_channels, bias=True) for in_ch in encoder_channels]
         )
         self.merge_block = MergeBlock()
 
     def forward(self, features):
         """features (List[torch.Tensor]): features from coarsest to finest"""
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/pooling.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/pooling.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 def global_catavgmax_pool2d(x):
     x_avg = F.adaptive_avg_pool2d(x, output_size=1)
     x_max = F.adaptive_max_pool2d(x, output_size=1)
     return torch.cat((x_avg, x_max), 1)
 
 
 def global_pool2d(x, pool_type):
-    """Selectable global pooling function
-    """
+    """Selectable global pooling function"""
     if pool_type == "avg":
         x = F.adaptive_avg_pool2d(x, output_size=1)
     elif pool_type == "max":
         x = F.adaptive_max_pool2d(x, output_size=1)
     elif pool_type == "avgmax":
         x = global_avgmax_pool2d(x)
     elif pool_type == "catavgmax":
@@ -40,17 +39,17 @@
 
     def forward(self, input):
         return input.view(input.size(0), -1)
 
 
 class GlobalPool2d(nn.Module):
     """Selectable global pooling layer
-    
-        Args:
-            pool_type (str): One of 'avg', 'max', 'avgmax', 'catavgmax'
+
+    Args:
+        pool_type (str): One of 'avg', 'max', 'avgmax', 'catavgmax'
     """
 
     def __init__(self, pool_type):
 
         super(GlobalPool2d, self).__init__()
         self.pool_type = pool_type
         self.pool = partial(global_pool2d, pool_type=pool_type)
@@ -70,44 +69,49 @@
     def __init__(self, flatten=False):
         super(FastGlobalAvgPool2d, self).__init__()
         self.flatten = flatten
 
     def forward(self, x):
         return x.mean(dim=(2, 3), keepdim=not self.flatten)
 
+    def extra_repr(self):
+        return f"flatten={self.flatten}"
+
 
 class BlurPool(nn.Module):
     """
     Idea from https://arxiv.org/abs/1904.11486
     Efficient implementation of Rect-3
     Args:
         channels (int): numbers of input channels. needed to construct gauss kernel
     """
 
-    def __init__(self, channels=0):
+    def __init__(self, channels=0, trainable=False):
         super(BlurPool, self).__init__()
         self.channels = channels
         filt = torch.tensor([1.0, 2.0, 1.0])
         filt = filt[:, None] * filt[None, :]
         filt = filt / torch.sum(filt)
         filt = filt[None, None, :, :].repeat((self.channels, 1, 1, 1))
-        self.register_buffer("filt", filt)
+        if trainable:
+            self.register_parameter("filt", torch.nn.Parameter(filt))
+        else:
+            self.register_buffer("filt", filt)
 
     def forward(self, inp):
         return F.conv2d(inp, self.filt, stride=2, padding=1, groups=inp.shape[1])
 
     def extra_repr(self):
         return f"channels={self.channels}"
 
 
 # from https://github.com/mrT23/TResNet/
 class SpaceToDepth(nn.Module):
     def __init__(self, block_size=4):
         super().__init__()
-        assert block_size in {2, 4}, "Space2Depth only supports blocks size = 4 or 2"
         self.block_size = block_size
 
     def forward(self, x):
         N, C, H, W = x.size()
         S = self.block_size
         x = x.view(N, C, H // S, S, W // S, S)  # (N, C, H//bs, bs, W//bs, bs)
         x = x.permute(0, 3, 5, 1, 2, 4).contiguous()  # (N, bs, bs, C, H//bs, W//bs)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/residual.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/residual.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,24 @@
 import math
 import torch
 import torch.nn as nn
 from functools import partial
+
 from .activated_batch_norm import ABN
 from .activations import activation_from_name
+from .conv import conv3x3, conv1x1
 
 # from pytorch_tools.modules import ABN
 # from pytorch_tools.modules import activation_from_name
 from pytorch_tools.modules import BlurPool
 from pytorch_tools.modules import FastGlobalAvgPool2d
 from pytorch_tools.utils.misc import make_divisible
 from pytorch_tools.modules import SpaceToDepth
 
 
-def conv3x3(in_planes, out_planes, stride=1, groups=1, dilation=1, bias=False):
-    """3x3 convolution with padding"""
-    return nn.Conv2d(
-        in_planes,
-        out_planes,
-        kernel_size=3,
-        stride=stride,
-        padding=dilation,
-        groups=groups,
-        bias=bias,
-        dilation=dilation,
-    )
-
-
-def conv1x1(in_planes, out_planes, stride=1, bias=False):
-    """1x1 convolution"""
-    return nn.Conv2d(in_planes, out_planes, kernel_size=1, stride=stride, bias=bias)
-
-
 class SEModule(nn.Module):
     def __init__(self, channels, reduction_channels, norm_act="relu"):
         super(SEModule, self).__init__()
 
         self.pool = FastGlobalAvgPool2d()
         # authors of original paper DO use bias
         self.fc1 = conv1x1(channels, reduction_channels, bias=True)
@@ -45,25 +28,28 @@
     def forward(self, x):
         x_se = self.pool(x)
         x_se = self.fc1(x_se)
         x_se = self.act1(x_se)
         x_se = self.fc2(x_se)
         return x * x_se.sigmoid()
 
+
 class SEVar3(nn.Module):
     """Variant of SE module from ECA paper (see above) which doesn't have dimensionality reduction"""
+
     def __init__(self, channels, *args):
         super().__init__()
 
         self.pool = FastGlobalAvgPool2d()
         # authors of original paper DO use bias
         self.fc1 = conv1x1(channels, channels, bias=True)
 
     def forward(self, x):
-        return x * self.fc1(self.pool(x))
+        return x * self.fc1(self.pool(x)).sigmoid()
+
 
 class ECAModule(nn.Module):
     """Efficient Channel Attention
     This implementation is different from the paper. I've removed all hyperparameters and
     use fixed kernel size of 3. If you think it may be better to use different k_size - feel free to open an issue.
     upd. 12.01.2020 increase kernel size
 
@@ -117,136 +103,143 @@
         self.sse = SSEModule(in_ch)
         self.cse = ECAModule()
         self.reduction_conv = conv1x1(in_ch * 2, in_ch, bias=True)  # use bias because there is no BN after
 
     def forward(self, x):
         return self.reduction_conv(torch.cat([self.sse(x), self.cse(x)], dim=1))
 
+
 class MSCAMModule(nn.Module):
     """Idea from Attentional Feature Fusion (MS-CAM)
     Combines global and local attention in a better manner than scSE
     """
 
-    def __init__(self, in_ch, reduced_ch, norm_layer=ABN, norm_act="relu"): # parse additional args for compatability
+    def __init__(self, in_ch, reduced_ch, norm_layer=ABN, norm_act="relu"):  # parse additional args for compatability
         super().__init__()
         self.global_attn = nn.Sequential(
             FastGlobalAvgPool2d(),
             conv1x1(in_ch, reduced_ch),
             norm_layer(reduced_ch, activation=norm_act),
             conv1x1(reduced_ch, in_ch),
-            norm_layer(in_ch, activation="identity"), # no last activation
+            norm_layer(in_ch, activation="identity"),  # no last activation
         )
-        # this 
+        # this
         self.local_attn = nn.Sequential(
             conv1x1(in_ch, reduced_ch),
             norm_layer(reduced_ch, activation=norm_act),
             conv1x1(reduced_ch, in_ch),
-            norm_layer(in_ch, activation="identity"), # no last activation
+            norm_layer(in_ch, activation="identity"),  # no last activation
         )
-        
+
     def forward(self, x):
         xl = self.local_attn(x)
         xg = self.global_attn(x)
         return x * (xl + xg).sigmoid()
 
+
 class FCAAttn(nn.Module):
     """Inspired by FcaNet: Frequency Channel Attention Networks (https://arxiv.org/pdf/2012.11879.pdf)
-    
+
     But I view it as positional encoding and multiply be a predefined set of filters
     """
+
     def __init__(self, channels, reduction_channels, norm_act="relu"):
 
         super().__init__()
 
-        self.pool = FastGlobalAvgPool2d()
+        # self.pool = FastGlobalAvgPool2d()
         # authors of original paper DO use bias
         self.fc = nn.Sequential(
             conv1x1(channels, reduction_channels, bias=True),
             activation_from_name(norm_act),
             conv1x1(reduction_channels, channels, bias=True),
             nn.Sigmoid(),
         )
         # dummy shape. would be overwritten later. not registering as buffer intentionally
-        self.pos_encoding = torch.ones(1, 1, 1, 1) 
+        self.pos_encoding = torch.ones(1, 1, 1, 1)
 
     def _get_pos_encoding(self, inp):
         """Want this to be generated for each input size separately"""
         self.pos_encoding = torch.ones_like(inp)
         c_part = inp.size(1) // 4
         xx = torch.linspace(0, math.pi, inp.size(3)).cos()[None].repeat(inp.size(2), 1)
         yy = torch.linspace(0, math.pi, inp.size(2)).cos()[None].repeat(inp.size(3), 1).T
         xy = torch.linspace(-math.pi, math.pi, inp.size(3)).cos().neg().repeat(inp.size(2), 1)
-        self.pos_encoding[:, c_part * 1:c_part * 2] = xx
-        self.pos_encoding[:, c_part * 2:c_part * 3] = yy
-        self.pos_encoding[:, c_part * 3:c_part * 4] = xy
+        self.pos_encoding[:, c_part * 1 : c_part * 2] = xx
+        self.pos_encoding[:, c_part * 2 : c_part * 3] = yy
+        self.pos_encoding[:, c_part * 3 : c_part * 4] = xy
         return self.pos_encoding
 
     def forward(self, x):
         if x.shape != self.pos_encoding.shape:
             self._get_pos_encoding(x)
-        x_se = self.fc(self.pool(x * self.pos_encoding))
+        x_se = (x * self.pos_encoding).sum(dim=(2, 3), keepdim=True)
+        x_se = self.fc(x_se)
         return x * x_se
 
+
 class FCA_ECA_Attn(nn.Module):
     """Inspired by FcaNet: Frequency Channel Attention Networks (https://arxiv.org/pdf/2012.11879.pdf)
-    
+
     But I view it as positional encoding and multiply be a predefined set of filters
     This class uses Efficient Channel Attention instead of SE
     """
+
     def __init__(self, *args, kernel_size=3, **kwargs):
         super().__init__()
         self.pool = FastGlobalAvgPool2d()
         self.conv = nn.Conv1d(1, 1, kernel_size=kernel_size, padding=kernel_size // 2, bias=False)
         # dummy shape. would be overwritten later. not registering as buffer intentionally
-        self.pos_encoding = torch.ones(1, 1, 1, 1) 
+        self.pos_encoding = torch.ones(1, 1, 1, 1)
 
     def _get_pos_encoding(self, inp):
         """Want this to be generated for each input size separately"""
         self.pos_encoding = torch.ones_like(inp)
         c_part = inp.size(1) // 4
         xx = torch.linspace(0, math.pi, inp.size(3)).cos()[None].repeat(inp.size(2), 1)
         yy = torch.linspace(0, math.pi, inp.size(2)).cos()[None].repeat(inp.size(3), 1).T
         xy = torch.linspace(-math.pi, math.pi, inp.size(3)).cos().neg().repeat(inp.size(2), 1)
-        self.pos_encoding[:, c_part * 1:c_part * 2] = xx
-        self.pos_encoding[:, c_part * 2:c_part * 3] = yy
-        self.pos_encoding[:, c_part * 3:c_part * 4] = xy
+        self.pos_encoding[:, c_part * 1 : c_part * 2] = xx
+        self.pos_encoding[:, c_part * 2 : c_part * 3] = yy
+        self.pos_encoding[:, c_part * 3 : c_part * 4] = xy
         return self.pos_encoding
 
     def forward(self, x):
         # FCA part
         if x.shape != self.pos_encoding.shape:
             self._get_pos_encoding(x)
         # ECA part
         x_s = self.pool(x * self.pos_encoding)
         x_s = self.conv(x_s.view(x.size(0), 1, -1))
         x_s = x_s.view(x.size(0), -1, 1, 1).sigmoid()
         return x * x_s.expand_as(x)
 
+
 class MyAttn(nn.Module):
     """Idea from Attentional Feature Fusion (MS-CAM)
     Combines global and local attention in a better manner than scSE
     """
 
-    def __init__(self, in_ch, reduced_ch, norm_layer=ABN, norm_act="relu"): # parse additional args for compatability
+    def __init__(self, in_ch, reduced_ch, norm_layer=ABN, norm_act="relu"):  # parse additional args for compatability
         super().__init__()
         self.global_attn = nn.Sequential(
             FastGlobalAvgPool2d(),
             conv1x1(in_ch, reduced_ch),
             norm_layer(reduced_ch, activation=norm_act),
             conv1x1(reduced_ch, in_ch),
-            norm_layer(in_ch, activation="identity"), # no last activation
+            norm_layer(in_ch, activation="identity"),  # no last activation
         )
-        # this 
+        # this
         self.local_attn = nn.Sequential(
             conv1x1(in_ch, reduced_ch),
             norm_layer(reduced_ch, activation=norm_act),
             conv1x1(reduced_ch, in_ch),
-            norm_layer(in_ch, activation="identity"), # no last activation
+            norm_layer(in_ch, activation="identity"),  # no last activation
         )
-        
+
     def forward(self, x):
         xl = self.local_attn(x)
         xg = self.global_attn(x)
         return x * (xl + xg).sigmoid()
 
 
 def get_attn(attn_type):
@@ -266,16 +259,18 @@
         "eca9": partial(ECAModule, kernel_size=9),
         "sse": SSEModule,
         "scse": SCSEModule,
         "se-var3": SEVar3,
         "ms-cam": MSCAMModule,
         "fca": FCAAttn,
         "fca-eca": FCA_ECA_Attn,
+        "xca": XCA,
+        "esa": ESA,
     }
-        
+
     if attn_type is None:
         return nn.Identity
     else:
         return ATT_TO_MODULE[attn_type.lower()]
 
 
 class DepthwiseSeparableConv(nn.Sequential):
@@ -355,17 +350,16 @@
     def __init__(self, keep_prob):
         super().__init__()
         self.keep_prob = keep_prob
 
     def forward(self, x):
         if not self.training:
             return x
-        batch_size = x.size(0)
         random_tensor = self.keep_prob
-        random_tensor += torch.rand([batch_size, 1, 1, 1], dtype=x.dtype, device=x.device)
+        random_tensor += torch.rand((x.size(0),) + (1,) * (x.dim() - 1), dtype=x.dtype, device=x.device)
         binary_tensor = torch.floor(random_tensor)
         output = x / self.keep_prob * binary_tensor
         return output
 
     def extra_repr(self):
         return f"keep_prob={self.keep_prob:.2f}"
 
@@ -572,15 +566,21 @@
 
 class CSPDarkBasicBlock(nn.Module):
     """Idea from https://github.com/WongKinYiu/CrossStagePartialNetworks
     But implementaion is different. This block divides input into two passes only one part through bottleneck
     """
 
     def __init__(
-        self, in_channels, out_channels, attn_type=None, norm_layer=ABN, norm_act="leaky_relu", keep_prob=1,
+        self,
+        in_channels,
+        out_channels,
+        attn_type=None,
+        norm_layer=ABN,
+        norm_act="leaky_relu",
+        keep_prob=1,
     ):
         super().__init__()
         mid_channels = int(in_channels * bottle_ratio)
         self.conv1 = conv1x1(in_channels, mid_channels)
         self.bn1 = norm_layer(mid_channels, activation=norm_act)
         self.conv2 = conv3x3(mid_channels, out_channels)
         # In original DarkNet they have activation after second BN but the most recent papers
@@ -867,21 +867,24 @@
                 BlurPool(channels=mid_chs) if antialias else nn.Identity(),
                 norm_layer(mid_chs, activation=norm_act),
                 conv3x3(mid_chs, out_chs),
             )
         else:
             self.bn1 = norm_layer(in_chs, activation=norm_act)
             self.block_1 = nn.Sequential(
-                conv3x3(in_chs // 4, in_chs // 4), norm_layer(in_chs // 4, activation=norm_act),
+                conv3x3(in_chs // 4, in_chs // 4),
+                norm_layer(in_chs // 4, activation=norm_act),
             )
             self.block_2 = nn.Sequential(
-                conv3x3(in_chs // 4, in_chs // 4), norm_layer(in_chs // 4, activation=norm_act),
+                conv3x3(in_chs // 4, in_chs // 4),
+                norm_layer(in_chs // 4, activation=norm_act),
             )
             self.block_3 = nn.Sequential(
-                conv3x3(in_chs // 4, in_chs // 4), norm_layer(in_chs // 4, activation=norm_act),
+                conv3x3(in_chs // 4, in_chs // 4),
+                norm_layer(in_chs // 4, activation=norm_act),
             )
             self.last_conv = conv3x3(in_chs, out_chs)  # expand in last conv in block
 
     def forward(self, x):
         if self.stride == 2:
             return self.blocks(x)
         # split in 4
@@ -913,15 +916,21 @@
         super().__init__()
         self.has_residual = in_chs == out_chs and stride == 1
         if in_chs != mid_chs:
             self.expansion = nn.Sequential(conv1x1(in_chs, mid_chs), norm_layer(mid_chs, activation=norm_act))
         else:
             self.expansion = nn.Identity()
         self.conv_dw = nn.Conv2d(
-            mid_chs, mid_chs, dw_kernel_size, stride=stride, groups=mid_chs, bias=False, padding=dw_kernel_size // 2,
+            mid_chs,
+            mid_chs,
+            dw_kernel_size,
+            stride=stride,
+            groups=mid_chs,
+            bias=False,
+            padding=dw_kernel_size // 2,
         )
         self.bn2 = norm_layer(mid_chs, activation=norm_act)
         # some models like MobileNet use mid_chs here instead of in_channels. But I don't care for now
         self.se = get_attn(attn_type)(mid_chs, in_chs // 4, norm_act)
         self.conv_pw1 = conv1x1(mid_chs, out_chs)
         self.bn3 = norm_layer(out_chs, activation="identity")
         self.drop_connect = DropConnect(keep_prob) if keep_prob < 1 else nn.Identity()
@@ -967,15 +976,21 @@
         if in_chs != mid_chs or force_expansion:
             self.expansion = nn.Sequential(norm_layer(in_chs, activation=norm_act), conv1x1(in_chs, mid_chs))
         else:
             self.expansion = nn.Identity()
         self.bn2 = norm_layer(mid_chs, activation=norm_act)
         dw_kernel_size = dw_str2_kernel_size if stride == 2 else dw_kernel_size
         self.conv_dw = nn.Conv2d(
-            mid_chs, mid_chs, dw_kernel_size, stride=stride, groups=mid_chs, bias=False, padding=dw_kernel_size // 2,
+            mid_chs,
+            mid_chs,
+            dw_kernel_size,
+            stride=stride,
+            groups=mid_chs,
+            bias=False,
+            padding=dw_kernel_size // 2,
         )
         # some models like MobileNet use mid_chs here instead of in_channels. But I don't care for now
         self.se = get_attn(attn_type)(mid_chs, in_chs // 4, norm_act)
         self.bn3 = norm_layer(mid_chs, activation=norm_act)  # Note it's NOT identity for PreAct
         self.conv_pw1 = conv1x1(mid_chs, out_chs)
         self.drop_connect = DropConnect(keep_prob) if keep_prob < 1 else nn.Identity()
 
@@ -1018,15 +1033,21 @@
         self.in_chs = in_chs
 
         self.pw1 = nn.Sequential(norm_layer(in_chs, activation=norm_act), conv1x1(in_chs, mid_chs))
         self.pw2 = nn.Sequential(norm_layer(mid_chs, activation=norm_act), conv1x1(mid_chs, out_chs))
 
         dw_kernel_size = dw_str2_kernel_size if stride == 2 else dw_kernel_size
         conv_dw = nn.Conv2d(
-            out_chs, out_chs, dw_kernel_size, stride=stride, groups=out_chs, bias=False, padding=dw_kernel_size // 2,
+            out_chs,
+            out_chs,
+            dw_kernel_size,
+            stride=stride,
+            groups=out_chs,
+            bias=False,
+            padding=dw_kernel_size // 2,
         )
         self.dw = nn.Sequential(norm_layer(out_chs, activation=norm_act), conv_dw)
 
         self.se = get_attn(attn_type)(mid_chs, in_chs // 4, norm_act)
         self.drop_connect = DropConnect(keep_prob) if keep_prob < 1 else nn.Identity()
 
     def forward(self, x):
@@ -1171,16 +1192,16 @@
     Args:
         in_channels (int): input channels for this stage
         out_channels (int): output channels for this stage
         num_blocks (int): number of residual blocks in stage
         stride (int): stride for first convolution
         bottle_ratio (float): how much channels are reduced inside blocks
         antialias (bool): flag to apply gaussiian smoothing before conv with stride 2
-    
-    Ref: TODO: add 
+
+    Ref: TODO: add
 
     """
 
     def __init__(
         self,
         in_chs,
         out_chs,
@@ -1259,7 +1280,232 @@
             x1, x2, x3, x4 = torch.chunk(x, chunks=4, dim=1)
             x2 = torch.cat([x2, x3, x4], dim=1)
         x2 = self.blocks(x2)
         x2 = self.x2_transition(x2)
         out = torch.cat([x1, x2], dim=1)
         # no explicit transition here. first conv in the next stage would perform transition
         return out
+
+
+class RepVGGBlock(nn.Module):
+    """
+    This block is inspired by [1] and [2]. The idea is to have `n_heads` parallel branches of convolutions which are then summed + residual
+    For performance they are implemented as one conv3x3. I removed normalization by making sure this block is variance preserving
+    RepVGGBlock(act=Identity)( N(0, 1)) ~= N(0, 1)
+
+    NOTE: this block requires correct initialization of conv weighs to work. Highly recommended to use with ConvWS
+    NOTE: for some reasons SELU activation still causes increase in variance. The possible solution is to use gain = 0.5 in ConvWS instead of 1
+
+    For inference this block could be replaced with `FusedRepVGGBlock` for significant speed-up
+
+    Args:
+        in_chs (int):
+            number of input channels
+        out_chs (int):
+            number of output channels. if out_chs > in_chs performs partial residual
+        n_heads (int):
+            number of parallel branches
+        act (nn.Module):
+            activation to use. recommended is nn.SELU
+        alpha (float):
+            parameter for skip init, balancing signal between block and residual path. output would be
+            x * (1 - alpha) + sum[conv3x3_i(x) * alpha], for i in range(n_heads)
+        trainable_alpha (bool):
+            if True make alpha a parameter, else it's un-trainable buffer
+            having trainable alpha may be beneficial. Timm repo says it could bring noticeable
+            slowdown for training. need to investigate
+
+    Ref:
+        [1] RepVGG: Making VGG-style ConvNets Great Again
+        [2] High-Performance Large-Scale Image Recognition Without Normalization
+    """
+
+    def __init__(self, in_chs, out_chs, n_heads=2, act=nn.SELU, alpha=0.2, trainable_alpha=False):
+        super().__init__()
+        self.in_chs = in_chs
+        self.out_chs = out_chs
+        self.n_heads = n_heads
+
+        assert 0 <= alpha <= 1
+
+        self.conv = nn.Conv2d(in_chs, out_chs * n_heads, kernel_size=3, padding=1)
+
+        # it's important to carefully initialize alpha so that this block is variance preserving
+        branch_alpha = torch.ones(1, out_chs, 1, 1) * (alpha / n_heads) ** 0.5
+        # take care of extra features without residual (they appear if out_chs > in_chs)
+        branch_alpha[:, in_chs:] = (1 / n_heads) ** 0.5
+        residual_alpha = torch.tensor((1 - alpha) ** 0.5)
+
+        if trainable_alpha:
+            self.register_parameter("skipinit_res", nn.Parameter(residual_alpha))
+            self.register_parameter("skipinit_branch", nn.Parameter(branch_alpha))
+        else:
+            self.register_buffer("skipinit_res", residual_alpha)
+            self.register_buffer("skipinit_branch", branch_alpha)
+
+        self.activation = act()
+
+    def forward(self, x):
+        proj = self.conv(x)
+        # same as out = reduce(lambda x, y: torch.chunk(out, self.n_heads, 1)) but faster
+        proj = proj.view(proj.size(0), self.n_heads, proj.size(1) // self.n_heads, proj.size(2), proj.size(3))
+        branch_res = proj.sum(1)
+        res = x * self.skipinit_res
+        if self.in_chs == self.out_chs:
+            branch_res = branch_res * self.skipinit_branch
+            branch_res += res
+        else:
+            branch_res = branch_res * self.skipinit_branch
+            branch_res[:, : self.in_chs] += res
+        out = self.activation(branch_res)
+        return out
+
+    def extra_repr(self):
+        return f"num_heads={self.n_heads}"
+
+
+class FusedRepVGGBlock(nn.Sequential):
+    def __init__(self, in_chs, out_chs, act=nn.SELU):
+        super().__init__()
+        self.add_module("conv", nn.Conv2d(in_chs, out_chs, kernel_size=3, padding=1))
+        self.add_module("activation", act())
+
+    def load_state_dict(self, state_dict):
+        if state_dict.get("skipinit_res", None) is None:
+            super().load_state_dict(state_dict)
+
+        self_w = self.conv.weight
+        self_b = self.conv.bias
+
+        kernel_id = torch.zeros_like(self_w)
+        kernel_id[: self_w.size(1), :, 1, 1] = torch.eye(self_w.size(1))
+        kernel_id *= state_dict["skipinit_res"]
+
+        kernel_conv = state_dict["conv.weight"].view(-1, *self_w.shape).sum(0)
+        bias_conv = state_dict["conv.bias"].view(-1, *self.conv.bias.shape).sum(0)
+
+        kernel_conv *= state_dict["skipinit_branch"].view(self_w.size(0), 1, 1, 1)
+        bias_conv *= state_dict["skipinit_branch"].flatten()
+
+        self.conv.weight.data = kernel_id + kernel_conv
+        self.conv.bias.data = bias_conv
+
+
+# modules from XCiT paper
+# XCA_Token is from timm, XCA is the same (convered by tests) but works direcly on B x C x H x W tensor
+class XCA_Token(nn.Module):
+    """Cross-Covariance Attention (XCA)
+    Operation where the channels are updated using a weighted sum. The weights are obtained from the (softmax
+    normalized) Cross-covariance matrix (Q^T \\cdot K \\in d_h \\times d_h)
+    """
+
+    def __init__(self, dim, num_heads=8, qkv_bias=False, attn_drop=0.0, proj_drop=0.0):
+        super().__init__()
+        self.num_heads = num_heads
+        self.temperature = nn.Parameter(torch.ones(num_heads, 1, 1))
+        self.qkv = nn.Linear(dim, dim * 3, bias=qkv_bias)
+        self.attn_drop = nn.Dropout(attn_drop)
+        self.proj = nn.Linear(dim, dim)
+        self.proj_drop = nn.Dropout(proj_drop)
+
+    def forward(self, x):
+        B, N, C = x.shape
+        # Result of next line is (qkv, B, num (H)eads,  (C')hannels per head, N)
+        qkv = self.qkv(x).reshape(B, N, 3, self.num_heads, C // self.num_heads).permute(2, 0, 3, 4, 1)
+        q, k, v = qkv[0], qkv[1], qkv[2]  # make torchscript happy (cannot use tensor as tuple)
+
+        # Paper section 3.2 l2-Normalization and temperature scaling
+        q = torch.nn.functional.normalize(q, dim=-1)
+        k = torch.nn.functional.normalize(k, dim=-1)
+        attn = (q @ k.transpose(-2, -1)) * self.temperature
+        attn = attn.softmax(dim=-1)
+        attn = self.attn_drop(attn)
+
+        # (B, H, C', N), permute -> (B, N, H, C')
+        x = (attn @ v).permute(0, 3, 1, 2).reshape(B, N, C)
+        x = self.proj(x)
+        x = self.proj_drop(x)
+        return x
+
+
+class XCA(nn.Module):
+    """Cross-Covariance Attention (XCA)
+    Operation where the channels are updated using a weighted sum. The weights are obtained from the (softmax
+    normalized) Cross-covariance matrix (Q^T \\cdot K \\in d_h \\times d_h)
+    This could be viewed as dynamic 1x1 convolution
+    """
+
+    def __init__(self, dim, num_heads=8, qkv_bias=True, attn_drop=0.0, proj_drop=0.0):
+        super().__init__()
+        self.num_heads = num_heads
+        self.temperature = nn.Parameter(torch.ones(num_heads, 1, 1))
+        self.qkv = conv1x1(dim, dim * 3, bias=qkv_bias)
+        self.attn_drop = nn.Dropout(attn_drop)
+        self.proj = conv1x1(dim, dim, bias=True)
+        self.proj_drop = nn.Dropout(proj_drop)
+
+    def forward(self, x):
+        B, C, H, W = x.shape
+        # C` == channels per head, Hd == num heads
+        # B x C x H x W -> B x 3*C x H x W -> B x 3 x Hd x C` x H*W -> 3 x B x Hd x C` x H*W
+        qkv = self.qkv(x).reshape(B, 3, self.num_heads, C // self.num_heads, -1).transpose(0, 1)
+        q, k, v = qkv[0], qkv[1], qkv[2]  # make torchscript happy
+
+        # Paper section 3.2 l2-Normalization and temperature scaling
+        q = torch.nn.functional.normalize(q, dim=-1)
+        k = torch.nn.functional.normalize(k, dim=-1)
+        # -> B x Hd x C` x C`
+        attn = (q @ k.transpose(-2, -1)) * self.temperature
+        attn = attn.softmax(dim=-1)
+        attn = self.attn_drop(attn)
+
+        # B x Hd x C` x C` @ B x Hd x C` x H*W -> B x C x H x W
+        x_out = (attn @ v).reshape(B, C, H, W)
+        x_out = self.proj(x_out)
+        x_out = self.proj_drop(x_out)
+        # in original paper there is no residual here
+        return x + x_out
+
+    def load_state_dict(self, state_dict):
+        # to allow loading from Linear layer
+        new_sd = {}
+        for k, v in state_dict.items():
+            if v.dim() == 2:
+                new_sd[k] = v[..., None, None]
+            else:
+                new_sd[k] = v
+        super().load_state_dict(new_sd)
+
+
+class ESA(nn.Module):
+    """
+    Efficient self-attention. Performs self-attention on channels after GAP to significantly reduce ammount of required compute
+    Close to SE-Var3 from ECA paper and XCA above
+
+    """
+
+    def __init__(self, dim, num_heads=8, qkv_bias=True, use_proj=True):
+        super().__init__()
+        self.num_heads = num_heads
+        self.pool = FastGlobalAvgPool2d()
+        self.qkv = conv1x1(dim, dim * 3, bias=qkv_bias)
+        self.temperature = nn.Parameter(torch.ones(num_heads, 1, 1))
+        self.proj = conv1x1(dim, dim, bias=True) if use_proj else nn.Identity()
+
+    def forward(self, x):
+        B, C = x.shape[:2]
+        # C` == channels per head, Hd == num heads
+        # B x C x H x W -> B x 3*C x 1 x 1 -> B x 3 x Hd x C` x 1 -> 3 x B x Hd x C` x 1
+        qkv = self.qkv(self.pool(x)).reshape(B, 3, self.num_heads, C // self.num_heads, -1).transpose(0, 1)
+        q, k, v = qkv[0], qkv[1], qkv[2]  # make torchscript happy
+
+        # Paper section 3.2 l2-Normalization and temperature scaling. BUT! scaling is for channels because we don't have enough tokens
+        q = torch.nn.functional.normalize(q, dim=-2)
+        k = torch.nn.functional.normalize(k, dim=-2)
+        # -> B x Hd x C` x C`
+        attn = (q @ k.transpose(-2, -1)) * self.temperature
+        attn = attn.softmax(dim=-1)
+
+        # B x Hd x C` x C` @ B x Hd x C` x 1 -> B x C x 1
+        x_out = (attn @ v).reshape(B, C, 1, 1)
+        x_out = self.proj(x_out)
+        return x + x_out.expand_as(x)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/activated_no_norm.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/activated_no_norm.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     This is just an activation wrapped in class to allow easy swaping with BN and GN
     Args:
         num_features (int): Not used. here for compatability
         activation (str): Name of the activation functions
         activation_param (float): Negative slope for the `leaky_relu` activation.
     """
 
-    def __init__(self, num_features, activation="relu", activation_param=0.01):
+    def __init__(self, num_features=-1, activation="relu", activation_param=0.01):
         super().__init__()
         self.num_features = num_features
         self.activation = ACT(activation)
         self.activation_param = activation_param
 
     def forward(self, x):
         func = ACT_FUNC_DICT[self.activation]
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/activated_batch_channel_norm.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/activated_batch_channel_norm.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 
 class ABCN(nn.Module):
     """Activated Batch Channel Normalization (BCN)
     This gathers a Batch Channel Normalization and an activation function in a single module
     BCN is basically a Batch Norm followed by Group Norm. In case of small batch size it's reccomended to use
     `estimated_stats` flag to force BN to use running statistics instead of batch
-    
+
     see Ref. for paper
 
     Args:
         num_features (int): Number of feature channels in the input and output.
         num_groups (int): Number of groups to separate the channels into for Group Norm
         eps (float): Small constant to prevent numerical issues.
         momentum (float): Momentum factor applied to compute running statistics.
@@ -69,15 +69,22 @@
         nn.init.constant_(self.bias_gn, 0)
 
     def forward(self, x):
         # in F.batch_norm `training` regulates whether to use batch stats of buffer stats
         # if `training` is True and buffers are given, they always would be updated!
         use_batch_stats = self.training and not self.estimated_stats
         x = F.batch_norm(
-            x, self.running_mean, self.running_var, self.weight, self.bias, use_batch_stats, self.momentum, self.eps,
+            x,
+            self.running_mean,
+            self.running_var,
+            self.weight,
+            self.bias,
+            use_batch_stats,
+            self.momentum,
+            self.eps,
         )
         if self.training and self.estimated_stats:
             with torch.no_grad():  # not sure if needed but just in case
                 # PyTorch BN uses biased var by default
                 var, mean = torch.var_mean(x, dim=(0, 2, 3), unbiased=False)
                 self.running_mean = self.running_mean.mul(1 - self.momentum).add(mean, alpha=self.momentum)
                 self.running_var = self.running_var.mul(1 - self.momentum).add(var, alpha=self.momentum)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/__init__.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,33 +15,34 @@
 
 # from .residual import Transition, DenseLayer
 from .weight_standartization import conv_to_ws_conv
 
 from .activations import ACT_DICT
 from .activations import ACT_FUNC_DICT
 from .activations import activation_from_name
-from .activations import Mish, MishNaive, Swish, SwishNaive
+from .activations import Mish, MishNaive
 
 from .activated_batch_norm import ABN
 from .activated_batch_norm import SyncABN
 from .activated_group_norm import AGN
 from .activated_batch_channel_norm import ABCN
 from .activated_no_norm import NoNormAct
 
+from . import conv
+
 try:
     from inplace_abn import InPlaceABN, InPlaceABNSync
 
     HAS_INPLACE_ABN = True
 except (ModuleNotFoundError, ImportError):
-    logger.warning("Inplace ABN is not installed. Using ABN by default")
     HAS_INPLACE_ABN = False
     InPlaceABN = ABN
     InPlaceABNSync = ABN
 
-# NOTE: after adding new normalization don't forget to also patch `filter_bn_from_wd` function
+
 def bn_from_name(norm_name):
     norm_name = norm_name.lower()
     if norm_name == "abn":
         return ABN
     elif norm_name in ("syncabn", "sync_abn", "abn_sync"):
         return SyncABN
     elif norm_name in ("inplaceabn", "inplace_abn") and HAS_INPLACE_ABN:
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/activated_group_norm.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/activated_group_norm.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,26 +7,32 @@
 from .activations import ACT
 from .activations import ACT_FUNC_DICT
 
 
 class AGN(nn.Module):
     """Activated Group Normalization
     This gathers a GroupNorm and an activation function in a single module
-    
+
     Args:
     num_features (int): Number of feature channels in the input and output.
     num_groups (int): Number of groups to separate the channels into
     eps (float): Small constant to prevent numerical issues.
     affine (bool): If `True` apply learned scale and shift transformation after normalization.
     activation (str): Name of the activation functions, one of: `relu`, `leaky_relu`, `elu` or `identity`.
     activation_param (float): Negative slope for the `leaky_relu` activation.
     """
 
     def __init__(
-        self, num_features, num_groups=32, eps=1e-5, affine=True, activation="relu", activation_param=0.01,
+        self,
+        num_features,
+        num_groups=32,
+        eps=1e-5,
+        affine=True,
+        activation="relu",
+        activation_param=0.01,
     ):
         super(AGN, self).__init__()
         self.num_features = num_features
         self.num_groups = num_groups
         self.affine = affine
         self.eps = eps
         self.activation = ACT(activation)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/decoder.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/decoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,17 +3,15 @@
 import torch.nn.functional as F
 from pytorch_tools.utils.misc import initialize
 from .activated_batch_norm import ABN
 from .residual import conv3x3, conv1x1, DepthwiseSeparableConv, get_attn
 
 
 class UnetDecoderBlock(nn.Module):
-    def __init__(
-        self, in_channels, out_channels, norm_layer=ABN, norm_act="relu", upsample=True, attn_type=None
-    ):
+    def __init__(self, in_channels, out_channels, norm_layer=ABN, norm_act="relu", upsample=True, attn_type=None):
         super(UnetDecoderBlock, self).__init__()
 
         conv1 = conv3x3(in_channels, out_channels)
         conv2 = conv3x3(out_channels, out_channels)
         abn1 = norm_layer(out_channels, activation=norm_act)
         abn2 = norm_layer(out_channels, activation=norm_act)
         self.block = nn.Sequential(conv1, abn1, conv2, abn2)
@@ -82,15 +80,16 @@
 
 class ASPP(nn.Module):
     def __init__(self, in_channels, atrous_rates, norm_layer=ABN, norm_act="relu"):
         super(ASPP, self).__init__()
         out_channels = 256
         norm_params = {"norm_layer": norm_layer, "norm_act": norm_act}
         self.conv0 = nn.Sequential(
-            conv1x1(in_channels, out_channels), norm_layer(out_channels, activation=norm_act),
+            conv1x1(in_channels, out_channels),
+            norm_layer(out_channels, activation=norm_act),
         )
         self.pool = ASPPPooling(in_channels, out_channels, **norm_params)
 
         self.project = nn.Sequential(
             nn.Conv2d(out_channels * 5, out_channels, 1, bias=False),
             norm_layer(out_channels, activation=norm_act),
             nn.Dropout(0.1),
@@ -128,15 +127,16 @@
         OUT_CHANNELS = 256
         super().__init__()
         norm_params = {"norm_layer": norm_layer, "norm_act": norm_act}
         if output_stride == 8:
             dilation_rates = [i * 2 for i in dilation_rates]
         self.aspp = ASPP(encoder_channels[0], dilation_rates, norm_layer, norm_act)
         self.conv0 = nn.Sequential(
-            conv3x3(OUT_CHANNELS, OUT_CHANNELS), norm_layer(OUT_CHANNELS, activation=norm_act),
+            conv3x3(OUT_CHANNELS, OUT_CHANNELS),
+            norm_layer(OUT_CHANNELS, activation=norm_act),
         )
         self.proj_conv = nn.Sequential(
             conv1x1(encoder_channels[3], PROJ_CONV_CHANNELS),
             norm_layer(PROJ_CONV_CHANNELS, activation=norm_act),
         )
 
         self.sep_conv1 = DepthwiseSeparableConv(OUT_CHANNELS + PROJ_CONV_CHANNELS, 256, **norm_params)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/modules/tf_same_ops.py` & `pytorch_tools-0.5.1/pytorch_tools/modules/tf_same_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,13 +79,15 @@
 
 
 def maxpool_to_same_maxpool(module):
     """Turn All MaxPool2d into SameMaxPool2d to match TF padding"""
     module_output = module
     if isinstance(module, nn.MaxPool2d):
         module_output = MaxPool2dSamePadding(
-            kernel_size=module.kernel_size, stride=module.stride, padding=0,  # explicitly set to 0
+            kernel_size=module.kernel_size,
+            stride=module.stride,
+            padding=0,  # explicitly set to 0
         )
     for name, child in module.named_children():
         module_output.add_module(name, maxpool_to_same_maxpool(child))
     del module
     return module_output
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/radam.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/radam.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/rmsprop.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/rmsprop.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 """Implementation of TF-like RMSprop with epsilong inside sqrt. The only difference is at line 52"""
 import torch
 from torch.optim import RMSprop as _RMSprop
 
+
 class RMSprop(_RMSprop):
     @torch.no_grad()
     def step(self, closure=None):
         """Performs a single optimization step.
         Arguments:
             closure (callable, optional): A closure that reevaluates the model
                 and returns the loss.
         """
         loss = None
         if closure is not None:
             with torch.enable_grad():
                 loss = closure()
 
         for group in self.param_groups:
-            for p in group['params']:
+            for p in group["params"]:
                 if p.grad is None:
                     continue
                 grad = p.grad
                 if grad.is_sparse:
-                    raise RuntimeError('RMSprop does not support sparse gradients')
+                    raise RuntimeError("RMSprop does not support sparse gradients")
                 state = self.state[p]
 
                 # State initialization
                 if len(state) == 0:
-                    state['step'] = 0
-                    # be default PyTorch inits with zeros. it doesn't converge well 
+                    state["step"] = 0
+                    # be default PyTorch inits with zeros. it doesn't converge well
                     # check https://github.com/pytorch/pytorch/issues/23796 for details
-                    state['square_avg'] = torch.ones_like(p, memory_format=torch.preserve_format)
-                    if group['momentum'] > 0:
-                        state['momentum_buffer'] = torch.zeros_like(p, memory_format=torch.preserve_format)
-                    if group['centered']:
-                        state['grad_avg'] = torch.zeros_like(p, memory_format=torch.preserve_format)
+                    state["square_avg"] = torch.ones_like(p, memory_format=torch.preserve_format)
+                    if group["momentum"] > 0:
+                        state["momentum_buffer"] = torch.zeros_like(p, memory_format=torch.preserve_format)
+                    if group["centered"]:
+                        state["grad_avg"] = torch.zeros_like(p, memory_format=torch.preserve_format)
 
-                square_avg = state['square_avg']
-                alpha = group['alpha']
+                square_avg = state["square_avg"]
+                alpha = group["alpha"]
 
-                state['step'] += 1
+                state["step"] += 1
 
-                if group['weight_decay'] != 0:
-                    grad = grad.add(p, alpha=group['weight_decay'])
+                if group["weight_decay"] != 0:
+                    grad = grad.add(p, alpha=group["weight_decay"])
 
                 square_avg.mul_(alpha).addcmul_(grad, grad, value=1 - alpha)
 
-                if group['centered']:
-                    grad_avg = state['grad_avg']
+                if group["centered"]:
+                    grad_avg = state["grad_avg"]
                     grad_avg.mul_(alpha).add_(grad, alpha=1 - alpha)
-                    avg = square_avg.addcmul(-1, grad_avg, grad_avg).add(group['eps']).sqrt_()  # eps moved in sqrt
+                    avg = square_avg.addcmul(-1, grad_avg, grad_avg).add(group["eps"]).sqrt_()  # eps moved in sqrt
                 else:
-                    avg = square_avg.add_(group['eps']).sqrt() # eps moved in sqrt
+                    avg = square_avg.add_(group["eps"]).sqrt()  # eps moved in sqrt
 
-                if group['momentum'] > 0:
-                    buf = state['momentum_buffer']
-                    buf.mul_(group['momentum']).addcdiv_(grad, avg)
-                    p.add_(buf, alpha=-group['lr'])
+                if group["momentum"] > 0:
+                    buf = state["momentum_buffer"]
+                    buf.mul_(group["momentum"]).addcdiv_(grad, avg)
+                    p.add_(buf, alpha=-group["lr"])
                 else:
-                    p.addcdiv_(grad, avg, value=-group['lr'])
+                    p.addcdiv_(grad, avg, value=-group["lr"])
 
-        return loss
+        return loss
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/lr_finder.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/lr_finder.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/lookahead.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/lookahead.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/__init__.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/sgdw.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/sgdw.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,19 @@
             raise ValueError(f"Invalid learning rate: {lr}")
         if momentum < 0.0:
             raise ValueError(f"Invalid momentum value: {momentum}")
         if weight_decay < 0.0:
             raise ValueError(f"Invalid weight_decay value: {weight_decay}")
 
         defaults = dict(
-            lr=lr, momentum=momentum, dampening=dampening, weight_decay=weight_decay, nesterov=nesterov,
+            lr=lr,
+            momentum=momentum,
+            dampening=dampening,
+            weight_decay=weight_decay,
+            nesterov=nesterov,
         )
         if nesterov and (momentum <= 0 or dampening != 0):
             raise ValueError("Nesterov momentum requires a momentum and zero dampening")
         super(SGDW, self).__init__(params, defaults)
 
     def __setstate__(self, state):
         super(SGDW, self).__setstate__(state)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/optim/schedulers.py` & `pytorch_tools-0.5.1/pytorch_tools/optim/schedulers.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/hrnet.py` & `pytorch_tools-0.5.1/pytorch_tools/models/hrnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,15 @@
 import logging
 from copy import deepcopy
 from functools import wraps, partial
 
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
-from torchvision.models.utils import load_state_dict_from_url
-
+from torch.hub import load_state_dict_from_url
 from pytorch_tools.modules.residual import conv1x1
 from pytorch_tools.modules.residual import conv3x3
 from pytorch_tools.modules.residual import BasicBlock
 from pytorch_tools.modules.residual import Bottleneck
 from pytorch_tools.modules import ABN
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.utils.misc import initialize
@@ -123,15 +122,15 @@
 
         return x_fuse
 
 
 class TransitionBlock(nn.Module):
     """Transition is where new branches for smaller resolution are born
     -- ==> --
-    
+
     -- ==> --
       \
        \=> --
     """
 
     def __init__(self, prev_channels, current_channels, norm_layer=ABN, norm_act="relu"):
         super().__init__()
@@ -191,17 +190,17 @@
         for i in range(1, 4):
             x[i] = x[i] + self.downsamp_modules[i - 1](x[i - 1])
         return self.final_layer(x[3])
 
 
 class HighResolutionNet(nn.Module):
     """HighResolution Nets constructor
-    Supports any width and small version of the network 
+    Supports any width and small version of the network
 
-    Ref: 
+    Ref:
         * HRNet paper https://arxiv.org/abs/1908.07919
 
 
     Args:
         width (int):
             Width of the branch with highest resolution. Other branches are scales accordingly. Better don't pass mannualy.
         small (bool): Flag to construct smaller version of the model with less number of blocks in each stage.
@@ -215,16 +214,16 @@
         norm_layer (str):
             Normalization layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory footprint.
             But increases backward time. Defaults to 'abn'.
         norm_act (str):
             Activation for normalizion layer. It's reccomended to use `leacky_relu` with `inplaceabn`. Default: 'relu'
         encoder (bool):
             Flag to overwrite forward pass to return 5 tensors with different resolutions. Defaults to False.
-            NOTE: HRNet first features have resolution 4x times smaller than input, not 2x as all other models. 
-            So it CAN'T be used as encoder in Unet and Linknet models 
+            NOTE: HRNet first features have resolution 4x times smaller than input, not 2x as all other models.
+            So it CAN'T be used as encoder in Unet and Linknet models
     """
 
     # drop_rate (float):
     #     Dropout probability before classifier, for training. Defaults to 0.
     def __init__(
         self,
         width=18,
@@ -257,15 +256,18 @@
         self.transition2 = TransitionBlock(channels[:2], channels[:3], **bn_args)
         self.stage3 = self._make_stage(  # 3 if small else 4
             n_modules=(4, 3)[small], n_branches=3, n_blocks=n_blocks[:3], n_chnls=channels[:3]
         )
 
         self.transition3 = TransitionBlock(channels[:3], channels, **bn_args)
         self.stage4 = self._make_stage(  # 2 if small else 3
-            n_modules=(3, 2)[small], n_branches=4, n_blocks=n_blocks, n_chnls=channels,
+            n_modules=(3, 2)[small],
+            n_branches=4,
+            n_blocks=n_blocks,
+            n_chnls=channels,
         )
 
         self.encoder = encoder
         if encoder:
             self.forward = self.encoder_features
         else:
             # Classification Head
@@ -274,15 +276,22 @@
             self.last_linear = nn.Linear(2048, num_classes)
         # initialize weights
         initialize(self)
 
     def _make_stage(self, n_modules, n_branches, n_blocks, n_chnls):
         modules = []
         for i in range(n_modules):
-            modules.append(HighResolutionModule(n_branches, n_blocks, n_chnls, **self.bn_args,))
+            modules.append(
+                HighResolutionModule(
+                    n_branches,
+                    n_blocks,
+                    n_chnls,
+                    **self.bn_args,
+                )
+            )
         return nn.Sequential(*modules)
 
     def encoder_features(self, x):
         # stem
         x = self.conv1(x)
         x = self.bn1(x)
         x = self.conv2(x)
@@ -374,17 +383,15 @@
     if pretrained:
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = HighResolutionNet(**kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"])
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/preprocessing.py` & `pytorch_tools-0.5.1/pytorch_tools/models/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,10 +23,8 @@
 
 def get_preprocessing_fn(pretrain_settings):
     input_space = pretrain_settings.get("input_space")
     input_range = pretrain_settings.get("input_range")
     mean = pretrain_settings.get("mean")
     std = pretrain_settings.get("std")
 
-    return functools.partial(
-        preprocess_input, mean=mean, std=std, input_space=input_space, input_range=input_range
-    )
+    return functools.partial(preprocess_input, mean=mean, std=std, input_space=input_space, input_range=input_range)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/b_model.py` & `pytorch_tools-0.5.1/pytorch_tools/models/b_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -214,15 +214,17 @@
         first_norm = nn.Identity() if block_fns[0].startswith("Pre") else norm_layer(stem_width, activation=norm_act)
         if stem_type == "default":
             self.stem_conv1 = nn.Sequential(conv3x3(in_channels, stem_width, stride=2), first_norm)
         elif stem_type == "s2d":
             # instead of default stem I'm using Space2Depth followed by conv. no norm because there is one at the beginning
             # of DarkStage. upd. there is norm in not PreAct version
             self.stem_conv1 = nn.Sequential(
-                SpaceToDepth(block_size=2), conv3x3(in_channels * 4, stem_width), first_norm,
+                SpaceToDepth(block_size=2),
+                conv3x3(in_channels * 4, stem_width),
+                first_norm,
             )
         else:
             raise ValueError(f"Stem type `{stem_type}` is not supported")
 
         bn_args = dict(norm_layer=norm_layer, norm_act=norm_act)
         block_name_to_module = {
             "XX": SimpleBasicBlock,
@@ -297,33 +299,33 @@
             self.head = nn.Sequential(
                 last_norm,
                 conv1x1(channels[3], head_width),
                 norm_layer(head_width, activation=head_norm_act),
                 FastGlobalAvgPool2d(flatten=True),
             )
             self.last_linear = nn.Linear(head_width, num_classes)
-        elif head_type == "default_nonorm": # if used in angular losses don't want norm
+        elif head_type == "default_nonorm":  # if used in angular losses don't want norm
             self.head = nn.Sequential(
                 last_norm,
-                conv1x1(channels[3], head_width, bias=True), # need bias because not followed by norm
+                conv1x1(channels[3], head_width, bias=True),  # need bias because not followed by norm
                 FastGlobalAvgPool2d(flatten=True),
             )
             self.last_linear = nn.Linear(head_width, num_classes)
         elif head_type == "mlp_bn_fc_bn":
             self.head = nn.Sequential(
                 last_norm,
                 conv1x1(channels[3], channels[3]),
                 FastGlobalAvgPool2d(flatten=True),
                 nn.BatchNorm1d(channels[3]),
                 pt.modules.activations.activation_from_name(head_norm_act),
                 nn.Linear(channels[3], head_width, bias=False),
                 nn.BatchNorm1d(head_width, affine=False),
             )
             self.last_linear = nn.Linear(head_width, num_classes)
-        elif head_type == "mlp_bn_fc": # same as above but without last BN
+        elif head_type == "mlp_bn_fc":  # same as above but without last BN
             self.head = nn.Sequential(
                 last_norm,
                 conv1x1(channels[3], channels[3]),
                 FastGlobalAvgPool2d(flatten=True),
                 nn.BatchNorm1d(channels[3]),
                 pt.modules.activations.activation_from_name(head_norm_act),
                 nn.Linear(channels[3], head_width, bias=False),
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/efficientnet.py` & `pytorch_tools-0.5.1/pytorch_tools/models/efficientnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,27 +14,27 @@
 import logging
 from copy import deepcopy
 from collections import OrderedDict
 from functools import wraps, partial
 
 import torch
 from torch import nn
-from torchvision.models.utils import load_state_dict_from_url
-
+from torch.hub import load_state_dict_from_url
 from pytorch_tools.modules import ABN
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.modules.residual import InvertedResidual
 from pytorch_tools.modules.residual import conv1x1, conv3x3
 from pytorch_tools.modules.tf_same_ops import conv_to_same_conv
 from pytorch_tools.modules.tf_same_ops import maxpool_to_same_maxpool
 from pytorch_tools.utils.misc import initialize
 from pytorch_tools.utils.misc import add_docs_for
 from pytorch_tools.utils.misc import make_divisible
 from pytorch_tools.utils.misc import DEFAULT_IMAGENET_SETTINGS
 from pytorch_tools.utils.misc import repeat_channels
+from pytorch_tools.utils.misc import patch_bn_mom
 
 # avoid overwriting doc string
 wraps = partial(wraps, assigned=("__module__", "__name__", "__qualname__", "__annotations__"))
 
 
 class EfficientNet(nn.Module):
     """EfficientNet B0-B7
@@ -140,15 +140,15 @@
             num_features = make_divisible(1280 * width_multiplier)
             self.conv_head = conv1x1(out_channels, num_features)
             self.bn2 = norm_layer(num_features, activation=norm_act)
             self.global_pool = nn.AdaptiveAvgPool2d(1)
             self.dropout = nn.Dropout(drop_rate, inplace=True)
             self.last_linear = nn.Linear(num_features, num_classes)
 
-        patch_bn_tf(self)  # adjust epsilon
+        patch_bn_mom(self, 0.01)  # adjust epsilon
         initialize(self)
         if match_tf_same_padding:
             conv_to_same_conv(self)
             maxpool_to_same_maxpool(self)
 
     def encoder_features(self, x):
         x0 = self.conv_stem(x)
@@ -215,15 +215,15 @@
             dilation //= 2
         if dilation == 1:
             break
     return blocks_args
 
 
 def _decode_block_string(block_string):
-    """ Gets a block through a string notation of arguments. """
+    """Gets a block through a string notation of arguments."""
     assert isinstance(block_string, str)
 
     ops = block_string.split("_")
     options = {}
     for op in ops:
         splits = re.split(r"(\d.*)", op)
         if len(splits) >= 2:
@@ -266,37 +266,37 @@
 PRETRAIN_SETTINGS = DEFAULT_IMAGENET_SETTINGS
 PRETRAIN_SETTINGS["interpolation"] = "bicubic"
 PRETRAIN_SETTINGS["crop_pct"] = 0.875
 
 CFGS = {
     # All pretrained models were trained on TF by Google and ported to PyTorch by Ross Wightman @rwightman
     # Due to framework little differences (BN epsilon and different padding in convs) this weights give slightly
-    # worse performance when loaded into model above but the drop is only about ~1% on Imagenet and doesn't really 
-    # mater for transfer learning 
+    # worse performance when loaded into model above but the drop is only about ~1% on Imagenet and doesn't really
+    # mater for transfer learning
     # upd. by default weights from Noisy Student paper are loaded due to a much better predictions
     "efficientnet-b0": {
         "default": {
             "params": {
-                "blocks_args": EFFNET_BLOCKARGS, "width_multiplier": 1.0, "depth_multiplier": 1.0}, 
+                "blocks_args": EFFNET_BLOCKARGS, "width_multiplier": 1.0, "depth_multiplier": 1.0},
                 **PRETRAIN_SETTINGS,
                 "input_size": [3, 224, 224],
             },
         "imagenet": {
             "url": "https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b0_ns-c0e6a31c.pth",
         },
         "imagenet2": {
             "url": "https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b0_aa-827b6e33.pth",
         },
     },
     "efficientnet-b1": {
         "default": {
             "params": {
-                "blocks_args": EFFNET_BLOCKARGS, "width_multiplier": 1.0, "depth_multiplier": 1.1}, 
+                "blocks_args": EFFNET_BLOCKARGS, "width_multiplier": 1.0, "depth_multiplier": 1.1},
                 **PRETRAIN_SETTINGS,
-                "input_size": [3, 240, 240], 
+                "input_size": [3, 240, 240],
                 "crop_pct": 0.882,
             },
         "imagenet": {
             "url": "https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b1_ns-99dd0c41.pth",
         },
         "imagenet2": {
             "url": "https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/tf_efficientnet_b1_aa-ea7a6ee0.pth",
@@ -387,55 +387,42 @@
         },
     },
 }
 
 # fmt: on
 
 
-def patch_bn_tf(module):
-    """TF ported weights use slightly different eps in BN. Need to adjust for better performance"""
-    if isinstance(module, ABN):
-        module.eps = 1e-3
-        module.momentum = 1e-2
-    for m in module.children():
-        patch_bn_tf(m)
-
-
 def _efficientnet(arch, pretrained=None, **kwargs):
     cfgs = deepcopy(CFGS)
     cfg_settings = cfgs[arch]["default"]
     cfg_params = cfg_settings.pop("params")
     cfg_params["blocks_args"] = decode_block_args(cfg_params["blocks_args"])
     if pretrained:
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = EfficientNet(**kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"])
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
                 "Using model pretrained for {} classes with {} classes. Last layer is initialized randomly".format(
                     cfg_settings["num_classes"], kwargs_cls
                 )
             )
             state_dict["classifier.weight"] = model.state_dict()["last_linear.weight"]
             state_dict["classifier.bias"] = model.state_dict()["last_linear.bias"]
         if kwargs.get("in_channels", 3) != 3:  # support pretrained for custom input channels
-            state_dict["conv_stem.weight"] = repeat_channels(
-                state_dict["conv_stem.weight"], kwargs["in_channels"]
-            )
+            state_dict["conv_stem.weight"] = repeat_channels(state_dict["conv_stem.weight"], kwargs["in_channels"])
         model.load_state_dict(state_dict)
     setattr(model, "pretrained_settings", cfg_settings)
     return model
 
 
 @wraps(EfficientNet)
 @add_docs_for(EfficientNet)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/resnet.py` & `pytorch_tools-0.5.1/pytorch_tools/models/resnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,26 +49,26 @@
             If not, returns a model pre-trained on 'str' dataset. `imagenet` is available
             for every model but some have more. Check the code to find out.
         num_classes (int):
             Number of classification classes. Defaults to 1000.
         in_channels (int):
             Number of input (color) channels. Defaults to 3.
         attn_type (Union[str, None]):
-            If given, selects attention type to use in blocks. One of 
+            If given, selects attention type to use in blocks. One of
             `se` - Squeeze-Excitation
             `eca` - Efficient Channel Attention
         groups (int):
             Number of convolution groups for 3x3 conv in Bottleneck. Defaults to 1.
         base_width (int):
             Factor determining bottleneck channels. `planes * base_width / 64 * groups`. Defaults to 64.
         stem_type (str):
-            Type on input stem. Supported options are: 
+            Type on input stem. Supported options are:
             '' - default. One 7x7 conv with 64 channels
             'deep' - three 3x3 conv with 32, 32, 64, channels
-            'space2depth' - Reshape followed by one convolution. Idea from TResNet paper 
+            'space2depth' - Reshape followed by one convolution. Idea from TResNet paper
         output_stride (List[8, 16, 32]): Applying dilation strategy to pretrained ResNet. Typically used in
             Semantic Segmentation. Defaults to 32.
             NOTE: Don't use this arg with `antialias` and `pretrained` together. it may produce weird results
         norm_layer (str):
             Normalization layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory footprint.
             But increases backward time. Defaults to 'abn'.
         norm_act (str):
@@ -76,15 +76,15 @@
         antialias (bool):
             Flag to turn on Rect-2 antialiasing from https://arxiv.org/abs/1904.11486. Defaults to False.
         encoder (bool):
             Flag to overwrite forward pass to return 5 tensors with different resolutions. Defaults to False.
         drop_rate (float):
             Dropout probability before classifier, for training. Defaults to 0.0.
         drop_connect_rate (float):
-            Drop rate for StochasticDepth. Randomly removes samples each block. Used as regularization during training. 
+            Drop rate for StochasticDepth. Randomly removes samples each block. Used as regularization during training.
             keep prob will be linearly decreased from 1 to 1 - drop_connect_rate each block. Ref: https://arxiv.org/abs/1603.09382
         init_bn0 (bool):
             Zero-initialize the last BN in each residual branch, so that the residual
             branch starts with zeros, and each residual block behaves like an identity.
             This improves the model by 0.2~0.3% according to https://arxiv.org/abs/1706.02677. Defaults to True.
     """
 
@@ -237,17 +237,15 @@
                     conv3x3(in_channels, stem_width // 2, 2),
                     norm_layer(stem_width // 2, activation=norm_act),
                     conv3x3(stem_width // 2, stem_width // 2),
                     norm_layer(stem_width // 2, activation=norm_act),
                     conv3x3(stem_width // 2, stem_width),
                 )
             else:
-                self.conv1 = nn.Conv2d(
-                    in_channels, stem_width, kernel_size=7, stride=2, padding=3, bias=False
-                )
+                self.conv1 = nn.Conv2d(in_channels, stem_width, kernel_size=7, stride=2, padding=3, bias=False)
             self.bn1 = norm_layer(stem_width, activation=norm_act)
             self.maxpool = nn.MaxPool2d(kernel_size=3, stride=2, padding=1)
 
     def _initialize_weights(self, init_bn0=False):
         for m in self.modules():
             if isinstance(m, nn.Conv2d):
                 nn.init.kaiming_normal_(m.weight, mode="fan_out", nonlinearity="relu")
@@ -336,33 +334,33 @@
         "imagenet2": {  # weigths from rwightman. Acc@1: 73.25. Acc@5: 91.32
             "url": "https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/resnet34-43635321.pth",
         },
     },
     "resnet50": {
         "default": {"params": {"block": Bottleneck, "layers": [3, 4, 6, 3]}, **DEFAULT_IMAGENET_SETTINGS,},
         "imagenet": {"url": "https://download.pytorch.org/models/resnet50-19c8e357.pth"},
-        # I couldn't validate this weights because they give Acc@1 0.1 maybe a bug somewhere. Still leaving them just in case 
+        # I couldn't validate this weights because they give Acc@1 0.1 maybe a bug somewhere. Still leaving them just in case
         # it works better that starting from scratch
         "imagenet_gn": {
-            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-101-GN-abf6008e.pth", 
+            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-101-GN-abf6008e.pth",
             "params": {"norm_layer": "agn"}
         },
         # Acc@1: 76.33. Acc@5: 93.34. This weights only work with weight standardization!
         "imagenet_gn_ws": {
-            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-50-GN-WS-fd84efb6.pth", 
+            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-50-GN-WS-fd84efb6.pth",
             "params": {"norm_layer": "agn"}
         },
     },
     "resnet101": {
         "default": {"params": {"block": Bottleneck, "layers": [3, 4, 23, 3]}, **DEFAULT_IMAGENET_SETTINGS,},
         "imagenet": {"url": "https://download.pytorch.org/models/resnet101-5d3b4d8f.pth"},
-        # I couldn't validate this weights because they give Acc@1 0.1 maybe a bug somewhere. Still leaving them just in case 
+        # I couldn't validate this weights because they give Acc@1 0.1 maybe a bug somewhere. Still leaving them just in case
         # it works better that starting from scratch
         "imagenet_gn": {
-            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-101-GN-abf6008e.pth", 
+            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-101-GN-abf6008e.pth",
             "params": {"norm_layer": "agn"}
         },
         # Acc@1: 77.85. Acc@5: 93.90. This weights only work with weight standardization!
         "imagenet_gn_ws": {
             "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/R-101-GN-WS-c067a7de.pth",
             "params": {"norm_layer": "agn"}
         },
@@ -396,15 +394,15 @@
         "imagenet": {"url": "https://download.pytorch.org/models/resnext50_32x4d-7cdf4587.pth"},
         # weights from rwightman
         "imagenet2": {
             "url": "https://github.com/rwightman/pytorch-image-models/releases/download/v0.1-weights/resnext50d_32x4d-103e99f8.pth"
         },
         # Acc@1: 77.28. Acc@5: 93.61. This weights only work with weight standardization!
         "imagenet_gn_ws": {
-            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/X-50-GN-WS-2dea43a8.pth", 
+            "url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/X-50-GN-WS-2dea43a8.pth",
             "params": {"norm_layer": "agn"}
         },
     },
     "resnext101_32x4d": {
         "default": {
             "params": {"block": Bottleneck, "layers": [3, 4, 23, 3], "base_width": 4, "groups": 32,},
             **DEFAULT_IMAGENET_SETTINGS,
@@ -545,17 +543,15 @@
     if pretrained:
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = ResNet(**kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"])
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/bit_resnet.py` & `pytorch_tools-0.5.1/pytorch_tools/models/bit_resnet.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 
 # this models are designed for trasfer learning only! not for training from scratch
 class ResNetV2(nn.Module):
     """
     Implementation of Pre-activation (v2) ResNet mode.
     Used to create Bit-M-50/101/152x1/2/3/4 models
-    
+
     Args:
         num_classes (int): Number of classification classes. Defaults to 5
     """
 
     def __init__(
         self,
         block_units,
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/vgg.py` & `pytorch_tools-0.5.1/pytorch_tools/models/vgg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from copy import deepcopy
 from functools import wraps, partial
 
 import torch
 import torch.nn as nn
-from torchvision.models.utils import load_state_dict_from_url
-
+from torch.hub import load_state_dict_from_url
 from pytorch_tools.modules import BlurPool
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.utils.misc import initialize
 from pytorch_tools.utils.misc import add_docs_for
 from pytorch_tools.utils.misc import DEFAULT_IMAGENET_SETTINGS
 
 # avoid overwriting doc string
@@ -20,19 +19,19 @@
     """
     Args:
         pretrained (str): if present, returns a model pre-trained on 'str' dataset
         num_classes (int, optional): [description]. Defaults to 1000.
         in_channels (int): Number of input (color) channels. Defaults to 3.
         norm_layer (ABN, optional): Which version of ABN to use. Choices are:
             'ABN' - dropin replacement for BN+Relu.
-            'InplaceABN' - efficient version. If used with `pretrain` Weights still 
-                will be loaded but performance may be worse than with ABN. 
-        encoder (bool, optional): Flag to return features with different resolution. 
+            'InplaceABN' - efficient version. If used with `pretrain` Weights still
+                will be loaded but performance may be worse than with ABN.
+        encoder (bool, optional): Flag to return features with different resolution.
             Defaults to False.
-        antialias (bool, optional): Flag to turn on Rect-2 antialiasing 
+        antialias (bool, optional): Flag to turn on Rect-2 antialiasing
             from https://arxiv.org/abs/1904.11486. Defaults to False.
     """
 
     def __init__(
         self,
         layers,
         pretrained=None,  # not used. here for proper signature.
@@ -166,17 +165,15 @@
     if pretrained:
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = VGG(**kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"])
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/__init__.py` & `pytorch_tools-0.5.1/pytorch_tools/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,8 +51,9 @@
 from .bit_resnet import bit_m_50x1
 from .bit_resnet import bit_m_50x3
 from .bit_resnet import bit_m_101x1
 from .bit_resnet import bit_m_101x3
 from .bit_resnet import bit_m_152x2
 from .bit_resnet import bit_m_152x4
 
-from .b_model import BNet
+from .b_model import BNet
+from .cmodel import CModel
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/tresnet.py` & `pytorch_tools-0.5.1/pytorch_tools/models/tresnet.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import logging
 from copy import deepcopy
 from functools import wraps, partial
 
 import torch
 import torch.nn as nn
-from torchvision.models.utils import load_state_dict_from_url
-
+from torch.hub import load_state_dict_from_url
 from pytorch_tools.models.resnet import ResNet
 from pytorch_tools.modules import TBasicBlock, TBottleneck
 from pytorch_tools.modules import FastGlobalAvgPool2d, BlurPool
 from pytorch_tools.modules import SpaceToDepth
 from pytorch_tools.modules.residual import conv1x1, conv3x3
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.modules import ABN
@@ -20,42 +19,42 @@
 wraps = partial(wraps, assigned=("__module__", "__name__", "__qualname__", "__annotations__"))
 
 
 class TResNet(ResNet):
     """TResNet M / TResNet L / XL
 
 
-    Ref: 
+    Ref:
         * TResNet paper: https://arxiv.org/abs/2003.13630
 
 
     Args:
         layers (List[int]):
             Numbers of layers in each block.
         pretrained (str, optional):
             If not, returns a model pre-trained on 'str' dataset. `imagenet` is available
             for every model but some have more. Check the code to find out.
         num_classes (int):
             Number of classification classes. Defaults to 1000.
         in_channels (int):
             Number of input (color) channels. Defaults to 3.
-        width_factor (int): 
+        width_factor (int):
             Stem width is 64 * width_factor. neede to make larger models
         output_stride (List[8, 16, 32]): Applying dilation strategy to pretrained ResNet. Typically used in
             Semantic Segmentation. Defaults to 32.
             NOTE: Don't use this arg with `antialias` and `pretrained` together. it may produce weird results
         norm_layer (str):
             Normalization layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory footprint.
             But increases backward time. Defaults to 'inplaceabn'.
         norm_act (str):
             Activation for normalizion layer. It's reccomended to use `leacky_relu` with `inplaceabn`.
         encoder (bool):
             Flag to overwrite forward pass to return 5 tensors with different resolutions. Defaults to False.
-            NOTE: TResNet first features have resolution 4x times smaller than input, not 2x as all other models. 
-            So it CAN'T be used as encoder in Unet and Linknet models 
+            NOTE: TResNet first features have resolution 4x times smaller than input, not 2x as all other models.
+            So it CAN'T be used as encoder in Unet and Linknet models
         drop_rate (float):
             Dropout probability before classifier, for training. Defaults to 0.
         drop_connect_rate (float):
             Drop rate for StochasticDepth. Randomly removes samples each block. Used as regularization during training. Ref: https://arxiv.org/abs/1603.09382
     """
 
     def __init__(
@@ -100,21 +99,17 @@
         self.block = TBasicBlock
         self.expansion = TBasicBlock.expansion
         self.layer1 = self._make_layer(stem_width, layers[0], stride=1, **largs)
         self.layer2 = self._make_layer(stem_width * 2, layers[1], stride=2, **largs)
 
         self.block = TBottleneck  # first 2 - Basic, last 2 - Bottleneck
         self.expansion = TBottleneck.expansion
-        self.layer3 = self._make_layer(
-            stem_width * 4, layers[2], stride=stride_3, dilation=dilation_3, **largs
-        )
+        self.layer3 = self._make_layer(stem_width * 4, layers[2], stride=stride_3, dilation=dilation_3, **largs)
         largs.update(attn_type=None)  # no se in last layer
-        self.layer4 = self._make_layer(
-            stem_width * 8, layers[3], stride=stride_4, dilation=dilation_4, **largs
-        )
+        self.layer4 = self._make_layer(stem_width * 8, layers[3], stride=stride_4, dilation=dilation_4, **largs)
         self.global_pool = FastGlobalAvgPool2d(flatten=True)
         self.num_features = stem_width * 8 * self.expansion
         self.encoder = encoder
         if not encoder:
             self.dropout = nn.Dropout(p=drop_rate, inplace=True)
             self.last_linear = nn.Linear(self.num_features, num_classes)
         else:
@@ -135,15 +130,15 @@
     "input_space": "RGB",
     "input_size": [3, 448, 448],
     "input_range": [0, 1],
     "mean": [0., 0., 0.],
     "std": [1., 1., 1.],
     "num_classes": 1000,
 }
-# for each model there are weights trained on 224 crops from imagenet and 
+# for each model there are weights trained on 224 crops from imagenet and
 # weights finetuned on 448x448 crops. I'm using the latest as default because they work better for
 # finetuning on large image sizes
 CFGS = {
     "tresnetm": {
         "default": {"params": {"layers": [3, 4, 11, 3]}, **PRETRAIN_SETTINGS,},
         # Acc@1 81.712 Acc@5 95.502 on 448 crops and proper normalization
         "imagenet": {"url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.2/patched_tresnet_m_448-a236aa30.pth"},
@@ -191,17 +186,15 @@
     if pretrained:
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = TResNet(**kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"], check_hash=True)
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/models/densenet.py` & `pytorch_tools-0.5.1/pytorch_tools/models/densenet.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 Models fully compatible with default torchvision weights
 """
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.utils.checkpoint as cp
 from collections import OrderedDict
-from torchvision.models.utils import load_state_dict_from_url
+from torch.hub import load_state_dict_from_url
 from functools import wraps, partial
 from pytorch_tools.modules.residual import conv1x1, conv3x3
 from pytorch_tools.modules import GlobalPool2d
 from pytorch_tools.utils.misc import initialize
 from pytorch_tools.utils.misc import add_docs_for
 from pytorch_tools.utils.misc import DEFAULT_IMAGENET_SETTINGS
 from pytorch_tools.modules import bn_from_name
@@ -27,15 +27,15 @@
 # avoid overwriting doc string
 wraps = partial(wraps, assigned=("__module__", "__name__", "__qualname__", "__annotations__"))
 
 
 class _Transition(nn.Module):
     r"""
     Transition Block as described in [DenseNet](https://arxiv.org/abs/1608.06993)
-    
+
     - Activation
     - 1x1 Convolution (with optional compression of the number of channels)
     - 2x2 Average Pooling
     """
 
     def __init__(self, in_planes, out_planes, norm_layer=ABN, norm_act="relu"):
         super(_Transition, self).__init__()
@@ -59,15 +59,21 @@
     return bn_function
 
 
 class _DenseLayer(nn.Module):
     expansion = 4
 
     def __init__(
-        self, in_planes, growth_rate, drop_rate=0.0, memory_efficient=False, norm_layer=ABN, norm_act="relu",
+        self,
+        in_planes,
+        growth_rate,
+        drop_rate=0.0,
+        memory_efficient=False,
+        norm_layer=ABN,
+        norm_act="relu",
     ):
         super(_DenseLayer, self).__init__()
 
         width = growth_rate * self.expansion
         self.norm1 = norm_layer(in_planes, activation=norm_act)
         self.conv1 = conv1x1(in_planes, width)
         self.norm2 = norm_layer(width, activation=norm_act)
@@ -101,38 +107,38 @@
         return torch.cat(out, 1)
 
 
 class DenseNet(nn.Module):
     r"""
 
     Args:
-        growth_rate (int): 
+        growth_rate (int):
             How many filters to add each layer (`k` in paper).
-        block_config (List[int]): 
+        block_config (List[int]):
             How many layers in each pooling block.
-        pretrained (str): 
+        pretrained (str):
             if present, returns a model pre-trained on 'str' dataset
-        num_classes (int): 
+        num_classes (int):
             Number of classification classes. Defaults to 1000.
-        drop_rate (float): 
+        drop_rate (float):
             Dropout probability after each DenseLayer. Defaults to 0.0.
-        in_channels (int): 
+        in_channels (int):
             Number of input (color) channels. Defaults to 3.
-        norm_layer (str): 
-            Nomaliztion layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory footprint. 
+        norm_layer (str):
+            Nomaliztion layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory footprint.
             But increases backward time. Defaults to 'abn'.
-        norm_act (str): 
+        norm_act (str):
             Activation for normalizion layer. It's reccomended to use `relu` with `abn`.
-        deep_stem (bool): 
+        deep_stem (bool):
             Whether to replace the 7x7 conv1 with 3 3x3 convolution layers. Defaults to False.
         stem_width (int):
             Number of filters in the input stem
-        encoder (bool): 
+        encoder (bool):
             Flag to overwrite forward pass to return 5 tensors with different resolutions. Defaults to False.
-        global_pool (str): 
+        global_pool (str):
             Global pooling type. One of 'avg', 'max', 'avgmax', 'catavgmax'. Defaults to 'avg'.
         memory_efficient (bool):
             Use checkpointing. Much more memory efficient, but slower.
             See `"paper" <https://arxiv.org/pdf/1707.06990.pdf>`_. Defaults to True.
     """
 
     def __init__(
@@ -255,15 +261,19 @@
                 state_dict[new_key] = state_dict.pop(key)
         super().load_state_dict(state_dict, **kwargs)
 
 
 CFGS = {
     "densenet121": {
         "default": {
-            "params": {"growth_rate": 32, "block_config": (6, 12, 24, 16), "stem_width": 64,},
+            "params": {
+                "growth_rate": 32,
+                "block_config": (6, 12, 24, 16),
+                "stem_width": 64,
+            },
             **DEFAULT_IMAGENET_SETTINGS,
         },
         "imagenet": {"url": "https://download.pytorch.org/models/densenet121-a639ec97.pth"},
         # EXAMPLE RESNET
         # 'imagenet_inplaceabn': {
         #     'params': {'block': BasicBlock, 'layers': [2, 2, 2, 2], 'norm_layer': 'inplaceabn', 'deepstem':True, 'antialias':True},
         #     'url' : 'pathtomodel',
@@ -289,15 +299,18 @@
             "params": {"growth_rate": 32, "block_config": (6, 12, 48, 32)},
             **DEFAULT_IMAGENET_SETTINGS,
         },
         "imagenet": {"url": "https://download.pytorch.org/models/densenet201-c1103571.pth"},
     },
     # DenseNet_BC
     "densenet121_bc": {
-        "default": {"params": {"growth_rate": 32, "layers": (6, 12, 24, 16)}, **DEFAULT_IMAGENET_SETTINGS,},
+        "default": {
+            "params": {"growth_rate": 32, "layers": (6, 12, 24, 16)},
+            **DEFAULT_IMAGENET_SETTINGS,
+        },
     },
     "densenet161_bc": {
         "default": {
             "params": {"growth_rate": 48, "block_config": (6, 12, 36, 24), "stem_width": 96},
             **DEFAULT_IMAGENET_SETTINGS,
         },
     },
@@ -324,17 +337,15 @@
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
 
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = DenseNet(**kwargs)
 
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"])
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/utils/preprocessing.py` & `pytorch_tools-0.5.1/pytorch_tools/utils/preprocessing.py`

 * *Files 12% similar despite different names*

```diff
@@ -23,10 +23,8 @@
 
 def get_preprocessing_fn(pretrain_settings):
     input_space = pretrain_settings.get("input_space")
     input_range = pretrain_settings.get("input_range")
     mean = pretrain_settings.get("mean")
     std = pretrain_settings.get("std")
 
-    return functools.partial(
-        preprocess_input, mean=mean, std=std, input_space=input_space, input_range=input_range
-    )
+    return functools.partial(preprocess_input, mean=mean, std=std, input_space=input_space, input_range=input_range)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/utils/rle.py` & `pytorch_tools-0.5.1/pytorch_tools/utils/rle.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # __all__ = ['rle_decode', 'rle_encode', 'rle_to_string']
 
 
 def rle_encode(mask):
     """
     Convert mask to EncodedPixels in run-length encoding
     from https://www.kaggle.com/stainsby/fast-tested-rle-and-input-routines
-    Args: 
+    Args:
         mask(np.array): mask to be converted
     """
     pixels = mask.T.flatten()
     # We need to allow for cases where there is a '1' at either end of the sequence.
     # We do this by padding with a zero at each end when needed.
     use_padding = False
     if pixels[0] or pixels[-1]:
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/utils/box.py` & `pytorch_tools-0.5.1/pytorch_tools/utils/box.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def delta2box(deltas, anchors):
     # type: (Tensor, Tensor)->Tensor
     """Convert anchors to boxes using deltas. Boxes are expected in 'ltrb' format
     Args:
         deltas (torch.Tensor): shape [N, 4] or [BS, N, 4]
         anchors (torch.Tensor): shape [N, 4] or [BS, N, 4]
     Returns:
-        bboxes (torch.Tensor): bboxes obtained from anchors by regression 
+        bboxes (torch.Tensor): bboxes obtained from anchors by regression
             Output shape is [N, 4] or [BS, N, 4] depending on input
     """
     # cast to fp32 to avoid numerical problems with exponent
     deltas, anchors = deltas.float(), anchors.float()
     anchors_wh = anchors[..., 2:] - anchors[..., :2]
     ctr = anchors[..., :2] + 0.5 * anchors_wh
     pred_ctr = deltas[..., :2] * anchors_wh + ctr
@@ -59,28 +59,28 @@
     """
     return (box[..., 2] - box[..., 0]) * (box[..., 3] - box[..., 1])
 
 
 def clip_bboxes(bboxes, size):
     # type: (Tensor, Tuple[int, int]) -> Tensor
     """Args:
-        bboxes (torch.Tensor): in `ltrb` format. Shape [N, 4]
-        size (Union[torch.Size, tuple]): (H, W). Shape [2,]"""
+    bboxes (torch.Tensor): in `ltrb` format. Shape [N, 4]
+    size (Union[torch.Size, tuple]): (H, W). Shape [2,]"""
     bboxes[:, 0::2] = bboxes[:, 0::2].clamp(0, size[1])
     bboxes[:, 1::2] = bboxes[:, 1::2].clamp(0, size[0])
     return bboxes
 
 
 def clip_bboxes_batch(bboxes, size):
     # type: (Tensor, Tensor) -> Tensor
     """Args:
-        This function could also accept not batched bboxes but it works
-        slower than `clip_bboxes` in that case
-        bboxes (torch.Tensor): in `ltrb` format. Shape [BS, N, 4]
-        size (torch.Tensor): (H, W). Shape [BS, 2] """
+    This function could also accept not batched bboxes but it works
+    slower than `clip_bboxes` in that case
+    bboxes (torch.Tensor): in `ltrb` format. Shape [BS, N, 4]
+    size (torch.Tensor): (H, W). Shape [BS, 2]"""
     size = size.to(bboxes)
     h_size = size[..., 0].view(-1, 1, 1)  # .float()
     w_size = size[..., 1].view(-1, 1, 1)  # .float()
     h_bboxes = bboxes[..., 1::2]
     w_bboxes = bboxes[..., 0::2]
     zeros = torch.zeros_like(h_bboxes)
     bboxes[..., 1::2] = h_bboxes.where(h_bboxes > 0, zeros).where(h_bboxes < h_size, h_size)
@@ -144,21 +144,25 @@
     iou = inter / (area1[None, :, None] + area2[:, None, :] - inter)  # [B,N,M]
     return iou
 
 
 # based on https://github.com/NVIDIA/retinanet-examples/
 # and on https://github.com/google/automl/
 def generate_anchors_boxes(
-    image_size, num_scales=3, aspect_ratios=(1.0, 2.0, 0.5), pyramid_levels=(3, 4, 5, 6, 7), anchor_scale=4,
+    image_size,
+    num_scales=3,
+    aspect_ratios=(1.0, 2.0, 0.5),
+    pyramid_levels=(3, 4, 5, 6, 7),
+    anchor_scale=4,
 ):
     # type: (Tuple[int, int], int, List[float], List[int], int) -> Tuple[Tensor, int]
     """Generates multiscale anchor boxes
     Minimum object size which could be detected is anchor_scale * 2**pyramid_levels[0]. By default it's 32px
     Maximum object size which could be detected is anchor_scale * 2**pyramid_levels[-1]. By default it's 512px
-    
+
     Args:
         image_size (int or (int, int)): shape of the image
         num_scales (int): integer number representing intermediate scales added on each level. For instances,
             num_scales=3 adds three additional anchor scales [2^0, 2^0.33, 2^0.66] on each level.
         aspect_ratios (List[int]): Aspect ratios of anchor boxes
         pyramid_levels (List[int]): Levels from which features are taken. Needed to calculate stride
         anchor_scale (float): scale of size of the base anchor. Lower values allows detection of smaller objects.
@@ -169,15 +173,15 @@
         num_anchors (int): number of anchors per location
     """
 
     if isinstance(image_size, int):
         image_size = (image_size, image_size)
     scale_vals = [anchor_scale * 2 ** (i / num_scales) for i in range(num_scales)]
     # from lowest stride to largest. Anchors from models should be in the same order!
-    strides = [2 ** i for i in pyramid_levels]
+    strides = [2**i for i in pyramid_levels]
 
     # get offsets for anchor boxes for one pixel
     num_anchors = num_scales * len(aspect_ratios)
     ratio_vals_sq = torch.tensor(aspect_ratios).repeat(num_scales).sqrt()
     # view -> repeat -> view to simulate numpy.tile
     scale_vals = torch.tensor(scale_vals).view(-1, 1).repeat(1, len(aspect_ratios)).view(-1, 1)
     wh = torch.stack([torch.ones(num_anchors) * ratio_vals_sq, torch.ones(num_anchors) / ratio_vals_sq], 1)
@@ -198,15 +202,15 @@
     # clip_bboxes(all_anchors, image_size)
     return all_anchors, num_anchors
 
 
 def generate_targets(anchors, batch_gt_boxes, num_classes, matched_iou=0.5, unmatched_iou=0.4):
     # type: (Tensor, Tensor, int, float, float) -> Tuple[Tensor, Tensor, Tensor]
     """Generate targets for regression and classification
-    
+
     Based on IoU between anchor and true bounding box there are three types of anchor boxes
     1) IoU >= matched_iou: Highest similarity. Matched/Positive. Mask value is 1
     2) matched_iou > IoU >= unmatched_iou: Medium similarity. Ignored. Mask value is -1
     3) unmatched_iou > IoU: Lowest similarity. Unmatched/Negative. Mask value is 0
 
     This function works on whole batch of images at once and is very efficient
     Args:
@@ -332,17 +336,15 @@
 
     batch_size = batch_cls_head.size(0)
     num_classes = batch_cls_head.size(-1)
 
     # It's much faster to calculate topk once for full batch here rather than doing it inside loop
     # In TF The same bbox may belong to two different objects
     # select `max_detection_points` scores and corresponding bboxes
-    scores_topk_all, cls_topk_indices_all = torch.topk(
-        batch_cls_head.view(batch_size, -1), k=max_detection_points
-    )
+    scores_topk_all, cls_topk_indices_all = torch.topk(batch_cls_head.view(batch_size, -1), k=max_detection_points)
     indices_all = cls_topk_indices_all // num_classes
     classes_all = (cls_topk_indices_all % num_classes).float()  # turn to float for onnx export
 
     # applying sigmoid after topk is slightly faster than applying before
     scores_topk_all = scores_topk_all.sigmoid()  # logits -> scores
 
     # Gather corresponding bounding boxes & anchors, then regress and clip
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/utils/misc.py` & `pytorch_tools-0.5.1/pytorch_tools/utils/misc.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 import os
 import math
 import time
 import torch
 import random
 import collections
 import numpy as np
-from functools import partial
 import torch.nn as nn
 import torch.nn.functional as F
 import torch.distributed as dist
+from typing import Optional, List, Dict
 
-
-def initialize_fn(m):
-    """m (nn.Module): module"""
+# 1.71 is default for ReLU. see NFNet paper for details and timm's implementation
+def initialize_fn(m: nn.Module, gamma: float = 1.71):
     if isinstance(m, nn.Conv2d):
         # nn.init.kaiming_uniform_ doesn't take into account groups
         # remove when https://github.com/pytorch/pytorch/issues/23854 is resolved
-        # this is needed for proper init of EffNet models
-        fan_out = m.kernel_size[0] * m.kernel_size[1] * m.out_channels
-        fan_out //= m.groups
-        m.weight.data.normal_(0, math.sqrt(2.0 / fan_out))
+        m.weight.data.normal_(0, gamma / m.weight[0].numel() ** 0.5)  # gamma * 1 / sqrt(fan-in)
         if m.bias is not None:
             nn.init.constant_(m.bias, 0)
     # No check for BN because in PyTorch it is initialized with 1 & 0 by default
     elif isinstance(m, nn.Linear):
         nn.init.kaiming_uniform_(m.weight, mode="fan_out", nonlinearity="linear")
         if m.bias is not None:
             nn.init.constant_(m.bias, 0)
 
 
-def initialize(module):
-    for m in module.modules():
-        initialize_fn(m)
+def initialize(module: nn.Module, gamma: float = 1.71):
+    iterator = module.modules() if hasattr(module, "modules") else module
+    for m in iterator:
+        initialize_fn(m, gamma=gamma)
+
 
+def zero_mean_conv_weight(w: torch.Tensor):
+    """zero mean conv would prevent mean shift in the network during training"""
+    return w - w.mean(dim=(1, 2, 3), keepdim=True)
 
-def initialize_iterator(module_iterator):
-    for m in module_iterator:
-        initialize_fn(m)
+
+def normalize_conv_weight(w: torch.Tensor, gamma: float = 1):
+    """w: Conv2d weight matrix; gamma: nonlinearity gain. should be 1 for identity, 1.72 for relu. see ... for details
+    Idea for implementation is borrowed from `timm` package
+    """
+    scale = torch.full((w.size(0),), fill_value=gamma * w[0].numel() ** -0.5, device=w.device)
+    return F.batch_norm(w.view(1, w.size(0), -1), None, None, weight=scale, training=True, momentum=0).reshape_as(w)
 
 
 def set_random_seed(seed):
     random.seed(seed)
     np.random.seed(seed)
     torch.manual_seed(seed)
     torch.cuda.manual_seed_all(seed)
@@ -85,89 +90,14 @@
         return x.detach().cpu().numpy()
     elif isinstance(x, (list, tuple, int, float)):
         return np.array(x)
     else:
         raise ValueError("Unsupported type")
 
 
-def to_tensor(x, dtype=None):
-    """Convert whatever to torch Tensor"""
-    if isinstance(x, torch.Tensor):
-        if dtype is not None:
-            x = x.type(dtype)
-        return x
-    elif isinstance(x, np.ndarray):
-        x = torch.from_numpy(x)
-        if dtype is not None:
-            x = x.type(dtype)
-        return x
-    elif isinstance(x, (list, tuple)):
-        x = np.array(x)
-        x = torch.from_numpy(x)
-        if dtype is not None:
-            x = x.type(dtype)
-        return x
-    else:
-        raise ValueError("Unsupported input type" + str(type(x)))
-
-
-class AverageMeter:
-    """Computes and stores the average and current value
-        Attributes:
-            val - last value
-            avg - true average
-            avg_smooth - smoothed average"""
-
-    def __init__(self, name="Meter", avg_mom=0.9):
-        self.avg_mom = avg_mom
-        self.name = name
-        self.reset()
-
-    def reset(self):
-        self.val = 0
-        self.avg = 0
-        self.avg_smooth = 0
-        self.count = 0
-
-    def update(self, val):
-        self.val = val
-        if self.count == 0:
-            self.avg_smooth = val
-        else:
-            self.avg_smooth *= self.avg_mom
-            self.avg_smooth += val * (1 - self.avg_mom)
-        self.count += 1
-        self.avg *= (self.count - 1) / self.count
-        self.avg += val / self.count
-
-    def __call__(self, val):
-        return self.update(val)
-
-    def __repr__(self):
-        return f"AverageMeter(name={self.name}, avg={self.avg:.3f}, count={self.count})"
-        # return f"{self.name}: {self.avg:.3f}" # maybe use this version for easier printing?
-
-
-class TimeMeter:
-    def __init__(self):
-        self.reset()
-
-    def reset(self):
-        self.batch_time = AverageMeter()
-        self.data_time = AverageMeter()
-        self.start = time.time()
-
-    def batch_start(self):
-        self.data_time.update(time.time() - self.start)
-
-    def batch_end(self):
-        self.batch_time.update(time.time() - self.start)
-        self.start = time.time()
-
-
 DEFAULT_IMAGENET_SETTINGS = {
     "input_space": "RGB",
     "input_size": [3, 224, 224],
     "input_range": [0, 1],
     "mean": [0.485, 0.456, 0.406],
     "std": [0.229, 0.224, 0.225],
     "num_classes": 1000,
@@ -182,79 +112,47 @@
     return int(os.environ.get("WORLD_SIZE", 1))
 
 
 def env_rank():
     return int(os.environ.get("RANK", 0))
 
 
-def reduce_tensor(tensor):
-    return sum_tensor(tensor) / env_world_size()
-
-
-def sum_tensor(tensor):
-    rt = tensor.clone()
-    dist.all_reduce(rt, op=dist.ReduceOp.SUM)
-    return rt
-
-
-def reduce_meter(meter):
-    """Args: meter (AverageMeter): meter to reduce"""
-    if env_world_size() == 1:
-        return meter
-    # can't reduce AverageMeter so need to reduce every attribute separately
-    reduce_attributes = ["val", "avg", "avg_smooth", "count"]
-    for attr in reduce_attributes:
-        old_value = to_tensor([getattr(meter, attr)]).float().cuda()
-        setattr(meter, attr, reduce_tensor(old_value).cpu().numpy()[0])
+def filter_from_weight_decay(model: nn.Module, skip_list: Optional[List[str]] = None):
+    decay = []
+    no_decay = []
+    skip_list = listify(skip_list)
+    for name, param in model.named_parameters():
+        if not param.requires_grad:
+            continue  # frozen weights
+        in_stop_list = any(skip_word in name for skip_word in skip_list)
+        if len(param.shape) == 1 or name.endswith(".bias") or in_stop_list:
+            no_decay.append(param)
+        else:
+            decay.append(param)
+    return [{"params": decay}, {"params": no_decay, "weight_decay": 0}]
 
 
-def filter_bn_from_wd(model):
-    """
-    Filter out batch norm parameters (and bias for conv) and remove them from weight decay. Gives
-    higher accuracy for large batch training.
-    Idea from: https://arxiv.org/pdf/1807.11205.pdf
-    Code from: https://github.com/cybertronai/imagenet18
-    Args:
-        model (torch.nn.Module): model
-    Returns:
-        dict with parameters
-    """
+def patch_bn_mom(module, momentum: float = 0.01):
+    """changes default bn momentum"""
     # import inside function to avoid problems with circular imports
     import pytorch_tools.modules as pt_modules
 
     NORM_CLASSES = (
         torch.nn.modules.batchnorm._BatchNorm,
         pt_modules.ABN,
         pt_modules.SyncABN,
         pt_modules.AGN,
         pt_modules.InPlaceABN,
         pt_modules.InPlaceABNSync,
     )
-    CONV_CLASSES = (
-        torch.nn.modules.Linear,  # also add linear here
-        torch.nn.modules.conv._ConvNd,
-        pt_modules.weight_standartization.WS_Conv2d,
-    )
+    if isinstance(module, NORM_CLASSES):
+        module.momentum = momentum
 
-    def _get_params(module):
-        # for BN filter both weight and bias
-        if isinstance(module, NORM_CLASSES):
-            return module.parameters()
-        # for conv & linear only filter bias
-        elif isinstance(module, CONV_CLASSES) and module.bias is not None:
-            return (module.bias,)  # want to return list
-        accum = set()
-        for child in module.children():
-            [accum.add(p) for p in _get_params(child)]
-        return accum
-
-    bn_params = _get_params(model)
-    bn_params2 = [p for p in model.parameters() if p in bn_params]
-    rem_params = [p for p in model.parameters() if p not in bn_params]
-    return [{"params": bn_params2, "weight_decay": 0}, {"params": rem_params}]
+    for m in module.children():
+        patch_bn_mom(m, momentum)
 
 
 def make_divisible(v, divisor=8):
     min_value = divisor
     new_v = max(min_value, int(v + divisor / 2) // divisor * divisor)
     if new_v < 0.9 * v:  # ensure round down does not go down by more than 10%.
         new_v += divisor
@@ -284,7 +182,16 @@
 
     def __iter__(self):
         return ([i.cuda(non_blocking=True), t.cuda(non_blocking=True)] for i, t in self.loader)
 
     def __len__(self):
         return len(self.loader)
 
+
+def update_dict(to_dict: Dict, from_dict: Dict) -> Dict:
+    """close to `to_dict.update(from_dict)` but correctly updates internal dicts"""
+    for k, v in from_dict.items():
+        if hasattr(v, "keys") and k in to_dict.keys():
+            to_dict[k].update(v)
+        else:
+            to_dict[k] = v
+    return to_dict
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/utils/visualization.py` & `pytorch_tools-0.5.1/pytorch_tools/utils/visualization.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/kld.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/kld.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/vgg_loss.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/vgg_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,17 +122,15 @@
 
         input_gram = [self.gram_matrix(x) for x in input_features]
         style_gram = [self.gram_matrix(x) for x in style_features]
 
         loss = 0
         # for i_g, s_g in zip(input_gram, style_gram):
 
-        loss = [
-            self.criterion(torch.stack(i_g), torch.stack(s_g)) for i_g, s_g in zip(input_gram, style_gram)
-        ]
+        loss = [self.criterion(torch.stack(i_g), torch.stack(s_g)) for i_g, s_g in zip(input_gram, style_gram)]
         return loss
 
     def get_features(self, x):
         """
         Extract feature maps from the intermediate layers.
         """
         if self.layers is None:
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/huber.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/huber.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from .base import Loss
 from .base import Reduction
 
 
 class SmoothL1Loss(Loss):
     """Huber loss aka Smooth L1 Loss
-    
+
     loss = 0.5 * x^2                  if |x| <= d
     loss = 0.5 * d^2 + d * (|x| - d)  if |x| > d
 
     Args:
         delta (float): point where the Huber loss function changes from a quadratic to linear
         reduction (str): The reduction type to apply to the output. {'none', 'mean', 'sum'}.
             'none' - no reduction will be applied
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/lovasz.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/lovasz.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,17 +94,15 @@
       y_true: [B, H, W] Tensor, ground truth y_true (between 0 and C - 1)
       classes: 'all' for all, 'present' for classes present in y_true, or a list of classes to average.
       per_image: compute the loss per image instead of per batch
       ignore: void class y_true
     """
     if per_image:
         loss = mean(
-            _lovasz_softmax_flat(
-                *_flatten_preds(pred.unsqueeze(0), lab.unsqueeze(0), ignore), classes=classes
-            )
+            _lovasz_softmax_flat(*_flatten_preds(pred.unsqueeze(0), lab.unsqueeze(0), ignore), classes=classes)
             for pred, lab in zip(y_pred, y_true)
         )
     else:
         loss = _lovasz_softmax_flat(*_flatten_preds(y_pred, y_true, ignore), classes=classes)
     return loss
 
 
@@ -198,28 +196,28 @@
     Args:
         mode (str): Target mode {'binary', 'multiclass', 'multilabel'}
                 'multiclass', 'binary' - expects y_true of shape [N, H, W]
                 'multilabel' - expects y_true of shape [N, C, H, W]. Lovasz doesn't support
                     multilabel case, so target would be turned to `multiclass` with max(dim=1)
         per_image: compute the loss per image instead of per batch
         ignore: void class y_true
-    
+
     Shape:
         y_pred: [N, C, H, W]. Should be raw logits output
         y_true: [N, C, H, W] or [N, H, W] depending on mode. Values in [0, C-1]
     """
 
     def __init__(self, mode="binary", per_image=False, ignore=None):
         super().__init__()
         self.mode = Mode(mode)
         self.ignore = ignore
         self.per_image = per_image
 
     def forward(self, y_pred, y_true):
-        if self.mode == Mode.MULTILABEL and y_true.dim() == 4: # double check
+        if self.mode == Mode.MULTILABEL and y_true.dim() == 4:  # double check
             # select one class for every pixel
             y_true = y_true.argmax(dim=1)
 
         if self.mode == Mode.BINARY:
             if y_pred.size(1) != 1:
                 raise ValueError("Expected y_pred to have only 1 class in `binary` loss mode")
             return _lovasz_hinge(y_pred.squeeze(), y_true, per_image=self.per_image, ignore=self.ignore)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/focal.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/focal.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from functools import partial
 
 from .base import Loss
 from .base import Mode
-from .base import Reduction
+from .base import _reduce
 from .functional import focal_loss_with_logits
 
 
 class FocalLoss(Loss):
     """Compute focal loss between target and output logits.
 
     Args:
@@ -32,15 +32,15 @@
             Reccomended value is `0.5`. See `Reference` for paper.
         ignore_label (None or int): If not None, targets may contain values to be ignored.
             Target values equal to ignore_label will be ignored from loss computation.
 
     Shape:
         y_pred (torch.Tensor): Tensor of arbitrary shape
         y_true (torch.Tensor): Tensor of the same shape as y_pred
-    
+
     References:
         https://github.com/open-mmlab/mmdetection/blob/master/mmdet/core/loss/losses.py
         https://github.com/BloodAxe/pytorch-toolbelt/blob/develop/pytorch_toolbelt/losses/functional.py
         Normalized focal loss: https://arxiv.org/abs/1909.07829
         Reduced focal loss: https://arxiv.org/abs/1903.01347
     """
 
@@ -52,50 +52,48 @@
         reduction="mean",
         normalized=False,
         combine_thr=0.0,
         ignore_label=-1,
         temperature=1.0,
     ):
         super().__init__()
-        # use Enum to validate that values are valid
-        Mode(mode)
-        Reduction(reduction)
-        self.mode = mode
+        self.mode = Mode(mode)
         self.gamma = gamma
         self.alpha = alpha
         self.reduction = reduction
         self.normalized = normalized
         self.combine_thr = combine_thr
         self.ignore_label = ignore_label
         self.temperature = temperature
 
     def forward(self, y_pred, y_true):
         y_pred /= self.temperature
         not_ignored = y_true.ne(self.ignore_label)
-        if self.mode == "multiclass":
+        if self.mode == Mode.MULTICLASS:
             # to hangle ignore label we set it to 0, then scatter and set it to ignore index back
             y_true = y_true.where(not_ignored, torch.zeros(1).to(y_true))
             y_true_one_hot = torch.zeros_like(y_pred)
             y_true_one_hot.scatter_(1, y_true.unsqueeze(1), 1.0)
             y_true = y_true_one_hot
             # need to avoid mask shape mismatch later
-            not_ignored = torch.stack([not_ignored,] * y_pred.size(1), dim=1)
+            not_ignored = torch.stack(
+                [
+                    not_ignored,
+                ]
+                * y_pred.size(1),
+                dim=1,
+            )
 
         loss = focal_loss_with_logits(
             y_pred,
             y_true,
             gamma=self.gamma,
             alpha=self.alpha,
             reduction="none",
             normalized=self.normalized,
             combine_thr=self.combine_thr,
         )
 
         # Filter anchors with -1 label from loss computation
         loss = loss.where(not_ignored, torch.zeros(1).to(loss))
 
-        if self.reduction == "mean":
-            return loss.mean()
-        elif self.reduction == "sum":
-            return loss.sum()
-        else:
-            return loss
+        return _reduce(loss, self.reduction)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/__init__.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/smooth.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/smooth.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,37 +36,39 @@
     def __init__(
         self,
         mode="multiclass",
         smoothing=0.0,
         weight=1.0,
         reduction="mean",
         from_logits=True,
-        temperature=1.0,
+        temperature=None,
         normalize=False,
     ):
         super().__init__()
         self.mode = Mode(mode)
         self.reduction = Reduction(reduction)
         self.confidence = 1.0 - smoothing
         self.smoothing = smoothing
         self.from_logits = from_logits
         self.register_buffer("weight", torch.tensor(weight))
-        self.temperature = temperature
+        if temperature is not None:
+            self.register_buffer("temperature", torch.tensor(temperature))
         assert not (normalize and mode == "binary"), "Normalize not supported for binary case"
         self.normalize = normalize
 
     def forward(self, y_pred, y_true):
         if self.normalize:
             y_pred = F.normalize(y_pred, dim=1)
-        if self.from_logits:  # only scale logits
+        if self.from_logits and hasattr(self, "temperature"):  # only scale logits
             y_pred /= self.temperature
 
         if self.mode == Mode.BINARY:
             # squeeze to allow different shapes like BSx1xHxW vs BSxHxW
             if self.from_logits:
+                y_true = y_true.to(dtype=y_pred.dtype)  # if target is long, make sure to cast to float
                 loss = F.binary_cross_entropy_with_logits(
                     y_pred.squeeze(), y_true.squeeze(), pos_weight=self.weight, reduction=self.reduction.value
                 )
             else:
                 loss = F.binary_cross_entropy(  # no pos weight in this case
                     y_pred.squeeze(), y_true.squeeze(), reduction=self.reduction.value
                 )
@@ -77,15 +79,28 @@
             y_true_one_hot = y_true.float()
         else:
             y_true_one_hot = torch.zeros_like(y_pred)
             y_true_one_hot.scatter_(1, y_true.unsqueeze(1), 1.0)
         y_pred = y_pred.float()
         logprobs = F.log_softmax(y_pred, dim=1) if self.from_logits else y_pred.log()
         # loss of each sample is weighted by it's target class
-        logprobs = logprobs * self.weight
-        sample_weights = self.weight * y_true_one_hot
+        weight = self.weight.view(
+            1,
+            -1,
+            *(
+                [
+                    1,
+                ]
+                * (y_pred.ndim - 2)
+            )
+        )  # match dimensions
+        logprobs = logprobs * weight
+        sample_weights = weight * y_true_one_hot
         # multiple labels handling
         nll_loss = -logprobs * y_true_one_hot
         nll_loss = nll_loss.sum(1)
         smooth_loss = -logprobs.mean(dim=1)
         loss = self.confidence * nll_loss + self.smoothing * smooth_loss
-        return loss.sum().div(sample_weights.sum())
+        if self.reduction == Reduction.NONE:
+            return loss
+        else:
+            return loss.sum().div(sample_weights.sum())
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/angular.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/angular.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/detection.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/detection.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/dice_jaccard.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/dice_jaccard.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import torch
-from .base import Loss, Mode
+from .base import Loss, Mode, _reduce
 from .functional import soft_dice_score, soft_jaccard_score
 
 
 class DiceLoss(Loss):
     """
     Implementation of Dice loss for image segmentation task.
     It supports binary, multiclass and multilabel cases
@@ -18,17 +18,18 @@
     Shape:
         y_pred: [N, C, H, W]
         y_true: [N, C, H, W] or [N, H, W] depending on mode
     """
 
     IOU_FUNCTION = soft_dice_score
 
-    def __init__(self, mode="binary", log_loss=False, from_logits=True, eps=1.):
+    def __init__(self, mode="binary", reduction="mean", log_loss=False, from_logits=True, eps=1.0):
         super(DiceLoss, self).__init__()
         self.mode = Mode(mode)  # raises an error if not valid
+        self.reduction = reduction
         self.log_loss = log_loss
         self.from_logits = from_logits
         self.eps = eps
 
     def forward(self, y_pred, y_true):
         if self.from_logits:
             # Apply activations to get [0..1] class probabilities
@@ -55,21 +56,20 @@
 
         scores = self.__class__.IOU_FUNCTION(y_pred, y_true.type(y_pred.dtype), dims=dims, eps=self.eps)
 
         if self.log_loss:
             loss = -torch.log(scores)
         else:
             loss = 1 - scores
-        
+
         # IoU loss is defined for non-empty classes
         # So we zero contribution of channel that does not have true pixels
         mask = y_true.sum(dims) > 0
         loss *= mask.float()
-
-        return loss.mean()
+        return _reduce(loss, self.reduction)
 
 
 class JaccardLoss(DiceLoss):
     """
     Implementation of Jaccard loss for image segmentation task.
     It supports binary, multiclass and multilabel cases
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/functional.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/losses/hinge.py` & `pytorch_tools-0.5.1/pytorch_tools/losses/hinge.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class BinaryHinge(Loss):
     """
     Implementation of Hinge loss for binary classification tasks.
     Could be used in classification with one-hot encoded target or in
     semantic segmentation
     """
+
     def __init__(self, margin=1, pos_weight=1):
         super().__init__()
         self.margin = margin
         self.pos_weight = pos_weight
-    
+
     def forward(self, y_pred, y_true):
         return F.binary_hinge(y_pred, y_true, self.margin, self.pos_weight)
-
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/wrapper.py` & `pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/wrapper.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,74 +1,82 @@
 import copy
 import torch
 from torch.cuda import amp
-from pytorch_tools.fit_wrapper.state import RunnerState
-from pytorch_tools.fit_wrapper.callbacks import Callbacks
-from pytorch_tools.fit_wrapper.callbacks import ConsoleLogger
-from pytorch_tools.utils.misc import to_numpy
+
+from .state import RunnerState
+from .callbacks import Callbacks
+from .callbacks import ConsoleLogger
+from .utils import to_numpy
 
 
 class Runner:
     """
 
     Args:
         model: model
         optimizer: optimizer
         criterion: Loss used for training
         callbacks (List): List of Callbacks to use. Defaults to ConsoleLogger().
-        gradient_clip_val (float): Gradient clipping value. 0 means no clip. Causes ~5% training slowdown
         accumulate_steps (int): if > 1 uses gradient accumulation across iterations to simulate larger batch size
         use_fp16 (bool): Flag which enables mixed precision
     """
 
     def __init__(
         self,
         model,
         optimizer,
         criterion,
         callbacks=ConsoleLogger(),
-        gradient_clip_val=0,
         accumulate_steps=1,
         use_fp16=False,
     ):
         super().__init__()
-        self.state = RunnerState(model=model, optimizer=optimizer, criterion=criterion, use_fp16=use_fp16)
+        self.state = RunnerState(
+            model=model, optimizer=optimizer, criterion=criterion, use_fp16=use_fp16, accumulate_steps=accumulate_steps
+        )
         self.callbacks = Callbacks(callbacks)
         self.callbacks.set_state(self.state)
-        self.gradient_clip_val = gradient_clip_val
-        self.accumulate_steps = accumulate_steps
 
     def fit(
-        self, train_loader, steps_per_epoch=None, val_loader=None, val_steps=None, epochs=1, start_epoch=0,
+        self,
+        train_loader,
+        steps_per_epoch=None,
+        val_loader=None,
+        val_steps=None,
+        check_val_every_n_epoch=1,
+        epochs=1,
+        start_epoch=0,
     ):
         """
         Args:
             train_loader: DataLoader with defined `len` and `batch_size`
             steps_per_epoch (int): How many steps to count as an epochs. Useful
                 when epoch is very long or it's not clearly defined. Defaults to None.
             val_loader: Validation DataLoader with defined `len` and `batch_size` Defaults to None.
             val_steps (int): same as `steps_per_epoch` but for val data. Defaults to None.
+            check_val_every_n_epoch (int): how often to perform validation
             epochs (int): Number of epochs to train for. Defaults to 1.
             start_epoch (int): From which epoch to start. Useful on restarts. Defaults to 0.
         """
         self.state.num_epochs = epochs
-        self.state.batch_size = 1
-        if train_loader.__dict__.get("batch_size") is not None:
-            self.state.batch_size = train_loader.batch_size
+        self.state.batch_size = getattr(train_loader, "batch_size", 1)
         self.callbacks.on_begin()
         for epoch in range(start_epoch, epochs):
             self.state.is_train = True
             self.state.epoch = epoch
             self.callbacks.on_epoch_begin()
             self.state.model.train()
             self._run_loader(train_loader, steps=steps_per_epoch)
             self.state.train_loss = copy.copy(self.state.loss_meter)
             self.state.train_metrics = copy.deepcopy(self.state.metric_meters)
-
-            if val_loader is not None:
+            self.state.val_loss = None
+            self.state.val_metrics = None
+            need_val = ((epoch + 1) % check_val_every_n_epoch) == 0
+            has_val_loader = val_loader is not None
+            if has_val_loader and need_val:
                 self.evaluate(val_loader, steps=val_steps)
                 self.state.val_loss = copy.copy(self.state.loss_meter)
                 self.state.val_metrics = copy.deepcopy(self.state.metric_meters)
             self.state.reduce_meters()
             self.callbacks.on_epoch_end()
         self.callbacks.on_end()
 
@@ -85,22 +93,20 @@
         with amp.autocast(self.state.use_fp16):
             output = self.state.model(data)
             loss = self.state.criterion(output, target)
         self.state.output = output
 
         if self.state.is_train:
             # backward for every batch
-            self.state.grad_scaler.scale(loss / self.accumulate_steps).backward()
-            # everything else only before making step
-            if self.state.step % self.accumulate_steps == 0:
+            self.state.grad_scaler.scale(loss / self.state.accumulate_steps).backward()
 
-                if self.gradient_clip_val > 0:
-                    self.state.grad_scaler.unscale_(self.state.optimizer)
-                    torch.nn.utils.clip_grad_norm_(self.state.model.parameters(), self.gradient_clip_val)
+            self.callbacks.on_after_backward()
 
+            # everything else only before making step
+            if self.state.step % self.state.accumulate_steps == 0:
                 self.state.grad_scaler.step(self.state.optimizer)
                 self.state.grad_scaler.update()
                 self.state.optimizer.zero_grad()
             torch.cuda.synchronize()
 
         # Update loss
         self.state.loss_meter.update(to_numpy(loss))
@@ -112,14 +118,16 @@
             metric.reset()
         self.state.epoch_size = steps or len(loader)  # steps overwrites len
         self.callbacks.on_loader_begin()
         with torch.set_grad_enabled(self.state.is_train):
             for i, batch in enumerate(loader):
                 if i == self.state.epoch_size:
                     break
+                # step resets each epoch
                 self.state.step = i
+                self.state.global_sample_step += self.state.batch_size * self.state.world_size
                 self.state.input = batch
                 self.callbacks.on_batch_begin()
                 self._make_step()
                 self.callbacks.on_batch_end()
         self.callbacks.on_loader_end()
         return
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/callbacks.py` & `pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/callbacks.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,48 @@
 import os
 import math
 import numpy as np
 from tqdm import tqdm
 from enum import Enum
+from loguru import logger
 from copy import deepcopy
+from typing import Optional, Tuple, Dict, List
+from dataclasses import dataclass
 from collections import OrderedDict
 from collections import defaultdict
+from collections.abc import Iterable
 
 import torch
 from torch.cuda import amp
+from torch.nn.parallel import DistributedDataParallel
 
-from pytorch_tools.fit_wrapper.state import RunnerState
-import pytorch_tools.utils.misc as utils
+from .state import RunnerState
+from .utils import listify, to_numpy, env_rank, AverageMeter, TimeMeter
 from pytorch_tools.utils.visualization import plot_confusion_matrix
 from pytorch_tools.utils.visualization import render_figure_to_tensor
 from pytorch_tools.utils.tensorboard import CorrectedSummaryWriter as SummaryWriter
 
 
 class Callback(object):
     """
     Abstract class that all callback(e.g., Logger) classes extends from.
     Must be extended before usage.
     usage example:
     begin
     ---epoch begin (one epoch - one run of every loader)
-    ------loader begin 
+    ------loader begin
     ---------batch begin
+    ---------on_after_backward
     ---------batch end
-    ------loader end 
+    ------loader end
     ---epoch end
     end
     """
 
-    def __init__(self):
+    def __init__(self, *args, **kwargs):
         self.state = RunnerState()
 
     def set_state(self, state):
         self.state = state
 
     def on_batch_begin(self):
         pass
@@ -58,21 +64,25 @@
 
     def on_begin(self):
         pass
 
     def on_end(self):
         pass
 
+    def on_after_backward(self):
+        """Called after ``loss.backward()`` but before optimizer does anything."""
+        pass
+
 
 class Callbacks(Callback):
     """Class that combines multiple callbacks into one. For internal use only"""
 
     def __init__(self, callbacks):
         super().__init__()
-        self.callbacks = utils.listify(callbacks)
+        self.callbacks = listify(callbacks)
 
     def set_state(self, state):
         for callback in self.callbacks:
             callback.set_state(state)
 
     def on_batch_begin(self):
         for callback in self.callbacks:
@@ -102,39 +112,52 @@
         for callback in self.callbacks:
             callback.on_begin()
 
     def on_end(self):
         for callback in self.callbacks:
             callback.on_end()
 
+    def on_after_backward(self):
+        for callback in self.callbacks:
+            callback.on_after_backward()
+
+
+def rank_zero_only(cls: Callback) -> Callback:
+    """Returns Identity callback if rank != zero. supports wrapping a class and an instance"""
+    is_rank_zero = env_rank() == 0
+    if isinstance(cls, type):  # cls is a class
+        return cls if is_rank_zero else Callback
+    else:  # cls is an instance of some Callback
+        return cls if is_rank_zero else Callback()
+
 
 class BatchMetrics(Callback):
     """
     Computes metrics values after each batch
     Args:
         metrics (List): Metrics to measure during training. All metrics
             must have `name` attribute.
     """
 
     def __init__(self, metrics):
         super().__init__()
-        self.metrics = utils.listify(metrics)
+        self.metrics = listify(metrics)
         self.metric_names = [m.name for m in self.metrics]
 
     def on_begin(self):
         for name in self.metric_names:
-            self.state.metric_meters[name] = utils.AverageMeter(name=name)
+            self.state.metric_meters[name] = AverageMeter(name=name)
 
     @torch.no_grad()
     def on_batch_end(self):
         _, target = self.state.input
         output = self.state.output
         with amp.autocast(self.state.use_fp16):
             for metric, name in zip(self.metrics, self.metric_names):
-                self.state.metric_meters[name].update(utils.to_numpy(metric(output, target).squeeze()))
+                self.state.metric_meters[name].update(to_numpy(metric(output, target).squeeze()))
 
 
 class LoaderMetrics(Callback):
     """
     Computes metrics values after running full loader
     Args:
         metrics (List): Metrics to measure during training. All metrics
@@ -142,23 +165,23 @@
         update_steps (int): how ofter to recompute
         recompute_each_batch: Flag to compute metrics after each batch.
             Can be slow.
     """
 
     def __init__(self, metrics):
         super().__init__()
-        self.metrics = utils.listify(metrics)
+        self.metrics = listify(metrics)
         self.metric_names = [m.name for m in self.metrics]
 
         self.target = None
         self.output = None
 
     def on_begin(self):
         for name in self.metric_names:
-            self.state.metric_meters[name] = utils.AverageMeter(name=name)
+            self.state.metric_meters[name] = AverageMeter(name=name)
 
     def on_loader_begin(self):
         self.target = []
         self.output = []
 
     def on_batch_end(self):
         _, target = self.state.input
@@ -168,27 +191,28 @@
     @torch.no_grad()
     def on_loader_end(self):
 
         target = torch.cat(self.target)
         output = torch.cat(self.output)
         with amp.autocast(self.state.use_fp16):
             for metric, name in zip(self.metrics, self.metric_names):
-                self.state.metric_meters[name].update(utils.to_numpy(metric(output, target).squeeze()))
+                self.state.metric_meters[name].update(to_numpy(metric(output, target).squeeze()))
 
 
+@rank_zero_only
 class Timer(Callback):
     """
     Profiles first epoch and prints time spend on data loader and on model.
     Usefull for profiling dataloader code performance
     """
 
     def __init__(self):
         super().__init__()
         self.has_printed = False
-        self.timer = utils.TimeMeter()
+        self.timer = TimeMeter()
 
     def on_batch_begin(self):
         self.timer.batch_start()
 
     def on_batch_end(self):
         self.timer.batch_end()
 
@@ -196,111 +220,107 @@
         self.timer.reset()
 
     def on_loader_end(self):
         if not self.has_printed:
             self.has_printed = True
             d_time = self.timer.data_time.avg_smooth
             b_time = self.timer.batch_time.avg_smooth
-            self.state.logger.info(f"TimeMeter profiling. Data time: {d_time:.2E}s. Model time: {b_time:.2E}s \n")
+            logger.info(f"TimeMeter profiling. Data time: {d_time:.2E}s. Model time: {b_time:.2E}s \n")
+
+
+@dataclass
+class DataStage:
+    # start and end epoch for current stage
+    start: int = 0
+    end: int = 1
+    lr: "Optional[ (float, float) | float ]" = 1
+    lr_mode: Optional[str] = "linear"
+    # not processed by `PhasesScheduler` but allows more advanced logic
+    extra_args: Optional[Dict] = None
+
+    def __post_init__(self):
+        # will pass for list, typle, omegaconf.listconfig
+        if not isinstance(self.lr, Iterable):
+            self.lr = [self.lr, self.lr]
+        assert self.start < self.end, "start > end in stages"
 
 
 class PhasesScheduler(Callback):
     """
     Scheduler that uses `phases` to process updates.
     Supported `mode`'s are {`linear`, `cos`, `poly`}
+    NOTE: loss specified in phases would be multiplied by original loss in param groups
 
     Args:
-        phases (List[Dict]): phases
-        change_every (int): how often to actually change the lr. changing too 
-            often may slowdown the training
+        phases (List[DataStage]): phases
+        change_every (int): how often to actually change the lr. changing too often may slowdown the training
 
     Example:
         PHASES = [
-            {"ep":[0,8],  "lr":[0,0.1], "mom":0.9, },
-            {"ep":[8,24], "lr":[0.1, 0.01], "mode":"cos"},
-            {'ep':[24, 30], "lr": 0.001},
+            {"start": 0, "end":8, "lr":[0,0.1]},
+            {"start": 8, "end": 24, "lr":[0.1, 0.01], "lr_mode":"cos"},
+            {"start": 24, "end": 30, "lr": 0.001},
         ]
     """
 
-    def __init__(self, phases, change_every=50):
+    def __init__(self, phases: List[DataStage], change_every=50):
+        if type(phases[0]) != DataStage:
+            phases = [DataStage(**ph) for ph in phases]
+
+        self.phases = phases
         self.change_every = change_every
         self.current_lr = None
-        self.current_mom = None
-        self.phases = [self._format_phase(p) for p in phases]
+        self.tot_epochs = max([p.end for p in phases])
         self.phase = self.phases[0]
-        self.tot_epochs = max([max(p["ep"]) for p in self.phases])
         super(PhasesScheduler, self).__init__()
 
-    def _format_phase(self, phase):
-        phase["ep"] = utils.listify(phase["ep"])
-        phase["lr"] = utils.listify(phase["lr"])
-        phase["mom"] = utils.listify(phase.get("mom", None))  # optional
-        if len(phase["lr"]) == 2 or len(phase["mom"]) == 2:
-            phase["mode"] = phase.get("mode", "linear")
-            assert len(phase["ep"]) == 2, "Linear learning rates must contain end epoch"
-        return phase
-
     @staticmethod
-    def _schedule(start, end, pct, mode):
+    def _schedule(start: int, end: int, pct: float, mode: str):
         """anneal from `start` to `end` as pct goes from 0.0 to 1.0."""
         if mode == "linear":
             return start + (end - start) * pct
         elif mode == "cos":
             return end + (start - end) / 2 * (math.cos(math.pi * pct) + 1)
         elif mode == "poly":
             gamma = (end / start) ** (1 / 100)
             return start * gamma ** (pct * 100)
         else:
             raise ValueError(f"Mode: `{mode}` is not supported in PhasesScheduler")
 
-    def _get_lr_mom(self, batch_curr):
+    def _get_lr(self, batch_curr: int) -> float:
         phase = self.phase
         batch_tot = self.state.epoch_size
-        if len(phase["ep"]) == 1:
-            perc = 0
-        else:
-            ep_start, ep_end = phase["ep"]
-            ep_curr, ep_tot = self.state.epoch - ep_start, ep_end - ep_start
-            perc = (ep_curr * batch_tot + batch_curr) / (ep_tot * batch_tot)
-        if len(phase["lr"]) == 1:
-            new_lr = phase["lr"][0]  # constant learning rate
-        else:
-            lr_start, lr_end = phase["lr"]
-            new_lr = self._schedule(lr_start, lr_end, perc, phase["mode"])
-
-        if len(phase["mom"]) == 0:
-            new_mom = self.current_mom
-        elif len(phase["mom"]) == 1:
-            new_mom = phase["mom"][0]
-        else:
-            mom_start, mom_end = phase["mom"]
-            new_mom = self._schedule(mom_start, mom_end, perc, phase["mode"])
+        ep_curr, ep_tot = self.state.epoch - phase.start, phase.end - phase.start
+        perc = (ep_curr * batch_tot + batch_curr) / ((ep_tot + 1) * batch_tot)
+        assert perc <= 1 and perc >= 0
+        lr_start, lr_end = phase.lr  # may be the same
+        new_lr = self._schedule(lr_start, lr_end, perc, phase.lr_mode)
+        return new_lr
 
-        return new_lr, new_mom
+    def on_begin(self):
+        self.original_lr = [pg.get("lr", 1) for pg in self.state.optimizer.param_groups]
 
     def on_epoch_begin(self):
         new_phase = None
         for phase in reversed(self.phases):
-            if self.state.epoch >= phase["ep"][0]:
+            if self.state.epoch >= phase.start:
                 new_phase = phase
                 break
-        if new_phase is None:
-            raise Exception("Epoch out of range")
+        if new_phase is None or self.state.epoch > phase.end:
+            raise ValueError("Epoch out of range")
         else:
             self.phase = new_phase
 
     def on_batch_begin(self):
-        lr, mom = self._get_lr_mom(self.state.step)
-        if (self.current_lr == lr and self.current_mom == mom) or (self.state.step % self.change_every != 0):
+        lr = self._get_lr(self.state.step)
+        if self.current_lr == lr or (self.state.step % self.change_every != 0):
             return
         self.current_lr = lr
-        self.current_mom = mom
-        for param_group in self.state.optimizer.param_groups:
-            param_group["lr"] = lr
-            param_group["momentum"] = mom
+        for orig_lr, param_group in zip(self.original_lr, self.state.optimizer.param_groups):
+            param_group["lr"] = lr * orig_lr
 
 
 class ReduceMode(Enum):
     MIN = "min"
     MAX = "max"
 
 
@@ -337,29 +357,30 @@
         if self.monitor_op(current, self.best):
             self._steps_since_best = 0
         elif self._steps_since_best > self.patience:
             for param_group in self.state.optimizer.param_groups:
                 if param_group["lr"] * self.factor > self.min_lr:
                     param_group["lr"] *= self.factor
             if self.verbose:
-                self.state.logger.info(f"ReduceLROnPlateau reducing learning rate to {param_group['lr'] * self.factor}")
+                logger.info(f"ReduceLROnPlateau reducing learning rate to {param_group['lr'] * self.factor}")
 
     def get_monitor_value(self):
         value = None
         if self.monitor == "loss":
             value = self.state.loss_meter.avg
         else:
             for name, metric_meter in self.state.metric_meters.items():
                 if name == self.monitor:
                     value = metric_meter.avg
         if value is None:
             raise ValueError(f"ReduceLROnPlateau can't find {self.monitor} value to monitor")
         return value
 
 
+@rank_zero_only
 class CheckpointSaver(Callback):
     """
     Save best model every epoch based on loss
 
     Args:
         save_dir (str): path to folder where to save the model
         save_name (str): name of the saved model. can additionally
@@ -400,17 +421,15 @@
         os.makedirs(self.save_dir, exist_ok=True)
 
     def on_epoch_end(self):
         current = self.get_monitor_value()
         if self.monitor_op(current, self.best):
             ep = self.state.epoch_log
             if self.verbose:
-                self.state.logger.info(
-                    f"Epoch {ep:2d}: best {self.monitor} improved from {self.best:.4f} to {current:.4f}"
-                )
+                logger.info(f"Epoch {ep:2d}: best {self.monitor} improved from {self.best:.4f} to {current:.4f}")
             self.best = current
             save_name = os.path.join(self.save_dir, self.save_name.format(ep=ep, metric=current))
             self._save_checkpoint(save_name)
 
     def _save_checkpoint(self, path):
         if hasattr(self.state.model, "module"):  # used for saving DDP models
             state_dict = self.state.model.module.state_dict()
@@ -430,114 +449,110 @@
                 if name == self.monitor:
                     value = metric_meter.avg
         if value is None:
             raise ValueError(f"CheckpointSaver can't find {self.monitor} value to monitor")
         return value
 
 
+@rank_zero_only
 class TensorBoard(Callback):
     """
     Saves training and validation statistics for TensorBoard
 
     Args:
         log_dir (str): path where to store logs
-        log_every (int): how often to write logs during training
+        log_every (int): how often (in batches) to write logs during training
     """
 
-    def __init__(self, log_dir, log_every=20):
+    def __init__(self, log_dir=None, log_every=20):
         super().__init__()
         self.log_dir = log_dir
         self.log_every = log_every
-        self.writer = None
-        self.current_step = 0
 
     def on_begin(self):
+        if self.state.tb_logger is not None:
+            return
         os.makedirs(self.log_dir, exist_ok=True)
-        self.writer = SummaryWriter(self.log_dir)
+        self.state.tb_logger = SummaryWriter(self.log_dir)
 
     def on_batch_end(self):
-        self.current_step += self.state.batch_size
-        if self.state.is_train and (self.current_step % self.log_every == 0):
+        if self.state.is_train and (self.state.step % self.log_every == 0):
             # TODO: select better name instead of train_ ?
-            self.writer.add_scalar("train_/loss", self.state.loss_meter.val, self.current_step)
+            self.state.tb_logger.add_scalar(
+                "train_/loss", self.state.loss_meter.avg_smooth, self.state.global_sample_step
+            )
             for name, metric in self.state.metric_meters.items():
-                self.writer.add_scalar(f"train_/{name}", metric.val, self.current_step)
+                self.state.tb_logger.add_scalar(f"train_/{name}", metric.avg_smooth, self.state.global_sample_step)
 
     def on_epoch_end(self):
-        self.writer.add_scalar("train/loss", self.state.train_loss.avg, self.current_step)
+        self.state.tb_logger.add_scalar("train/loss", self.state.train_loss.avg, self.state.global_sample_step)
         for name, metric in self.state.train_metrics.items():
-            self.writer.add_scalar(f"train/{name}", metric.avg, self.current_step)
+            self.state.tb_logger.add_scalar(f"train/{name}", metric.avg, self.state.global_sample_step)
 
         lr = sorted([pg["lr"] for pg in self.state.optimizer.param_groups])[-1]  # largest lr
-        self.writer.add_scalar("train_/lr", lr, self.current_step)
-        self.writer.add_scalar("train/epoch", self.state.epoch, self.current_step)
+        self.state.tb_logger.add_scalar("train_/lr", lr, self.state.global_sample_step)
+        self.state.tb_logger.add_scalar("train/epoch", self.state.epoch, self.state.global_sample_step)
         # don't log if no val
         if self.state.val_loss is None:
             return
 
-        self.writer.add_scalar("val/loss", self.state.val_loss.avg, self.current_step)
+        self.state.tb_logger.add_scalar("val/loss", self.state.val_loss.avg, self.state.global_sample_step)
         for name, metric in self.state.val_metrics.items():
-            self.writer.add_scalar(f"val/{name}", metric.avg, self.current_step)
+            self.state.tb_logger.add_scalar(f"val/{name}", metric.avg, self.state.global_sample_step)
 
     def on_end(self):
-        self.writer.close()
+        self.state.tb_logger.close()
 
 
-class TensorBoardWithCM(TensorBoard):
+class TensorBoardCM(Callback):
     """
-    Saves training and validation statistics for TensorBoard
-    And also saves Confusion Matrix as image
+    Saves training and validation Confusion Matrix as image
 
     Args:
-        log_dir (str): path where to store logs
-        log_every (int): how often to write logs during training
         class_namess (List[str]): list of class names for proper visualization
     """
 
-    def __init__(self, log_dir, log_every=20, class_names=None):
-        super().__init__(log_dir, log_every)
+    def __init__(self, class_names=None):
         self.class_names = class_names
         self.n_classes = None  # will infer implicitly later
         self.cmap = None
         self.train_cm_img = None
         self.val_cm_img = None
 
     def on_batch_end(self):
-        super().on_batch_end()
         if self.cmap is None:
             self.n_classes = self.state.output.shape[1]
             self.cmap = np.zeros((self.n_classes, self.n_classes), dtype=int)
             if self.class_names is None:
                 self.class_names = [str(i) for i in range(self.n_classes)]
 
         target = self.state.input[1]
         if len(target.shape) == 2:
             target = target.argmax(1)
         predict = self.state.output.argmax(1)
         for tr, pr in zip(target, predict):
             self.cmap[tr, pr] += 1
 
     def on_loader_end(self):
-        super().on_loader_end()
         f = plot_confusion_matrix(self.cmap, self.class_names, normalize=True, show=False)
         cm_img = render_figure_to_tensor(f)
         if self.state.is_train:
             self.train_cm_img = cm_img
         else:
             self.val_cm_img = cm_img
         self.cmap = None
 
     def on_epoch_end(self):
-        super().on_epoch_end()
         if self.train_cm_img is not None:
-            self.writer.add_image("train/confusion_matrix", self.train_cm_img, self.current_step)
+            self.state.tb_logger.add_image("train/confusion_matrix", self.train_cm_img, self.state.global_sample_step)
         if self.val_cm_img is not None:
-            self.writer.add_image("val/confusion_matrix", self.val_cm_img, self.current_step)
+            self.state.tb_logger.add_image("val/confusion_matrix", self.val_cm_img, self.state.global_sample_step)
 
 
+@rank_zero_only
 class ConsoleLogger(Callback):
     """Prints training progress to console for monitoring."""
 
     def on_loader_begin(self):
         if hasattr(tqdm, "_instances"):  # prevents many printing issues
             tqdm._instances.clear()
         stage_str = "train" if self.state.is_train else "validat"
@@ -550,42 +565,97 @@
         desc.update({name: f"{m.avg:.3f}" for (name, m) in self.state.metric_meters.items()})
         self.pbar.set_postfix(**desc)
         self.pbar.update()
         self.pbar.close()
 
     def on_batch_end(self):
         desc = OrderedDict({"Loss": f"{self.state.loss_meter.avg_smooth:.4f}"})
-        desc.update({name: f"{m.avg_smooth:.3f}" for (name, m) in self.state.metric_meters.items()})
+        desc.update({name: f"{m.avg:.3f}" for (name, m) in self.state.metric_meters.items()})
         self.pbar.set_postfix(**desc)
         self.pbar.update()
 
 
 class FileLogger(Callback):
-    """Logs loss and metrics every epoch. 
+    """Logs loss and metrics every epoch.
     You have to manually configure loguru.logger to enable actual logging to file"""
 
     def on_epoch_begin(self):
-        self.state.logger.info(f"Epoch {self.state.epoch_log} | lr {self.current_lr:.2e}")
+        logger.info(f"Epoch {self.state.epoch_log} | lr {self.current_lr:.2e}")
 
     def on_epoch_end(self):
         loss, metrics = self.state.train_loss, self.state.train_metrics
-        self.state.logger.info("Train " + self._format_meters(loss, metrics))
+        logger.info("Train " + self._format_meters(loss, metrics))
         if self.state.val_loss is not None:
             loss, metrics = self.state.val_loss, self.state.val_metrics
-            self.state.logger.info("Val   " + self._format_meters(loss, metrics))
+            logger.info("Val   " + self._format_meters(loss, metrics))
 
     @property
     def current_lr(self):
         return sorted([pg["lr"] for pg in self.state.optimizer.param_groups])[-1]
 
     @staticmethod
     def _format_meters(loss, metrics):
         return f"loss: {loss.avg:.4f} | " + " | ".join(f"{m.name}: {m.avg:.4f}" for m in metrics.values())
 
 
+class GradientClipping(Callback):
+    """Clips gradients by max norm"""
+
+    def __init__(self, gradient_clip_val):
+        self.gradient_clip_val = gradient_clip_val
+        assert gradient_clip_val > 0, "Invalid value for gradient clipping"
+
+    def on_after_backward(self):
+        if self.state.step % self.state.accumulate_steps != 0:
+            return
+        self.state.grad_scaler.unscale_(self.state.optimizer)
+        torch.nn.utils.clip_grad_norm_(self.state.model.parameters(), self.gradient_clip_val)
+
+
+class AdaptiveGradientClipping(Callback):
+    """Clips gradient based on max norm.
+
+    Ref:
+        High-Performance Large-Scale Image Recognition Without Normalization
+        Official JAX impl (paper authors): https://github.com/deepmind/deepmind-research/tree/master/nfnets
+        Phil Wang's PyTorch gist: https://gist.github.com/lucidrains/0d6560077edac419ab5d3aa29e674d5c
+        Timm code: https://github.com/rwightman/pytorch-image-models/blob/master/timm/utils/agc.py
+    """
+
+    def __init__(self, clip_factor, eps=1e-3):
+        self.clip_factor = clip_factor
+        self.eps = eps
+
+    @staticmethod
+    def _unitwise_norm(x, norm_type=2.0):
+        if x.ndim <= 1:
+            return x.norm(norm_type)
+        else:
+            # works for nn.ConvNd and nn,Linear where output dim is first in the kernel/weight tensor
+            # might need special cases for other weights (possibly MHA) where this may not be true
+            return x.norm(norm_type, dim=tuple(range(1, x.ndim)), keepdim=True)
+
+    def on_after_backward(self):
+        if self.state.step % self.state.accumulate_steps != 0:
+            return
+
+        self.state.grad_scaler.unscale_(self.state.optimizer)
+
+        for p in self.state.model.parameters():
+            if p.grad is None:
+                continue
+            p_data = p.detach()
+            g_data = p.grad.detach()
+            max_norm = self._unitwise_norm(p_data).clamp_(min=self.eps).mul_(self.clip_factor)
+            grad_norm = self._unitwise_norm(g_data)
+            clipped_grad = g_data * (max_norm / grad_norm.clamp(min=1e-6))
+            new_grads = torch.where(grad_norm < max_norm, g_data, clipped_grad)
+            p.grad.detach().copy_(new_grads)
+
+
 class Mixup(Callback):
     """Performs mixup on input. Only for classification.
     Mixup blends two images by linear interpolation between them with small
     lambda drown from Beta distribution. Labels become a liner blend of true labels for
     original images.
     Ref: https://arxiv.org/abs/1710.09412
     According to https://arxiv.org/abs/2001.06268 mixing images from different batches give better results
@@ -645,14 +715,17 @@
         self.num_classes = num_classes
         self.prob = prob
         self.prev_input = None
 
     def on_batch_begin(self):
         self.state.input = self.cutmix(*self.state.input)
 
+    def on_loader_begin(self):
+        self.prev_input = None  # avoid leak from test to train
+
     @torch.no_grad()
     def cutmix(self, data, target):
         if target.dim() == 1:  # if not one hot
             target_one_hot = torch.zeros(target.size(0), self.num_classes, dtype=torch.float, device=data.device)
             target_one_hot.scatter_(1, target.unsqueeze(1), 1.0)
         else:
             target_one_hot = target
@@ -670,15 +743,15 @@
         lam = (bbh2 - bbh1) * (bbw2 - bbw1) / (H * W)
         data[:, :, bbh1:bbh2, bbw1:bbw2] = prev_data[perm, :, bbh1:bbh2, bbw1:bbw2]
         mixed_target = (1 - lam) * target_one_hot + lam * prev_target[perm]
         return data, mixed_target
 
     @staticmethod
     def rand_bbox(H, W, lam):
-        """ returns bbox with area close to lam*H*W """
+        """returns bbox with area close to lam*H*W"""
         cut_rat = np.sqrt(lam)
         cut_h = np.int(H * cut_rat)
         cut_w = np.int(W * cut_rat)
         # uniform
         ch = np.random.randint(H)
         cw = np.random.randint(W)
         bbh1 = np.clip(ch - cut_h // 2, 0, H)
@@ -728,17 +801,17 @@
     def on_epoch_end(self):
         current_rate = self.drop_rate * min(1, self.state.epoch / self.epochs)
         setattr(self.state.model, self.attr_name, current_rate)
 
 
 class ResetOptimizer(Callback):
     """Set's Optimizers state to empty for epoch in `reset_epoch`. Could be used for restarts.
-        Args:
-            reset_epoch (List[int]): after which epochs to reset optimizer
-            verbose (bool): Flag to print that optimizer was reset."""
+    Args:
+        reset_epoch (List[int]): after which epochs to reset optimizer
+        verbose (bool): Flag to print that optimizer was reset."""
 
     def __init__(self, reset_epochs=[], verbose=True):
         super().__init__()
         self.reset_epochs = set(reset_epochs)
         self.verbose = verbose
 
     def on_epoch_end(self):
@@ -746,66 +819,74 @@
             # any optimizer inherited from torch.Optimizer has state which can be reset
             if hasattr(self.state.optimizer, "optimizer"):  # for lookahead
                 self.state.optimizer.optimizer.state = defaultdict(dict)
             else:
                 self.state.optimizer.state = defaultdict(dict)
 
             if self.verbose:
-                self.state.logger.info("Reseting optimizer")
+                logger.info("Reseting optimizer")
 
 
 # docstring from https://github.com/rwightman/pytorch-image-models
 class ModelEma(Callback):
-    """ Model Exponential Moving Average
+    """Model Exponential Moving Average
     Keeps a moving average of everything in the model state_dict (parameters and buffers).
     This is intended to allow functionality like
     https://www.tensorflow.org/api_docs/python/tf/train/ExponentialMovingAverage
 
     A smoothed version of the weights is necessary for some training schemes to perform well.
     E.g. Google's hyper-params for training MNASNet, MobileNet-V3, EfficientNet, etc that use
     RMSprop with a short 2.4-3 epoch decay period and slow LR decay rate of .96-.99 requires EMA
-    smoothing of weights to match results. 
-    
+    smoothing of weights to match results.
+
     Current implementation follows TensorFlow and uses the following formula:
     ema -= (1 - decay) * (ema - model)
     This is mathematically equivalent to the classic formula below but inplace is faster
     ema = decay * ema + (1 - decay) * model
 
     NOTE: Pay attention to the decay constant you are using relative to your update count per epoch.
-    
+
     NOTE: put this Callback AFTER Checkpoint saver! Otherwise you would validate EMA weights but save
     model weights
 
     NOTE: Need to be used in all process (not only master)! otherwise you would save not the best model bur some random
 
     NOTE: Pass model to ModelEma after cuda() and AMP but before SyncBN and DDP wrapper
 
     Args:
         model (nn.Module): model after cuda and AMP
         decay (float): decay for EMA for every step
-        decay_every (int): how oftern to really decay weights. Decaying every step produced a 
+        decay_every (int): how oftern to really decay weights. Decaying every step produced a
             visible training slowdown. Real decay factor is adjusted to match every step update.
     """
 
-    def __init__(self, model, decay=0.9999, decay_every=10):
+    def __init__(self, decay=0.9999, decay_every=10):
         super().__init__()
-        self.ema = deepcopy(model).eval()
-        for p in self.ema.parameters():
-            p.requires_grad_(False)
+        assert isinstance(decay, float), "Decay in EMA should be float"
+        self.ema = None
         self.model_copy = None
-        self.decay_factor = 1 - decay ** decay_every  # simulate every step decay
+        self.decay_factor = 1 - decay**decay_every  # simulate every step decay
         self.decay_every = decay_every
 
+    def on_begin(self):
+        if self.ema is not None:
+            return
+        model = self.state.model
+        if isinstance(self.state.model, DistributedDataParallel):
+            model = model.module
+        self.ema = deepcopy(model).eval().requires_grad_(False)
+        self.state.communication_dict["ema_model"] = self.ema
+
     def on_batch_end(self):
         if not self.state.is_train or (self.state.step % self.decay_every != 0):
             return
 
         with torch.no_grad():
             for (ema_v, m_v) in zip(self.ema.state_dict().values(), self.state.model.state_dict().values()):
-                if m_v.numel() == 1:  # to prevent errors on `num_batches_tracked` in BN
+                if m_v.dtype == torch.long:  # to prevent errors on `num_batches_tracked` in BN
                     continue
                 ema_v.sub_(ema_v.sub(m_v), alpha=self.decay_factor)
 
     def on_loader_begin(self):
         if self.state.is_train:
             return
         # validate on ema model
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/fit_wrapper/README.md` & `pytorch_tools-0.5.1/pytorch_tools/fit_wrapper/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 # Overview
-This module contains model runner (very close to `model.fit` in Keras) for **supervised** tasks.  
-`Runner` is used to actually run the train loop calling `Callbacks` at appropriate times.  
+This module contains model runner (very close to `model.fit` in Keras) for **supervised** tasks.
+`Runner` is used to actually run the train loop calling `Callbacks` at appropriate times.
 Mixed precision is also supported. Pass `use_fp16` to Runner to enable it. No more changes are required.
 
-Main idea of this runner is to be as simple as possible. All core functionality is ~100 lines of code.  
+Main idea of this runner is to be as simple as possible. All core functionality is ~100 lines of code.
 
 ## Minimal example
 This code will run training for 5 epochs.
 ```python
 from pytorch_tools.fit_wrapper import Runner
 model = ... (any model)
 optimizer = ... (any optimizer)
 criterions = ... (any loss function)
 metrics = ... (any metrics or None)
 train_loader = ... (dataloader with defined __len__)
 runner = Runner(model, optimizer, criterion, metrics)
 runner.fit(train_loader, epochs=5)
 ```
 
-## Real example 
-This code will run training for 5 epochs in mixed precision with validation every epoch. 
-* `Timer` will measure performance of your dataloader in comparison to model time. 
-* `ConsoleLogger` will print training logs to console. 
-* `TensorBoard` will log training loss and metrics to TensorBoard. 
+## Real example
+This code will run training for 5 epochs in mixed precision with validation every epoch.
+* `Timer` will measure performance of your dataloader in comparison to model time.
+* `ConsoleLogger` will print training logs to console.
+* `TensorBoard` will log training loss and metrics to TensorBoard.
 * `CheckpointSaver` will save best model according to validation loss.
 ```python
 import pytorch_tools as pt
 val_loader = ... (validation dataloader with defined __len__)
 runner = pt.fit_wrapper.Runner(
     model,
     optimizer,
@@ -41,15 +41,18 @@
     use_fp16=True,
 )
 runner.fit(train_loader, epochs=5, val_loader=val_loader)
 ```
 ## Distributed Training
 This runner is very simple and requires writing thin wrapper for DDP every time. The preferred (and the only tested way) of running distributed training is using
 `python3 -m torch.distributed.launch --nproc_per_node=$NUM_GPUS <your training code .py>`
-`torch.distributed.launch` implicitly sets environmental variables which code for callbacks relies on. Make sure to properly set `RANK` and `WORLD_SIZE`  
+`torch.distributed.launch` implicitly sets environmental variables which code for callbacks relies on. Make sure to properly set `RANK` and `WORLD_SIZE`
 
 ## How to
-### Add custom step logic  
-Monkey patch `Runner._make_step` function with yours  
+### Add custom step logic
+Monkey patch `Runner._make_step` function with yours
 
 ### Process multiple inputs/outputs
-Instead of modifying Runner move this logic inside Loss function.
+Instead of modifying Runner move this logic inside Loss function.
+
+### Limitations
+Currently trainer is well suited for supervised tasks. GANs e.t.c are not well supported...
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/wrapper.py` & `pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,46 +60,47 @@
             for f, arg in zip(self.backward_aug, args):
                 batch = f(batch, arg)
             transformed_batches.append(batch)
         return torch.cat(transformed_batches, 0)
 
 
 class TTA(nn.Module):
-    """Module wrapper for convinient TTA. 
+    """Module wrapper for convinient TTA.
     Wrapper add augmentation layers to your model like this:
 
             Input
               |           # input batch; shape B, H, W, C
          / / / \ \ \      # duplicate image for augmentation; shape N*B, H, W, C
         | | |   | | |     # apply augmentations (flips, rotation, shifts)
      your nn.Module model
         | | |   | | |     # reverse transformations (this part is skipped for classification)
          \ \ \ / / /      # merge predictions (mean, max, gmean)
               |           # output mask; shape B, H, W, C
             Output
-            
+
     Args:
-        model (nn.Module): 
+        model (nn.Module):
         segm (bool): Flag to revert augmentations before merging. Requires output of a model
             to be of the same size as input. Defaults to False.
         h_flip (bool): Horizontal flip.
         v_flip (bool): Vertical flip.
         h_shift (List[int]): list of horizontal shifts in pixels (e.g. [10, -10])
         v_shift (List[int]): list of vertical shifts in pixels (e.g. [10, -10])
         rotation (List[int]): list of angles (deg) for rotation should be divisible by 90 deg (e.g. [90, 180, 270])
         add (List[float]): list of floats to add to input images.
         mul (List[float]): list of float to multiply input. Ex: [0.9, 1.1]
-        merge (str): Mode of merging augmented predictions. One of 'mean', 'gmean' and 'max'. 
+        merge (str): Mode of merging augmented predictions. One of 'mean', 'gmean' and 'max'.
             When using 'gmean' option make sure that predictions are less than 1 or number of augs isn't too large
             otherwise it could lead to an overflow.
-        activation (str): Activation to apply to predictions before merging. One of {None, `sigmoid`, `softmax`}.  
-    
+        activation (str): Activation to apply to predictions before merging. One of {None, `sigmoid`, `softmax`}.
+
     Returns:
         nn.Module
     """
+
     def __init__(
         self,
         model,
         segm=False,
         h_flip=False,
         v_flip=False,
         h_shift=None,
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/functional.py` & `pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/functional.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/tta_wrapper/README.md` & `pytorch_tools-0.5.1/pytorch_tools/tta_wrapper/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Test Time Augmentation Wrapper
-This module wraps existing PyTorch model, performs inference on multiple augmented images and them merges the predictions into one. 
+This module wraps existing PyTorch model, performs inference on multiple augmented images and them merges the predictions into one.
 
 Wrapper adds augmentation layers to your model like this:
 ```
             Input
               |           # input batch; shape B, H, W, C
          / / / \ \ \      # duplicate image for augmentation; shape N*B, H, W, C
         | | |   | | |     # apply augmentations (flips, rotation, shifts)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/detection_models/efficientdet.py` & `pytorch_tools-0.5.1/pytorch_tools/detection_models/efficientdet.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,30 +19,30 @@
 from pytorch_tools.modules.residual import DepthwiseSeparableConv
 from pytorch_tools.modules.tf_same_ops import conv_to_same_conv
 from pytorch_tools.modules.tf_same_ops import maxpool_to_same_maxpool
 
 from pytorch_tools.segmentation_models.encoders import get_encoder
 
 import pytorch_tools.utils.box as box_utils
+from pytorch_tools.utils.misc import initialize
+from pytorch_tools.utils.misc import patch_bn_mom
 from pytorch_tools.utils.misc import DEFAULT_IMAGENET_SETTINGS
-from pytorch_tools.utils.misc import initialize_iterator
-from pytorch_tools.models.efficientnet import patch_bn_tf
 
 
 class EfficientDet(nn.Module):
     """
     Implementation of the EfficientDet Object Detection model
 
     Main difference from other implementations available are:
     * cleanest code. all model is defined in this file with only small modules
         imported from somewhere else
     * ability to freeze batch norm in encoder with one line
     * fast train speed and low memory consumption. partly due to memory efficient Swish
         partly due to heavy use of inplace operations
-    
+
     Args:
         pretrained (str): one of `coco` or None. if `coco` - load pretrained weights
         encoder_name (str): name of classification model (without last dense layers) used as feature
                 extractor to build detection model. It could be any model even `resnet`
         encoder_weights (str): one of ``None`` (random initialization), ``imagenet`` (pre-trained on ImageNet)
         pyramid_channels (int): size of features after BiFPN. Default 256
         num_fpn_layers (int): Number of BiFPN layers
@@ -55,15 +55,15 @@
         encoder_norm_act (str): Activation for normalization layer in encoder
         decoder_norm_layer (str): Normalization to use in head convolutions. Default (none) is not to use normalization.
                 Current implementation is optimized for `GroupNorm`, not `BatchNorm` check code for details
         decoder_norm_act (str): Activation for normalization layer in head convolutions
         match_tf_same_padding (bool): If True patches Conv and MaxPool to implements tf-like asymmetric padding
             Should only be used to validate pretrained weights. Not needed for training. Gives ~10% slowdown
         anchors_per_location (int): Number of anchors per feature map pixel. In fact it only affects the size of output
-        
+
     Ref:
         EfficientDet: Scalable and Efficient Object Detection - https://arxiv.org/abs/1911.09070
     """
 
     def __init__(
         self,
         pretrained="coco",  # Not used. here for proper signature
@@ -114,39 +114,34 @@
         # The convolution layers in the head are shared among all levels, but
         # each level has its batch normalization to capture the statistical
         # difference among different levels.
         def make_head_norm():
             return nn.ModuleList(
                 [
                     nn.ModuleList(
-                        [
-                            norm_layer(pyramid_channels, activation=decoder_norm_act)
-                            for _ in range(num_head_repeats)
-                        ]
+                        [norm_layer(pyramid_channels, activation=decoder_norm_act) for _ in range(num_head_repeats)]
                     )
                     for _ in range(5)
                 ]
             )
 
         self.cls_convs = make_head(num_classes * anchors_per_location)
         self.cls_head_conv = DepthwiseSeparableConv(
             pyramid_channels, num_classes * anchors_per_location, use_norm=False
         )
         self.cls_norms = make_head_norm()
 
         self.box_convs = make_head(4 * anchors_per_location)
-        self.box_head_conv = DepthwiseSeparableConv(
-            pyramid_channels, 4 * anchors_per_location, use_norm=False
-        )
+        self.box_head_conv = DepthwiseSeparableConv(pyramid_channels, 4 * anchors_per_location, use_norm=False)
         self.box_norms = make_head_norm()
 
         self.num_classes = num_classes
         self.num_head_repeats = num_head_repeats
 
-        patch_bn_tf(self)
+        patch_bn_mom(self, 0.01)
         self._initialize_weights()
         if match_tf_same_padding:
             conv_to_same_conv(self)
             maxpool_to_same_maxpool(self)
 
     # Name from mmdetectin for convenience
     def extract_features(self, x):
@@ -194,26 +189,26 @@
         box_outputs = box_outputs[..., [1, 0, 3, 2]]
         return class_outputs, box_outputs
 
     @torch.no_grad()
     def predict(self, x):
         """
         Run forward on given images and decode raw prediction into bboxes
-		Returns:
+                Returns:
             torch.Tensor with bboxes, scores and classes. bboxes in `lrtb` format
             shape [BS, MAX_DETECTION_PER_IMAGE, 6]
-		"""
+        """
         class_outputs, box_outputs = self.forward(x)
         anchors = box_utils.generate_anchors_boxes(x.shape[-2:])[0]
         return box_utils.decode(class_outputs, box_outputs, anchors)
 
     def _initialize_weights(self):
         # init everything except encoder
         no_encoder_m = [m for n, m in self.named_modules() if not "encoder" in n]
-        initialize_iterator(no_encoder_m)
+        initialize(no_encoder_m)
         # need to init last bias so that after sigmoid it's 0.01
         cls_bias_init = -torch.log(torch.tensor((1 - 0.01) / 0.01))  # -4.59
         nn.init.constant_(self.cls_head_conv[1].bias, cls_bias_init)
 
 
 PRETRAIN_SETTINGS = {**DEFAULT_IMAGENET_SETTINGS, "input_size": (512, 512), "crop_pct": 1, "num_classes": 90}
 
@@ -324,15 +319,16 @@
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
                 f"Using model pretrained for {cfg_settings['num_classes']} classes with {kwargs_cls} classes. Last layer is initialized randomly"
             )
             state_dict["cls_head_conv.1.weight"] = model.state_dict()[f"cls_head_conv.1.weight"]
             state_dict["cls_head_conv.1.bias"] = model.state_dict()["cls_head_conv.1.bias"]
-        model.load_state_dict(state_dict, strict=True)
+        # strict=False to avoid error on extra bias in BiFPN
+        model.load_state_dict(state_dict, strict=False)
     setattr(model, "pretrained_settings", cfg_settings)
     return model
 
 
 @wraps(EfficientDet)
 def efficientdet_d0(pretrained="coco", **kwargs):
     return _efficientdet("efficientdet_d0", pretrained, **kwargs)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/detection_models/retinanet.py` & `pytorch_tools-0.5.1/pytorch_tools/detection_models/retinanet.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,39 +7,39 @@
 
 from pytorch_tools.modules.fpn import FPN
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.modules.residual import conv3x3
 from pytorch_tools.segmentation_models.encoders import get_encoder
 import pytorch_tools.utils.box as box_utils
 from pytorch_tools.utils.misc import DEFAULT_IMAGENET_SETTINGS
-from pytorch_tools.utils.misc import initialize_iterator
+from pytorch_tools.utils.misc import initialize
 
 
 class RetinaNet(nn.Module):
-    """RetinaNet 
+    """RetinaNet
     Main difference from other implementations are:
     * support of any custom encoder from this repo
     * optional normalization layer in box classification head
     * ability to freeze batch norm in encoder with one line
-    
+
     Args:
-        pretrained (str): one of `coco` or None. if `coco` - load pretrained weights 
+        pretrained (str): one of `coco` or None. if `coco` - load pretrained weights
         encoder_name (str): name of classification model (without last dense layers) used as feature
             extractor to build detection model
         encoder_weights (str): one of ``None`` (random initialization), ``imagenet`` (pre-trained on ImageNet)
         pyramid_channels (int): size of features after FPN. Default 256
-        num_classes (int): a number of classes to predict 
+        num_classes (int): a number of classes to predict
             class_outputs shape is (BS, *, NUM_CLASSES) where each row in * corresponds to one bbox
         encoder_norm_layer (str): Normalization layer to use in encoder. If using pretrained
             it should be the same as in pretrained weights
         encoder_norm_act (str): Activation for normalization layer in encoder
-        decoder_norm_layer (str): Normalization to use in head convolutions. Default (none) is not to use normalization. 
+        decoder_norm_layer (str): Normalization to use in head convolutions. Default (none) is not to use normalization.
             Current implementation is optimized for `GroupNorm`, not `BatchNorm` check code for details
         decoder_norm_act (str): Activation for normalization layer in head convolutions
-    
+
     Ref:
         Focal Loss for Dense Object Detection - https://arxiv.org/abs/1708.02002
         Mmdetection - https://github.com/open-mmlab/mmdetection/ (at commit b9daf23)
         TF TPU version - https://github.com/tensorflow/tpu/tree/master/models/official/retinanet
     """
 
     def __init__(
@@ -127,15 +127,15 @@
         class_outputs, box_outputs = self.forward(x)
         anchors = box_utils.generate_anchors_boxes(x.shape[-2:])[0]
         return box_utils.decode(class_outputs, box_outputs, anchors)
 
     def _initialize_weights(self):
         # init everything except encoder
         no_encoder_m = [m for n, m in self.named_modules() if not "encoder" in n]
-        initialize_iterator(no_encoder_m)
+        initialize(no_encoder_m)
         # need to init last bias so that after sigmoid it's 0.01
         cls_bias_init = -torch.log(torch.tensor((1 - 0.01) / 0.01))  # -4.59
         nn.init.constant_(self.cls_head_conv.bias, cls_bias_init)
 
 
 # Don't really know input size for the models. 512 is just a guess
 PRETRAIN_SETTINGS = {**DEFAULT_IMAGENET_SETTINGS, "input_size": (512, 512), "crop_pct": 1, "num_classes": 80}
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/metrics/accuracy.py` & `pytorch_tools-0.5.1/pytorch_tools/metrics/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class Accuracy:
     """
     Accuracy with support for binary and multiclass classification.
     Also supports images
-    
+
     Args:
         y_pred (Tensor): raw logits of shape (N, C) or (N, C, H, W)
         y_true (Long Tensor): true classes of shape (N,) or one-hot encoded of shape (N, C)
             For images target should have shape (N, C, H, W) or (N, 1, H, W)
     """
 
     def __init__(self, topk=1):
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/metrics/psnr.py` & `pytorch_tools-0.5.1/pytorch_tools/metrics/psnr.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,18 +51,16 @@
         img1 = img1.astype(np.float64)
         img2 = img2.astype(np.float64)
         kernel = cv2.getGaussianKernel(11, 1.5)
         window = np.outer(kernel, kernel.transpose())
 
         mu1 = cv2.filter2D(img1, -1, window)[5:-5, 5:-5]  # valid
         mu2 = cv2.filter2D(img2, -1, window)[5:-5, 5:-5]
-        mu1_sq = mu1 ** 2
-        mu2_sq = mu2 ** 2
+        mu1_sq = mu1**2
+        mu2_sq = mu2**2
         mu1_mu2 = mu1 * mu2
-        sigma1_sq = cv2.filter2D(img1 ** 2, -1, window)[5:-5, 5:-5] - mu1_sq
-        sigma2_sq = cv2.filter2D(img2 ** 2, -1, window)[5:-5, 5:-5] - mu2_sq
+        sigma1_sq = cv2.filter2D(img1**2, -1, window)[5:-5, 5:-5] - mu1_sq
+        sigma2_sq = cv2.filter2D(img2**2, -1, window)[5:-5, 5:-5] - mu2_sq
         sigma12 = cv2.filter2D(img1 * img2, -1, window)[5:-5, 5:-5] - mu1_mu2
 
-        ssim_map = ((2 * mu1_mu2 + C1) * (2 * sigma12 + C2)) / (
-            (mu1_sq + mu2_sq + C1) * (sigma1_sq + sigma2_sq + C2)
-        )
+        ssim_map = ((2 * mu1_mu2 + C1) * (2 * sigma12 + C2)) / ((mu1_sq + mu2_sq + C1) * (sigma1_sq + sigma2_sq + C2))
         return ssim_map.mean()
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/metrics/dice_jaccard.py` & `pytorch_tools-0.5.1/pytorch_tools/metrics/dice_jaccard.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/hrnet.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/hrnet.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,30 @@
 import logging
 from copy import deepcopy
 from functools import wraps
 
 import torch
 import torch.nn as nn
-from torchvision.models.utils import load_state_dict_from_url
+from torch.hub import load_state_dict_from_url
 
 from pytorch_tools.modules.residual import conv1x1
 from pytorch_tools.modules.residual import conv3x3
 from pytorch_tools.modules import ABN
 from pytorch_tools.modules import InPlaceABN
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.modules.spatial_ocr_block import SpatialOCR
 from pytorch_tools.modules.spatial_ocr_block import SpatialOCR_Gather
 
 from pytorch_tools.utils.misc import initialize
 from pytorch_tools.utils.misc import repeat_channels
+from pytorch_tools.utils.misc import patch_bn_mom
 
 from .encoders import get_encoder
 
 
-def patch_bn_mom(module):
-    """changes default bn momentum"""
-    if isinstance(module, ABN) or isinstance(module, InPlaceABN):
-        module.momentum = 0.01
-    for m in module.children():
-        patch_bn_mom(m)
-
-
 def patch_inplace_abn(module):
     """changes weight from InplaceABN to be compatible with usual ABN"""
     if isinstance(module, ABN):
         module.weight = nn.Parameter(module.weight.abs() + 1e-5)
     for m in module.children():
         patch_inplace_abn(m)
 
@@ -41,23 +34,23 @@
     NOTE: for this model input size should be divisible by 32!
 
     Args:
         encoder_name (str): name of classification model used as feature extractor to build segmentation model.
         encoder_weights (str): one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
         num_classes (int): a number of classes for output (output shape - ``(batch, classes, h, w)``).
         pretrained (Union[str, None]): hrnet_w48 and hrnet_w48+OCR have pretrained weights. init models using functions rather than
-            from class to load them. Available options are: None, `cityscape` 
+            from class to load them. Available options are: None, `cityscape`
         last_upsample (bool): Flag to enable upsampling predictions to the original image size. If set to `False` prediction
             would be 4x times smaller than input image. Default True.
         drop_rate (float): Probability of spatial dropout on last feature map
-        OCR (bool): Flag to add object context block to the model. See `Ref` section for paper. 
+        OCR (bool): Flag to add object context block to the model. See `Ref` section for paper.
         norm_layer (str): Normalization layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory
             footprint. But increases backward time. Defaults to 'abn'.
         norm_act (str): Activation for normalizion layer. 'inplaceabn' doesn't support `ReLU` activation.
-    
+
     Ref:
         Deep High-Resolution Representation Learning for Visual Recognition: https://arxiv.org/abs/1908.07919
         Object-Contextual Representations for Semantic Segmentation: https://arxiv.org/abs/1909.11065
     """
 
     def __init__(
         self,
@@ -83,15 +76,16 @@
         )
         norm_layer = bn_from_name(norm_layer)
         final_channels = sum(self.encoder.out_shapes[:4])
 
         self.OCR = OCR
         if OCR:
             self.conv3x3 = nn.Sequential(
-                conv3x3(final_channels, 512, bias=True), norm_layer(512, activation=norm_act),
+                conv3x3(final_channels, 512, bias=True),
+                norm_layer(512, activation=norm_act),
             )
             self.ocr_gather_head = SpatialOCR_Gather()
             self.ocr_distri_head = SpatialOCR(
                 in_channels=512, key_channels=256, out_channels=512, norm_layer=norm_layer, norm_act=norm_act
             )
             self.head = conv1x1(512, num_classes, bias=True)
             self.aux_head = nn.Sequential(  # in OCR first conv is 3x3
@@ -168,15 +162,15 @@
             **SETTINGS,
         },
         "cityscape": {"url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.3/hrnet_w48_cityscapes_cls19_1024x2048_ohem_trainvalset_remapped.pth"},
     },
     "hrnet_w48_ocr": {
         "default": {
             "params": {"encoder_name": "hrnet_w48", "OCR": True},
-            "input_space": "BGR", # this weights were trained using cv2.imread 
+            "input_space": "BGR", # this weights were trained using cv2.imread
             "norm_layer": "inplace_abn",
             **SETTINGS,
         },
         "cityscape": {"url": "https://github.com/bonlime/pytorch-tools/releases/download/v0.1.3/hrnet_w48_ocr_1_latest_remapped.pth"},
     },
 }
 # fmt: on
@@ -187,17 +181,15 @@
     if pretrained:
         pretrained_settings = cfgs[arch][pretrained]
         pretrained_params = pretrained_settings.pop("params", {})
         cfg_settings.update(pretrained_settings)
         cfg_params.update(pretrained_params)
     common_args = set(cfg_params.keys()).intersection(set(kwargs.keys()))
     if common_args:
-        logging.warning(
-            f"Args {common_args} are going to be overwritten by default params for {pretrained} weights"
-        )
+        logging.warning(f"Args {common_args} are going to be overwritten by default params for {pretrained} weights")
     kwargs.update(cfg_params)
     model = HRNet(**kwargs)
     if pretrained:
         state_dict = load_state_dict_from_url(cfgs[arch][pretrained]["url"])
         kwargs_cls = kwargs.get("num_classes", None)
         if kwargs_cls and kwargs_cls != cfg_settings["num_classes"]:
             logging.warning(
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/linknet.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/linknet.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/segm_bifpn.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/segm_bifpn.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 This file defines segmentation model based on Efficient Det networks
 In paper they mention the following:
 
 `We modify our EfficientDet model to keep feature level {P2, P3, ..., P7} in BiFPN, but only use
-P2 for the final per-pixel classification. For ... B4 backbone ... we set the channel size to 128 
+P2 for the final per-pixel classification. For ... B4 backbone ... we set the channel size to 128
 for BiFPN and 256 for classification head. Both BiFPN and classification head are repeated by 3 times.`
 
 I only use features {P2, P3, P4, P5} because very often such large OS is not needed.
 """
 
 import torch
 import torch.nn as nn
@@ -16,15 +16,15 @@
 from pytorch_tools.modules.bifpn import BiFPN
 from pytorch_tools.modules import bn_from_name
 from pytorch_tools.modules.residual import conv1x1
 from pytorch_tools.modules.residual import DepthwiseSeparableConv
 from pytorch_tools.modules.tf_same_ops import conv_to_same_conv
 from pytorch_tools.modules.tf_same_ops import maxpool_to_same_maxpool
 
-from pytorch_tools.models.efficientnet import patch_bn_tf
+from pytorch_tools.utils.misc import patch_bn_mom
 from pytorch_tools.segmentation_models.encoders import get_encoder
 
 
 class SegmentationBiFPN(nn.Module):
     def __init__(
         self,
         encoder_name="efficientnet_b0",
@@ -64,15 +64,15 @@
             DepthwiseSeparableConv(head_channels, num_classes, use_norm=False),
         )
 
         self.upsample = nn.Upsample(scale_factor=4, mode="bilinear") if last_upsample else nn.Identity()
 
         self.num_classes = num_classes
 
-        patch_bn_tf(self)
+        patch_bn_mom(self, 0.01)
         # set last layer bias for better convergence with sigmoid loss
         # -4.59 = -np.log((1 - 0.01) / 0.01)
         nn.init.constant_(self.cls_head_conv[-1][1].bias, -4.59)
 
     def _initialize_weights(self):
         pass
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/encoders.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/encoders.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/segm_fpn.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/segm_fpn.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,31 +6,29 @@
 from pytorch_tools.modules.residual import conv1x1
 from pytorch_tools.modules.residual import conv3x3
 from pytorch_tools.modules.decoder import SegmentationUpsample
 from pytorch_tools.segmentation_models.encoders import get_encoder
 
 
 class PanopticDecoder(nn.Module):
-    """ Takes a feature pyramid, upscales the feature map to the same size and merges by sum or concatenation"""
+    """Takes a feature pyramid, upscales the feature map to the same size and merges by sum or concatenation"""
 
     def __init__(
         self,
         pyramid_channels=256,
         segmentation_channels=128,
         merge_policy="add",
         upsamples=[3, 2, 1, 0],
         **bn_args,
     ):
 
         super().__init__()
         self.seg_blocks = nn.ModuleList(
             [
-                SegmentationUpsample(
-                    pyramid_channels, segmentation_channels, n_upsamples=n_upsamples, **bn_args
-                )
+                SegmentationUpsample(pyramid_channels, segmentation_channels, n_upsamples=n_upsamples, **bn_args)
                 for n_upsamples in upsamples
             ]
         )
         self.policy = merge_policy
 
     def forward(self, features):
         c5, c4, c3, c2 = features
@@ -48,27 +46,27 @@
     Ref https://arxiv.org/pdf/1901.02446.pdf
 
     Args:
         encoder_name (str): name of classification model (without last dense layers) used as feature
             extractor to build segmentation model.
         encoder_weights (str): one of ``None`` (random initialization), ``imagenet`` (pre-training on ImageNet).
         pyramid_channels (int): Feature pyramid output channels. Defaults to 256.
-        num_fpn_layers (int): a number of layers in FPN module. Only supprted in SegmentationBiFPN 
+        num_fpn_layers (int): a number of layers in FPN module. Only supprted in SegmentationBiFPN
         segmentation_channels (int): Number of segmentation output channels. Defaults to 128.
         num_classes (int): a number of classes for output (output shape - ``(batch, classes, h, w)``).
         merge_policy (str): One of `add` of `cat`. `sum` would sum resulting feature maps.
             `cat` would concatenate them. Defaults to "add".
         last_upsample (bool): Flag to enable upsampling predictions to the original image size. If set to `False` prediction
             would be 4x times smaller than input image. Default True.
         output_stride (int): one of 32 or 16. Changes the model output stride and upsampling blocks accordingly
         drop_rate (float): Probability of spatial dropout on last feature map
         norm_layer (str): Normalization layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers memory
             footprint. But increases backward time. Defaults to 'abn'.
         norm_act (str): Activation for normalizion layer. 'inplaceabn' doesn't support `ReLU` activation.
-    
+
     """
 
     FEATURE_PYRAMID = FPN
 
     def __init__(
         self,
         encoder_name="resnet34",
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/deeplabv3_plus.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/deeplabv3_plus.py`

 * *Files identical despite different names*

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/unet.py` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/unet.py`

 * *Files 4% similar despite different names*

```diff
@@ -84,14 +84,15 @@
         decoder_attention_type (Union[str, None]): Attention to use in decoder layers. Options are:
             `se`, `sse`, `eca`, `scse`. Check code for reference papers and details about each type of attention.
         encoder_norm_layer (str): Normalization layer to use. One of 'abn', 'inplaceabn'. The inplace version lowers
             memory footprint. But increases backward time. Defaults to 'abn'.
         encoder_norm_act (str): Activation for normalizion layer. 'inplaceabn' doesn't support `ReLU` activation.
         decoder_norm_layer (str): same as encoder_norm_layer but for decoder
         decoder_norm_act (str): same as encoder_norm_act but for decoder
+        sigmoid_init (bool): if True, set last layer bias to -4.6 for faster convergence with sigmoid loss. usefull for binary classification problems
 
     Returns:
         ``torch.nn.Module``: **Unet**
     .. _Unet:
         https://arxiv.org/pdf/1505.04597
     """
 
@@ -105,14 +106,15 @@
         output_stride=32,
         drop_rate=0,
         decoder_attention_type=None,
         encoder_norm_layer="abn",
         encoder_norm_act="relu",
         decoder_norm_layer="abn",
         decoder_norm_act="relu",
+        sigmoid_init=True,
         **encoder_params,
     ):
         if output_stride != 32:
             encoder_params["output_stride"] = output_stride
         encoder = get_encoder(
             encoder_name,
             norm_layer=encoder_norm_layer,
@@ -130,10 +132,11 @@
             attn_type=decoder_attention_type,
             norm_layer=bn_from_name(decoder_norm_layer),
             norm_act=decoder_norm_act,
         )
 
         super().__init__(encoder, decoder)
         self.name = f"u-{encoder_name}"
-        # set last layer bias for better convergence with sigmoid loss
-        # -4.59 = -np.log((1 - 0.01) / 0.01)
-        nn.init.constant_(self.decoder.final_conv.bias, -4.59)
+        if sigmoid_init:
+            # set last layer bias for better convergence with sigmoid loss
+            # -4.59 = -np.log((1 - 0.01) / 0.01)
+            nn.init.constant_(self.decoder.final_conv.bias, -4.59)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools/segmentation_models/README.md` & `pytorch_tools-0.5.1/pytorch_tools/segmentation_models/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # PyTorch Segmentation Models Zoo
-All models here were either written from scratch or refactored from open-source implementations.  
+All models here were either written from scratch or refactored from open-source implementations.
 All models here use `Activated Normalization` layers instead of traditional `Normalization` followed by `Activation`. It makes changing activation function and normalization layer easy and convenient. It also allows using [Inplace Activated Batch Norm](https://github.com/mapillary/inplace_abn) from the box, which is essential for reducing memory footprint in segmentation tasks.
 
 
-## Encoders 
+## Encoders
 All [models](../models/) could be used as feature extractors (aka backbones) for segmentation architectures. Almost all combinations of backbones and segm.model are supported.
 
 
 ## Features
 * Unified API. Create `Unet, SegmentaionFPN, HRnet` models using the same code
 * Support for custom number of input channels in pretrained encoders
 * All core functionality covered with tests
 
 
 ## Repositories used
-* [Torch Vision Main Repo](https://github.com/pytorch/vision)  
+* [Torch Vision Main Repo](https://github.com/pytorch/vision)
 * [Cadene pretrained models](https://github.com/Cadene/pretrained-models.pytorch/)
 * [Ross Wightman models](https://github.com/rwightman/pytorch-image-models/)
-* [Pytorch Toolbelt by @BloodAxe](https://github.com/BloodAxe/pytorch-toolbelt)  
-* [Segmentation Models py @qubvel](https://github.com/qubvel/segmentation_models.pytorch)  
-* [Original HRNet for Segmentation](https://github.com/HRNet/HRNet-Semantic-Segmentation)
+* [Pytorch Toolbelt by @BloodAxe](https://github.com/BloodAxe/pytorch-toolbelt)
+* [Segmentation Models py @qubvel](https://github.com/qubvel/segmentation_models.pytorch)
+* [Original HRNet for Segmentation](https://github.com/HRNet/HRNet-Semantic-Segmentation)
```

### Comparing `pytorch_tools-0.1.9/pytorch_tools.egg-info/SOURCES.txt` & `pytorch_tools-0.5.1/pytorch_tools.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 README.md
 requirements.txt
 setup.py
 pytorch_tools/__init__.py
 pytorch_tools.egg-info/PKG-INFO
 pytorch_tools.egg-info/SOURCES.txt
@@ -12,14 +13,15 @@
 pytorch_tools/detection_models/__init__.py
 pytorch_tools/detection_models/efficientdet.py
 pytorch_tools/detection_models/retinanet.py
 pytorch_tools/fit_wrapper/README.md
 pytorch_tools/fit_wrapper/__init__.py
 pytorch_tools/fit_wrapper/callbacks.py
 pytorch_tools/fit_wrapper/state.py
+pytorch_tools/fit_wrapper/utils.py
 pytorch_tools/fit_wrapper/wrapper.py
 pytorch_tools/losses/README.md
 pytorch_tools/losses/__init__.py
 pytorch_tools/losses/angular.py
 pytorch_tools/losses/base.py
 pytorch_tools/losses/detection.py
 pytorch_tools/losses/dice_jaccard.py
@@ -37,37 +39,41 @@
 pytorch_tools/metrics/accuracy.py
 pytorch_tools/metrics/dice_jaccard.py
 pytorch_tools/metrics/psnr.py
 pytorch_tools/models/README.md
 pytorch_tools/models/__init__.py
 pytorch_tools/models/b_model.py
 pytorch_tools/models/bit_resnet.py
+pytorch_tools/models/cmodel.py
 pytorch_tools/models/densenet.py
 pytorch_tools/models/efficientnet.py
 pytorch_tools/models/hrnet.py
 pytorch_tools/models/preprocessing.py
 pytorch_tools/models/resnet.py
 pytorch_tools/models/tresnet.py
 pytorch_tools/models/vgg.py
 pytorch_tools/modules/__init__.py
 pytorch_tools/modules/activated_batch_channel_norm.py
 pytorch_tools/modules/activated_batch_norm.py
 pytorch_tools/modules/activated_group_norm.py
 pytorch_tools/modules/activated_no_norm.py
 pytorch_tools/modules/activations.py
 pytorch_tools/modules/bifpn.py
+pytorch_tools/modules/conv.py
 pytorch_tools/modules/decoder.py
 pytorch_tools/modules/fpn.py
+pytorch_tools/modules/mlp.py
 pytorch_tools/modules/pooling.py
 pytorch_tools/modules/residual.py
 pytorch_tools/modules/spatial_ocr_block.py
 pytorch_tools/modules/tf_same_ops.py
 pytorch_tools/modules/weight_standartization.py
 pytorch_tools/optim/README.md
 pytorch_tools/optim/__init__.py
+pytorch_tools/optim/adamp.py
 pytorch_tools/optim/adamw.py
 pytorch_tools/optim/lookahead.py
 pytorch_tools/optim/lr_finder.py
 pytorch_tools/optim/radam.py
 pytorch_tools/optim/rmsprop.py
 pytorch_tools/optim/schedulers.py
 pytorch_tools/optim/sgdw.py
@@ -83,30 +89,38 @@
 pytorch_tools/segmentation_models/unet.py
 pytorch_tools/tta_wrapper/README.md
 pytorch_tools/tta_wrapper/__init__.py
 pytorch_tools/tta_wrapper/functional.py
 pytorch_tools/tta_wrapper/wrapper.py
 pytorch_tools/utils/__init__.py
 pytorch_tools/utils/box.py
+pytorch_tools/utils/fuse.py
+pytorch_tools/utils/guided_filter.py
 pytorch_tools/utils/misc.py
 pytorch_tools/utils/preprocessing.py
 pytorch_tools/utils/rle.py
 pytorch_tools/utils/tensorboard.py
+pytorch_tools/utils/tiles.py
 pytorch_tools/utils/visualization.py
 tests/benchmarking/README.md
 tests/benchmarking/benchmarking_example.py
 tests/benchmarking/memory_test.py
 tests/detection_models/test_det_models.py
 tests/fit_wrapper/test_runner.py
+tests/fit_wrapper/test_utils.py
 tests/imgs/cityscapes_sample.jpg
 tests/imgs/cityscapes_sample2.jpg
 tests/imgs/dog.jpg
 tests/imgs/helmet.jpeg
 tests/losses/test_losses.py
 tests/metrics/test_metric.py
+tests/models/modules.py
+tests/models/test_cmodel.py
 tests/models/test_models.py
 tests/models/test_weights.py
 tests/modules/test_modules.py
 tests/segmentation_models/test_segm_models.py
 tests/tta_wrapper/test_tta.py
 tests/utils/test_box_utils.py
-tests/utils/test_misc_utils.py
+tests/utils/test_misc_utils.py
+tests/utils/test_model_fuse.py
+tests/utils/test_tiles.py
```

