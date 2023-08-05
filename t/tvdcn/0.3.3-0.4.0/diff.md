# Comparing `tmp/tvdcn-0.3.3.tar.gz` & `tmp/tvdcn-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tvdcn-0.3.3.tar", last modified: Fri Jul  7 18:51:30 2023, max compression
+gzip compressed data, was "tvdcn-0.4.0.tar", last modified: Sat Aug  5 19:15:44 2023, max compression
```

## Comparing `tvdcn-0.3.3.tar` & `tvdcn-0.4.0.tar`

### file list

```diff
@@ -1,56 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.094404 tvdcn-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-07 18:49:18.000000 tvdcn-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-07 18:49:18.000000 tvdcn-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-07 18:51:30.094404 tvdcn-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7714 2023-07-07 18:49:18.000000 tvdcn-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-07 18:49:18.000000 tvdcn-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-07 18:49:18.000000 tvdcn-0.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-07-07 18:51:30.094404 tvdcn-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-07-07 18:49:18.000000 tvdcn-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.074403 tvdcn-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tests/test_compatibility_with_torchvision.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tests/test_grad.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.074403 tvdcn-0.3.3/tvdcn/
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.078403 tvdcn-0.3.3/tvdcn/csrc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.082404 tvdcn-0.3.3/tvdcn/csrc/ops/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.082404 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/
--rw-r--r--   0 runner    (1001) docker     (123)    20496 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27299 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    35674 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.086404 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/
--rw-r--r--   0 runner    (1001) docker     (123)    23594 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    30424 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    38850 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    26564 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    30412 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34230 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv3d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    27339 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    31183 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    34997 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.086404 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/
--rw-r--r--   0 runner    (1001) docker     (123)    10352 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv1d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    13592 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv2d_kernels.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/dispatch/deform_conv3d_kernels.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.090404 tvdcn-0.3.3/tvdcn/csrc/ops/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/ops/utils/tensor_utils.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/csrc/tvdcn.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.090404 tvdcn-0.3.3/tvdcn/ops/
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.094404 tvdcn-0.3.3/tvdcn/ops/activations/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/activations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/activations/mask_sigmoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/activations/mask_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/deform_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/ops/deform_conv_transpose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-07-07 18:49:18.000000 tvdcn-0.3.3/tvdcn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 18:51:30.078403 tvdcn-0.3.3/tvdcn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8995 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-07 18:51:30.000000 tvdcn-0.3.3/tvdcn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-08-05 19:13:49.000000 tvdcn-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-08-05 19:13:49.000000 tvdcn-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-08-05 19:15:44.160912 tvdcn-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7533 2023-08-05 19:13:49.000000 tvdcn-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-05 19:13:49.000000 tvdcn-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 19:13:49.000000 tvdcn-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-08-05 19:15:44.160912 tvdcn-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3800 2023-08-05 19:13:49.000000 tvdcn-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tests/test_compatibility_with_torchvision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tests/test_grad.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tvdcn/
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tvdcn/csrc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.148911 tvdcn-0.4.0/tvdcn/csrc/ops/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.148911 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autocast/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.152912 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5143 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5130 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/autograd/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.156911 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)    22174 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23851 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    27875 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    38520 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    31869 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24019 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28031 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32013 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/
+-rw-r--r--   0 runner    (1001) docker     (123)    25429 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    23843 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32763 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    27867 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41853 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    31861 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    24011 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose1d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28023 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose2d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32005 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv3d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose2d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/deform_conv_transpose3d.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/csrc/ops/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/ops/utils/tensor_utils.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/csrc/tvdcn.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.160912 tvdcn-0.4.0/tvdcn/ops/activations/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/activations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/activations/mask_sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/activations/mask_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30949 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/deform_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33905 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/ops/deform_conv_transpose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-08-05 19:13:49.000000 tvdcn-0.4.0/tvdcn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:15:44.144911 tvdcn-0.4.0/tvdcn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8814 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2439 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 19:15:44.000000 tvdcn-0.4.0/tvdcn.egg-info/top_level.txt
```

### Comparing `tvdcn-0.3.3/LICENSE.txt` & `tvdcn-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/PKG-INFO` & `tvdcn-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.3
+Version: 0.4.0
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -32,35 +32,32 @@
 
 Torchvision+ Deformable Convolution Networks
 ========
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)](https://github.com/inspiros/tvdcn/actions)
 [![PyPI](https://img.shields.io/pypi/v/tvdcn)](https://pypi.org/project/tvdcn)
 [![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)](LICENSE.txt)
 
-This package contains the PyTorch implementations of the **2D Deformable Convolution** operation
+This package contains the PyTorch implementations of the **Deformable Convolution** operation
 (the commonly used  `torchvision.ops.deform_conv2d`) proposed in https://arxiv.org/abs/1811.11168,
-as well as its **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
-
-And beyond that, the package also provides the **transposed** versions of them,
-which interestingly noone has ever proposed to use.
-The main idea is, while `offset` in deformable convolution guides the convolution kernel where to get the inputs to
-compute the output; in transposed deformable convolution, it guides the convolution kernel where to write the outputs.
+and the **Transposed Deformable Convolution** proposed in https://arxiv.org/abs/2210.09446
+(currently without interpolation kernel scaling).
+It also supports their **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
 
 ## Highlights
 
 - **Supported operations:** _(All are implemented in C++/Cuda)_
 
   - `tvdcn.ops.deform_conv1d`
   - `tvdcn.ops.deform_conv2d`
   - `tvdcn.ops.deform_conv3d`
   - `tvdcn.ops.deform_conv_transpose1d`
   - `tvdcn.ops.deform_conv_transpose2d`
   - `tvdcn.ops.deform_conv_transpose3d`
 
-- And the following **supplementary operations** (for activating `mask`):
+- And the following **supplementary operations** (`mask` activation proposed in https://arxiv.org/abs/2211.05778):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
 - Both `offset` and `mask` can be turned off, and can be applied in separate groups.
 
 - All the `nn.Module` wrappers for these operations are implemented,
```

### Comparing `tvdcn-0.3.3/README.md` & `tvdcn-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 Torchvision+ Deformable Convolution Networks
 ========
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)](https://github.com/inspiros/tvdcn/actions)
 [![PyPI](https://img.shields.io/pypi/v/tvdcn)](https://pypi.org/project/tvdcn)
 [![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)](LICENSE.txt)
 
-This package contains the PyTorch implementations of the **2D Deformable Convolution** operation
+This package contains the PyTorch implementations of the **Deformable Convolution** operation
 (the commonly used  `torchvision.ops.deform_conv2d`) proposed in https://arxiv.org/abs/1811.11168,
-as well as its **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
-
-And beyond that, the package also provides the **transposed** versions of them,
-which interestingly noone has ever proposed to use.
-The main idea is, while `offset` in deformable convolution guides the convolution kernel where to get the inputs to
-compute the output; in transposed deformable convolution, it guides the convolution kernel where to write the outputs.
+and the **Transposed Deformable Convolution** proposed in https://arxiv.org/abs/2210.09446
+(currently without interpolation kernel scaling).
+It also supports their **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
 
 ## Highlights
 
 - **Supported operations:** _(All are implemented in C++/Cuda)_
 
   - `tvdcn.ops.deform_conv1d`
   - `tvdcn.ops.deform_conv2d`
   - `tvdcn.ops.deform_conv3d`
   - `tvdcn.ops.deform_conv_transpose1d`
   - `tvdcn.ops.deform_conv_transpose2d`
   - `tvdcn.ops.deform_conv_transpose3d`
 
-- And the following **supplementary operations** (for activating `mask`):
+- And the following **supplementary operations** (`mask` activation proposed in https://arxiv.org/abs/2211.05778):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
 - Both `offset` and `mask` can be turned off, and can be applied in separate groups.
 
 - All the `nn.Module` wrappers for these operations are implemented,
```

### Comparing `tvdcn-0.3.3/pyproject.toml` & `tvdcn-0.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/setup.cfg` & `tvdcn-0.4.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/setup.py` & `tvdcn-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,22 +27,23 @@
     extensions_dir = os.path.join(PACKAGE_ROOT, 'csrc')
 
     main_file = (glob.glob(os.path.join(extensions_dir, '*.cpp')) +
                  glob.glob(os.path.join(extensions_dir, 'ops', '*.cpp'))
                  )
 
     source_cpu = (glob.glob(os.path.join(extensions_dir, 'ops', 'cpu', '*.cpp')) +
-                  glob.glob(os.path.join(extensions_dir, 'ops', 'dispatch', '*.cpp')) +
                   glob.glob(os.path.join(extensions_dir, 'ops', 'autograd', '*.cpp')) +
                   glob.glob(os.path.join(extensions_dir, 'ops', 'quantized', 'cpu', '*.cpp')) +
                   glob.glob(os.path.join(extensions_dir, 'ops', 'utils', '*.cpp'))
                   )
 
-    source_cuda = glob.glob(os.path.join(extensions_dir, 'ops', 'cuda', '*.cu'))
-    source_cuda += glob.glob(os.path.join(extensions_dir, 'ops', 'autocast', '*.cpp'))
+    source_cuda = (glob.glob(os.path.join(extensions_dir, 'ops', 'cuda', '*.cu')) +
+                   glob.glob(os.path.join(extensions_dir, 'ops', 'cuda', '*.cpp')) +
+                   glob.glob(os.path.join(extensions_dir, 'ops', 'autocast', '*.cpp'))
+                   )
 
     sources = main_file + source_cpu
     extension = CppExtension
     extra_compile_args = {'cxx': []}
     extra_compile_args['cxx'].append('/std:c++17' if sys.platform == 'win32' else '-std=c++17')
     define_macros = []
 
@@ -96,14 +97,14 @@
 
 
 def setup_package():
     setup(
         version=get_version(),
         ext_modules=get_extensions(),
         cmdclass={
-            'build_ext': torch.utils.cpp_extension.BuildExtension.with_options(use_ninja=False)
+            'build_ext': torch.utils.cpp_extension.BuildExtension
         },
     )
 
 
 if __name__ == '__main__':
     setup_package()
```

### Comparing `tvdcn-0.3.3/tests/test_compatibility_with_torchvision.py` & `tvdcn-0.4.0/tests/test_compatibility_with_torchvision.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tests/test_grad.py` & `tvdcn-0.4.0/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv1d_kernels_cpu.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_common_kernels.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,477 +1,479 @@
 #include <ATen/ATen.h>
 
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
-        namespace {
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t sample(
-                    const at::TensorAccessor<scalar_t, 3> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const index_t x) {
-                return (0 <= x && x < width) ? input[b][c][x] : static_cast<scalar_t>(0);
-            }
+        namespace cpu {
+            namespace {
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t sample(
+                        const at::TensorAccessor<scalar_t, 3> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const index_t x) {
+                    return (0 <= x && x < width) ? input[b][c][x] : static_cast<scalar_t>(0);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t interpolate_sample(
-                    const at::TensorAccessor<scalar_t, 3> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const scalar_t x) {
-                if (x <= -1 || width <= x)
-                    return 0;
-
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dx_h = x - x_l;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_x_l = x_l >= 0;
-                bool valid_x_h = x_h < width;
-
-                scalar_t val = 0;
-                if (valid_x_l) val += dx_l * input[b][c][x_l];
-                if (valid_x_h) val += dx_h * input[b][c][x_h];
-                return val;
-            }
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t interpolate_sample(
+                        const at::TensorAccessor<scalar_t, 3> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const scalar_t x) {
+                    if (x <= -1 || width <= x)
+                        return 0;
+
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_x_l = x_l >= 0;
+                    bool valid_x_h = x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_x_l) val += dx_l * input[b][c][x_l];
+                    if (valid_x_h) val += dx_h * input[b][c][x_h];
+                    return val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ void insert(
-                    at::TensorAccessor<scalar_t, 3> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const index_t x,
-                    const scalar_t val) {
-                if (0 <= x && x < width)
-                    output[b][c][x] += val;
-            }
+                template<typename scalar_t, typename index_t>
+                __forceinline__ void insert(
+                        at::TensorAccessor<scalar_t, 3> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const index_t x,
+                        const scalar_t val) {
+                    if (0 <= x && x < width)
+                        output[b][c][x] += val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ void interpolate_insert(
-                    at::TensorAccessor<scalar_t, 3> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const scalar_t x,
-                    const scalar_t val) {
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
+                template<typename scalar_t, typename index_t>
+                __forceinline__ void interpolate_insert(
+                        at::TensorAccessor<scalar_t, 3> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const scalar_t x,
+                        const scalar_t val) {
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dx_l = 1 - dx_h;
 
-                scalar_t dx_h = x - x_l;
-                scalar_t dx_l = 1 - dx_h;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
 
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
+                    if (valid_x_l) output[b][c][x_l] += dx_l * val;
+                    if (valid_x_h) output[b][c][x_h] += dx_h * val;
+                }
 
-                if (valid_x_l) output[b][c][x_l] += dx_l * val;
-                if (valid_x_h) output[b][c][x_h] += dx_h * val;
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t coordinate_weight(
+                        const at::TensorAccessor<scalar_t, 3> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const scalar_t x) {
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dx_h = 1;
+                    scalar_t dx_l = -1;
+
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_x_l) val += dx_l * input[b][c][x_l];
+                    if (valid_x_h) val += dx_h * input[b][c][x_h];
+                    return val;
+                }
             }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t coordinate_weight(
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static void arr2col_kernel(
+                    const index_t n_kernels,
                     const at::TensorAccessor<scalar_t, 3> input,
-                    const index_t b,
-                    const index_t c,
+                    const at::TensorAccessor<scalar_t, 5> offset,
+                    const at::TensorAccessor<scalar_t, 4> mask,
                     const index_t width,
-                    const scalar_t x) {
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dx_h = 1;
-                scalar_t dx_l = -1;
-
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                scalar_t val = 0;
-                if (valid_x_l) val += dx_l * input[b][c][x_l];
-                if (valid_x_h) val += dx_h * input[b][c][x_h];
-                return val;
-            }
-        }
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t in_channels,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 4> columns) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t w = index % out_w;
+                    const index_t c = (index / out_w) % in_channels;
+                    const index_t b = index / (out_w * in_channels);
 
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void arr2col_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 3> input,
-                const at::TensorAccessor<scalar_t, 5> offset,
-                const at::TensorAccessor<scalar_t, 4> mask,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t in_channels,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 4> columns) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t w = index % out_w;
-                const index_t c = (index / out_w) % in_channels;
-                const index_t b = index / (out_w * in_channels);
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                for (index_t i = 0; i < weight_w; ++i) {
-                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
+                    const index_t offset_group_idx = c / c_per_offset_group;
+                    const index_t mask_group_idx = c / c_per_mask_group;
 
-                    scalar_t val, mask_val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
-                                input, b, c, width,
-                                x + offset[b][offset_group_idx][i][0][w]);
-                    else
-                        val = sample(input, b, c, width, x);
+                    for (index_t i = 0; i < weight_w; ++i) {
+                        const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    if constexpr (modulated)
-                        mask_val = mask[b][mask_group_idx][i][w];
-                    else
-                        mask_val = static_cast<scalar_t>(1);
+                        scalar_t val, mask_val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, width,
+                                    x + offset[b][offset_group_idx][i][0][w]);
+                        else
+                            val = sample(input, b, c, width, x);
+
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
 
-                    columns[c][i][b][w] = val * mask_val;
+                        columns[c][i][b][w] = val * mask_val;
+                    }
                 }
             }
-        }
 
-        void arr2col_cpu(
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &columns) {
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "arr2col_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto columns_accessor =
-                            columns.accessor<scalar_t, 4>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        arr2col_kernel<deformable, modulated, scalar_t, index_t>(
-                                n_kernels,
-                                input.accessor<scalar_t, 3>(),
-                                offset.accessor<scalar_t, 5>(),
-                                mask.accessor<scalar_t, 4>(),
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                in_channels,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                columns_accessor);
+            void arr2col(
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &columns) {
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        input.scalar_type(), "arr2col", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto columns_accessor =
+                                columns.accessor<scalar_t, 4>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            arr2col_kernel<deformable, modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    input.accessor<scalar_t, 3>(),
+                                    offset.accessor<scalar_t, 5>(),
+                                    mask.accessor<scalar_t, 4>(),
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    in_channels,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    columns_accessor);
+                        }));
                     }));
                 }));
-            }));
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void col2arr_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 4> columns,
-                const at::TensorAccessor<scalar_t, 5> offset,
-                const at::TensorAccessor<scalar_t, 4> mask,
-                const index_t in_channels,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 3> grad_input) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t i = index % weight_w;
-                const index_t w = (index / weight_w) % out_w;
-                const index_t c = (index / (weight_w * out_w)) % in_channels;
-                const index_t b = (index / (weight_w * out_w * in_channels));
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                const index_t x = (w * stride_w - pad_w) + i * dilation_w;
-
-                scalar_t mask_val;
-                if constexpr (modulated)
-                    mask_val = mask[b][mask_group_idx][i][w];
-                else
-                    mask_val = static_cast<scalar_t>(1);
-
-                scalar_t val = columns[c][i][b][w] * mask_val;
-
-                if constexpr (deformable)
-                    interpolate_insert(
-                            grad_input, b, c, width,
-                            x + offset[b][offset_group_idx][i][0][w],
-                            val);
-                else
-                    insert(grad_input, b, c, width, x, val);
             }
-        }
 
-        void col2arr_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_input) {
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2arr_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
-                    auto grad_input_accessor =
-                            grad_input.accessor<scalar_t, 3>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2arr_kernel<deformable, modulated, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 5>(),
-                                mask.accessor<scalar_t, 4>(),
-                                in_channels,
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_input_accessor);
-                    }));
-                }));
-            }));
-        }
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static void col2arr_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 4> columns,
+                    const at::TensorAccessor<scalar_t, 5> offset,
+                    const at::TensorAccessor<scalar_t, 4> mask,
+                    const index_t in_channels,
+                    const index_t width,
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 3> grad_input) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t i = index % weight_w;
+                    const index_t w = (index / weight_w) % out_w;
+                    const index_t c = (index / (weight_w * out_w)) % in_channels;
+                    const index_t b = (index / (weight_w * out_w * in_channels));
 
-        template<bool modulated, typename scalar_t, typename index_t>
-        static void deform_conv1d_compute_grad_offset_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 4> columns,
-                const at::TensorAccessor<scalar_t, 3> input,
-                const at::TensorAccessor<scalar_t, 5> offset,
-                const at::TensorAccessor<scalar_t, 4> mask,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t offset_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 5> grad_offset) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t i = index % weight_w;
-                const index_t w = (index / weight_w) % out_w;
-                const index_t g = (index / (weight_w * out_w)) % offset_groups;
-                const index_t b = index / (weight_w * out_w * offset_groups);
-
-                scalar_t grad_offset_val = 0;
-
-                const index_t c_start = g * c_per_offset_group;
-                const index_t c_end = c_start + c_per_offset_group;
-                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    scalar_t weight = coordinate_weight(
-                            input, b, c, width,
-                            x + offset[b][g][i][0][w]);
-
                     scalar_t mask_val;
                     if constexpr (modulated)
                         mask_val = mask[b][mask_group_idx][i][w];
                     else
                         mask_val = static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][b][w] * weight * mask_val;
-                }
+                    scalar_t val = columns[c][i][b][w] * mask_val;
 
-                grad_offset[b][g][i][0][w] = grad_offset_val;
+                    if constexpr (deformable)
+                        interpolate_insert(
+                                grad_input, b, c, width,
+                                x + offset[b][offset_group_idx][i][0][w],
+                                val);
+                    else
+                        insert(grad_input, b, c, width, x, val);
+                }
             }
-        }
 
-        void deform_conv1d_compute_grad_offset_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_offset) {
-            if (!deformable) return;
-            const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv1d_compute_grad_offset_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_offset_accessor =
-                            grad_offset.accessor<scalar_t, 5>();
-                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv1d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 4>(),
-                                input.accessor<scalar_t, 3>(),
-                                offset.accessor<scalar_t, 5>(),
-                                mask.accessor<scalar_t, 4>(),
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                offset_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_offset_accessor);
+            void col2arr(
+                    const at::Tensor &columns,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_input) {
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "col2arr", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                        auto grad_input_accessor =
+                                grad_input.accessor<scalar_t, 3>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            col2arr_kernel<deformable, modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 4>(),
+                                    offset.accessor<scalar_t, 5>(),
+                                    mask.accessor<scalar_t, 4>(),
+                                    in_channels,
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_input_accessor);
+                        }));
                     }));
                 }));
-            }));
-        }
+            }
 
-        template<bool deformable, typename scalar_t, typename index_t>
-        static void deform_conv1d_compute_grad_mask_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 4> columns,
-                const at::TensorAccessor<scalar_t, 3> input,
-                const at::TensorAccessor<scalar_t, 5> offset,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t mask_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 4> grad_mask) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t i = index % weight_w;
-                const index_t w = (index / weight_w) % out_w;
-                const index_t g = (index / (weight_w * out_w)) % mask_groups;
-                const index_t b = index / (out_w * weight_w * mask_groups);
-
-                scalar_t grad_mask_val = 0;
-
-                const index_t c_start = g * c_per_mask_group;
-                const index_t c_end = c_start + c_per_mask_group;
-                for (index_t c = c_start; c < c_end; ++c) {
-                    const index_t offset_group_idx = c / c_per_offset_group;
+            template<bool modulated, typename scalar_t, typename index_t>
+            static void deform_conv1d_compute_grad_offset_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 4> columns,
+                    const at::TensorAccessor<scalar_t, 3> input,
+                    const at::TensorAccessor<scalar_t, 5> offset,
+                    const at::TensorAccessor<scalar_t, 4> mask,
+                    const index_t width,
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t offset_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 5> grad_offset) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t i = index % weight_w;
+                    const index_t w = (index / weight_w) % out_w;
+                    const index_t g = (index / (weight_w * out_w)) % offset_groups;
+                    const index_t b = index / (weight_w * out_w * offset_groups);
+
+                    scalar_t grad_offset_val = 0;
+
+                    const index_t c_start = g * c_per_offset_group;
+                    const index_t c_end = c_start + c_per_offset_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t mask_group_idx = c / c_per_mask_group;
 
-                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
+                        const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    scalar_t val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
+                        scalar_t weight = coordinate_weight(
                                 input, b, c, width,
-                                x + offset[b][offset_group_idx][i][0][w]);
-                    else
-                        val = sample(input, b, c, width, x);
+                                x + offset[b][g][i][0][w]);
+
+                        scalar_t mask_val;
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
+
+                        grad_offset_val += columns[c][i][b][w] * weight * mask_val;
+                    }
 
-                    grad_mask_val += columns[c][i][b][w] * val;
+                    grad_offset[b][g][i][0][w] = grad_offset_val;
                 }
+            }
 
-                grad_mask[b][g][i][w] = grad_mask_val;
+            void deform_conv1d_compute_grad_offset(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_offset) {
+                if (!deformable) return;
+                const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv1d_compute_grad_offset", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_offset_accessor =
+                                grad_offset.accessor<scalar_t, 5>();
+                        TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                            deform_conv1d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 4>(),
+                                    input.accessor<scalar_t, 3>(),
+                                    offset.accessor<scalar_t, 5>(),
+                                    mask.accessor<scalar_t, 4>(),
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    offset_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_offset_accessor);
+                        }));
+                    }));
+                }));
             }
-        }
 
-        void deform_conv1d_compute_grad_mask_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_mask) {
-            if (!modulated) return;
-            const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv1d_compute_grad_mask_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_mask_accessor =
-                            grad_mask.accessor<scalar_t, 4>();
-                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv1d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 4>(),
-                                input.accessor<scalar_t, 3>(),
-                                offset.accessor<scalar_t, 5>(),
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                mask_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_mask_accessor);
+            template<bool deformable, typename scalar_t, typename index_t>
+            static void deform_conv1d_compute_grad_mask_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 4> columns,
+                    const at::TensorAccessor<scalar_t, 3> input,
+                    const at::TensorAccessor<scalar_t, 5> offset,
+                    const index_t width,
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t mask_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 4> grad_mask) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t i = index % weight_w;
+                    const index_t w = (index / weight_w) % out_w;
+                    const index_t g = (index / (weight_w * out_w)) % mask_groups;
+                    const index_t b = index / (out_w * weight_w * mask_groups);
+
+                    scalar_t grad_mask_val = 0;
+
+                    const index_t c_start = g * c_per_mask_group;
+                    const index_t c_end = c_start + c_per_mask_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t offset_group_idx = c / c_per_offset_group;
+
+                        const index_t x = (w * stride_w - pad_w) + i * dilation_w;
+
+                        scalar_t val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, width,
+                                    x + offset[b][offset_group_idx][i][0][w]);
+                        else
+                            val = sample(input, b, c, width, x);
+
+                        grad_mask_val += columns[c][i][b][w] * val;
+                    }
+
+                    grad_mask[b][g][i][w] = grad_mask_val;
+                }
+            }
+
+            void deform_conv1d_compute_grad_mask(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_mask) {
+                if (!modulated) return;
+                const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv1d_compute_grad_mask", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_mask_accessor =
+                                grad_mask.accessor<scalar_t, 4>();
+                        TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                            deform_conv1d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 4>(),
+                                    input.accessor<scalar_t, 3>(),
+                                    offset.accessor<scalar_t, 5>(),
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    mask_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_mask_accessor);
+                        }));
                     }));
                 }));
-            }));
+            }
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv2d_kernels_cpu.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv2d_common_kernels.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,603 +1,605 @@
 #include <ATen/ATen.h>
 
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
-        namespace {
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t sample(
-                    const at::TensorAccessor<scalar_t, 4> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const index_t y,
-                    const index_t x) {
-                return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
-            }
+        namespace cpu {
+            namespace {
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t sample(
+                        const at::TensorAccessor<scalar_t, 4> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const index_t y,
+                        const index_t x) {
+                    return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t interpolate_sample(
-                    const at::TensorAccessor<scalar_t, 4> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t y,
-                    const scalar_t x) {
-                if (y <= -1 || height <= y || x <= -1 || width <= x)
-                    return 0;
-
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_y_l = y_l >= 0;
-                bool valid_y_h = y_h < height;
-                bool valid_x_l = x_l >= 0;
-                bool valid_x_h = x_h < width;
-
-                scalar_t val = 0;
-                if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
-                if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
-                if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
-                if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
-                return val;
-            }
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t interpolate_sample(
+                        const at::TensorAccessor<scalar_t, 4> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t y,
+                        const scalar_t x) {
+                    if (y <= -1 || height <= y || x <= -1 || width <= x)
+                        return 0;
+
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_y_l = y_l >= 0;
+                    bool valid_y_h = y_h < height;
+                    bool valid_x_l = x_l >= 0;
+                    bool valid_x_h = x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
+                    if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
+                    if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
+                    if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
+                    return val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ void insert(
-                    at::TensorAccessor<scalar_t, 4> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const index_t y,
-                    const index_t x,
-                    const scalar_t val) {
-                if (0 <= y && y < height && 0 <= x && x < width)
-                    output[b][c][y][x] += val;
-            }
+                template<typename scalar_t, typename index_t>
+                __forceinline__ void insert(
+                        at::TensorAccessor<scalar_t, 4> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const index_t y,
+                        const index_t x,
+                        const scalar_t val) {
+                    if (0 <= y && y < height && 0 <= x && x < width)
+                        output[b][c][y][x] += val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ void interpolate_insert(
-                    at::TensorAccessor<scalar_t, 4> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const scalar_t val) {
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                if (valid_y_l && valid_x_l) output[b][c][y_l][x_l] += dy_l * dx_l * val;
-                if (valid_y_l && valid_x_h) output[b][c][y_l][x_h] += dy_l * dx_h * val;
-                if (valid_y_h && valid_x_l) output[b][c][y_h][x_l] += dy_h * dx_l * val;
-                if (valid_y_h && valid_x_h) output[b][c][y_h][x_h] += dy_h * dx_h * val;
+                template<typename scalar_t, typename index_t>
+                __forceinline__ void interpolate_insert(
+                        at::TensorAccessor<scalar_t, 4> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const scalar_t val) {
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    if (valid_y_l && valid_x_l) output[b][c][y_l][x_l] += dy_l * dx_l * val;
+                    if (valid_y_l && valid_x_h) output[b][c][y_l][x_h] += dy_l * dx_h * val;
+                    if (valid_y_h && valid_x_l) output[b][c][y_h][x_l] += dy_h * dx_l * val;
+                    if (valid_y_h && valid_x_h) output[b][c][y_h][x_h] += dy_h * dx_h * val;
+                }
+
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t coordinate_weight(
+                        const at::TensorAccessor<scalar_t, 4> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const index_t direction) {
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dy_h = (direction == 0) ? static_cast<scalar_t>(1) : y - y_l;
+                    scalar_t dy_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dy_h;
+                    scalar_t dx_h = (direction == 1) ? static_cast<scalar_t>(1) : x - x_l;
+                    scalar_t dx_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dx_h;
+
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
+                    if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
+                    if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
+                    if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
+                    return val;
+                }
             }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t coordinate_weight(
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static void im2col_kernel(
+                    const index_t n_kernels,
                     const at::TensorAccessor<scalar_t, 4> input,
-                    const index_t b,
-                    const index_t c,
+                    const at::TensorAccessor<scalar_t, 7> offset,
+                    const at::TensorAccessor<scalar_t, 6> mask,
                     const index_t height,
                     const index_t width,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const index_t direction) {
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dy_h = (direction == 0) ? static_cast<scalar_t>(1) : y - y_l;
-                scalar_t dy_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dy_h;
-                scalar_t dx_h = (direction == 1) ? static_cast<scalar_t>(1) : x - x_l;
-                scalar_t dx_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dx_h;
-
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                scalar_t val = 0;
-                if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
-                if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
-                if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
-                if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
-                return val;
-            }
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void im2col_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t in_channels,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 6> columns) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t w = index % out_w;
-                const index_t h = (index / out_w) % out_h;
-                const index_t c = (index / (out_w * out_h)) % in_channels;
-                const index_t b = index / (out_w * out_h * in_channels);
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                for (index_t i = 0; i < weight_h; ++i) {
-                    for (index_t j = 0; j < weight_w; ++j) {
-                        const index_t y = (h * stride_h - pad_h) + i * dilation_h;
-                        const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t in_channels,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 6> columns) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t w = index % out_w;
+                    const index_t h = (index / out_w) % out_h;
+                    const index_t c = (index / (out_w * out_h)) % in_channels;
+                    const index_t b = index / (out_w * out_h * in_channels);
 
-                        scalar_t val, mask_val;
-                        if constexpr (deformable)
-                            val = interpolate_sample(
-                                    input, b, c, height, width,
-                                    y + offset[b][offset_group_idx][i][j][0][h][w],
-                                    x + offset[b][offset_group_idx][i][j][1][h][w]);
-                        else
-                            val = sample(input, b, c, height, width, y, x);
+                    const index_t offset_group_idx = c / c_per_offset_group;
+                    const index_t mask_group_idx = c / c_per_mask_group;
 
-                        if constexpr (modulated)
-                            mask_val = mask[b][mask_group_idx][i][j][h][w];
-                        else
-                            mask_val = static_cast<scalar_t>(1);
+                    for (index_t i = 0; i < weight_h; ++i) {
+                        for (index_t j = 0; j < weight_w; ++j) {
+                            const index_t y = (h * stride_h - pad_h) + i * dilation_h;
+                            const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+
+                            scalar_t val, mask_val;
+                            if constexpr (deformable)
+                                val = interpolate_sample(
+                                        input, b, c, height, width,
+                                        y + offset[b][offset_group_idx][i][j][0][h][w],
+                                        x + offset[b][offset_group_idx][i][j][1][h][w]);
+                            else
+                                val = sample(input, b, c, height, width, y, x);
+
+                            if constexpr (modulated)
+                                mask_val = mask[b][mask_group_idx][i][j][h][w];
+                            else
+                                mask_val = static_cast<scalar_t>(1);
 
-                        columns[c][i][j][b][h][w] = val * mask_val;
+                            columns[c][i][j][b][h][w] = val * mask_val;
+                        }
                     }
                 }
             }
-        }
 
-        void im2col_cpu(
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &columns) {
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "im2col_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto columns_accessor =
-                            columns.accessor<scalar_t, 6>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        im2col_kernel<deformable, modulated, scalar_t, index_t>(
-                                n_kernels,
-                                input.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 7>(),
-                                mask.accessor<scalar_t, 6>(),
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                in_channels,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                columns_accessor);
+            void im2col(
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &columns) {
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        input.scalar_type(), "im2col", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto columns_accessor =
+                                columns.accessor<scalar_t, 6>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            im2col_kernel<deformable, modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    input.accessor<scalar_t, 4>(),
+                                    offset.accessor<scalar_t, 7>(),
+                                    mask.accessor<scalar_t, 6>(),
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    in_channels,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    columns_accessor);
+                        }));
                     }));
                 }));
-            }));
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void col2im_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
-                const index_t in_channels,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 4> grad_input) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t j = index % weight_w;
-                const index_t i = (index / weight_w) % weight_h;
-                const index_t w = (index / (weight_w * weight_h)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
-                const index_t c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
-                const index_t b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                const index_t y = (h * stride_h - pad_h) + i * dilation_h;
-                const index_t x = (w * stride_w - pad_w) + j * dilation_w;
-
-                scalar_t mask_val;
-                if constexpr (modulated)
-                    mask_val = mask[b][mask_group_idx][i][j][h][w];
-                else
-                    mask_val = static_cast<scalar_t>(1);
-
-                scalar_t val = columns[c][i][j][b][h][w] * mask_val;
-
-                if constexpr (deformable)
-                    interpolate_insert(
-                            grad_input, b, c, height, width,
-                            y + offset[b][offset_group_idx][i][j][0][h][w],
-                            x + offset[b][offset_group_idx][i][j][1][h][w],
-                            val);
-                else
-                    insert(grad_input, b, c, height, width, y, x, val);
             }
