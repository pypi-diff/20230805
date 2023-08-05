# Comparing `tmp/autogluon.multimodal-0.8.3b20230803.tar.gz` & `tmp/autogluon.multimodal-0.8.3b20230804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.multimodal-0.8.3b20230803.tar", last modified: Thu Aug  3 09:04:28 2023, max compression
+gzip compressed data, was "autogluon.multimodal-0.8.3b20230804.tar", last modified: Fri Aug  4 09:04:19 2023, max compression
```

## Comparing `autogluon.multimodal-0.8.3b20230803.tar` & `autogluon.multimodal-0.8.3b20230804.tar`

### file list

```diff
@@ -1,153 +1,153 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.277652 autogluon.multimodal-0.8.3b20230803/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-03 09:04:28.277652 autogluon.multimodal-0.8.3b20230803/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 09:04:28.277652 autogluon.multimodal-0.8.3b20230803/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.261652 autogluon.multimodal-0.8.3b20230803/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.261652 autogluon.multimodal-0.8.3b20230803/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/cli/prepare_detection_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/cli/voc2coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
--rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.269652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.269652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.269652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.269652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/datamodule.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.269652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/dataset_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/infer_types.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/mixup.py
--rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/preprocess_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_categorical.py
--rw-r--r--   0 runner    (1001) docker     (123)    14534 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_document.py
--rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.273652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6275 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_numerical.py
--rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    21349 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/randaug.py
--rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/template_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/trivial_augmenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    86709 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/matcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.273652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/adaptation_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/categorical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/categorical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8474 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/clip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7244 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/document_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/ft_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.273652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/fusion_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/fusion_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/fusion_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/huggingface_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mmdet_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mmocr_text_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mmocr_text_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)    10077 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/ner_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/numerical_mlp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/numerical_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)    12914 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/t_few.py
--rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/timm_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26208 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.277652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/deepspeed.py
--rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_distiller.py
--rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_mmdet.py
--rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_ner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/losses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   120569 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/problem_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.277652 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/cloud_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/colormap.py
--rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22986 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/download.py
--rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    11759 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/few_shot_learning.py
--rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/hpo.py
--rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/label_studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/load.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/mmcv.py
--rw-r--r--   0 runner    (1001) docker     (123)    22641 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/nlpaug.py
--rw-r--r--   0 runner    (1001) docker     (123)    53339 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/object_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/object_detection_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/onnx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/ovd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-03 09:03:51.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/save.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 09:04:28.265652 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 09:04:28.000000 autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.810466 autogluon.multimodal-0.8.3b20230804/
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-04 09:04:19.806466 autogluon.multimodal-0.8.3b20230804/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 09:04:19.810466 autogluon.multimodal-0.8.3b20230804/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.790465 autogluon.multimodal-0.8.3b20230804/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.790465 autogluon.multimodal-0.8.3b20230804/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5218 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/prepare_detection_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/voc2coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/schedule_1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/faster_rcnn_r50_fpn_1x_voc0712.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1949 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_l_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_m_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_nano_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_x_8xb8-300e_coco.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.794466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.798466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/datamodule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.798466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32962 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/infer_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/mixup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32638 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/preprocess_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14380 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_document.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13863 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.798466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6072 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6757 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/randaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3610 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/template_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25379 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8404 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/trivial_augmenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21216 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86709 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/matcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.802466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22571 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/adaptation_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4737 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8852 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/clip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7114 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/document_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ft_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.802466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7327 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6378 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8983 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11872 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/huggingface_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4456 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24886 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmdet_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ner_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20906 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8156 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13183 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/t_few.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11772 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/timm_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27987 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.802466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14966 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/deepspeed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21377 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_distiller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17746 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_mmdet.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17070 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_ner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12454 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/losses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31587 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   120595 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26209 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/problem_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.806466 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7748 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cloud_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3881 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/colormap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29543 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22866 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10418 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11505 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13844 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/few_shot_learning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8626 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/hpo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18762 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13437 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/label_studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/load.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18206 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13643 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7080 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/mmcv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23000 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/nlpaug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53339 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18477 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5607 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/onnx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/ovd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4782 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-08-04 09:03:48.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/save.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 09:04:19.790465 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12686 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 09:04:19.000000 autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/zip-safe
```

### Comparing `autogluon.multimodal-0.8.3b20230803/PKG-INFO` & `autogluon.multimodal-0.8.3b20230804/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.3b20230803
+Version: 0.8.3b20230804
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.8.3b20230803/setup.py` & `autogluon.multimodal-0.8.3b20230804/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/cli/prepare_detection_dataset.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/prepare_detection_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/cli/voc2coco.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/cli/voc2coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/default_runtime.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/faster_rcnn/faster_rcnn_r50_fpn.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/voc/voc0712.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_s_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tiny_8xb8-300e_coco.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/detection/yolox/yolox_tta.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinB.cfg.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/configs/pretrain/ovd/grounding_dino/GroundingDINO_SwinT_OGC.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/constants.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/constants.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/__init__.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/collator.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/collator.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/datamodule.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/datamodule.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/dataset.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/dataset_mmlab/multi_image_mix_dataset.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/infer_types.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/infer_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/label_encoder.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/mixup.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/mixup.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/preprocess_dataframe.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/preprocess_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_categorical.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_categorical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_document.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,25 +8,21 @@
 import PIL
 import pytesseract
 import torch
 from nptyping import NDArray
 from PIL import ImageFile
 from torch import nn
 from torchvision import transforms
-from transformers import AutoTokenizer
 
 from ..constants import AUTOMM, BBOX, DOCUMENT_PDF
 from .collator import PadCollator, StackCollator
 from .utils import construct_image_processor, image_mean_std
 
 logger = logging.getLogger(__name__)
 
-# Disable tokenizer parallelism
-os.environ["TOKENIZERS_PARALLELISM"] = "false"
-
 
 class DocumentProcessor:
     """
     Prepare document data for Document Classification.
     OCR (Optical character recognition) is applied to get the document texts and bounding boxes.
     Both texts and images will be processed.
     """
