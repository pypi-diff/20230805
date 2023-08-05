# Comparing `tmp/deeplake-3.6.8.tar.gz` & `tmp/deeplake-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deeplake-3.6.8.tar", last modified: Fri Jul  7 15:36:44 2023, max compression
+gzip compressed data, was "deeplake-3.6.9.tar", last modified: Tue Jul 11 17:36:07 2023, max compression
```

## Comparing `deeplake-3.6.8.tar` & `deeplake-3.6.9.tar`

### file list

```diff
@@ -1,399 +1,399 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/
--rw-r--r--   0 root         (0) root         (0)    15975 2023-07-07 15:35:13.000000 deeplake-3.6.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       36 2023-07-07 15:35:13.000000 deeplake-3.6.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    26013 2023-07-07 15:36:44.987345 deeplake-3.6.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    25284 2023-07-07 15:35:13.000000 deeplake-3.6.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/
--rw-r--r--   0 root         (0) root         (0)     2567 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/api/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100629 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4693 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/info.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/link.py
--rw-r--r--   0 root         (0) root         (0)     1698 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     2703 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/read.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/api/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3038 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_access_method.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_agreement.py
--rw-r--r--   0 root         (0) root         (0)    89755 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_api.py
--rw-r--r--   0 root         (0) root         (0)     6968 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_api_tiling.py
--rw-r--r--   0 root         (0) root         (0)    11668 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_api_with_compression.py
--rw-r--r--   0 root         (0) root         (0)     2654 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_chunk_sizes.py
--rw-r--r--   0 root         (0) root         (0)     2490 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_connect_datasets.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_dicom.py
--rw-r--r--   0 root         (0) root         (0)     6192 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_downsample.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_events.py
--rw-r--r--   0 root         (0) root         (0)     5056 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_grayscale.py
--rw-r--r--   0 root         (0) root         (0)      247 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_hosted_datasets.py
--rw-r--r--   0 root         (0) root         (0)     6513 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_info.py
--rw-r--r--   0 root         (0) root         (0)     6911 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_insertion_out_of_order.py
--rw-r--r--   0 root         (0) root         (0)     6823 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_json.py
--rw-r--r--   0 root         (0) root         (0)    25678 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_link.py
--rw-r--r--   0 root         (0) root         (0)     3293 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_link_tiled.py
--rw-r--r--   0 root         (0) root         (0)     1789 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_linking.py
--rw-r--r--   0 root         (0) root         (0)     1024 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_mesh.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_meta.py
--rw-r--r--   0 root         (0) root         (0)     4109 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_nifti.py
--rw-r--r--   0 root         (0) root         (0)     7900 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_none.py
--rw-r--r--   0 root         (0) root         (0)      952 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_partial_upload.py
--rw-r--r--   0 root         (0) root         (0)     1605 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_pickle.py
--rw-r--r--   0 root         (0) root         (0)     5680 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     4249 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_polygons.py
--rw-r--r--   0 root         (0) root         (0)    10559 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_pop.py
--rw-r--r--   0 root         (0) root         (0)     1577 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)    18861 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_rechunk.py
--rw-r--r--   0 root         (0) root         (0)     8962 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_reset.py
--rw-r--r--   0 root         (0) root         (0)     4578 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_sample_info.py
--rw-r--r--   0 root         (0) root         (0)     2982 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_text.py
--rw-r--r--   0 root         (0) root         (0)    25990 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_update_samples.py
--rw-r--r--   0 root         (0) root         (0)     7499 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_video.py
--rw-r--r--   0 root         (0) root         (0)     4153 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tests/test_views.py
--rw-r--r--   0 root         (0) root         (0)     1368 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/api/tiled.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/auto/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake/auto/structured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/structured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      635 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/structured/base.py
--rw-r--r--   0 root         (0) root         (0)     7081 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/structured/dataframe.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7975 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_coco_template.py
--rw-r--r--   0 root         (0) root         (0)    13490 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     5371 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_kaggle.py
--rw-r--r--   0 root         (0) root         (0)     5519 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/tests/test_yolo_template.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/unstructured/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/__init__.py
--rw-r--r--   0 root         (0) root         (0)      537 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/unstructured/coco/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/coco.py
--rw-r--r--   0 root         (0) root         (0)      669 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/constants.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/convert.py
--rw-r--r--   0 root         (0) root         (0)     5237 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/coco/utils.py
--rw-r--r--   0 root         (0) root         (0)     6693 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/image_classification.py
--rw-r--r--   0 root         (0) root         (0)     3533 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/kaggle.py
--rw-r--r--   0 root         (0) root         (0)     4514 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/auto/unstructured/yolo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/__init__.py
--rw-r--r--   0 root         (0) root         (0)      278 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/constants.py
--rw-r--r--   0 root         (0) root         (0)     7394 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/utils.py
--rw-r--r--   0 root         (0) root         (0)    12937 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/auto/unstructured/yolo/yolo.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/cli/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5913 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/auth.py
--rw-r--r--   0 root         (0) root         (0)      410 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/commands.py
--rw-r--r--   0 root         (0) root         (0)      931 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/cli/test_cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/client/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19099 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/client.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/config.py
--rw-r--r--   0 root         (0) root         (0)      690 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/log.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/test_client.py
--rw-r--r--   0 root         (0) root         (0)     3324 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/client/utils.py
--rw-r--r--   0 root         (0) root         (0)     3876 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/compression.py
--rw-r--r--   0 root         (0) root         (0)     7420 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/
--rw-r--r--   0 root         (0) root         (0)       23 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/chunk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24150 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/base_chunk.py
--rw-r--r--   0 root         (0) root         (0)    25311 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/chunk_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     6147 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/sample_compressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)     4926 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/test_chunk_compressed.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/test_sample_compressed.py
--rw-r--r--   0 root         (0) root         (0)     5446 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/test_uncompressed.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk/uncompressed_chunk.py
--rw-r--r--   0 root         (0) root         (0)   118602 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)    39478 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compression.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/compute/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/__init__.py
--rw-r--r--   0 root         (0) root         (0)      911 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/process.py
--rw-r--r--   0 root         (0) root         (0)     2332 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/provider.py
--rw-r--r--   0 root         (0) root         (0)      640 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/ray.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/serial.py
--rw-r--r--   0 root         (0) root         (0)      576 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/compute/thread.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/dataset/
--rw-r--r--   0 root         (0) root         (0)      903 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)   181668 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    15791 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/deeplake_cloud_dataset.py
--rw-r--r--   0 root         (0) root         (0)    11965 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/deeplake_query_dataset.py
--rw-r--r--   0 root         (0) root         (0)     5265 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/deeplake_query_tensor.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/invalid_view.py
--rw-r--r--   0 root         (0) root         (0)     4769 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/dataset/view_entry.py
--rw-r--r--   0 root         (0) root         (0)     4348 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/fast_forwarding.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/index/
--rw-r--r--   0 root         (0) root         (0)      138 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/index/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17507 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/index/index.py
--rw-r--r--   0 root         (0) root         (0)    20369 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/io.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/ipc.py
--rw-r--r--   0 root         (0) root         (0)    13074 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/link_creds.py
--rw-r--r--   0 root         (0) root         (0)    16043 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/linked_chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     2277 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/linked_sample.py
--rw-r--r--   0 root         (0) root         (0)     2597 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/linked_tiled_sample.py
--rw-r--r--   0 root         (0) root         (0)     8835 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/lock.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/meta/
--rw-r--r--   0 root         (0) root         (0)       97 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3595 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/dataset_meta.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/meta/encode/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25591 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/base_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/byte_positions.py
--rw-r--r--   0 root         (0) root         (0)    13495 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/chunk_id.py
--rw-r--r--   0 root         (0) root         (0)     1551 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/creds.py
--rw-r--r--   0 root         (0) root         (0)     3972 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/pad.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/sequence.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/shape.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/meta/encode/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      226 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     2237 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
--rw-r--r--   0 root         (0) root         (0)     1452 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     2114 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
--rw-r--r--   0 root         (0) root         (0)     3673 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder.py
--rw-r--r--   0 root         (0) root         (0)     2810 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
--rw-r--r--   0 root         (0) root         (0)     7515 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/encode/tile.py
--rw-r--r--   0 root         (0) root         (0)      503 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/meta.py
--rw-r--r--   0 root         (0) root         (0)    13344 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/meta/tensor_meta.py
--rw-r--r--   0 root         (0) root         (0)      906 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/partial_reader.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/partial_sample.py
--rw-r--r--   0 root         (0) root         (0)     5269 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/polygon.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/query/
--rw-r--r--   0 root         (0) root         (0)       82 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12021 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/autocomplete.py
--rw-r--r--   0 root         (0) root         (0)    14326 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/filter.py
--rw-r--r--   0 root         (0) root         (0)     8905 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/query/query.py
--rw-r--r--   0 root         (0) root         (0)    20658 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/sample.py
--rw-r--r--   0 root         (0) root         (0)    22849 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/storage/
--rw-r--r--   0 root         (0) root         (0)      495 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13833 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/azure.py
--rw-r--r--   0 root         (0) root         (0)     1053 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/deeplake_memory_object.py
--rw-r--r--   0 root         (0) root         (0)    19080 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/gcs.py
--rw-r--r--   0 root         (0) root         (0)    13053 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/google_drive.py
--rw-r--r--   0 root         (0) root         (0)     8347 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/local.py
--rw-r--r--   0 root         (0) root         (0)    19492 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/lru_cache.py
--rw-r--r--   0 root         (0) root         (0)     3705 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/memory.py
--rw-r--r--   0 root         (0) root         (0)     7111 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/provider.py
--rw-r--r--   0 root         (0) root         (0)    25799 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/storage/s3.py
--rw-r--r--   0 root         (0) root         (0)    50495 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tensor.py
--rw-r--r--   0 root         (0) root         (0)     7485 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tensor_link.py
--rw-r--r--   0 root         (0) root         (0)     5152 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7602 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_compression.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_compute.py
--rw-r--r--   0 root         (0) root         (0)    12917 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_deeplake_indra_dataset.py
--rw-r--r--   0 root         (0) root         (0)      913 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_io.py
--rw-r--r--   0 root         (0) root         (0)     4312 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_locking.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_readonly.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tests/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/tiling/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4790 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/deserialize.py
--rw-r--r--   0 root         (0) root         (0)     1701 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/optimizer.py
--rw-r--r--   0 root         (0) root         (0)     4731 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/sample_tiles.py
--rw-r--r--   0 root         (0) root         (0)     2893 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/serialize.py
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/test_optimizer.py
--rw-r--r--   0 root         (0) root         (0)     2367 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/tiling/test_serialize.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.967345 deeplake-3.6.8/deeplake/core/transform/
--rw-r--r--   0 root         (0) root         (0)      111 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52842 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/test_transform.py
--rw-r--r--   0 root         (0) root         (0)    29645 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/transform.py
--rw-r--r--   0 root         (0) root         (0)     5970 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/transform_dataset.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/transform/transform_tensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/
--rw-r--r--   0 root         (0) root         (0)      682 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26865 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/deeplake_vectorstore.py
--rw-r--r--   0 root         (0) root         (0)    38773 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/
--rw-r--r--   0 root         (0) root         (0)      330 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15186 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py
--rw-r--r--   0 root         (0) root         (0)    11509 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/
--rw-r--r--   0 root         (0) root         (0)      286 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3212 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/filter.py
--rw-r--r--   0 root         (0) root         (0)     3542 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4511 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/query.py
--rw-r--r--   0 root         (0) root         (0)     2562 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1795 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
--rw-r--r--   0 root         (0) root         (0)      275 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)      781 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
--rw-r--r--   0 root         (0) root         (0)      186 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
--rw-r--r--   0 root         (0) root         (0)     1512 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/
--rw-r--r--   0 root         (0) root         (0)       93 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6949 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
--rw-r--r--   0 root         (0) root         (0)     2047 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
--rw-r--r--   0 root         (0) root         (0)     5040 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1924 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
--rw-r--r--   0 root         (0) root         (0)     1886 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
--rw-r--r--   0 root         (0) root         (0)     1557 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/vector_search.py
--rw-r--r--   0 root         (0) root         (0)    13192 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/utils.py
--rw-r--r--   0 root         (0) root         (0)     3399 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/vectorstore/vector_search/vector_search.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/core/version_control/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1954 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/commit_chunk_map.py
--rw-r--r--   0 root         (0) root         (0)     6337 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/commit_diff.py
--rw-r--r--   0 root         (0) root         (0)     3109 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/commit_node.py
--rw-r--r--   0 root         (0) root         (0)     4828 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/dataset_diff.py
--rw-r--r--   0 root         (0) root         (0)    19869 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/test_merge.py
--rw-r--r--   0 root         (0) root         (0)    84800 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/core/version_control/test_version_control.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/enterprise/
--rw-r--r--   0 root         (0) root         (0)      257 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7381 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/convert_to_libdeeplake.py
--rw-r--r--   0 root         (0) root         (0)    29584 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/dataloader.py
--rw-r--r--   0 root         (0) root         (0)     6010 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/dummy_dataloader.py
--rw-r--r--   0 root         (0) root         (0)     4391 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/libdeeplake_query.py
--rw-r--r--   0 root         (0) root         (0)    25912 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/test_pytorch.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/test_query.py
--rw-r--r--   0 root         (0) root         (0)    22454 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/test_tensorflow.py
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/enterprise/util.py
--rw-r--r--   0 root         (0) root         (0)     1590 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/hooks.py
--rw-r--r--   0 root         (0) root         (0)     5050 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/htype.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/
--rw-r--r--   0 root         (0) root         (0)       99 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/huggingface/
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/huggingface/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5503 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/huggingface/huggingface.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/mmdet/
--rw-r--r--   0 root         (0) root         (0)      118 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/__init__.py
--rw-r--r--   0 root         (0) root         (0)    62754 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_.py
--rw-r--r--   0 root         (0) root         (0)     4739 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_runners.py
--rw-r--r--   0 root         (0) root         (0)    19660 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/pytorch/
--rw-r--r--   0 root         (0) root         (0)       40 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9862 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/common.py
--rw-r--r--   0 root         (0) root         (0)     7317 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4424 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/pytorch.py
--rw-r--r--   0 root         (0) root         (0)     6919 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/pytorch/shuffle_buffer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/tf/
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1270 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/common.py
--rw-r--r--   0 root         (0) root         (0)     2453 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/datasettotensorflow.py
--rw-r--r--   0 root         (0) root         (0)     5330 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/integrations/wandb/
--rw-r--r--   0 root         (0) root         (0)       21 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/wandb/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12089 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/integrations/wandb/wandb.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/requirements/
--rw-r--r--   0 root         (0) root         (0)      476 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/common.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/docs.txt
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/plugins.txt
--rw-r--r--   0 root         (0) root         (0)      304 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/requirements/tests.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.977345 deeplake-3.6.8/deeplake/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1404 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/cache_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2554 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/client_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/common.py
--rw-r--r--   0 root         (0) root         (0)     4304 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/dataset_fixtures.py
--rw-r--r--   0 root         (0) root         (0)    16369 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/path_fixtures.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/tests/storage_fixtures.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/util/
--rw-r--r--   0 root         (0) root         (0)       86 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3531 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/access_method.py
--rw-r--r--   0 root         (0) root         (0)     1130 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/agreement.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/array_list.py
--rw-r--r--   0 root         (0) root         (0)      619 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/assert_byte_indexes.py
--rw-r--r--   0 root         (0) root         (0)     2961 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/auto.py
--rw-r--r--   0 root         (0) root         (0)     5740 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/bugout_reporter.py
--rw-r--r--   0 root         (0) root         (0)       54 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/bugout_token.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/cache_chain.py
--rw-r--r--   0 root         (0) root         (0)     4494 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/casting.py
--rw-r--r--   0 root         (0) root         (0)      310 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/check_installation.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/check_latest_version.py
--rw-r--r--   0 root         (0) root         (0)     3151 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/chunk_engine.py
--rw-r--r--   0 root         (0) root         (0)     4597 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/class_label.py
--rw-r--r--   0 root         (0) root         (0)      231 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/compression.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/compute.py
--rw-r--r--   0 root         (0) root         (0)     5404 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1170 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/dataset.py
--rw-r--r--   0 root         (0) root         (0)      443 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/delete_entry.py
--rw-r--r--   0 root         (0) root         (0)    15912 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/diff.py
--rw-r--r--   0 root         (0) root         (0)     4945 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/downsample.py
--rw-r--r--   0 root         (0) root         (0)       84 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/empty_sample.py
--rw-r--r--   0 root         (0) root         (0)    15682 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/encoder.py
--rw-r--r--   0 root         (0) root         (0)    35113 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/exif.py
--rw-r--r--   0 root         (0) root         (0)     1819 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/from_tfds.py
--rw-r--r--   0 root         (0) root         (0)      136 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/generate_id.py
--rw-r--r--   0 root         (0) root         (0)      306 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/hash.py
--rw-r--r--   0 root         (0) root         (0)     2799 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/htype.py
--rw-r--r--   0 root         (0) root         (0)     1517 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/image.py
--rw-r--r--   0 root         (0) root         (0)      873 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/invalid_view_op.py
--rw-r--r--   0 root         (0) root         (0)      135 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)     1001 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/iteration_warning.py
--rw-r--r--   0 root         (0) root         (0)      507 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/join_chunks.py
--rw-r--r--   0 root         (0) root         (0)     6422 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/json.py
--rw-r--r--   0 root         (0) root         (0)     7549 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/keys.py
--rw-r--r--   0 root         (0) root         (0)     3071 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/link.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/logging.py
--rw-r--r--   0 root         (0) root         (0)    37497 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/merge.py
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/modified.py
--rw-r--r--   0 root         (0) root         (0)      903 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/notebook.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/util/object_3d/
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3374 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/mesh.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/mesh_parser.py
--rw-r--r--   0 root         (0) root         (0)      185 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/mesh_reader.py
--rw-r--r--   0 root         (0) root         (0)     1021 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/object_base_3d.py
--rw-r--r--   0 root         (0) root         (0)      695 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_parser.py
--rw-r--r--   0 root         (0) root         (0)     1323 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_parser_base.py
--rw-r--r--   0 root         (0) root         (0)     6188 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_parsers.py
--rw-r--r--   0 root         (0) root         (0)     1663 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_reader.py
--rw-r--r--   0 root         (0) root         (0)     3221 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_reader_base.py
--rw-r--r--   0 root         (0) root         (0)    10213 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/ply_readers.py
--rw-r--r--   0 root         (0) root         (0)     7187 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/point_cloud.py
--rw-r--r--   0 root         (0) root         (0)     1160 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/object_3d/read_3d_data.py
--rw-r--r--   0 root         (0) root         (0)     3986 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/path.py
--rw-r--r--   0 root         (0) root         (0)     3220 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/pretty_print.py
--rw-r--r--   0 root         (0) root         (0)     2763 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/remove_cache.py
--rw-r--r--   0 root         (0) root         (0)     4137 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/scheduling.py
--rw-r--r--   0 root         (0) root         (0)     3140 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      182 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     4204 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/spinner.py
--rw-r--r--   0 root         (0) root         (0)     1153 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/split.py
--rw-r--r--   0 root         (0) root         (0)     8767 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/storage.py
--rw-r--r--   0 root         (0) root         (0)     1131 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tag.py
--rw-r--r--   0 root         (0) root         (0)     1425 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      951 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/testing.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/util/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1476 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_auto.py
--rw-r--r--   0 root         (0) root         (0)     1757 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_connect_dataset.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_iterable_ordered_dict.py
--rw-r--r--   0 root         (0) root         (0)      628 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_keys.py
--rw-r--r--   0 root         (0) root         (0)      892 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_read.py
--rw-r--r--   0 root         (0) root         (0)     1071 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_shape_interval.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_shuffle.py
--rw-r--r--   0 root         (0) root         (0)      698 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_split.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_tensor_db.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_token.py
--rw-r--r--   0 root         (0) root         (0)     2428 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/tests/test_version_control.py
--rw-r--r--   0 root         (0) root         (0)      276 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/threading.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/token.py
--rw-r--r--   0 root         (0) root         (0)    25277 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/transform.py
--rw-r--r--   0 root         (0) root         (0)    31615 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/version_control.py
--rw-r--r--   0 root         (0) root         (0)      927 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/video.py
--rw-r--r--   0 root         (0) root         (0)      167 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/util/warnings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.987345 deeplake-3.6.8/deeplake/visualizer/
--rw-r--r--   0 root         (0) root         (0)       34 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/visualizer/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6466 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/visualizer/video_streaming.py
--rw-r--r--   0 root         (0) root         (0)     6722 2023-07-07 15:35:13.000000 deeplake-3.6.8/deeplake/visualizer/visualizer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-07 15:36:44.957345 deeplake-3.6.8/deeplake.egg-info/
--rw-r--r--   0 root         (0) root         (0)    26013 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12710 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       58 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)     1075 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-07 15:36:44.000000 deeplake-3.6.8/deeplake.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      311 2023-07-07 15:36:44.987345 deeplake-3.6.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     3357 2023-07-07 15:35:13.000000 deeplake-3.6.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.324043 deeplake-3.6.9/
+-rw-r--r--   0 root         (0) root         (0)    15975 2023-07-11 17:34:53.000000 deeplake-3.6.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       36 2023-07-11 17:34:53.000000 deeplake-3.6.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    26013 2023-07-11 17:36:07.324043 deeplake-3.6.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    25284 2023-07-11 17:34:53.000000 deeplake-3.6.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.294043 deeplake-3.6.9/deeplake/
+-rw-r--r--   0 root         (0) root         (0)     2567 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.294043 deeplake-3.6.9/deeplake/api/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   101672 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4693 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/info.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/link.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     2703 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/read.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/api/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3038 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_access_method.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_agreement.py
+-rw-r--r--   0 root         (0) root         (0)    89755 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)     6968 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_api_tiling.py
+-rw-r--r--   0 root         (0) root         (0)    11668 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_api_with_compression.py
+-rw-r--r--   0 root         (0) root         (0)     2654 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_chunk_sizes.py
+-rw-r--r--   0 root         (0) root         (0)     2490 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_connect_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_dicom.py
+-rw-r--r--   0 root         (0) root         (0)     6192 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_downsample.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_events.py
+-rw-r--r--   0 root         (0) root         (0)     5056 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_grayscale.py
+-rw-r--r--   0 root         (0) root         (0)      247 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_hosted_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     6513 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_info.py
+-rw-r--r--   0 root         (0) root         (0)     6911 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_insertion_out_of_order.py
+-rw-r--r--   0 root         (0) root         (0)     6823 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_json.py
+-rw-r--r--   0 root         (0) root         (0)    25678 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_link.py
+-rw-r--r--   0 root         (0) root         (0)     3293 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_link_tiled.py
+-rw-r--r--   0 root         (0) root         (0)     1789 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_linking.py
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_mesh.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_meta.py
+-rw-r--r--   0 root         (0) root         (0)     4109 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_nifti.py
+-rw-r--r--   0 root         (0) root         (0)     7900 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_none.py
+-rw-r--r--   0 root         (0) root         (0)      952 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_partial_upload.py
+-rw-r--r--   0 root         (0) root         (0)     1605 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_pickle.py
+-rw-r--r--   0 root         (0) root         (0)     5680 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     4249 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_polygons.py
+-rw-r--r--   0 root         (0) root         (0)    10559 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_pop.py
+-rw-r--r--   0 root         (0) root         (0)     1577 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)    18861 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_rechunk.py
+-rw-r--r--   0 root         (0) root         (0)     8962 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_reset.py
+-rw-r--r--   0 root         (0) root         (0)     4578 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_sample_info.py
+-rw-r--r--   0 root         (0) root         (0)     2982 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_text.py
+-rw-r--r--   0 root         (0) root         (0)    25990 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_update_samples.py
+-rw-r--r--   0 root         (0) root         (0)     7499 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_video.py
+-rw-r--r--   0 root         (0) root         (0)     4153 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tests/test_views.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/api/tiled.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/auto/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/auto/structured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/structured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      635 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/structured/base.py
+-rw-r--r--   0 root         (0) root         (0)     7081 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/structured/dataframe.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/auto/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7975 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/tests/test_coco_template.py
+-rw-r--r--   0 root         (0) root         (0)    13490 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/tests/test_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     5371 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/tests/test_kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     5519 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/tests/test_yolo_template.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/auto/unstructured/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      537 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/auto/unstructured/coco/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/coco/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/coco/coco.py
+-rw-r--r--   0 root         (0) root         (0)      669 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/coco/constants.py
+-rw-r--r--   0 root         (0) root         (0)     1709 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/coco/convert.py
+-rw-r--r--   0 root         (0) root         (0)     5237 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/coco/utils.py
+-rw-r--r--   0 root         (0) root         (0)     6693 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/image_classification.py
+-rw-r--r--   0 root         (0) root         (0)     3533 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/kaggle.py
+-rw-r--r--   0 root         (0) root         (0)     4514 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/auto/unstructured/yolo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/yolo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      278 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/yolo/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7394 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/yolo/utils.py
+-rw-r--r--   0 root         (0) root         (0)    12937 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/auto/unstructured/yolo/yolo.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/cli/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5913 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/cli/auth.py
+-rw-r--r--   0 root         (0) root         (0)      410 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/cli/commands.py
+-rw-r--r--   0 root         (0) root         (0)      931 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/cli/test_cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/client/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18981 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/client/config.py
+-rw-r--r--   0 root         (0) root         (0)      690 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/client/log.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/client/test_client.py
+-rw-r--r--   0 root         (0) root         (0)     3324 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/compression.py
+-rw-r--r--   0 root         (0) root         (0)     7420 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/chunk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24150 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/base_chunk.py
+-rw-r--r--   0 root         (0) root         (0)    25311 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/chunk_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     6147 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/sample_compressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)     4926 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/test_chunk_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/test_sample_compressed.py
+-rw-r--r--   0 root         (0) root         (0)     5446 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/test_uncompressed.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk/uncompressed_chunk.py
+-rw-r--r--   0 root         (0) root         (0)   118602 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)    39478 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compression.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/compute/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compute/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      911 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compute/process.py
+-rw-r--r--   0 root         (0) root         (0)     2332 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compute/provider.py
+-rw-r--r--   0 root         (0) root         (0)      640 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compute/ray.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compute/serial.py
+-rw-r--r--   0 root         (0) root         (0)      576 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/compute/thread.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/dataset/
+-rw-r--r--   0 root         (0) root         (0)      903 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   181487 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    15791 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/deeplake_cloud_dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11965 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/deeplake_query_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     5265 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/deeplake_query_tensor.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/invalid_view.py
+-rw-r--r--   0 root         (0) root         (0)     4769 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/dataset/view_entry.py
+-rw-r--r--   0 root         (0) root         (0)     4348 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/fast_forwarding.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/index/
+-rw-r--r--   0 root         (0) root         (0)      138 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/index/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17507 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/index/index.py
+-rw-r--r--   0 root         (0) root         (0)    20369 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/io.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/ipc.py
+-rw-r--r--   0 root         (0) root         (0)    13074 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/link_creds.py
+-rw-r--r--   0 root         (0) root         (0)    16043 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/linked_chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     2277 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/linked_sample.py
+-rw-r--r--   0 root         (0) root         (0)     2597 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/linked_tiled_sample.py
+-rw-r--r--   0 root         (0) root         (0)     9146 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/lock.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/meta/
+-rw-r--r--   0 root         (0) root         (0)       97 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/dataset_meta.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.304043 deeplake-3.6.9/deeplake/core/meta/encode/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25591 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/base_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/byte_positions.py
+-rw-r--r--   0 root         (0) root         (0)    13495 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/chunk_id.py
+-rw-r--r--   0 root         (0) root         (0)     1551 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/creds.py
+-rw-r--r--   0 root         (0) root         (0)     3972 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/pad.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/sequence.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/shape.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/meta/encode/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      226 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     2237 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     2114 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     3673 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/test_shape_encoder.py
+-rw-r--r--   0 root         (0) root         (0)     2810 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py
+-rw-r--r--   0 root         (0) root         (0)     7515 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/encode/tile.py
+-rw-r--r--   0 root         (0) root         (0)      503 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/meta.py
+-rw-r--r--   0 root         (0) root         (0)    13344 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/meta/tensor_meta.py
+-rw-r--r--   0 root         (0) root         (0)      906 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/partial_reader.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/partial_sample.py
+-rw-r--r--   0 root         (0) root         (0)     5269 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/polygon.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/query/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/query/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12021 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/query/autocomplete.py
+-rw-r--r--   0 root         (0) root         (0)    14326 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/query/filter.py
+-rw-r--r--   0 root         (0) root         (0)     8905 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/query/query.py
+-rw-r--r--   0 root         (0) root         (0)    20658 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/sample.py
+-rw-r--r--   0 root         (0) root         (0)    22849 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/storage/
+-rw-r--r--   0 root         (0) root         (0)      495 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13833 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/azure.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/deeplake_memory_object.py
+-rw-r--r--   0 root         (0) root         (0)    19080 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/gcs.py
+-rw-r--r--   0 root         (0) root         (0)    13053 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/google_drive.py
+-rw-r--r--   0 root         (0) root         (0)     8347 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/local.py
+-rw-r--r--   0 root         (0) root         (0)    19492 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/lru_cache.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/memory.py
+-rw-r--r--   0 root         (0) root         (0)     7111 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/provider.py
+-rw-r--r--   0 root         (0) root         (0)    25799 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/storage/s3.py
+-rw-r--r--   0 root         (0) root         (0)    50495 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tensor.py
+-rw-r--r--   0 root         (0) root         (0)     7485 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tensor_link.py
+-rw-r--r--   0 root         (0) root         (0)     5152 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7602 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_compression.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_compute.py
+-rw-r--r--   0 root         (0) root         (0)    12917 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_deeplake_indra_dataset.py
+-rw-r--r--   0 root         (0) root         (0)      913 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     4312 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_locking.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_readonly.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tests/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/tiling/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4790 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/deserialize.py
+-rw-r--r--   0 root         (0) root         (0)     1701 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     4731 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/sample_tiles.py
+-rw-r--r--   0 root         (0) root         (0)     2893 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/serialize.py
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/test_optimizer.py
+-rw-r--r--   0 root         (0) root         (0)     2367 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/tiling/test_serialize.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/transform/
+-rw-r--r--   0 root         (0) root         (0)      111 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/transform/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52842 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/transform/test_transform.py
+-rw-r--r--   0 root         (0) root         (0)    29645 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/transform/transform.py
+-rw-r--r--   0 root         (0) root         (0)     5970 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/transform/transform_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/transform/transform_tensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/
+-rw-r--r--   0 root         (0) root         (0)      682 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27385 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/deeplake_vectorstore.py
+-rw-r--r--   0 root         (0) root         (0)    39034 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/test_deeplake_vectorstore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/dataset/
+-rw-r--r--   0 root         (0) root         (0)      330 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/dataset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15186 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/dataset/dataset.py
+-rw-r--r--   0 root         (0) root         (0)    11509 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/filter/
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/filter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/filter/filter.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/filter/test_filter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/query.py
+-rw-r--r--   0 root         (0) root         (0)     2562 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1795 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/test_indra.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/
+-rw-r--r--   0 root         (0) root         (0)      275 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      781 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py
+-rw-r--r--   0 root         (0) root         (0)      186 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/order.py
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6949 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py
+-rw-r--r--   0 root         (0) root         (0)     5040 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/search_algorithm.py
+-rw-r--r--   0 root         (0) root         (0)     1886 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/test_vector_search.py
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/vector_search.py
+-rw-r--r--   0 root         (0) root         (0)    13192 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3399 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/vectorstore/vector_search/vector_search.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/core/version_control/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1954 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/commit_chunk_map.py
+-rw-r--r--   0 root         (0) root         (0)     6337 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/commit_diff.py
+-rw-r--r--   0 root         (0) root         (0)     3109 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/commit_node.py
+-rw-r--r--   0 root         (0) root         (0)     4944 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/dataset_diff.py
+-rw-r--r--   0 root         (0) root         (0)    19869 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/test_merge.py
+-rw-r--r--   0 root         (0) root         (0)    84800 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/core/version_control/test_version_control.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/enterprise/
+-rw-r--r--   0 root         (0) root         (0)      257 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7381 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/convert_to_libdeeplake.py
+-rw-r--r--   0 root         (0) root         (0)    29584 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     6010 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/dummy_dataloader.py
+-rw-r--r--   0 root         (0) root         (0)     4391 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/libdeeplake_query.py
+-rw-r--r--   0 root         (0) root         (0)    25912 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/test_pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/test_query.py
+-rw-r--r--   0 root         (0) root         (0)    22454 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/test_tensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/enterprise/util.py
+-rw-r--r--   0 root         (0) root         (0)     1590 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/hooks.py
+-rw-r--r--   0 root         (0) root         (0)     5050 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/htype.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/integrations/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/integrations/huggingface/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/huggingface/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5503 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/huggingface/huggingface.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/integrations/mmdet/
+-rw-r--r--   0 root         (0) root         (0)      118 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/mmdet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    62754 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/mmdet/mmdet_.py
+-rw-r--r--   0 root         (0) root         (0)     4739 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/mmdet/mmdet_runners.py
+-rw-r--r--   0 root         (0) root         (0)    19660 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/mmdet/mmdet_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/integrations/pytorch/
+-rw-r--r--   0 root         (0) root         (0)       40 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/pytorch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9862 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/pytorch/common.py
+-rw-r--r--   0 root         (0) root         (0)     7317 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/pytorch/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4424 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/pytorch/pytorch.py
+-rw-r--r--   0 root         (0) root         (0)     6919 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/pytorch/shuffle_buffer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/integrations/tf/
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/tf/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/tf/common.py
+-rw-r--r--   0 root         (0) root         (0)     2453 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/tf/datasettotensorflow.py
+-rw-r--r--   0 root         (0) root         (0)     5330 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/integrations/wandb/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/wandb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12089 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/integrations/wandb/wandb.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/requirements/
+-rw-r--r--   0 root         (0) root         (0)      476 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/requirements/common.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/requirements/docs.txt
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/requirements/plugins.txt
+-rw-r--r--   0 root         (0) root         (0)      304 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/requirements/tests.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.314043 deeplake-3.6.9/deeplake/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1404 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/cache_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2554 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/client_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/common.py
+-rw-r--r--   0 root         (0) root         (0)     4304 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/dataset_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)    16369 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/path_fixtures.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/tests/storage_fixtures.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.324043 deeplake-3.6.9/deeplake/util/
+-rw-r--r--   0 root         (0) root         (0)       86 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3531 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/access_method.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/agreement.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/array_list.py
+-rw-r--r--   0 root         (0) root         (0)      619 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/assert_byte_indexes.py
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/auto.py
+-rw-r--r--   0 root         (0) root         (0)     5740 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/bugout_reporter.py
+-rw-r--r--   0 root         (0) root         (0)       54 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/bugout_token.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/cache_chain.py
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/casting.py
+-rw-r--r--   0 root         (0) root         (0)      310 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/check_installation.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/check_latest_version.py
+-rw-r--r--   0 root         (0) root         (0)     3151 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/chunk_engine.py
+-rw-r--r--   0 root         (0) root         (0)     4597 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/class_label.py
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/compression.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/compute.py
+-rw-r--r--   0 root         (0) root         (0)     5404 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/dataset.py
+-rw-r--r--   0 root         (0) root         (0)      443 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/delete_entry.py
+-rw-r--r--   0 root         (0) root         (0)    15912 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/diff.py
+-rw-r--r--   0 root         (0) root         (0)     4945 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/downsample.py
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/empty_sample.py
+-rw-r--r--   0 root         (0) root         (0)    15682 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/encoder.py
+-rw-r--r--   0 root         (0) root         (0)    35113 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/exif.py
+-rw-r--r--   0 root         (0) root         (0)     1819 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/from_tfds.py
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/generate_id.py
+-rw-r--r--   0 root         (0) root         (0)      306 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/hash.py
+-rw-r--r--   0 root         (0) root         (0)     2799 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/htype.py
+-rw-r--r--   0 root         (0) root         (0)     1517 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/image.py
+-rw-r--r--   0 root         (0) root         (0)      873 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/invalid_view_op.py
+-rw-r--r--   0 root         (0) root         (0)      135 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/iteration_warning.py
+-rw-r--r--   0 root         (0) root         (0)      507 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/join_chunks.py
+-rw-r--r--   0 root         (0) root         (0)     6422 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/json.py
+-rw-r--r--   0 root         (0) root         (0)     7549 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/keys.py
+-rw-r--r--   0 root         (0) root         (0)     3071 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/link.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/logging.py
+-rw-r--r--   0 root         (0) root         (0)    37497 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/merge.py
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/modified.py
+-rw-r--r--   0 root         (0) root         (0)      903 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/notebook.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.324043 deeplake-3.6.9/deeplake/util/object_3d/
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3374 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/mesh.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/mesh_parser.py
+-rw-r--r--   0 root         (0) root         (0)      185 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/mesh_reader.py
+-rw-r--r--   0 root         (0) root         (0)     1021 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/object_base_3d.py
+-rw-r--r--   0 root         (0) root         (0)      695 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/ply_parser.py
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/ply_parser_base.py
+-rw-r--r--   0 root         (0) root         (0)     6188 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/ply_parsers.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/ply_reader.py
+-rw-r--r--   0 root         (0) root         (0)     3221 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/ply_reader_base.py
+-rw-r--r--   0 root         (0) root         (0)    10213 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/ply_readers.py
+-rw-r--r--   0 root         (0) root         (0)     7187 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/point_cloud.py
+-rw-r--r--   0 root         (0) root         (0)     1160 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/object_3d/read_3d_data.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/path.py
+-rw-r--r--   0 root         (0) root         (0)     3220 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/pretty_print.py
+-rw-r--r--   0 root         (0) root         (0)     2763 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/remove_cache.py
+-rw-r--r--   0 root         (0) root         (0)     4137 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/scheduling.py
+-rw-r--r--   0 root         (0) root         (0)     3140 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      182 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     4204 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/spinner.py
+-rw-r--r--   0 root         (0) root         (0)     1153 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/split.py
+-rw-r--r--   0 root         (0) root         (0)     8767 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/storage.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tag.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/testing.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.324043 deeplake-3.6.9/deeplake/util/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1476 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_auto.py
+-rw-r--r--   0 root         (0) root         (0)     1757 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_connect_dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_iterable_ordered_dict.py
+-rw-r--r--   0 root         (0) root         (0)      628 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_keys.py
+-rw-r--r--   0 root         (0) root         (0)      892 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_read.py
+-rw-r--r--   0 root         (0) root         (0)     1071 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_shape_interval.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)      698 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_split.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_tensor_db.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_token.py
+-rw-r--r--   0 root         (0) root         (0)     2428 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/tests/test_version_control.py
+-rw-r--r--   0 root         (0) root         (0)      276 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/threading.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/token.py
+-rw-r--r--   0 root         (0) root         (0)    25277 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/transform.py
+-rw-r--r--   0 root         (0) root         (0)    31615 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/version_control.py
+-rw-r--r--   0 root         (0) root         (0)      927 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/video.py
+-rw-r--r--   0 root         (0) root         (0)      167 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/util/warnings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.324043 deeplake-3.6.9/deeplake/visualizer/
+-rw-r--r--   0 root         (0) root         (0)       34 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/visualizer/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6466 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/visualizer/video_streaming.py
+-rw-r--r--   0 root         (0) root         (0)     6722 2023-07-11 17:34:53.000000 deeplake-3.6.9/deeplake/visualizer/visualizer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-11 17:36:07.294043 deeplake-3.6.9/deeplake.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    26013 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12710 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       58 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-11 17:36:07.000000 deeplake-3.6.9/deeplake.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      311 2023-07-11 17:36:07.324043 deeplake-3.6.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     3357 2023-07-11 17:34:53.000000 deeplake-3.6.9/setup.py
```

### Comparing `deeplake-3.6.8/LICENSE` & `deeplake-3.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/PKG-INFO` & `deeplake-3.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.8
+Version: 3.6.9
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.8 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.9 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.8/README.md` & `deeplake-3.6.9/README.md`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/__init__.py` & `deeplake-3.6.9/deeplake/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     "config",
     "delete",
     "copy",
     "rename",
 ]
 
 
-__version__ = "3.6.8"
+__version__ = "3.6.9"
 warn_if_update_required(__version__)
 __encoded_version__ = np.array(__version__)
 config = {"s3": Config(max_pool_connections=50, connect_timeout=300, read_timeout=300)}
 
 
 deeplake_reporter.tags.append(f"version:{__version__}")
```