-        }
 
-        void col2im_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_input) {
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2im_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
-                    auto grad_input_accessor =
-                            grad_input.accessor<scalar_t, 4>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2im_kernel<deformable, modulated, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 6>(),
-                                offset.accessor<scalar_t, 7>(),
-                                mask.accessor<scalar_t, 6>(),
-                                in_channels,
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_input_accessor);
-                    }));
-                }));
-            }));
-        }
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static void col2im_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 6> columns,
+                    const at::TensorAccessor<scalar_t, 7> offset,
+                    const at::TensorAccessor<scalar_t, 6> mask,
+                    const index_t in_channels,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 4> grad_input) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t j = index % weight_w;
+                    const index_t i = (index / weight_w) % weight_h;
+                    const index_t w = (index / (weight_w * weight_h)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
+                    const index_t c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
+                    const index_t b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
 
-        template<bool modulated, typename scalar_t, typename index_t>
-        static void deform_conv2d_compute_grad_offset_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const at::TensorAccessor<scalar_t, 6> mask,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t offset_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 7> grad_offset) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t o = index % 2;
-                const index_t j = (index / 2) % weight_w;
-                const index_t i = (index / (2 * weight_w)) % weight_h;
-                const index_t w = (index / (2 * weight_w * weight_h)) % out_w;
-                const index_t h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
-                const index_t g = (index / (2 * weight_w * weight_h * out_w * out_h)) % offset_groups;
-                const index_t b = index / (2 * weight_w * weight_h * out_w * out_h * offset_groups);
-
-                scalar_t grad_offset_val = 0;
-
-                const index_t c_start = g * c_per_offset_group;
-                const index_t c_end = c_start + c_per_offset_group;
-                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    scalar_t weight = coordinate_weight(
-                            input, b, c, height, width,
-                            y + offset[b][g][i][j][0][h][w],
-                            x + offset[b][g][i][j][1][h][w],
-                            o);
-
                     scalar_t mask_val;
                     if constexpr (modulated)
                         mask_val = mask[b][mask_group_idx][i][j][h][w];
                     else
                         mask_val = static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
-                }
+                    scalar_t val = columns[c][i][j][b][h][w] * mask_val;
 
-                grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
+                    if constexpr (deformable)
+                        interpolate_insert(
+                                grad_input, b, c, height, width,
+                                y + offset[b][offset_group_idx][i][j][0][h][w],
+                                x + offset[b][offset_group_idx][i][j][1][h][w],
+                                val);
+                    else
+                        insert(grad_input, b, c, height, width, y, x, val);
+                }
             }
-        }
 
-        void deform_conv2d_compute_grad_offset_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_offset) {
-            if (!deformable) return;
-            const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_h * out_w * weight_h * weight_w * 2;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_offset_accessor =
-                            grad_offset.accessor<scalar_t, 7>();
-                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 6>(),
-                                input.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 7>(),
-                                mask.accessor<scalar_t, 6>(),
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                offset_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_offset_accessor);
+            void col2im(
+                    const at::Tensor &columns,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_input) {
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "col2im", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                        auto grad_input_accessor =
+                                grad_input.accessor<scalar_t, 4>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            col2im_kernel<deformable, modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 6>(),
+                                    offset.accessor<scalar_t, 7>(),
+                                    mask.accessor<scalar_t, 6>(),
+                                    in_channels,
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_input_accessor);
+                        }));
                     }));
                 }));
-            }));
-        }
+            }
 
-        template<bool deformable, typename scalar_t, typename index_t>
-        static void deform_conv2d_compute_grad_mask_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 6> columns,
-                const at::TensorAccessor<scalar_t, 4> input,
-                const at::TensorAccessor<scalar_t, 7> offset,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t mask_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 6> grad_mask) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t j = index % weight_w;
-                const index_t i = (index / weight_w) % weight_h;
-                const index_t w = (index / (weight_w * weight_h)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
-                const index_t g = (index / (weight_w * weight_h * out_w * out_h)) % mask_groups;
-                const index_t b = index / (out_w * out_h * weight_w * weight_h * mask_groups);
-
-                scalar_t grad_mask_val = 0;
-
-                const index_t c_start = g * c_per_mask_group;
-                const index_t c_end = c_start + c_per_mask_group;
-                for (index_t c = c_start; c < c_end; ++c) {
-                    const index_t offset_group_idx = c / c_per_offset_group;
+            template<bool modulated, typename scalar_t, typename index_t>
+            static void deform_conv2d_compute_grad_offset_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 6> columns,
+                    const at::TensorAccessor<scalar_t, 4> input,
+                    const at::TensorAccessor<scalar_t, 7> offset,
+                    const at::TensorAccessor<scalar_t, 6> mask,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t offset_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 7> grad_offset) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t o = index % 2;
+                    const index_t j = (index / 2) % weight_w;
+                    const index_t i = (index / (2 * weight_w)) % weight_h;
+                    const index_t w = (index / (2 * weight_w * weight_h)) % out_w;
+                    const index_t h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
+                    const index_t g = (index / (2 * weight_w * weight_h * out_w * out_h)) % offset_groups;
+                    const index_t b = index / (2 * weight_w * weight_h * out_w * out_h * offset_groups);
+
+                    scalar_t grad_offset_val = 0;
+
+                    const index_t c_start = g * c_per_offset_group;
+                    const index_t c_end = c_start + c_per_offset_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t mask_group_idx = c / c_per_mask_group;
 
-                    const index_t y = (h * stride_h - pad_h) + i * dilation_h;
-                    const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+                        const index_t y = (h * stride_h - pad_h) + i * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    scalar_t val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
+                        scalar_t weight = coordinate_weight(
                                 input, b, c, height, width,
-                                y + offset[b][offset_group_idx][i][j][0][h][w],
-                                x + offset[b][offset_group_idx][i][j][1][h][w]);
-                    else
-                        val = sample(input, b, c, height, width, y, x);
+                                y + offset[b][g][i][j][0][h][w],
+                                x + offset[b][g][i][j][1][h][w],
+                                o);
+
+                        scalar_t mask_val;
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][j][h][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
+
+                        grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
+                    }
 
-                    grad_mask_val += columns[c][i][j][b][h][w] * val;
+                    grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
                 }
+            }
 
-                grad_mask[b][g][i][j][h][w] = grad_mask_val;
+            void deform_conv2d_compute_grad_offset(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_offset) {
+                if (!deformable) return;
+                const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_h * out_w * weight_h * weight_w * 2;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv2d_compute_grad_offset", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_offset_accessor =
+                                grad_offset.accessor<scalar_t, 7>();
+                        TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                            deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 6>(),
+                                    input.accessor<scalar_t, 4>(),
+                                    offset.accessor<scalar_t, 7>(),
+                                    mask.accessor<scalar_t, 6>(),
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    offset_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_offset_accessor);
+                        }));
+                    }));
+                }));
             }
-        }
 
-        void deform_conv2d_compute_grad_mask_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_mask) {
-            if (!modulated) return;
-            const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_h * out_w * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_mask_accessor =
-                            grad_mask.accessor<scalar_t, 6>();
-                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 6>(),
-                                input.accessor<scalar_t, 4>(),
-                                offset.accessor<scalar_t, 7>(),
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                mask_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_mask_accessor);
+            template<bool deformable, typename scalar_t, typename index_t>
+            static void deform_conv2d_compute_grad_mask_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 6> columns,
+                    const at::TensorAccessor<scalar_t, 4> input,
+                    const at::TensorAccessor<scalar_t, 7> offset,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t mask_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 6> grad_mask) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t j = index % weight_w;
+                    const index_t i = (index / weight_w) % weight_h;
+                    const index_t w = (index / (weight_w * weight_h)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
+                    const index_t g = (index / (weight_w * weight_h * out_w * out_h)) % mask_groups;
+                    const index_t b = index / (out_w * out_h * weight_w * weight_h * mask_groups);
+
+                    scalar_t grad_mask_val = 0;
+
+                    const index_t c_start = g * c_per_mask_group;
+                    const index_t c_end = c_start + c_per_mask_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t offset_group_idx = c / c_per_offset_group;
+
+                        const index_t y = (h * stride_h - pad_h) + i * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+
+                        scalar_t val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, height, width,
+                                    y + offset[b][offset_group_idx][i][j][0][h][w],
+                                    x + offset[b][offset_group_idx][i][j][1][h][w]);
+                        else
+                            val = sample(input, b, c, height, width, y, x);
+
+                        grad_mask_val += columns[c][i][j][b][h][w] * val;
+                    }
+
+                    grad_mask[b][g][i][j][h][w] = grad_mask_val;
+                }
+            }
+
+            void deform_conv2d_compute_grad_mask(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_mask) {
+                if (!modulated) return;
+                const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_h * out_w * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv2d_compute_grad_mask", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_mask_accessor =
+                                grad_mask.accessor<scalar_t, 6>();
+                        TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                            deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 6>(),
+                                    input.accessor<scalar_t, 4>(),
+                                    offset.accessor<scalar_t, 7>(),
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    mask_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_mask_accessor);
+                        }));
                     }));
                 }));
-            }));
+            }
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/cpu/deform_conv3d_kernels_cpu.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv3d_common_kernels.cpp`

 * *Files 1% similar despite different names*

```diff
@@ -1,762 +1,765 @@
 #include <ATen/ATen.h>
 
 #include "cpu_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
-        namespace {
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t sample(
-                    const at::TensorAccessor<scalar_t, 5> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const index_t z,
-                    const index_t y,
-                    const index_t x) {
-                return (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width) ?
-                       input[b][c][z][y][x] : static_cast<scalar_t>(0);
-            }
+        namespace cpu {
+            namespace {
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t sample(
+                        const at::TensorAccessor<scalar_t, 5> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const index_t z,
+                        const index_t y,
+                        const index_t x) {
+                    return (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width) ?
+                           input[b][c][z][y][x] : static_cast<scalar_t>(0);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t interpolate_sample(
-                    const at::TensorAccessor<scalar_t, 5> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t z,
-                    const scalar_t y,
-                    const scalar_t x) {
-                if (z <= -1 || depth <= z || y <= -1 || height <= y || x <= -1 || width <= x)
-                    return 0;
-
-                index_t z_l = floor(z);
-                index_t z_h = z_l + 1;
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dz_h = z - z_l;
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dz_l = 1 - dz_h;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_z_l = z_l >= 0;
-                bool valid_z_h = z_h < depth;
-                bool valid_y_l = y_l >= 0;
-                bool valid_y_h = y_h < height;
-                bool valid_x_l = x_l >= 0;
-                bool valid_x_h = x_h < width;
-
-                scalar_t val = 0;
-                if (valid_z_l && valid_y_l && valid_x_l)
-                    val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
-                if (valid_z_l && valid_y_l && valid_x_h)
-                    val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
-                if (valid_z_l && valid_y_h && valid_x_l)
-                    val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
-                if (valid_z_l && valid_y_h && valid_x_h)
-                    val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
-                if (valid_z_h && valid_y_l && valid_x_l)
-                    val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
-                if (valid_z_h && valid_y_l && valid_x_h)
-                    val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
-                if (valid_z_h && valid_y_h && valid_x_l)
-                    val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
-                if (valid_z_h && valid_y_h && valid_x_h)
-                    val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
-                return val;
-            }
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t interpolate_sample(
+                        const at::TensorAccessor<scalar_t, 5> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t z,
+                        const scalar_t y,
+                        const scalar_t x) {
+                    if (z <= -1 || depth <= z || y <= -1 || height <= y || x <= -1 || width <= x)
+                        return 0;
+
+                    index_t z_l = floor(z);
+                    index_t z_h = z_l + 1;
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dz_h = z - z_l;
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dz_l = 1 - dz_h;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_z_l = z_l >= 0;
+                    bool valid_z_h = z_h < depth;
+                    bool valid_y_l = y_l >= 0;
+                    bool valid_y_h = y_h < height;
+                    bool valid_x_l = x_l >= 0;
+                    bool valid_x_h = x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_z_l && valid_y_l && valid_x_l)
+                        val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
+                    if (valid_z_l && valid_y_l && valid_x_h)
+                        val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
+                    if (valid_z_l && valid_y_h && valid_x_l)
+                        val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
+                    if (valid_z_l && valid_y_h && valid_x_h)
+                        val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
+                    if (valid_z_h && valid_y_l && valid_x_l)
+                        val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
+                    if (valid_z_h && valid_y_l && valid_x_h)
+                        val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
+                    if (valid_z_h && valid_y_h && valid_x_l)
+                        val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
+                    if (valid_z_h && valid_y_h && valid_x_h)
+                        val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
+                    return val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ void insert(
-                    at::TensorAccessor<scalar_t, 5> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const index_t z,
-                    const index_t y,
-                    const index_t x,
-                    const scalar_t val) {
-                if (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width)
-                    output[b][c][z][y][x] += val;
-            }
+                template<typename scalar_t, typename index_t>
+                __forceinline__ void insert(
+                        at::TensorAccessor<scalar_t, 5> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const index_t z,
+                        const index_t y,
+                        const index_t x,
+                        const scalar_t val) {
+                    if (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width)
+                        output[b][c][z][y][x] += val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ void interpolate_insert(
-                    at::TensorAccessor<scalar_t, 5> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t z,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const scalar_t val) {
-                index_t z_l = floor(z);
-                index_t z_h = z_l + 1;
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dz_h = z - z_l;
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dz_l = 1 - dz_h;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_z_l = 0 <= z_l && z_l < depth;
-                bool valid_z_h = 0 <= z_h && z_h < depth;
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                if (valid_z_l && valid_y_l && valid_x_l)
-                    output[b][c][z_l][y_l][x_l] += dz_l * dy_l * dx_l * val;
-                if (valid_z_l && valid_y_l && valid_x_h)
-                    output[b][c][z_l][y_l][x_h] += dz_l * dy_l * dx_h * val;
-                if (valid_z_l && valid_y_h && valid_x_l)
-                    output[b][c][z_l][y_h][x_l] += dz_l * dy_h * dx_l * val;
-                if (valid_z_l && valid_y_h && valid_x_h)
-                    output[b][c][z_l][y_h][x_h] += dz_l * dy_h * dx_h * val;
-                if (valid_z_h && valid_y_l && valid_x_l)
-                    output[b][c][z_h][y_l][x_l] += dz_h * dy_l * dx_l * val;
-                if (valid_z_h && valid_y_l && valid_x_h)
-                    output[b][c][z_h][y_l][x_h] += dz_h * dy_l * dx_h * val;
-                if (valid_z_h && valid_y_h && valid_x_l)
-                    output[b][c][z_h][y_h][x_l] += dz_h * dy_h * dx_l * val;
-                if (valid_z_h && valid_y_h && valid_x_h)
-                    output[b][c][z_h][y_h][x_h] += dz_h * dy_h * dx_h * val;
+                template<typename scalar_t, typename index_t>
+                __forceinline__ void interpolate_insert(
+                        at::TensorAccessor<scalar_t, 5> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t z,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const scalar_t val) {
+                    index_t z_l = floor(z);
+                    index_t z_h = z_l + 1;
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dz_h = z - z_l;
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dz_l = 1 - dz_h;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_z_l = 0 <= z_l && z_l < depth;
+                    bool valid_z_h = 0 <= z_h && z_h < depth;
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    if (valid_z_l && valid_y_l && valid_x_l)
+                        output[b][c][z_l][y_l][x_l] += dz_l * dy_l * dx_l * val;
+                    if (valid_z_l && valid_y_l && valid_x_h)
+                        output[b][c][z_l][y_l][x_h] += dz_l * dy_l * dx_h * val;
+                    if (valid_z_l && valid_y_h && valid_x_l)
+                        output[b][c][z_l][y_h][x_l] += dz_l * dy_h * dx_l * val;
+                    if (valid_z_l && valid_y_h && valid_x_h)
+                        output[b][c][z_l][y_h][x_h] += dz_l * dy_h * dx_h * val;
+                    if (valid_z_h && valid_y_l && valid_x_l)
+                        output[b][c][z_h][y_l][x_l] += dz_h * dy_l * dx_l * val;
+                    if (valid_z_h && valid_y_l && valid_x_h)
+                        output[b][c][z_h][y_l][x_h] += dz_h * dy_l * dx_h * val;
+                    if (valid_z_h && valid_y_h && valid_x_l)
+                        output[b][c][z_h][y_h][x_l] += dz_h * dy_h * dx_l * val;
+                    if (valid_z_h && valid_y_h && valid_x_h)
+                        output[b][c][z_h][y_h][x_h] += dz_h * dy_h * dx_h * val;
+                }
+
+                template<typename scalar_t, typename index_t>
+                __forceinline__ scalar_t coordinate_weight(
+                        const at::TensorAccessor<scalar_t, 5> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t z,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const index_t direction) {
+                    index_t z_l = floor(z);
+                    index_t z_h = z_l + 1;
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dz_h = (direction == 0) ? static_cast<scalar_t>(1) : z - z_l;
+                    scalar_t dy_h = (direction == 1) ? static_cast<scalar_t>(1) : y - y_l;
+                    scalar_t dx_h = (direction == 2) ? static_cast<scalar_t>(1) : x - x_l;
+                    scalar_t dz_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dz_h;
+                    scalar_t dy_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dy_h;
+                    scalar_t dx_l = (direction == 2) ? static_cast<scalar_t>(-1) : 1 - dx_h;
+
+                    bool valid_z_l = 0 <= z_l && z_l < depth;
+                    bool valid_z_h = 0 <= z_h && z_h < depth;
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_z_l && valid_y_l && valid_x_l)
+                        val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
+                    if (valid_z_l && valid_y_l && valid_x_h)
+                        val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
+                    if (valid_z_l && valid_y_h && valid_x_l)
+                        val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
+                    if (valid_z_l && valid_y_h && valid_x_h)
+                        val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
+                    if (valid_z_h && valid_y_l && valid_x_l)
+                        val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
+                    if (valid_z_h && valid_y_l && valid_x_h)
+                        val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
+                    if (valid_z_h && valid_y_h && valid_x_l)
+                        val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
+                    if (valid_z_h && valid_y_h && valid_x_h)
+                        val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
+                    return val;
+                }
             }
 
-            template<typename scalar_t, typename index_t>
-            __forceinline__ scalar_t coordinate_weight(
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static void vol2col_kernel(
+                    const index_t n_kernels,
                     const at::TensorAccessor<scalar_t, 5> input,
-                    const index_t b,
-                    const index_t c,
+                    const at::TensorAccessor<scalar_t, 9> offset,
+                    const at::TensorAccessor<scalar_t, 8> mask,
                     const index_t depth,
                     const index_t height,
                     const index_t width,
-                    const scalar_t z,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const index_t direction) {
-                index_t z_l = floor(z);
-                index_t z_h = z_l + 1;
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dz_h = (direction == 0) ? static_cast<scalar_t>(1) : z - z_l;
-                scalar_t dy_h = (direction == 1) ? static_cast<scalar_t>(1) : y - y_l;
-                scalar_t dx_h = (direction == 2) ? static_cast<scalar_t>(1) : x - x_l;
-                scalar_t dz_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dz_h;
-                scalar_t dy_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dy_h;
-                scalar_t dx_l = (direction == 2) ? static_cast<scalar_t>(-1) : 1 - dx_h;
-
-                bool valid_z_l = 0 <= z_l && z_l < depth;
-                bool valid_z_h = 0 <= z_h && z_h < depth;
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                scalar_t val = 0;
-                if (valid_z_l && valid_y_l && valid_x_l)
-                    val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
-                if (valid_z_l && valid_y_l && valid_x_h)
-                    val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
-                if (valid_z_l && valid_y_h && valid_x_l)
-                    val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
-                if (valid_z_l && valid_y_h && valid_x_h)
-                    val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
-                if (valid_z_h && valid_y_l && valid_x_l)
-                    val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
-                if (valid_z_h && valid_y_l && valid_x_h)
-                    val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
-                if (valid_z_h && valid_y_h && valid_x_l)
-                    val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
-                if (valid_z_h && valid_y_h && valid_x_h)
-                    val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
-                return val;
-            }
-        }
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t in_channels,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 8> columns) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t w = index % out_w;
+                    const index_t h = (index / out_w) % out_h;
+                    const index_t d = (index / (out_w * out_h)) % out_d;
+                    const index_t c = (index / (out_w * out_h * out_d)) % in_channels;
+                    const index_t b = index / (out_w * out_h * out_d * in_channels);
 
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void vol2col_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 5> input,
-                const at::TensorAccessor<scalar_t, 9> offset,
-                const at::TensorAccessor<scalar_t, 8> mask,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t in_channels,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 8> columns) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t w = index % out_w;
-                const index_t h = (index / out_w) % out_h;
-                const index_t d = (index / (out_w * out_h)) % out_d;
-                const index_t c = (index / (out_w * out_h * out_d)) % in_channels;
-                const index_t b = index / (out_w * out_h * out_d * in_channels);
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                for (index_t i = 0; i < weight_d; ++i) {
-                    for (index_t j = 0; j < weight_h; ++j) {
-                        for (index_t k = 0; k < weight_w; ++k) {
-                            const index_t z = (d * stride_d - pad_d) + i * dilation_d;
-                            const index_t y = (h * stride_h - pad_h) + j * dilation_h;
-                            const index_t x = (w * stride_w - pad_w) + k * dilation_w;
-
-                            scalar_t val, mask_val;
-                            if constexpr (deformable)
-                                val = interpolate_sample(
-                                        input, b, c, depth, height, width,
-                                        z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                        y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                        x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
-                            else
-                                val = sample(input, b, c, depth, height, width, z, y, x);
-
-                            if constexpr (modulated)
-                                mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
-                            else
-                                mask_val = static_cast<scalar_t>(1);
+                    const index_t offset_group_idx = c / c_per_offset_group;
+                    const index_t mask_group_idx = c / c_per_mask_group;
+
+                    for (index_t i = 0; i < weight_d; ++i) {
+                        for (index_t j = 0; j < weight_h; ++j) {
+                            for (index_t k = 0; k < weight_w; ++k) {
+                                const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                                const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                                const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+
+                                scalar_t val, mask_val;
+                                if constexpr (deformable)
+                                    val = interpolate_sample(
+                                            input, b, c, depth, height, width,
+                                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                                else
+                                    val = sample(input, b, c, depth, height, width, z, y, x);
+
+                                if constexpr (modulated)
+                                    mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                                else
+                                    mask_val = static_cast<scalar_t>(1);
 
-                            columns[c][i][j][k][b][d][h][w] = val * mask_val;
+                                columns[c][i][j][k][b][d][h][w] = val * mask_val;
+                            }
                         }
                     }
                 }
             }
-        }
 
-        void vol2col_cpu(
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &columns) {
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "vol2col_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto columns_accessor =
-                            columns.accessor<scalar_t, 8>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        vol2col_kernel<deformable, modulated, scalar_t, index_t>(
-                                n_kernels,
-                                input.accessor<scalar_t, 5>(),
-                                offset.accessor<scalar_t, 9>(),
-                                mask.accessor<scalar_t, 8>(),
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                in_channels,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                columns_accessor);
+            void vol2col(
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &columns) {
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        input.scalar_type(), "vol2col", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto columns_accessor =
+                                columns.accessor<scalar_t, 8>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            vol2col_kernel<deformable, modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    input.accessor<scalar_t, 5>(),
+                                    offset.accessor<scalar_t, 9>(),
+                                    mask.accessor<scalar_t, 8>(),
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    in_channels,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    columns_accessor);
+                        }));
                     }));
                 }));
-            }));
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static void col2vol_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 8> columns,
-                const at::TensorAccessor<scalar_t, 9> offset,
-                const at::TensorAccessor<scalar_t, 8> mask,
-                const index_t in_channels,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 5> grad_input) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t k = index % weight_w;
-                const index_t j = (index / weight_w) % weight_h;
-                const index_t i = (index / (weight_w * weight_h)) % weight_d;
-                const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
-                const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
-                const index_t c = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % in_channels;
-                const index_t b = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * in_channels));
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                const index_t z = (d * stride_d - pad_d) + i * dilation_d;
-                const index_t y = (h * stride_h - pad_h) + j * dilation_h;
-                const index_t x = (w * stride_w - pad_w) + k * dilation_w;
-
-                scalar_t mask_val;
-                if constexpr (modulated)
-                    mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
-                else
-                    mask_val = static_cast<scalar_t>(1);
-
-                scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
-
-                if constexpr (deformable)
-                    interpolate_insert(
-                            grad_input, b, c, depth, height, width,
-                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
-                            val);
-                else
-                    insert(grad_input, b, c, depth, height, width, z, y, x, val);
             }
-        }
 
-        void col2vol_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_input) {
-            const int64_t n_kernels =
-                    (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2vol_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
-                    auto grad_input_accessor =
-                            grad_input.accessor<scalar_t, 5>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2vol_kernel<deformable, modulated, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 8>(),
-                                offset.accessor<scalar_t, 9>(),
-                                mask.accessor<scalar_t, 8>(),
-                                in_channels,
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_input_accessor);
-                    }));
-                }));
-            }));
-        }
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static void col2vol_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 8> columns,
+                    const at::TensorAccessor<scalar_t, 9> offset,
+                    const at::TensorAccessor<scalar_t, 8> mask,
+                    const index_t in_channels,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 5> grad_input) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t k = index % weight_w;
+                    const index_t j = (index / weight_w) % weight_h;
+                    const index_t i = (index / (weight_w * weight_h)) % weight_d;
+                    const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
+                    const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                    const index_t c = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % in_channels;
+                    const index_t b = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * in_channels));
 
-        template<bool modulated, typename scalar_t, typename index_t>
-        static void deform_conv3d_compute_grad_offset_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 8> columns,
-                const at::TensorAccessor<scalar_t, 5> input,
-                const at::TensorAccessor<scalar_t, 9> offset,
-                const at::TensorAccessor<scalar_t, 8> mask,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t offset_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 9> grad_offset) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t o = index % 3;
-                const index_t k = (index / 3) % weight_w;
-                const index_t j = (index / (3 * weight_w)) % weight_h;
-                const index_t i = (index / (3 * weight_w * weight_h)) % weight_d;
-                const index_t w = (index / (3 * weight_w * weight_h * weight_d)) % out_w;
-                const index_t h = (index / (3 * weight_w * weight_h * weight_d * out_w)) % out_h;
-                const index_t d = (index / (3 * weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
-                const index_t g =
-                        (index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d)) % offset_groups;
-                const index_t b = index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d * offset_groups);
-
-                scalar_t grad_offset_val = 0;
-
-                const index_t c_start = g * c_per_offset_group;
-                const index_t c_end = c_start + c_per_offset_group;
-                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                     const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    scalar_t weight =
-                            coordinate_weight(
-                                    input, b, c, depth, height, width,
-                                    z + offset[b][g][i][j][k][0][d][h][w],
-                                    y + offset[b][g][i][j][k][1][d][h][w],
-                                    x + offset[b][g][i][j][k][2][d][h][w],
-                                    o);
-
                     scalar_t mask_val;
                     if constexpr (modulated)
                         mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
                     else
                         mask_val = static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
-                }
+                    scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
 
-                grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
+                    if constexpr (deformable)
+                        interpolate_insert(
+                                grad_input, b, c, depth, height, width,
+                                z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
+                                val);
+                    else
+                        insert(grad_input, b, c, depth, height, width, z, y, x, val);
+                }
             }
-        }
 
-        void deform_conv3d_compute_grad_offset_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_offset) {
-            if (!deformable) return;
-            const int64_t n_kernels =
-                    (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv3d_compute_grad_offset_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_offset_accessor =
-                            grad_offset.accessor<scalar_t, 9>();
-                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv3d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 8>(),
-                                input.accessor<scalar_t, 5>(),
-                                offset.accessor<scalar_t, 9>(),
-                                mask.accessor<scalar_t, 8>(),
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                offset_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_offset_accessor);
+            void col2vol(
+                    const at::Tensor &columns,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_input) {
+                const int64_t n_kernels =
+                        (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "col2vol", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                        auto grad_input_accessor =
+                                grad_input.accessor<scalar_t, 5>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            col2vol_kernel<deformable, modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 8>(),
+                                    offset.accessor<scalar_t, 9>(),
+                                    mask.accessor<scalar_t, 8>(),
+                                    in_channels,
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_input_accessor);
+                        }));
                     }));
                 }));
-            }));
-        }
+            }
 
-        template<bool deformable, typename scalar_t, typename index_t>
-        static void deform_conv3d_compute_grad_mask_kernel(
-                const index_t n_kernels,
-                const at::TensorAccessor<scalar_t, 8> columns,
-                const at::TensorAccessor<scalar_t, 5> input,
-                const at::TensorAccessor<scalar_t, 9> offset,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t mask_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::TensorAccessor<scalar_t, 8> grad_mask) {
-            CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t k = index % weight_w;
-                const index_t j = (index / weight_w) % weight_h;
-                const index_t i = (index / (weight_w * weight_h)) % weight_d;
-                const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
-                const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
-                const index_t g = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % mask_groups;
-                const index_t b = index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * mask_groups);
-
-                scalar_t grad_mask_val = 0;
-
-                const index_t c_start = g * c_per_mask_group;
-                const index_t c_end = c_start + c_per_mask_group;
-                for (index_t c = c_start; c < c_end; ++c) {
-                    const index_t offset_group_idx = c / c_per_offset_group;
+            template<bool modulated, typename scalar_t, typename index_t>
+            static void deform_conv3d_compute_grad_offset_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 8> columns,
+                    const at::TensorAccessor<scalar_t, 5> input,
+                    const at::TensorAccessor<scalar_t, 9> offset,
+                    const at::TensorAccessor<scalar_t, 8> mask,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t offset_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 9> grad_offset) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t o = index % 3;
+                    const index_t k = (index / 3) % weight_w;
+                    const index_t j = (index / (3 * weight_w)) % weight_h;
+                    const index_t i = (index / (3 * weight_w * weight_h)) % weight_d;
+                    const index_t w = (index / (3 * weight_w * weight_h * weight_d)) % out_w;
+                    const index_t h = (index / (3 * weight_w * weight_h * weight_d * out_w)) % out_h;
+                    const index_t d = (index / (3 * weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                    const index_t g =
+                            (index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d)) % offset_groups;
+                    const index_t b =
+                            index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d * offset_groups);
+
+                    scalar_t grad_offset_val = 0;
+
+                    const index_t c_start = g * c_per_offset_group;
+                    const index_t c_end = c_start + c_per_offset_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t mask_group_idx = c / c_per_mask_group;
+
+                        const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                        const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    const index_t z = (d * stride_d - pad_d) + i * dilation_d;
-                    const index_t y = (h * stride_h - pad_h) + j * dilation_h;
-                    const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+                        scalar_t weight =
+                                coordinate_weight(
+                                        input, b, c, depth, height, width,
+                                        z + offset[b][g][i][j][k][0][d][h][w],
+                                        y + offset[b][g][i][j][k][1][d][h][w],
+                                        x + offset[b][g][i][j][k][2][d][h][w],
+                                        o);
+
+                        scalar_t mask_val;
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
 
-                    scalar_t val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
-                                input, b, c, depth, height, width,
-                                z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
-                    else
-                        val = sample(input, b, c, depth, height, width, z, y, x);
+                        grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
+                    }
 
-                    grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
+                    grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
                 }
+            }
 
-                grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
+            void deform_conv3d_compute_grad_offset(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_offset) {
+                if (!deformable) return;
+                const int64_t n_kernels =
+                        (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv3d_compute_grad_offset", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_offset_accessor =
+                                grad_offset.accessor<scalar_t, 9>();
+                        TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                            deform_conv3d_compute_grad_offset_kernel<modulated, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 8>(),
+                                    input.accessor<scalar_t, 5>(),
+                                    offset.accessor<scalar_t, 9>(),
+                                    mask.accessor<scalar_t, 8>(),
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    offset_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_offset_accessor);
+                        }));
+                    }));
+                }));
             }
-        }
 
-        void deform_conv3d_compute_grad_mask_cpu(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_mask) {
-            if (!modulated) return;
-            const int64_t n_kernels =
-                    (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv3d_compute_grad_mask_cpu", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_mask_accessor =
-                            grad_mask.accessor<scalar_t, 8>();
-                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv3d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
-                                n_kernels,
-                                columns.accessor<scalar_t, 8>(),
-                                input.accessor<scalar_t, 5>(),
-                                offset.accessor<scalar_t, 9>(),
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                mask_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_mask_accessor);
+            template<bool deformable, typename scalar_t, typename index_t>
+            static void deform_conv3d_compute_grad_mask_kernel(
+                    const index_t n_kernels,
+                    const at::TensorAccessor<scalar_t, 8> columns,
+                    const at::TensorAccessor<scalar_t, 5> input,
+                    const at::TensorAccessor<scalar_t, 9> offset,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t mask_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::TensorAccessor<scalar_t, 8> grad_mask) {
+                CPU_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t k = index % weight_w;
+                    const index_t j = (index / weight_w) % weight_h;
+                    const index_t i = (index / (weight_w * weight_h)) % weight_d;
+                    const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
+                    const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                    const index_t g = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % mask_groups;
+                    const index_t b = index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * mask_groups);
+
+                    scalar_t grad_mask_val = 0;
+
+                    const index_t c_start = g * c_per_mask_group;
+                    const index_t c_end = c_start + c_per_mask_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t offset_group_idx = c / c_per_offset_group;
+
+                        const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                        const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+
+                        scalar_t val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, depth, height, width,
+                                    z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                    y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                    x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                        else
+                            val = sample(input, b, c, depth, height, width, z, y, x);
+
+                        grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
+                    }
+
+                    grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
+                }
+            }
+
+            void deform_conv3d_compute_grad_mask(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_mask) {
+                if (!modulated) return;
+                const int64_t n_kernels =
+                        (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv3d_compute_grad_mask", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_mask_accessor =
+                                grad_mask.accessor<scalar_t, 8>();
+                        TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                            deform_conv3d_compute_grad_mask_kernel<deformable, scalar_t, index_t>(
+                                    n_kernels,
+                                    columns.accessor<scalar_t, 8>(),
+                                    input.accessor<scalar_t, 5>(),
+                                    offset.accessor<scalar_t, 9>(),
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    mask_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_mask_accessor);
+                        }));
                     }));
                 }));
