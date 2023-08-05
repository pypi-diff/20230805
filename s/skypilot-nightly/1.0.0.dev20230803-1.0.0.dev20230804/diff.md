# Comparing `tmp/skypilot-nightly-1.0.0.dev20230803.tar.gz` & `tmp/skypilot-nightly-1.0.0.dev20230804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skypilot-nightly-1.0.0.dev20230803.tar", last modified: Thu Aug  3 10:40:48 2023, max compression
+gzip compressed data, was "skypilot-nightly-1.0.0.dev20230804.tar", last modified: Fri Aug  4 10:40:26 2023, max compression
```

## Comparing `skypilot-nightly-1.0.0.dev20230803.tar` & `skypilot-nightly-1.0.0.dev20230804.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.280140 skypilot-nightly-1.0.0.dev20230803/
--rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-03 10:40:48.280140 skypilot-nightly-1.0.0.dev20230803/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 10:40:48.280140 skypilot-nightly-1.0.0.dev20230803/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-03 10:40:36.000000 skypilot-nightly-1.0.0.dev20230803/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.240140 skypilot-nightly-1.0.0.dev20230803/sky/
--rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-03 10:40:36.000000 skypilot-nightly-1.0.0.dev20230803/sky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.240140 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/cloudflare.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/adaptors/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/authentication.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.244140 skypilot-nightly-1.0.0.dev20230803/sky/backends/
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)   116682 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/backend_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   207126 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/cloud_vm_ray_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/docker_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/local_docker_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.244140 skypilot-nightly-1.0.0.dev20230803/sky/backends/monkey_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/monkey_patches/monkey_patch_ray_up.py
--rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/onprem_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/backends/wheel_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.244140 skypilot-nightly-1.0.0.dev20230803/sky/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/benchmark/benchmark_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/benchmark/benchmark_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/check.py
--rw-r--r--   0 runner    (1001) docker     (123)   173874 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/cloud_stores.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.248140 skypilot-nightly-1.0.0.dev20230803/sky/clouds/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    46013 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/ibm.py
--rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/kubernetes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/local.py
--rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/oci.py
--rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/scp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.248140 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/
--rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/aws_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/azure_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.252140 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
--rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/gcp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/ibm_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/lambda_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/oci_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/scp_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/dag.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.252140 skypilot-nightly-1.0.0.dev20230803/sky/data/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/data/data_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/data/data_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/data/mounting_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)   110767 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/data/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/data/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/execution.py
--rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.252140 skypilot-nightly-1.0.0.dev20230803/sky/provision/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/provision/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.252140 skypilot-nightly-1.0.0.dev20230803/sky/provision/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/provision/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/provision/aws/instance.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.252140 skypilot-nightly-1.0.0.dev20230803/sky/provision/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/provision/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/provision/gcp/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/provision/gcp/instance_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    46508 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.252140 skypilot-nightly-1.0.0.dev20230803/sky/setup_files/
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/setup_files/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-03 10:40:36.000000 skypilot-nightly-1.0.0.dev20230803/sky/setup_files/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/sky_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.256140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/
--rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/attempt_skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/autostop_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/events.py
--rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/job_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/log_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.232139 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.256140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.256140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)    53219 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.260140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/azure-config-template.json
--rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/azure-vm-template.json
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.260140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/node.py
--rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.260140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/vpc_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.260140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.260140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/lambda_cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/lambda_cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/lambda_cloud/lambda_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/lambda_cloud/node_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.264140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/query_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.264140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/node_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/scp_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.264140 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/autoscaler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/cli.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/command_runner.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/job_head.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/log_monitor.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/updater.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/worker.py.patch
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/skylet.py
--rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skylet/subprocess_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/skypilot_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.268140 skypilot-nightly-1.0.0.dev20230803/sky/spot/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    26791 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.268140 skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/dashboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.268140 skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.268140 skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    21311 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/recovery_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/spot_state.py
--rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/spot/spot_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/status_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)    39296 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.272140 skypilot-nightly-1.0.0.dev20230803/sky/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/aws-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/azure-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/gcp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/gcp-tpu-create.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/gcp-tpu-delete.sh.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/ibm-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/kubernetes-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/lambda-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/local-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/oci-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/scp-ray.yml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/templates/spot-controller.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.272140 skypilot-nightly-1.0.0.dev20230803/sky/usage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/usage/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/usage/usage_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.276140 skypilot-nightly-1.0.0.dev20230803/sky/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/accelerator_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.276140 skypilot-nightly-1.0.0.dev20230803/sky/utils/cli_utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/cli_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/cli_utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/command_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/dag_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/env_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.276140 skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/create_cluster.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/delete_cluster.sh
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/generate_kind_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/schemas.py
--rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/subprocess_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/timeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/tpu_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/ux_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/sky/utils/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.276140 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-03 10:40:48.000000 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-08-03 10:40:48.000000 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 10:40:48.000000 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-03 10:40:48.000000 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-03 10:40:48.000000 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-03 10:40:48.000000 skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 10:40:48.280140 skypilot-nightly-1.0.0.dev20230803/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_global_user_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_list_accelerators.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_onprem.py
--rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_optimizer_dryruns.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_optimizer_random_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_pycryptodome_version.py
--rw-r--r--   0 runner    (1001) docker     (123)   145911 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_smoke.py
--rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_spot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-03 10:40:27.000000 skypilot-nightly-1.0.0.dev20230803/tests/test_wheels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.210019 skypilot-nightly-1.0.0.dev20230804/
+-rw-r--r--   0 runner    (1001) docker     (123)    12170 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8781 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 10:40:26.210019 skypilot-nightly-1.0.0.dev20230804/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 10:40:18.000000 skypilot-nightly-1.0.0.dev20230804/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.182019 skypilot-nightly-1.0.0.dev20230804/sky/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-08-04 10:40:18.000000 skypilot-nightly-1.0.0.dev20230804/sky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.182019 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/cloudflare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2193 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3964 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/adaptors/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16982 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/authentication.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116682 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/backend_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   207600 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/cloud_vm_ray_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8321 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/docker_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16448 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/local_docker_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/backends/monkey_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/monkey_patches/monkey_patch_ray_up.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24438 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/onprem_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5903 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/backends/wheel_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8723 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24638 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)   173874 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11758 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/cloud_stores.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.186019 skypilot-nightly-1.0.0.dev20230804/sky/clouds/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39211 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25872 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26964 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46013 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20574 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16936 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/kubernetes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12103 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7989 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24397 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/oci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/scp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)    12366 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11756 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/aws_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7050 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/azure_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23189 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20092 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8679 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18557 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4198 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21163 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/gcp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/ibm_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5414 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/lambda_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7582 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/oci_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/scp_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40110 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/dag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7384 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/data_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21399 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/data_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/mounting_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110767 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6807 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/data/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41456 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/execution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26274 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43765 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/provision/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/instance.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6361 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9598 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46508 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.190019 skypilot-nightly-1.0.0.dev20230804/sky/setup_files/
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/setup_files/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-08-04 10:40:18.000000 skypilot-nightly-1.0.0.dev20230804/sky/setup_files/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/sky_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/
+-rw-r--r--   0 runner    (1001) docker     (123)    12568 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/attempt_skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4378 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/autostop_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32722 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/job_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19585 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/log_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.178019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32698 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53219 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29406 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4344 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-config-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10633 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-vm-template.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17469 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37472 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14292 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.194019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38280 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34628 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/vpc_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11154 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13611 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/lambda_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13650 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/node_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4234 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20136 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17048 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/query_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4683 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22219 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/node_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15481 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/scp_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.198019 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/autoscaler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/cli.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/command_runner.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/job_head.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/log_monitor.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      658 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/resource_demand_scheduler.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/updater.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/worker.py.patch
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/skylet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2649 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skylet/subprocess_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5654 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/skypilot_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26791 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/dashboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    24920 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/recovery_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22484 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34333 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/status_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39567 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10985 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/aws-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/azure-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    11988 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-tpu-create.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-tpu-delete.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/ibm-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    15341 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/kubernetes-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/lambda-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/local-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/oci-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/scp-ray.yml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/templates/spot-controller.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.202019 skypilot-nightly-1.0.0.dev20230804/sky/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/usage/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17294 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/usage/usage_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/sky/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2806 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/accelerator_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15219 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15075 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/command_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12344 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/dag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2777 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      852 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/env_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1788 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/create_cluster.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      927 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/delete_cluster.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/generate_kind_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5774 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/subprocess_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/timeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/tpu_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/ux_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/sky/utils/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9591 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-08-04 10:40:26.000000 skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 10:40:26.206019 skypilot-nightly-1.0.0.dev20230804/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4730 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5061 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_global_user_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5943 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3620 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_list_accelerators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_onprem.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22937 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_dryruns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_random_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_pycryptodome_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)   145911 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7215 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_spot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4048 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-08-04 10:40:13.000000 skypilot-nightly-1.0.0.dev20230804/tests/test_wheels.py
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/LICENSE` & `skypilot-nightly-1.0.0.dev20230804/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230804/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230804/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230803
+Version: 1.0.0.dev20230804
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230803
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230804
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/README.md` & `skypilot-nightly-1.0.0.dev20230804/README.md`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/pyproject.toml` & `skypilot-nightly-1.0.0.dev20230804/pyproject.toml`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/setup.py` & `skypilot-nightly-1.0.0.dev20230804/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/__init__.py` & `skypilot-nightly-1.0.0.dev20230804/sky/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """The SkyPilot package."""
 import os
 
 # Replaced with the current commit when building the wheels.