### Comparing `deeplake-3.6.8/deeplake/api/dataset.py` & `deeplake-3.6.9/deeplake/api/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,14 +91,16 @@
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
         reset: bool = False,
         check_integrity: bool = True,
+        lock_enabled: Optional[bool] = True,
+        lock_timeout: Optional[int] = 0,
     ):
         """Returns a :class:`~deeplake.core.dataset.Dataset` object referencing either a new or existing dataset.
 
         Examples:
 
             >>> ds = deeplake.dataset("hub://username/dataset")
             >>> ds = deeplake.dataset("s3://mybucket/my_dataset")
@@ -158,14 +160,16 @@
                         - Raises an exception if ``DEEPLAKE_DOWNLOAD_PATH`` environment variable is not set.
                         - The 'local' access method can be modified to specify num_workers and/or scheduler to be used in case dataset needs to be downloaded.
                           If dataset needs to be downloaded, 'local:2:processed' will use 2 workers and use processed scheduler, while 'local:3' will use 3 workers
                           and default scheduler (threaded), and 'local:processed' will use a single worker and use processed scheduler.
             reset (bool): If the specified dataset cannot be loaded due to a corrupted HEAD state of the branch being loaded,
                           setting ``reset=True`` will reset HEAD changes and load the previous version.
             check_integrity (bool): If the param is True it will do integrity check during dataset loading otherwise the check is not performed
+            lock_timeout (int): Number of seconds to wait before throwing a LockException. If None, wait indefinitely
+            lock_enabled (bool): If true, the dataset manages a write lock. NOTE: Only set to False if you are managing concurrent access externally
 
         ..
             # noqa: DAR101
 
         Returns:
             Dataset: Dataset created using the arguments provided.
 
@@ -238,14 +242,16 @@
 
         dataset_kwargs: Dict[str, Union[None, str, bool, int, Dict]] = {
             "path": path,
             "read_only": read_only,
             "token": token,
             "org_id": org_id,
             "verbose": verbose,
+            "lock_timeout": lock_timeout,
+            "lock_enabled": lock_enabled,
         }
 
         if access_method == "stream":
             dataset_kwargs.update(
                 {
                     "address": address,
                     "storage": cache_chain,
@@ -343,14 +349,16 @@
         overwrite: bool = False,
         public: bool = False,
         memory_cache_size: int = DEFAULT_MEMORY_CACHE_SIZE,
         local_cache_size: int = DEFAULT_LOCAL_CACHE_SIZE,
         creds: Optional[Union[Dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
+        lock_enabled: Optional[bool] = True,
+        lock_timeout: Optional[int] = 0,
         verbose: bool = True,
     ) -> Dataset:
         """Creates an empty dataset
 
         Args:
             path (str, pathlib.Path): - The full path to the dataset. It can be:
                 - a Deep Lake cloud path of the form ``hub://org_id/dataset_name``. Requires registration with Deep Lake.