-            }));
+            }
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv1d_kernels_cuda.cu` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_common_kernels.cu`

 * *Files 0% similar despite different names*

```diff
@@ -1,499 +1,501 @@
 #include <ATen/ATen.h>
 
 #include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
-        namespace {
-            constexpr float threadsFraction = 1.0;
+        namespace cuda {
+            namespace {
+                constexpr float threadsFraction = 1.0;
+
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t sample(
+                        const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const index_t x) {
+                    return (0 <= x && x < width) ? input[b][c][x] : static_cast<scalar_t>(0);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const index_t x) {
-                return (0 <= x && x < width) ? input[b][c][x] : static_cast<scalar_t>(0);
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t interpolate_sample(
+                        const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const scalar_t x) {
+                    if (x <= -1 || width <= x)
+                        return 0;
+
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_x_l = x_l >= 0;
+                    bool valid_x_h = x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_x_l) val += dx_l * input[b][c][x_l];
+                    if (valid_x_h) val += dx_h * input[b][c][x_h];
+                    return val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t interpolate_sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const scalar_t x) {
-                if (x <= -1 || width <= x)
-                    return 0;
-
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dx_h = x - x_l;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_x_l = x_l >= 0;
-                bool valid_x_h = x_h < width;
-
-                scalar_t val = 0;
-                if (valid_x_l) val += dx_l * input[b][c][x_l];
-                if (valid_x_h) val += dx_h * input[b][c][x_h];
-                return val;
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ void insert(
+                        at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const index_t x,
+                        const scalar_t val) {
+                    if (0 <= x && x < width)
+                        gpuAtomicAdd(&output[b][c][x], val);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const index_t x,
-                    const scalar_t val) {
-                if (0 <= x && x < width)
-                    gpuAtomicAdd(&output[b][c][x], val);
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ void interpolate_insert(
+                        at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const scalar_t x,
+                        const scalar_t val) {
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void interpolate_insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t width,
-                    const scalar_t x,
-                    const scalar_t val) {
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dx_l = 1 - dx_h;
 
-                scalar_t dx_h = x - x_l;
-                scalar_t dx_l = 1 - dx_h;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
 
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
+                    if (valid_x_l) gpuAtomicAdd(&output[b][c][x_l], dx_l * val);
+                    if (valid_x_h) gpuAtomicAdd(&output[b][c][x_h], dx_h * val);
+                }
 
-                if (valid_x_l) gpuAtomicAdd(&output[b][c][x_l], dx_l * val);
-                if (valid_x_h) gpuAtomicAdd(&output[b][c][x_h], dx_h * val);
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t coordinate_weight(
+                        const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t width,
+                        const scalar_t x) {
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dx_h = 1;
+                    scalar_t dx_l = -1;
+
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_x_l) val += dx_l * input[b][c][x_l];
+                    if (valid_x_h) val += dx_h * input[b][c][x_h];
+                    return val;
+                }
             }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t coordinate_weight(
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void arr2col_kernel(
+                    const index_t n_kernels,
                     const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
+                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> mask,
                     const index_t width,
-                    const scalar_t x) {
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dx_h = 1;
-                scalar_t dx_l = -1;
-
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                scalar_t val = 0;
-                if (valid_x_l) val += dx_l * input[b][c][x_l];
-                if (valid_x_h) val += dx_h * input[b][c][x_h];
-                return val;
-            }
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void arr2col_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> mask,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t in_channels,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t w = index % out_w;
-                const index_t c = (index / out_w) % in_channels;
-                const index_t b = index / (out_w * in_channels);
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t in_channels,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t w = index % out_w;
+                    const index_t c = (index / out_w) % in_channels;
+                    const index_t b = index / (out_w * in_channels);
 
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                for (index_t i = 0; i < weight_w; ++i) {
-                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
+                    const index_t offset_group_idx = c / c_per_offset_group;
+                    const index_t mask_group_idx = c / c_per_mask_group;
 
-                    scalar_t val, mask_val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
-                                input, b, c, width,
-                                x + offset[b][offset_group_idx][i][0][w]);
-                    else
-                        val = sample(input, b, c, width, x);
+                    for (index_t i = 0; i < weight_w; ++i) {
+                        const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    if constexpr (modulated)
-                        mask_val = mask[b][mask_group_idx][i][w];
-                    else
-                        mask_val = static_cast<scalar_t>(1);
+                        scalar_t val, mask_val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, width,
+                                    x + offset[b][offset_group_idx][i][0][w]);
+                        else
+                            val = sample(input, b, c, width, x);
+
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
 
-                    columns[c][i][b][w] = val * mask_val;
+                        columns[c][i][b][w] = val * mask_val;
+                    }
                 }
             }
-        }
 
-        void arr2col_cuda(
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &columns) {
-            at::cuda::CUDAGuard device_guard(input.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "arr2col_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto columns_accessor =
-                            columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        arr2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                in_channels,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                columns_accessor);
+            void arr2col(
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &columns) {
+                at::cuda::CUDAGuard device_guard(input.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        input.scalar_type(), "arr2col", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto columns_accessor =
+                                columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            arr2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    in_channels,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    columns_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void col2arr_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> mask,
-                const index_t in_channels,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> grad_input) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t i = index % weight_w;
-                const index_t w = (index / weight_w) % out_w;
-                const index_t c = (index / (weight_w * out_w)) % in_channels;
-                const index_t b = (index / (weight_w * out_w * in_channels));
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                const index_t x = (w * stride_w - pad_w) + i * dilation_w;
-
-                scalar_t mask_val;
-                if constexpr (modulated)
-                    mask_val = mask[b][mask_group_idx][i][w];
-                else
-                    mask_val = static_cast<scalar_t>(1);
-
-                scalar_t val = columns[c][i][b][w] * mask_val;
-
-                if constexpr (deformable)
-                    interpolate_insert(
-                            grad_input, b, c, width,
-                            x + offset[b][offset_group_idx][i][0][w],
-                            val);
-                else
-                    insert(grad_input, b, c, width, x, val);
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
             }
-        }
 
-        void col2arr_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_input) {
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2arr_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
-                    auto grad_input_accessor =
-                            grad_input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2arr_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                in_channels,
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_input_accessor);
-                    }));
-                }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void col2arr_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> mask,
+                    const index_t in_channels,
+                    const index_t width,
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> grad_input) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t i = index % weight_w;
+                    const index_t w = (index / weight_w) % out_w;
+                    const index_t c = (index / (weight_w * out_w)) % in_channels;
+                    const index_t b = (index / (weight_w * out_w * in_channels));
 
-        template<bool modulated, typename scalar_t, typename index_t>
-        static __global__ void deform_conv1d_compute_grad_offset_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> mask,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t offset_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> grad_offset) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t i = index % weight_w;
-                const index_t w = (index / weight_w) % out_w;
-                const index_t g = (index / (weight_w * out_w)) % offset_groups;
-                const index_t b = index / (weight_w * out_w * offset_groups);
-
-                scalar_t grad_offset_val = 0;
-
-                const index_t c_start = g * c_per_offset_group;
-                const index_t c_end = c_start + c_per_offset_group;
-                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    scalar_t weight = coordinate_weight(
-                            input, b, c, width,
-                            x + offset[b][g][i][0][w]);
-
                     scalar_t mask_val;
                     if constexpr (modulated)
                         mask_val = mask[b][mask_group_idx][i][w];
                     else
                         mask_val = static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][b][w] * weight * mask_val;
-                }
+                    scalar_t val = columns[c][i][b][w] * mask_val;
 
-                grad_offset[b][g][i][0][w] = grad_offset_val;
+                    if constexpr (deformable)
+                        interpolate_insert(
+                                grad_input, b, c, width,
+                                x + offset[b][offset_group_idx][i][0][w],
+                                val);
+                    else
+                        insert(grad_input, b, c, width, x, val);
+                }
             }
-        }
 
-        void deform_conv1d_compute_grad_offset_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_offset) {
-            if (!deformable) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv1d_compute_grad_offset_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_offset_accessor =
-                            grad_offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv1d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                offset_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_offset_accessor);
+            void col2arr(
+                    const at::Tensor &columns,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_input) {
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_w * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "col2arr", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                        auto grad_input_accessor =
+                                grad_input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            col2arr_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    in_channels,
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_input_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
+            }
 
-        template<bool deformable, typename scalar_t, typename index_t>
-        static __global__ void deform_conv1d_compute_grad_mask_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
-                const index_t width,
-                const index_t weight_w,
-                const index_t stride_w,
-                const index_t pad_w,
-                const index_t dilation_w,
-                const index_t out_w,
-                const index_t mask_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> grad_mask) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t i = index % weight_w;
-                const index_t w = (index / weight_w) % out_w;
-                const index_t g = (index / (weight_w * out_w)) % mask_groups;
-                const index_t b = index / (out_w * weight_w * mask_groups);
-
-                scalar_t grad_mask_val = 0;
-
-                const index_t c_start = g * c_per_mask_group;
-                const index_t c_end = c_start + c_per_mask_group;
-                for (index_t c = c_start; c < c_end; ++c) {
-                    const index_t offset_group_idx = c / c_per_offset_group;
+            template<bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void deform_conv1d_compute_grad_offset_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
+                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> mask,
+                    const index_t width,
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t offset_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> grad_offset) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t i = index % weight_w;
+                    const index_t w = (index / weight_w) % out_w;
+                    const index_t g = (index / (weight_w * out_w)) % offset_groups;
+                    const index_t b = index / (weight_w * out_w * offset_groups);
+
+                    scalar_t grad_offset_val = 0;
+
+                    const index_t c_start = g * c_per_offset_group;
+                    const index_t c_end = c_start + c_per_offset_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t mask_group_idx = c / c_per_mask_group;
 
-                    const index_t x = (w * stride_w - pad_w) + i * dilation_w;
+                        const index_t x = (w * stride_w - pad_w) + i * dilation_w;
 
-                    scalar_t val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
+                        scalar_t weight = coordinate_weight(
                                 input, b, c, width,
-                                x + offset[b][offset_group_idx][i][0][w]);
-                    else
-                        val = sample(input, b, c, width, x);
+                                x + offset[b][g][i][0][w]);
+
+                        scalar_t mask_val;
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
+
+                        grad_offset_val += columns[c][i][b][w] * weight * mask_val;
+                    }
 
-                    grad_mask_val += columns[c][i][b][w] * val;
+                    grad_offset[b][g][i][0][w] = grad_offset_val;
                 }
+            }
 
-                grad_mask[b][g][i][w] = grad_mask_val;
+            void deform_conv1d_compute_grad_offset(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_offset) {
+                if (!deformable) return;
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_w * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv1d_compute_grad_offset", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_offset_accessor =
+                                grad_offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                            deform_conv1d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    offset_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_offset_accessor);
+                        }));
+                    }));
+                }));
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
             }
-        }
 
-        void deform_conv1d_compute_grad_mask_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const int64_t in_channels,
-                const int64_t width,
-                const int64_t weight_w,
-                const int64_t stride_w,
-                const int64_t pad_w,
-                const int64_t dilation_w,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_mask) {
-            if (!modulated) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv1d_compute_grad_mask_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_mask_accessor =
-                            grad_mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv1d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                width,
-                                weight_w,
-                                stride_w,
-                                pad_w,
-                                dilation_w,
-                                out_w,
-                                mask_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_mask_accessor);
+            template<bool deformable, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void deform_conv1d_compute_grad_mask_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 3, at::RestrictPtrTraits, index_t> input,
+                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> offset,
+                    const index_t width,
+                    const index_t weight_w,
+                    const index_t stride_w,
+                    const index_t pad_w,
+                    const index_t dilation_w,
+                    const index_t out_w,
+                    const index_t mask_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> grad_mask) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t i = index % weight_w;
+                    const index_t w = (index / weight_w) % out_w;
+                    const index_t g = (index / (weight_w * out_w)) % mask_groups;
+                    const index_t b = index / (out_w * weight_w * mask_groups);
+
+                    scalar_t grad_mask_val = 0;
+
+                    const index_t c_start = g * c_per_mask_group;
+                    const index_t c_end = c_start + c_per_mask_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t offset_group_idx = c / c_per_offset_group;
+
+                        const index_t x = (w * stride_w - pad_w) + i * dilation_w;
+
+                        scalar_t val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, width,
+                                    x + offset[b][offset_group_idx][i][0][w]);
+                        else
+                            val = sample(input, b, c, width, x);
+
+                        grad_mask_val += columns[c][i][b][w] * val;
+                    }
+
+                    grad_mask[b][g][i][w] = grad_mask_val;
+                }
+            }
+
+            void deform_conv1d_compute_grad_mask(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const int64_t in_channels,
+                    const int64_t width,
+                    const int64_t weight_w,
+                    const int64_t stride_w,
+                    const int64_t pad_w,
+                    const int64_t dilation_w,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_mask) {
+                if (!modulated) return;
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_w * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv1d_compute_grad_mask", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_mask_accessor =
+                                grad_mask.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                            deform_conv1d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    input.generic_packed_accessor<scalar_t, 3, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    width,
+                                    weight_w,
+                                    stride_w,
+                                    pad_w,
+                                    dilation_w,
+                                    out_w,
+                                    mask_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_mask_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
+            }
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv2d_kernels_cuda.cu` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_common_kernels.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,625 +1,627 @@
 #include <ATen/ATen.h>
 
 #include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
-        namespace {
-            constexpr float threadsFraction = 0.75;
+        namespace cuda {
+            namespace {
+                constexpr float threadsFraction = 0.75;
+
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t sample(
+                        const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const index_t y,
+                        const index_t x) {
+                    return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const index_t y,
-                    const index_t x) {
-                return (0 <= y && y < height && 0 <= x && x < width) ? input[b][c][y][x] : static_cast<scalar_t>(0);
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t interpolate_sample(
+                        const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t y,
+                        const scalar_t x) {
+                    if (y <= -1 || height <= y || x <= -1 || width <= x)
+                        return 0;
+
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_y_l = y_l >= 0;
+                    bool valid_y_h = y_h < height;
+                    bool valid_x_l = x_l >= 0;
+                    bool valid_x_h = x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
+                    if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
+                    if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
+                    if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
+                    return val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t interpolate_sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t y,
-                    const scalar_t x) {
-                if (y <= -1 || height <= y || x <= -1 || width <= x)
-                    return 0;
-
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_y_l = y_l >= 0;
-                bool valid_y_h = y_h < height;
-                bool valid_x_l = x_l >= 0;
-                bool valid_x_h = x_h < width;
-
-                scalar_t val = 0;
-                if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
-                if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
-                if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
-                if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
-                return val;
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ void insert(
+                        at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const index_t y,
+                        const index_t x,
+                        const scalar_t val) {
+                    if (0 <= y && y < height && 0 <= x && x < width)
+                        gpuAtomicAdd(&output[b][c][y][x], val);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const index_t y,
-                    const index_t x,
-                    const scalar_t val) {
-                if (0 <= y && y < height && 0 <= x && x < width)
-                    gpuAtomicAdd(&output[b][c][y][x], val);
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ void interpolate_insert(
+                        at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const scalar_t val) {
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    if (valid_y_l && valid_x_l) gpuAtomicAdd(&output[b][c][y_l][x_l], dy_l * dx_l * val);
+                    if (valid_y_l && valid_x_h) gpuAtomicAdd(&output[b][c][y_l][x_h], dy_l * dx_h * val);
+                    if (valid_y_h && valid_x_l) gpuAtomicAdd(&output[b][c][y_h][x_l], dy_h * dx_l * val);
+                    if (valid_y_h && valid_x_h) gpuAtomicAdd(&output[b][c][y_h][x_h], dy_h * dx_h * val);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void interpolate_insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const scalar_t val) {
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                if (valid_y_l && valid_x_l) gpuAtomicAdd(&output[b][c][y_l][x_l], dy_l * dx_l * val);
-                if (valid_y_l && valid_x_h) gpuAtomicAdd(&output[b][c][y_l][x_h], dy_l * dx_h * val);
-                if (valid_y_h && valid_x_l) gpuAtomicAdd(&output[b][c][y_h][x_l], dy_h * dx_l * val);
-                if (valid_y_h && valid_x_h) gpuAtomicAdd(&output[b][c][y_h][x_h], dy_h * dx_h * val);
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t coordinate_weight(
+                        const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const index_t direction) {
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dy_h = (direction == 0) ? static_cast<scalar_t>(1) : y - y_l;
+                    scalar_t dy_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dy_h;
+                    scalar_t dx_h = (direction == 1) ? static_cast<scalar_t>(1) : x - x_l;
+                    scalar_t dx_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dx_h;
+
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
+                    if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
+                    if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
+                    if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
+                    return val;
+                }
             }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t coordinate_weight(
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void im2col_kernel(
+                    const index_t n_kernels,
                     const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
+                    const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
                     const index_t height,
                     const index_t width,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const index_t direction) {
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dy_h = (direction == 0) ? static_cast<scalar_t>(1) : y - y_l;
-                scalar_t dy_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dy_h;
-                scalar_t dx_h = (direction == 1) ? static_cast<scalar_t>(1) : x - x_l;
-                scalar_t dx_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dx_h;
-
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                scalar_t val = 0;
-                if (valid_y_l && valid_x_l) val += dy_l * dx_l * input[b][c][y_l][x_l];
-                if (valid_y_l && valid_x_h) val += dy_l * dx_h * input[b][c][y_l][x_h];
-                if (valid_y_h && valid_x_l) val += dy_h * dx_l * input[b][c][y_h][x_l];
-                if (valid_y_h && valid_x_h) val += dy_h * dx_h * input[b][c][y_h][x_h];
-                return val;
-            }
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void im2col_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t in_channels,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t w = index % out_w;
-                const index_t h = (index / out_w) % out_h;
-                const index_t c = (index / (out_w * out_h)) % in_channels;
-                const index_t b = index / (out_w * out_h * in_channels);
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                for (index_t i = 0; i < weight_h; ++i) {
-                    for (index_t j = 0; j < weight_w; ++j) {
-                        const index_t y = (h * stride_h - pad_h) + i * dilation_h;
-                        const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t in_channels,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t w = index % out_w;
+                    const index_t h = (index / out_w) % out_h;
+                    const index_t c = (index / (out_w * out_h)) % in_channels;
+                    const index_t b = index / (out_w * out_h * in_channels);
 
-                        scalar_t val, mask_val;
-                        if constexpr (deformable)
-                            val = interpolate_sample(
-                                    input, b, c, height, width,
-                                    y + offset[b][offset_group_idx][i][j][0][h][w],
-                                    x + offset[b][offset_group_idx][i][j][1][h][w]);
-                        else
-                            val = sample(input, b, c, height, width, y, x);
+                    const index_t offset_group_idx = c / c_per_offset_group;
+                    const index_t mask_group_idx = c / c_per_mask_group;
 
-                        if constexpr (modulated)
-                            mask_val = mask[b][mask_group_idx][i][j][h][w];
-                        else
-                            mask_val = static_cast<scalar_t>(1);
+                    for (index_t i = 0; i < weight_h; ++i) {
+                        for (index_t j = 0; j < weight_w; ++j) {
+                            const index_t y = (h * stride_h - pad_h) + i * dilation_h;
+                            const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+
+                            scalar_t val, mask_val;
+                            if constexpr (deformable)
+                                val = interpolate_sample(
+                                        input, b, c, height, width,
+                                        y + offset[b][offset_group_idx][i][j][0][h][w],
+                                        x + offset[b][offset_group_idx][i][j][1][h][w]);
+                            else
+                                val = sample(input, b, c, height, width, y, x);
+
+                            if constexpr (modulated)
+                                mask_val = mask[b][mask_group_idx][i][j][h][w];
+                            else
+                                mask_val = static_cast<scalar_t>(1);
 
-                        columns[c][i][j][b][h][w] = val * mask_val;
+                            columns[c][i][j][b][h][w] = val * mask_val;
+                        }
                     }
                 }
             }
-        }
 
-        void im2col_cuda(
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &columns) {
-            at::cuda::CUDAGuard device_guard(input.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "im2col_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto columns_accessor =
-                            columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        im2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                in_channels,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                columns_accessor);
+            void im2col(
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &columns) {
+                at::cuda::CUDAGuard device_guard(input.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        input.scalar_type(), "im2col", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto columns_accessor =
+                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            im2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    in_channels,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    columns_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void col2im_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
-                const index_t in_channels,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> grad_input) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t j = index % weight_w;
-                const index_t i = (index / weight_w) % weight_h;
-                const index_t w = (index / (weight_w * weight_h)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
-                const index_t c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
-                const index_t b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                const index_t y = (h * stride_h - pad_h) + i * dilation_h;
-                const index_t x = (w * stride_w - pad_w) + j * dilation_w;
-
-                scalar_t mask_val;
-                if constexpr (modulated)
-                    mask_val = mask[b][mask_group_idx][i][j][h][w];
-                else
-                    mask_val = static_cast<scalar_t>(1);
-
-                scalar_t val = columns[c][i][j][b][h][w] * mask_val;
-
-                if constexpr (deformable)
-                    interpolate_insert(
-                            grad_input, b, c, height, width,
-                            y + offset[b][offset_group_idx][i][j][0][h][w],
-                            x + offset[b][offset_group_idx][i][j][1][h][w],
-                            val);
-                else
-                    insert(grad_input, b, c, height, width, y, x, val);
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
             }
-        }
 
-        void col2im_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_input) {
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2im_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
-                    auto grad_input_accessor =
-                            grad_input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2im_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                in_channels,
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_input_accessor);
-                    }));
-                }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void col2im_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
+                    const index_t in_channels,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> grad_input) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t j = index % weight_w;
+                    const index_t i = (index / weight_w) % weight_h;
+                    const index_t w = (index / (weight_w * weight_h)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
+                    const index_t c = (index / (weight_w * weight_h * out_w * out_h)) % in_channels;
+                    const index_t b = (index / (weight_w * weight_h * out_w * out_h * in_channels));
 
-        template<bool modulated, typename scalar_t, typename index_t>
-        static __global__ void deform_conv2d_compute_grad_offset_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t offset_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> grad_offset) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t o = index % 2;
-                const index_t j = (index / 2) % weight_w;
-                const index_t i = (index / (2 * weight_w)) % weight_h;
-                const index_t w = (index / (2 * weight_w * weight_h)) % out_w;
-                const index_t h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
-                const index_t g = (index / (2 * weight_w * weight_h * out_w * out_h)) % offset_groups;
-                const index_t b = index / (2 * weight_w * weight_h * out_w * out_h * offset_groups);
-
-                scalar_t grad_offset_val = 0;
-
-                const index_t c_start = g * c_per_offset_group;
-                const index_t c_end = c_start + c_per_offset_group;
-                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t y = (h * stride_h - pad_h) + i * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    scalar_t weight = coordinate_weight(
-                            input, b, c, height, width,
-                            y + offset[b][g][i][j][0][h][w],
-                            x + offset[b][g][i][j][1][h][w],
-                            o);
-
                     scalar_t mask_val;
                     if constexpr (modulated)
                         mask_val = mask[b][mask_group_idx][i][j][h][w];
                     else
                         mask_val = static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
-                }
+                    scalar_t val = columns[c][i][j][b][h][w] * mask_val;
 
-                grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
+                    if constexpr (deformable)
+                        interpolate_insert(
+                                grad_input, b, c, height, width,
+                                y + offset[b][offset_group_idx][i][j][0][h][w],
+                                x + offset[b][offset_group_idx][i][j][1][h][w],
+                                val);
+                    else
+                        insert(grad_input, b, c, height, width, y, x, val);
+                }
             }
-        }
 
-        void deform_conv2d_compute_grad_offset_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_offset) {
-            if (!deformable) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_h * out_w * weight_h * weight_w * 2;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_offset_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_offset_accessor =
-                            grad_offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                offset_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_offset_accessor);
+            void col2im(
+                    const at::Tensor &columns,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_input) {
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_h * out_w * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "col2im", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                        auto grad_input_accessor =
+                                grad_input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            col2im_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                    in_channels,
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_input_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
+            }
 
-        template<bool deformable, typename scalar_t, typename index_t>
-        static __global__ void deform_conv2d_compute_grad_mask_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
-                const index_t height,
-                const index_t width,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t mask_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> grad_mask) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t j = index % weight_w;
-                const index_t i = (index / weight_w) % weight_h;
-                const index_t w = (index / (weight_w * weight_h)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
-                const index_t g = (index / (weight_w * weight_h * out_w * out_h)) % mask_groups;
-                const index_t b = index / (out_w * out_h * weight_w * weight_h * mask_groups);
-
-                scalar_t grad_mask_val = 0;
-
-                const index_t c_start = g * c_per_mask_group;
-                const index_t c_end = c_start + c_per_mask_group;
-                for (index_t c = c_start; c < c_end; ++c) {
-                    const index_t offset_group_idx = c / c_per_offset_group;
+            template<bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void deform_conv2d_compute_grad_offset_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                    const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> mask,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t offset_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> grad_offset) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t o = index % 2;
+                    const index_t j = (index / 2) % weight_w;
+                    const index_t i = (index / (2 * weight_w)) % weight_h;
+                    const index_t w = (index / (2 * weight_w * weight_h)) % out_w;
+                    const index_t h = (index / (2 * weight_w * weight_h * out_w)) % out_h;
+                    const index_t g = (index / (2 * weight_w * weight_h * out_w * out_h)) % offset_groups;
+                    const index_t b = index / (2 * weight_w * weight_h * out_w * out_h * offset_groups);
+
+                    scalar_t grad_offset_val = 0;
+
+                    const index_t c_start = g * c_per_offset_group;
+                    const index_t c_end = c_start + c_per_offset_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t mask_group_idx = c / c_per_mask_group;
 
-                    const index_t y = (h * stride_h - pad_h) + i * dilation_h;
-                    const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+                        const index_t y = (h * stride_h - pad_h) + i * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + j * dilation_w;
 
-                    scalar_t val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
+                        scalar_t weight = coordinate_weight(
                                 input, b, c, height, width,
-                                y + offset[b][offset_group_idx][i][j][0][h][w],
-                                x + offset[b][offset_group_idx][i][j][1][h][w]);
-                    else
-                        val = sample(input, b, c, height, width, y, x);
+                                y + offset[b][g][i][j][0][h][w],
+                                x + offset[b][g][i][j][1][h][w],
+                                o);
+
+                        scalar_t mask_val;
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][j][h][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
+
+                        grad_offset_val += columns[c][i][j][b][h][w] * weight * mask_val;
+                    }
 
-                    grad_mask_val += columns[c][i][j][b][h][w] * val;
+                    grad_offset[b][g][i][j][o][h][w] = grad_offset_val;
                 }
+            }
 
-                grad_mask[b][g][i][j][h][w] = grad_mask_val;
+            void deform_conv2d_compute_grad_offset(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_offset) {
+                if (!deformable) return;
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * offset_groups * out_h * out_w * weight_h * weight_w * 2;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv2d_compute_grad_offset", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_offset_accessor =
+                                grad_offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                            deform_conv2d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                    input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    offset_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_offset_accessor);
+                        }));
+                    }));
+                }));
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
             }
-        }
 
-        void deform_conv2d_compute_grad_mask_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const int64_t in_channels,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_mask) {
-            if (!modulated) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_h * out_w * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv2d_compute_grad_mask_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_mask_accessor =
-                            grad_mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
-                                height,
-                                width,
-                                weight_h,
-                                weight_w,
-                                stride_h,
-                                stride_w,
-                                pad_h,
-                                pad_w,
-                                dilation_h,
-                                dilation_w,
-                                out_h,
-                                out_w,
-                                mask_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_mask_accessor);
+            template<bool deformable, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void deform_conv2d_compute_grad_mask_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 4, at::RestrictPtrTraits, index_t> input,
+                    const at::GenericPackedTensorAccessor<scalar_t, 7, at::RestrictPtrTraits, index_t> offset,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t mask_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 6, at::RestrictPtrTraits, index_t> grad_mask) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t j = index % weight_w;
+                    const index_t i = (index / weight_w) % weight_h;
+                    const index_t w = (index / (weight_w * weight_h)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * out_w)) % out_h;
+                    const index_t g = (index / (weight_w * weight_h * out_w * out_h)) % mask_groups;
+                    const index_t b = index / (out_w * out_h * weight_w * weight_h * mask_groups);
+
+                    scalar_t grad_mask_val = 0;
+
+                    const index_t c_start = g * c_per_mask_group;
+                    const index_t c_end = c_start + c_per_mask_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t offset_group_idx = c / c_per_offset_group;
+
+                        const index_t y = (h * stride_h - pad_h) + i * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + j * dilation_w;
+
+                        scalar_t val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, height, width,
+                                    y + offset[b][offset_group_idx][i][j][0][h][w],
+                                    x + offset[b][offset_group_idx][i][j][1][h][w]);
+                        else
+                            val = sample(input, b, c, height, width, y, x);
+
+                        grad_mask_val += columns[c][i][j][b][h][w] * val;
+                    }
+
+                    grad_mask[b][g][i][j][h][w] = grad_mask_val;
+                }
+            }
+
+            void deform_conv2d_compute_grad_mask(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const int64_t in_channels,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_mask) {
+                if (!modulated) return;
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * mask_groups * out_h * out_w * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv2d_compute_grad_mask", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_mask_accessor =
+                                grad_mask.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                            deform_conv2d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 6, at::RestrictPtrTraits, index_t>(),
+                                    input.generic_packed_accessor<scalar_t, 4, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 7, at::RestrictPtrTraits, index_t>(),
+                                    height,
+                                    width,
+                                    weight_h,
+                                    weight_w,
+                                    stride_h,
+                                    stride_w,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_h,
+                                    out_w,
+                                    mask_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_mask_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
+            }
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/cuda/deform_conv3d_kernels_cuda.cu` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_common_kernels.cu`

 * *Files 1% similar despite different names*