-__commit__ = '6f52a0bf21a2f538fe8cc71d43d823f82d2b4bc4'
-__version__ = '1.0.0-dev20230803'
+__commit__ = 'ca2a092a1cc26d26fb49f94a11cfe5f369df0f25'
+__version__ = '1.0.0-dev20230804'
 __root_dir__ = os.path.dirname(os.path.abspath(__file__))
 
 # Keep this order to avoid cyclic imports
 from sky import backends
 from sky import benchmark
 from sky import clouds
 from sky.clouds.service_catalog import list_accelerators
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/aws.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/azure.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/cloudflare.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/cloudflare.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/docker.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/docker.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/gcp.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/ibm.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/kubernetes.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/adaptors/oci.py` & `skypilot-nightly-1.0.0.dev20230804/sky/adaptors/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/authentication.py` & `skypilot-nightly-1.0.0.dev20230804/sky/authentication.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/backend.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/backend_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/backend_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/cloud_vm_ray_backend.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/cloud_vm_ray_backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -625,19 +625,27 @@
 
     class GangSchedulingStatus(enum.Enum):
         """Enum for gang scheduling status."""
         CLUSTER_READY = 0
         GANG_FAILED = 1
         HEAD_FAILED = 2
 
-    def __init__(self, log_dir: str, dag: 'dag.Dag',
+    def __init__(self,
+                 log_dir: str,
+                 dag: 'dag.Dag',
                  optimize_target: 'optimizer.OptimizeTarget',
                  requested_features: Set[clouds.CloudImplementationFeatures],
-                 local_wheel_path: pathlib.Path, wheel_hash: str):
+                 local_wheel_path: pathlib.Path,
+                 wheel_hash: str,
+                 blocked_resources: Optional[Iterable[
+                     resources_lib.Resources]] = None):
         self._blocked_resources: Set[resources_lib.Resources] = set()