@@ -99,34 +95,30 @@
         # If True, normal text foundation models (e.g., bert-base) can be used.
         self.is_text_only_flag = model.is_text_only_flag
 
         self.pad_token_box = [0, 0, 0, 0]  # cls box token
         self.sep_token_box = [1000, 1000, 1000, 1000]  # sep box token
 
         # For document text processing.
+        # Disable tokenizer parallelism
+        os.environ["TOKENIZERS_PARALLELISM"] = "false"
+        self.tokenizer_name = model.tokenizer_name
         self.tokenizer = model.tokenizer
         if text_max_len is None or text_max_len <= 0:
             self.text_max_len = self.tokenizer.model_max_length
         else:
             if text_max_len < self.tokenizer.model_max_length:
                 warnings.warn(
                     f"provided max length: {text_max_len} "
                     f"is smaller than {model.checkpoint_name}'s default: {self.tokenizer.model_max_length}"
                 )
             self.text_max_len = min(text_max_len, self.tokenizer.model_max_length)
 
         self.tokenizer.model_max_length = self.text_max_len
 
-    @staticmethod
-    def get_pretrained_tokenizer(
-        tokenizer_name: str,
-        checkpoint_name: str,
-    ):
-        return AutoTokenizer.from_pretrained(checkpoint_name)
-
     def collate_fn(self, text_column_names: Optional[List] = None) -> Dict:
         """
         Collate multimodal features into a batch.
         This function will be used when creating Pytorch DataLoader.
 
         Returns
         -------
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_image.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_label.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_label.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmlab_base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_mmlab/process_mmocr.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_ner.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ner.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,60 +3,58 @@
 import warnings
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 from nptyping import NDArray
 from omegaconf import DictConfig
 from torch import nn
-from transformers import AutoConfig, AutoTokenizer, BertTokenizer, CLIPTokenizer, ElectraTokenizer
 
 from ..constants import AUTOMM, NER_ANNOTATION, NER_TEXT, TEXT, TEXT_NER
 from .collator import PadCollator, StackCollator
 from .utils import process_ner_annotations, tokenize_ner_text
 
 logger = logging.getLogger(__name__)
 
-# Disable tokenizer parallelism
-os.environ["TOKENIZERS_PARALLELISM"] = "false"
-
 
 class NerProcessor:
     """
     Prepare NER data for the model specified by "prefix".
     """
 
     def __init__(
         self,
         model: nn.Module,
         max_len: Optional[int] = None,
-        config: Optional[DictConfig] = None,
+        entity_map: Optional[DictConfig] = None,
     ):
         """
         Parameters
         ----------
         model
             The NER model.
         max_len
             The max length of the tokenizer.
-        config
-            Config dictionary.
+        entity_map
+            The map between tags and tag indexes. e.g., {"PER":2, "LOC":3}.
         """
         self.prefix = model.prefix
         self.text_token_ids_key = model.text_token_ids_key
         self.text_valid_length_key = model.text_valid_length_key
         self.text_segment_ids_key = model.text_segment_ids_key
         self.text_token_word_mapping_key = model.text_token_word_mapping_key
         self.text_word_offsets_key = model.text_word_offsets_key
         self.label_key = model.label_key
 
         self.tokenizer = None
-        self.tokenizer_name = model.prefix
+        self.tokenizer_name = model.tokenizer_name
         self.max_len = max_len
-        self.config = config
+        self.entity_map = entity_map
 
+        # Disable tokenizer parallelism
+        os.environ["TOKENIZERS_PARALLELISM"] = "false"
         if self.prefix == NER_TEXT:
             self.tokenizer = model.tokenizer
 
             if max_len is None or max_len <= 0:
                 self.max_len = self.tokenizer.model_max_length
             else:
                 if max_len < self.tokenizer.model_max_length:
@@ -64,21 +62,14 @@
                         f"provided max length: {max_len} "
                         f"is smaller than {model.checkpoint_name}'s default: {self.tokenizer.model_max_length}"
                     )
                 self.max_len = min(max_len, self.tokenizer.model_max_length)
 
             self.tokenizer.model_max_length = self.max_len
 
-    @staticmethod
-    def get_pretrained_tokenizer(
-        tokenizer_name: str,
-        checkpoint_name: str,
-    ):
-        return AutoTokenizer.from_pretrained(checkpoint_name)
-
     def collate_fn(self, text_column_names: Optional[List] = None) -> Dict:
         """
         Collate multimodal features into a batch.
         This function will be used when creating Pytorch DataLoader.
 
         Returns
         -------