```diff
@@ -1,784 +1,787 @@
 #include <ATen/ATen.h>
 
 #include "cuda_helpers.h"
 #include "../utils/dispatch.h"
 
 namespace tvdcn {
     namespace ops {
-        namespace {
-            constexpr float threadsFraction = 0.5;
+        namespace cuda {
+            namespace {
+                constexpr float threadsFraction = 0.5;
+
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t sample(
+                        const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const index_t z,
+                        const index_t y,
+                        const index_t x) {
+                    return (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width) ?
+                           input[b][c][z][y][x] : static_cast<scalar_t>(0);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const index_t z,
-                    const index_t y,
-                    const index_t x) {
-                return (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width) ?
-                       input[b][c][z][y][x] : static_cast<scalar_t>(0);
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t interpolate_sample(
+                        const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t z,
+                        const scalar_t y,
+                        const scalar_t x) {
+                    if (z <= -1 || depth <= z || y <= -1 || height <= y || x <= -1 || width <= x)
+                        return 0;
+
+                    index_t z_l = floor(z);
+                    index_t z_h = z_l + 1;
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dz_h = z - z_l;
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dz_l = 1 - dz_h;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_z_l = z_l >= 0;
+                    bool valid_z_h = z_h < depth;
+                    bool valid_y_l = y_l >= 0;
+                    bool valid_y_h = y_h < height;
+                    bool valid_x_l = x_l >= 0;
+                    bool valid_x_h = x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_z_l && valid_y_l && valid_x_l)
+                        val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
+                    if (valid_z_l && valid_y_l && valid_x_h)
+                        val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
+                    if (valid_z_l && valid_y_h && valid_x_l)
+                        val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
+                    if (valid_z_l && valid_y_h && valid_x_h)
+                        val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
+                    if (valid_z_h && valid_y_l && valid_x_l)
+                        val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
+                    if (valid_z_h && valid_y_l && valid_x_h)
+                        val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
+                    if (valid_z_h && valid_y_h && valid_x_l)
+                        val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
+                    if (valid_z_h && valid_y_h && valid_x_h)
+                        val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
+                    return val;
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t interpolate_sample(
-                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t z,
-                    const scalar_t y,
-                    const scalar_t x) {
-                if (z <= -1 || depth <= z || y <= -1 || height <= y || x <= -1 || width <= x)
-                    return 0;
-
-                index_t z_l = floor(z);
-                index_t z_h = z_l + 1;
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dz_h = z - z_l;
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dz_l = 1 - dz_h;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_z_l = z_l >= 0;
-                bool valid_z_h = z_h < depth;
-                bool valid_y_l = y_l >= 0;
-                bool valid_y_h = y_h < height;
-                bool valid_x_l = x_l >= 0;
-                bool valid_x_h = x_h < width;
-
-                scalar_t val = 0;
-                if (valid_z_l && valid_y_l && valid_x_l)
-                    val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
-                if (valid_z_l && valid_y_l && valid_x_h)
-                    val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
-                if (valid_z_l && valid_y_h && valid_x_l)
-                    val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
-                if (valid_z_l && valid_y_h && valid_x_h)
-                    val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
-                if (valid_z_h && valid_y_l && valid_x_l)
-                    val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
-                if (valid_z_h && valid_y_l && valid_x_h)
-                    val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
-                if (valid_z_h && valid_y_h && valid_x_l)
-                    val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
-                if (valid_z_h && valid_y_h && valid_x_h)
-                    val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
-                return val;
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ void insert(
+                        at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const index_t z,
+                        const index_t y,
+                        const index_t x,
+                        const scalar_t val) {
+                    if (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width)
+                        gpuAtomicAdd(&output[b][c][z][y][x], val);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const index_t z,
-                    const index_t y,
-                    const index_t x,
-                    const scalar_t val) {
-                if (0 <= z && z < depth && 0 <= y && y < height && 0 <= x && x < width)
-                    gpuAtomicAdd(&output[b][c][z][y][x], val);
-            }
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ void interpolate_insert(
+                        at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> output,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t z,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const scalar_t val) {
+                    index_t z_l = floor(z);
+                    index_t z_h = z_l + 1;
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dz_h = z - z_l;
+                    scalar_t dy_h = y - y_l;
+                    scalar_t dx_h = x - x_l;
+                    scalar_t dz_l = 1 - dz_h;
+                    scalar_t dy_l = 1 - dy_h;
+                    scalar_t dx_l = 1 - dx_h;
+
+                    bool valid_z_l = 0 <= z_l && z_l < depth;
+                    bool valid_z_h = 0 <= z_h && z_h < depth;
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    if (valid_z_l && valid_y_l && valid_x_l)
+                        gpuAtomicAdd(&output[b][c][z_l][y_l][x_l], dz_l * dy_l * dx_l * val);
+                    if (valid_z_l && valid_y_l && valid_x_h)
+                        gpuAtomicAdd(&output[b][c][z_l][y_l][x_h], dz_l * dy_l * dx_h * val);
+                    if (valid_z_l && valid_y_h && valid_x_l)
+                        gpuAtomicAdd(&output[b][c][z_l][y_h][x_l], dz_l * dy_h * dx_l * val);
+                    if (valid_z_l && valid_y_h && valid_x_h)
+                        gpuAtomicAdd(&output[b][c][z_l][y_h][x_h], dz_l * dy_h * dx_h * val);
+                    if (valid_z_h && valid_y_l && valid_x_l)
+                        gpuAtomicAdd(&output[b][c][z_h][y_l][x_l], dz_h * dy_l * dx_l * val);
+                    if (valid_z_h && valid_y_l && valid_x_h)
+                        gpuAtomicAdd(&output[b][c][z_h][y_l][x_h], dz_h * dy_l * dx_h * val);
+                    if (valid_z_h && valid_y_h && valid_x_l)
+                        gpuAtomicAdd(&output[b][c][z_h][y_h][x_l], dz_h * dy_h * dx_l * val);
+                    if (valid_z_h && valid_y_h && valid_x_h)
+                        gpuAtomicAdd(&output[b][c][z_h][y_h][x_h], dz_h * dy_h * dx_h * val);
+                }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ void interpolate_insert(
-                    at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> output,
-                    const index_t b,
-                    const index_t c,
-                    const index_t depth,
-                    const index_t height,
-                    const index_t width,
-                    const scalar_t z,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const scalar_t val) {
-                index_t z_l = floor(z);
-                index_t z_h = z_l + 1;
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dz_h = z - z_l;
-                scalar_t dy_h = y - y_l;
-                scalar_t dx_h = x - x_l;
-                scalar_t dz_l = 1 - dz_h;
-                scalar_t dy_l = 1 - dy_h;
-                scalar_t dx_l = 1 - dx_h;
-
-                bool valid_z_l = 0 <= z_l && z_l < depth;
-                bool valid_z_h = 0 <= z_h && z_h < depth;
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                if (valid_z_l && valid_y_l && valid_x_l)
-                    gpuAtomicAdd(&output[b][c][z_l][y_l][x_l], dz_l * dy_l * dx_l * val);
-                if (valid_z_l && valid_y_l && valid_x_h)
-                    gpuAtomicAdd(&output[b][c][z_l][y_l][x_h], dz_l * dy_l * dx_h * val);
-                if (valid_z_l && valid_y_h && valid_x_l)
-                    gpuAtomicAdd(&output[b][c][z_l][y_h][x_l], dz_l * dy_h * dx_l * val);
-                if (valid_z_l && valid_y_h && valid_x_h)
-                    gpuAtomicAdd(&output[b][c][z_l][y_h][x_h], dz_l * dy_h * dx_h * val);
-                if (valid_z_h && valid_y_l && valid_x_l)
-                    gpuAtomicAdd(&output[b][c][z_h][y_l][x_l], dz_h * dy_l * dx_l * val);
-                if (valid_z_h && valid_y_l && valid_x_h)
-                    gpuAtomicAdd(&output[b][c][z_h][y_l][x_h], dz_h * dy_l * dx_h * val);
-                if (valid_z_h && valid_y_h && valid_x_l)
-                    gpuAtomicAdd(&output[b][c][z_h][y_h][x_l], dz_h * dy_h * dx_l * val);
-                if (valid_z_h && valid_y_h && valid_x_h)
-                    gpuAtomicAdd(&output[b][c][z_h][y_h][x_h], dz_h * dy_h * dx_h * val);
+                template<typename scalar_t, typename index_t>
+                __device__ __forceinline__ scalar_t coordinate_weight(
+                        const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
+                        const index_t b,
+                        const index_t c,
+                        const index_t depth,
+                        const index_t height,
+                        const index_t width,
+                        const scalar_t z,
+                        const scalar_t y,
+                        const scalar_t x,
+                        const index_t direction) {
+                    index_t z_l = floor(z);
+                    index_t z_h = z_l + 1;
+                    index_t y_l = floor(y);
+                    index_t y_h = y_l + 1;
+                    index_t x_l = floor(x);
+                    index_t x_h = x_l + 1;
+
+                    scalar_t dz_h = (direction == 0) ? static_cast<scalar_t>(1) : z - z_l;
+                    scalar_t dy_h = (direction == 1) ? static_cast<scalar_t>(1) : y - y_l;
+                    scalar_t dx_h = (direction == 2) ? static_cast<scalar_t>(1) : x - x_l;
+                    scalar_t dz_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dz_h;
+                    scalar_t dy_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dy_h;
+                    scalar_t dx_l = (direction == 2) ? static_cast<scalar_t>(-1) : 1 - dx_h;
+
+                    bool valid_z_l = 0 <= z_l && z_l < depth;
+                    bool valid_z_h = 0 <= z_h && z_h < depth;
+                    bool valid_y_l = 0 <= y_l && y_l < height;
+                    bool valid_y_h = 0 <= y_h && y_h < height;
+                    bool valid_x_l = 0 <= x_l && x_l < width;
+                    bool valid_x_h = 0 <= x_h && x_h < width;
+
+                    scalar_t val = 0;
+                    if (valid_z_l && valid_y_l && valid_x_l)
+                        val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
+                    if (valid_z_l && valid_y_l && valid_x_h)
+                        val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
+                    if (valid_z_l && valid_y_h && valid_x_l)
+                        val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
+                    if (valid_z_l && valid_y_h && valid_x_h)
+                        val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
+                    if (valid_z_h && valid_y_l && valid_x_l)
+                        val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
+                    if (valid_z_h && valid_y_l && valid_x_h)
+                        val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
+                    if (valid_z_h && valid_y_h && valid_x_l)
+                        val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
+                    if (valid_z_h && valid_y_h && valid_x_h)
+                        val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
+                    return val;
+                }
             }
 
-            template<typename scalar_t, typename index_t>
-            __device__ __forceinline__ scalar_t coordinate_weight(
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void vol2col_kernel(
+                    const index_t n_kernels,
                     const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
-                    const index_t b,
-                    const index_t c,
+                    const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> mask,
                     const index_t depth,
                     const index_t height,
                     const index_t width,
-                    const scalar_t z,
-                    const scalar_t y,
-                    const scalar_t x,
-                    const index_t direction) {
-                index_t z_l = floor(z);
-                index_t z_h = z_l + 1;
-                index_t y_l = floor(y);
-                index_t y_h = y_l + 1;
-                index_t x_l = floor(x);
-                index_t x_h = x_l + 1;
-
-                scalar_t dz_h = (direction == 0) ? static_cast<scalar_t>(1) : z - z_l;
-                scalar_t dy_h = (direction == 1) ? static_cast<scalar_t>(1) : y - y_l;
-                scalar_t dx_h = (direction == 2) ? static_cast<scalar_t>(1) : x - x_l;
-                scalar_t dz_l = (direction == 0) ? static_cast<scalar_t>(-1) : 1 - dz_h;
-                scalar_t dy_l = (direction == 1) ? static_cast<scalar_t>(-1) : 1 - dy_h;
-                scalar_t dx_l = (direction == 2) ? static_cast<scalar_t>(-1) : 1 - dx_h;
-
-                bool valid_z_l = 0 <= z_l && z_l < depth;
-                bool valid_z_h = 0 <= z_h && z_h < depth;
-                bool valid_y_l = 0 <= y_l && y_l < height;
-                bool valid_y_h = 0 <= y_h && y_h < height;
-                bool valid_x_l = 0 <= x_l && x_l < width;
-                bool valid_x_h = 0 <= x_h && x_h < width;
-
-                scalar_t val = 0;
-                if (valid_z_l && valid_y_l && valid_x_l)
-                    val += dz_l * dy_l * dx_l * input[b][c][z_l][y_l][x_l];
-                if (valid_z_l && valid_y_l && valid_x_h)
-                    val += dz_l * dy_l * dx_h * input[b][c][z_l][y_l][x_h];
-                if (valid_z_l && valid_y_h && valid_x_l)
-                    val += dz_l * dy_h * dx_l * input[b][c][z_l][y_h][x_l];
-                if (valid_z_l && valid_y_h && valid_x_h)
-                    val += dz_l * dy_h * dx_h * input[b][c][z_l][y_h][x_h];
-                if (valid_z_h && valid_y_l && valid_x_l)
-                    val += dz_h * dy_l * dx_l * input[b][c][z_h][y_l][x_l];
-                if (valid_z_h && valid_y_l && valid_x_h)
-                    val += dz_h * dy_l * dx_h * input[b][c][z_h][y_l][x_h];
-                if (valid_z_h && valid_y_h && valid_x_l)
-                    val += dz_h * dy_h * dx_l * input[b][c][z_h][y_h][x_l];
-                if (valid_z_h && valid_y_h && valid_x_h)
-                    val += dz_h * dy_h * dx_h * input[b][c][z_h][y_h][x_h];
-                return val;
-            }
-        }
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t in_channels,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t w = index % out_w;
+                    const index_t h = (index / out_w) % out_h;
+                    const index_t d = (index / (out_w * out_h)) % out_d;
+                    const index_t c = (index / (out_w * out_h * out_d)) % in_channels;
+                    const index_t b = index / (out_w * out_h * out_d * in_channels);
 
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void vol2col_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> mask,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t in_channels,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t w = index % out_w;
-                const index_t h = (index / out_w) % out_h;
-                const index_t d = (index / (out_w * out_h)) % out_d;
-                const index_t c = (index / (out_w * out_h * out_d)) % in_channels;
-                const index_t b = index / (out_w * out_h * out_d * in_channels);
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                for (index_t i = 0; i < weight_d; ++i) {
-                    for (index_t j = 0; j < weight_h; ++j) {
-                        for (index_t k = 0; k < weight_w; ++k) {
-                            const index_t z = (d * stride_d - pad_d) + i * dilation_d;
-                            const index_t y = (h * stride_h - pad_h) + j * dilation_h;
-                            const index_t x = (w * stride_w - pad_w) + k * dilation_w;
-
-                            scalar_t val, mask_val;
-                            if constexpr (deformable)
-                                val = interpolate_sample(
-                                        input, b, c, depth, height, width,
-                                        z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                        y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                        x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
-                            else
-                                val = sample(input, b, c, depth, height, width, z, y, x);
-
-                            if constexpr (modulated)
-                                mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
-                            else
-                                mask_val = static_cast<scalar_t>(1);
+                    const index_t offset_group_idx = c / c_per_offset_group;
+                    const index_t mask_group_idx = c / c_per_mask_group;
+
+                    for (index_t i = 0; i < weight_d; ++i) {
+                        for (index_t j = 0; j < weight_h; ++j) {
+                            for (index_t k = 0; k < weight_w; ++k) {
+                                const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                                const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                                const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+
+                                scalar_t val, mask_val;
+                                if constexpr (deformable)
+                                    val = interpolate_sample(
+                                            input, b, c, depth, height, width,
+                                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                                else
+                                    val = sample(input, b, c, depth, height, width, z, y, x);
+
+                                if constexpr (modulated)
+                                    mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                                else
+                                    mask_val = static_cast<scalar_t>(1);
 
-                            columns[c][i][j][k][b][d][h][w] = val * mask_val;
+                                columns[c][i][j][k][b][d][h][w] = val * mask_val;
+                            }
                         }
                     }
                 }
             }
-        }
 
-        void vol2col_cuda(
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &columns) {
-            at::cuda::CUDAGuard device_guard(input.get_device());
-            const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    input.scalar_type(), "vol2col_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto columns_accessor =
-                            columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        vol2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                in_channels,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                columns_accessor);
+            void vol2col(
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &columns) {
+                at::cuda::CUDAGuard device_guard(input.get_device());
+                const int64_t n_kernels = (int64_t) batch_sz * in_channels * out_d * out_h * out_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        input.scalar_type(), "vol2col", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto columns_accessor =
+                                columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            vol2col_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    in_channels,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    columns_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
-
-        template<bool deformable, bool modulated, typename scalar_t, typename index_t>
-        static __global__ void col2vol_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> mask,
-                const index_t in_channels,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> grad_input) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t k = index % weight_w;
-                const index_t j = (index / weight_w) % weight_h;
-                const index_t i = (index / (weight_w * weight_h)) % weight_d;
-                const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
-                const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
-                const index_t c = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % in_channels;
-                const index_t b = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * in_channels));
-
-                const index_t offset_group_idx = c / c_per_offset_group;
-                const index_t mask_group_idx = c / c_per_mask_group;
-
-                const index_t z = (d * stride_d - pad_d) + i * dilation_d;
-                const index_t y = (h * stride_h - pad_h) + j * dilation_h;
-                const index_t x = (w * stride_w - pad_w) + k * dilation_w;
-
-                scalar_t mask_val;
-                if constexpr (modulated)
-                    mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
-                else
-                    mask_val = static_cast<scalar_t>(1);
-
-                scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
-
-                if constexpr (deformable)
-                    interpolate_insert(
-                            grad_input, b, c, depth, height, width,
-                            z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                            y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                            x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
-                            val);
-                else
-                    insert(grad_input, b, c, depth, height, width, z, y, x, val);
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
             }
-        }
 
-        void col2vol_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_input) {
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels =
-                    (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "col2vol_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
-                    auto grad_input_accessor =
-                            grad_input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
-                        col2vol_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
-                                in_channels,
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_input_accessor);
-                    }));
-                }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
+            template<bool deformable, bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void col2vol_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> mask,
+                    const index_t in_channels,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> grad_input) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t k = index % weight_w;
+                    const index_t j = (index / weight_w) % weight_h;
+                    const index_t i = (index / (weight_w * weight_h)) % weight_d;
+                    const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
+                    const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                    const index_t c = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % in_channels;
+                    const index_t b = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * in_channels));
 
-        template<bool modulated, typename scalar_t, typename index_t>
-        static __global__ void deform_conv3d_compute_grad_offset_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
-                const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> mask,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t offset_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> grad_offset) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t o = index % 3;
-                const index_t k = (index / 3) % weight_w;
-                const index_t j = (index / (3 * weight_w)) % weight_h;
-                const index_t i = (index / (3 * weight_w * weight_h)) % weight_d;
-                const index_t w = (index / (3 * weight_w * weight_h * weight_d)) % out_w;
-                const index_t h = (index / (3 * weight_w * weight_h * weight_d * out_w)) % out_h;
-                const index_t d = (index / (3 * weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
-                const index_t g =
-                        (index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d)) % offset_groups;
-                const index_t b = index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d * offset_groups);
-
-                scalar_t grad_offset_val = 0;
-
-                const index_t c_start = g * c_per_offset_group;
-                const index_t c_end = c_start + c_per_offset_group;
-                for (index_t c = c_start; c < c_end; ++c) {
+                    const index_t offset_group_idx = c / c_per_offset_group;
                     const index_t mask_group_idx = c / c_per_mask_group;
 
                     const index_t z = (d * stride_d - pad_d) + i * dilation_d;
                     const index_t y = (h * stride_h - pad_h) + j * dilation_h;
                     const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    scalar_t weight =
-                            coordinate_weight(
-                                    input, b, c, depth, height, width,
-                                    z + offset[b][g][i][j][k][0][d][h][w],
-                                    y + offset[b][g][i][j][k][1][d][h][w],
-                                    x + offset[b][g][i][j][k][2][d][h][w],
-                                    o);
-
                     scalar_t mask_val;
                     if constexpr (modulated)
                         mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
                     else
                         mask_val = static_cast<scalar_t>(1);
 
-                    grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
-                }
+                    scalar_t val = columns[c][i][j][k][b][d][h][w] * mask_val;
 
-                grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
+                    if constexpr (deformable)
+                        interpolate_insert(
+                                grad_input, b, c, depth, height, width,
+                                z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                x + offset[b][offset_group_idx][i][j][k][2][d][h][w],
+                                val);
+                    else
+                        insert(grad_input, b, c, depth, height, width, z, y, x, val);
+                }
             }
-        }
 
-        void deform_conv3d_compute_grad_offset_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_offset) {
-            if (!deformable) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels =
-                    (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv3d_compute_grad_offset_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_offset_accessor =
-                            grad_offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION(modulated, ([&] {
-                        deform_conv3d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
-                                mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                offset_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_offset_accessor);
+            void col2vol(
+                    const at::Tensor &columns,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_input) {
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels =
+                        (int64_t) batch_sz * in_channels * out_d * out_h * out_w * weight_d * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "col2vol", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE(n_kernels, ([&] {
+                        auto grad_input_accessor =
+                                grad_input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION2(deformable, modulated, ([&] {
+                            col2vol_kernel<deformable, modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
+                                    in_channels,
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_input_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
-        }
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
+            }
 
-        template<bool deformable, typename scalar_t, typename index_t>
-        static __global__ void deform_conv3d_compute_grad_mask_kernel(
-                const index_t n_kernels,
-                const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns,
-                const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
-                const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
-                const index_t depth,
-                const index_t height,
-                const index_t width,
-                const index_t weight_d,
-                const index_t weight_h,
-                const index_t weight_w,
-                const index_t stride_d,
-                const index_t stride_h,
-                const index_t stride_w,
-                const index_t pad_d,
-                const index_t pad_h,
-                const index_t pad_w,
-                const index_t dilation_d,
-                const index_t dilation_h,
-                const index_t dilation_w,
-                const index_t out_d,
-                const index_t out_h,
-                const index_t out_w,
-                const index_t mask_groups,
-                const index_t c_per_offset_group,
-                const index_t c_per_mask_group,
-                at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> grad_mask) {
-            CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
-                const index_t k = index % weight_w;
-                const index_t j = (index / weight_w) % weight_h;
-                const index_t i = (index / (weight_w * weight_h)) % weight_d;
-                const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
-                const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
-                const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
-                const index_t g = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % mask_groups;
-                const index_t b = index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * mask_groups);
-
-                scalar_t grad_mask_val = 0;
-
-                const index_t c_start = g * c_per_mask_group;
-                const index_t c_end = c_start + c_per_mask_group;
-                for (index_t c = c_start; c < c_end; ++c) {
-                    const index_t offset_group_idx = c / c_per_offset_group;
+            template<bool modulated, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void deform_conv3d_compute_grad_offset_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
+                    const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
+                    const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> mask,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t offset_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> grad_offset) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t o = index % 3;
+                    const index_t k = (index / 3) % weight_w;
+                    const index_t j = (index / (3 * weight_w)) % weight_h;
+                    const index_t i = (index / (3 * weight_w * weight_h)) % weight_d;
+                    const index_t w = (index / (3 * weight_w * weight_h * weight_d)) % out_w;
+                    const index_t h = (index / (3 * weight_w * weight_h * weight_d * out_w)) % out_h;
+                    const index_t d = (index / (3 * weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                    const index_t g =
+                            (index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d)) % offset_groups;
+                    const index_t b =
+                            index / (3 * weight_w * weight_h * weight_d * out_w * out_h * out_d * offset_groups);
+
+                    scalar_t grad_offset_val = 0;
+
+                    const index_t c_start = g * c_per_offset_group;
+                    const index_t c_end = c_start + c_per_offset_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t mask_group_idx = c / c_per_mask_group;
+
+                        const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                        const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + k * dilation_w;
 
-                    const index_t z = (d * stride_d - pad_d) + i * dilation_d;
-                    const index_t y = (h * stride_h - pad_h) + j * dilation_h;
-                    const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+                        scalar_t weight =
+                                coordinate_weight(
+                                        input, b, c, depth, height, width,
+                                        z + offset[b][g][i][j][k][0][d][h][w],
+                                        y + offset[b][g][i][j][k][1][d][h][w],
+                                        x + offset[b][g][i][j][k][2][d][h][w],
+                                        o);
+
+                        scalar_t mask_val;
+                        if constexpr (modulated)
+                            mask_val = mask[b][mask_group_idx][i][j][k][d][h][w];
+                        else
+                            mask_val = static_cast<scalar_t>(1);
 
-                    scalar_t val;
-                    if constexpr (deformable)
-                        val = interpolate_sample(
-                                input, b, c, depth, height, width,
-                                z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
-                                y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
-                                x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
-                    else
-                        val = sample(input, b, c, depth, height, width, z, y, x);
+                        grad_offset_val += columns[c][i][j][k][b][d][h][w] * weight * mask_val;
+                    }
 
-                    grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
+                    grad_offset[b][g][i][j][k][o][d][h][w] = grad_offset_val;
                 }
+            }
 
-                grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
+            void deform_conv3d_compute_grad_offset(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const at::Tensor &mask,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_offset) {
+                if (!deformable) return;
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels =
+                        (int64_t) batch_sz * offset_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w * 3;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv3d_compute_grad_offset", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_offset_accessor =
+                                grad_offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION(modulated, ([&] {
+                            deform_conv3d_compute_grad_offset_kernel<modulated, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
+                                    input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
+                                    mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    offset_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_offset_accessor);
+                        }));
+                    }));
+                }));
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
             }
-        }
 
-        void deform_conv3d_compute_grad_mask_cuda(
-                const at::Tensor &columns,
-                const at::Tensor &input,
-                const at::Tensor &offset,
-                const int64_t in_channels,
-                const int64_t depth,
-                const int64_t height,
-                const int64_t width,
-                const int64_t weight_d,
-                const int64_t weight_h,
-                const int64_t weight_w,
-                const int64_t stride_d,
-                const int64_t stride_h,
-                const int64_t stride_w,
-                const int64_t pad_d,
-                const int64_t pad_h,
-                const int64_t pad_w,
-                const int64_t dilation_d,
-                const int64_t dilation_h,
-                const int64_t dilation_w,
-                const int64_t out_d,
-                const int64_t out_h,
-                const int64_t out_w,
-                const int64_t batch_sz,
-                const int64_t offset_groups,
-                const int64_t mask_groups,
-                const bool deformable,
-                const bool modulated,
-                at::Tensor &grad_mask) {
-            if (!modulated) return;
-            at::cuda::CUDAGuard device_guard(columns.get_device());
-            const int64_t n_kernels =
-                    (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
-            const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
-            const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
-
-            const unsigned int threads = GET_THREADS(threadsFraction);
-            const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
-
-            AT_DISPATCH_FLOATING_TYPES_AND_HALF(
-                    columns.scalar_type(), "deform_conv3d_compute_grad_mask_cuda", ([&] {
-                TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
-                    auto grad_mask_accessor =
-                            grad_mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>();
-                    TVDCN_DISPATCH_CONDITION(deformable, ([&] {
-                        deform_conv3d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
-                                n_kernels,
-                                columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
-                                input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
-                                offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
-                                depth,
-                                height,
-                                width,
-                                weight_d,
-                                weight_h,
-                                weight_w,
-                                stride_d,
-                                stride_h,
-                                stride_w,
-                                pad_d,
-                                pad_h,
-                                pad_w,
-                                dilation_d,
-                                dilation_h,
-                                dilation_w,
-                                out_d,
-                                out_h,
-                                out_w,
-                                mask_groups,
-                                c_per_offset_group,
-                                c_per_mask_group,
-                                grad_mask_accessor);
+            template<bool deformable, typename scalar_t, typename index_t>
+            static __launch_bounds__(1024) __global__ void deform_conv3d_compute_grad_mask_kernel(
+                    const index_t n_kernels,
+                    const at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> columns,
+                    const at::GenericPackedTensorAccessor<scalar_t, 5, at::RestrictPtrTraits, index_t> input,
+                    const at::GenericPackedTensorAccessor<scalar_t, 9, at::RestrictPtrTraits, index_t> offset,
+                    const index_t depth,
+                    const index_t height,
+                    const index_t width,
+                    const index_t weight_d,
+                    const index_t weight_h,
+                    const index_t weight_w,
+                    const index_t stride_d,
+                    const index_t stride_h,
+                    const index_t stride_w,
+                    const index_t pad_d,
+                    const index_t pad_h,
+                    const index_t pad_w,
+                    const index_t dilation_d,
+                    const index_t dilation_h,
+                    const index_t dilation_w,
+                    const index_t out_d,
+                    const index_t out_h,
+                    const index_t out_w,
+                    const index_t mask_groups,
+                    const index_t c_per_offset_group,
+                    const index_t c_per_mask_group,
+                    at::GenericPackedTensorAccessor<scalar_t, 8, at::RestrictPtrTraits, index_t> grad_mask) {
+                CUDA_1D_KERNEL_LOOP_T(index, n_kernels, index_t) {
+                    const index_t k = index % weight_w;
+                    const index_t j = (index / weight_w) % weight_h;
+                    const index_t i = (index / (weight_w * weight_h)) % weight_d;
+                    const index_t w = (index / (weight_w * weight_h * weight_d)) % out_w;
+                    const index_t h = (index / (weight_w * weight_h * weight_d * out_w)) % out_h;
+                    const index_t d = (index / (weight_w * weight_h * weight_d * out_w * out_h)) % out_d;
+                    const index_t g = (index / (weight_w * weight_h * weight_d * out_w * out_h * out_d)) % mask_groups;
+                    const index_t b = index / (weight_w * weight_h * weight_d * out_w * out_h * out_d * mask_groups);
+
+                    scalar_t grad_mask_val = 0;
+
+                    const index_t c_start = g * c_per_mask_group;
+                    const index_t c_end = c_start + c_per_mask_group;
+                    for (index_t c = c_start; c < c_end; ++c) {
+                        const index_t offset_group_idx = c / c_per_offset_group;
+
+                        const index_t z = (d * stride_d - pad_d) + i * dilation_d;
+                        const index_t y = (h * stride_h - pad_h) + j * dilation_h;
+                        const index_t x = (w * stride_w - pad_w) + k * dilation_w;
+
+                        scalar_t val;
+                        if constexpr (deformable)
+                            val = interpolate_sample(
+                                    input, b, c, depth, height, width,
+                                    z + offset[b][offset_group_idx][i][j][k][0][d][h][w],
+                                    y + offset[b][offset_group_idx][i][j][k][1][d][h][w],
+                                    x + offset[b][offset_group_idx][i][j][k][2][d][h][w]);
+                        else
+                            val = sample(input, b, c, depth, height, width, z, y, x);
+
+                        grad_mask_val += columns[c][i][j][k][b][d][h][w] * val;
+                    }
+
+                    grad_mask[b][g][i][j][k][d][h][w] = grad_mask_val;
+                }
+            }
+
+            void deform_conv3d_compute_grad_mask(
+                    const at::Tensor &columns,
+                    const at::Tensor &input,
+                    const at::Tensor &offset,
+                    const int64_t in_channels,
+                    const int64_t depth,
+                    const int64_t height,
+                    const int64_t width,
+                    const int64_t weight_d,
+                    const int64_t weight_h,
+                    const int64_t weight_w,
+                    const int64_t stride_d,
+                    const int64_t stride_h,
+                    const int64_t stride_w,
+                    const int64_t pad_d,
+                    const int64_t pad_h,
+                    const int64_t pad_w,
+                    const int64_t dilation_d,
+                    const int64_t dilation_h,
+                    const int64_t dilation_w,
+                    const int64_t out_d,
+                    const int64_t out_h,
+                    const int64_t out_w,
+                    const int64_t batch_sz,
+                    const int64_t offset_groups,
+                    const int64_t mask_groups,
+                    const bool deformable,
+                    const bool modulated,
+                    at::Tensor &grad_mask) {
+                if (!modulated) return;
+                at::cuda::CUDAGuard device_guard(columns.get_device());
+                const int64_t n_kernels =
+                        (int64_t) batch_sz * mask_groups * out_d * out_h * out_w * weight_d * weight_h * weight_w;
+                const int64_t c_per_offset_group = deformable ? in_channels / offset_groups : 1;
+                const int64_t c_per_mask_group = modulated ? in_channels / mask_groups : 1;
+
+                const unsigned int threads = GET_THREADS(threadsFraction);
+                const unsigned int blocks = GET_BLOCKS(threads, n_kernels);
+
+                AT_DISPATCH_FLOATING_TYPES_AND_HALF(
+                        columns.scalar_type(), "deform_conv3d_compute_grad_mask", ([&] {
+                    TVDCN_DISPATCH_INDEX_TYPE2(n_kernels, columns.numel(), ([&] {
+                        auto grad_mask_accessor =
+                                grad_mask.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>();
+                        TVDCN_DISPATCH_CONDITION(deformable, ([&] {
+                            deform_conv3d_compute_grad_mask_kernel<deformable, scalar_t, index_t><<<blocks, threads>>>(
+                                    n_kernels,
+                                    columns.generic_packed_accessor<scalar_t, 8, at::RestrictPtrTraits, index_t>(),
+                                    input.generic_packed_accessor<scalar_t, 5, at::RestrictPtrTraits, index_t>(),
+                                    offset.generic_packed_accessor<scalar_t, 9, at::RestrictPtrTraits, index_t>(),
+                                    depth,
+                                    height,
+                                    width,
+                                    weight_d,
+                                    weight_h,
+                                    weight_w,
+                                    stride_d,
+                                    stride_h,
+                                    stride_w,
+                                    pad_d,
+                                    pad_h,
+                                    pad_w,
+                                    dilation_d,
+                                    dilation_h,
+                                    dilation_w,
+                                    out_d,
+                                    out_h,
+                                    out_w,
+                                    mask_groups,
+                                    c_per_offset_group,
+                                    c_per_mask_group,
+                                    grad_mask_accessor);
+                        }));
                     }));
                 }));
-            }));
-            C10_CUDA_KERNEL_LAUNCH_CHECK();
+                C10_CUDA_KERNEL_LAUNCH_CHECK();
+            }
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv1d.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv1d_kernel.cpp`

 * *Files 7% similar despite different names*