@@ -365,15 +373,16 @@
             creds (dict, str, optional): The string ``ENV`` or a dictionary containing credentials used to access the dataset at the path.
                 - If 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token' are present, these take precedence over credentials present in the environment or in credentials file. Currently only works with s3 paths.
                 - It supports 'aws_access_key_id', 'aws_secret_access_key', 'aws_session_token', 'endpoint_url', 'aws_region', 'profile_name' as keys.
                 - If 'ENV' is passed, credentials are fetched from the environment variables. This is also the case when creds is not passed for cloud datasets. For datasets connected to hub cloud, specifying 'ENV' will override the credentials fetched from Activeloop and use local ones.
             token (str, optional): Activeloop token, used for fetching credentials to the dataset at path if it is a Deep Lake dataset. This is optional, tokens are normally autogenerated.
             org_id (str, Optional): Organization id to be used for enabling enterprise features. Only applicable for local datasets.
             verbose (bool): If True, logs will be printed. Defaults to True.
-
+            lock_timeout (int): Number of seconds to wait before throwing a LockException. If None, wait indefinitely
+            lock_enabled (bool): If true, the dataset manages a write lock. NOTE: Only set to False if you are managing concurrent access externally
         Returns:
             Dataset: Dataset created using the arguments provided.
 
         Raises:
             DatasetHandlerError: If a Dataset already exists at the given path and overwrite is False.
             UserNotLoggedInException: When user is not logged in
             InvalidTokenException: If the specified toke is invalid