+        if blocked_resources:
+            # blocked_resources is not None and not empty.
+            self._blocked_resources.update(blocked_resources)
 
         self.log_dir = os.path.expanduser(log_dir)
         self._dag = dag
         self._optimize_target = optimize_target
         self._requested_features = requested_features
         self._local_wheel_path = local_wheel_path
         self._wheel_hash = wheel_hash
@@ -2561,16 +2569,21 @@
 
                 # After this "round" of optimization across clouds, provisioning
                 # may still have not succeeded. This while loop will then kick
                 # in if retry_until_up is set, which will kick off new "rounds"
                 # of optimization infinitely.
                 try:
                     provisioner = RetryingVmProvisioner(
-                        self.log_dir, self._dag, self._optimize_target,
-                        self._requested_features, local_wheel_path, wheel_hash)
+                        self.log_dir,
+                        self._dag,
+                        self._optimize_target,
+                        self._requested_features,
+                        local_wheel_path,
+                        wheel_hash,
+                        blocked_resources=task.blocked_resources)
                     config_dict = provisioner.provision_with_retries(
                         task, to_provision_config, dryrun, stream_logs)
                     break
                 except exceptions.ResourcesUnavailableError as e:
                     # Do not remove the stopped cluster from the global state
                     # if failed to start.
                     if e.no_failover:
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/docker_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/docker_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/local_docker_backend.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/local_docker_backend.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/monkey_patches/monkey_patch_ray_up.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/monkey_patches/monkey_patch_ray_up.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/onprem_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/onprem_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/backends/wheel_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/backends/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/benchmark/benchmark_state.py` & `skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/benchmark/benchmark_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/benchmark/benchmark_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/check.py` & `skypilot-nightly-1.0.0.dev20230804/sky/check.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/cli.py` & `skypilot-nightly-1.0.0.dev20230804/sky/cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/cloud_stores.py` & `skypilot-nightly-1.0.0.dev20230804/sky/cloud_stores.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/__init__.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/aws.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/azure.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/cloud.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/gcp.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/ibm.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/ibm.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/kubernetes.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/kubernetes.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/local.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/local.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/oci.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/oci.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/scp.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/scp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/__init__.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/aws_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/aws_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/azure_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/azure_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/common.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/common.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_aws.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_aws.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_azure.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_azure.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_gcp.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/data_fetchers/fetch_lambda_cloud.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/gcp_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/gcp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/ibm_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/ibm_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/lambda_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/lambda_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/oci_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/oci_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/clouds/service_catalog/scp_catalog.py` & `skypilot-nightly-1.0.0.dev20230804/sky/clouds/service_catalog/scp_catalog.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/core.py` & `skypilot-nightly-1.0.0.dev20230804/sky/core.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/dag.py` & `skypilot-nightly-1.0.0.dev20230804/sky/dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/data/data_transfer.py` & `skypilot-nightly-1.0.0.dev20230804/sky/data/data_transfer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/data/data_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/data/data_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/data/mounting_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/data/mounting_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/data/storage.py` & `skypilot-nightly-1.0.0.dev20230804/sky/data/storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/data/storage_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/data/storage_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/exceptions.py` & `skypilot-nightly-1.0.0.dev20230804/sky/exceptions.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/execution.py` & `skypilot-nightly-1.0.0.dev20230804/sky/execution.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/global_user_state.py` & `skypilot-nightly-1.0.0.dev20230804/sky/global_user_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/optimizer.py` & `skypilot-nightly-1.0.0.dev20230804/sky/optimizer.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/provision/__init__.py` & `skypilot-nightly-1.0.0.dev20230804/sky/provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/provision/aws/instance.py` & `skypilot-nightly-1.0.0.dev20230804/sky/provision/aws/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/provision/gcp/instance.py` & `skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/provision/gcp/instance_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/provision/gcp/instance_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/resources.py` & `skypilot-nightly-1.0.0.dev20230804/sky/resources.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/setup_files/MANIFEST.in` & `skypilot-nightly-1.0.0.dev20230804/sky/setup_files/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/setup_files/setup.py` & `skypilot-nightly-1.0.0.dev20230804/sky/setup_files/setup.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/sky_logging.py` & `skypilot-nightly-1.0.0.dev20230804/sky/sky_logging.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/LICENSE` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/LICENSE`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/attempt_skylet.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/attempt_skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/autostop_lib.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/autostop_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/configs.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/configs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/constants.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/events.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/events.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/job_lib.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/job_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/log_lib.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/log_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/cloudwatch/cloudwatch_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/aws/utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/aws/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/azure-config-template.json` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-config-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/azure-vm-template.json` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/azure-vm-template.json`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/azure/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/azure/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/constants.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/node.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/gcp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/gcp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/ibm/vpc_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/ibm/vpc_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/kubernetes/utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/kubernetes/utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/lambda_cloud/lambda_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/lambda_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/lambda_cloud/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/lambda_cloud/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/oci/query_helper.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/oci/query_helper.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/node_provider.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/node_provider.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/providers/scp/scp_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/providers/scp/scp_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/__init__.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/log_monitor.py.patch` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/log_monitor.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/resource_demand_scheduler.py.patch` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/resource_demand_scheduler.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/ray_patches/worker.py.patch` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/ray_patches/worker.py.patch`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/skylet.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/skylet.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skylet/subprocess_daemon.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skylet/subprocess_daemon.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/skypilot_config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/skypilot_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/__init__.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/__init__.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/constants.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/controller.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/controller.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/dashboard.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/static/favicon.ico` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/dashboard/templates/index.html` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/dashboard/templates/index.html`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/recovery_strategy.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/recovery_strategy.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,25 @@
-"""The strategy to handle launching/recovery/termination of spot clusters."""
+"""The strategy to handle launching/recovery/termination of spot clusters.
+
+In the YAML file, the user can specify the strategy to use for spot jobs.
+
+resources:
+    spot_recovery: EAGER_NEXT_REGION
+"""
 import time
 import traceback
 import typing
 from typing import Optional, Tuple
 
 import sky