@@ -130,15 +121,15 @@
             if column_modality == NER_ANNOTATION:
                 annotation_column = column_name
 
         ner_text = all_features[text_column]
         if is_training or annotation_column is not None:
             ner_annotation = all_features[annotation_column]
             label, col_tokens, token_to_word_mappings, word_offsets = process_ner_annotations(
-                ner_annotation, ner_text, self.config.entity_map, self.tokenizer
+                ner_annotation, ner_text, self.entity_map, self.tokenizer
             )
             ret.update({self.label_key: label})
         else:
             col_tokens, token_to_word_mappings, word_offsets = tokenize_ner_text(ner_text, self.tokenizer)
             ret.update({self.label_key: np.array([], dtype=np.int32)})
 
         ret.update(
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_numerical.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_numerical.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_ovd.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/process_text.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/process_text.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 from copy import deepcopy
 from typing import Any, Dict, List, Optional, Union
 
 import numpy as np
 from nptyping import NDArray
 from omegaconf import DictConfig
 from torch import nn
-from transformers import AutoConfig, AutoTokenizer, BertTokenizer, CLIPTokenizer, ElectraTokenizer
 
 from ..constants import CHOICES_IDS, COLUMN, TEXT, TEXT_SEGMENT_IDS, TEXT_TOKEN_IDS, TEXT_VALID_LENGTH
 from .collator import PadCollator, StackCollator
 from .template_engine import TemplateEngine
 from .trivial_augmenter import TrivialAugment
 from .utils import (
     extract_value_from_config,
@@ -24,51 +23,39 @@
 
 logger = logging.getLogger(__name__)
 
 # Disable tokenizer parallelism
 os.environ["TOKENIZERS_PARALLELISM"] = "false"
 
 
-ALL_TOKENIZERS = {
-    "bert": BertTokenizer,
-    "clip": CLIPTokenizer,
-    "electra": ElectraTokenizer,
-    "hf_auto": AutoTokenizer,
-}
-
-
 class TextProcessor:
     """
     Prepare text data for the model specified by "prefix". For multiple models requiring text data,
     we need to create a TextProcessor for each related model so that they will have independent input.
     """
 
     def __init__(
         self,
         model: nn.Module,
-        tokenizer_name: Optional[str] = "hf_auto",
         max_len: Optional[int] = None,
         insert_sep: Optional[bool] = True,
         text_segment_num: Optional[int] = 1,
         stochastic_chunk: Optional[bool] = False,
         requires_column_info: bool = False,
         text_detection_length: Optional[int] = None,
         text_trivial_aug_maxscale: Optional[float] = 0.0,
         train_augment_types: Optional[List[str]] = None,
         template_config: Optional[DictConfig] = None,
         normalize_text: Optional[bool] = False,
-        use_fast: Optional[bool] = True,
     ):
         """
         Parameters
         ----------
         model
             The model for which this processor would be created.
-        tokenizer_name
-            Name of the huggingface tokenizer type (default "hf_auto").
         max_len
             The maximum length of text tokens.
         insert_sep
             Whether to insert SEP tokens.
         text_segment_num
             The number of text segments.
         stochastic_chunk
@@ -83,32 +70,20 @@
             https://arxiv.org/pdf/2103.10158.pdf
         train_augment_types
             All possible augmentation operations
         normalize_text
             Whether to normalize text to resolve encoding problems.
             Examples of normalized texts can be found at
             https://github.com/autogluon/autogluon/tree/master/examples/automm/kaggle_feedback_prize#15-a-few-examples-of-normalized-texts
-        use_fast
-            Use a fast Rust-based tokenizer if it is supported for a given model.
-            If a fast tokenizer is not available for a given model, a normal Python-based tokenizer is returned instead.
-            See: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoTokenizer.from_pretrained.use_fast
-
         """
         self.prefix = model.prefix
-        self.tokenizer_name = tokenizer_name
         self.requires_column_info = requires_column_info
-        # Use the model's tokenizer if it exists.
-        if hasattr(model, "tokenizer"):
-            self.tokenizer = model.tokenizer
-        else:
-            self.tokenizer = self.get_pretrained_tokenizer(
-                tokenizer_name=tokenizer_name,
-                checkpoint_name=model.checkpoint_name,
-                use_fast=use_fast,
-            )
+        self.tokenizer_name = model.tokenizer_name
+        # model should have a tokenizer
+        self.tokenizer = model.tokenizer
         if hasattr(self.tokenizer, "deprecation_warnings"):
             # Disable the warning "Token indices sequence length is longer than the specified maximum sequence..."
             # See https://github.com/huggingface/transformers/blob/6ac77534bfe97c00e0127bb4fc846ae0faf1c9c5/src/transformers/tokenization_utils_base.py#L3362
             self.tokenizer.deprecation_warnings["sequence-length-is-longer-than-the-specified-maximum"] = True
 
         self.cls_token_id, self.sep_token_id, self.eos_token_id = self.get_special_tokens(tokenizer=self.tokenizer)
         self.max_len = get_text_token_max_len(
@@ -371,53 +346,14 @@
             cls_id = sep_id = eos_id
 
         if cls_id is None or sep_id is None or eos_id is None:
             raise ValueError(f"tokenizer class: {tokenizer.__class__.__name__} has no valid cls, sep, and eos ids.")
         return cls_id, sep_id, eos_id
 
     @staticmethod
-    def get_pretrained_tokenizer(
-        tokenizer_name: str,
-        checkpoint_name: str,
-        use_fast: Optional[bool] = True,
-    ):
-        """
-        Load the tokenizer for a pre-trained huggingface checkpoint.
-
-        Parameters
-        ----------
-        tokenizer_name
-            The tokenizer type, e.g., "bert", "clip", "electra", and "hf_auto".
-        checkpoint_name
-            Name of a pre-trained checkpoint.
-        use_fast
-            Use a fast Rust-based tokenizer if it is supported for a given model.
-            If a fast tokenizer is not available for a given model, a normal Python-based tokenizer is returned instead.
-            See: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoTokenizer.from_pretrained.use_fast
-
-        Returns
-        -------
-        A tokenizer instance.
-        """
-        try:
-            tokenizer_class = ALL_TOKENIZERS[tokenizer_name]
-            return tokenizer_class.from_pretrained(checkpoint_name, use_fast=use_fast)
-        except TypeError as e:
-            try:
-                tokenizer_class = ALL_TOKENIZERS["bert"]
-                tokenizer = tokenizer_class.from_pretrained(checkpoint_name)
-                logger.warning(
-                    f"Current checkpoint {checkpoint_name} does not support AutoTokenizer. "
-                    "Switch to BertTokenizer instead."
-                )
-                return tokenizer
-            except:
-                raise e
-
-    @staticmethod
     def get_trimmed_lengths(
         lengths: List[int],
         max_length: int,
         do_merge: bool = False,
     ) -> List:
         """
         Get the trimmed lengths of multiple text token sequences. It will make sure that
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/randaug.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/randaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/template_engine.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/template_engine.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/templates.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/templates.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/trivial_augmenter.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/trivial_augmenter.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/data/utils.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/data/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/matcher.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/__init__.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/adaptation_layers.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/adaptation_layers.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/categorical_mlp.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/categorical_transformer.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/categorical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/clip.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/clip.py`

 * *Files 18% similar despite different names*

```diff
@@ -14,15 +14,21 @@
     LABEL,
     LOGIT_SCALE,
     LOGITS,
     MASKS,
     TEXT_TOKEN_IDS,
     TEXT_VALID_LENGTH,
 )
-from .utils import assign_layer_ids, get_column_features, get_hf_config_and_model, init_weights
+from .utils import (
+    assign_layer_ids,
+    get_column_features,
+    get_hf_config_and_model,
+    get_pretrained_tokenizer,
+    init_weights,
+)
 
 logger = logging.getLogger(__name__)
 
 
 class CLIPForImageText(nn.Module):
     """
     Support the CLIP model.
@@ -31,35 +37,43 @@
 
     def __init__(
         self,
         prefix: str,
         checkpoint_name: str,
         num_classes: Optional[int] = None,
         pretrained: Optional[bool] = True,
+        tokenizer_name: Optional[str] = "clip",
     ):
         """
         Load the pretrained CLIP from huggingface transformers.
 
         Parameters
         ----------
         prefix
             The model prefix.
         checkpoint_name
             Name of the checkpoint.
         num_classes
             The number of classes. 1 for a regression task.
         pretrained
             Whether using the pretrained weights. If pretrained=True, download the pretrained model.
+        tokenizer_name
+            Name of the huggingface tokenizer type.
         """
         super().__init__()
         logger.debug(f"initializing {checkpoint_name}")
         self.checkpoint_name = checkpoint_name
         self.num_classes = num_classes
 
         self.config, self.model = get_hf_config_and_model(checkpoint_name=checkpoint_name, pretrained=pretrained)
+        self.tokenizer_name = tokenizer_name
+        self.tokenizer = get_pretrained_tokenizer(
+            tokenizer_name=self.tokenizer_name,
+            checkpoint_name=self.checkpoint_name,
+        )
 
         self.out_features = self.model.config.projection_dim
 
         self.head = nn.Linear(self.out_features, num_classes) if num_classes else nn.Identity()
         self.head.apply(init_weights)
 
         self.prefix = prefix
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/document_transformer.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/document_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 import inspect
 import logging
 from typing import Callable, Dict, List, Optional, Tuple, Union, cast
 
-import torch
-from torch import nn
-from transformers import AutoTokenizer, LayoutLMTokenizer, LayoutLMTokenizerFast, RobertaTokenizerFast
 from transformers import logging as hf_logging
 
 from ..constants import (
     ATTENTION_MASK,
     AUTOMM,
     BBOX,
     COLUMN,
@@ -22,15 +19,15 @@
     PIXEL_VALUES,
     TEXT_SEGMENT_IDS,
     TEXT_TOKEN_IDS,
     TEXT_VALID_LENGTH,
     TOKEN_TYPE_IDS,
 )
 from .huggingface_text import HFAutoModelForTextPrediction
-from .utils import DummyLayer, assign_layer_ids, get_column_features, get_hf_config_and_model, init_weights
+from .utils import get_column_features
 
 hf_logging.set_verbosity_error()
 
 logger = logging.getLogger(__name__)
 
 
 class DocumentTransformer(HFAutoModelForTextPrediction):
@@ -43,14 +40,15 @@
         prefix: str,
         checkpoint_name: str = "microsoft/layoutlmv3-base",
         num_classes: Optional[int] = 0,
         pooling_mode: Optional[str] = "cls",
         gradient_checkpointing: Optional[bool] = False,
         low_cpu_mem_usage: Optional[bool] = False,
         pretrained: Optional[bool] = True,
+        tokenizer_name: Optional[str] = "hf_auto",
     ):
         """
         Load a pretrained huggingface layout-aware document transformer backbone.
 
         Parameters
         ----------
         prefix
@@ -73,46 +71,47 @@
             The pooling mode for the Transformer. Can be "cls", or "mean"
         gradient_checkpointing
             Whether to enable gradient checkpointing
         low_cpu_mem_usage
             Whether to turn on the optimization of reducing the peak CPU memory usage when loading the pretrained model.
         pretrained
             Whether using the pretrained weights. If pretrained=True, download the pretrained model.
+        tokenizer_name
+            Name of the huggingface tokenizer type.
         """
+        logger.debug(f"initializing {checkpoint_name}")
         super().__init__(
             prefix=prefix,
             checkpoint_name=checkpoint_name,
             num_classes=num_classes,
             pooling_mode=pooling_mode,
             gradient_checkpointing=gradient_checkpointing,
             low_cpu_mem_usage=low_cpu_mem_usage,
             pretrained=pretrained,
+            tokenizer_name=tokenizer_name,
         )
-        logger.debug(f"initializing {checkpoint_name}")
-
-        self.tokenizer = AutoTokenizer.from_pretrained(checkpoint_name)
-        self.is_text_only_flag = self.is_text_only(self.tokenizer)
+        self.is_text_only_flag = self.is_text_only()
 
         if self.is_text_only_flag:
             logger.debug(f"Checkpoint: {checkpoint_name} uses the text data only for classification.")
 
-    def is_text_only(self, tokenizer):
+    def is_text_only(self):
         """
         Check the tokenizer to see if it is a text only tokenizer.
 
         Parameters
         ----------
         tokenizer
             The tokenizer to be used.
 
         Returns
         -------
         True if the tokenizer only accept text, otherwise, False.
         """
-        model_args = list(inspect.signature(tokenizer.__call__).parameters.keys())
+        model_args = list(inspect.signature(self.tokenizer.__call__).parameters.keys())
         # Tokenizers of document foundation models usually have a "boxes" argument.
         if "boxes" not in model_args:
             return True
         else:
             return False
 
     @property
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/ft_transformer.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ft_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/base.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/base.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/fusion_mlp.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/fusion_ner.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/fusion/fusion_transformer.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/fusion/fusion_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/huggingface_text.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/huggingface_text.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import logging
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
-from transformers import AutoTokenizer
 from transformers import logging as hf_logging
 from transformers.models.t5 import T5PreTrainedModel
 
 from ..constants import (
     AUTOMM,
     COLUMN,
     COLUMN_FEATURES,
@@ -15,15 +14,22 @@
     LABEL,
     LOGITS,
     MASKS,
     TEXT_SEGMENT_IDS,
     TEXT_TOKEN_IDS,
     TEXT_VALID_LENGTH,
 )
-from .utils import DummyLayer, assign_layer_ids, get_column_features, get_hf_config_and_model, init_weights
+from .utils import (
+    DummyLayer,
+    assign_layer_ids,
+    get_column_features,
+    get_hf_config_and_model,
+    get_pretrained_tokenizer,
+    init_weights,
+)
 
 hf_logging.set_verbosity_error()
 
 logger = logging.getLogger(__name__)
 
 
 class HFAutoModelForTextPrediction(nn.Module):
@@ -37,14 +43,16 @@
         prefix: str,
         checkpoint_name: str = "microsoft/deberta-v3-base",
         num_classes: Optional[int] = 0,
         pooling_mode: Optional[str] = "cls",
         gradient_checkpointing: Optional[bool] = False,
         low_cpu_mem_usage: Optional[bool] = False,
         pretrained: Optional[bool] = True,
+        tokenizer_name: Optional[str] = "hf_auto",
+        use_fast: Optional[bool] = True,
     ):
         """
         Load a pretrained huggingface text transformer backbone.
 
         Parameters
         ----------
         prefix
@@ -68,24 +76,35 @@
             The pooling mode for the Transformer. Can be "cls", or "mean"
         gradient_checkpointing
             Whether to enable gradient checkpointing
         low_cpu_mem_usage
             Whether to turn on the optimization of reducing the peak CPU memory usage when loading the pretrained model.
         pretrained
             Whether using the pretrained weights. If pretrained=True, download the pretrained model.
+        tokenizer_name
+            Name of the huggingface tokenizer type.
+        use_fast
+            Use a fast Rust-based tokenizer if it is supported for a given model.
+            If a fast tokenizer is not available for a given model, a normal Python-based tokenizer is returned instead.
+            See: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoTokenizer.from_pretrained.use_fast
         """
         super().__init__()
         logger.debug(f"initializing {checkpoint_name}")
         self.checkpoint_name = checkpoint_name
         self.num_classes = num_classes
 
         self.config, self.model = get_hf_config_and_model(
             checkpoint_name=checkpoint_name, pretrained=pretrained, low_cpu_mem_usage=low_cpu_mem_usage
         )
-        self._hf_model_input_names = AutoTokenizer.from_pretrained(checkpoint_name).model_input_names
+        self.tokenizer_name = tokenizer_name
+        self.tokenizer = get_pretrained_tokenizer(
+            tokenizer_name=self.tokenizer_name,
+            checkpoint_name=self.checkpoint_name,
+            use_fast=use_fast,
+        )
 
         if isinstance(self.model, T5PreTrainedModel):
             self.is_t5 = True
             # Remove the decoder in T5. We will only use the T5 encoder for extracting the embeddings
             del self.model.decoder
         else:
             self.is_t5 = False
@@ -184,15 +203,15 @@
                 #  Reference: https://discuss.pytorch.org/t/checkpoint-with-no-grad-requiring-inputs-problem/19117/9
                 inputs_embeds = self.dummy_layer(inputs_embeds)
             outputs = self.model.encoder(
                 inputs_embeds=inputs_embeds,
                 attention_mask=text_masks,
             )
         else:
-            if "token_type_ids" in self._hf_model_input_names:
+            if "token_type_ids" in self.tokenizer.model_input_names:
                 outputs = self.model(
                     input_ids=text_token_ids,
                     token_type_ids=text_segment_ids,
                     attention_mask=text_masks,
                 )
             else:
                 outputs = self.model(
@@ -288,13 +307,11 @@
             logger.debug(f"outer layers are treated as head: {names}")
         for n in names:
             assert n not in name_to_id
             name_to_id[n] = 0
 
         return name_to_id
 
-    def save(self, save_path: str = "./", tokenizers: Optional[dict] = None):
+    def save(self, save_path: str = "./"):
         self.model.save_pretrained(save_path)
-        logger.info(f"Model weights for {self.prefix} are saved to {save_path}.")
-        if self.prefix in tokenizers:
-            tokenizers[self.prefix].save_pretrained(save_path)
-            logger.info(f"Tokenizer {self.prefix} saved to {save_path}.")
+        self.tokenizer.save_pretrained(save_path)
+        logger.info(f"Model weights and tokenizer for {self.prefix} are saved to {save_path}.")
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mlp.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mmdet_image.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmdet_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mmocr_text_detection.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/mmocr_text_recognition.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/mmocr_text_recognition.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/ner_text.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ner_text.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
 from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
-from transformers import AutoTokenizer
 from transformers import logging as hf_logging
 
 from ..constants import (
     AUTOMM,
     COLUMN,
     COLUMN_FEATURES,
     FEATURES,
@@ -19,15 +18,15 @@
     TEXT_SEGMENT_IDS,
     TEXT_TOKEN_IDS,
     TEXT_VALID_LENGTH,
     TOKEN_WORD_MAPPING,
     WORD_OFFSETS,
 )
 from .huggingface_text import HFAutoModelForTextPrediction
-from .utils import DummyLayer, assign_layer_ids, get_column_features, get_hf_config_and_model, init_weights
+from .utils import assign_layer_ids, get_column_features, get_pretrained_tokenizer
 
 hf_logging.set_verbosity_error()
 
 logger = logging.getLogger(__name__)
 
 
 class HFAutoModelForNER(HFAutoModelForTextPrediction):
@@ -40,14 +39,15 @@
         prefix: str,
         checkpoint_name: str = "microsoft/deberta-v3-base",
         num_classes: Optional[int] = 0,
         pooling_mode: Optional[str] = "cls",
         gradient_checkpointing: Optional[bool] = False,
         low_cpu_mem_usage: Optional[bool] = False,
         pretrained: Optional[bool] = True,
+        tokenizer_name: Optional[str] = "hf_auto",
     ):
         """
         Load a pretrained huggingface text transformer backbone.
         Parameters
         ----------
         prefix
             The model prefix.
@@ -63,32 +63,36 @@
             The pooling mode to be used, it is not used in the NER task.
         gradient_checkpointing
             Whether to enable gradient checkpointing
         low_cpu_mem_usage
             Whether to turn on the optimization of reducing the peak CPU memory usage when loading the pretrained model.
         pretrained
             Whether using the pretrained weights. If pretrained=True, download the pretrained model.
+        tokenizer_name
+            Name of the huggingface tokenizer type.
         """
+        logger.debug(f"initializing {checkpoint_name}")
         super().__init__(
             prefix=prefix,
             checkpoint_name=checkpoint_name,
             num_classes=num_classes,
             pooling_mode=pooling_mode,
             gradient_checkpointing=gradient_checkpointing,
             low_cpu_mem_usage=low_cpu_mem_usage,
             pretrained=pretrained,
+            tokenizer_name=tokenizer_name,
         )
 
-        logger.debug(f"initializing {checkpoint_name}")
-
         if self.config.model_type in {"gpt2", "roberta"}:
             # Refer to this PR: https://github.com/huggingface/transformers/pull/12116
-            self.tokenizer = AutoTokenizer.from_pretrained(checkpoint_name, add_prefix_space=True)
-        else:
-            self.tokenizer = AutoTokenizer.from_pretrained(checkpoint_name)
+            self.tokenizer = get_pretrained_tokenizer(
+                tokenizer_name=self.tokenizer_name,
+                checkpoint_name=self.checkpoint_name,
+                add_prefix_space=True,
+            )
 
         # some checkpoint such as deberta does not specify model_max_length
         # here, we reset it using model config.
         if hasattr(self.model.config, "max_position_embeddings"):
             self.tokenizer.model_max_length = self.model.config.max_position_embeddings
         if hasattr(self.model.config, "n_positions"):
             self.tokenizer.model_max_length = self.model.config.n_positions
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/numerical_mlp.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_mlp.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/numerical_transformer.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/numerical_transformer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/ovd.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/t_few.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/t_few.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import random
 from functools import lru_cache
 from typing import Dict, List, Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch import nn
-from transformers import AutoConfig, AutoModelForSeq2SeqLM, AutoTokenizer
+from transformers import AutoConfig, AutoModelForSeq2SeqLM
 from transformers import logging as hf_logging
 
 from ..constants import (
     AUTOMM,
     CHOICES_IDS,
     COLUMN,
     COLUMN_FEATURES,
@@ -22,15 +22,15 @@
     LOGITS,
     MASKS,
     TEMPLATE_LOGITS,
     TEXT_SEGMENT_IDS,
     TEXT_TOKEN_IDS,
     TEXT_VALID_LENGTH,
 )
-from .utils import DummyLayer, assign_layer_ids, get_column_features
+from .utils import DummyLayer, assign_layer_ids, get_column_features, get_pretrained_tokenizer
 
 hf_logging.set_verbosity_error()
 
 logger = logging.getLogger(__name__)
 
 
 @lru_cache(None)
@@ -51,14 +51,15 @@
         num_classes: Optional[int] = 0,
         length_norm: float = 1.0,  # Normalizes length to adjust for length bias in target template
         unlikely_loss: float = 1.0,  # Adds loss term that lowers probability of incorrect outputs
         mc_loss: float = 1.0,  # Adds multiple choice cross entropy loss
         gradient_checkpointing: Optional[bool] = False,
         low_cpu_mem_usage: Optional[bool] = False,
         pretrained: Optional[bool] = True,
+        tokenizer_name: Optional[str] = "hf_auto",
     ):
         """
         Load a pretrained T5-based text transformer backbone.
 
         Parameters
         ----------
         prefix
@@ -80,29 +81,35 @@
             Adds multiple choice cross entropy loss
         gradient_checkpointing
             Whether to enable gradient checkpointing
         low_cpu_mem_usage
             Whether to turn on the optimization of reducing the peak CPU memory usage when loading the pretrained model.
         pretrained
             Whether using the pretrained weights. If pretrained=True, download the pretrained model.
+        tokenizer_name
+            Name of the huggingface tokenizer type.
         """
         super().__init__()
         logger.debug(f"initializing {checkpoint_name}")
 
         self.checkpoint_name = checkpoint_name
         self.num_classes = num_classes
 
         self.config = AutoConfig.from_pretrained(checkpoint_name)
 
         if pretrained:
             self.model = AutoModelForSeq2SeqLM.from_pretrained(checkpoint_name, low_cpu_mem_usage=low_cpu_mem_usage)
         else:
             self.model = AutoModelForSeq2SeqLM.from_config(self.config)
 