@@ -429,14 +438,16 @@
             "path": path,
             "storage": cache_chain,
             "read_only": storage.read_only,
             "public": public,
             "token": token,
             "org_id": org_id,
             "verbose": verbose,
+            "lock_timeout": lock_timeout,
+            "lock_enabled": lock_enabled,
         }
         ret = dataset._load(dataset_kwargs, create=True)
         return ret
 
     @staticmethod
     @spinner
     def load(
@@ -447,14 +458,16 @@
         creds: Optional[Union[dict, str]] = None,
         token: Optional[str] = None,
         org_id: Optional[str] = None,
         verbose: bool = True,
         access_method: str = "stream",
         reset: bool = False,
         check_integrity: bool = True,
+        lock_timeout: Optional[int] = 0,
+        lock_enabled: Optional[bool] = True,
     ) -> Dataset:
         """Loads an existing dataset
 
         Examples:
 
             >>> ds = deeplake.load("hub://username/dataset")
             >>> ds = deeplake.load("s3://mybucket/my_dataset")
@@ -574,14 +587,16 @@
 
         dataset_kwargs: Dict[str, Union[None, str, bool, int, Dict]] = {
             "path": path,
             "read_only": read_only,
             "token": token,
             "org_id": org_id,
             "verbose": verbose,
+            "lock_timeout": lock_timeout,
+            "lock_enabled": lock_enabled,
         }
 
         if access_method == "stream":
             dataset_kwargs.update(
                 {
                     "address": address,
                     "storage": cache_chain,
```

### Comparing `deeplake-3.6.8/deeplake/api/info.py` & `deeplake-3.6.9/deeplake/api/info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/link.py` & `deeplake-3.6.9/deeplake/api/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/link_tiled.py` & `deeplake-3.6.9/deeplake/api/link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/read.py` & `deeplake-3.6.9/deeplake/api/read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_access_method.py` & `deeplake-3.6.9/deeplake/api/tests/test_access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_agreement.py` & `deeplake-3.6.9/deeplake/api/tests/test_agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_api.py` & `deeplake-3.6.9/deeplake/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_api_tiling.py` & `deeplake-3.6.9/deeplake/api/tests/test_api_tiling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_api_with_compression.py` & `deeplake-3.6.9/deeplake/api/tests/test_api_with_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_chunk_sizes.py` & `deeplake-3.6.9/deeplake/api/tests/test_chunk_sizes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_connect_datasets.py` & `deeplake-3.6.9/deeplake/api/tests/test_connect_datasets.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_dataset.py` & `deeplake-3.6.9/deeplake/api/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_dicom.py` & `deeplake-3.6.9/deeplake/api/tests/test_dicom.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_downsample.py` & `deeplake-3.6.9/deeplake/api/tests/test_downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_events.py` & `deeplake-3.6.9/deeplake/api/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_grayscale.py` & `deeplake-3.6.9/deeplake/api/tests/test_grayscale.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_info.py` & `deeplake-3.6.9/deeplake/api/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_insertion_out_of_order.py` & `deeplake-3.6.9/deeplake/api/tests/test_insertion_out_of_order.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_json.py` & `deeplake-3.6.9/deeplake/api/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_link.py` & `deeplake-3.6.9/deeplake/api/tests/test_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_link_tiled.py` & `deeplake-3.6.9/deeplake/api/tests/test_link_tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_linking.py` & `deeplake-3.6.9/deeplake/api/tests/test_linking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_mesh.py` & `deeplake-3.6.9/deeplake/api/tests/test_mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_meta.py` & `deeplake-3.6.9/deeplake/api/tests/test_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_nifti.py` & `deeplake-3.6.9/deeplake/api/tests/test_nifti.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_none.py` & `deeplake-3.6.9/deeplake/api/tests/test_none.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_partial_upload.py` & `deeplake-3.6.9/deeplake/api/tests/test_partial_upload.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_pickle.py` & `deeplake-3.6.9/deeplake/api/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_point_cloud.py` & `deeplake-3.6.9/deeplake/api/tests/test_point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_polygons.py` & `deeplake-3.6.9/deeplake/api/tests/test_polygons.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_pop.py` & `deeplake-3.6.9/deeplake/api/tests/test_pop.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_readonly.py` & `deeplake-3.6.9/deeplake/api/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_rechunk.py` & `deeplake-3.6.9/deeplake/api/tests/test_rechunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_reset.py` & `deeplake-3.6.9/deeplake/api/tests/test_reset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_sample_info.py` & `deeplake-3.6.9/deeplake/api/tests/test_sample_info.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_text.py` & `deeplake-3.6.9/deeplake/api/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_update_samples.py` & `deeplake-3.6.9/deeplake/api/tests/test_update_samples.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_video.py` & `deeplake-3.6.9/deeplake/api/tests/test_video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tests/test_views.py` & `deeplake-3.6.9/deeplake/api/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/api/tiled.py` & `deeplake-3.6.9/deeplake/api/tiled.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/structured/base.py` & `deeplake-3.6.9/deeplake/auto/structured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/structured/dataframe.py` & `deeplake-3.6.9/deeplake/auto/structured/dataframe.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/tests/test_coco_template.py` & `deeplake-3.6.9/deeplake/auto/tests/test_coco_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/tests/test_ingestion.py` & `deeplake-3.6.9/deeplake/auto/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/tests/test_kaggle.py` & `deeplake-3.6.9/deeplake/auto/tests/test_kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/tests/test_yolo_template.py` & `deeplake-3.6.9/deeplake/auto/tests/test_yolo_template.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/base.py` & `deeplake-3.6.9/deeplake/auto/unstructured/base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/coco/coco.py` & `deeplake-3.6.9/deeplake/auto/unstructured/coco/coco.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/coco/constants.py` & `deeplake-3.6.9/deeplake/auto/unstructured/coco/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/coco/convert.py` & `deeplake-3.6.9/deeplake/auto/unstructured/coco/convert.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/coco/utils.py` & `deeplake-3.6.9/deeplake/auto/unstructured/coco/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/image_classification.py` & `deeplake-3.6.9/deeplake/auto/unstructured/image_classification.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/kaggle.py` & `deeplake-3.6.9/deeplake/auto/unstructured/kaggle.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/util.py` & `deeplake-3.6.9/deeplake/auto/unstructured/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/yolo/utils.py` & `deeplake-3.6.9/deeplake/auto/unstructured/yolo/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/auto/unstructured/yolo/yolo.py` & `deeplake-3.6.9/deeplake/auto/unstructured/yolo/yolo.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/cli/auth.py` & `deeplake-3.6.9/deeplake/cli/auth.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/cli/test_cli.py` & `deeplake-3.6.9/deeplake/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/client/client.py` & `deeplake-3.6.9/deeplake/client/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -310,16 +310,14 @@
                 "repository": repository,
             },
             endpoint=self.endpoint(),
         )
 
         if response.status_code == 200:
             logger.info("Your Deep Lake dataset has been successfully created!")
-            if public is False:
-                logger.info("The dataset is private so make sure you are logged in!")
 
     def get_managed_creds(self, org_id, creds_key):
         """Retrieves the managed credentials for the given org_id and creds_key.
 
         Args:
             org_id (str): The name of the user/organization to which the dataset belongs.
             creds_key (str): The key corresponding to the managed credentials.