+from sky import backends
 from sky import exceptions
 from sky import global_user_state
 from sky import sky_logging
 from sky import status_lib
-from sky import backends
 from sky.backends import backend_utils
 from sky.skylet import job_lib
 from sky.spot import spot_utils
 from sky.usage import usage_lib
 from sky.utils import common_utils
 from sky.utils import ux_utils
 
@@ -353,15 +359,16 @@
                     return None
             gap_seconds = backoff.current_backoff()
             logger.info('Retrying to launch the spot cluster in '
                         f'{gap_seconds:.1f} seconds.')
             time.sleep(gap_seconds)
 
 
-class FailoverStrategyExecutor(StrategyExecutor, name='FAILOVER', default=True):
+class FailoverStrategyExecutor(StrategyExecutor, name='FAILOVER',
+                               default=False):
     """Failover strategy: wait in same region and failover after timout."""
 
     _MAX_RETRY_CNT = 240  # Retry for 4 hours.
 
     def __init__(self, cluster_name: str, backend: 'backends.Backend',
                  task: 'task_lib.Task', retry_until_up: bool) -> None:
         super().__init__(cluster_name, backend, task, retry_until_up)
@@ -381,29 +388,28 @@
             handle = global_user_state.get_handle_from_cluster_name(
                 self.cluster_name)
             assert isinstance(handle, backends.CloudVmRayResourceHandle), (
                 'Cluster should be launched.', handle)
             launched_resources = handle.launched_resources
             self._launched_cloud_region = (launched_resources.cloud,
                                            launched_resources.region)