```diff
@@ -65,274 +65,281 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
-#include <torch/autograd.h>
+#include <ATen/ATen.h>
+#include <torch/library.h>
 
-#include "dispatch/deform_conv1d_kernels.h"
-#include "utils/parallel_helpers.h"
-#include "utils/tensor_utils.h"
+#include "deform_conv1d_common_kernels.h"
+#include "../utils/parallel_helpers.h"
+#include "../utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv1d_forward(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                at::IntArrayRef stride,
-                at::IntArrayRef padding,
-                at::IntArrayRef dilation,
-                int64_t groups) {
-            at::CheckedFrom c = "deform_conv1d_forward";
-            auto args = {
-                    at::TensorArg(input, "input", 1),
-                    at::TensorArg(weight, "weight", 2),
-                    at::TensorArg(offset, "offset", 3),
-                    at::TensorArg(mask, "mask", 4),
-                    at::TensorArg(bias, "bias", 5)};
-            at::checkAllSameType(c, args);
-            at::checkAllSameDevice(c, args);
-
-            bool deformable = offset.defined() && offset.numel();
-            bool modulated = mask.defined() && mask.numel();
-            bool with_bias = bias.defined() && bias.numel();
-
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            TORCH_CHECK(input_c.ndimension() == 3)
-            TORCH_CHECK(weight_c.ndimension() == 3)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
-
-            int64_t batch_sz = input_c.size(0);
-            int64_t in_channels = input_c.size(1);
-            int64_t in_w = input_c.size(2);
-
-            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int64_t out_channels = weight_c.size(0);
-            int64_t weight_w = weight_c.size(2);
-
-            int64_t stride_w = stride[0];
-
-            int64_t pad_w = padding[0];
-
-            int64_t dilation_w = dilation[0];
-
-            int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
-
-            TORCH_CHECK(
-                    weight_w > 0,
-                    " weight_w: ",
-                    weight_w)
-            TORCH_CHECK(
-                    stride_w > 0,
-                    " stride_w: ",
-                    stride_w)
-            TORCH_CHECK(
-                    pad_w >= 0,
-                    " pad_w: ",
-                    pad_w)
-            TORCH_CHECK(
-                    dilation_w > 0,
-                    " dilation_w: ",
-                    dilation_w)
-
-            TORCH_CHECK(weight_c.size(1) * groups == in_channels)
-            TORCH_CHECK(weight_c.size(0) % groups == 0)
-
-            int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
-            int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
-
-            TORCH_CHECK(
-                    !deformable || offset_c.size(0) == input_c.size(0),
-                    "invalid batch size of offset")
-            TORCH_CHECK(
-                    !deformable || offset_groups > 0,
-                    "The shape of the offset tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2).\nGot offset.size(1)=",
-                    offset.size(1),
-                    ", while weight.size(2)=",
-                    weight_w)
-            TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(1) == offset_groups * weight_w,
-                    "offset.shape[1] is not valid. got: ",
-                    offset_c.size(1),
-                    " expected: ",
-                    offset_groups * weight_w)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(2) == out_w,
-                    "offset output dims: (",
-                    offset_c.size(2),
-                    ") - ",
-                    "computed output dims: (",
-                    out_w,
-                    ")")
-
-            TORCH_CHECK(
-                    !modulated || mask_c.size(0) == input_c.size(0),
-                    "invalid batch size of mask")
-            TORCH_CHECK(
-                    !modulated || mask_groups > 0,
-                    "The shape of the mask tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2).\nGot mask.size(1)=",
-                    mask.size(1),
-                    ", while weight.size(2)=",
-                    weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(1) == mask_groups * weight_w,
-                    "mask.shape[1] is not valid. got: ",
-                    mask_c.size(1),
-                    " expected: ",
-                    mask_groups * weight_w)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(2) == out_w,
-                    "mask output dims: (",
-                    mask_c.size(2),
-                    ") - ",
-                    "computed output dims: (",
-                    out_w,
-                    ")")
-
-            TORCH_CHECK(
-                    out_w > 0,
-                    "Calculated output size too small - out_w: ",
-                    out_w)
-
-            auto output = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
-
-            // Separate batches into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_w});
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+        using namespace cuda;
+
+        namespace {
+            at::Tensor deform_conv1d_forward_kernel(
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups) {
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
+
+                at::CheckedFrom c = "deform_conv1d_forward_kernel";
+                std::vector<at::TensorArg> args;
+                args.reserve(5);
+                args.emplace_back(at::TensorArg(input, "input", 1));
+                args.emplace_back(at::TensorArg(weight, "weight", 2));
+                if (deformable)
+                    args.emplace_back(at::TensorArg(offset.value(), "offset", 3));
+                if (modulated)
+                    args.emplace_back(at::TensorArg(mask.value(), "mask", 4));
+                if (with_bias)
+                    args.emplace_back(at::TensorArg(bias.value(), "bias", 5));
+                at::checkAllSameGPUExceptUndefined(c, args);
+                at::checkAllSameTypeExceptUndefined(c, args);
+
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
+
+                TORCH_CHECK(input_c.ndimension() == 3)
+                TORCH_CHECK(weight_c.ndimension() == 3)
+                TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
+                TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_w = input_c.size(2);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_w = weight_c.size(2);
+
+                int64_t stride_w = stride[0];
+
+                int64_t pad_w = padding[0];
+
+                int64_t dilation_w = dilation[0];
+
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                TORCH_CHECK(
+                        weight_w > 0,
+                        " weight_w: ",
+                        weight_w)
+                TORCH_CHECK(
+                        stride_w > 0,
+                        " stride_w: ",
+                        stride_w)
+                TORCH_CHECK(
+                        pad_w >= 0,
+                        " pad_w: ",
+                        pad_w)
+                TORCH_CHECK(
+                        dilation_w > 0,
+                        " dilation_w: ",
+                        dilation_w)
+
+                TORCH_CHECK(weight_c.size(1) * groups == in_channels)
+                TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+                int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
+
+                TORCH_CHECK(
+                        !deformable || offset_c.size(0) == input_c.size(0),
+                        "invalid batch size of offset")
+                TORCH_CHECK(
+                        !deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot offset.size(1)=",
+                        offset_c.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
+                TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(1) == offset_groups * weight_w,
+                        "offset.shape[1] is not valid. got: ",
+                        offset_c.size(1),
+                        " expected: ",
+                        offset_groups * weight_w)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(2) == out_w,
+                        "offset output dims: (",
+                        offset_c.size(2),
+                        ") - ",
+                        "computed output dims: (",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        !modulated || mask_c.size(0) == input_c.size(0),
+                        "invalid batch size of mask")
+                TORCH_CHECK(
+                        !modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot mask.size(1)=",
+                        mask_c.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
+                TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(1) == mask_groups * weight_w,
+                        "mask.shape[1] is not valid. got: ",
+                        mask_c.size(1),
+                        " expected: ",
+                        mask_groups * weight_w)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(2) == out_w,
+                        "mask output dims: (",
+                        mask_c.size(2),
+                        ") - ",
+                        "computed output dims: (",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        out_w > 0,
+                        "Calculated output size too small - out_w: ",
+                        out_w)
+
+                auto output = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
+
+                // Separate batches into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_w});
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_w,
+                                              1,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0});
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_w,
-                                          1,
                                           out_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0});
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          0, 0, 0});
+
+                output = output.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      mask_groups,
-                                      weight_w,
+                                      out_channels,
                                       out_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0});
+                auto output_buf = at::zeros(
+                        {batch_sz / n_parallel_imgs,
+                         out_channels,
+                         n_parallel_imgs,
+                         out_w},
+                        output.options());
 
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_w});
-            auto output_buf = at::zeros(
-                    {batch_sz / n_parallel_imgs,
-                     out_channels,
-                     n_parallel_imgs,
-                     out_w},
-                    output.options());
-
-            // Separate channels into convolution groups
-            output_buf = output_buf.view({output_buf.size(0),
-                                          groups,
-                                          output_buf.size(1) / groups,
-                                          output_buf.size(2),
-                                          output_buf.size(3)});
-            weight_c = weight_c.view({groups,
-                                      weight_c.size(0) / groups,
-                                      weight_c.size(1),
-                                      weight_c.size(2)});
-
-            // Sample points and perform convolution
-            auto columns = at::empty({groups,
-                                      in_channels * weight_w / groups,
-                                      n_parallel_imgs * out_w},
-                                     input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              out_w});
-            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                arr2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
+                // Separate channels into convolution groups
+                output_buf = output_buf.view({output_buf.size(0),
+                                              groups,
+                                              output_buf.size(1) / groups,
+                                              output_buf.size(2),
+                                              output_buf.size(3)});
+                weight_c = weight_c.view({groups,
+                                          weight_c.size(0) / groups,
+                                          weight_c.size(1),
+                                          weight_c.size(2)});
+
+                // Sample points and perform convolution
+                auto columns = at::empty({groups,
+                                          in_channels * weight_w / groups,
+                                          n_parallel_imgs * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    arr2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
 
-                for (int64_t g = 0; g < groups; g++) {
-                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    for (int64_t g = 0; g < groups; g++) {
+                        output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    }
                 }
-            }
 
-            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
-                                          out_channels,
-                                          n_parallel_imgs,
-                                          out_w});
-            output_buf.transpose_(1, 2);
-            output.copy_(output_buf);
-            output = output.view({batch_sz, out_channels, out_w});
-            if (with_bias)
-                output.add_(bias_c.view({1, out_channels, 1}));
+                output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                              out_channels,
+                                              n_parallel_imgs,
+                                              out_w});
+                output_buf.transpose_(1, 2);
+                output.copy_(output_buf);
+                output = output.view({batch_sz, out_channels, out_w});
+                if (with_bias)
+                    output.add_(bias_c.view({1, out_channels, 1}));
 
-            return output;
-        }
+                return output;
+            }
 
-        namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-            _deform_conv1d_backward(
+            deform_conv1d_backward_kernel(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
-                    const at::Tensor &offset,
-                    const at::Tensor &mask,
-                    const at::Tensor &bias,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
                     int64_t groups) {
-                bool deformable = offset.defined() && offset.numel();
-                bool modulated = mask.defined() && mask.numel();
-                bool with_bias = bias.defined() && bias.numel();
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
 
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
-                at::Tensor offset_c = offset.contiguous();
-                at::Tensor mask_c = mask.contiguous();
-                at::Tensor bias_c = bias.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
 
                 int64_t batch_sz = input_c.size(0);
                 int64_t in_channels = input_c.size(1);
                 int64_t in_w = input_c.size(2);
 
                 int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
@@ -343,16 +350,16 @@
 
                 int64_t pad_w = padding[0];
 
                 int64_t dilation_w = dilation[0];
 
                 int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
-                int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
+                int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
                 auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
 
@@ -492,129 +499,24 @@
                     for (int64_t g = 0; g < groups; g++) {
                         grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                     }
                 }
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
-                grad_offset = grad_offset.view_as(offset);
-                grad_mask = grad_mask.view_as(mask);
+                grad_offset = deformable ? grad_offset.view_as(offset.value()) : at::Tensor();
+                grad_mask = modulated ? grad_mask.view_as(mask.value()) : at::Tensor();
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
-        class DeformConv1dFunction
-                : public torch::autograd::Function<DeformConv1dFunction> {
-        public:
-            static torch::autograd::variable_list forward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::Variable &input,
-                    const torch::autograd::Variable &weight,
-                    const torch::autograd::Variable &offset,
-                    const torch::autograd::Variable &mask,
-                    const torch::autograd::Variable &bias,
-                    at::IntArrayRef stride,
-                    at::IntArrayRef padding,
-                    at::IntArrayRef dilation,
-                    int64_t groups) {
-                at::AutoDispatchBelowADInplaceOrView g;
-                auto output = deform_conv1d_forward(
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        dilation,
-                        groups);
-
-                ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride.vec();
-                ctx->saved_data["padding"] = padding.vec();
-                ctx->saved_data["dilation"] = dilation.vec();
-                ctx->saved_data["groups"] = groups;
-
-                return {
-                        output,
-                };
-            }
-
-            static torch::autograd::variable_list backward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::variable_list &grad_output) {
-                auto saved = ctx->get_saved_variables();
-                auto input = saved[0];
-                auto weight = saved[1];
-                auto offset = saved[2];
-                auto mask = saved[3];
-                auto bias = saved[4];
-
-                auto stride = ctx->saved_data["stride"].toIntVector();
-                auto padding = ctx->saved_data["padding"].toIntVector();
-                auto dilation = ctx->saved_data["dilation"].toIntVector();
-                auto groups = ctx->saved_data["groups"].toInt();
-
-                auto grads = detail::_deform_conv1d_backward(
-                        grad_output[0],
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        dilation,
-                        groups);
-                auto grad_input = std::get<0>(grads);
-                auto grad_weight = std::get<1>(grads);
-                auto grad_offset = std::get<2>(grads);
-                auto grad_mask = std::get<3>(grads);
-                auto grad_bias = std::get<4>(grads);
-
-                return {
-                        grad_input,
-                        grad_weight,
-                        grad_offset,
-                        grad_mask,
-                        grad_bias,
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                };
-            }
-        };
-
-        at::Tensor deform_conv1d(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::optional<at::Tensor> &offset = {},
-                const at::optional<at::Tensor> &mask = {},
-                const at::optional<at::Tensor> &bias = {},
-                at::IntArrayRef stride = 1,
-                at::IntArrayRef padding = 0,
-                at::IntArrayRef dilation = 1,
-                int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv1d")
-            auto result = DeformConv1dFunction::apply(
-                    input,
-                    weight,
-                    offset.value_or(input.new_zeros(0)),
-                    mask.value_or(input.new_zeros(0)),
-                    bias.value_or(input.new_zeros(0)),
-                    stride,
-                    padding,
-                    dilation,
-                    groups);
-            return result[0];
-        }
-
-        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
-            m.def("tvdcn::deform_conv1d(Tensor input, Tensor weight, "
-                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
-                  "int[1] stride=1, int[1] padding=0, int[1] dilation=1, int groups=1) -> Tensor",
-                  &deform_conv1d);
+        TORCH_LIBRARY_IMPL(tvdcn, CUDA, m) {
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::deform_conv1d"),
+                    TORCH_FN(deform_conv1d_forward_kernel));
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::_deform_conv1d_backward"),
+                    TORCH_FN(deform_conv1d_backward_kernel));
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv2d.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv2d_kernel.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -65,318 +65,325 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
-#include <torch/autograd.h>
+#include <ATen/ATen.h>
+#include <torch/library.h>
 
-#include "dispatch/deform_conv2d_kernels.h"
-#include "utils/parallel_helpers.h"
-#include "utils/tensor_utils.h"
+#include "deform_conv2d_common_kernels.h"
+#include "../utils/parallel_helpers.h"
+#include "../utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv2d_forward(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                at::IntArrayRef stride,
-                at::IntArrayRef padding,
-                at::IntArrayRef dilation,
-                int64_t groups) {
-            at::CheckedFrom c = "deform_conv2d_forward";
-            auto args = {
-                    at::TensorArg(input, "input", 1),
-                    at::TensorArg(weight, "weight", 2),
-                    at::TensorArg(offset, "offset", 3),
-                    at::TensorArg(mask, "mask", 4),
-                    at::TensorArg(bias, "bias", 5)};
-            at::checkAllSameType(c, args);
-            at::checkAllSameDevice(c, args);
-
-            bool deformable = offset.defined() && offset.numel();
-            bool modulated = mask.defined() && mask.numel();
-            bool with_bias = bias.defined() && bias.numel();
-
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            TORCH_CHECK(input_c.ndimension() == 4)
-            TORCH_CHECK(weight_c.ndimension() == 4)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
-
-            int64_t batch_sz = input_c.size(0);
-            int64_t in_channels = input_c.size(1);
-            int64_t in_h = input_c.size(2);
-            int64_t in_w = input_c.size(3);
-
-            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int64_t out_channels = weight_c.size(0);
-            int64_t weight_h = weight_c.size(2);
-            int64_t weight_w = weight_c.size(3);
-
-            int64_t stride_h = stride[0];
-            int64_t stride_w = stride[1];
-
-            int64_t pad_h = padding[0];
-            int64_t pad_w = padding[1];
-
-            int64_t dilation_h = dilation[0];
-            int64_t dilation_w = dilation[1];
-
-            int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
-
-            TORCH_CHECK(
-                    weight_h > 0 && weight_w > 0,
-                    "weight_h: ",
-                    weight_h,
-                    " weight_w: ",
-                    weight_w)
-            TORCH_CHECK(
-                    stride_h > 0 && stride_w > 0,
-                    "stride_h: ",
-                    stride_h,
-                    " stride_w: ",
-                    stride_w)
-            TORCH_CHECK(
-                    pad_h >= 0 && pad_w >= 0,
-                    "pad_h: ",
-                    pad_h,
-                    " pad_w: ",
-                    pad_w)
-            TORCH_CHECK(
-                    dilation_h > 0 && dilation_w > 0,
-                    "dilation_h: ",
-                    dilation_h,
-                    " dilation_w: ",
-                    dilation_w)
-
-            TORCH_CHECK(weight_c.size(1) * groups == in_channels)
-            TORCH_CHECK(weight_c.size(0) % groups == 0)
-
-            int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
-            int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
-
-            TORCH_CHECK(
-                    !deformable || offset_c.size(0) == input_c.size(0),
-                    "invalid batch size of offset")
-            TORCH_CHECK(
-                    !deformable || offset_groups > 0,
-                    "The shape of the offset tensor at dimension 1 is not valid. It should "
-                    "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
-                    offset.size(1),
-                    ", while 2 * weight.size(2) * weight.size(3)=",
-                    2 * weight_h * weight_w)
-            TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w,
-                    "offset.shape[1] is not valid. got: ",
-                    offset_c.size(1),
-                    " expected: ",
-                    offset_groups * 2 * weight_h * weight_w)
-            TORCH_CHECK(
-                    !deformable || (offset_c.size(2) == out_h &&
-                                    offset_c.size(3) == out_w),
-                    "offset output dims: (",
-                    offset_c.size(2),
-                    ", ",
-                    offset_c.size(3),
-                    ") - ",
-                    "computed output dims: (",
-                    out_h,
-                    ", ",
-                    out_w,
-                    ")")
-
-            TORCH_CHECK(
-                    !modulated || mask_c.size(0) == input_c.size(0),
-                    "invalid batch size of mask")
-            TORCH_CHECK(
-                    !modulated || mask_groups > 0,
-                    "The shape of the mask tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
-                    mask.size(1),
-                    ", while weight.size(2) * weight.size(3)=",
-                    weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(1) == mask_groups * weight_h * weight_w,
-                    "mask.shape[1] is not valid. got: ",
-                    mask_c.size(1),
-                    " expected: ",
-                    mask_groups * weight_h * weight_w)
-            TORCH_CHECK(
-                    !modulated || (mask_c.size(2) == out_h &&
-                                   mask_c.size(3) == out_w),
-                    "mask output dims: (",
-                    mask_c.size(2),
-                    ", ",
-                    mask_c.size(3),
-                    ") - ",
-                    "computed output dims: (",
-                    out_h,
-                    ", ",
-                    out_w,
-                    ")")
-
-            TORCH_CHECK(
-                    out_h > 0 && out_w > 0,
-                    "Calculated output size too small - out_h: ",
-                    out_h,
-                    " out_w: ",
-                    out_w)
-
-            auto output = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
-
-            // Separate batches into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_h,
-                                    in_w});
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+        using namespace cuda;
+
+        namespace {
+            at::Tensor deform_conv2d_forward_kernel(
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups) {
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
+
+                at::CheckedFrom c = "deform_conv2d_forward_kernel";
+                std::vector<at::TensorArg> args;
+                args.reserve(5);
+                args.emplace_back(at::TensorArg(input, "input", 1));
+                args.emplace_back(at::TensorArg(weight, "weight", 2));
+                if (deformable)
+                    args.emplace_back(at::TensorArg(offset.value(), "offset", 3));
+                if (modulated)
+                    args.emplace_back(at::TensorArg(mask.value(), "mask", 4));
+                if (with_bias)
+                    args.emplace_back(at::TensorArg(bias.value(), "bias", 5));
+                at::checkAllSameGPUExceptUndefined(c, args);
+                at::checkAllSameTypeExceptUndefined(c, args);
+
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
+
+                TORCH_CHECK(input_c.ndimension() == 4)
+                TORCH_CHECK(weight_c.ndimension() == 4)
+                TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
+                TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_h = input_c.size(2);
+                int64_t in_w = input_c.size(3);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_h = weight_c.size(2);
+                int64_t weight_w = weight_c.size(3);
+
+                int64_t stride_h = stride[0];
+                int64_t stride_w = stride[1];
+
+                int64_t pad_h = padding[0];
+                int64_t pad_w = padding[1];
+
+                int64_t dilation_h = dilation[0];
+                int64_t dilation_w = dilation[1];
+
+                int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                TORCH_CHECK(
+                        weight_h > 0 && weight_w > 0,
+                        "weight_h: ",
+                        weight_h,
+                        " weight_w: ",
+                        weight_w)
+                TORCH_CHECK(
+                        stride_h > 0 && stride_w > 0,
+                        "stride_h: ",
+                        stride_h,
+                        " stride_w: ",
+                        stride_w)
+                TORCH_CHECK(
+                        pad_h >= 0 && pad_w >= 0,
+                        "pad_h: ",
+                        pad_h,
+                        " pad_w: ",
+                        pad_w)
+                TORCH_CHECK(
+                        dilation_h > 0 && dilation_w > 0,
+                        "dilation_h: ",
+                        dilation_h,
+                        " dilation_w: ",
+                        dilation_w)
+
+                TORCH_CHECK(weight_c.size(1) * groups == in_channels)
+                TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+                int64_t offset_groups = deformable ? offset_c.size(1) / (2 * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_h * weight_w) : 0;
+
+                TORCH_CHECK(
+                        !deformable || offset_c.size(0) == input_c.size(0),
+                        "invalid batch size of offset")
+                TORCH_CHECK(
+                        !deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
+                        offset_c.size(1),
+                        ", while 2 * weight.size(2) * weight.size(3)=",
+                        2 * weight_h * weight_w)
+                TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w,
+                        "offset.shape[1] is not valid. got: ",
+                        offset_c.size(1),
+                        " expected: ",
+                        offset_groups * 2 * weight_h * weight_w)
+                TORCH_CHECK(
+                        !deformable || (offset_c.size(2) == out_h &&
+                                        offset_c.size(3) == out_w),
+                        "offset output dims: (",
+                        offset_c.size(2),
+                        ", ",
+                        offset_c.size(3),
+                        ") - ",
+                        "computed output dims: (",
+                        out_h,
+                        ", ",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        !modulated || mask_c.size(0) == input_c.size(0),
+                        "invalid batch size of mask")
+                TORCH_CHECK(
+                        !modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
+                        mask_c.size(1),
+                        ", while weight.size(2) * weight.size(3)=",
+                        weight_h * weight_w)
+                TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(1) == mask_groups * weight_h * weight_w,
+                        "mask.shape[1] is not valid. got: ",
+                        mask_c.size(1),
+                        " expected: ",
+                        mask_groups * weight_h * weight_w)
+                TORCH_CHECK(
+                        !modulated || (mask_c.size(2) == out_h &&
+                                       mask_c.size(3) == out_w),
+                        "mask output dims: (",
+                        mask_c.size(2),
+                        ", ",
+                        mask_c.size(3),
+                        ") - ",
+                        "computed output dims: (",
+                        out_h,
+                        ", ",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        out_h > 0 && out_w > 0,
+                        "Calculated output size too small - out_h: ",
+                        out_h,
+                        " out_w: ",
+                        out_w)
+
+                auto output = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
+
+                // Separate batches into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_h,
+                                        in_w});
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_h,
+                                              weight_w,
+                                              2,
+                                              out_h,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0});
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_h,
                                           weight_w,
-                                          2,
                                           out_h,
                                           out_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0});
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          0, 0, 0, 0, 0});
+
+                output = output.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      mask_groups,
-                                      weight_h,
-                                      weight_w,
+                                      out_channels,
                                       out_h,
                                       out_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0});
+                auto output_buf = at::zeros(
+                        {batch_sz / n_parallel_imgs,
+                         out_channels,
+                         n_parallel_imgs,
+                         out_h,
+                         out_w},
+                        output.options());
 
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_h,
-                                  out_w});
-            auto output_buf = at::zeros(
-                    {batch_sz / n_parallel_imgs,
-                     out_channels,
-                     n_parallel_imgs,
-                     out_h,
-                     out_w},
-                    output.options());
-
-            // Separate channels into convolution groups
-            output_buf = output_buf.view({output_buf.size(0),
-                                          groups,
-                                          output_buf.size(1) / groups,
-                                          output_buf.size(2),
-                                          output_buf.size(3),
-                                          output_buf.size(4)});
-            weight_c = weight_c.view({groups,
-                                      weight_c.size(0) / groups,
-                                      weight_c.size(1),
-                                      weight_c.size(2),
-                                      weight_c.size(3)});
-
-            // Sample points and perform convolution
-            auto columns = at::empty({groups,
-                                      in_channels * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_h * out_w},
-                                     input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_h,
-                                              weight_w,
+                // Separate channels into convolution groups
+                output_buf = output_buf.view({output_buf.size(0),
+                                              groups,
+                                              output_buf.size(1) / groups,
+                                              output_buf.size(2),
+                                              output_buf.size(3),
+                                              output_buf.size(4)});
+                weight_c = weight_c.view({groups,
+                                          weight_c.size(0) / groups,
+                                          weight_c.size(1),
+                                          weight_c.size(2),
+                                          weight_c.size(3)});
+
+                // Sample points and perform convolution
+                auto columns = at::empty({groups,
+                                          in_channels * weight_h * weight_w / groups,
+                                          n_parallel_imgs * out_h * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_h,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_h,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    im2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_h,
+                            in_w,
+                            weight_h,
+                            weight_w,
+                            stride_h,
+                            stride_w,
+                            pad_h,
+                            pad_w,
+                            dilation_h,
+                            dilation_w,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    }
+                }
+
+                output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                              out_channels,
                                               n_parallel_imgs,
                                               out_h,
                                               out_w});
-            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                im2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_h,
-                        in_w,
-                        weight_h,
-                        weight_w,
-                        stride_h,
-                        stride_w,
-                        pad_h,
-                        pad_w,
-                        dilation_h,
-                        dilation_w,
-                        out_h,
-                        out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
+                output_buf.transpose_(1, 2);
+                output.copy_(output_buf);
+                output = output.view({batch_sz, out_channels, out_h, out_w});
+                if (with_bias)
+                    output.add_(bias_c.view({1, out_channels, 1, 1}));
 
-                for (int64_t g = 0; g < groups; g++) {
-                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                }
+                return output;
             }
 
-            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
-                                          out_channels,
-                                          n_parallel_imgs,
-                                          out_h,
-                                          out_w});
-            output_buf.transpose_(1, 2);
-            output.copy_(output_buf);
-            output = output.view({batch_sz, out_channels, out_h, out_w});
-            if (with_bias)
-                output.add_(bias_c.view({1, out_channels, 1, 1}));
-
-            return output;
-        }
-
-        namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-            _deform_conv2d_backward(
+            deform_conv2d_backward_kernel(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
-                    const at::Tensor &offset,
-                    const at::Tensor &mask,
-                    const at::Tensor &bias,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
                     int64_t groups) {
-                bool deformable = offset.defined() && offset.numel();
-                bool modulated = mask.defined() && mask.numel();
-                bool with_bias = bias.defined() && bias.numel();
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
 
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
-                at::Tensor offset_c = offset.contiguous();
-                at::Tensor mask_c = mask.contiguous();
-                at::Tensor bias_c = bias.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
 
                 int64_t batch_sz = input_c.size(0);
                 int64_t in_channels = input_c.size(1);
                 int64_t in_h = input_c.size(2);
                 int64_t in_w = input_c.size(3);
 
                 int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
@@ -393,16 +400,16 @@
 
                 int64_t dilation_h = dilation[0];
                 int64_t dilation_w = dilation[1];
 
                 int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
                 int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
-                int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
+                int64_t offset_groups = deformable ? offset_c.size(1) / (2 * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
                 auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
 
@@ -575,129 +582,24 @@
                     for (int64_t g = 0; g < groups; g++) {
                         grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                     }
                 }
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
-                grad_offset = grad_offset.view_as(offset);
-                grad_mask = grad_mask.view_as(mask);
+                grad_offset = deformable ? grad_offset.view_as(offset.value()) : at::Tensor();
+                grad_mask = modulated ? grad_mask.view_as(mask.value()) : at::Tensor();
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
-        class DeformConv2dFunction
-                : public torch::autograd::Function<DeformConv2dFunction> {
-        public:
-            static torch::autograd::variable_list forward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::Variable &input,
-                    const torch::autograd::Variable &weight,
-                    const torch::autograd::Variable &offset,
-                    const torch::autograd::Variable &mask,
-                    const torch::autograd::Variable &bias,
-                    at::IntArrayRef stride,
-                    at::IntArrayRef padding,
-                    at::IntArrayRef dilation,
-                    int64_t groups) {
-                at::AutoDispatchBelowADInplaceOrView g;
-                auto output = deform_conv2d_forward(
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        dilation,
-                        groups);
-
-                ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride.vec();
-                ctx->saved_data["padding"] = padding.vec();
-                ctx->saved_data["dilation"] = dilation.vec();
-                ctx->saved_data["groups"] = groups;
-
-                return {
-                        output,
-                };
-            }
-
-            static torch::autograd::variable_list backward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::variable_list &grad_output) {
-                auto saved = ctx->get_saved_variables();
-                auto input = saved[0];
-                auto weight = saved[1];
-                auto offset = saved[2];
-                auto mask = saved[3];
-                auto bias = saved[4];
-
-                auto stride = ctx->saved_data["stride"].toIntVector();
-                auto padding = ctx->saved_data["padding"].toIntVector();
-                auto dilation = ctx->saved_data["dilation"].toIntVector();
-                auto groups = ctx->saved_data["groups"].toInt();
-
-                auto grads = detail::_deform_conv2d_backward(
-                        grad_output[0],
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        dilation,
-                        groups);
-                auto grad_input = std::get<0>(grads);
-                auto grad_weight = std::get<1>(grads);
-                auto grad_offset = std::get<2>(grads);
-                auto grad_mask = std::get<3>(grads);
-                auto grad_bias = std::get<4>(grads);
-
-                return {
-                        grad_input,
-                        grad_weight,
-                        grad_offset,
-                        grad_mask,
-                        grad_bias,
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                };
-            }
-        };
-
-        at::Tensor deform_conv2d(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::optional<at::Tensor> &offset = {},
-                const at::optional<at::Tensor> &mask = {},
-                const at::optional<at::Tensor> &bias = {},
-                at::IntArrayRef stride = 1,
-                at::IntArrayRef padding = 0,
-                at::IntArrayRef dilation = 1,
-                int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv2d")
-            auto result = DeformConv2dFunction::apply(
-                    input,
-                    weight,
-                    offset.value_or(input.new_zeros(0)),
-                    mask.value_or(input.new_zeros(0)),
-                    bias.value_or(input.new_zeros(0)),
-                    stride,
-                    padding,
-                    dilation,
-                    groups);
-            return result[0];
-        }
-
-        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
-            m.def("tvdcn::deform_conv2d(Tensor input, Tensor weight, "
-                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
-                  "int[2] stride=1, int[2] padding=0, int[2] dilation=1, int groups=1) -> Tensor",
-                  &deform_conv2d);
+        TORCH_LIBRARY_IMPL(tvdcn, CUDA, m) {
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::deform_conv2d"),
+                    TORCH_FN(deform_conv2d_forward_kernel));
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::_deform_conv2d_backward"),
+                    TORCH_FN(deform_conv2d_backward_kernel));
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv3d.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv3d_kernel.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -65,362 +65,369 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
-#include <torch/autograd.h>
+#include <ATen/ATen.h>
+#include <torch/library.h>
 
-#include "dispatch/deform_conv3d_kernels.h"
-#include "utils/parallel_helpers.h"
-#include "utils/tensor_utils.h"
+#include "deform_conv3d_common_kernels.h"
+#include "../utils/parallel_helpers.h"
+#include "../utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv3d_forward(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                at::IntArrayRef stride,
-                at::IntArrayRef padding,
-                at::IntArrayRef dilation,
-                int64_t groups) {
-            at::CheckedFrom c = "deform_conv3d_forward";
-            auto args = {
-                    at::TensorArg(input, "input", 1),
-                    at::TensorArg(weight, "weight", 2),
-                    at::TensorArg(offset, "offset", 3),
-                    at::TensorArg(mask, "mask", 4),
-                    at::TensorArg(bias, "bias", 5)};
-            at::checkAllSameType(c, args);
-            at::checkAllSameDevice(c, args);
-
-            bool deformable = offset.defined() && offset.numel();
-            bool modulated = mask.defined() && mask.numel();
-            bool with_bias = bias.defined() && bias.numel();
-
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            TORCH_CHECK(input_c.ndimension() == 5)
-            TORCH_CHECK(weight_c.ndimension() == 5)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
-
-            int64_t batch_sz = input_c.size(0);
-            int64_t in_channels = input_c.size(1);
-            int64_t in_d = input_c.size(2);
-            int64_t in_h = input_c.size(3);
-            int64_t in_w = input_c.size(4);
-
-            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int64_t out_channels = weight_c.size(0);
-            int64_t weight_d = weight_c.size(2);
-            int64_t weight_h = weight_c.size(3);
-            int64_t weight_w = weight_c.size(4);
-
-            int64_t stride_d = stride[0];
-            int64_t stride_h = stride[1];
-            int64_t stride_w = stride[2];
-
-            int64_t pad_d = padding[0];
-            int64_t pad_h = padding[1];
-            int64_t pad_w = padding[2];
-
-            int64_t dilation_d = dilation[0];
-            int64_t dilation_h = dilation[1];
-            int64_t dilation_w = dilation[2];
-
-            int64_t out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
-            int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
-            int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
-
-            TORCH_CHECK(
-                    weight_d > 0 && weight_h > 0 && weight_w > 0,
-                    "weight_d: ",
-                    weight_d,
-                    " weight_h: ",
-                    weight_h,
-                    " weight_w: ",
-                    weight_w)
-            TORCH_CHECK(
-                    stride_d > 0 && stride_h > 0 && stride_w > 0,
-                    " stride_d: ",
-                    stride_d,
-                    "stride_h: ",
-                    stride_h,
-                    " stride_w: ",
-                    stride_w)
-            TORCH_CHECK(
-                    pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
-                    "pad_d: ",
-                    pad_d,
-                    " pad_h: ",
-                    pad_h,
-                    " pad_w: ",
-                    pad_w)
-            TORCH_CHECK(
-                    dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
-                    "dilation_d: ",
-                    dilation_d,
-                    " dilation_h: ",
-                    dilation_h,
-                    " dilation_w: ",
-                    dilation_w)
-
-            TORCH_CHECK(weight_c.size(1) * groups == in_channels)
-            TORCH_CHECK(weight_c.size(0) % groups == 0)
-
-            int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
-            int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
-
-            TORCH_CHECK(
-                    !deformable || offset_c.size(0) == input_c.size(0),
-                    "invalid batch size of offset")
-            TORCH_CHECK(
-                    !deformable || offset_groups > 0,
-                    "The shape of the offset tensor at dimension 1 is not valid. It should "
-                    "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
-                    offset.size(1),
-                    ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
-                    3 * weight_d * weight_h * weight_w)
-            TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
-                    "offset.shape[1] is not valid. got: ",
-                    offset_c.size(1),
-                    " expected: ",
-                    offset_groups * 3 * weight_d * weight_h * weight_w)
-            TORCH_CHECK(
-                    !deformable || (offset_c.size(2) == out_d &&
-                                    offset_c.size(3) == out_h &&
-                                    offset_c.size(4) == out_w),
-                    "offset output dims: (",
-                    offset_c.size(2),
-                    ", ",
-                    offset_c.size(3),
-                    ", ",
-                    offset_c.size(4),
-                    ") - ",
-                    "computed output dims: (",
-                    out_d,
-                    ", ",
-                    out_h,
-                    ", ",
-                    out_w,
-                    ")")
-
-            TORCH_CHECK(
-                    !modulated || mask_c.size(0) == input_c.size(0),
-                    "invalid batch size of mask")
-            TORCH_CHECK(
-                    !modulated || mask_groups > 0,
-                    "The shape of the mask tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
-                    mask.size(1),
-                    ", while weight.size(2) * weight.size(3) * weight.size(4)=",
-                    weight_d * weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
-                    "mask.shape[1] is not valid. got: ",
-                    mask_c.size(1),
-                    " expected: ",
-                    mask_groups * weight_d * weight_h * weight_w)
-            TORCH_CHECK(
-                    !modulated || (mask_c.size(2) == out_d &&
-                                   mask_c.size(3) == out_h &&
-                                   mask_c.size(4) == out_w),
-                    "mask output dims: (",
-                    mask_c.size(2),
-                    ", ",
-                    mask_c.size(3),
-                    ", ",
-                    mask_c.size(4),
-                    ") - ",
-                    "computed output dims: (",
-                    out_d,
-                    ", ",
-                    out_h,
-                    ", ",
-                    out_w,
-                    ")")
-
-            TORCH_CHECK(
-                    out_d > 0 && out_h > 0 && out_w > 0,
-                    "Calculated output size too small - out_d: ",
-                    out_d,
-                    " out_h: ",
-                    out_h,
-                    " out_w: ",
-                    out_w)
-
-            auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
-
-            // Separate batches into blocks
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    in_channels,
-                                    in_d,
-                                    in_h,
-                                    in_w});
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          offset_groups,
-                                          weight_d,
-                                          weight_h,
-                                          weight_w,
-                                          3,
-                                          out_d,
-                                          out_h,
-                                          out_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0, 0, 0});
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_d,
-                                      weight_h,
-                                      weight_w,
-                                      out_d,
-                                      out_h,
-                                      out_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0, 0, 0});
+        using namespace cuda;
 
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_d,
-                                  out_h,
-                                  out_w});
-            auto output_buf = at::zeros(
-                    {batch_sz / n_parallel_imgs,
-                     out_channels,
-                     n_parallel_imgs,
-                     out_d,
-                     out_h,
-                     out_w},
-                    output.options());
-
-            // Separate channels into convolution groups
-            output_buf = output_buf.view({output_buf.size(0),
-                                          groups,
-                                          output_buf.size(1) / groups,
-                                          output_buf.size(2),
-                                          output_buf.size(3),
-                                          output_buf.size(4),
-                                          output_buf.size(5)});
-            weight_c = weight_c.view({groups,
-                                      weight_c.size(0) / groups,
-                                      weight_c.size(1),
-                                      weight_c.size(2),
-                                      weight_c.size(3),
-                                      weight_c.size(4)});
-
-            // Sample points and perform convolution
-            auto columns = at::empty({groups,
-                                      in_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * out_d * out_h * out_w},
-                                     input_c.options());
-            auto columns_view = columns.view({in_channels,
-                                              weight_d,
-                                              weight_h,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              out_d,
-                                              out_h,
-                                              out_w});
-            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                vol2col(
-                        input_c[b],
-                        offset_c[b],
-                        mask_c[b],
-                        in_channels,
-                        in_d,
-                        in_h,
-                        in_w,
+        namespace {
+            at::Tensor deform_conv3d_forward_kernel(
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups) {
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
+
+                at::CheckedFrom c = "deform_conv3d_forward_kernel";
+                std::vector<at::TensorArg> args;
+                args.reserve(5);
+                args.emplace_back(at::TensorArg(input, "input", 1));
+                args.emplace_back(at::TensorArg(weight, "weight", 2));
+                if (deformable)
+                    args.emplace_back(at::TensorArg(offset.value(), "offset", 3));
+                if (modulated)
+                    args.emplace_back(at::TensorArg(mask.value(), "mask", 4));
+                if (with_bias)
+                    args.emplace_back(at::TensorArg(bias.value(), "bias", 5));
+                at::checkAllSameGPUExceptUndefined(c, args);
+                at::checkAllSameTypeExceptUndefined(c, args);
+
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
+
+                TORCH_CHECK(input_c.ndimension() == 5)
+                TORCH_CHECK(weight_c.ndimension() == 5)
+                TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
+                TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_d = input_c.size(2);
+                int64_t in_h = input_c.size(3);
+                int64_t in_w = input_c.size(4);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_d = weight_c.size(2);
+                int64_t weight_h = weight_c.size(3);
+                int64_t weight_w = weight_c.size(4);
+
+                int64_t stride_d = stride[0];
+                int64_t stride_h = stride[1];
+                int64_t stride_w = stride[2];
+
+                int64_t pad_d = padding[0];
+                int64_t pad_h = padding[1];
+                int64_t pad_w = padding[2];
+
+                int64_t dilation_d = dilation[0];
+                int64_t dilation_h = dilation[1];
+                int64_t dilation_w = dilation[2];
+
+                int64_t out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
+                int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                TORCH_CHECK(
+                        weight_d > 0 && weight_h > 0 && weight_w > 0,
+                        "weight_d: ",
                         weight_d,
+                        " weight_h: ",
                         weight_h,
-                        weight_w,
+                        " weight_w: ",
+                        weight_w)
+                TORCH_CHECK(
+                        stride_d > 0 && stride_h > 0 && stride_w > 0,
+                        " stride_d: ",
                         stride_d,
+                        "stride_h: ",
                         stride_h,
-                        stride_w,
+                        " stride_w: ",
+                        stride_w)
+                TORCH_CHECK(
+                        pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
+                        "pad_d: ",
                         pad_d,
+                        " pad_h: ",
                         pad_h,
-                        pad_w,
+                        " pad_w: ",
+                        pad_w)
+                TORCH_CHECK(
+                        dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
+                        "dilation_d: ",
                         dilation_d,
+                        " dilation_h: ",
                         dilation_h,
-                        dilation_w,
+                        " dilation_w: ",
+                        dilation_w)
+
+                TORCH_CHECK(weight_c.size(1) * groups == in_channels)
+                TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+                int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
+
+                TORCH_CHECK(
+                        !deformable || offset_c.size(0) == input_c.size(0),
+                        "invalid batch size of offset")
+                TORCH_CHECK(
+                        !deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                        offset_c.size(1),
+                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                        3 * weight_d * weight_h * weight_w)
+                TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
+                        "offset.shape[1] is not valid. got: ",
+                        offset_c.size(1),
+                        " expected: ",
+                        offset_groups * 3 * weight_d * weight_h * weight_w)
+                TORCH_CHECK(
+                        !deformable || (offset_c.size(2) == out_d &&
+                                        offset_c.size(3) == out_h &&
+                                        offset_c.size(4) == out_w),
+                        "offset output dims: (",
+                        offset_c.size(2),
+                        ", ",
+                        offset_c.size(3),
+                        ", ",
+                        offset_c.size(4),
+                        ") - ",
+                        "computed output dims: (",
                         out_d,
+                        ", ",
                         out_h,
+                        ", ",
                         out_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        columns_view);
+                        ")")
 
-                for (int64_t g = 0; g < groups; g++) {
-                    output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                }
-            }
+                TORCH_CHECK(
+                        !modulated || mask_c.size(0) == input_c.size(0),
+                        "invalid batch size of mask")
+                TORCH_CHECK(
+                        !modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                        mask_c.size(1),
+                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                        weight_d * weight_h * weight_w)
+                TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
+                        "mask.shape[1] is not valid. got: ",
+                        mask_c.size(1),
+                        " expected: ",
+                        mask_groups * weight_d * weight_h * weight_w)
+                TORCH_CHECK(
+                        !modulated || (mask_c.size(2) == out_d &&
+                                       mask_c.size(3) == out_h &&
+                                       mask_c.size(4) == out_w),
+                        "mask output dims: (",
+                        mask_c.size(2),
+                        ", ",
+                        mask_c.size(3),
+                        ", ",
+                        mask_c.size(4),
+                        ") - ",
+                        "computed output dims: (",
+                        out_d,
+                        ", ",
+                        out_h,
+                        ", ",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        out_d > 0 && out_h > 0 && out_w > 0,
+                        "Calculated output size too small - out_d: ",
+                        out_d,
+                        " out_h: ",
+                        out_h,
+                        " out_w: ",
+                        out_w)
+
+                auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
 
-            output_buf = output_buf.view({batch_sz / n_parallel_imgs,
-                                          out_channels,
+                // Separate batches into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_d,
+                                        in_h,
+                                        in_w});
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_d,
+                                              weight_h,
+                                              weight_w,
+                                              3,
+                                              out_d,
+                                              out_h,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0, 0, 0});
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
+                                          mask_groups,
+                                          weight_d,
+                                          weight_h,
+                                          weight_w,
                                           out_d,
                                           out_h,
                                           out_w});
-            output_buf.transpose_(1, 2);
-            output.copy_(output_buf);
-            output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
-            if (with_bias)
-                output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0});
 
-            return output;
-        }
+                output = output.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      out_channels,
+                                      out_d,
+                                      out_h,
+                                      out_w});
+                auto output_buf = at::zeros(
+                        {batch_sz / n_parallel_imgs,
+                         out_channels,
+                         n_parallel_imgs,
+                         out_d,
+                         out_h,
+                         out_w},
+                        output.options());
+
+                // Separate channels into convolution groups
+                output_buf = output_buf.view({output_buf.size(0),
+                                              groups,
+                                              output_buf.size(1) / groups,
+                                              output_buf.size(2),
+                                              output_buf.size(3),
+                                              output_buf.size(4),
+                                              output_buf.size(5)});
+                weight_c = weight_c.view({groups,
+                                          weight_c.size(0) / groups,
+                                          weight_c.size(1),
+                                          weight_c.size(2),
+                                          weight_c.size(3),
+                                          weight_c.size(4)});
+
+                // Sample points and perform convolution
+                auto columns = at::empty({groups,
+                                          in_channels * weight_d * weight_h * weight_w / groups,
+                                          n_parallel_imgs * out_d * out_h * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_d,
+                                                  weight_h,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_d,
+                                                  out_h,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    vol2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_d,
+                            in_h,
+                            in_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            out_d,
+                            out_h,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
+
+                    for (int64_t g = 0; g < groups; g++) {
+                        output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    }
+                }
+
+                output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                              out_channels,
+                                              n_parallel_imgs,
+                                              out_d,
+                                              out_h,
+                                              out_w});
+                output_buf.transpose_(1, 2);
+                output.copy_(output_buf);
+                output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+                if (with_bias)
+                    output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
+
+                return output;
+            }
 
-        namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-            _deform_conv3d_backward(
+            deform_conv3d_backward_kernel(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
-                    const at::Tensor &offset,
-                    const at::Tensor &mask,
-                    const at::Tensor &bias,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef dilation,
                     int64_t groups) {
-                bool deformable = offset.defined() && offset.numel();
-                bool modulated = mask.defined() && mask.numel();
-                bool with_bias = bias.defined() && bias.numel();
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
 
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
-                at::Tensor offset_c = offset.contiguous();
-                at::Tensor mask_c = mask.contiguous();
-                at::Tensor bias_c = bias.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
 
                 int64_t batch_sz = input_c.size(0);
                 int64_t in_channels = input_c.size(1);
                 int64_t in_d = input_c.size(2);
                 int64_t in_h = input_c.size(3);
                 int64_t in_w = input_c.size(4);
 
@@ -443,16 +450,16 @@
                 int64_t dilation_h = dilation[1];
                 int64_t dilation_w = dilation[2];
 
                 int64_t out_d = (in_d + 2 * pad_d - (dilation_d * (weight_d - 1) + 1)) / stride_d + 1;
                 int64_t out_h = (in_h + 2 * pad_h - (dilation_h * (weight_h - 1) + 1)) / stride_h + 1;
                 int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
-                int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
+                int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
                 auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
 
@@ -658,129 +665,24 @@
                     for (int64_t g = 0; g < groups; g++) {
                         grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                     }
                 }
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
-                grad_offset = grad_offset.view_as(offset);
-                grad_mask = grad_mask.view_as(mask);
+                grad_offset = deformable ? grad_offset.view_as(offset.value()) : at::Tensor();
+                grad_mask = modulated ? grad_mask.view_as(mask.value()) : at::Tensor();
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
-        class DeformConv3dFunction
-                : public torch::autograd::Function<DeformConv3dFunction> {
-        public:
-            static torch::autograd::variable_list forward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::Variable &input,
-                    const torch::autograd::Variable &weight,
-                    const torch::autograd::Variable &offset,
-                    const torch::autograd::Variable &mask,
-                    const torch::autograd::Variable &bias,
-                    at::IntArrayRef stride,
-                    at::IntArrayRef padding,
-                    at::IntArrayRef dilation,
-                    int64_t groups) {
-                at::AutoDispatchBelowADInplaceOrView g;
-                auto output = deform_conv3d_forward(
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        dilation,
-                        groups);
-
-                ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride.vec();
-                ctx->saved_data["padding"] = padding.vec();
-                ctx->saved_data["dilation"] = dilation.vec();
-                ctx->saved_data["groups"] = groups;
-
-                return {
-                        output,
-                };
-            }
-
-            static torch::autograd::variable_list backward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::variable_list &grad_output) {
-                auto saved = ctx->get_saved_variables();
-                auto input = saved[0];
-                auto weight = saved[1];
-                auto offset = saved[2];
-                auto mask = saved[3];
-                auto bias = saved[4];
-
-                auto stride = ctx->saved_data["stride"].toIntVector();
-                auto padding = ctx->saved_data["padding"].toIntVector();
-                auto dilation = ctx->saved_data["dilation"].toIntVector();
-                auto groups = ctx->saved_data["groups"].toInt();
-
-                auto grads = detail::_deform_conv3d_backward(
-                        grad_output[0],
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        dilation,
-                        groups);
-                auto grad_input = std::get<0>(grads);
-                auto grad_weight = std::get<1>(grads);
-                auto grad_offset = std::get<2>(grads);
-                auto grad_mask = std::get<3>(grads);
-                auto grad_bias = std::get<4>(grads);
-
-                return {
-                        grad_input,
-                        grad_weight,
-                        grad_offset,
-                        grad_mask,
-                        grad_bias,
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                };
-            }
-        };
-
-        at::Tensor deform_conv3d(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::optional<at::Tensor> &offset = {},
-                const at::optional<at::Tensor> &mask = {},
-                const at::optional<at::Tensor> &bias = {},
-                at::IntArrayRef stride = 1,
-                at::IntArrayRef padding = 0,
-                at::IntArrayRef dilation = 1,
-                int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv.deform_conv3d")
-            auto result = DeformConv3dFunction::apply(
-                    input,
-                    weight,
-                    offset.value_or(input.new_zeros(0)),
-                    mask.value_or(input.new_zeros(0)),
-                    bias.value_or(input.new_zeros(0)),
-                    stride,
-                    padding,
-                    dilation,
-                    groups);
-            return result[0];
-        }
-
-        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
-            m.def("tvdcn::deform_conv3d(Tensor input, Tensor weight, "
-                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
-                  "int[3] stride=1, int[3] padding=0, int[3] dilation=1, int groups=1) -> Tensor",
-                  &deform_conv3d);
+        TORCH_LIBRARY_IMPL(tvdcn, CUDA, m) {
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::deform_conv3d"),
+                    TORCH_FN(deform_conv3d_forward_kernel));
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::_deform_conv3d_backward"),
+                    TORCH_FN(deform_conv3d_backward_kernel));
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose1d.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv1d_kernel.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -65,560 +65,458 @@
 
 // modified from
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
-#include <torch/autograd.h>
+#include <ATen/ATen.h>
+#include <torch/library.h>
 
-#include "dispatch/deform_conv1d_kernels.h"
-#include "utils/parallel_helpers.h"
-#include "utils/tensor_utils.h"
+#include "deform_conv1d_common_kernels.h"
+#include "../utils/parallel_helpers.h"
+#include "../utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv_transpose1d_forward(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                at::IntArrayRef stride,
-                at::IntArrayRef padding,
-                at::IntArrayRef output_padding,
-                at::IntArrayRef dilation,
-                int64_t groups) {
-            at::CheckedFrom c = "deform_conv_transpose2d_forward";
-            auto args = {
-                    at::TensorArg(input, "input", 1),
-                    at::TensorArg(weight, "weight", 2),
-                    at::TensorArg(offset, "offset", 3),
-                    at::TensorArg(mask, "mask", 4),
-                    at::TensorArg(bias, "bias", 5)};
-            at::checkAllSameType(c, args);
-            at::checkAllSameDevice(c, args);
-
-            bool deformable = offset.defined() && offset.numel();
-            bool modulated = mask.defined() && mask.numel();
-            bool with_bias = bias.defined() && bias.numel();
-
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            TORCH_CHECK(input_c.ndimension() == 3)
-            TORCH_CHECK(weight_c.ndimension() == 3)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
-
-            int64_t batch_sz = input_c.size(0);
-            int64_t in_channels = input_c.size(1);
-            int64_t in_w = input_c.size(2);
-
-            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int64_t out_channels = weight_c.size(1) * groups;
-            int64_t weight_w = weight_c.size(2);
-
-            int64_t stride_w = stride[0];
-
-            int64_t pad_w = padding[0];
-
-            int64_t out_pad_w = output_padding[0];
-
-            int64_t dilation_w = dilation[0];
-
-            int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
-
-            TORCH_CHECK(
-                    weight_w > 0,
-                    " weight_w: ",
-                    weight_w)
-            TORCH_CHECK(
-                    stride_w > 0,
-                    " stride_w: ",
-                    stride_w)
-            TORCH_CHECK(
-                    pad_w >= 0,
-                    " pad_w: ",
-                    pad_w)
-            TORCH_CHECK(
-                    dilation_w > 0,
-                    " dilation_w: ",
-                    dilation_w)
-
-            TORCH_CHECK(weight_c.size(1) * groups == out_channels)
-            TORCH_CHECK(weight_c.size(0) % groups == 0)
-
-            int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
-            int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
-
-            TORCH_CHECK(
-                    !deformable || offset_c.size(0) == input_c.size(0),
-                    "invalid batch size of offset")
-            TORCH_CHECK(
-                    !deformable || offset_groups > 0,
-                    "The shape of the offset tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2).\nGot offset.size(1)=",
-                    offset.size(1),
-                    ", while weight.size(2)=",
-                    weight_w)
-            TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(1) == offset_groups * weight_w,
-                    "offset.shape[1] is not valid. got: ",
-                    offset_c.size(1),
-                    " expected: ",
-                    offset_groups * weight_w)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(2) == in_w,
-                    "offset output dims: (",
-                    offset_c.size(2),
-                    ") - ",
-                    "input dims: (",
-                    in_w,
-                    ")")
-
-            TORCH_CHECK(
-                    !modulated || mask_c.size(0) == input_c.size(0),
-                    "invalid batch size of mask")
-            TORCH_CHECK(
-                    !modulated || mask_groups > 0,
-                    "The shape of the mask tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2).\nGot mask.size(1)=",
-                    mask.size(1),
-                    ", while weight.size(2)=",
-                    weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(1) == mask_groups * weight_w,
-                    "mask.shape[1] is not valid. got: ",
-                    mask_c.size(1),
-                    " expected: ",
-                    mask_groups * weight_w)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(2) == in_w,
-                    "mask output dims: (",
-                    mask_c.size(2),
-                    ") - ",
-                    "input dims: (",
-                    in_w,
-                    ")")
-
-            TORCH_CHECK(
-                    out_w > 0,
-                    "Calculated output size too small - out_w: ",
-                    out_w)
-
-            auto output = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
-
-            // Separate batches into blocks
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_w});
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+        using namespace cpu;
+
+        namespace {
+            at::Tensor deform_conv1d_forward_kernel(
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups) {
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
+
+                at::CheckedFrom c = "deform_conv1d_forward_kernel";
+                std::vector<at::TensorArg> args;
+                args.reserve(5);
+                args.emplace_back(at::TensorArg(input, "input", 1));
+                args.emplace_back(at::TensorArg(weight, "weight", 2));
+                if (deformable)
+                    args.emplace_back(at::TensorArg(offset.value(), "offset", 3));
+                if (modulated)
+                    args.emplace_back(at::TensorArg(mask.value(), "mask", 4));
+                if (with_bias)
+                    args.emplace_back(at::TensorArg(bias.value(), "bias", 5));
+                at::checkDeviceTypeExceptUndefined(c, args, at::kCPU);
+                at::checkAllSameTypeExceptUndefined(c, args);
+
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
+
+                TORCH_CHECK(input_c.ndimension() == 3)
+                TORCH_CHECK(weight_c.ndimension() == 3)
+                TORCH_CHECK(!deformable || offset_c.ndimension() == 3)
+                TORCH_CHECK(!modulated || mask_c.ndimension() == 3)
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_w = input_c.size(2);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(0);
+                int64_t weight_w = weight_c.size(2);
+
+                int64_t stride_w = stride[0];
+
+                int64_t pad_w = padding[0];
+
+                int64_t dilation_w = dilation[0];
+
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
+
+                TORCH_CHECK(
+                        weight_w > 0,
+                        " weight_w: ",
+                        weight_w)
+                TORCH_CHECK(
+                        stride_w > 0,
+                        " stride_w: ",
+                        stride_w)
+                TORCH_CHECK(
+                        pad_w >= 0,
+                        " pad_w: ",
+                        pad_w)
+                TORCH_CHECK(
+                        dilation_w > 0,
+                        " dilation_w: ",
+                        dilation_w)
+
+                TORCH_CHECK(weight_c.size(1) * groups == in_channels)
+                TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+                int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
+
+                TORCH_CHECK(
+                        !deformable || offset_c.size(0) == input_c.size(0),
+                        "invalid batch size of offset")
+                TORCH_CHECK(
+                        !deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot offset.size(1)=",
+                        offset_c.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
+                TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(1) == offset_groups * weight_w,
+                        "offset.shape[1] is not valid. got: ",
+                        offset_c.size(1),
+                        " expected: ",
+                        offset_groups * weight_w)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(2) == out_w,
+                        "offset output dims: (",
+                        offset_c.size(2),
+                        ") - ",
+                        "computed output dims: (",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        !modulated || mask_c.size(0) == input_c.size(0),
+                        "invalid batch size of mask")
+                TORCH_CHECK(
+                        !modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2).\nGot mask.size(1)=",
+                        mask_c.size(1),
+                        ", while weight.size(2)=",
+                        weight_w)
+                TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(1) == mask_groups * weight_w,
+                        "mask.shape[1] is not valid. got: ",
+                        mask_c.size(1),
+                        " expected: ",
+                        mask_groups * weight_w)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(2) == out_w,
+                        "mask output dims: (",
+                        mask_c.size(2),
+                        ") - ",
+                        "computed output dims: (",
+                        out_w,
+                        ")")
+
+                TORCH_CHECK(
+                        out_w > 0,
+                        "Calculated output size too small - out_w: ",
+                        out_w)
+
+                auto output = at::zeros({batch_sz, out_channels, out_w}, input_c.options());
+
+                // Separate batches into blocks
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        in_channels,
+                                        in_w});
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_w,
+                                              1,
+                                              out_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0});
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          offset_groups,
+                                          mask_groups,
                                           weight_w,
-                                          1,
-                                          in_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                          out_w});
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0});
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_w,
-                                      in_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          0, 0, 0});
+
+                output = output.view({batch_sz / n_parallel_imgs,
                                       n_parallel_imgs,
-                                      0, 0, 0});
+                                      out_channels,
+                                      out_w});
+                auto output_buf = at::zeros(
+                        {batch_sz / n_parallel_imgs,
+                         out_channels,
+                         n_parallel_imgs,
+                         out_w},
+                        output.options());
 
-            // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_w}).permute({0, 2, 3, 1, 4}).contiguous();
-            weight_c = weight_c.view({groups,
-                                      weight_c.size(0) / groups,
-                                      weight_c.size(1),
-                                      weight_c.size(2)});
-
-            // Sample points and perform convolution
-            auto columns = at::empty({groups,
-                                      out_channels * weight_w / groups,
-                                      n_parallel_imgs * in_w},
-                                     input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              in_w});
-            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int64_t g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
-                }
+                // Separate channels into convolution groups
+                output_buf = output_buf.view({output_buf.size(0),
+                                              groups,
+                                              output_buf.size(1) / groups,
+                                              output_buf.size(2),
+                                              output_buf.size(3)});
+                weight_c = weight_c.view({groups,
+                                          weight_c.size(0) / groups,
+                                          weight_c.size(1),
+                                          weight_c.size(2)});
 
-                auto output_b = output[b];
-                col2arr(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_w,
-                        weight_w,
-                        stride_w,
-                        pad_w,
-                        dilation_w,
-                        in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        output_b);
-            }
+                // Sample points and perform convolution
+                auto columns = at::empty({groups,
+                                          in_channels * weight_w / groups,
+                                          n_parallel_imgs * out_w},
+                                         input_c.options());
+                auto columns_view = columns.view({in_channels,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  out_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    arr2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
+                            in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            columns_view);
 
-            output = output.view({batch_sz, out_channels, out_w});
-            if (with_bias)
-                output.add_(bias_c.view({1, out_channels, 1}));
+                    for (int64_t g = 0; g < groups; g++) {
+                        output_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
+                    }
+                }
 
-            return output;
-        }
+                output_buf = output_buf.view({batch_sz / n_parallel_imgs,
+                                              out_channels,
+                                              n_parallel_imgs,
+                                              out_w});
+                output_buf.transpose_(1, 2);
+                output.copy_(output_buf);
+                output = output.view({batch_sz, out_channels, out_w});
+                if (with_bias)
+                    output.add_(bias_c.view({1, out_channels, 1}));
+
+                return output;
+            }
 
-        namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-            _deform_conv_transpose1d_backward(
+            deform_conv1d_backward_kernel(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
-                    const at::Tensor &offset,
-                    const at::Tensor &mask,
-                    const at::Tensor &bias,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
-                    at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
                     int64_t groups) {
-                bool deformable = offset.defined() && offset.numel();
-                bool modulated = mask.defined() && mask.numel();
-                bool with_bias = bias.defined() && bias.numel();
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
 
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
-                at::Tensor offset_c = offset.contiguous();
-                at::Tensor mask_c = mask.contiguous();
-                at::Tensor bias_c = bias.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
 
                 int64_t batch_sz = input_c.size(0);
                 int64_t in_channels = input_c.size(1);
                 int64_t in_w = input_c.size(2);
 
                 int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
-                int64_t out_channels = weight_c.size(1) * groups;
+                int64_t out_channels = weight_c.size(0);
                 int64_t weight_w = weight_c.size(2);
 
                 int64_t stride_w = stride[0];
 
                 int64_t pad_w = padding[0];
 
-                int64_t out_pad_w = output_padding[0];
-
                 int64_t dilation_w = dilation[0];
 
-                int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+                int64_t out_w = (in_w + 2 * pad_w - (dilation_w * (weight_w - 1) + 1)) / stride_w + 1;
 
-                int64_t offset_groups = deformable ? offset.size(1) / weight_w : 0;
-                int64_t mask_groups = modulated ? mask.size(1) / weight_w : 0;
+                int64_t offset_groups = deformable ? offset_c.size(1) / weight_w : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / weight_w : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
                 auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
-                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
-                                              n_parallel_imgs,
-                                              out_channels,
-                                              out_w});
-
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
                                         in_w});
                 grad_input = grad_input.view_as(input_c);
                 if (deformable)
                     offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               offset_groups,
                                               weight_w,
                                               1,
-                                              in_w});
+                                              out_w});
                 else
                     offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               0, 0, 0, 0});
                 grad_offset = grad_offset.view_as(offset_c);
                 if (modulated)
                     mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           mask_groups,
                                           weight_w,
-                                          in_w});
+                                          out_w});
                 else
                     mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           0, 0, 0});
                 grad_mask = grad_mask.view_as(mask_c);
 
-                auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
-                                                 in_channels,
-                                                 n_parallel_imgs,
-                                                 in_w}, input_c.options());
-
                 // Separate channels into convolution groups
-                input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                        n_parallel_imgs,
-                                        groups,
-                                        in_channels / groups,
-                                        in_w}).permute({0, 2, 3, 1, 4}).contiguous();
-
-                grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
-                                                      groups,
-                                                      grad_input_buf.size(1) / groups,
-                                                      grad_input_buf.size(2),
-                                                      grad_input_buf.size(3)});
+                grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              groups,
+                                              out_channels / groups,
+                                              out_w}).permute({0, 2, 3, 1, 4}).contiguous();
 
                 weight_c = weight_c.view({groups,
-                                          in_channels / groups,
                                           out_channels / groups,
+                                          in_channels / groups,
                                           weight_w});
                 grad_weight = grad_weight.view_as(weight_c);
 
                 auto columns = at::empty({groups,
-                                          out_channels * weight_w / groups,
-                                          n_parallel_imgs * in_w},
+                                          in_channels * weight_w / groups,
+                                          n_parallel_imgs * out_w},
                                          input_c.options());
-                auto columns_view = columns.view({out_channels,
+                auto columns_view = columns.view({in_channels,
                                                   weight_w,
                                                   n_parallel_imgs,
-                                                  in_w});
+                                                  out_w});
                 for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                     columns.zero_();
                     for (int64_t g = 0; g < groups; g++) {
-                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), grad_out_c[b][g].flatten(1));
                     }
 
                     auto grad_offset_b = grad_offset[b];
                     deform_conv1d_compute_grad_offset(
                             columns_view,
-                            grad_out_c[b],
+                            input_c[b],
                             offset_c[b],
                             mask_c[b],
-                            out_channels,
-                            out_w,
+                            in_channels,
+                            in_w,
                             weight_w,
                             stride_w,
                             pad_w,
                             dilation_w,
-                            in_w,
+                            out_w,
                             n_parallel_imgs,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
                             grad_offset_b);
 
                     auto grad_mask_b = grad_mask[b];
                     deform_conv1d_compute_grad_mask(
                             columns_view,
-                            grad_out_c[b],
+                            input_c[b],
                             offset_c[b],
-                            out_channels,
-                            out_w,
+                            in_channels,
+                            in_w,
                             weight_w,
                             stride_w,
                             pad_w,
                             dilation_w,
-                            in_w,
+                            out_w,
                             n_parallel_imgs,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
                             grad_mask_b);
 
-                    arr2col(
-                            grad_out_c[b],
+                    auto grad_input_b = grad_input[b];
+                    col2arr(
+                            columns_view,
                             offset_c[b],
                             mask_c[b],
-                            out_channels,
-                            out_w,
+                            in_channels,
+                            in_w,
                             weight_w,
                             stride_w,
                             pad_w,
                             dilation_w,
+                            out_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            grad_input_b);
+
+                    arr2col(
+                            input_c[b],
+                            offset_c[b],
+                            mask_c[b],
+                            in_channels,
                             in_w,
+                            weight_w,
+                            stride_w,
+                            pad_w,
+                            dilation_w,
+                            out_w,
                             n_parallel_imgs,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
                             columns_view);
 
                     for (int64_t g = 0; g < groups; g++) {
-                        grad_input_buf[b][g].flatten(1).addmm_(weight_c[g].flatten(1), columns[g]);
-                        grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
+                        grad_weight[g].flatten(1).addmm_(grad_out_c[b][g].flatten(1), columns[g].transpose(1, 0));
                     }
                 }
 
-                grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
-                                                      in_channels,
-                                                      n_parallel_imgs,
-                                                      in_w}).transpose_(1, 2);
-                grad_input.copy_(grad_input_buf);
-
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
-                grad_offset = grad_offset.view_as(offset);
-                grad_mask = grad_mask.view_as(mask);
+                grad_offset = deformable ? grad_offset.view_as(offset.value()) : at::Tensor();
+                grad_mask = modulated ? grad_mask.view_as(mask.value()) : at::Tensor();
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
-        class DeformConvTranspose1dFunction
-                : public torch::autograd::Function<DeformConvTranspose1dFunction> {
-        public:
-            static torch::autograd::variable_list forward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::Variable &input,
-                    const torch::autograd::Variable &weight,
-                    const torch::autograd::Variable &offset,
-                    const torch::autograd::Variable &mask,
-                    const torch::autograd::Variable &bias,
-                    at::IntArrayRef stride,
-                    at::IntArrayRef padding,
-                    at::IntArrayRef output_padding,
-                    at::IntArrayRef dilation,
-                    int64_t groups) {
-                at::AutoDispatchBelowADInplaceOrView g;
-                auto output = deform_conv_transpose1d_forward(
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        output_padding,
-                        dilation,
-                        groups);
-
-                ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride.vec();
-                ctx->saved_data["padding"] = padding.vec();
-                ctx->saved_data["output_padding"] = output_padding.vec();
-                ctx->saved_data["dilation"] = dilation.vec();
-                ctx->saved_data["groups"] = groups;
-
-                return {
-                        output,
-                };
-            }
-
-            static torch::autograd::variable_list backward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::variable_list &grad_output) {
-                auto saved = ctx->get_saved_variables();
-                auto input = saved[0];
-                auto weight = saved[1];
-                auto offset = saved[2];
-                auto mask = saved[3];
-                auto bias = saved[4];
-
-                auto stride = ctx->saved_data["stride"].toIntVector();
-                auto padding = ctx->saved_data["padding"].toIntVector();
-                auto output_padding = ctx->saved_data["output_padding"].toIntVector();
-                auto dilation = ctx->saved_data["dilation"].toIntVector();
-                auto groups = ctx->saved_data["groups"].toInt();
-
-                auto grads = detail::_deform_conv_transpose1d_backward(
-                        grad_output[0],
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        output_padding,
-                        dilation,
-                        groups);
-                auto grad_input = std::get<0>(grads);
-                auto grad_weight = std::get<1>(grads);
-                auto grad_offset = std::get<2>(grads);
-                auto grad_mask = std::get<3>(grads);
-                auto grad_bias = std::get<4>(grads);
-
-                return {
-                        grad_input,
-                        grad_weight,
-                        grad_offset,
-                        grad_mask,
-                        grad_bias,
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                };
-            }
-        };
-
-        at::Tensor deform_conv_transpose1d(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::optional<at::Tensor> &offset = {},
-                const at::optional<at::Tensor> &mask = {},
-                const at::optional<at::Tensor> &bias = {},
-                at::IntArrayRef stride = 1,
-                at::IntArrayRef padding = 0,
-                at::IntArrayRef output_padding = 0,
-                at::IntArrayRef dilation = 1,
-                int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose1d")
-            auto result = DeformConvTranspose1dFunction::apply(
-                    input,
-                    weight,
-                    offset.value_or(input.new_zeros(0)),
-                    mask.value_or(input.new_zeros(0)),
-                    bias.value_or(input.new_zeros(0)),
-                    stride,
-                    padding,
-                    output_padding,
-                    dilation,
-                    groups);
-            return result[0];
-        }
-
-        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
-            m.def("tvdcn::deform_conv_transpose1d(Tensor input, Tensor weight, "
-                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
-                  "int[1] stride=1, int[1] padding=0, int[1] output_padding=0, "
-                  "int[1] dilation=1, int groups=1) -> Tensor",
-                  &deform_conv_transpose1d);
+        TORCH_LIBRARY_IMPL(tvdcn, CPU, m) {
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::deform_conv1d"),
+                    TORCH_FN(deform_conv1d_forward_kernel));
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::_deform_conv1d_backward"),
+                    TORCH_FN(deform_conv1d_backward_kernel));
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose2d.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cpu/deform_conv_transpose3d_kernel.cpp`

 * *Files 10% similar despite different names*