```

### Comparing `deeplake-3.6.8/deeplake/client/config.py` & `deeplake-3.6.9/deeplake/client/config.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/client/log.py` & `deeplake-3.6.9/deeplake/client/log.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/client/test_client.py` & `deeplake-3.6.9/deeplake/client/test_client.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/client/utils.py` & `deeplake-3.6.9/deeplake/client/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/compression.py` & `deeplake-3.6.9/deeplake/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/constants.py` & `deeplake-3.6.9/deeplake/constants.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/base_chunk.py` & `deeplake-3.6.9/deeplake/core/chunk/base_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/chunk_compressed_chunk.py` & `deeplake-3.6.9/deeplake/core/chunk/chunk_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/sample_compressed_chunk.py` & `deeplake-3.6.9/deeplake/core/chunk/sample_compressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/test_chunk_compressed.py` & `deeplake-3.6.9/deeplake/core/chunk/test_chunk_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/test_sample_compressed.py` & `deeplake-3.6.9/deeplake/core/chunk/test_sample_compressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/test_uncompressed.py` & `deeplake-3.6.9/deeplake/core/chunk/test_uncompressed.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk/uncompressed_chunk.py` & `deeplake-3.6.9/deeplake/core/chunk/uncompressed_chunk.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/chunk_engine.py` & `deeplake-3.6.9/deeplake/core/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/compression.py` & `deeplake-3.6.9/deeplake/core/compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/compute/process.py` & `deeplake-3.6.9/deeplake/core/compute/process.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/compute/provider.py` & `deeplake-3.6.9/deeplake/core/compute/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/compute/ray.py` & `deeplake-3.6.9/deeplake/core/compute/ray.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/compute/serial.py` & `deeplake-3.6.9/deeplake/core/compute/serial.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/compute/thread.py` & `deeplake-3.6.9/deeplake/core/compute/thread.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/dataset/__init__.py` & `deeplake-3.6.9/deeplake/core/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/dataset/dataset.py` & `deeplake-3.6.9/deeplake/core/dataset/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -160,15 +160,16 @@
         verbose: bool = True,
         version_state: Optional[Dict[str, Any]] = None,
         path: Optional[Union[str, pathlib.Path]] = None,
         address: Optional[str] = None,
         is_iteration: bool = False,
         link_creds=None,
         pad_tensors: bool = False,