-        self.tokenizer = AutoTokenizer.from_pretrained(checkpoint_name)
+        self.tokenizer_name = tokenizer_name
+        self.tokenizer = get_pretrained_tokenizer(
+            tokenizer_name=self.tokenizer_name,
+            checkpoint_name=self.checkpoint_name,
+        )
         self.eos_token = self.tokenizer.eos_token
         self.out_features = (
             self.model.config.hidden_size
         )  # required attribute for some features, e.g. data augmentation
 
         self.gradient_checkpointing = gradient_checkpointing
         if gradient_checkpointing:
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/timm_image.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/timm_image.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/models/utils.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/models/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,31 @@
 import logging
 import re
+import warnings
 from typing import Dict, List, Optional, Tuple
 
 import torch
 from torch import nn
 from torch.nn.modules.loss import _Loss
-from transformers import AutoConfig, AutoModel
+from transformers import AutoConfig, AutoModel, AutoTokenizer, BertTokenizer, CLIPTokenizer, ElectraTokenizer
 
 from ..constants import AUTOMM, COLUMN_FEATURES, FEATURES, LOGITS, MASKS, OCR, REGRESSION
 from .adaptation_layers import IA3Linear, IA3LoRALinear, LoRALinear
 
 logger = logging.getLogger(__name__)
 
 