+        else:
+            self._launched_cloud_region = None
         return job_submitted_at
 
     def recover(self) -> float:
         # 1. Cancel the jobs and launch the cluster with the STOPPED status,
         #    so that it will try on the current region first until timeout.
         # 2. Tear down the cluster, if the step 1 failed to launch the cluster.
         # 3. Launch the cluster with no cloud/region constraint or respect the
         #    original user specification.
 
         # Step 1
         self._try_cancel_all_jobs()
 
-        # Retry the entire block until the cluster is up, so that the ratio of
-        # the time spent in the current region and the time spent in the other
-        # region is consistent during the retry.
         while True:
             # Add region constraint to the task, to retry on the same region
             # first (if valid).
             if self._launched_cloud_region is not None:
                 task = self.dag.tasks[0]
                 resources = list(task.resources)[0]
                 original_resources = resources
@@ -418,26 +424,100 @@
                 task.set_resources({original_resources})
                 if job_submitted_at is not None:
                     return job_submitted_at
 
             # Step 2
             logger.debug('Terminating unhealthy spot cluster and '
                          'reset cloud region.')
-            self._launched_cloud_region = None
             terminate_cluster(self.cluster_name)
 
             # Step 3
             logger.debug('Relaunch the cluster  without constraining to prior '
                          'cloud/region.')
             # Not using self.launch to avoid the retry until up logic.
             job_submitted_at = self._launch(max_retry=self._MAX_RETRY_CNT,
                                             raise_on_failure=False)
             if job_submitted_at is None:
                 # Failed to launch the cluster.
                 if self.retry_until_up:
+                    gap_seconds = self.RETRY_INIT_GAP_SECONDS
+                    logger.info('Retrying to recover the spot cluster in '
+                                f'{gap_seconds:.1f} seconds.')
+                    time.sleep(gap_seconds)
+                    continue
+                with ux_utils.print_exception_no_traceback():
+                    raise exceptions.ResourcesUnavailableError(
+                        f'Failed to recover the spot cluster after retrying '
+                        f'{self._MAX_RETRY_CNT} times.')
+
+            return job_submitted_at
+
+
+class EagerFailoverStrategyExecutor(FailoverStrategyExecutor,
+                                    name='EAGER_NEXT_REGION',
+                                    default=True):
+    """Eager failover strategy.
+
+    This strategy is an extension of the FAILOVER strategy. Instead of waiting
+    in the same region when the preemption happens, it immediately terminates
+    the cluster and relaunches it in a different region. This is based on the
+    observation that the preemption is likely to happen again shortly in the
+    same region, so trying other regions first is more likely to get a longer
+    running cluster.
+    """
+
+    def recover(self) -> float:
+        # 1. Terminate the current cluster
+        # 2. Launch again by explicitly blocking the previously launched region
+        # (this will failover through the entire search space except the
+        # previously launched region)
+        # 3. (If step 2 failed) Retry forever: Launch again with no blocked
+        # locations (this will failover through the entire search space)
+        #
+        # The entire search space is defined by the original task request,
+        # task.resources.
+
+        # Step 1
+        logger.debug('Terminating unhealthy spot cluster and '
+                     'reset cloud region.')
+        terminate_cluster(self.cluster_name)
+
+        # Step 2
+        logger.debug('Relaunch the cluster skipping the previously launched '
+                     'cloud/region.')
+        if self._launched_cloud_region is not None:
+            task = self.dag.tasks[0]
+            requested_resources = list(task.resources)[0]
+            if (requested_resources.region is None and
+                    requested_resources.zone is None):
+                # Optimization: We only block the previously launched region,
+                # if the requested resources does not specify a region or zone,
+                # because, otherwise, we will spend unnecessary time for
+                # skipping the only specified region/zone.
+                launched_cloud, launched_region = self._launched_cloud_region
+                task.blocked_resources = {
+                    requested_resources.copy(cloud=launched_cloud,
+                                             region=launched_region)
+                }
+                # Not using self.launch to avoid the retry until up logic.
+                job_submitted_at = self._launch(raise_on_failure=False)
+                task.blocked_resources = None
+                if job_submitted_at is not None:
+                    return job_submitted_at
+
+        while True:
+            # Step 3
+            logger.debug('Relaunch the cluster without constraining to prior '
+                         'cloud/region.')
+            # Not using self.launch to avoid the retry until up logic.
+            job_submitted_at = self._launch(max_retry=self._MAX_RETRY_CNT,
+                                            raise_on_failure=False)
+            if job_submitted_at is None:
+                # Failed to launch the cluster.
+                if self.retry_until_up:
                     gap_seconds = self.RETRY_INIT_GAP_SECONDS
                     logger.info('Retrying to recover the spot cluster in '
                                 f'{gap_seconds:.1f} seconds.')
                     time.sleep(gap_seconds)
                     continue
                 with ux_utils.print_exception_no_traceback():
                     raise exceptions.ResourcesUnavailableError(
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/spot_state.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_state.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/spot/spot_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/spot/spot_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/status_lib.py` & `skypilot-nightly-1.0.0.dev20230804/sky/status_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/task.py` & `skypilot-nightly-1.0.0.dev20230804/sky/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Task: a coarse-grained stage in an application."""
 import inspect
 import json
 import os
 import re
 import typing
-from typing import Any, Callable, Dict, List, Optional, Set, Tuple, Union
+from typing import Any, Callable, Dict, Iterable, List, Optional, Set, Tuple, Union
 
 import yaml
 
 import sky
 from sky import clouds
 from sky import exceptions
 from sky import global_user_state
@@ -114,14 +114,15 @@
         run: Optional[CommandOrCommandGen] = None,
         envs: Optional[Dict[str, str]] = None,
         workdir: Optional[str] = None,
         num_nodes: Optional[int] = None,
         # Advanced:
         docker_image: Optional[str] = None,
         event_callback: Optional[str] = None,
+        blocked_resources: Optional[Iterable['resources_lib.Resources']] = None,
     ):
         """Initializes a Task.
 
         All fields are optional.  ``Task.run`` is the actual program: either a
         shell command to run (str) or a command generator for different nodes
         (lambda; see below).
 
@@ -168,14 +169,15 @@
             treated as 1 node.  If > 1, each node will execute its own
             setup/run command, where ``run`` can either be a str, meaning all
             nodes get the same command, or a lambda, with the semantics
             documented above.
           docker_image: (EXPERIMENTAL: Only in effect when LocalDockerBackend
             is used.) The base docker image that this Task will be built on.
             Defaults to 'gpuci/miniforge-cuda:11.4-devel-ubuntu18.04'.
+          blocked_resources: A set of resources that this task cannot run on.
         """
         self.name = name
         self.run = run
         self.storage_mounts: Dict[str, storage_lib.Storage] = {}
         self.storage_plans: Dict[storage_lib.Storage,
                                  storage_lib.StoreType] = {}
         self.setup = setup
@@ -190,14 +192,17 @@
 
         self.inputs = None
         self.outputs = None
         self.estimated_inputs_size_gigabytes = None
         self.estimated_outputs_size_gigabytes = None
         # Default to CPUNode
         self.resources = {sky.Resources()}
+        # Resources that this task cannot run on.
+        self.blocked_resources = blocked_resources
+
         self.time_estimator_func: Optional[Callable[['sky.Resources'],
                                                     int]] = None
         self.file_mounts: Optional[Dict[str, str]] = None
 
         # Only set when 'self' is a spot controller task: 'self.spot_dag' is
         # the underlying managed spot dag (sky.Dag object).
         self.spot_dag: Optional['sky.Dag'] = None
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/aws-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/aws-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/azure-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/azure-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/gcp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/gcp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/ibm-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/ibm-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/kubernetes-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/kubernetes-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/lambda-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/lambda-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/local-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/local-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/oci-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/oci-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/scp-ray.yml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/scp-ray.yml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/templates/spot-controller.yaml.j2` & `skypilot-nightly-1.0.0.dev20230804/sky/templates/spot-controller.yaml.j2`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/usage/constants.py` & `skypilot-nightly-1.0.0.dev20230804/sky/usage/constants.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/usage/usage_lib.py` & `skypilot-nightly-1.0.0.dev20230804/sky/usage/usage_lib.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/accelerator_registry.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/accelerator_registry.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/cli_utils/status_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/cli_utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/command_runner.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/command_runner.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/common_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/dag_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/dag_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/db_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/env_options.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/env_options.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/create_cluster.sh` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/create_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/delete_cluster.sh` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/delete_cluster.sh`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/kubernetes/generate_kind_config.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/kubernetes/generate_kind_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/log_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/schemas.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/schemas.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/subprocess_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/subprocess_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/timeline.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/timeline.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/tpu_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/tpu_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/ux_utils.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/ux_utils.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/sky/utils/validator.py` & `skypilot-nightly-1.0.0.dev20230804/sky/utils/validator.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/PKG-INFO` & `skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skypilot-nightly
-Version: 1.0.0.dev20230803
+Version: 1.0.0.dev20230804
 Summary: SkyPilot: An intercloud broker for the clouds
 Author: SkyPilot Team
 License: Apache 2.0
 Project-URL: Homepage, https://github.com/skypilot-org/skypilot
 Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230803
+Metadata-Version: 2.1 Name: skypilot-nightly Version: 1.0.0.dev20230804
 Summary: SkyPilot: An intercloud broker for the clouds Author: SkyPilot Team
 License: Apache 2.0 Project-URL: Homepage, https://github.com/skypilot-org/
 skypilot Project-URL: Issues, https://github.com/skypilot-org/skypilot/issues
 Project-URL: Discussion, https://github.com/skypilot-org/skypilot/discussions
 Project-URL: Documentation, https://skypilot.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/SOURCES.txt` & `skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/skypilot_nightly.egg-info/requires.txt` & `skypilot-nightly-1.0.0.dev20230804/skypilot_nightly.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_cli.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_config.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_jobs.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_jobs.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_list_accelerators.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_list_accelerators.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_onprem.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_onprem.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_optimizer_dryruns.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_dryruns.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_optimizer_random_dag.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_optimizer_random_dag.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_smoke.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_smoke.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_spot.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_spot.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_storage.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `skypilot-nightly-1.0.0.dev20230803/tests/test_wheels.py` & `skypilot-nightly-1.0.0.dev20230804/tests/test_wheels.py`

 * *Files identical despite different names*