-        lock: bool = True,
+        lock_enabled: bool = True,
+        lock_timeout: Optional[int] = 0,
         enabled_tensors: Optional[List[str]] = None,
         view_base: Optional["Dataset"] = None,
         libdeeplake_dataset=None,
         **kwargs,
     ):
         """Initializes a new or existing dataset.
 
@@ -185,15 +186,16 @@
             version_state (Dict[str, Any], Optional): The version state of the dataset, includes commit_id, commit_node, branch, branch_commit_map and commit_node_map.
             path (str, pathlib.Path): The path to the dataset.
             address (Optional[str]): The version address of the dataset.
             is_iteration (bool): If this Dataset is being used as an iterator.
             link_creds (LinkCreds, Optional): The LinkCreds object used to access tensors that have external data linked to them.
             pad_tensors (bool): If ``True``, shorter tensors will be padded to the length of the longest tensor.
             **kwargs: Passing subclass variables through without errors.
-            lock (bool): Whether the dataset should be locked for writing. Only applicable for S3, Deep Lake storage and GCS datasets. No effect if read_only=True.
+            lock_enabled (bool): Whether the dataset should be locked for writing. Only applicable for S3, Deep Lake storage and GCS datasets. No effect if read_only=True.
+            lock_timeout (int): How many seconds to wait for a lock before throwing an exception. If None, wait indefinitely
             enabled_tensors (List[str], Optional): List of tensors that are enabled in this view. By default all tensors are enabled.
             view_base (Optional["Dataset"]): Base dataset of this view.
             libdeeplake_dataset : The libdeeplake dataset object corresponding to this dataset.
 
         Raises:
             ValueError: If an existing local path is given, it must be a directory.
             ImproperDatasetInitialization: Exactly one argument out of 'path' and 'storage' needs to be specified.
@@ -233,15 +235,16 @@
         d["_view_base"] = view_base
         d["_view_use_parent_commit"] = False
         d["_update_hooks"] = {}
         d["_commit_hooks"] = {}
         d["_checkout_hooks"] = {}
         d["_parent_dataset"] = None
         d["_pad_tensors"] = pad_tensors
-        d["_locking_enabled"] = lock
+        d["_locking_enabled"] = lock_enabled
+        d["_lock_timeout"] = lock_timeout
         d["_temp_tensors"] = []
         d["_vc_info_updated"] = True
         dct = self.__dict__
         dct.update(d)
 
         try:
             self._set_derived_attributes(address=address)
@@ -1828,26 +1831,14 @@
     @property
     def has_head_changes(self):
         """Returns True if currently at head node and uncommitted changes are present."""
         return self.is_head_node and current_commit_has_change(
             self.version_state, self.storage
         )
 
-    def _acquire_lock(self, timeout: Optional[int] = None):
-        if timeout is not None:
-            start_time = time()
-        while True:
-            try:
-                self._set_read_only(False, True)
-                return
-            except LockedException:
-                if timeout is not None and time() - start_time > timeout:
-                    raise LockedException()
-                sleep(1)
-
     def _set_read_only(self, value: bool, err: bool):
         storage = self.storage
         self.__dict__["_read_only"] = value
 
         if value:
             storage.enable_readonly()
             if isinstance(storage, LRUCache) and storage.next_storage is not None:
```

### Comparing `deeplake-3.6.8/deeplake/core/dataset/deeplake_cloud_dataset.py` & `deeplake-3.6.9/deeplake/core/dataset/deeplake_cloud_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/dataset/deeplake_query_dataset.py` & `deeplake-3.6.9/deeplake/core/dataset/deeplake_query_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/dataset/deeplake_query_tensor.py` & `deeplake-3.6.9/deeplake/core/dataset/deeplake_query_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/dataset/invalid_view.py` & `deeplake-3.6.9/deeplake/core/dataset/invalid_view.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/dataset/view_entry.py` & `deeplake-3.6.9/deeplake/core/dataset/view_entry.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/fast_forwarding.py` & `deeplake-3.6.9/deeplake/core/fast_forwarding.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/index/index.py` & `deeplake-3.6.9/deeplake/core/index/index.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/io.py` & `deeplake-3.6.9/deeplake/core/io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/ipc.py` & `deeplake-3.6.9/deeplake/core/ipc.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/link_creds.py` & `deeplake-3.6.9/deeplake/core/link_creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/linked_chunk_engine.py` & `deeplake-3.6.9/deeplake/core/linked_chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/linked_sample.py` & `deeplake-3.6.9/deeplake/core/linked_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/linked_tiled_sample.py` & `deeplake-3.6.9/deeplake/core/linked_tiled_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/lock.py` & `deeplake-3.6.9/deeplake/core/lock.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
         if not byts:
             raise LockedException()
         nodeid, timestamp, tag = _parse_lock_bytes(byts)
         if tag != self.tag or nodeid != uuid.getnode():
             raise LockedException()
         self._write_lock()
 
-    def acquire(self, timeout: Optional[int] = None):
+    def acquire(self, timeout: Optional[int] = 0):
         storage = self.storage
         path = self.path
         if timeout is not None:
             start_time = time.time()
         while True:
             try:
                 byts = storage.get(path)
@@ -155,50 +155,52 @@
         lock = deeplake.core.lock.Lock(s3)  # Raises LockedException
 
         The lock is updated every 2 mins by an internal thread. The lock is valid for 5 mins after the last update.
 
     Args:
         storage (StorageProvider): The storage provder to be locked.
         lock_lost_callback (Callable, optional): Called if the lock is lost after acquiring.
-
+        timeout(int, optional): Keep trying to acquire the lock for the given number of seconds before throwing a LockedException. Passing None will wait forever
     Raises:
         LockedException: If the storage is already locked by a different machine.
     """
 
     def __init__(
         self,
         storage: StorageProvider,
         path: Optional[str] = None,
         lock_lost_callback: Optional[Callable] = None,
+        timeout: Optional[int] = 0,
     ):
         self.storage = storage
         self.path = get_dataset_lock_key() if path is None else path
         self.lock_lost_callback = lock_lost_callback
         self.acquired = False
         self._thread_lock = threading.Lock()
         self._previous_update_timestamp = None
         self.lock = Lock(storage, self.path, deeplake.constants.DATASET_LOCK_VALIDITY)
         self.acquired = False
+        self.timeout = timeout
         self.acquire()
         atexit.register(self.release)
 
     def acquire(self):
         if self.acquired:
             return