+ALL_TOKENIZERS = {
+    "bert": BertTokenizer,
+    "clip": CLIPTokenizer,
+    "electra": ElectraTokenizer,
+    "hf_auto": AutoTokenizer,
+}
+
+
 class DummyLayer(nn.Module):
     """
     DummyLayer to ensure that the gradient checkpointing will assign output layer as require_grad=True.
     Reference: https://discuss.pytorch.org/t/checkpoint-with-no-grad-requiring-inputs-problem/19117/9
     """
 
     def __init__(self):
@@ -745,7 +754,52 @@
         return
 
     is_frozen_layer = lambda n: any(bb in n for bb in frozen_layers)
 
     for n, p in model.named_parameters():
         if is_frozen_layer(n):
             p.requires_grad = False
+
+
+def get_pretrained_tokenizer(
+    tokenizer_name: str,
+    checkpoint_name: str,
+    use_fast: Optional[bool] = True,
+    add_prefix_space: Optional[bool] = None,
+):
+    """
+    Load the tokenizer for a pre-trained huggingface checkpoint.
+
+    Parameters
+    ----------
+    tokenizer_name
+        The tokenizer type, e.g., "bert", "clip", "electra", and "hf_auto".
+    checkpoint_name
+        Name of a pre-trained checkpoint.
+    use_fast
+        Use a fast Rust-based tokenizer if it is supported for a given model.
+        If a fast tokenizer is not available for a given model, a normal Python-based tokenizer is returned instead.
+        See: https://huggingface.co/docs/transformers/model_doc/auto#transformers.AutoTokenizer.from_pretrained.use_fast
+
+    Returns
+    -------
+    A tokenizer instance.
+    """
+    try:
+        tokenizer_class = ALL_TOKENIZERS[tokenizer_name]
+        if add_prefix_space is None:
+            return tokenizer_class.from_pretrained(checkpoint_name, use_fast=use_fast)
+        else:
+            return tokenizer_class.from_pretrained(
+                checkpoint_name, use_fast=use_fast, add_prefix_space=add_prefix_space
+            )
+    except TypeError as e:
+        try:
+            tokenizer = BertTokenizer.from_pretrained(checkpoint_name)
+            warnings.warn(
+                f"Current checkpoint {checkpoint_name} does not support AutoTokenizer. "
+                "Switch to BertTokenizer instead.",
+                UserWarning,
+            )
+            return tokenizer
+        except:
+            raise e
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/deepspeed.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/deepspeed.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_distiller.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_distiller.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_matcher.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_mmdet.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_mmdet.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_module.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_module.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lit_ner.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lit_ner.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/losses.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/losses.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/lr_scheduler.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/lr_scheduler.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/optimization/utils.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/optimization/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/predictor.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/predictor.py`

 * *Files 0% similar despite different names*

```diff
@@ -2590,14 +2590,15 @@
             with open(os.path.join(path, "data_processors.pkl"), "rb") as fp:
                 data_processors = CustomUnpickler(fp).load()
             # Load text tokenizers after loading data processors.
             for modality in [
                 TEXT,
                 TEXT_NER,
                 NER,
+                DOCUMENT,
             ]:  # NER is included for backward compatibility
                 if modality in data_processors:
                     data_processors[modality] = load_text_tokenizers(
                         text_processors=data_processors[modality],
                         path=path,
                     )
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/presets.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/problem_types.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/problem_types.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/registry.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/registry.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/__init__.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/cache.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cache.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/checkpoint.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/cloud_io.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/cloud_io.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/colormap.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/colormap.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/config.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/config.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/data.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,25 +143,23 @@
             size=model_config.image_size,
             max_img_num_per_col=model_config.max_img_num_per_col,
             missing_value_strategy=config.data.image.missing_value_strategy,
         )
     elif data_type == TEXT:
         data_processor = TextProcessor(
             model=model,
-            tokenizer_name=model_config.tokenizer_name,
             max_len=model_config.max_text_len,
             insert_sep=model_config.insert_sep,
             text_segment_num=model_config.text_segment_num,
             stochastic_chunk=model_config.stochastic_chunk,
             text_detection_length=OmegaConf.select(model_config, "text_aug_detect_length"),
             text_trivial_aug_maxscale=OmegaConf.select(model_config, "text_trivial_aug_maxscale"),
             train_augment_types=OmegaConf.select(model_config, "text_train_augment_types"),
             template_config=getattr(config.data, "templates", OmegaConf.create({"turn_on": False})),
             normalize_text=getattr(config.data.text, "normalize_text", False),
-            use_fast=OmegaConf.select(model_config, "use_fast", default=True),
         )
     elif data_type == CATEGORICAL:
         data_processor = CategoricalProcessor(
             model=model,
         )
     elif data_type == NUMERICAL:
         data_processor = NumericalProcessor(
@@ -170,15 +168,15 @@
         )
     elif data_type == LABEL:
         data_processor = LabelProcessor(model=model)
     elif data_type == TEXT_NER:
         data_processor = NerProcessor(
             model=model,
             max_len=model_config.max_text_len,
-            config=config,
+            entity_map=config.entity_map,
         )
     elif data_type == ROIS:
         data_processor = MMDetProcessor(
             model=model,
             max_img_num_per_col=model_config.max_img_num_per_col,
             missing_value_strategy=config.data.image.missing_value_strategy,
         )
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/download.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/download.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/environment.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/environment.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/export.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/export.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         """
         Save model weights and config to local directory.
         Model weights are saved in file `pytorch_model.bin` (timm, hf) or '<ckpt_name>.pth' (mmdet);
         Configs are saved in file `config.json` (timm, hf) or  '<ckpt_name>.py' (mmdet).
 
         Parameters
         ----------
-        path : str
+        save_path : str
             Path to directory where models and configs should be saved.
         """
 
         if not save_path:
             save_path = self._save_path if self._save_path else "./"
 
         supported_models = {
@@ -57,25 +57,19 @@
                     models[model_key].append(self._model)
 
         if not models:
             raise NotImplementedError(
                 f"No models available for dump. Current supported models are: {supported_models.keys()}"
             )
 
-        # get tokenizers for hf_text
-        text_processors = self._data_processors.get(TEXT, {})
-        tokenizers = {}
-        for per_processor in text_processors:
-            tokenizers[per_processor.prefix] = per_processor.tokenizer
-
         for model_key in models:
             for per_model in models[model_key]:
                 subdir = os.path.join(save_path, per_model.prefix)
                 os.makedirs(subdir, exist_ok=True)
-                per_model.save(save_path=subdir, tokenizers=tokenizers)
+                per_model.save(save_path=subdir)
 
         return save_path
 
     def export_onnx(
         self,
         data: Union[dict, pd.DataFrame],
         path: Optional[str] = None,
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/few_shot_learning.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/few_shot_learning.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/hpo.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/hpo.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/inference.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/inference.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/label_studio.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/label_studio.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/load.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/load.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 import os
 import pickle
 from typing import Dict, List, Optional, Tuple, Union
 
 from ..constants import LAST_CHECKPOINT, MODEL_CHECKPOINT
 from ..data import DocumentProcessor, NerProcessor, TextProcessor
+from ..models.utils import get_pretrained_tokenizer
 
 logger = logging.getLogger(__name__)
 
 
 def load_text_tokenizers(
     text_processors: Union[List[TextProcessor], List[NerProcessor], List[DocumentProcessor]],
     path: str,
@@ -27,15 +28,15 @@
     Returns
     -------
     A list of text/ner processors with tokenizers loaded.
     """
     for per_text_processor in text_processors:
         if isinstance(per_text_processor.tokenizer, str):
             per_path = os.path.join(path, per_text_processor.tokenizer)
-            per_text_processor.tokenizer = per_text_processor.get_pretrained_tokenizer(
+            per_text_processor.tokenizer = get_pretrained_tokenizer(
                 tokenizer_name=per_text_processor.tokenizer_name,
                 checkpoint_name=per_path,
             )
     return text_processors
 
 
 class CustomUnpickler(pickle.Unpickler):
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/log.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/log.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/matcher.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/matcher.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/metric.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/metric.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/misc.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/misc.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/mmcv.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/mmcv.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/model.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,14 +192,15 @@
     """
     if model_name.lower().startswith(CLIP):
         model = CLIPForImageText(
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             num_classes=num_classes,
             pretrained=pretrained,
+            tokenizer_name=model_config.tokenizer_name,
         )
     elif model_name.lower().startswith(TIMM_IMAGE):
         model = TimmAutoModelForImagePrediction(
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             num_classes=num_classes,
             mix_choice=model_config.mix_choice,
@@ -210,26 +211,29 @@
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             num_classes=num_classes,
             pooling_mode=OmegaConf.select(model_config, "pooling_mode", default="cls"),
             gradient_checkpointing=OmegaConf.select(model_config, "gradient_checkpointing"),
             low_cpu_mem_usage=OmegaConf.select(model_config, "low_cpu_mem_usage", default=False),
             pretrained=pretrained,
+            tokenizer_name=model_config.tokenizer_name,
+            use_fast=OmegaConf.select(model_config, "use_fast", default=True),
         )
     elif model_name.lower().startswith(T_FEW):
         model = TFewModel(
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             length_norm=model_config.length_norm,  # Normalizes length to adjust for length bias in target template
             unlikely_loss=model_config.unlikely_loss,  # Adds loss term that lowers probability of incorrect outputs
             mc_loss=model_config.mc_loss,  # Adds multiple choice cross entropy loss
             num_classes=num_classes,
             gradient_checkpointing=OmegaConf.select(model_config, "gradient_checkpointing"),
             low_cpu_mem_usage=OmegaConf.select(model_config, "low_cpu_mem_usage", default=False),
             pretrained=pretrained,
+            tokenizer_name=model_config.tokenizer_name,
         )
     elif model_name.lower().startswith(NUMERICAL_MLP):
         model = NumericalMLP(
             prefix=model_name,
             in_features=num_numerical_columns,
             hidden_features=model_config.hidden_size,
             out_features=model_config.hidden_size,
@@ -302,14 +306,15 @@
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             num_classes=num_classes,
             pooling_mode=OmegaConf.select(model_config, "pooling_mode", default="cls"),
             gradient_checkpointing=OmegaConf.select(model_config, "gradient_checkpointing"),
             low_cpu_mem_usage=OmegaConf.select(model_config, "low_cpu_mem_usage", default=False),
             pretrained=pretrained,
+            tokenizer_name=model_config.tokenizer_name,
         )
     elif model_name.lower().startswith(MMDET_IMAGE):
         model = MMDetAutoModelForObjectDetection(
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             config_file=OmegaConf.select(model_config, "config_file", default=None),
             classes=classes,
@@ -337,14 +342,15 @@
         model = HFAutoModelForNER(
             prefix=model_name,
             checkpoint_name=model_config.checkpoint_name,
             num_classes=num_classes,
             gradient_checkpointing=OmegaConf.select(model_config, "gradient_checkpointing"),
             low_cpu_mem_usage=OmegaConf.select(model_config, "low_cpu_mem_usage", default=False),
             pretrained=pretrained,
+            tokenizer_name=model_config.tokenizer_name,
         )
     elif model_name.lower().startswith(FUSION_MLP):
         model = functools.partial(
             MultimodalFusionMLP,
             prefix=model_name,
             hidden_features=model_config.hidden_sizes,
             num_classes=num_classes,
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/nlpaug.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/nlpaug.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/object_detection.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/object_detection_visualizer.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/object_detection_visualizer.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/onnx.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/onnx.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/ovd.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/ovd.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/pipeline.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon/multimodal/utils/save.py` & `autogluon.multimodal-0.8.3b20230804/src/autogluon/multimodal/utils/save.py`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/PKG-INFO` & `autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.multimodal
-Version: 0.8.3b20230803
+Version: 0.8.3b20230804
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/SOURCES.txt` & `autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autogluon.multimodal-0.8.3b20230803/src/autogluon.multimodal.egg-info/requires.txt` & `autogluon.multimodal-0.8.3b20230804/src/autogluon.multimodal.egg-info/requires.txt`

 * *Files 9% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 torchvision<0.16.0,>=0.14.0
 scikit-image<0.20.0,>=0.19.1
 text-unidecode<1.4,>=1.3
 torchmetrics<1.1.0,>=1.0.0
 transformers[sentencepiece]<4.27.0,>=4.23.0
 nptyping<2.5.0,>=1.4.4
 omegaconf<2.3.0,>=2.1.1
-autogluon.core[raytune]==0.8.3b20230803
-autogluon.features==0.8.3b20230803
-autogluon.common==0.8.3b20230803
+autogluon.core[raytune]==0.8.3b20230804
+autogluon.features==0.8.3b20230804
+autogluon.common==0.8.3b20230804
 pytorch-metric-learning<2.0,>=1.3.0
 nlpaug<1.2.0,>=1.1.10
 nltk<4.0.0,>=3.4.5
 openmim<0.4.0,>=0.3.7
 defusedxml<0.7.2,>=0.7.1
 jinja2<3.2,>=3.0.3
 tensorboard<3,>=2.9
```