```diff
@@ -67,490 +67,575 @@
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
 
-#include "dispatch/deform_conv2d_kernels.h"
-#include "utils/parallel_helpers.h"
-#include "utils/tensor_utils.h"
+#include "deform_conv3d_common_kernels.h"
+#include "../utils/parallel_helpers.h"
+#include "../utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv_transpose2d_forward(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                at::IntArrayRef stride,
-                at::IntArrayRef padding,
-                at::IntArrayRef output_padding,
-                at::IntArrayRef dilation,
-                int64_t groups) {
-            at::CheckedFrom c = "deform_conv_transpose2d_forward";
-            auto args = {
-                    at::TensorArg(input, "input", 1),
-                    at::TensorArg(weight, "weight", 2),
-                    at::TensorArg(offset, "offset", 3),
-                    at::TensorArg(mask, "mask", 4),
-                    at::TensorArg(bias, "bias", 5)};
-            at::checkAllSameType(c, args);
-            at::checkAllSameDevice(c, args);
-
-            bool deformable = offset.defined() && offset.numel();
-            bool modulated = mask.defined() && mask.numel();
-            bool with_bias = bias.defined() && bias.numel();
-
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            TORCH_CHECK(input_c.ndimension() == 4)
-            TORCH_CHECK(weight_c.ndimension() == 4)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 4)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 4)
-
-            int64_t batch_sz = input_c.size(0);
-            int64_t in_channels = input_c.size(1);
-            int64_t in_h = input_c.size(2);
-            int64_t in_w = input_c.size(3);
-
-            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int64_t out_channels = weight_c.size(1) * groups;
-            int64_t weight_h = weight_c.size(2);
-            int64_t weight_w = weight_c.size(3);
-
-            int64_t stride_h = stride[0];
-            int64_t stride_w = stride[1];
-
-            int64_t pad_h = padding[0];
-            int64_t pad_w = padding[1];
-
-            int64_t out_pad_h = output_padding[0];
-            int64_t out_pad_w = output_padding[1];
-
-            int64_t dilation_h = dilation[0];
-            int64_t dilation_w = dilation[1];
-
-            int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
-
-            TORCH_CHECK(
-                    weight_h > 0 && weight_w > 0,
-                    "weight_h: ",
-                    weight_h,
-                    " weight_w: ",
-                    weight_w)
-            TORCH_CHECK(
-                    stride_h > 0 && stride_w > 0,
-                    "stride_h: ",
-                    stride_h,
-                    " stride_w: ",
-                    stride_w)
-            TORCH_CHECK(
-                    pad_h >= 0 && pad_w >= 0,
-                    "pad_h: ",
-                    pad_h,
-                    " pad_w: ",
-                    pad_w)
-            TORCH_CHECK(
-                    dilation_h > 0 && dilation_w > 0,
-                    "dilation_h: ",
-                    dilation_h,
-                    " dilation_w: ",
-                    dilation_w)
-
-            TORCH_CHECK(weight_c.size(1) * groups == out_channels)
-            TORCH_CHECK(weight_c.size(0) % groups == 0)
-
-            int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
-            int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
-
-            TORCH_CHECK(
-                    !deformable || offset_c.size(0) == input_c.size(0),
-                    "invalid batch size of offset")
-            TORCH_CHECK(
-                    !deformable || offset_groups > 0,
-                    "The shape of the offset tensor at dimension 1 is not valid. It should "
-                    "be a multiple of 2 * weight.size(2) * weight.size(3).\nGot offset.size(1)=",
-                    offset.size(1),
-                    ", while 2 * weight.size(2) * weight.size(3)=",
-                    2 * weight_h * weight_w)
-            TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(1) == offset_groups * 2 * weight_h * weight_w,
-                    "offset.shape[1] is not valid. got: ",
-                    offset_c.size(1),
-                    " expected: ",
-                    offset_groups * 2 * weight_h * weight_w)
-            TORCH_CHECK(
-                    !deformable || (offset_c.size(2) == in_h &&
-                                    offset_c.size(3) == in_w),
-                    "offset input dims: (",
-                    offset_c.size(2),
-                    ", ",
-                    offset_c.size(3),
-                    ") - ",
-                    "input dims: (",
-                    in_h,
-                    ", ",
-                    in_w,
-                    ")")
-
-            TORCH_CHECK(
-                    !modulated || mask_c.size(0) == input_c.size(0),
-                    "invalid batch size of mask")
-            TORCH_CHECK(
-                    !modulated || mask_groups > 0,
-                    "The shape of the mask tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2) * weight.size(3).\nGot mask.size(1)=",
-                    mask.size(1),
-                    ", while weight.size(2) * weight.size(3)=",
-                    weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(1) == mask_groups * weight_h * weight_w,
-                    "mask.shape[1] is not valid. got: ",
-                    mask_c.size(1),
-                    " expected: ",
-                    mask_groups * weight_h * weight_w)
-            TORCH_CHECK(
-                    !modulated || (mask_c.size(2) == in_h &&
-                                   mask_c.size(3) == in_w),
-                    "mask input dims: (",
-                    mask_c.size(2),
-                    ", ",
-                    mask_c.size(3),
-                    ") - ",
-                    "input dims: (",
-                    in_h,
-                    ", ",
-                    in_w,
-                    ")")
-
-            TORCH_CHECK(
-                    out_h > 0 && out_w > 0,
-                    "Calculated output size too small - out_h: ",
-                    out_h,
-                    " out_w: ",
-                    out_w)
-
-            auto output = at::zeros({batch_sz, out_channels, out_h, out_w}, input_c.options());
-
-            // Separate batches into blocks
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_h,
-                                  out_w});
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          offset_groups,
-                                          weight_h,
-                                          weight_w,
-                                          2,
-                                          in_h,
-                                          in_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0});
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_h,
-                                      weight_w,
-                                      in_h,
-                                      in_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0});
+        using namespace cpu;
 
-            // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_h,
-                                    in_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
-            weight_c = weight_c.view({groups,
-                                      weight_c.size(0) / groups,
-                                      weight_c.size(1),
-                                      weight_c.size(2),
-                                      weight_c.size(3)});
-
-            // Sample points and perform convolution
-            auto columns = at::empty({groups,
-                                      out_channels * weight_h * weight_w / groups,
-                                      n_parallel_imgs * in_h * in_w},
-                                     input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_h,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              in_h,
-                                              in_w});
-            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int64_t g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
-                }
+        namespace {
+            at::Tensor deform_conv_transpose3d_forward_kernel(
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups) {
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
+
+                at::CheckedFrom c = "deform_conv_transpose3d_forward_kernel";
+                std::vector<at::TensorArg> args;
+                args.reserve(5);
+                args.emplace_back(at::TensorArg(input, "input", 1));
+                args.emplace_back(at::TensorArg(weight, "weight", 2));
+                if (deformable)
+                    args.emplace_back(at::TensorArg(offset.value(), "offset", 3));
+                if (modulated)
+                    args.emplace_back(at::TensorArg(mask.value(), "mask", 4));
+                if (with_bias)
+                    args.emplace_back(at::TensorArg(bias.value(), "bias", 5));
+                at::checkDeviceTypeExceptUndefined(c, args, at::kCPU);
+                at::checkAllSameTypeExceptUndefined(c, args);
 
-                auto output_b = output[b];
-                col2im(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_h,
-                        out_w,
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
+
+                TORCH_CHECK(input_c.ndimension() == 5)
+                TORCH_CHECK(weight_c.ndimension() == 5)
+                TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
+                TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_d = input_c.size(2);
+                int64_t in_h = input_c.size(3);
+                int64_t in_w = input_c.size(4);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(1) * groups;
+                int64_t weight_d = weight_c.size(2);
+                int64_t weight_h = weight_c.size(3);
+                int64_t weight_w = weight_c.size(4);
+
+                int64_t stride_d = stride[0];
+                int64_t stride_h = stride[1];
+                int64_t stride_w = stride[2];
+
+                int64_t pad_d = padding[0];
+                int64_t pad_h = padding[1];
+                int64_t pad_w = padding[2];
+
+                int64_t out_pad_d = output_padding[0];
+                int64_t out_pad_h = output_padding[1];
+                int64_t out_pad_w = output_padding[2];
+
+                int64_t dilation_d = dilation[0];
+                int64_t dilation_h = dilation[1];
+                int64_t dilation_w = dilation[2];
+
+                int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
+                int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+                int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+
+                TORCH_CHECK(
+                        weight_d > 0 && weight_h > 0 && weight_w > 0,
+                        "weight_d: ",
+                        weight_d,
+                        " weight_h: ",
                         weight_h,
-                        weight_w,
+                        " weight_w: ",
+                        weight_w)
+                TORCH_CHECK(
+                        stride_d > 0 && stride_h > 0 && stride_w > 0,
+                        " stride_d: ",
+                        stride_d,
+                        "stride_h: ",
                         stride_h,
-                        stride_w,
+                        " stride_w: ",
+                        stride_w)
+                TORCH_CHECK(
+                        pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
+                        "pad_d: ",
+                        pad_d,
+                        " pad_h: ",
                         pad_h,
-                        pad_w,
+                        " pad_w: ",
+                        pad_w)
+                TORCH_CHECK(
+                        dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
+                        "dilation_d: ",
+                        dilation_d,
+                        " dilation_h: ",
                         dilation_h,
-                        dilation_w,
+                        " dilation_w: ",
+                        dilation_w)
+
+                TORCH_CHECK(weight_c.size(1) * groups == out_channels)
+                TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+                int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
+
+                TORCH_CHECK(
+                        !deformable || offset_c.size(0) == input_c.size(0),
+                        "invalid batch size of offset")
+                TORCH_CHECK(
+                        !deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                        offset_c.size(1),
+                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                        3 * weight_d * weight_h * weight_w)
+                TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
+                        "offset.shape[1] is not valid. got: ",
+                        offset_c.size(1),
+                        " expected: ",
+                        offset_groups * 3 * weight_d * weight_h * weight_w)
+                TORCH_CHECK(
+                        !deformable || (offset_c.size(2) == in_d &&
+                                        offset_c.size(3) == in_h &&
+                                        offset_c.size(4) == in_w),
+                        "offset input dims: (",
+                        offset_c.size(2),
+                        ", ",
+                        offset_c.size(3),
+                        ", ",
+                        offset_c.size(4),
+                        ") - ",
+                        "input dims: (",
+                        in_d,
+                        ", ",
                         in_h,
+                        ", ",
                         in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        output_b);
-            }
+                        ")")
 
-            output = output.view({batch_sz, out_channels, out_h, out_w});
-            if (with_bias)
-                output.add_(bias_c.view({1, out_channels, 1, 1}));
+                TORCH_CHECK(
+                        !modulated || mask_c.size(0) == input_c.size(0),
+                        "invalid batch size of mask")
+                TORCH_CHECK(
+                        !modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                        mask_c.size(1),
+                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                        weight_d * weight_h * weight_w)
+                TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
+                        "mask.shape[1] is not valid. got: ",
+                        mask_c.size(1),
+                        " expected: ",
+                        mask_groups * weight_d * weight_h * weight_w)
+                TORCH_CHECK(
+                        !modulated || (mask_c.size(2) == in_d &&
+                                       mask_c.size(3) == in_h &&
+                                       mask_c.size(4) == in_w),
+                        "mask input dims: (",
+                        mask_c.size(2),
+                        ", ",
+                        mask_c.size(3),
+                        ", ",
+                        mask_c.size(4),
+                        ") - ",
+                        "input dims: (",
+                        in_d,
+                        ", ",
+                        in_h,
+                        ", ",
+                        in_w,
+                        ")")
 
-            return output;
-        }
+                TORCH_CHECK(
+                        out_d > 0 && out_h > 0 && out_w > 0,
+                        "Calculated output size too small - out_d: ",
+                        out_d,
+                        " out_h: ",
+                        out_h,
+                        " out_w: ",
+                        out_w)
+
+                auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
+
+                // Separate batches into blocks
+                output = output.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      out_channels,
+                                      out_d,
+                                      out_h,
+                                      out_w});
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_d,
+                                              weight_h,
+                                              weight_w,
+                                              3,
+                                              in_d,
+                                              in_h,
+                                              in_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0, 0, 0});
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          mask_groups,
+                                          weight_d,
+                                          weight_h,
+                                          weight_w,
+                                          in_d,
+                                          in_h,
+                                          in_w});
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0});
+
+                // Separate channels into convolution groups
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        groups,
+                                        in_channels / groups,
+                                        in_d,
+                                        in_h,
+                                        in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+                weight_c = weight_c.view({groups,
+                                          weight_c.size(0) / groups,
+                                          weight_c.size(1),
+                                          weight_c.size(2),
+                                          weight_c.size(3),
+                                          weight_c.size(4)});
+
+                // Sample points and perform convolution
+                auto columns = at::empty({groups,
+                                          out_channels * weight_d * weight_h * weight_w / groups,
+                                          n_parallel_imgs * in_d * in_h * in_w},
+                                         input_c.options());
+                auto columns_view = columns.view({out_channels,
+                                                  weight_d,
+                                                  weight_h,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  in_d,
+                                                  in_h,
+                                                  in_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                    }
+
+                    auto output_b = output[b];
+                    col2vol(
+                            columns_view,
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_d,
+                            out_h,
+                            out_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            in_d,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            output_b);
+                }
+
+                output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+                if (with_bias)
+                    output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
+
+                return output;
+            }
 
-        namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-            _deform_conv_transpose2d_backward(
+            deform_conv_transpose3d_backward_kernel(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
-                    const at::Tensor &offset,
-                    const at::Tensor &mask,
-                    const at::Tensor &bias,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
                     int64_t groups) {
-                bool deformable = offset.defined() && offset.numel();
-                bool modulated = mask.defined() && mask.numel();
-                bool with_bias = bias.defined() && bias.numel();
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
 
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
-                at::Tensor offset_c = offset.contiguous();
-                at::Tensor mask_c = mask.contiguous();
-                at::Tensor bias_c = bias.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
 
                 int64_t batch_sz = input_c.size(0);
                 int64_t in_channels = input_c.size(1);
-                int64_t in_h = input_c.size(2);
-                int64_t in_w = input_c.size(3);
+                int64_t in_d = input_c.size(2);
+                int64_t in_h = input_c.size(3);
+                int64_t in_w = input_c.size(4);
 
                 int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
 
                 int64_t out_channels = weight_c.size(1) * groups;
-                int64_t weight_h = weight_c.size(2);
-                int64_t weight_w = weight_c.size(3);
-
-                int64_t stride_h = stride[0];
-                int64_t stride_w = stride[1];
-
-                int64_t pad_h = padding[0];
-                int64_t pad_w = padding[1];
-
-                int64_t out_pad_h = output_padding[0];
-                int64_t out_pad_w = output_padding[1];
-
-                int64_t dilation_h = dilation[0];
-                int64_t dilation_w = dilation[1];
+                int64_t weight_d = weight_c.size(2);
+                int64_t weight_h = weight_c.size(3);
+                int64_t weight_w = weight_c.size(4);
+
+                int64_t stride_d = stride[0];
+                int64_t stride_h = stride[1];
+                int64_t stride_w = stride[2];
+
+                int64_t pad_d = padding[0];
+                int64_t pad_h = padding[1];
+                int64_t pad_w = padding[2];
+
+                int64_t out_pad_d = output_padding[0];
+                int64_t out_pad_h = output_padding[1];
+                int64_t out_pad_w = output_padding[2];
+
+                int64_t dilation_d = dilation[0];
+                int64_t dilation_h = dilation[1];
+                int64_t dilation_w = dilation[2];
 
+                int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
                 int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
                 int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
-                int64_t offset_groups = deformable ? offset.size(1) / (2 * weight_h * weight_w) : 0;
-                int64_t mask_groups = modulated ? mask.size(1) / (weight_h * weight_w) : 0;
+                int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
-                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3})) : at::zeros_like(bias_c);
+                auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
 
                 // Separate into blocks
                 grad_out_c = grad_out_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               out_channels,
+                                              out_d,
                                               out_h,
                                               out_w});
 
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         in_channels,
+                                        in_d,
                                         in_h,
                                         in_w});
                 grad_input = grad_input.view_as(input_c);
                 if (deformable)
                     offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
                                               offset_groups,
+                                              weight_d,
                                               weight_h,
                                               weight_w,
-                                              2,
+                                              3,
+                                              in_d,
                                               in_h,
                                               in_w});
                 else
                     offset_c = offset_c.view({batch_sz / n_parallel_imgs,
                                               n_parallel_imgs,
-                                              0, 0, 0, 0, 0, 0});
+                                              0, 0, 0, 0, 0, 0, 0, 0});
                 grad_offset = grad_offset.view_as(offset_c);
                 if (modulated)
                     mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
                                           mask_groups,
+                                          weight_d,
                                           weight_h,
                                           weight_w,
+                                          in_d,
                                           in_h,
                                           in_w});
                 else
                     mask_c = mask_c.view({batch_sz / n_parallel_imgs,
                                           n_parallel_imgs,
-                                          0, 0, 0, 0, 0});
+                                          0, 0, 0, 0, 0, 0, 0});
                 grad_mask = grad_mask.view_as(mask_c);
 
                 auto grad_input_buf = at::zeros({batch_sz / n_parallel_imgs,
                                                  in_channels,
                                                  n_parallel_imgs,
+                                                 in_d,
                                                  in_h,
                                                  in_w}, input_c.options());
 
                 // Separate channels into convolution groups
                 input_c = input_c.view({batch_sz / n_parallel_imgs,
                                         n_parallel_imgs,
                                         groups,
                                         in_channels / groups,
+                                        in_d,
                                         in_h,
-                                        in_w}).permute({0, 2, 3, 1, 4, 5}).contiguous();
+                                        in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
 
                 grad_input_buf = grad_input_buf.view({grad_input_buf.size(0),
                                                       groups,
                                                       grad_input_buf.size(1) / groups,
                                                       grad_input_buf.size(2),
                                                       grad_input_buf.size(3),
-                                                      grad_input_buf.size(4)});
+                                                      grad_input_buf.size(4),
+                                                      grad_input_buf.size(5)});
 
                 weight_c = weight_c.view({groups,
                                           in_channels / groups,
                                           out_channels / groups,
+                                          weight_d,
                                           weight_h,
                                           weight_w});
                 grad_weight = grad_weight.view_as(weight_c);
 
                 auto columns = at::empty({groups,
-                                          out_channels * weight_h * weight_w / groups,
-                                          n_parallel_imgs * in_h * in_w},
+                                          out_channels * weight_d * weight_h * weight_w / groups,
+                                          n_parallel_imgs * in_d * in_h * in_w},
                                          input_c.options());
                 auto columns_view = columns.view({out_channels,
+                                                  weight_d,
                                                   weight_h,
                                                   weight_w,
                                                   n_parallel_imgs,
+                                                  in_d,
                                                   in_h,
                                                   in_w});
                 for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
                     columns.zero_();
                     for (int64_t g = 0; g < groups; g++) {
                         columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
                     }
 
                     auto grad_offset_b = grad_offset[b];
-                    deform_conv2d_compute_grad_offset(
+                    deform_conv3d_compute_grad_offset(
                             columns_view,
                             grad_out_c[b],
                             offset_c[b],
                             mask_c[b],
                             out_channels,
+                            out_d,
                             out_h,
                             out_w,
+                            weight_d,
                             weight_h,
                             weight_w,
+                            stride_d,
                             stride_h,
                             stride_w,
+                            pad_d,
                             pad_h,
                             pad_w,
+                            dilation_d,
                             dilation_h,
                             dilation_w,
+                            in_d,
                             in_h,
                             in_w,
                             n_parallel_imgs,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
                             grad_offset_b);
 
                     auto grad_mask_b = grad_mask[b];
-                    deform_conv2d_compute_grad_mask(
+                    deform_conv3d_compute_grad_mask(
                             columns_view,
                             grad_out_c[b],
                             offset_c[b],
                             out_channels,
+                            out_d,
                             out_h,
                             out_w,
+                            weight_d,
                             weight_h,
                             weight_w,
+                            stride_d,
                             stride_h,
                             stride_w,
+                            pad_d,
                             pad_h,
                             pad_w,
+                            dilation_d,
                             dilation_h,
                             dilation_w,
+                            in_d,
                             in_h,
                             in_w,
                             n_parallel_imgs,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
                             grad_mask_b);
 
-                    im2col(
+                    vol2col(
                             grad_out_c[b],
                             offset_c[b],
                             mask_c[b],
                             out_channels,
+                            out_d,
                             out_h,
                             out_w,
+                            weight_d,
                             weight_h,
                             weight_w,
+                            stride_d,
                             stride_h,
                             stride_w,
+                            pad_d,
                             pad_h,
                             pad_w,
+                            dilation_d,
                             dilation_h,
                             dilation_w,
+                            in_d,
                             in_h,
                             in_w,
                             n_parallel_imgs,
                             offset_groups,
                             mask_groups,
                             deformable,
                             modulated,
@@ -561,144 +646,31 @@
                         grad_weight[g].flatten(1).addmm_(input_c[b][g].flatten(1), columns[g].transpose(1, 0));
                     }
                 }
 
                 grad_input_buf = grad_input_buf.view({batch_sz / n_parallel_imgs,
                                                       in_channels,
                                                       n_parallel_imgs,
+                                                      in_d,
                                                       in_h,
                                                       in_w}).transpose_(1, 2);
                 grad_input.copy_(grad_input_buf);
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
-                grad_offset = grad_offset.view_as(offset);
-                grad_mask = grad_mask.view_as(mask);
+                grad_offset = deformable ? grad_offset.view_as(offset.value()) : at::Tensor();
+                grad_mask = modulated ? grad_mask.view_as(mask.value()) : at::Tensor();
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
-        class DeformConvTranspose2dFunction
-                : public torch::autograd::Function<DeformConvTranspose2dFunction> {
-        public:
-            static torch::autograd::variable_list forward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::Variable &input,
-                    const torch::autograd::Variable &weight,
-                    const torch::autograd::Variable &offset,
-                    const torch::autograd::Variable &mask,
-                    const torch::autograd::Variable &bias,
-                    at::IntArrayRef stride,
-                    at::IntArrayRef padding,
-                    at::IntArrayRef output_padding,
-                    at::IntArrayRef dilation,
-                    int64_t groups) {
-                at::AutoDispatchBelowADInplaceOrView g;
-                auto output = deform_conv_transpose2d_forward(
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        output_padding,
-                        dilation,
-                        groups);
-
-                ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride.vec();
-                ctx->saved_data["padding"] = padding.vec();
-                ctx->saved_data["output_padding"] = output_padding.vec();
-                ctx->saved_data["dilation"] = dilation.vec();
-                ctx->saved_data["groups"] = groups;
-
-                return {
-                        output,
-                };
-            }
-
-            static torch::autograd::variable_list backward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::variable_list &grad_output) {
-                auto saved = ctx->get_saved_variables();
-                auto input = saved[0];
-                auto weight = saved[1];
-                auto offset = saved[2];
-                auto mask = saved[3];
-                auto bias = saved[4];
-
-                auto stride = ctx->saved_data["stride"].toIntVector();
-                auto padding = ctx->saved_data["padding"].toIntVector();
-                auto output_padding = ctx->saved_data["output_padding"].toIntVector();
-                auto dilation = ctx->saved_data["dilation"].toIntVector();
-                auto groups = ctx->saved_data["groups"].toInt();
-
-                auto grads = detail::_deform_conv_transpose2d_backward(
-                        grad_output[0],
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        output_padding,
-                        dilation,
-                        groups);
-                auto grad_input = std::get<0>(grads);
-                auto grad_weight = std::get<1>(grads);
-                auto grad_offset = std::get<2>(grads);
-                auto grad_mask = std::get<3>(grads);
-                auto grad_bias = std::get<4>(grads);
-
-                return {
-                        grad_input,
-                        grad_weight,
-                        grad_offset,
-                        grad_mask,
-                        grad_bias,
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                };
-            }
-        };
-
-        at::Tensor deform_conv_transpose2d(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::optional<at::Tensor> &offset = {},
-                const at::optional<at::Tensor> &mask = {},
-                const at::optional<at::Tensor> &bias = {},
-                at::IntArrayRef stride = 1,
-                at::IntArrayRef padding = 0,
-                at::IntArrayRef output_padding = 0,
-                at::IntArrayRef dilation = 1,
-                int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose2d")
-            auto result = DeformConvTranspose2dFunction::apply(
-                    input,
-                    weight,
-                    offset.value_or(input.new_zeros(0)),
-                    mask.value_or(input.new_zeros(0)),
-                    bias.value_or(input.new_zeros(0)),
-                    stride,
-                    padding,
-                    output_padding,
-                    dilation,
-                    groups);
-            return result[0];
-        }
-
-        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
-            m.def("tvdcn::deform_conv_transpose2d(Tensor input, Tensor weight, "
-                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
-                  "int[2] stride=1, int[2] padding=0, int[2] output_padding=0, "
-                  "int[2] dilation=1, int groups=1) -> Tensor",
-                  &deform_conv_transpose2d);
+        TORCH_LIBRARY_IMPL(tvdcn, CPU, m) {
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::deform_conv_transpose3d"),
+                    TORCH_FN(deform_conv_transpose3d_forward_kernel));
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::_deform_conv_transpose3d_backward"),
+                    TORCH_FN(deform_conv_transpose3d_backward_kernel));
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/deform_conv_transpose3d.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/cuda/deform_conv_transpose3d_kernel.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -67,345 +67,351 @@
 // https://github.com/open-mmlab/mmdetection/blob/master/mmdet/ops/dcn/src/deform_conv_cuda.cpp
 
 // modified from
 // https://github.com/pytorch/vision/blob/master/torchvision/csrc/cpu/deform_conv2d_kernel.cpp
 
 #include <torch/autograd.h>
 
-#include "dispatch/deform_conv3d_kernels.h"
-#include "utils/parallel_helpers.h"
-#include "utils/tensor_utils.h"
+#include "deform_conv3d_common_kernels.h"
+#include "../utils/parallel_helpers.h"
+#include "../utils/tensor_utils.h"
 
 namespace tvdcn {
     namespace ops {
-        at::Tensor deform_conv_transpose3d_forward(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::Tensor &offset,
-                const at::Tensor &mask,
-                const at::Tensor &bias,
-                at::IntArrayRef stride,
-                at::IntArrayRef padding,
-                at::IntArrayRef output_padding,
-                at::IntArrayRef dilation,
-                int64_t groups) {
-            at::CheckedFrom c = "deform_conv_transpose3d_forward";
-            auto args = {
-                    at::TensorArg(input, "input", 1),
-                    at::TensorArg(weight, "weight", 2),
-                    at::TensorArg(offset, "offset", 3),
-                    at::TensorArg(mask, "mask", 4),
-                    at::TensorArg(bias, "bias", 5)};
-            at::checkAllSameType(c, args);
-            at::checkAllSameDevice(c, args);
-
-            bool deformable = offset.defined() && offset.numel();
-            bool modulated = mask.defined() && mask.numel();
-            bool with_bias = bias.defined() && bias.numel();
-
-            at::Tensor input_c = input.contiguous();
-            at::Tensor weight_c = weight.contiguous();
-            at::Tensor offset_c = offset.contiguous();
-            at::Tensor mask_c = mask.contiguous();
-            at::Tensor bias_c = bias.contiguous();
-
-            TORCH_CHECK(input_c.ndimension() == 5)
-            TORCH_CHECK(weight_c.ndimension() == 5)
-            TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
-            TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
-
-            int64_t batch_sz = input_c.size(0);
-            int64_t in_channels = input_c.size(1);
-            int64_t in_d = input_c.size(2);
-            int64_t in_h = input_c.size(3);
-            int64_t in_w = input_c.size(4);
-
-            int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
-
-            int64_t out_channels = weight_c.size(1) * groups;
-            int64_t weight_d = weight_c.size(2);
-            int64_t weight_h = weight_c.size(3);
-            int64_t weight_w = weight_c.size(4);
-
-            int64_t stride_d = stride[0];
-            int64_t stride_h = stride[1];
-            int64_t stride_w = stride[2];
-
-            int64_t pad_d = padding[0];
-            int64_t pad_h = padding[1];
-            int64_t pad_w = padding[2];
-
-            int64_t out_pad_d = output_padding[0];
-            int64_t out_pad_h = output_padding[1];
-            int64_t out_pad_w = output_padding[2];
-
-            int64_t dilation_d = dilation[0];
-            int64_t dilation_h = dilation[1];
-            int64_t dilation_w = dilation[2];
-
-            int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
-            int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
-            int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
-
-            TORCH_CHECK(
-                    weight_d > 0 && weight_h > 0 && weight_w > 0,
-                    "weight_d: ",
-                    weight_d,
-                    " weight_h: ",
-                    weight_h,
-                    " weight_w: ",
-                    weight_w)
-            TORCH_CHECK(
-                    stride_d > 0 && stride_h > 0 && stride_w > 0,
-                    " stride_d: ",
-                    stride_d,
-                    "stride_h: ",
-                    stride_h,
-                    " stride_w: ",
-                    stride_w)
-            TORCH_CHECK(
-                    pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
-                    "pad_d: ",
-                    pad_d,
-                    " pad_h: ",
-                    pad_h,
-                    " pad_w: ",
-                    pad_w)
-            TORCH_CHECK(
-                    dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
-                    "dilation_d: ",
-                    dilation_d,
-                    " dilation_h: ",
-                    dilation_h,
-                    " dilation_w: ",
-                    dilation_w)
-
-            TORCH_CHECK(weight_c.size(1) * groups == out_channels)
-            TORCH_CHECK(weight_c.size(0) % groups == 0)
-
-            int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
-            int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
-
-            TORCH_CHECK(
-                    !deformable || offset_c.size(0) == input_c.size(0),
-                    "invalid batch size of offset")
-            TORCH_CHECK(
-                    !deformable || offset_groups > 0,
-                    "The shape of the offset tensor at dimension 1 is not valid. It should "
-                    "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
-                    offset.size(1),
-                    ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
-                    3 * weight_d * weight_h * weight_w)
-            TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
-            TORCH_CHECK(
-                    !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
-                    "offset.shape[1] is not valid. got: ",
-                    offset_c.size(1),
-                    " expected: ",
-                    offset_groups * 3 * weight_d * weight_h * weight_w)
-            TORCH_CHECK(
-                    !deformable || (offset_c.size(2) == in_d &&
-                                    offset_c.size(3) == in_h &&
-                                    offset_c.size(4) == in_w),
-                    "offset input dims: (",
-                    offset_c.size(2),
-                    ", ",
-                    offset_c.size(3),
-                    ", ",
-                    offset_c.size(4),
-                    ") - ",
-                    "input dims: (",
-                    in_d,
-                    ", ",
-                    in_h,
-                    ", ",
-                    in_w,
-                    ")")
-
-            TORCH_CHECK(
-                    !modulated || mask_c.size(0) == input_c.size(0),
-                    "invalid batch size of mask")
-            TORCH_CHECK(
-                    !modulated || mask_groups > 0,
-                    "The shape of the mask tensor at dimension 1 is not valid. It should "
-                    "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
-                    mask.size(1),
-                    ", while weight.size(2) * weight.size(3) * weight.size(4)=",
-                    weight_d * weight_h * weight_w)
-            TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
-            TORCH_CHECK(
-                    !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
-                    "mask.shape[1] is not valid. got: ",
-                    mask_c.size(1),
-                    " expected: ",
-                    mask_groups * weight_d * weight_h * weight_w)
-            TORCH_CHECK(
-                    !modulated || (mask_c.size(2) == in_d &&
-                                   mask_c.size(3) == in_h &&
-                                   mask_c.size(4) == in_w),
-                    "mask input dims: (",
-                    mask_c.size(2),
-                    ", ",
-                    mask_c.size(3),
-                    ", ",
-                    mask_c.size(4),
-                    ") - ",
-                    "input dims: (",
-                    in_d,
-                    ", ",
-                    in_h,
-                    ", ",
-                    in_w,
-                    ")")
-
-            TORCH_CHECK(
-                    out_d > 0 && out_h > 0 && out_w > 0,
-                    "Calculated output size too small - out_d: ",
-                    out_d,
-                    " out_h: ",
-                    out_h,
-                    " out_w: ",
-                    out_w)
-
-            auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
-
-            // Separate batches into blocks
-            output = output.view({batch_sz / n_parallel_imgs,
-                                  n_parallel_imgs,
-                                  out_channels,
-                                  out_d,
-                                  out_h,
-                                  out_w});
-            if (deformable)
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          offset_groups,
-                                          weight_d,
-                                          weight_h,
-                                          weight_w,
-                                          3,
-                                          in_d,
-                                          in_h,
-                                          in_w});
-            else
-                offset_c = offset_c.view({batch_sz / n_parallel_imgs,
-                                          n_parallel_imgs,
-                                          0, 0, 0, 0, 0, 0, 0, 0});
-            if (modulated)
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      mask_groups,
-                                      weight_d,
-                                      weight_h,
-                                      weight_w,
-                                      in_d,
-                                      in_h,
-                                      in_w});
-            else
-                mask_c = mask_c.view({batch_sz / n_parallel_imgs,
-                                      n_parallel_imgs,
-                                      0, 0, 0, 0, 0, 0, 0});
+        using namespace cuda;
 
-            // Separate channels into convolution groups
-            input_c = input_c.view({batch_sz / n_parallel_imgs,
-                                    n_parallel_imgs,
-                                    groups,
-                                    in_channels / groups,
-                                    in_d,
-                                    in_h,
-                                    in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
-            weight_c = weight_c.view({groups,
-                                      weight_c.size(0) / groups,
-                                      weight_c.size(1),
-                                      weight_c.size(2),
-                                      weight_c.size(3),
-                                      weight_c.size(4)});
-
-            // Sample points and perform convolution
-            auto columns = at::empty({groups,
-                                      out_channels * weight_d * weight_h * weight_w / groups,
-                                      n_parallel_imgs * in_d * in_h * in_w},
-                                     input_c.options());
-            auto columns_view = columns.view({out_channels,
-                                              weight_d,
-                                              weight_h,
-                                              weight_w,
-                                              n_parallel_imgs,
-                                              in_d,
-                                              in_h,
-                                              in_w});
-            for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
-                columns.zero_();
-                for (int64_t g = 0; g < groups; g++) {
-                    columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
-                }
+        namespace {
+            at::Tensor deform_conv_transpose3d_forward_kernel(
+                    const at::Tensor &input,
+                    const at::Tensor &weight,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
+                    at::IntArrayRef stride,
+                    at::IntArrayRef padding,
+                    at::IntArrayRef output_padding,
+                    at::IntArrayRef dilation,
+                    int64_t groups) {
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
+
+                at::CheckedFrom c = "deform_conv_transpose3d_forward_kernel";
+                std::vector<at::TensorArg> args;
+                args.reserve(5);
+                args.emplace_back(at::TensorArg(input, "input", 1));
+                args.emplace_back(at::TensorArg(weight, "weight", 2));
+                if (deformable)
+                    args.emplace_back(at::TensorArg(offset.value(), "offset", 3));
+                if (modulated)
+                    args.emplace_back(at::TensorArg(mask.value(), "mask", 4));
+                if (with_bias)
+                    args.emplace_back(at::TensorArg(bias.value(), "bias", 5));
+                at::checkAllSameGPUExceptUndefined(c, args);
+                at::checkAllSameTypeExceptUndefined(c, args);
 
-                auto output_b = output[b];
-                col2vol(
-                        columns_view,
-                        offset_c[b],
-                        mask_c[b],
-                        out_channels,
-                        out_d,
-                        out_h,
-                        out_w,
+                at::Tensor input_c = input.contiguous();
+                at::Tensor weight_c = weight.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
+
+                TORCH_CHECK(input_c.ndimension() == 5)
+                TORCH_CHECK(weight_c.ndimension() == 5)
+                TORCH_CHECK(!deformable || offset_c.ndimension() == 5)
+                TORCH_CHECK(!modulated || mask_c.ndimension() == 5)
+
+                int64_t batch_sz = input_c.size(0);
+                int64_t in_channels = input_c.size(1);
+                int64_t in_d = input_c.size(2);
+                int64_t in_h = input_c.size(3);
+                int64_t in_w = input_c.size(4);
+
+                int64_t n_parallel_imgs = get_greatest_divisor_below_bound(batch_sz, kMaxParallelImgs);
+
+                int64_t out_channels = weight_c.size(1) * groups;
+                int64_t weight_d = weight_c.size(2);
+                int64_t weight_h = weight_c.size(3);
+                int64_t weight_w = weight_c.size(4);
+
+                int64_t stride_d = stride[0];
+                int64_t stride_h = stride[1];
+                int64_t stride_w = stride[2];
+
+                int64_t pad_d = padding[0];
+                int64_t pad_h = padding[1];
+                int64_t pad_w = padding[2];
+
+                int64_t out_pad_d = output_padding[0];
+                int64_t out_pad_h = output_padding[1];
+                int64_t out_pad_w = output_padding[2];
+
+                int64_t dilation_d = dilation[0];
+                int64_t dilation_h = dilation[1];
+                int64_t dilation_w = dilation[2];
+
+                int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
+                int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
+                int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
+
+                TORCH_CHECK(
+                        weight_d > 0 && weight_h > 0 && weight_w > 0,
+                        "weight_d: ",
                         weight_d,
+                        " weight_h: ",
                         weight_h,
-                        weight_w,
+                        " weight_w: ",
+                        weight_w)
+                TORCH_CHECK(
+                        stride_d > 0 && stride_h > 0 && stride_w > 0,
+                        " stride_d: ",
                         stride_d,
+                        "stride_h: ",
                         stride_h,
-                        stride_w,
+                        " stride_w: ",
+                        stride_w)
+                TORCH_CHECK(
+                        pad_d >= 0 && pad_h >= 0 && pad_w >= 0,
+                        "pad_d: ",
                         pad_d,
+                        " pad_h: ",
                         pad_h,
-                        pad_w,
+                        " pad_w: ",
+                        pad_w)
+                TORCH_CHECK(
+                        dilation_d > 0 && dilation_h > 0 && dilation_w > 0,
+                        "dilation_d: ",
                         dilation_d,
+                        " dilation_h: ",
                         dilation_h,
-                        dilation_w,
+                        " dilation_w: ",
+                        dilation_w)
+
+                TORCH_CHECK(weight_c.size(1) * groups == out_channels)
+                TORCH_CHECK(weight_c.size(0) % groups == 0)
+
+                int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
+
+                TORCH_CHECK(
+                        !deformable || offset_c.size(0) == input_c.size(0),
+                        "invalid batch size of offset")
+                TORCH_CHECK(
+                        !deformable || offset_groups > 0,
+                        "The shape of the offset tensor at dimension 1 is not valid. It should "
+                        "be a multiple of 3 * weight.size(2) * weight.size(3) * weight.size(4).\nGot offset.size(1)=",
+                        offset_c.size(1),
+                        ", while 3 * weight.size(2) * weight.size(3) * weight.size(3)=",
+                        3 * weight_d * weight_h * weight_w)
+                TORCH_CHECK(!deformable || input_c.size(1) % offset_groups == 0)
+                TORCH_CHECK(
+                        !deformable || offset_c.size(1) == offset_groups * 3 * weight_d * weight_h * weight_w,
+                        "offset.shape[1] is not valid. got: ",
+                        offset_c.size(1),
+                        " expected: ",
+                        offset_groups * 3 * weight_d * weight_h * weight_w)
+                TORCH_CHECK(
+                        !deformable || (offset_c.size(2) == in_d &&
+                                        offset_c.size(3) == in_h &&
+                                        offset_c.size(4) == in_w),
+                        "offset input dims: (",
+                        offset_c.size(2),
+                        ", ",
+                        offset_c.size(3),
+                        ", ",
+                        offset_c.size(4),
+                        ") - ",
+                        "input dims: (",
                         in_d,
+                        ", ",
                         in_h,
+                        ", ",
                         in_w,
-                        n_parallel_imgs,
-                        offset_groups,
-                        mask_groups,
-                        deformable,
-                        modulated,
-                        output_b);
-            }
+                        ")")
 
-            output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
-            if (with_bias)
-                output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
+                TORCH_CHECK(
+                        !modulated || mask_c.size(0) == input_c.size(0),
+                        "invalid batch size of mask")
+                TORCH_CHECK(
+                        !modulated || mask_groups > 0,
+                        "The shape of the mask tensor at dimension 1 is not valid. It should "
+                        "be a multiple of weight.size(2) * weight.size(3) * weight.size(4).\nGot mask.size(1)=",
+                        mask_c.size(1),
+                        ", while weight.size(2) * weight.size(3) * weight.size(4)=",
+                        weight_d * weight_h * weight_w)
+                TORCH_CHECK(!modulated || input_c.size(1) % mask_groups == 0)
+                TORCH_CHECK(
+                        !modulated || mask_c.size(1) == mask_groups * weight_d * weight_h * weight_w,
+                        "mask.shape[1] is not valid. got: ",
+                        mask_c.size(1),
+                        " expected: ",
+                        mask_groups * weight_d * weight_h * weight_w)
+                TORCH_CHECK(
+                        !modulated || (mask_c.size(2) == in_d &&
+                                       mask_c.size(3) == in_h &&
+                                       mask_c.size(4) == in_w),
+                        "mask input dims: (",
+                        mask_c.size(2),
+                        ", ",
+                        mask_c.size(3),
+                        ", ",
+                        mask_c.size(4),
+                        ") - ",
+                        "input dims: (",
+                        in_d,
+                        ", ",
+                        in_h,
+                        ", ",
+                        in_w,
+                        ")")
 
-            return output;
-        }
+                TORCH_CHECK(
+                        out_d > 0 && out_h > 0 && out_w > 0,
+                        "Calculated output size too small - out_d: ",
+                        out_d,
+                        " out_h: ",
+                        out_h,
+                        " out_w: ",
+                        out_w)
+
+                auto output = at::zeros({batch_sz, out_channels, out_d, out_h, out_w}, input_c.options());
+
+                // Separate batches into blocks
+                output = output.view({batch_sz / n_parallel_imgs,
+                                      n_parallel_imgs,
+                                      out_channels,
+                                      out_d,
+                                      out_h,
+                                      out_w});
+                if (deformable)
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              offset_groups,
+                                              weight_d,
+                                              weight_h,
+                                              weight_w,
+                                              3,
+                                              in_d,
+                                              in_h,
+                                              in_w});
+                else
+                    offset_c = offset_c.view({batch_sz / n_parallel_imgs,
+                                              n_parallel_imgs,
+                                              0, 0, 0, 0, 0, 0, 0, 0});
+                if (modulated)
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          mask_groups,
+                                          weight_d,
+                                          weight_h,
+                                          weight_w,
+                                          in_d,
+                                          in_h,
+                                          in_w});
+                else
+                    mask_c = mask_c.view({batch_sz / n_parallel_imgs,
+                                          n_parallel_imgs,
+                                          0, 0, 0, 0, 0, 0, 0});
+
+                // Separate channels into convolution groups
+                input_c = input_c.view({batch_sz / n_parallel_imgs,
+                                        n_parallel_imgs,
+                                        groups,
+                                        in_channels / groups,
+                                        in_d,
+                                        in_h,
+                                        in_w}).permute({0, 2, 3, 1, 4, 5, 6}).contiguous();
+                weight_c = weight_c.view({groups,
+                                          weight_c.size(0) / groups,
+                                          weight_c.size(1),
+                                          weight_c.size(2),
+                                          weight_c.size(3),
+                                          weight_c.size(4)});
+
+                // Sample points and perform convolution
+                auto columns = at::empty({groups,
+                                          out_channels * weight_d * weight_h * weight_w / groups,
+                                          n_parallel_imgs * in_d * in_h * in_w},
+                                         input_c.options());
+                auto columns_view = columns.view({out_channels,
+                                                  weight_d,
+                                                  weight_h,
+                                                  weight_w,
+                                                  n_parallel_imgs,
+                                                  in_d,
+                                                  in_h,
+                                                  in_w});
+                for (int64_t b = 0; b < batch_sz / n_parallel_imgs; b++) {
+                    columns.zero_();
+                    for (int64_t g = 0; g < groups; g++) {
+                        columns[g].addmm_(weight_c[g].flatten(1).transpose(0, 1), input_c[b][g].flatten(1));
+                    }
+
+                    auto output_b = output[b];
+                    col2vol(
+                            columns_view,
+                            offset_c[b],
+                            mask_c[b],
+                            out_channels,
+                            out_d,
+                            out_h,
+                            out_w,
+                            weight_d,
+                            weight_h,
+                            weight_w,
+                            stride_d,
+                            stride_h,
+                            stride_w,
+                            pad_d,
+                            pad_h,
+                            pad_w,
+                            dilation_d,
+                            dilation_h,
+                            dilation_w,
+                            in_d,
+                            in_h,
+                            in_w,
+                            n_parallel_imgs,
+                            offset_groups,
+                            mask_groups,
+                            deformable,
+                            modulated,
+                            output_b);
+                }
+
+                output = output.view({batch_sz, out_channels, out_d, out_h, out_w});
+                if (with_bias)
+                    output.add_(bias_c.view({1, out_channels, 1, 1, 1}));
+
+                return output;
+            }
 
-        namespace detail {
             std::tuple<at::Tensor, at::Tensor, at::Tensor, at::Tensor, at::Tensor>
-            _deform_conv_transpose3d_backward(
+            deform_conv_transpose3d_backward_kernel(
                     const at::Tensor &grad_out,
                     const at::Tensor &input,
                     const at::Tensor &weight,
-                    const at::Tensor &offset,
-                    const at::Tensor &mask,
-                    const at::Tensor &bias,
+                    const at::optional<at::Tensor> &offset,
+                    const at::optional<at::Tensor> &mask,
+                    const at::optional<at::Tensor> &bias,
                     at::IntArrayRef stride,
                     at::IntArrayRef padding,
                     at::IntArrayRef output_padding,
                     at::IntArrayRef dilation,
                     int64_t groups) {
-                bool deformable = offset.defined() && offset.numel();
-                bool modulated = mask.defined() && mask.numel();
-                bool with_bias = bias.defined() && bias.numel();
+                bool deformable = offset.has_value() && offset->defined();
+                bool modulated = mask.has_value() && mask->defined();
+                bool with_bias = bias.has_value() && bias->defined();
 
                 at::Tensor grad_out_c = grad_out.contiguous();
                 at::Tensor input_c = input.contiguous();
                 at::Tensor weight_c = weight.contiguous();
-                at::Tensor offset_c = offset.contiguous();
-                at::Tensor mask_c = mask.contiguous();
-                at::Tensor bias_c = bias.contiguous();
+                at::Tensor offset_c = (deformable ? offset.value() : input.new_zeros(0)).contiguous();
+                at::Tensor mask_c = (modulated ? mask.value() : input.new_zeros(0)).contiguous();
+                at::Tensor bias_c = (with_bias ? bias.value() : input.new_zeros(0)).contiguous();
 
                 int64_t batch_sz = input_c.size(0);
                 int64_t in_channels = input_c.size(1);
                 int64_t in_d = input_c.size(2);
                 int64_t in_h = input_c.size(3);
                 int64_t in_w = input_c.size(4);
 
@@ -432,16 +438,16 @@
                 int64_t dilation_h = dilation[1];
                 int64_t dilation_w = dilation[2];
 
                 int64_t out_d = (in_d - 1) * stride_d - 2 * pad_d + dilation_d * (weight_d - 1) + 1 + out_pad_d;
                 int64_t out_h = (in_h - 1) * stride_h - 2 * pad_h + dilation_h * (weight_h - 1) + 1 + out_pad_h;
                 int64_t out_w = (in_w - 1) * stride_w - 2 * pad_w + dilation_w * (weight_w - 1) + 1 + out_pad_w;
 
-                int64_t offset_groups = deformable ? offset.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
-                int64_t mask_groups = modulated ? mask.size(1) / (weight_d * weight_h * weight_w) : 0;
+                int64_t offset_groups = deformable ? offset_c.size(1) / (3 * weight_d * weight_h * weight_w) : 0;
+                int64_t mask_groups = modulated ? mask_c.size(1) / (weight_d * weight_h * weight_w) : 0;
 
                 auto grad_input = at::zeros_like(input_c);
                 auto grad_weight = at::zeros_like(weight_c);
                 auto grad_offset = at::zeros_like(offset_c);
                 auto grad_mask = at::zeros_like(mask_c);
                 auto grad_bias = with_bias ? grad_out_c.sum(at::IntArrayRef({0, 2, 3, 4})) : at::zeros_like(bias_c);
 
@@ -647,138 +653,24 @@
                                                       in_d,
                                                       in_h,
                                                       in_w}).transpose_(1, 2);
                 grad_input.copy_(grad_input_buf);
 
                 grad_input = grad_input.view_as(input);
                 grad_weight = grad_weight.view_as(weight);
-                grad_offset = grad_offset.view_as(offset);
-                grad_mask = grad_mask.view_as(mask);
+                grad_offset = deformable ? grad_offset.view_as(offset.value()) : at::Tensor();
+                grad_mask = modulated ? grad_mask.view_as(mask.value()) : at::Tensor();
 
                 return std::make_tuple(grad_input, grad_weight, grad_offset, grad_mask, grad_bias);
             }
         }
 
-        class DeformConvTranspose3dFunction
-                : public torch::autograd::Function<DeformConvTranspose3dFunction> {
-        public:
-            static torch::autograd::variable_list forward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::Variable &input,
-                    const torch::autograd::Variable &weight,
-                    const torch::autograd::Variable &offset,
-                    const torch::autograd::Variable &mask,
-                    const torch::autograd::Variable &bias,
-                    at::IntArrayRef stride,
-                    at::IntArrayRef padding,
-                    at::IntArrayRef output_padding,
-                    at::IntArrayRef dilation,
-                    int64_t groups) {
-                at::AutoDispatchBelowADInplaceOrView g;
-                auto output = deform_conv_transpose3d_forward(
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        output_padding,
-                        dilation,
-                        groups);
-
-                ctx->save_for_backward({input, weight, offset, mask, bias});
-                ctx->saved_data["stride"] = stride.vec();
-                ctx->saved_data["padding"] = padding.vec();
-                ctx->saved_data["output_padding"] = output_padding.vec();
-                ctx->saved_data["dilation"] = dilation.vec();
-                ctx->saved_data["groups"] = groups;
-
-                return {
-                        output,
-                };
-            }
-
-            static torch::autograd::variable_list backward(
-                    torch::autograd::AutogradContext *ctx,
-                    const torch::autograd::variable_list &grad_output) {
-                auto saved = ctx->get_saved_variables();
-                auto input = saved[0];
-                auto weight = saved[1];
-                auto offset = saved[2];
-                auto mask = saved[3];
-                auto bias = saved[4];
-
-                auto stride = ctx->saved_data["stride"].toIntVector();
-                auto padding = ctx->saved_data["padding"].toIntVector();
-                auto output_padding = ctx->saved_data["output_padding"].toIntVector();
-                auto dilation = ctx->saved_data["dilation"].toIntVector();
-                auto groups = ctx->saved_data["groups"].toInt();
-
-                auto grads = detail::_deform_conv_transpose3d_backward(
-                        grad_output[0],
-                        input,
-                        weight,
-                        offset,
-                        mask,
-                        bias,
-                        stride,
-                        padding,
-                        output_padding,
-                        dilation,
-                        groups);
-                auto grad_input = std::get<0>(grads);
-                auto grad_weight = std::get<1>(grads);
-                auto grad_offset = std::get<2>(grads);
-                auto grad_mask = std::get<3>(grads);
-                auto grad_bias = std::get<4>(grads);
-
-                return {
-                        grad_input,
-                        grad_weight,
-                        grad_offset,
-                        grad_mask,
-                        grad_bias,
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                        torch::autograd::Variable(),
-                };
-            }
-        };
-
-        at::Tensor deform_conv_transpose3d(
-                const at::Tensor &input,
-                const at::Tensor &weight,
-                const at::optional<at::Tensor> &offset = {},
-                const at::optional<at::Tensor> &mask = {},
-                const at::optional<at::Tensor> &bias = {},
-                at::IntArrayRef stride = 1,
-                at::IntArrayRef padding = 0,
-                at::IntArrayRef output_padding = 0,
-                at::IntArrayRef dilation = 1,
-                int64_t groups = 1) {
-            C10_LOG_API_USAGE_ONCE("tvdcn.csrc.ops.deform_conv_transpose.deform_conv_transpose3d")
-            auto result = DeformConvTranspose3dFunction::apply(
-                    input,
-                    weight,
-                    offset.value_or(input.new_zeros(0)),
-                    mask.value_or(input.new_zeros(0)),
-                    bias.value_or(input.new_zeros(0)),
-                    stride,
-                    padding,
-                    output_padding,
-                    dilation,
-                    groups);
-            return result[0];
-        }
-
-        TORCH_LIBRARY_FRAGMENT(tvdcn, m) {
-            m.def("tvdcn::deform_conv_transpose3d(Tensor input, Tensor weight, "
-                  "Tensor? offset=None, Tensor? mask=None, Tensor? bias=None, "
-                  "int[3] stride=1, int[3] padding=0, int[3] output_padding=0, "
-                  "int[3] dilation=1, int groups=1) -> Tensor",
-                  &deform_conv_transpose3d);
+        TORCH_LIBRARY_IMPL(tvdcn, CUDA, m) {
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::deform_conv_transpose3d"),
+                    TORCH_FN(deform_conv_transpose3d_forward_kernel));
+            m.impl(
+                    TORCH_SELECTIVE_NAME("tvdcn::_deform_conv_transpose3d_backward"),
+                    TORCH_FN(deform_conv_transpose3d_backward_kernel));
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/ops/utils/tensor_utils.cpp` & `tvdcn-0.4.0/tvdcn/csrc/ops/utils/tensor_utils.cpp`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,52 @@
 #include <ATen/TensorUtils.h>
 
 namespace at {
-    namespace {
-        inline std::vector<int> definedPositions(ArrayRef<TensorArg> tensors) {
-            std::vector<int> res = {};
-            for (int i = 0; i < tensors.size(); i++) {
-                if (tensors[i]->defined())
-                    res.push_back(i);
-            }
-            return res;
+    static inline IntArrayRef definedPositions(ArrayRef<TensorArg> tensors) {
+        std::vector<int64_t> res;
+        res.reserve(tensors.size());
+        for (const auto i: c10::irange(tensors.size())) {
+            if (tensors[i]->defined())
+                res.emplace_back(i);
+        }
+        return res;
+    }
+
+    static void checkDeviceType(CheckedFrom c,
+                                const TensorArg &t,
+                                DeviceType device_type) {
+        TORCH_CHECK(
+                !t->defined() || t->device().type() == device_type,
+                "Expected tensor for argument #",
+                t.pos,
+                " '",
+                t.name,
+                "' to have ",
+                device_type,
+                " DeviceType, but got tensor with ",
+                t->device().type(),
+                " DeviceType (while checking arguments for ", c, ")");
+    }
+
+    void checkDeviceType(
+            CheckedFrom c,
+            ArrayRef<TensorArg> tensors,
+            DeviceType device_type) {
+        for (const auto i: c10::irange(tensors.size())) {
+            checkDeviceType(c, tensors[i], device_type);
+        }
+    }
+
+    void checkDeviceTypeExceptUndefined(
+            CheckedFrom c,
+            ArrayRef<TensorArg> tensors,
+            DeviceType device_type) {
+        auto defined_pos = definedPositions(tensors);
+        for (const auto i: c10::irange(defined_pos.size())) {
+            checkDeviceType(c, tensors[defined_pos[i]], device_type);
         }
     }
 
     void checkSameDeviceType(
             CheckedFrom c,
             const TensorArg &t1,
             const TensorArg &t2) {
@@ -35,26 +69,26 @@
     }
 
     void checkAllSameDeviceType(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         if (tensors.size() < 2)
             return;
-        for (int i = 1; i < tensors.size(); i++) {
+        for (const auto i: c10::irange(1, tensors.size())) {
             checkSameDeviceType(c, tensors[0], tensors[i]);
         }
     }
 
     void checkAllSameDeviceTypeExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (int i = 1; i < defined_pos.size(); i++) {
+        for (const auto i: c10::irange(1, defined_pos.size())) {
             checkSameDeviceType(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
         }
     }
 
     void checkSameDevice(
             CheckedFrom c,
             const TensorArg &t1,
@@ -78,43 +112,43 @@
     }
 
     void checkAllSameDevice(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         if (tensors.size() < 2)
             return;
-        for (int i = 1; i < tensors.size(); i++) {
+        for (const auto i: c10::irange(1, tensors.size())) {
             checkSameDevice(c, tensors[0], tensors[i]);
         }
     }
 
     void checkAllSameDeviceExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (int i = 1; i < defined_pos.size(); i++) {
+        for (const auto i: c10::irange(1, defined_pos.size())) {
             checkSameDevice(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
         }
     }
 
     void checkAllSameGPUExceptUndefined(
             CheckedFrom c,
             ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (int i = 1; i < defined_pos.size(); i++) {
+        for (const auto i: c10::irange(1, defined_pos.size())) {
             checkSameGPU(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
         }
     }
 
     void checkAllSameTypeExceptUndefined(CheckedFrom c, ArrayRef<TensorArg> tensors) {
         auto defined_pos = definedPositions(tensors);
         if (defined_pos.size() < 2)
             return;
-        for (int i = 1; i < defined_pos.size(); i++) {
+        for (const auto i: c10::irange(1, defined_pos.size())) {
             checkSameType(c, tensors[defined_pos[0]], tensors[defined_pos[i]]);
         }
     }
 }
```

### Comparing `tvdcn-0.3.3/tvdcn/csrc/tvdcn.cpp` & `tvdcn-0.4.0/tvdcn/csrc/tvdcn.cpp`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tvdcn/extension.py` & `tvdcn-0.4.0/tvdcn/extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import ctypes
 import importlib
 import os
 import sys
 from warnings import warn
 
 import torch
+from torch._classes import _ClassNamespace
+from torch._ops import _OpNamespace
+
+extension_namespace = os.path.basename(os.path.dirname(__file__))
 
 
 def _get_extension_path(lib_name):
     lib_dir = os.path.dirname(__file__)
     if os.name == 'nt':
         # Register the main library location on the default DLL path
         import ctypes
@@ -76,37 +80,40 @@
 
 
     def _has_ops():  # noqa: F811
         return True
 
 except (ImportError, OSError):
     pass
+finally:
+    _classes = _ClassNamespace(extension_namespace)
+    _ops = _OpNamespace(extension_namespace)
 
 
 def _assert_has_ops():
     if not _has_ops():
         raise RuntimeError(
             'Couldn\'t load custom C++ ops. Recompile C++ extension with:\n'
             '\tpython setup.py build_ext --inplace'
         )
 
 
 def _check_cuda_version(minor=True):
     """
-    Make sure that CUDA versions match between the pytorch install and tvdcn install
+    Make sure that CUDA versions match between the pytorch install and C++ extension install
 
     Args:
         minor (bool): If ``False``, ignore minor version difference.
          Defaults to ``True``.
     """
     if not _HAS_OPS:
         return -1
     from torch.version import cuda as torch_version_cuda
 
-    _version = torch.ops.tvdcn._cuda_version()
+    _version = _ops._cuda_version()
     if _version != -1 and torch_version_cuda is not None:
         ext_version = str(_version)
         if int(ext_version) < 10000:
             ext_major = int(ext_version[0])
             ext_minor = int(ext_version[2])
         else:
             ext_major = int(ext_version[0:2])
@@ -157,15 +164,15 @@
 
 def cuda_version():
     """
     Get compiled Cuda version.
     """
     if not _HAS_OPS:
         return -1
-    return torch.ops.tvdcn._cuda_version()
+    return _ops._cuda_version()
 
 
 def with_cuda():
     """
     Check if C++ extension is compiled with Cuda.
     """
     return cuda_version() != -1
```

### Comparing `tvdcn-0.3.3/tvdcn/ops/activations/mask_sigmoid.py` & `tvdcn-0.4.0/tvdcn/ops/activations/mask_sigmoid.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tvdcn/ops/activations/mask_softmax.py` & `tvdcn-0.4.0/tvdcn/ops/activations/mask_softmax.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tvdcn/ops/deform_conv.py` & `tvdcn-0.4.0/tvdcn/ops/deform_conv.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tvdcn/ops/deform_conv_transpose.py` & `tvdcn-0.4.0/tvdcn/ops/deform_conv_transpose.py`

 * *Files identical despite different names*

### Comparing `tvdcn-0.3.3/tvdcn/utils.py` & `tvdcn-0.4.0/tvdcn/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
+import os
 from types import FunctionType
 from typing import Any
 
 import torch
 
+extension_namespace = os.path.basename(os.path.dirname(__file__))
+
 
 def _log_api_usage_once(obj: Any) -> None:
     """
     Logs API usage(module and name) within an organization.
     In a large ecosystem, it's often useful to track the PyTorch and
-    TorchVision APIs usage. This API provides the similar functionality to the
+    Extension APIs usage. This API provides the similar functionality to the
     logging module in the Python stdlib. It can be used for debugging purpose
     to log which methods are used and by default it is inactive, unless the user
     manually subscribes a logger via the `SetAPIUsageLogger method <https://github.com/pytorch/pytorch/blob/eb3b9fe719b21fae13c7a7cf3253f970290a573e/c10/util/Logging.cpp#L114>`_.
     Please note it is triggered only once for the same API call within a process.
     It does not collect any data from open-source users since it is no-op by default.
     For more information, please refer to
     * PyTorch note: https://pytorch.org/docs/stable/notes/large_scale_deployments.html#api-usage-logging;
     * Logging policy: https://github.com/pytorch/vision/issues/5052;
     Args:
         obj (class instance or method): an object to extract info from.
     """
     module = obj.__module__
-    if not module.startswith('tvdcn'):
-        module = f'tvdcn.internal.{module}'
+    if not module.startswith(extension_namespace):
+        module = f'{extension_namespace}.internal.{module}'
     name = obj.__class__.__name__
     if isinstance(obj, FunctionType):
         name = obj.__name__
     torch._C._log_api_usage_once(f'{module}.{name}')
```

### Comparing `tvdcn-0.3.3/tvdcn.egg-info/PKG-INFO` & `tvdcn-0.4.0/tvdcn.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tvdcn
-Version: 0.3.3
+Version: 0.4.0
 Summary: Torchvision+ Deformable Convolutional Networks
 Home-page: https://github.com/inspiros/tvdcn
 Author: Hoang-Nhat Tran (inspiros)
 Author-email: hnhat.tran@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/inspiros/tvdcn
 Keywords: deform_conv; deformable convolution
@@ -32,35 +32,32 @@
 
 Torchvision+ Deformable Convolution Networks
 ========
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/inspiros/tvdcn/build_wheels.yml)](https://github.com/inspiros/tvdcn/actions)
 [![PyPI](https://img.shields.io/pypi/v/tvdcn)](https://pypi.org/project/tvdcn)
 [![GitHub](https://img.shields.io/github/license/inspiros/tvdcn)](LICENSE.txt)
 
-This package contains the PyTorch implementations of the **2D Deformable Convolution** operation
+This package contains the PyTorch implementations of the **Deformable Convolution** operation
 (the commonly used  `torchvision.ops.deform_conv2d`) proposed in https://arxiv.org/abs/1811.11168,
-as well as its **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
-
-And beyond that, the package also provides the **transposed** versions of them,
-which interestingly noone has ever proposed to use.
-The main idea is, while `offset` in deformable convolution guides the convolution kernel where to get the inputs to
-compute the output; in transposed deformable convolution, it guides the convolution kernel where to write the outputs.
+and the **Transposed Deformable Convolution** proposed in https://arxiv.org/abs/2210.09446
+(currently without interpolation kernel scaling).
+It also supports their **1D** and **3D** equivalences, which are not available in `torchvision` (thus the name).
 
 ## Highlights
 
 - **Supported operations:** _(All are implemented in C++/Cuda)_
 
   - `tvdcn.ops.deform_conv1d`
   - `tvdcn.ops.deform_conv2d`
   - `tvdcn.ops.deform_conv3d`
   - `tvdcn.ops.deform_conv_transpose1d`
   - `tvdcn.ops.deform_conv_transpose2d`
   - `tvdcn.ops.deform_conv_transpose3d`
 
-- And the following **supplementary operations** (for activating `mask`):
+- And the following **supplementary operations** (`mask` activation proposed in https://arxiv.org/abs/2211.05778):
   - `tvdcn.ops.mask_softmax1d`
   - `tvdcn.ops.mask_softmax2d`
   - `tvdcn.ops.mask_softmax3d`
 
 - Both `offset` and `mask` can be turned off, and can be applied in separate groups.
 
 - All the `nn.Module` wrappers for these operations are implemented,
```