-        self.lock.acquire(timeout=0)
+        self.lock.acquire(timeout=self.timeout)
         self._thread = threading.Thread(target=self._lock_loop, daemon=True)
         self._thread.start()
         self.acquired = True
 
     def _lock_loop(self):
         try:
             while True:
                 time.sleep(deeplake.constants.DATASET_LOCK_UPDATE_INTERVAL)
                 try:
-                    self.lock.refresh_lock(timeout=0)
+                    self.lock.refresh_lock(timeout=self.timeout)
                 except LockedException:
                     if self.lock_lost_callback:
                         self.lock_lost_callback()
                     return
         except Exception:  # Thread termination
             return
 
@@ -242,20 +244,21 @@
         LockedException: If the storage is already locked by a different machine.
     """
     storage = get_base_storage(dataset.storage)
     version = dataset.version_state["commit_id"]
     key = _get_lock_key(get_path_from_storage(storage), version)
     lock = _LOCKS.get(key)
     if lock:
-        lock.acquire()
+        lock.acquire(dataset._lock_timeout)
     else:
         lock = PersistentLock(
             storage,
             path=_get_lock_file_path(version),
             lock_lost_callback=lock_lost_callback,
+            timeout=dataset._lock_timeout,
         )
         _LOCKS[key] = lock
     _REFS[key].add(id(dataset))
 
 
 def unlock_dataset(dataset):
     """Unlocks a storage provider that was locked by this machine.
```

### Comparing `deeplake-3.6.8/deeplake/core/meta/dataset_meta.py` & `deeplake-3.6.9/deeplake/core/meta/dataset_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/base_encoder.py` & `deeplake-3.6.9/deeplake/core/meta/encode/base_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/byte_positions.py` & `deeplake-3.6.9/deeplake/core/meta/encode/byte_positions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/chunk_id.py` & `deeplake-3.6.9/deeplake/core/meta/encode/chunk_id.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/creds.py` & `deeplake-3.6.9/deeplake/core/meta/encode/creds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/pad.py` & `deeplake-3.6.9/deeplake/core/meta/encode/pad.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/sequence.py` & `deeplake-3.6.9/deeplake/core/meta/encode/sequence.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/shape.py` & `deeplake-3.6.9/deeplake/core/meta/encode/shape.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py` & `deeplake-3.6.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py` & `deeplake-3.6.9/deeplake/core/meta/encode/tests/test_byte_positions_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py` & `deeplake-3.6.9/deeplake/core/meta/encode/tests/test_chunk_id_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder.py` & `deeplake-3.6.9/deeplake/core/meta/encode/tests/test_shape_encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py` & `deeplake-3.6.9/deeplake/core/meta/encode/tests/test_shape_encoder_updates.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/encode/tile.py` & `deeplake-3.6.9/deeplake/core/meta/encode/tile.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/meta/tensor_meta.py` & `deeplake-3.6.9/deeplake/core/meta/tensor_meta.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/partial_reader.py` & `deeplake-3.6.9/deeplake/core/partial_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/partial_sample.py` & `deeplake-3.6.9/deeplake/core/partial_sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/polygon.py` & `deeplake-3.6.9/deeplake/core/polygon.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/query/autocomplete.py` & `deeplake-3.6.9/deeplake/core/query/autocomplete.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/query/filter.py` & `deeplake-3.6.9/deeplake/core/query/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/query/query.py` & `deeplake-3.6.9/deeplake/core/query/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/sample.py` & `deeplake-3.6.9/deeplake/core/sample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/serialize.py` & `deeplake-3.6.9/deeplake/core/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/azure.py` & `deeplake-3.6.9/deeplake/core/storage/azure.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/deeplake_memory_object.py` & `deeplake-3.6.9/deeplake/core/storage/deeplake_memory_object.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/gcs.py` & `deeplake-3.6.9/deeplake/core/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/google_drive.py` & `deeplake-3.6.9/deeplake/core/storage/google_drive.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/local.py` & `deeplake-3.6.9/deeplake/core/storage/local.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/lru_cache.py` & `deeplake-3.6.9/deeplake/core/storage/lru_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/memory.py` & `deeplake-3.6.9/deeplake/core/storage/memory.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/provider.py` & `deeplake-3.6.9/deeplake/core/storage/provider.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/storage/s3.py` & `deeplake-3.6.9/deeplake/core/storage/s3.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tensor.py` & `deeplake-3.6.9/deeplake/core/tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tensor_link.py` & `deeplake-3.6.9/deeplake/core/tensor_link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/test_serialize.py` & `deeplake-3.6.9/deeplake/core/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_compression.py` & `deeplake-3.6.9/deeplake/core/tests/test_compression.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_compute.py` & `deeplake-3.6.9/deeplake/core/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_deeplake_indra_dataset.py` & `deeplake-3.6.9/deeplake/core/tests/test_deeplake_indra_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_io.py` & `deeplake-3.6.9/deeplake/core/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_locking.py` & `deeplake-3.6.9/deeplake/core/tests/test_locking.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_readonly.py` & `deeplake-3.6.9/deeplake/core/tests/test_readonly.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tests/test_serialize.py` & `deeplake-3.6.9/deeplake/core/tests/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tiling/deserialize.py` & `deeplake-3.6.9/deeplake/core/tiling/deserialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tiling/optimizer.py` & `deeplake-3.6.9/deeplake/core/tiling/optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tiling/sample_tiles.py` & `deeplake-3.6.9/deeplake/core/tiling/sample_tiles.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tiling/serialize.py` & `deeplake-3.6.9/deeplake/core/tiling/serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tiling/test_optimizer.py` & `deeplake-3.6.9/deeplake/core/tiling/test_optimizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/tiling/test_serialize.py` & `deeplake-3.6.9/deeplake/core/tiling/test_serialize.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/transform/test_transform.py` & `deeplake-3.6.9/deeplake/core/transform/test_transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/transform/transform.py` & `deeplake-3.6.9/deeplake/core/transform/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/transform/transform_dataset.py` & `deeplake-3.6.9/deeplake/core/transform/transform_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/transform/transform_tensor.py` & `deeplake-3.6.9/deeplake/core/transform/transform_tensor.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/__init__.py` & `deeplake-3.6.9/deeplake/core/vectorstore/__init__.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/deeplake_vectorstore.py` & `deeplake-3.6.9/deeplake/core/vectorstore/deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,25 @@
                 "embedding_tensor": embedding_tensor,
                 "embedding": True if embedding is not None else False,
                 "return_tensors": return_tensors,
                 "return_view": return_view,
             },
         )
 
+        if (
+            exec_option is None
+            and self.exec_option is not "python"
+            and isinstance(filter, Callable)
+        ):
+            logger.warning(
+                'Switching exec_option to "python" (runs on client) because filter is specified as a function. '
+                f'To continue using the original exec_option "{self.exec_option}", please specify the filter as a dictionary or use the "query" parameter to specify a TQL query.'
+            )
+            exec_option = "python"
+
         exec_option = exec_option or self.exec_option
 
         utils.parse_search_args(
             embedding_data=embedding_data,
             embedding_function=embedding_function,
             initial_embedding_function=self.embedding_function,
             embedding=embedding,
```

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/test_deeplake_vectorstore.py` & `deeplake-3.6.9/deeplake/core/vectorstore/test_deeplake_vectorstore.py`

 * *Files 1% similar despite different names*

```diff
@@ -277,18 +277,26 @@
     data_ce_v = vector_store_cloud.search(
         embedding=query_embedding, k=2, return_view=True
     )
     assert len(data_ce_v) == 2
     assert isinstance(data_ce_v.text[0].data()["value"], str)
     assert data_ce_v.embedding[0].numpy().size > 0
 
+    # Check that filter_fn with cloud dataset (and therefore "compute_engine" exec option) switches to "python" automatically.
+    with pytest.warns(None):
+        _ = vector_store_cloud.search(
+            filter=filter_fn,
+        )
+
     # Check exceptions
     # Invalid exec option
     with pytest.raises(ValueError):
-        vector_store.search(embedding=query_embedding, exec_option="remote_tensor_db")
+        vector_store.search(
+            embedding=query_embedding, exec_option="invalid_exec_option"
+        )
     # Search without parameters
     with pytest.raises(ValueError):
         vector_store.search()
     # Query with python exec_option
     with pytest.raises(ValueError):
         vector_store.search(query="dummy", exec_option="python")
     # Returning a tensor that does not exist
```

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/dataset.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/filter.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/filter/filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/filter/test_filter.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/filter/test_filter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/query.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/test_indra.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/test_indra.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/tql_distance_metrics/distance_metric.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/indra/vector_search.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/indra/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/ingest_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/ingestion/test_data_ingestion.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/search_algorithm.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/search_algorithm.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/test_vector_search.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/test_vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/python/vector_search.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/python/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/utils.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/vectorstore/vector_search/vector_search.py` & `deeplake-3.6.9/deeplake/core/vectorstore/vector_search/vector_search.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/version_control/commit_chunk_map.py` & `deeplake-3.6.9/deeplake/core/version_control/commit_chunk_map.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/version_control/commit_diff.py` & `deeplake-3.6.9/deeplake/core/version_control/commit_diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/version_control/commit_node.py` & `deeplake-3.6.9/deeplake/core/version_control/commit_node.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/version_control/dataset_diff.py` & `deeplake-3.6.9/deeplake/core/version_control/dataset_diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,18 +32,21 @@
                 self.info_updated.to_bytes(1, "big"),
                 len(self.renamed).to_bytes(8, "big"),
                 *(
                     b"".join(
                         [
                             len(old_name).to_bytes(8, "big"),
                             len(new_name).to_bytes(8, "big"),
-                            (old_name + new_name).encode("utf-8"),
+                            (old_name + new_name),
                         ]
                     )
-                    for old_name, new_name in self.renamed.items()
+                    for old_name, new_name in map(
+                        lambda n: (n[0].encode("utf-8"), n[1].encode("utf-8")),
+                        self.renamed.items(),
+                    )
                 ),
                 len(self.deleted).to_bytes(8, "big"),
                 *(
                     b"".join([len(name).to_bytes(8, "big"), name.encode("utf-8")])
                     for name in self.deleted
                 ),
             ]
```

### Comparing `deeplake-3.6.8/deeplake/core/version_control/test_merge.py` & `deeplake-3.6.9/deeplake/core/version_control/test_merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/core/version_control/test_version_control.py` & `deeplake-3.6.9/deeplake/core/version_control/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/convert_to_libdeeplake.py` & `deeplake-3.6.9/deeplake/enterprise/convert_to_libdeeplake.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/dataloader.py` & `deeplake-3.6.9/deeplake/enterprise/dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/dummy_dataloader.py` & `deeplake-3.6.9/deeplake/enterprise/dummy_dataloader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/libdeeplake_query.py` & `deeplake-3.6.9/deeplake/enterprise/libdeeplake_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/test_pytorch.py` & `deeplake-3.6.9/deeplake/enterprise/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/test_query.py` & `deeplake-3.6.9/deeplake/enterprise/test_query.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/test_tensorflow.py` & `deeplake-3.6.9/deeplake/enterprise/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/enterprise/util.py` & `deeplake-3.6.9/deeplake/enterprise/util.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/hooks.py` & `deeplake-3.6.9/deeplake/hooks.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/htype.py` & `deeplake-3.6.9/deeplake/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/huggingface/huggingface.py` & `deeplake-3.6.9/deeplake/integrations/huggingface/huggingface.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_.py` & `deeplake-3.6.9/deeplake/integrations/mmdet/mmdet_.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_runners.py` & `deeplake-3.6.9/deeplake/integrations/mmdet/mmdet_runners.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/mmdet/mmdet_utils.py` & `deeplake-3.6.9/deeplake/integrations/mmdet/mmdet_utils.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/pytorch/common.py` & `deeplake-3.6.9/deeplake/integrations/pytorch/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/pytorch/dataset.py` & `deeplake-3.6.9/deeplake/integrations/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/pytorch/pytorch.py` & `deeplake-3.6.9/deeplake/integrations/pytorch/pytorch.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/pytorch/shuffle_buffer.py` & `deeplake-3.6.9/deeplake/integrations/pytorch/shuffle_buffer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/tf/common.py` & `deeplake-3.6.9/deeplake/integrations/tf/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/tf/datasettotensorflow.py` & `deeplake-3.6.9/deeplake/integrations/tf/datasettotensorflow.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/tf/deeplake_tensorflow_dataset.py` & `deeplake-3.6.9/deeplake/integrations/tf/deeplake_tensorflow_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/integrations/wandb/wandb.py` & `deeplake-3.6.9/deeplake/integrations/wandb/wandb.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/tests/cache_fixtures.py` & `deeplake-3.6.9/deeplake/tests/cache_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/tests/client_fixtures.py` & `deeplake-3.6.9/deeplake/tests/client_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/tests/common.py` & `deeplake-3.6.9/deeplake/tests/common.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/tests/dataset_fixtures.py` & `deeplake-3.6.9/deeplake/tests/dataset_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/tests/path_fixtures.py` & `deeplake-3.6.9/deeplake/tests/path_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/tests/storage_fixtures.py` & `deeplake-3.6.9/deeplake/tests/storage_fixtures.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/access_method.py` & `deeplake-3.6.9/deeplake/util/access_method.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/agreement.py` & `deeplake-3.6.9/deeplake/util/agreement.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/array_list.py` & `deeplake-3.6.9/deeplake/util/array_list.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/assert_byte_indexes.py` & `deeplake-3.6.9/deeplake/util/assert_byte_indexes.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/auto.py` & `deeplake-3.6.9/deeplake/util/auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/bugout_reporter.py` & `deeplake-3.6.9/deeplake/util/bugout_reporter.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/cache_chain.py` & `deeplake-3.6.9/deeplake/util/cache_chain.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/casting.py` & `deeplake-3.6.9/deeplake/util/casting.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/check_latest_version.py` & `deeplake-3.6.9/deeplake/util/check_latest_version.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/chunk_engine.py` & `deeplake-3.6.9/deeplake/util/chunk_engine.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/class_label.py` & `deeplake-3.6.9/deeplake/util/class_label.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/compute.py` & `deeplake-3.6.9/deeplake/util/compute.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/connect_dataset.py` & `deeplake-3.6.9/deeplake/util/connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/dataset.py` & `deeplake-3.6.9/deeplake/util/dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/diff.py` & `deeplake-3.6.9/deeplake/util/diff.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/downsample.py` & `deeplake-3.6.9/deeplake/util/downsample.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/encoder.py` & `deeplake-3.6.9/deeplake/util/encoder.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/exceptions.py` & `deeplake-3.6.9/deeplake/util/exceptions.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/exif.py` & `deeplake-3.6.9/deeplake/util/exif.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/from_tfds.py` & `deeplake-3.6.9/deeplake/util/from_tfds.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/htype.py` & `deeplake-3.6.9/deeplake/util/htype.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/image.py` & `deeplake-3.6.9/deeplake/util/image.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/invalid_view_op.py` & `deeplake-3.6.9/deeplake/util/invalid_view_op.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/iteration_warning.py` & `deeplake-3.6.9/deeplake/util/iteration_warning.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/json.py` & `deeplake-3.6.9/deeplake/util/json.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/keys.py` & `deeplake-3.6.9/deeplake/util/keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/link.py` & `deeplake-3.6.9/deeplake/util/link.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/logging.py` & `deeplake-3.6.9/deeplake/util/logging.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/merge.py` & `deeplake-3.6.9/deeplake/util/merge.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/modified.py` & `deeplake-3.6.9/deeplake/util/modified.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/notebook.py` & `deeplake-3.6.9/deeplake/util/notebook.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/mesh.py` & `deeplake-3.6.9/deeplake/util/object_3d/mesh.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/object_base_3d.py` & `deeplake-3.6.9/deeplake/util/object_3d/object_base_3d.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/ply_parser.py` & `deeplake-3.6.9/deeplake/util/object_3d/ply_parser.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/ply_parser_base.py` & `deeplake-3.6.9/deeplake/util/object_3d/ply_parser_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/ply_parsers.py` & `deeplake-3.6.9/deeplake/util/object_3d/ply_parsers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/ply_reader.py` & `deeplake-3.6.9/deeplake/util/object_3d/ply_reader.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/ply_reader_base.py` & `deeplake-3.6.9/deeplake/util/object_3d/ply_reader_base.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/ply_readers.py` & `deeplake-3.6.9/deeplake/util/object_3d/ply_readers.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/point_cloud.py` & `deeplake-3.6.9/deeplake/util/object_3d/point_cloud.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/object_3d/read_3d_data.py` & `deeplake-3.6.9/deeplake/util/object_3d/read_3d_data.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/path.py` & `deeplake-3.6.9/deeplake/util/path.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/pretty_print.py` & `deeplake-3.6.9/deeplake/util/pretty_print.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/remove_cache.py` & `deeplake-3.6.9/deeplake/util/remove_cache.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/scheduling.py` & `deeplake-3.6.9/deeplake/util/scheduling.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/shape_interval.py` & `deeplake-3.6.9/deeplake/util/shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/spinner.py` & `deeplake-3.6.9/deeplake/util/spinner.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/split.py` & `deeplake-3.6.9/deeplake/util/split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/storage.py` & `deeplake-3.6.9/deeplake/util/storage.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tag.py` & `deeplake-3.6.9/deeplake/util/tag.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tensor_db.py` & `deeplake-3.6.9/deeplake/util/tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/testing.py` & `deeplake-3.6.9/deeplake/util/testing.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_auto.py` & `deeplake-3.6.9/deeplake/util/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_connect_dataset.py` & `deeplake-3.6.9/deeplake/util/tests/test_connect_dataset.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_iterable_ordered_dict.py` & `deeplake-3.6.9/deeplake/util/tests/test_iterable_ordered_dict.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_keys.py` & `deeplake-3.6.9/deeplake/util/tests/test_keys.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_read.py` & `deeplake-3.6.9/deeplake/util/tests/test_read.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_shape_interval.py` & `deeplake-3.6.9/deeplake/util/tests/test_shape_interval.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_split.py` & `deeplake-3.6.9/deeplake/util/tests/test_split.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_tensor_db.py` & `deeplake-3.6.9/deeplake/util/tests/test_tensor_db.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/tests/test_version_control.py` & `deeplake-3.6.9/deeplake/util/tests/test_version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/transform.py` & `deeplake-3.6.9/deeplake/util/transform.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/version_control.py` & `deeplake-3.6.9/deeplake/util/version_control.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/util/video.py` & `deeplake-3.6.9/deeplake/util/video.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/visualizer/video_streaming.py` & `deeplake-3.6.9/deeplake/visualizer/video_streaming.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake/visualizer/visualizer.py` & `deeplake-3.6.9/deeplake/visualizer/visualizer.py`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake.egg-info/PKG-INFO` & `deeplake-3.6.9/deeplake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deeplake
-Version: 3.6.8
+Version: 3.6.9
 Summary: Activeloop Deep Lake
 Home-page: UNKNOWN
 Author: activeloop.ai
 Author-email: support@activeloop.ai
 License: MPL-2.0
 Project-URL: Documentation, https://docs.activeloop.ai/
 Project-URL: Source, https://github.com/activeloopai/deeplake
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deeplake Version: 3.6.8 Summary: Activeloop Deep
+Metadata-Version: 2.1 Name: deeplake Version: 3.6.9 Summary: Activeloop Deep
 Lake Home-page: UNKNOWN Author: activeloop.ai Author-email:
 support@activeloop.ai License: MPL-2.0 Project-URL: Documentation, https://
 docs.activeloop.ai/ Project-URL: Source, https://github.com/activeloopai/
 deeplake Platform: UNKNOWN Classifier: License :: OSI Approved :: Mozilla
 Public License 2.0 (MPL 2.0) Description-Content-Type: text/markdown Provides-
 Extra: all Provides-Extra: audio Provides-Extra: av Provides-Extra: azure
 Provides-Extra: dicom Provides-Extra: enterprise Provides-Extra: gcp Provides-
```

### Comparing `deeplake-3.6.8/deeplake.egg-info/SOURCES.txt` & `deeplake-3.6.9/deeplake.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/deeplake.egg-info/requires.txt` & `deeplake-3.6.9/deeplake.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `deeplake-3.6.8/setup.py` & `deeplake-3.6.9/setup.py`

 * *Files identical despite different names*

