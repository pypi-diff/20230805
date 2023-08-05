# Comparing `tmp/colossalai-nightly-2023.7.8.tar.gz` & `tmp/colossalai-nightly-2023.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colossalai-nightly-2023.7.8.tar", last modified: Sat Jul  8 00:17:20 2023, max compression
+gzip compressed data, was "colossalai-nightly-2023.8.5.tar", last modified: Sat Aug  5 00:14:59 2023, max compression
```

## Comparing `colossalai-nightly-2023.7.8.tar` & `colossalai-nightly-2023.8.5.tar`

### file list

```diff
@@ -1,955 +1,949 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/
--rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    20789 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_C/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_C/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_meta_registration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_monkey_patch.py
--rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/meta_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/envs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/graph_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/node_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/graph_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/symbolic_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/tracer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.926462 colossalai-nightly-2023.7.8/colossalai/amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/amp_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/apex_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_fp16_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
--rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/naive_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/_grad_scaler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/torch_amp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/build_c_ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
--rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/operation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.930462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/amp_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/base_offload_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/mem_optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region.py
--rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/training_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_apply_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    22686 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/pipeline_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/pipeline_shard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.934462 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.938463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4033 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.942463 colossalai-nightly-2023.7.8/colossalai/booster/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/accelerator.py
--rw-r--r--   0 runner    (1001) docker     (123)    12659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/booster.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/bf16.py
--rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_apex.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_naive.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp8.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/mixed_precision_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/booster/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/dp_plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15137 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/gemini_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9752 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/low_level_zero_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2327 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/plugin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6820 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_ddp_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8877 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_fsdp_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/builder/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/builder/builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/checkpoint_io_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/general_checkpoint_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/index_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    22100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/checkpoint_io/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/benchmark/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.946463 colossalai-nightly-2023.7.8/colossalai/cli/check/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/check/check_installation.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/cli/launcher/
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/hostinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/multinode_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cli/launcher/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/cluster/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/device_mesh_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/dist_coordinator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/cluster/process_group_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/communication/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/collective.py
--rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/p2p.py
--rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/p2p_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/ring.py
--rw-r--r--   0 runner    (1001) docker     (123)     5095 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/communication/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/context/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/moe_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/parallel_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/parallel_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.950464 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/process_group_initializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/context/random/
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/random/seed_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/context/singleton_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/device/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/alpha_beta_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/calc_pipeline_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/device/device_mesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/_base_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.954464 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_base_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/engine/schedule/
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_base_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_non_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_compatibility.py
--rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_12.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_13.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/codegen/activation_checkpoint_codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/graph_module.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/adding_split_node_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/concrete_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/meta_info_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/passes_for_gpt2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/shard_1d_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/split_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/passes/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.958464 colossalai-nightly-2023.7.8/colossalai/fx/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/dataflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/memory_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/opcount.py
--rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/shard_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/profiler/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_meta_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_symbolic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/_tracer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.962465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/experimental.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/fx/tracer/tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/global_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/initialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/interface/optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/kernel/
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.966465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.970465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/
--rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/compat.h
--rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.970465 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/
--rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
--rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/
--rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
--rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
--rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
--rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
--rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
--rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
--rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/type_shim.h
--rw-r--r--   0 runner    (1001) docker     (123)    24864 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/layer_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/multihead_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/scaled_softmax.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/jit/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_dropout_add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_gelu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/jit/option.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/lazy/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/lazy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23592 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/lazy/lazy_init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/logging/
--rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/logging/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.974466 colossalai-nightly-2023.7.8/colossalai/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/_ops/
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/addmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/batch_norm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/element_wise.py
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/_ops/view.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/base_layer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/normalization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/experts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/routers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.978466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/loss/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_1d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_3d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/delayed.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/multistep.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/onecycle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/poly.py
--rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.982466 colossalai-nightly-2023.7.8/colossalai/nn/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2d.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2p5d.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_3d.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/colossalai_optimizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/hybrid_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lars.py
--rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/optimizer/nvme_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/data_parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.986467 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
--rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/colo_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/module_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/nn/parallel/reducer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/layer_spec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/fx.py
--rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/topo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/pipelinable.py
--rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/pipeline_process_group.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/pipeline/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/registry/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/registry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/registry/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/_operation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/parallel_module.py
--rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/qkv_fused_linear.py
--rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/layer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.990467 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/bloom.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/autopolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/basepolicy.py
--rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/policies/vit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shard_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/sharder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shardformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/colo_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/colo_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    21790 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/compute_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.994467 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/comm_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/dist_spec_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/distspec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/op_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/param_op_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/process_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    36486 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/shape_consistency.py
--rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/sharding_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/tensor_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/pytest_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/random.py
--rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/testing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_base_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_checkpoint_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_commons_.py
--rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_log_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_lr_scheduler_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_metric_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/activation_checkpoint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/module_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.998468 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     9794 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/convertor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)     4813 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpoint_io/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/checkpointing.py
--rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/cuda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/base_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/data_parallel_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/moe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/profiler/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/comm_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/pcie_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/prof_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/rank_recorder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/tensor_detector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/utils/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/zero/
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.002468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/search_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/colo_init_context.py
--rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)    29879 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_optimizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/gemini/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/
--rw-r--r--   0 runner    (1001) docker     (123)      466 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/gemini_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
--rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/init_context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.006468 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/commons.py
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/zero_hook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_param.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9957 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      410 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/base_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/bucket_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/gradient_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     3353 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/parameter_store.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    26595 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/low_level/low_level_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/colossalai/zero/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.010469 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39364 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-08 00:17:19.000000 colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/op_builder/
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/cpu_adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/fused_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/layernorm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/moe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/multi_head_attn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/scaled_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/scaled_upper_triangle_masked_softmax.py
--rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/op_builder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/requirements/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:19.922461 colossalai-nightly-2023.7.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/components_to_test/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/beit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/hanging_param_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/inline_op_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/nested_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/repeated_computed_layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/resnet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/simple_net.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/components_to_test/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/dummy_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/components_to_test/utils/executor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/diffusers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/timm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/torchaudio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/torchrec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.014469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/albert.py
--rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/t5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_bias_addition.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_mod_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_nested_ckpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_shape_prop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_symbolic_profile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/zoo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_aten.py
--rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_meta_mode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.018469 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.022470 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.022470 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
--rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
--rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/tests/test_shardformer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:20.026470 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bloom.py
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_gpt2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_llama.py
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_t5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_vit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/tests/test_shardformer/test_with_torch_ddp.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-08 00:17:06.000000 colossalai-nightly-2023.7.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.365292 colossalai-nightly-2023.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    22244 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-05 00:14:59.365292 colossalai-nightly-2023.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    21486 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/_C/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_C/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20609 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/_meta_registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/_monkey_patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18694 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/meta_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/envs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18761 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9920 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/graph_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8526 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/node_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/passes/graph_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9892 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/passes/shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/symbolic_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1107 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/custom_leaf_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15758 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/tracer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/amp_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/amp/apex_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/apex_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/apex_amp/apex_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13454 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/_fp16_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4755 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2596 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6098 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/naive_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26520 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/_grad_scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3344 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/torch_amp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/build_c_ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7716 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18543 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/operation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.281289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.285289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4050 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7900 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25633 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9721 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7399 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/where.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/shard_metainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.285289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7003 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/amp_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/base_offload_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/mem_optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/region.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20381 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/region_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10128 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18888 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18549 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/training_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.285289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/comm_metainfo_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/runtime_apply_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22684 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/runtime_preparation_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.285289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/pipeline_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/pipeline_shard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.285289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2662 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18744 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.289289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4187 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5270 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6009 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12452 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14746 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20532 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16514 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.289289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5258 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24314 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12308 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9295 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43483 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3727 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19134 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5041 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13270 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4031 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3835 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10911 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/sharding_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.293289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9989 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5784 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20520 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9158 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.293289 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9116 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/reshape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/sharding.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.293289 colossalai-nightly-2023.8.5/colossalai/booster/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/accelerator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/booster.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.293289 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/bf16.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp16_apex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp16_naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp16_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp8.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/mixed_precision_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.293289 colossalai-nightly-2023.8.5/colossalai/booster/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/dp_plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18997 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/gemini_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13170 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/low_level_zero_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/plugin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/torch_ddp_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8906 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/booster/plugin/torch_fsdp_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/builder/builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/checkpoint_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/checkpoint_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15021 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/checkpoint_io/checkpoint_io_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/checkpoint_io/general_checkpoint_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/checkpoint_io/index_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23714 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/checkpoint_io/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/cli/benchmark/
+-rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/benchmark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/benchmark/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/benchmark/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4859 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/benchmark/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/cli/check/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8495 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/check/check_installation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/cli/launcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/launcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/launcher/hostinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/launcher/multinode_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10034 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cli/launcher/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/cluster/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4207 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cluster/device_mesh_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7307 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cluster/dist_coordinator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/cluster/process_group_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/communication/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/communication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/communication/collective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19462 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/communication/p2p.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/communication/p2p_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/communication/ring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5096 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/communication/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.297289 colossalai-nightly-2023.8.5/colossalai/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/moe_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23924 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/parallel_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/parallel_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6239 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12842 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/process_group_initializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/context/random/
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/random/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/random/_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/random/seed_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/context/singleton_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/device/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/device/alpha_beta_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/device/calc_pipeline_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23687 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/device/device_mesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7864 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/_base_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/engine/gradient_accumulation/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_accumulation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_accumulation/_gradient_accumulation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_base_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2100 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_moe_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_zero_gradient_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.301290 colossalai-nightly-2023.8.5/colossalai/engine/schedule/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/schedule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/schedule/_base_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3876 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/schedule/_non_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41258 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/schedule/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/engine/schedule/_pipeline_schedule_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.305290 colossalai-nightly-2023.8.5/colossalai/fx/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/_compatibility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19408 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/_meta_regist_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/_meta_regist_13.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.305290 colossalai-nightly-2023.8.5/colossalai/fx/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44753 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/codegen/activation_checkpoint_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7373 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/graph_module.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.305290 colossalai-nightly-2023.8.5/colossalai/fx/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/adding_split_node_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12179 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/concrete_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13967 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/meta_info_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16288 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/passes_for_gpt2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6821 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/shard_1d_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14022 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/split_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/passes/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.305290 colossalai-nightly-2023.8.5/colossalai/fx/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/dataflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.305290 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7047 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.305290 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6632 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1591 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/torch_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/memory_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13226 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/opcount.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15387 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/shard_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/profiler/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/_meta_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/_symbolic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/_tracer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26969 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/experimental.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.309290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.313290 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/activation_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/convolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6769 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/pooling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24624 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/fx/tracer/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/global_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21027 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/initialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.313290 colossalai-nightly-2023.8.5/colossalai/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/interface/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/interface/optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.313290 colossalai-nightly-2023.8.5/colossalai/kernel/
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.313290 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.313290 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/
+-rw-r--r--   0 runner    (1001) docker     (123)     2606 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/compat.h
+-rw-r--r--   0 runner    (1001) docker     (123)    16815 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5187 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/cpu_adam.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.317290 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)     7526 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    37586 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.317290 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/
+-rw-r--r--   0 runner    (1001) docker     (123)     8585 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/context.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3415 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+-rw-r--r--   0 runner    (1001) docker     (123)    48403 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13619 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4877 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    26286 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5046 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     5200 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    13278 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    13114 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     6478 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    16988 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21701 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22850 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu
+-rw-r--r--   0 runner    (1001) docker     (123)    14851 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/type_shim.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/layer_norm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.317290 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/mha/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/mha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/mha/flash_attn_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2534 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/mha/mem_eff_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/mha/mha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/mha/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/multihead_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6710 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/scaled_softmax.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.317290 colossalai-nightly-2023.8.5/colossalai/kernel/jit/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/jit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      893 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/jit/bias_dropout_add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/jit/bias_gelu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/jit/option.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/lazy/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/lazy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24273 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/lazy/lazy_init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)     1597 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7511 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/logging/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/nn/_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8713 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4153 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/addmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/batch_norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/element_wise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/embedding_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/_ops/view.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/nn/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/base_layer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6304 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/normalization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.321290 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8241 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/experts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9431 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/routers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49753 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34900 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50524 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37643 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50769 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22769 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2967 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51441 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6411 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2401 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/vanilla/
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/vanilla/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14535 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/vanilla/layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/layer/wrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/wrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/layer/wrapper/pipeline_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.325291 colossalai-nightly-2023.8.5/colossalai/nn/loss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/loss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_1d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5536 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6362 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_3d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.329291 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6171 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7800 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/delayed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/multistep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/onecycle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/poly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3687 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.329291 colossalai-nightly-2023.8.5/colossalai/nn/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/metric/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/metric/accuracy_2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/metric/accuracy_2p5d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/metric/accuracy_3d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.329291 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/colossalai_optimizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8234 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/fused_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/fused_lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/fused_sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7338 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/hybrid_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/lars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6778 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/optimizer/nvme_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.329291 colossalai-nightly-2023.8.5/colossalai/nn/parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/data_parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.329291 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.329291 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28600 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/copyer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10057 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7481 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2020 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/colo_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/module_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/nn/parallel/reducer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/layer_spec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/adaptor/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/adaptor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6154 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/adaptor/fx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7051 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/topo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11415 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/pipelinable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/pipeline_process_group.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59170 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/_pipeline_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14859 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/_pipeline_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9012 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/pipeline/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/registry/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/registry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/registry/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9628 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/_operation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3544 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12750 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14617 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8789 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/parallel_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20697 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/qkv_fused_linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/layer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.333291 colossalai-nightly-2023.8.5/colossalai/shardformer/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3955 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/modeling/bloom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.337291 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6168 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/autopolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6266 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/basepolicy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12461 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8385 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6139 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5183 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/policies/vit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.337291 colossalai-nightly-2023.8.5/colossalai/shardformer/shard/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/shard/shard_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7140 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/shard/sharder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/shardformer/shard/shardformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.337291 colossalai-nightly-2023.8.5/colossalai/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4449 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/colo_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13185 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/colo_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21790 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/compute_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.337291 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14992 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11262 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/comm_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24565 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/layout_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9277 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3263 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8688 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/dist_spec_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/distspec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/op_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/param_op_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/process_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36486 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/shape_consistency.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11605 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/sharding_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/tensor_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.337291 colossalai-nightly-2023.8.5/colossalai/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5605 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/testing/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/testing/pytest_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/testing/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8629 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/testing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.337291 colossalai-nightly-2023.8.5/colossalai/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14776 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_base_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3247 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_checkpoint_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_commons_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13106 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_log_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_lr_scheduler_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16131 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_metric_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9856 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/activation_checkpoint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/checkpoint/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/checkpoint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/checkpoint/module_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/checkpoint/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11400 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/checkpointing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17450 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/cuda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/data_sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/data_sampler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/data_sampler/base_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7128 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/data_sampler/data_parallel_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6425 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3912 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/moe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/multi_tensor_apply/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/multi_tensor_apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/profiler/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10914 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/comm_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/pcie_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/prof_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8616 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/profiler/stateful_tensor_mem_extention.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/rank_recorder/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/rank_recorder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/rank_recorder/rank_recorder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.341291 colossalai-nightly-2023.8.5/colossalai/utils/tensor_detector/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/tensor_detector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/tensor_detector/tensor_detector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/utils/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22079 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9531 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6714 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/search_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/colo_init_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37822 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6627 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33517 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_optimizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3980 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/memory_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/memory_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/param_runtime_order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10482 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4168 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/gemini/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/
+-rw-r--r--   0 runner    (1001) docker     (123)      466 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/gemini_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.345291 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4814 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/paramhooks/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/paramhooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/stateful_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6449 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/tensor_placement_policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/tensor_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/legacy/init_ctx/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/init_ctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11385 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/init_ctx/init_context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/base_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/commons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/reduce_scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29261 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/sharded_model_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/zero_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_optim/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_optim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19215 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_param/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_param/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_param/sharded_param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_param/sharded_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9464 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/base_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3739 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/bucket_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/gradient_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/parameter_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/tensor_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24933 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/low_level/low_level_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/colossalai/zero/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.349292 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    26192 2023-08-05 00:14:59.000000 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39129 2023-08-05 00:14:59.000000 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 00:14:59.000000 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-08-05 00:14:59.000000 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-05 00:14:59.000000 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-08-05 00:14:59.000000 colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/op_builder/
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8943 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/cpu_adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/fused_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/layernorm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/moe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/multi_head_attn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/scaled_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/scaled_upper_triangle_masked_softmax.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8210 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/op_builder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/requirements/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 00:14:59.365292 colossalai-nightly-2023.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6229 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.277289 colossalai-nightly-2023.8.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/components_to_test/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1396 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/beit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3270 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2857 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/hanging_param_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/inline_op_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/nested_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1401 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/repeated_computed_layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1183 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/resnet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1587 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/simple_net.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/components_to_test/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/utils/dummy_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/components_to_test/utils/executor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/diffusers/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/diffusers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/diffusers/diffusers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/timm/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/timm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7513 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/timm/timm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchaudio/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchaudio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5409 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchaudio/torchaudio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchrec/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchrec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchrec/torchrec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.353292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchvision/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchvision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchvision/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4023 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/albert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7419 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/t5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_analyzer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4330 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_bias_addition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_mod_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_nested_ckpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_shape_prop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_symbolic_profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/zoo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/test_aten.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1925 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/test_flop_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/test_meta_mode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_auto_parallel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_pass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_pass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1806 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_pass/test_node_converting_pass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4172 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.357292 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11050 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2053 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.361292 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11552 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7693 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4842 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6740 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6205 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12886 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11802 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8173 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4372 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13108 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8356 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2623 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18730 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3153 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9001 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12527 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3556 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8918 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.361292 colossalai-nightly-2023.8.5/tests/test_shardformer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:59.361292 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_bert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_bloom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_gpt2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_llama.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_t5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_vit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/tests/test_shardformer/test_with_torch_ddp.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-05 00:14:48.000000 colossalai-nightly-2023.8.5/version.txt
```

### Comparing `colossalai-nightly-2023.7.8/LICENSE` & `colossalai-nightly-2023.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/PKG-INFO` & `colossalai-nightly-2023.8.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.7.8
+Version: 2023.8.5
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -32,22 +32,23 @@
         
         
            | [English](README.md) | [中文](docs/README-zh-Hans.md) |
         
         </div>
         
         ## Latest News
+        * [2023/07] [HPC-AI Tech Raises 22 Million USD in Series A Funding](https://www.hpc-ai.tech/blog/hpc-ai-tech-raises-22-million-usd-in-series-a-funding-to-fuel-team-expansion-and-business-growth)
+        * [2023/07] [65B Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
         * [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
         * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana)
         * [2023/03] [AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs)
         * [2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt)
         * [2023/01] [Hardware Savings Up to 46 Times for AIGC and  Automatic Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02)
         * [2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper)
         * [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding)
-        * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
         
         ## Table of Contents
         <ul>
          <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
          <li><a href="#Features">Features</a> </li>
          <li>
            <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
@@ -56,14 +57,15 @@
              <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
              <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
            </ul>
          </li>
          <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
+             <li><a href="#LLaMA">LLaMA</a></li>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
              <li><a href="#ViT">ViT</a></li>
              <li><a href="#Recommendation-System-Models">Recommendation System Models</a></li>
@@ -223,14 +225,23 @@
         - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
         
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Parallel Training Demo
         
+        ### LLaMA
+        <p align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/images/LLaMA_pretraining.png" width=600/>
+        </p>
+        
+        - 65-billion-parameter large model pretraining accelerated by 38%
+        [[code]](https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/llama)
+        [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining)
+        
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
         - Save 50% GPU resources and 10.7% acceleration
         
@@ -459,15 +470,16 @@
           title={Colossal-AI: A Unified Deep Learning System For Large-Scale Parallel Training},
           author={Bian, Zhengda and Liu, Hongxin and Wang, Boxiang and Huang, Haichen and Li, Yongbin and Wang, Chuanrui and Cui, Fan and You, Yang},
           journal={arXiv preprint arXiv:2110.14883},
           year={2021}
         }
         ```
         
-        Colossal-AI has been accepted as official tutorial by top conferences [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/Conferences/AAAI-23/), [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), etc.
+        Colossal-AI has been accepted as official tutorial by top conferences [NeurIPS](https://nips.cc/), [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/Conferences/AAAI-23/), 
+        [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), [NVIDIA GTC](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-S51482/) ,etc.
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.8 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.8.5 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -22,43 +22,47 @@
  (https://img.shields.io/badge/%F0%9F%A4%97HuggingFace-Join-yellow)](https://
 huggingface.co/hpcai-tech) [![slack badge](https://img.shields.io/badge/Slack-
   join-blueviolet?logo=slack&)](https://join.slack.com/t/colossalaiworkspace/
   shared_invite/zt-z7b26eeb-CBp7jouvu~r0~lcFzX832w) [![WeChat badge](https://
        img.shields.io/badge/å¾®ä¿¡-å å¥-green?logo=wechat&)](https://
     raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
     WeChat.png) | [English](README.md) | [ä¸­æ](docs/README-zh-Hans.md) |
-## Latest News * [2023/03] [ColossalChat: An Open-Source Solution for Cloning
-ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/
-colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-
-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver
-Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction]
-(https://www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund
-Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-
-google-fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source
-Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU
-Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
+## Latest News * [2023/07] [HPC-AI Tech Raises 22 Million USD in Series A
+Funding](https://www.hpc-ai.tech/blog/hpc-ai-tech-raises-22-million-usd-in-
+series-a-funding-to-fuel-team-expansion-and-business-growth) * [2023/07] [65B
+Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like
+Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
+* [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a
+Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-
+open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-
+5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-
+Efficient Open-Source Solution for Protein Folding Structure Prediction](https:
+//www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund Colossal-
+AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-
+fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source Solution
+Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory]
+(https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
 Savings Up to 46 Times for AIGC and Automatic Parallelism](https://medium.com/
 pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-
 savings-up-to-46x-for-stable-1453b48f3f02) * [2022/11] [Diffusion Pretraining
 and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/
 blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper) *
 [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
-09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
-/www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
-fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
+analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) ## Table
+of Contents
     * Why_Colossal-AI
     * Features
     * Colossal-AI_for_Real_World_Applications
           o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
             Complete_RLHF_Pipeline
           o AIGC:_Acceleration_of_Stable_Diffusion
           o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
+          o LLaMA
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
           o Recommendation_System_Models
@@ -151,15 +155,20 @@
 - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
 acceleration and 39% cost reduce.
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                            xTrimoMultimer_Table.jpg]
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
 accelerating structure prediction of protein monomers and multimer by 11x.
                                                                   (back_to_top)
-## Parallel Training Demo ### GPT-3
+## Parallel Training Demo ### LLaMA
+   [https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/
+                         images/LLaMA_pretraining.png]
+- 65-billion-parameter large model pretraining accelerated by 38% [[code]]
+(https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/
+llama) [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining) ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
 main/colossalai/img/(updated)GPT-2.png] - 24x larger model size on the same
@@ -281,16 +290,18 @@
 like to credit these amazing projects as listed in the [Reference List](./docs/
 REFERENCE.md). To cite this project, you can use the following BibTeX citation.
 ``` @article{bian2021colossal, title={Colossal-AI: A Unified Deep Learning
 System For Large-Scale Parallel Training}, author={Bian, Zhengda and Liu,
 Hongxin and Wang, Boxiang and Huang, Haichen and Li, Yongbin and Wang, Chuanrui
 and Cui, Fan and You, Yang}, journal={arXiv preprint arXiv:2110.14883}, year=
 {2021} } ``` Colossal-AI has been accepted as official tutorial by top
-conferences [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/
-Conferences/AAAI-23/), [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://
-cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), etc.
+conferences [NeurIPS](https://nips.cc/), [SC](https://sc22.supercomputing.org/
+), [AAAI](https://aaai.org/Conferences/AAAI-23/), [PPoPP](https://
+ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://
+www.isc-hpc.com/), [NVIDIA GTC](https://www.nvidia.com/en-us/on-demand/session/
+gtcspring23-S51482/) ,etc.
                                                                   (back_to_top)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 GPU :: NVIDIA CUDA Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: System :: Distributed Computing Requires-
 Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `colossalai-nightly-2023.7.8/README.md` & `colossalai-nightly-2023.8.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,22 +21,23 @@
 
 
    | [English](README.md) | [中文](docs/README-zh-Hans.md) |
 
 </div>
 
 ## Latest News
+* [2023/07] [HPC-AI Tech Raises 22 Million USD in Series A Funding](https://www.hpc-ai.tech/blog/hpc-ai-tech-raises-22-million-usd-in-series-a-funding-to-fuel-team-expansion-and-business-growth)
+* [2023/07] [65B Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
 * [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
 * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana)
 * [2023/03] [AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs)
 * [2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt)
 * [2023/01] [Hardware Savings Up to 46 Times for AIGC and  Automatic Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02)
 * [2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper)
 * [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding)
-* [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
 
 ## Table of Contents
 <ul>
  <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
  <li><a href="#Features">Features</a> </li>
  <li>
    <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
@@ -45,14 +46,15 @@
      <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
      <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
    </ul>
  </li>
  <li>
    <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
    <ul>
+     <li><a href="#LLaMA">LLaMA</a></li>
      <li><a href="#GPT-3">GPT-3</a></li>
      <li><a href="#GPT-2">GPT-2</a></li>
      <li><a href="#BERT">BERT</a></li>
      <li><a href="#PaLM">PaLM</a></li>
      <li><a href="#OPT">OPT</a></li>
      <li><a href="#ViT">ViT</a></li>
      <li><a href="#Recommendation-System-Models">Recommendation System Models</a></li>
@@ -212,14 +214,23 @@
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
 
 
 <p align="right">(<a href="#top">back to top</a>)</p>
 
 ## Parallel Training Demo
 
+### LLaMA
+<p align="center">
+<img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/images/LLaMA_pretraining.png" width=600/>
+</p>
+
+- 65-billion-parameter large model pretraining accelerated by 38%
+[[code]](https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/llama)
+[[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining)
+
 ### GPT-3
 <p align="center">
 <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
 </p>
 
 - Save 50% GPU resources and 10.7% acceleration
 
@@ -448,10 +459,11 @@
   title={Colossal-AI: A Unified Deep Learning System For Large-Scale Parallel Training},
   author={Bian, Zhengda and Liu, Hongxin and Wang, Boxiang and Huang, Haichen and Li, Yongbin and Wang, Chuanrui and Cui, Fan and You, Yang},
   journal={arXiv preprint arXiv:2110.14883},
   year={2021}
 }
 ```
 
-Colossal-AI has been accepted as official tutorial by top conferences [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/Conferences/AAAI-23/), [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), etc.
+Colossal-AI has been accepted as official tutorial by top conferences [NeurIPS](https://nips.cc/), [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/Conferences/AAAI-23/), 
+[PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), [NVIDIA GTC](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-S51482/) ,etc.
 
 <p align="right">(<a href="#top">back to top</a>)</p>
```

#### html2text {}

```diff
@@ -15,43 +15,47 @@
  (https://img.shields.io/badge/%F0%9F%A4%97HuggingFace-Join-yellow)](https://
 huggingface.co/hpcai-tech) [![slack badge](https://img.shields.io/badge/Slack-
   join-blueviolet?logo=slack&)](https://join.slack.com/t/colossalaiworkspace/
   shared_invite/zt-z7b26eeb-CBp7jouvu~r0~lcFzX832w) [![WeChat badge](https://
        img.shields.io/badge/å¾®ä¿¡-å å¥-green?logo=wechat&)](https://
     raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
     WeChat.png) | [English](README.md) | [ä¸­æ](docs/README-zh-Hans.md) |
-## Latest News * [2023/03] [ColossalChat: An Open-Source Solution for Cloning
-ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/
-colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-
-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver
-Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction]
-(https://www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund
-Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-
-google-fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source
-Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU
-Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
+## Latest News * [2023/07] [HPC-AI Tech Raises 22 Million USD in Series A
+Funding](https://www.hpc-ai.tech/blog/hpc-ai-tech-raises-22-million-usd-in-
+series-a-funding-to-fuel-team-expansion-and-business-growth) * [2023/07] [65B
+Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like
+Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
+* [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a
+Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-
+open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-
+5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-
+Efficient Open-Source Solution for Protein Folding Structure Prediction](https:
+//www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund Colossal-
+AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-
+fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source Solution
+Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory]
+(https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
 Savings Up to 46 Times for AIGC and Automatic Parallelism](https://medium.com/
 pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-
 savings-up-to-46x-for-stable-1453b48f3f02) * [2022/11] [Diffusion Pretraining
 and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/
 blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper) *
 [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
-09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
-/www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
-fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
+analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) ## Table
+of Contents
     * Why_Colossal-AI
     * Features
     * Colossal-AI_for_Real_World_Applications
           o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
             Complete_RLHF_Pipeline
           o AIGC:_Acceleration_of_Stable_Diffusion
           o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
+          o LLaMA
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
           o Recommendation_System_Models
@@ -144,15 +148,20 @@
 - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
 acceleration and 39% cost reduce.
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                            xTrimoMultimer_Table.jpg]
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
 accelerating structure prediction of protein monomers and multimer by 11x.
                                                                   (back_to_top)
-## Parallel Training Demo ### GPT-3
+## Parallel Training Demo ### LLaMA
+   [https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/
+                         images/LLaMA_pretraining.png]
+- 65-billion-parameter large model pretraining accelerated by 38% [[code]]
+(https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/
+llama) [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining) ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
 main/colossalai/img/(updated)GPT-2.png] - 24x larger model size on the same
@@ -274,11 +283,13 @@
 like to credit these amazing projects as listed in the [Reference List](./docs/
 REFERENCE.md). To cite this project, you can use the following BibTeX citation.
 ``` @article{bian2021colossal, title={Colossal-AI: A Unified Deep Learning
 System For Large-Scale Parallel Training}, author={Bian, Zhengda and Liu,
 Hongxin and Wang, Boxiang and Huang, Haichen and Li, Yongbin and Wang, Chuanrui
 and Cui, Fan and You, Yang}, journal={arXiv preprint arXiv:2110.14883}, year=
 {2021} } ``` Colossal-AI has been accepted as official tutorial by top
-conferences [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/
-Conferences/AAAI-23/), [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://
-cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), etc.
+conferences [NeurIPS](https://nips.cc/), [SC](https://sc22.supercomputing.org/
+), [AAAI](https://aaai.org/Conferences/AAAI-23/), [PPoPP](https://
+ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://
+www.isc-hpc.com/), [NVIDIA GTC](https://www.nvidia.com/en-us/on-demand/session/
+gtcspring23-S51482/) ,etc.
                                                                   (back_to_top)
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_meta_registration.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/_meta_registration.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/_monkey_patch.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/_monkey_patch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/flop_tensor.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/_subclasses/meta_tensor.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/_subclasses/meta_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/codegen.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/graph_module.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/node_util.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/node_util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/graph_profile.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/passes/graph_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/passes/shape_prop.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/passes/shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/symbolic_profile.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/bias_addition.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/custom_leaf_module.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/custom_leaf_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/proxy.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/symbolic_trace.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/_analyzer/fx/tracer/tracer.py` & `colossalai-nightly-2023.8.5/colossalai/_analyzer/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/amp/apex_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/apex_amp/apex_amp.py` & `colossalai-nightly-2023.8.5/colossalai/amp/apex_amp/apex_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_fp16_optimizer.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/_fp16_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/base_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/constant_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/grad_scaler/dynamic_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/base.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/mixed_precision_mixin/fp16.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/naive_amp/naive_amp.py` & `colossalai-nightly-2023.8.5/colossalai/amp/naive_amp/naive_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/_grad_scaler.py` & `colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/_grad_scaler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/amp/torch_amp/torch_amp.py` & `colossalai-nightly-2023.8.5/colossalai/amp/torch_amp/torch_amp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/ckpt_solver_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/ckpt_solver_chen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/ckpt_solver_rotor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/checkpoint/operation.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/checkpoint/operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/activation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/binary_elementwise_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/non_spmd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/meta_registry/where.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/meta_registry/where.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/registry.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/meta_profiler/shard_metainfo.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/meta_profiler/shard_metainfo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/amp_optimizer.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/amp_optimizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-from typing import Dict, Tuple
 from enum import Enum
+from typing import Dict, Tuple
+
 import torch
 from torch.optim import Optimizer
 
+from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
 from colossalai.logging import get_dist_logger
 from colossalai.nn.optimizer import ColossalaiOptimizer
-from colossalai.amp.naive_amp.grad_scaler import DynamicGradScaler
 from colossalai.utils import get_current_device
 
 from .base_offload_module import BaseOffloadModule
-from .region_manager import RegionManager
 from .region import Region
+from .region_manager import RegionManager
 
 
 class OptimState(Enum):
     SCALED = 0
     UNSCALED = 1
 
-class AMPOptimizer(ColossalaiOptimizer):
 
+class AMPOptimizer(ColossalaiOptimizer):
     """
     A wrapper for Optimizer.
     Code reference: https://github.com/hpcaitech/ColossalAI/blob/main/colossalai/nn/optimizer/zero_optimizer.py
 
     Args:
         optimizer (Optimizer): An Optimizer instance.
         module (BaseOffloadModule): A ``BaseOffloadModule`` instance.
@@ -170,8 +171,8 @@
                 if param in self.optim.state:
                     self.optim.state[fake_param] = self.optim.state.pop(param)
 
             group['params'] = fake_params_list
 
         # Leverage state_dict() and load_state_dict() to
         # recast preexisting per-param state tensors
-        self.optim.load_state_dict(self.optim.state_dict())
+        self.optim.load_state_dict(self.optim.state_dict())
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/base_offload_module.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/base_offload_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/mem_optimize.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/mem_optimize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/region.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/region_manager.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/region_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/runtime.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/runtime.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/solver.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/training_simulator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/training_simulator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/offload/util.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/offload/util.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/comm_metainfo_pass.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/comm_metainfo_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/meta_info_prop.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_apply_pass.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/runtime_apply_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/passes/runtime_preparation_pass.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/passes/runtime_preparation_pass.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                 size[dim] = dim_size * total_shard_size
         size = torch.Size(size)
 
     return size
 
 
 def solution_annotation_pass(gm: torch.fx.GraphModule, solution: List[int],
-                               strategies_constructor: StrategiesConstructor):
+                             strategies_constructor: StrategiesConstructor):
     """
     This method is used to stick the solution strategy to the nodes and add the information
     required in runtime into graph as placeholder nodes.
     """
     mod_graph = gm.graph
 
     nodes = [strategies_vector.node for strategies_vector in strategies_constructor.leaf_strategies]
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/constants.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/initialize.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/node_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/normal_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/permute_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/registry.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/batch_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/binary_elementwise_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/conv_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/embedding_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getattr_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/getitem_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/layer_norm_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/matmul_strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/normal_pooling_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/output_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/placeholder_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/reshape_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/softmax_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/strategy_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/sum_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/tensor_constructor_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/unary_elementwise_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import copy
 from typing import List
 
-from colossalai.auto_parallel.tensor_shard.sharding_strategy import (MemoryCost, ShardingStrategy, TrainCycleItem)
+from colossalai.auto_parallel.tensor_shard.sharding_strategy import MemoryCost, ShardingStrategy, TrainCycleItem
 
 from .strategy_generator import FollowingStrategyGenerator
 
 __all__ = ['UnaryElementwiseGenerator']
 
 
 class UnaryElementwiseGenerator(FollowingStrategyGenerator):
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/strategy/where_generator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/tensor_constructor_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/unary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/node_handler/where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/options.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/options.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/sharding_strategy.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/sharding_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/cost_graph.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/graph_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/solver.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/solver.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/solver/strategies_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/broadcast.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/factory.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/factory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/misc.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/misc.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/reshape.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/reshape.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/auto_parallel/tensor_shard/utils/sharding.py` & `colossalai-nightly-2023.8.5/colossalai/auto_parallel/tensor_shard/utils/sharding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/accelerator.py` & `colossalai-nightly-2023.8.5/colossalai/booster/accelerator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/booster.py` & `colossalai-nightly-2023.8.5/colossalai/booster/booster.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import torch
 import torch.nn as nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
 from colossalai.checkpoint_io import GeneralCheckpointIO
-from colossalai.interface import ModelWrapper
+from colossalai.interface import ModelWrapper, OptimizerWrapper
 
 from .accelerator import Accelerator
 from .mixed_precision import MixedPrecision, mixed_precision_factory
 from .plugin import Plugin
 
 __all__ = ['Booster']
 
@@ -149,26 +149,28 @@
                          return_loss: bool = True,
                          return_outputs: bool = False) -> Tuple[Optional[torch.Tensor], ...]:
         # TODO: implement this method
         # run pipeline forward backward pass
         # return loss or outputs if needed
         pass
 
-    def no_sync(self, model: nn.Module) -> contextmanager:
+    def no_sync(self, model: nn.Module = None, optimizer: OptimizerWrapper = None) -> contextmanager:
         """Context manager to disable gradient synchronization across DP process groups.
+           Support torch DDP and Low Level ZeRO-1 for now.
 
         Args:
-            model (nn.Module): The model to be disabled gradient synchronization.
+            model (nn.Module): The model to be disabled gradient synchronization, for DDP
+            optimizer (OptimizerWrapper): The optimizer to be disabled gradient synchronization, for ZeRO1-1
 
         Returns:
             contextmanager: Context to disable gradient synchronization.
         """
         assert self.plugin is not None, f'no_sync is only enabled when a plugin is provided and the plugin supports no_sync.'
-        assert self.plugin.support_no_sync, f'The plugin {self.plugin.__class__.__name__} does not support no_sync.'
-        return self.plugin.no_sync(model)
+        assert self.plugin.support_no_sync(), f'The plugin {self.plugin.__class__.__name__} does not support no_sync.'
+        return self.plugin.no_sync(model, optimizer)
 
     def load_model(self, model: Union[nn.Module, ModelWrapper], checkpoint: str, strict: bool = True):
         """Load model from checkpoint.
 
         Args:
             model (nn.Module or ModelWrapper): A model boosted by Booster.
             checkpoint (str): Path to the checkpoint. It must be a local path.
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_apex.py` & `colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp16_apex.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_naive.py` & `colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp16_naive.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/fp16_torch.py` & `colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/fp16_torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/mixed_precision/mixed_precision_base.py` & `colossalai-nightly-2023.8.5/colossalai/booster/mixed_precision/mixed_precision_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 class MixedPrecision(ABC):
     """
     An abstract class for mixed precision training.
     """
 
     @abstractmethod
-    def configure(self,
-                  model: nn.Module,
-                  optimizer: Optional[Optimizer] = None,
-                  criterion: Optional[Callable] = None,
-                  ) -> Tuple[nn.Module, OptimizerWrapper, Callable]:
+    def configure(
+        self,
+        model: nn.Module,
+        optimizer: Optional[Optimizer] = None,
+        criterion: Optional[Callable] = None,
+    ) -> Tuple[nn.Module, OptimizerWrapper, Callable]:
         # TODO: implement this method
         pass
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/plugin/dp_plugin_base.py` & `colossalai-nightly-2023.8.5/colossalai/booster/plugin/dp_plugin_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/plugin/gemini_plugin.py` & `colossalai-nightly-2023.8.5/colossalai/booster/plugin/gemini_plugin.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,35 @@
+import gc
 import logging
 import os
 import warnings
 from pathlib import Path
 from typing import Callable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
 from torch.utils.data import DataLoader
 
 from colossalai.checkpoint_io import CheckpointIndexFile, CheckpointIO, GeneralCheckpointIO
-from colossalai.checkpoint_io.utils import get_model_base_filenames, get_shard_filename, save_state_dict
+from colossalai.checkpoint_io.utils import (
+    get_model_base_filenames,
+    get_optimizer_base_filenames,
+    get_shard_filename,
+    load_shard_state_dict,
+    save_state_dict,
+    save_state_dict_shards,
+)
 from colossalai.cluster import DistCoordinator
 from colossalai.interface import ModelWrapper, OptimizerWrapper
 from colossalai.utils import get_current_device
 from colossalai.zero import GeminiDDP, zero_model_wrapper, zero_optim_wrapper
+from colossalai.zero.gemini import ZeroOptimizer
 from colossalai.zero.gemini.memory_tracer import MemStats
 
 from .dp_plugin_base import DPPluginBase
 
 __all__ = ['GeminiPlugin']
 
 SUPPORTED_PRECISION = ['fp16', 'bf16']
@@ -33,15 +42,15 @@
         super().__init__()
         self.coordinator = DistCoordinator()
 
     def save_unsharded_model(self, model: GeminiDDP, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
         """
         Save sharded model to checkpoint but only on master process.
         The model should be unwrapped in self.load_model via ModelWrapper.unwrap.
-        As there is communication when getting state dict, this must be called on all processes.
+        As there is communication when getting state dict, model.state_dict() must be called on all processes.
         """
         state_dict = model.state_dict(only_rank_0=True)
         if self.coordinator.is_master():
             save_state_dict(state_dict, checkpoint, use_safetensors)
 
     def load_unsharded_model(self, model: GeminiDDP, checkpoint: str, strict: bool = True):
         """
@@ -50,15 +59,15 @@
         """
         super().load_unsharded_model(model, checkpoint, strict=strict)
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save unsharded optimizer state dict to checkpoint.
         After calling optimizer.state_dict(), the complete optimizer states will be collected on master rank.
-        As there is communication when getting state dict, this must be called on all processes.
+        As there is communication when getting state dict, optimizer.state_dict() must be called on all processes.
         The saving process will only be executed by master rank.
         """
         state_dict = optimizer.state_dict()
         if self.coordinator.is_master():
             save_state_dict(state_dict, checkpoint, use_safetensors=False)
 
     def load_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str):
@@ -72,73 +81,147 @@
                            model: GeminiDDP,
                            checkpoint_path: str,
                            gather_dtensor: bool = False,
                            prefix: Optional[str] = None,
                            max_shard_size: int = 1024,
                            use_safetensors: bool = False):
         """
-        Save sharded model
+        Save sharded model.
+        As there is communication when getting state dict, model.state_dict() must be called on all processes.
         """
         if os.path.isfile(checkpoint_path):
             logging.error(f"Provided path ({checkpoint_path}) should be a directory, not a file")
             return
 
         Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
 
         state_dict_shard = model.state_dict_shard(max_shard_size=max_shard_size, only_rank_0=True, dtype=torch.float32)
         weights_name, save_index_file = get_model_base_filenames(prefix, use_safetensors)
-        total_size = 0
         index_file = CheckpointIndexFile(checkpoint_path)
-        for idx, shard_pair in enumerate(state_dict_shard):
-            if not self.coordinator.is_master():
-                continue
-            shard = shard_pair[0]
-            shard_file = get_shard_filename(weights_name, idx)
-            total_size = total_size + shard_pair[1]
-            for key in shard.keys():
-                index_file.append_weight_map(key, shard_file)
-
-            checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
-            save_state_dict(shard, checkpoint_file_path, use_safetensors)
 
-        index_file.append_meta_data("total_size", total_size)
+        # Save shards of optimizer states.
+        is_master = self.coordinator.is_master()
+        total_size = save_state_dict_shards(sharded_state_dict=state_dict_shard,
+                                            checkpoint=checkpoint_path,
+                                            index_file=index_file,
+                                            base_filename=weights_name,
+                                            is_master=is_master,
+                                            use_safetensors=use_safetensors)
 
         # only save the index file on the master rank
         if self.coordinator.is_master():
+            index_file.append_meta_data("total_size", total_size)
             index_file.write_index_file(save_index_file)
-        logging.info(f"The model is split into checkpoint shards. "
-                     f"You can find where each parameters has been saved in the "
-                     f"index located at {save_index_file}.")
+            logging.info(f"The model is split into checkpoint shards. "
+                         f"You can find where each parameters has been saved in the "
+                         f"index located at {save_index_file}.")
 
     def load_sharded_model(self,
                            model: GeminiDDP,
                            checkpoint_index_file: Path,
                            strict: bool = False,
                            use_safetensors: bool = False):
         """
-        load shard model, load model from multiple files
+        Load shard model, load model from multiple files.
         """
         return super().load_sharded_model(model, checkpoint_index_file, strict, use_safetensors, load_sub_module=False)
 
     def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: Path, gather_dtensor: bool, prefix: str,
                                size_per_shard: int):
         """
         Save sharded optimizer state dict to checkpoint folder.
         As there is communication when getting state dict, this must be called on all processes.
         """
+
+        # If optimizer is wrapped, unwrap it.
+        if isinstance(optimizer, OptimizerWrapper):
+            optimizer = optimizer.unwrap()
+
+        assert isinstance(optimizer, ZeroOptimizer)
+
+        if os.path.isfile(checkpoint):
+            logging.error(f"Provided path ({checkpoint}) should be a directory, not a file")
+            return
+
         Path(checkpoint).mkdir(parents=True, exist_ok=True)
-        super().save_sharded_optimizer(optimizer, checkpoint, gather_dtensor, prefix, size_per_shard)
+
+        # Preparing file paths and index file.
+        states_name, save_index_file, param_group_file = get_optimizer_base_filenames(prefix)
+        index_file = CheckpointIndexFile(checkpoint)
+
+        # Store the information of param groups to param_group_file.
+        index_file.append_meta_data("param_groups", param_group_file)
+        group_file_path = os.path.join(checkpoint, param_group_file)
+        param_groups = optimizer.get_param_groups_for_saving()
+        torch.save(param_groups, group_file_path)
+
+        # States are broken into shards within max_shard_size.
+        state_dict_shard = optimizer.state_shard(prefix=prefix, max_shard_size=size_per_shard, only_rank_0=True)
+
+        # Save shards of optimizer states.
+        is_master = self.coordinator.is_master()
+        total_size = save_state_dict_shards(sharded_state_dict=state_dict_shard,
+                                            checkpoint=checkpoint,
+                                            index_file=index_file,
+                                            base_filename=states_name,
+                                            is_master=is_master,
+                                            use_safetensors=False)
+
+        # Wrap up index file. Only save it on master rank.
+        if self.coordinator.is_master():
+            index_file.append_meta_data("total_size", total_size)
+            index_file.write_index_file(save_index_file)
+            logging.info(f"The optimizer is going to be split to checkpoint shards. "
+                         f"You can find where each parameters has been saved in the "
+                         f"index located at {save_index_file}.")
 
     def load_sharded_optimizer(self, optimizer: Optimizer, checkpoint_index_file: Path, prefix: str):
         """
         Loading sharded optimizer from checkpoint folder, with index file given.
         For each process, only loading optimizer states of parameters it controls.
         """
-        # TODO(Baizhou): To be implemented.
-        pass
+
+        if not os.path.isfile(checkpoint_index_file):
+            logging.error(f"Provided path ({checkpoint_index_file}) should be a file")
+
+        # If optimizer is wrapped, unwrap it.
+        if isinstance(optimizer, OptimizerWrapper):
+            optimizer = optimizer.unwrap()
+
+        assert isinstance(optimizer, ZeroOptimizer)
+
+        # Read checkpoint index file.
+        ckpt_index_file = CheckpointIndexFile.from_file(checkpoint_index_file)
+
+        # Load param_groups.
+        param_group_path = ckpt_index_file.get_param_group_filename()
+        if param_group_path is None:
+            raise RuntimeError(f'Invalid index file path {checkpoint_index_file} for an optimizer. \
+                               Lacking param group file under current directory.')
+        saved_param_groups = torch.load(param_group_path)
+        optimizer.load_param_groups(saved_param_groups)
+
+        checkpoint_files, _ = ckpt_index_file.get_checkpoint_filenames()
+
+        # Load optimizer states from shard files under checkpoint path.
+        # For each file, only load the states managed by current process.
+        for shard_file in checkpoint_files:
+            state_dict_shard = load_shard_state_dict(Path(shard_file), use_safetensors=False)
+            optimizer.load_param_states(state_dict_shard)
+            del state_dict_shard
+            gc.collect()
+
+        optimizer.optimizer_loading_epilogue()
+
+    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        if self.coordinator.is_master():
+            super().save_lr_scheduler(lr_scheduler, checkpoint)
 
 
 class GeminiModel(ModelWrapper):
 
     def __init__(self, module: nn.Module, gemini_config: dict, verbose: bool = False) -> None:
         super().__init__(module)
         self.module = zero_model_wrapper(module, zero_stage=3, gemini_config=gemini_config, verbose=verbose)
@@ -321,9 +404,9 @@
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return GeminiCheckpointIO()
 
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
         raise NotImplementedError
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/plugin/low_level_zero_plugin.py` & `colossalai-nightly-2023.8.5/colossalai/booster/plugin/torch_fsdp_plugin.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,196 +1,194 @@
 import warnings
-from functools import partial
-from typing import Callable, Iterator, List, Optional, Tuple, Union
+from pathlib import Path
+from typing import Callable, Iterable, Iterator, List, Optional, Tuple, Union
 
 import torch
 import torch.nn as nn
-from torch import Tensor
+from packaging import version
+from torch.distributed import ProcessGroup
+
+if version.parse(torch.__version__) >= version.parse('1.12.0'):
+    from torch.distributed.fsdp import FullStateDictConfig
+    from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
+    from torch.distributed.fsdp import StateDictType
+    from torch.distributed.fsdp.fully_sharded_data_parallel import (
+        BackwardPrefetch,
+        CPUOffload,
+        FullStateDictConfig,
+        MixedPrecision,
+        ShardingStrategy,
+    )
+else:
+    raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
+
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler as LRScheduler
-from torch.utils._pytree import tree_map
 from torch.utils.data import DataLoader
 
-from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO
+from colossalai.checkpoint_io import CheckpointIO, GeneralCheckpointIO, utils
+from colossalai.cluster import DistCoordinator
 from colossalai.interface import ModelWrapper, OptimizerWrapper
-from colossalai.utils import get_current_device
-from colossalai.zero import zero_model_wrapper, zero_optim_wrapper
 
 from .dp_plugin_base import DPPluginBase
-from .torch_ddp_plugin import TorchDDPCheckpointIO
 
-__all__ = ['LowLevelZeroPlugin']
+__all__ = ['TorchFSDPPlugin']
 
 
-def _convert_floating_point(x, dtype: torch.dtype = torch.float16):
-    if isinstance(x, torch.Tensor) and torch.is_floating_point(x):
-        return x.to(dtype)
-    return x
+class TorchFSDPCheckpointIO(GeneralCheckpointIO):
 
+    def __init__(self) -> None:
+        super().__init__()
+        self.coordinator = DistCoordinator()
 
-SUPPORTED_PRECISION = ['fp16', 'bf16', 'fp32']
-
+    def load_unsharded_model(self, model: nn.Module, checkpoint: str, strict: bool):
+        checkpoint = utils.load_state_dict(checkpoint)
+        model.load_state_dict(checkpoint)
+
+    def load_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: Path):
+        checkpoint = utils.load_state_dict(checkpoint)
+        fsdp_model = optimizer.unwrap_model()
+        sharded_osd = FSDP.scatter_full_optim_state_dict(checkpoint, fsdp_model)
+        optimizer.load_state_dict(sharded_osd)
 
-class LowLevelZeroCheckpointIO(TorchDDPCheckpointIO):
+    def save_unsharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, use_safetensors: bool):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        # the model should be unwrapped in self.load_model via ModelWrapper.unwrap
+        cfg = FullStateDictConfig(offload_to_cpu=True, rank0_only=True)
+        with FSDP.state_dict_type(model, StateDictType.FULL_STATE_DICT, cfg):
+            full_model_state = model.state_dict()
+        utils.save_state_dict(full_model_state, checkpoint_file_path=checkpoint, use_safetensors=use_safetensors)
 
     def save_unsharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool):
         """
         Save optimizer to checkpoint but only on master process.
         """
-        # TODO(ver217): optimizer state dict is sharded, and cannot get full state dict now
-        warnings.warn(
-            'LowLevelZeroPlugin does not support save full optimizer checkpoint now. Save it on every process.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        GeneralCheckpointIO.save_unsharded_optimizer(self, optimizer, checkpoint, gather_dtensor)
-
-    def load_optimizer(self, optimizer: Optimizer, checkpoint: str):
-        warnings.warn(
-            'LowLevelZeroPlugin can only load optimizer checkpoint saved by itself with the same number of processes.')
-        checkpoint = f'{checkpoint}.rank{self.coordinator.rank}'
-        super().load_optimizer(optimizer, checkpoint)
+        assert isinstance(optimizer, FSDPOptimizerWrapper)
+        fsdp_model = optimizer.unwrap_model()
+        full_optimizer_state = FSDP.full_optim_state_dict(fsdp_model, optim=optimizer, rank0_only=True)
+        utils.save_state_dict(full_optimizer_state, checkpoint_file_path=checkpoint, use_safetensors=False)
+
+    def save_sharded_model(self, model: nn.Module, checkpoint: str, gather_dtensor: bool, prefix: Optional[str],
+                           size_per_shard: int, use_safetensors: bool):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded model checkpoint is not supported yet.")
 
+    def load_sharded_model(self,
+                           model: nn.Module,
+                           checkpoint_index_file: Path,
+                           strict: bool = False,
+                           use_safetensors: bool = False,
+                           load_sub_module: bool = True):
+        """
+        Load model to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded model checkpoint is not supported yet.")
 
-class LowLevelZeroModel(ModelWrapper):
+    def save_sharded_optimizer(self, optimizer: Optimizer, checkpoint: str, gather_dtensor: bool, prefix: str,
+                               size_per_shard: int):
+        """
+        Save optimizer to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
 
-    def __init__(self, module: nn.Module, stage: int, precision: str) -> None:
+    def load_sharded_optimizer(self, optimizer: Optimizer, index_file_path: str, size_per_shard: int):
+        """
+        Load optimizer to checkpoint but only on master process.
+        """
+        raise NotImplementedError("Sharded optimizer checkpoint is not supported yet.")
+
+    def save_lr_scheduler(self, lr_scheduler: LRScheduler, checkpoint: str):
+        """
+        Save model to checkpoint but only on master process.
+        """
+        if self.coordinator.is_master():
+            super().save_lr_scheduler(lr_scheduler, checkpoint)
+
+
+class TorchFSDPModel(ModelWrapper):
+
+    def __init__(self, module: nn.Module, *args, **kwargs) -> None:
         super().__init__(module)
-        self.dtype = None
-        if precision == 'fp16':
-            self.dtype = torch.float16
-        elif precision == 'bf16':
-            self.dtype = torch.bfloat16
-        module = zero_model_wrapper(module, zero_stage=stage)
-        if self.dtype is not None:
-            module = module.to(self.dtype)
-        module = module.to(get_current_device())
-        self.module = module
-        self.convert_fn = None
-        if self.dtype is not None:
-            self.convert_fn = partial(_convert_floating_point, dtype=self.dtype)
-
-    def forward(self, *args, **kwargs):
-        if self.convert_fn is not None:
-            args = tree_map(self.convert_fn, args)
-            kwargs = tree_map(self.convert_fn, kwargs)
-        return super().forward(*args, **kwargs)
-
-
-class LowLevelZeroOptimizer(OptimizerWrapper):
-
-    def __init__(self,
-                 module: nn.Module,
-                 optimizer: Optimizer,
-                 zero_optim_config: dict,
-                 optim_kwargs: dict,
-                 verbose: bool = False) -> None:
-        optimizer = zero_optim_wrapper(module,
-                                       optimizer,
-                                       optim_config=zero_optim_config,
-                                       **optim_kwargs,
-                                       verbose=verbose)
-        super().__init__(optimizer)
+        self.module = FSDP(module, *args, **kwargs)
 
-    def backward(self, loss: Tensor, *args, **kwargs):
-        self.optim.backward(loss)
+    def unwrap(self):
+        return self.module
 
-    def clip_grad_by_norm(self,
-                          max_norm: Union[float, int],
-                          norm_type: Union[float, int] = 2,
-                          error_if_nonfinite: bool = False,
-                          *args,
-                          **kwargs) -> Tensor:
-        warnings.warn(f'LowLevelZero controls grad clipping by itself, so you should not use clip_grad_by_norm')
 
-    def clip_grad_by_value(self, clip_value: float, *args, **kwargs) -> None:
-        raise NotImplementedError('LowLevelZero does not support clip_grad_by_value')
+class FSDPOptimizerWrapper(OptimizerWrapper):
 
+    def __init__(self, optimizer: Optimizer, model: nn.Module):
+        self.model = model
+        super().__init__(optimizer)
 
-class LowLevelZeroPlugin(DPPluginBase):
+    def unwrap_model(self) -> nn.Module:
+        return self.model
+
+
+class TorchFSDPPlugin(DPPluginBase):
     """
-    Plugin for low level zero.
+    Plugin for PyTorch FSDP.
 
     Example:
         >>> from colossalai.booster import Booster
-        >>> from colossalai.booster.plugin import LowLevelZeroPlugin
+        >>> from colossalai.booster.plugin import TorchFSDPPlugin
         >>>
         >>> model, train_dataset, optimizer, criterion = ...
-        >>> plugin = LowLevelZeroPlugin()
+        >>> plugin = TorchFSDPPlugin()
 
-        >>> train_dataloader = plugin.prepare_dataloader(train_dataset, batch_size=8)
+        >>> train_dataloader = plugin.prepare_train_dataloader(train_dataset, batch_size=8)
         >>> booster = Booster(plugin=plugin)
         >>> model, optimizer, train_dataloader, criterion = booster.boost(model, optimizer, train_dataloader, criterion)
 
     Args:
-        strage (int, optional): ZeRO stage. Defaults to 1.
-        precision (str, optional): precision. Support 'fp16', 'bf16' and 'fp32'. Defaults to 'fp16'.
-        initial_scale (float, optional): Initial scale used by DynamicGradScaler. Defaults to 2**32.
-        min_scale (float, optional): Min scale used by DynamicGradScaler. Defaults to 1.
-        growth_factor (float, optional): growth_factor used by DynamicGradScaler. Defaults to 2.
-        backoff_factor (float, optional): backoff_factor used by DynamicGradScaler. Defaults to 0.5.
-        growth_interval (float, optional): growth_interval used by DynamicGradScaler. Defaults to 1000.
-        hysteresis (float, optional): hysteresis used by DynamicGradScaler. Defaults to 2.
-        max_scale (int, optional): max_scale used by DynamicGradScaler. Defaults to 2**32.
-        max_norm (float, optional): max_norm used for `clip_grad_norm`. You should notice that you shall not do
-            clip_grad_norm by yourself when using ZeRO DDP. The ZeRO optimizer will take care of clip_grad_norm.
-        norm_type (float, optional): norm_type used for `clip_grad_norm`.
-        reduce_bucket_size_in_m (int, optional): grad reduce bucket size in M. Defaults to 12.
-        communication_dtype (torch.dtype, optional): communication dtype. If not specified, the dtype of param will be used. Defaults to None.
-        overlap_communication (bool, optional): whether to overlap communication and computation. Defaults to True.
-        cpu_offload (bool, optional): whether to offload grad, master weight and optimizer state to cpu. Defaults to False.
-        verbose (bool, optional): verbose mode. Debug info including grad overflow will be printed. Defaults to False.
+        See https://pytorch.org/docs/stable/fsdp.html for details.
     """
 
-    def __init__(
-        self,
-        stage: int = 1,
-        precision: str = 'fp16',
-        initial_scale: float = 2**32,
-        min_scale: float = 1,
-        growth_factor: float = 2,
-        backoff_factor: float = 0.5,
-        growth_interval: int = 1000,
-        hysteresis: int = 2,
-        max_scale: float = 2**32,
-        max_norm: float = 0.0,
-        norm_type: float = 2.0,
-        reduce_bucket_size_in_m: int = 12,
-        communication_dtype: Optional[torch.dtype] = None,
-        overlap_communication: bool = True,
-        cpu_offload: bool = False,
-        verbose: bool = False,
-    ) -> None:
-        super().__init__()
-        assert stage in (1, 2), f'LowLevelZeroPlugin only supports stage 1/2 training'
-        assert precision in SUPPORTED_PRECISION, f'LowLevelZeroPlugin only supports {SUPPORTED_PRECISION} training'
+    if version.parse(torch.__version__) >= version.parse('1.12.0'):
 
-        self.stage = stage
-        self.precision = precision
-        self.zero_optim_config = dict(reduce_bucket_size=reduce_bucket_size_in_m * 1024 * 1024,
-                                      communication_dtype=communication_dtype,
-                                      overlap_communication=overlap_communication,
-                                      cpu_offload=cpu_offload)
-        self.optim_kwargs = dict(initial_scale=initial_scale,
-                                 growth_factor=growth_factor,
-                                 backoff_factor=backoff_factor,
-                                 growth_interval=growth_interval,
-                                 hysteresis=hysteresis,
-                                 min_scale=min_scale,
-                                 max_scale=max_scale,
-                                 max_norm=max_norm,
-                                 norm_type=norm_type)
-        self.verbose = verbose
+        def __init__(
+            self,
+            process_group: Optional[ProcessGroup] = None,
+            sharding_strategy: Optional[ShardingStrategy] = None,
+            cpu_offload: Optional[CPUOffload] = None,
+            auto_wrap_policy: Optional[Callable] = None,
+            backward_prefetch: Optional[BackwardPrefetch] = None,
+            mixed_precision: Optional[MixedPrecision] = None,
+            ignored_modules: Optional[Iterable[torch.nn.Module]] = None,
+            param_init_fn: Optional[Callable[[nn.Module], None]] = None,
+            sync_module_states: bool = False,
+        ):
+            super().__init__()
+            self.fsdp_kwargs = dict(process_group=process_group,
+                                    sharding_strategy=sharding_strategy,
+                                    cpu_offload=cpu_offload,
+                                    auto_wrap_policy=auto_wrap_policy,
+                                    backward_prefetch=backward_prefetch,
+                                    mixed_precision=mixed_precision,
+                                    ignored_modules=ignored_modules,
+                                    param_init_fn=param_init_fn,
+                                    sync_module_states=sync_module_states)
+    else:
+        raise RuntimeError("FSDP is not supported while torch version under 1.12.0.")
 
     def support_no_sync(self) -> bool:
-        return False
+        False
+
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
+        raise NotImplementedError("Torch fsdp no_sync func not supported yet.")
 
     def control_precision(self) -> bool:
         return True
 
     def supported_precisions(self) -> List[str]:
-        return SUPPORTED_PRECISION
+        return ['fp16', 'bf16']
 
     def control_device(self) -> bool:
         return True
 
     def supported_devices(self) -> List[str]:
         return ['cuda']
 
@@ -199,28 +197,27 @@
         model: nn.Module,
         optimizer: Optional[Optimizer] = None,
         criterion: Optional[Callable] = None,
         dataloader: Optional[DataLoader] = None,
         lr_scheduler: Optional[LRScheduler] = None,
     ) -> Tuple[nn.Module, OptimizerWrapper, Callable, DataLoader, LRScheduler]:
 
-        if not isinstance(model, ModelWrapper):
-            model = LowLevelZeroModel(model, self.stage, self.precision)
+        # wrap the model with PyTorch FSDP
+        fsdp_model = TorchFSDPModel(model, device_id=torch.cuda.current_device(), **self.fsdp_kwargs)
+
+        if optimizer is not None:
+            if len(optimizer.param_groups) > 1:
+                warnings.warn(
+                    'TorchFSDPPlugin does not support optimizer that use multi param groups. The results may not be as expected if used.'
+                )
+            optimizer.__init__(fsdp_model.parameters(), **optimizer.defaults)
 
-        if optimizer is not None and \
-                not isinstance(optimizer, OptimizerWrapper):
-            optimizer = LowLevelZeroOptimizer(model.unwrap(),
-                                              optimizer,
-                                              self.zero_optim_config,
-                                              self.optim_kwargs,
-                                              self.verbose)
+            if not isinstance(optimizer, FSDPOptimizerWrapper):
+                optimizer = FSDPOptimizerWrapper(optimizer, fsdp_model)
 
-        return model, optimizer, criterion, dataloader, lr_scheduler
+        return fsdp_model, optimizer, criterion, dataloader, lr_scheduler
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
-        return LowLevelZeroCheckpointIO()
-
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
-        raise NotImplementedError
+        return TorchFSDPCheckpointIO()
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/plugin/plugin_base.py` & `colossalai-nightly-2023.8.5/colossalai/booster/plugin/plugin_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     def get_checkpoint_io(self) -> CheckpointIO:
         """
         Get checkpoint io object for this plugin, only invoked when control_checkpoint_io is True.
         """
         pass
 
     @abstractmethod
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
         """
         Context manager to disable gradient synchronization.
         """
         pass
 
     @abstractmethod
     def prepare_dataloader(self,
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/booster/plugin/torch_ddp_plugin.py` & `colossalai-nightly-2023.8.5/colossalai/booster/plugin/torch_ddp_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,10 +164,10 @@
 
     def control_checkpoint_io(self) -> bool:
         return True
 
     def get_checkpoint_io(self) -> CheckpointIO:
         return TorchDDPCheckpointIO()
 
-    def no_sync(self, model: nn.Module) -> Iterator[None]:
+    def no_sync(self, model: nn.Module, optimizer: OptimizerWrapper) -> Iterator[None]:
         assert isinstance(model, TorchDDPModel), 'Model is not boosted by TorchDDPPlugin.'
         return model.module.no_sync()
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/builder/builder.py` & `colossalai-nightly-2023.8.5/colossalai/builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/checkpoint_io_base.py` & `colossalai-nightly-2023.8.5/colossalai/checkpoint_io/checkpoint_io_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/general_checkpoint_io.py` & `colossalai-nightly-2023.8.5/colossalai/checkpoint_io/general_checkpoint_io.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import gc
 import logging
 import os
 from functools import reduce
 from pathlib import Path
 from typing import Iterator, Optional, OrderedDict, Tuple
 
+import torch.distributed as dist
 import torch.nn as nn
 from torch.optim import Optimizer
 
 from colossalai.interface import OptimizerWrapper
 
 from .checkpoint_io_base import CheckpointIO
 from .index_file import CheckpointIndexFile
 from .utils import (
     get_model_base_filenames,
     get_optimizer_base_filenames,
     get_shard_filename,
-    has_index_file,
     is_safetensors_available,
     load_param_groups_into_optimizer,
     load_shard_state_dict,
     load_state_dict,
     load_state_dict_into_model,
     load_states_into_optimizer,
     save_param_groups,
     save_state_dict,
+    save_state_dict_shards,
     shard_model_checkpoint,
     shard_optimizer_checkpoint,
     sharded_optimizer_loading_epilogue,
     unwrap_optimizer,
 )
 
 __all__ = ['GeneralCheckpointIO']
@@ -118,23 +119,21 @@
 
         # Store the information of param groups to param_group_file.
         index_file.append_meta_data("param_groups", param_group_file)
         group_file_path = os.path.join(checkpoint, param_group_file)
         save_param_groups(state_dict, group_file_path)
 
         # Save shards of optimizer states.
-        total_size = 0
-        for idx, shard_pair in enumerate(sharded_state):
-            shard, current_size = shard_pair
-            shard_file = get_shard_filename(states_name, idx)
-            total_size = total_size + current_size
-            for key in shard.keys():
-                index_file.append_weight_map(key, shard_file)
-            checkpoint_file_path = os.path.join(checkpoint, shard_file)
-            save_state_dict(shard, checkpoint_file_path, use_safetensors=False)
+        # In general cases, is_master is set to True to get the right behavior.
+        total_size = save_state_dict_shards(sharded_state_dict=sharded_state,
+                                            checkpoint=checkpoint,
+                                            index_file=index_file,
+                                            base_filename=states_name,
+                                            is_master=True,
+                                            use_safetensors=False)
 
         # Wrap up index file.
         index_file.append_meta_data("total_size", total_size)
         index_file.write_index_file(save_index_file)
         logging.info(f"The optimizer is going to be split to checkpoint shards. "
                      f"You can find where each parameters has been saved in the "
                      f"index located at {save_index_file}.")
@@ -168,26 +167,25 @@
             return
 
         Path(checkpoint_path).mkdir(parents=True, exist_ok=True)
 
         # shard checkpoint
         state_dict = model.state_dict()
         state_dict_shard = shard_model_checkpoint(state_dict, max_shard_size=max_shard_size)
-
         weights_name, save_index_file = get_model_base_filenames(prefix, use_safetensors)
-        total_size = 0
         index_file = CheckpointIndexFile(checkpoint_path)
-        for idx, shard_pair in enumerate(state_dict_shard):
-            shard = shard_pair[0]
-            shard_file = get_shard_filename(weights_name, idx)
-            total_size = total_size + shard_pair[1]
-            for key in shard.keys():
-                index_file.append_weight_map(key, shard_file)
-            checkpoint_file_path = os.path.join(checkpoint_path, shard_file)
-            save_state_dict(shard, checkpoint_file_path, use_safetensors)
+
+        # Save shards of optimizer states.
+        # In general cases, is_master is set to True to get the right behavior.
+        total_size = save_state_dict_shards(sharded_state_dict=state_dict_shard,
+                                            checkpoint=checkpoint_path,
+                                            index_file=index_file,
+                                            base_filename=weights_name,
+                                            is_master=True,
+                                            use_safetensors=use_safetensors)
 
         index_file.append_meta_data("total_size", total_size)
         index_file.write_index_file(save_index_file)
         logging.info(f"The model is going to be split to checkpoint shards. "
                      f"You can find where each parameters has been saved in the "
                      f"index located at {save_index_file}.")
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/index_file.py` & `colossalai-nightly-2023.8.5/colossalai/checkpoint_io/index_file.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/checkpoint_io/utils.py` & `colossalai-nightly-2023.8.5/colossalai/checkpoint_io/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # coding=utf-8
+import os
 import re
 from collections import abc as container_abcs
 from collections import defaultdict
 from itertools import chain
 from pathlib import Path
 from typing import Iterator, List, Mapping, Optional, OrderedDict, Tuple
 
@@ -99,14 +100,51 @@
     # TODO(Baizhou): ColossalaiOptimizer will be replaced with OptimizerWrapper in the future
     unwrapped_optim = optimizer.optim
     if isinstance(unwrapped_optim, ColossalaiOptimizer):
         unwrapped_optim = unwrapped_optim.optim
     return unwrapped_optim
 
 
+def save_state_dict_shards(sharded_state_dict: Iterator[Tuple[OrderedDict, int]],
+                           checkpoint: str,
+                           index_file: "CheckpointIndexFile",
+                           base_filename: str,
+                           is_master: bool,
+                           use_safetensors: bool = False) -> int:
+    '''
+    Save sharded state dict only on master rank, this method can be used by both model and optimizer states.
+    Args:
+        sharded_state_dict (Iterator[Tuple[OrderedDict, int]]): a generator of shards, each shard contains state dict and shard size.
+        checkpoint (str): The path of checkpoint directory as string.
+        index_file (CheckpointIndexFile): The index file object to be updated.
+        base_filename (str): Decides the prefix of filenames of shards.
+        is_master (bool): Whether current rank is master.
+        use_safetensors (bool): Whether to use safetensors to save checkpoint.
+
+    Returns:
+        int: the total size of shards
+    '''
+
+    total_size = 0
+    for idx, shard_pair in enumerate(sharded_state_dict):
+        if not is_master:
+            continue
+        shard, current_size = shard_pair
+        shard_file = get_shard_filename(base_filename, idx)
+        total_size = total_size + current_size
+        for key in shard.keys():
+            index_file.append_weight_map(key, shard_file)
+        checkpoint_file_path = os.path.join(checkpoint, shard_file)
+
+        # Only save on master rank.
+        save_state_dict(shard, checkpoint_file_path, use_safetensors=use_safetensors)
+
+    return total_size
+
+
 def shard_model_checkpoint(state_dict: torch.Tensor, max_shard_size: int = 1024) -> Iterator[Tuple[OrderedDict, int]]:
     """
     Splits a model state dictionary in sub-checkpoints so that the final size of each sub-checkpoint does not exceed a
     given size.
     """
     current_block = {}
     current_block_size = 0
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/cli/benchmark/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/benchmark.py` & `colossalai-nightly-2023.8.5/colossalai/cli/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/benchmark/utils.py` & `colossalai-nightly-2023.8.5/colossalai/cli/benchmark/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 import time
+from typing import Callable, Dict, List, Tuple
+
 import torch
 
+from colossalai.context import Config, ParallelMode
 from colossalai.utils import MultiTimer
-from colossalai.context import ParallelMode, Config
-from typing import List, Dict, Tuple, Callable
 
 
 def get_time_stamp() -> int:
     """
     Return the time stamp for profiling.
 
     Returns:
@@ -21,16 +22,16 @@
 
 
 def get_memory_states() -> Tuple[float]:
     """
     Return the memory statistics.
 
     Returns:
-        max_allocated (float): the allocated CUDA memory 
-        max_cached (float):  the cached CUDA memory 
+        max_allocated (float): the allocated CUDA memory
+        max_cached (float):  the cached CUDA memory
     """
 
     max_allocated = torch.cuda.max_memory_allocated() / (1024**3)
     max_cached = torch.cuda.max_memory_reserved() / (1024**3)
     torch.cuda.reset_peak_memory_stats()
     torch.cuda.empty_cache()
     return max_allocated, max_cached
@@ -97,15 +98,15 @@
 
     Args:
         model (torch.nn.Module): a PyTorch model
         warmup_steps (int): the number of steps for warmup
         profile_steps (int): the number of steps for profiling
         data_func (Callable): a function to generate random data
         timer (colossalai.utils.Multitimer): a timer instance for time recording
-    
+
     Returns:
         fwd_time (float): the average forward time taken by forward pass in second
         bwd_time (float): the average backward time taken by forward pass in second
         max_allocated (float): the maximum GPU memory allocated in GB
         max_cached (float): the maximum GPU memory cached in GB
     """
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/check/check_installation.py` & `colossalai-nightly-2023.8.5/colossalai/cli/check/check_installation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/launcher/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/cli/launcher/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/launcher/hostinfo.py` & `colossalai-nightly-2023.8.5/colossalai/cli/launcher/hostinfo.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,19 +42,16 @@
         if hostname in ("localhost", "127.0.0.1", "0.0.0.0"):
             return True
 
         hostname = socket.getfqdn(hostname)
         localhost = socket.gethostname()
         localaddrs = socket.getaddrinfo(localhost, port)
         targetaddrs = socket.getaddrinfo(hostname, port)
-        for (family, socktype, proto, canonname, sockaddr) in localaddrs:
-            for (rfamily, rsocktype, rproto, rcanonname, rsockaddr) in targetaddrs:
-                if rsockaddr[0] == sockaddr[0]:
-                    return True
-        return False
+
+        return localaddrs == targetaddrs
 
     def __str__(self):
         return f'hostname: {self.hostname}, port: {self.port}'
 
     def __repr__(self):
         return self.__str__()
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/launcher/multinode_runner.py` & `colossalai-nightly-2023.8.5/colossalai/cli/launcher/multinode_runner.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cli/launcher/run.py` & `colossalai-nightly-2023.8.5/colossalai/cli/launcher/run.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cluster/device_mesh_manager.py` & `colossalai-nightly-2023.8.5/colossalai/cluster/device_mesh_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cluster/dist_coordinator.py` & `colossalai-nightly-2023.8.5/colossalai/cluster/dist_coordinator.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/cluster/process_group_manager.py` & `colossalai-nightly-2023.8.5/colossalai/cluster/process_group_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/communication/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/communication/collective.py` & `colossalai-nightly-2023.8.5/colossalai/communication/collective.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/communication/p2p.py` & `colossalai-nightly-2023.8.5/colossalai/communication/p2p.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 #!/usr/bin/env python
 # -*- encoding: utf-8 -*-
 
+import operator
+from functools import reduce
 from typing import List, Tuple, Union
+
 import torch
 import torch.distributed as dist
 
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.core import global_context as gpc
 from colossalai.utils import get_current_device
-from functools import reduce
-import operator
-from .utils import split_tensor_into_1d_equal_chunks, gather_split_1d_tensor
+
+from .utils import gather_split_1d_tensor, split_tensor_into_1d_equal_chunks
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 
 
 def _get_tensor_shape(tensor_shape: TensorShape, chunk_tensor: bool = False) -> Tuple[TensorShape, bool]:
     """get the exact tensor shape when communicating and return whether the tensor is a chunk
 
@@ -256,15 +258,15 @@
 
 def send_forward_recv_backward(output_tensor,
                                output_grad_shape,
                                recv_next=True,
                                next_rank=None,
                                dtype=torch.float,
                                scatter_gather_tensors=False) -> Union[torch.Tensor, List[torch.Tensor]]:
-    """Batched communication operation. Sends the input tensor to the 
+    """Batched communication operation. Sends the input tensor to the
     next stage in pipeline, while receives the gradient tensor from the
     next stage in pipeline as the input gradient tensor of this stage.
 
     Args:
         output_tensor (Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]): Tensor to be sent.
         output_grad_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
 
@@ -315,15 +317,15 @@
 def send_forward_recv_forward(output_tensor,
                               input_tensor_shape,
                               recv_prev=True,
                               prev_rank=None,
                               next_rank=None,
                               dtype=torch.float,
                               scatter_gather_tensors=False) -> Union[torch.Tensor, List[torch.Tensor]]:
-    """Batched communication operation. Sends the input tensor to the 
+    """Batched communication operation. Sends the input tensor to the
     next stage in pipeline, while receives the output tensor from the
     previous stage in pipeline as the input of this stage.
 
     Args:
         output_tensor (Union[:class:`torch.Tensor`, List[:class:`torch.Tensor`]]): Tensor to be sent.
         input_tensor_shape (Union[:class:`torch.Size`, List[:class:`torch.Size`]]): The shape of the tensor to be received.
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/communication/p2p_v2.py` & `colossalai-nightly-2023.8.5/colossalai/communication/p2p_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/communication/ring.py` & `colossalai-nightly-2023.8.5/colossalai/communication/ring.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/communication/utils.py` & `colossalai-nightly-2023.8.5/colossalai/communication/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
+from typing import List, Tuple, Union
+
 import torch
 import torch.distributed as dist
 
 from colossalai.context.parallel_mode import ParallelMode
 from colossalai.core import global_context as gpc
 from colossalai.utils import get_current_device
-from typing import Union, List, Tuple
 
 TensorShape = Union[torch.Size, List[int], Tuple[int]]
 
 
 def send_meta_helper(obj, next_rank, tensor_kwargs):
     send_shape = torch.tensor(obj.size(), **tensor_kwargs)
     send_ndims = torch.tensor(len(obj.size()), **tensor_kwargs)
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/constants.py` & `colossalai-nightly-2023.8.5/colossalai/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/config.py` & `colossalai-nightly-2023.8.5/colossalai/context/config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/moe_context.py` & `colossalai-nightly-2023.8.5/colossalai/context/moe_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/parallel_context.py` & `colossalai-nightly-2023.8.5/colossalai/context/parallel_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/parallel_mode.py` & `colossalai-nightly-2023.8.5/colossalai/context/parallel_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_1d.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2d.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_2p5d.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_3d.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_data.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_data.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_model.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_pipeline.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_pipeline.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_sequence.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_sequence.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/initializer_tensor.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/initializer_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/process_group_initializer/process_group_initializer.py` & `colossalai-nightly-2023.8.5/colossalai/context/process_group_initializer/process_group_initializer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/random/_helper.py` & `colossalai-nightly-2023.8.5/colossalai/context/random/_helper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/random/seed_manager.py` & `colossalai-nightly-2023.8.5/colossalai/context/random/seed_manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/context/singleton_meta.py` & `colossalai-nightly-2023.8.5/colossalai/context/singleton_meta.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/device/alpha_beta_profiler.py` & `colossalai-nightly-2023.8.5/colossalai/device/alpha_beta_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/device/calc_pipeline_strategy.py` & `colossalai-nightly-2023.8.5/colossalai/device/calc_pipeline_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/device/device_mesh.py` & `colossalai-nightly-2023.8.5/colossalai/device/device_mesh.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/_base_engine.py` & `colossalai-nightly-2023.8.5/colossalai/engine/_base_engine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_accumulation/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_accumulation/_gradient_accumulation.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_accumulation/_gradient_accumulation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_base_gradient_handler.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_base_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_data_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_moe_gradient_handler.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_moe_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_pipeline_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_sequence_parallel_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/_zero_gradient_handler.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/_zero_gradient_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/gradient_handler/utils.py` & `colossalai-nightly-2023.8.5/colossalai/engine/gradient_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_base_schedule.py` & `colossalai-nightly-2023.8.5/colossalai/engine/schedule/_base_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_non_pipeline_schedule.py` & `colossalai-nightly-2023.8.5/colossalai/engine/schedule/_non_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule.py` & `colossalai-nightly-2023.8.5/colossalai/engine/schedule/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/engine/schedule/_pipeline_schedule_v2.py` & `colossalai-nightly-2023.8.5/colossalai/engine/schedule/_pipeline_schedule_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/_compatibility.py` & `colossalai-nightly-2023.8.5/colossalai/fx/_compatibility.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_12.py` & `colossalai-nightly-2023.8.5/colossalai/fx/_meta_regist_12.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/_meta_regist_13.py` & `colossalai-nightly-2023.8.5/colossalai/fx/_meta_regist_13.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/codegen/activation_checkpoint_codegen.py` & `colossalai-nightly-2023.8.5/colossalai/fx/codegen/activation_checkpoint_codegen.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/graph_module.py` & `colossalai-nightly-2023.8.5/colossalai/fx/graph_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/adding_split_node_pass.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/adding_split_node_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/concrete_info_prop.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/concrete_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/meta_info_prop.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/meta_info_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/passes_for_gpt2_test.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/passes_for_gpt2_test.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/shard_1d_pass.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/shard_1d_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/split_module.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/split_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/passes/utils.py` & `colossalai-nightly-2023.8.5/colossalai/fx/passes/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/constants.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/dataflow.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/dataflow.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/constants.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/constants.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/activation_function.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/normalization.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/pooling.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/activation_function.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/activation_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/attention.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/convolution.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/normalization.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/pooling.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/profiler_module/rnn.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/profiler_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/registry.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/experimental/shard_utils.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/experimental/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/memory_utils.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/memory_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/opcount.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/opcount.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/profiler.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/shard_utils.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/shard_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/profiler/tensor.py` & `colossalai-nightly-2023.8.5/colossalai/fx/profiler/tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/proxy.py` & `colossalai-nightly-2023.8.5/colossalai/fx/proxy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_meta_trace.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/_meta_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_symbolic_trace.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/_symbolic_trace.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/_tracer_utils.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/_tracer_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addbmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/bias_addition_function.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_function/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/bias_addition_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/conv.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/bias_addition_patch/patched_bias_addition_module/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/experimental.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/experimental.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/arithmetic.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/convolution.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/normalization.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/python_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_function/torch_ops.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/convolution.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/convolution.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/normalization.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/pooling.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/pooling.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/meta_patch/patched_module/rnn.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/meta_patch/patched_module/rnn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/registry.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/fx/tracer/tracer.py` & `colossalai-nightly-2023.8.5/colossalai/fx/tracer/tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/global_variables.py` & `colossalai-nightly-2023.8.5/colossalai/global_variables.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/initialize.py` & `colossalai-nightly-2023.8.5/colossalai/initialize.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/interface/model.py` & `colossalai-nightly-2023.8.5/colossalai/interface/model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/interface/optimizer.py` & `colossalai-nightly-2023.8.5/colossalai/interface/optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/cpu_adam.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/cpu_adam.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/cpu_adam.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/cross_entropy.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/cublas_wrappers.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/cuda_util.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/dropout_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/general_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/block_reduce.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/context.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/context.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/cross_entropy_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/cublas_wrappers.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/cuda_util.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/normalize_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/softmax_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/kernels/transform_kernels.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/layer_norm_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/layer_norm_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/moe_cuda.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/moe_cuda_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_adam.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_apply.cuh`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_l2norm_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_lamb.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_scale_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multi_tensor_sgd_kernel.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/multihead_attention_1d.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.cpp`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/scaled_upper_triang_masked_softmax_cuda.cu`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/csrc/type_shim.h` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/csrc/type_shim.h`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/layer_norm.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/layer_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/multihead_attention.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/cuda_native/scaled_softmax.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/cuda_native/scaled_softmax.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     scaled_masked_softmax = None
     scaled_upper_triang_masked_softmax = None
 
 
 class AttnMaskType(enum.Enum):
     padding = 1
     causal = 2
+    paddedcausal = 3
 
 
 class ScaledUpperTriangMaskedSoftmax(torch.autograd.Function):
     """
     Fused operation which performs following three operations in sequence
 
         1.  Scale the tensor.
@@ -135,27 +136,27 @@
                 and 16 < sk <= 2048    # sk must be 16 ~ 2048
                 and sq % 4 == 0    # sq must be divisor of 4
                 and attn_batches % 4 == 0    # np * b must be divisor of 4
            ):
             if 0 <= sk <= 2048:
                 batch_per_block = self.get_batch_per_block(sq, sk, b, np)
 
-                if self.attn_mask_type == AttnMaskType.causal:
+                if self.attn_mask_type.value > 1:
                     if attn_batches % batch_per_block == 0:
                         return True
                 else:
                     if sq % batch_per_block == 0:
                         return True
         return False
 
     def forward_fused_softmax(self, input, mask):
         b, np, sq, sk = input.size()
         scale = self.scale if self.scale is not None else 1.0
 
-        if self.attn_mask_type == AttnMaskType.causal:
+        if self.attn_mask_type.value > 1:
             assert sq == sk, "causal mask is only for self attention"
 
             # input is 3D tensor (attn_batches, sq, sk)
             input = input.view(-1, sq, sk)
             probs = ScaledUpperTriangMaskedSoftmax.apply(input, scale)
             return probs.view(b, np, sq, sk)
         else:
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_dropout_add.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/jit/bias_dropout_add.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/jit/bias_gelu.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/jit/bias_gelu.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/jit/option.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/jit/option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/builder.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/cpu_adam.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/fused_optim.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/layernorm.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/moe.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/kernel/op_builder/utils.py` & `colossalai-nightly-2023.8.5/colossalai/kernel/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/lazy/lazy_init.py` & `colossalai-nightly-2023.8.5/colossalai/lazy/lazy_init.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from contextlib import contextmanager
 from types import MethodType
 from typing import Callable, Dict, Optional, Union
 
 import torch
 import torch.distributed as dist
 import torch.nn as nn
 from torch import Tensor
@@ -57,20 +58,23 @@
 
 
 class _MyTensor(Tensor):
     """This class is only for correctness verification.
     """
     _pre_op_fn: Callable[['LazyTensor'], None] = lambda *args: None
 
+    default_device: Optional[torch.device] = None
+
     def __new__(cls, func, *args, concrete_data=None, **kwargs) -> '_MyTensor':
         cls._pre_op_fn()
         if concrete_data is not None:
             # uniform api as LazyTensor
             data = concrete_data
         else:
+            kwargs['device'] = cls.default_device
             data = func(*args, **kwargs)
         return Tensor._make_subclass(cls, data, require_grad=data.requires_grad)
 
     @classmethod
     def __torch_function__(cls, func, types, args=(), kwargs=None):
         cls._pre_op_fn()
         return super().__torch_function__(func, types, args, kwargs)
@@ -138,14 +142,16 @@
 
     """
 
     _repr = True
     _meta_data: Optional[MetaTensor] = None    # shape, dtype, device
     _pre_op_fn: Callable[['LazyTensor'], None] = lambda *args: None
 
+    default_device: Optional[torch.device] = None
+
     @staticmethod
     def __new__(cls, func, *args, meta_data=None, concrete_data=None, **kwargs):
         if concrete_data is not None:
             # some ops don't support meta backend and should have concrete data
             elem = concrete_data
         else:
             if meta_data is None:
@@ -155,14 +161,16 @@
             elem = meta_data._tensor
         # As a meta tensor cannot be modified __class__ to torch.Tensor, we should use an empty real tensor here
         r = torch.Tensor._make_subclass(cls, _EMPTY_DATA, require_grad=elem.requires_grad)
         r._meta_data = meta_data
         return r
 
     def __init__(self, func, *args, meta_data=None, concrete_data=None, **kwargs):
+        if func.__name__ in _NORMAL_FACTORY:
+            kwargs = {**kwargs, 'device': LazyTensor.default_device}
         self._factory_method = (func, args, kwargs)    # (func, args, kwargs)
         self._op_buffer = []    # (func, args, kwargs, replace)
         self._materialized_data: Optional[torch.Tensor] = concrete_data    # materialized data
 
     def materialize(self) -> torch.Tensor:
         """Materialize the ``LazyTensor`` to ``torch.Tensor`` by modifying __class__ (inplace).
 
@@ -202,24 +210,19 @@
         return x
 
     def _materialize_data(self) -> torch.Tensor:
         # self._materialized_data should be generated after the first call of this function
         if self._materialized_data is None:
             # apply factory method
             func, args, kwargs = self._factory_method
-
             # apply cached sequence
             self._pre_op_fn()
 
-            try:
-                init_val = func(*tree_map(self._replace_with_materialized, args),
-                                **tree_map(self._replace_with_materialized, kwargs))
-            except TypeError as e:
-                print(f'init fn: {func.__name__}')
-                raise e
+            init_val = func(*tree_map(self._replace_with_materialized, args),
+                            **tree_map(self._replace_with_materialized, kwargs))
 
             self._materialized_data = self._rerun_ops(init_val)
         return self._materialized_data
 
     def _rerun_ops(self, target=None) -> torch.Tensor:
         """Do lazy execution by rerunning all (stored) related operations.
 
@@ -301,14 +304,15 @@
                 if isinstance(y, MetaTensor):
                     if y in meta_to_lazy:
                         # inplace op, just return origin lazy tensor
                         return meta_to_lazy[y]
                     else:
                         # out of place op, create new lazy tensor
                         fn = lambda *a, **kw: func(*a, **kw) if i is None else func(*a, **kw)[i]
+                        fn.__name__ = func.__name__
                         lazy_y = LazyTensor(fn, *args, meta_data=y, **kwargs)
                         return lazy_y
                 elif type(y) is Tensor:
                     # for early materialized tensor
                     return LazyTensor(lambda: None, concrete_data=y)
                 return y
 
@@ -431,22 +435,29 @@
         This API is still experimental and further modifications can be made to it.
         For example:
             1. Quantization strategies can be applied before allocating real memory.
             2. Lazy initialization seems slower than normal initialization.
     """
     _replaced: bool = False
 
-    def __init__(self, tensor_cls: Union[_MyTensor, LazyTensor] = LazyTensor):
+    def __init__(self,
+                 tensor_cls: Union[_MyTensor, LazyTensor] = LazyTensor,
+                 default_device: Optional[Union[torch.device, str, int]] = None):
+        assert tensor_cls is LazyTensor or tensor_cls is _MyTensor
         self.overrides = {}
         self.tensor_cls = tensor_cls
+        self.old_default_device = LazyTensor.default_device
+        self.default_device = default_device
 
     def __enter__(self):
         if LazyInitContext._replaced:
             raise RuntimeError(f'LazyInitContext is not reentrant')
         LazyInitContext._replaced = True
+        self.old_default_device = self.tensor_cls.default_device
+        self.tensor_cls.default_device = self.default_device
 
         def wrap_factory_method(target):
             # factory functions (eg. torch.empty())
             def wrapper(*args, **kwargs):
                 return self.tensor_cls(target, *args, **kwargs)
 
             return wrapper, target
@@ -514,14 +525,15 @@
             if callable(getattr(torch, target, None))
         })
 
         for name, (wrapper, orig) in self.overrides.items():
             setattr(torch, name, wrapper)
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        self.tensor_cls.default_device = self.old_default_device
         LazyInitContext._replaced = False
         for name, (wrapper, orig) in self.overrides.items():
             setattr(torch, name, orig)
 
     @staticmethod
     def materialize(module: nn.Module, verbose: bool = False) -> nn.Module:
         """Initialize all ``nn.Parameter`` from ``LazyTensor``. This function will modify the module in-place.
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/logging/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/logging/logger.py` & `colossalai-nightly-2023.8.5/colossalai/logging/logger.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/addmm.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/addmm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/batch_norm.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/batch_norm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/element_wise.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/element_wise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/embedding_bag.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/embedding_bag.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/layernorm.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/linear.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/loss.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/_ops/view.py` & `colossalai-nightly-2023.8.5/colossalai/nn/_ops/view.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/init.py` & `colossalai-nightly-2023.8.5/colossalai/nn/init.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/base_layer.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/base_layer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/dropout.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/linear.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/colossalai_layer/normalization.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/colossalai_layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/checkpoint.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/experts.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/experts.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/routers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/routers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/moe/utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/moe/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_1d/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_1d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2d/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_2p5d/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_2p5d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_3d/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_3d/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/parallel_sequence/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/parallel_sequence/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/utils/common.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/vanilla/layers.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/vanilla/layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/layer/wrapper/pipeline_wrapper.py` & `colossalai-nightly-2023.8.5/colossalai/nn/layer/wrapper/pipeline_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/loss/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/nn/loss/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_1d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_1d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_2p5d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_3d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/loss/loss_moe.py` & `colossalai-nightly-2023.8.5/colossalai/nn/loss/loss_moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/cosine.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/cosine.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/delayed.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/delayed.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/linear.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/multistep.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/multistep.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/onecycle.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/onecycle.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/poly.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/poly.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/lr_scheduler/torch.py` & `colossalai-nightly-2023.8.5/colossalai/nn/lr_scheduler/torch.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/metric/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/nn/metric/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/metric/accuracy_2d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_2p5d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/metric/accuracy_2p5d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/metric/accuracy_3d.py` & `colossalai-nightly-2023.8.5/colossalai/nn/metric/accuracy_3d.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/colossalai_optimizer.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/colossalai_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/cpu_adam.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_adam.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/fused_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_lamb.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/fused_lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/fused_sgd.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/fused_sgd.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/hybrid_adam.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/hybrid_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lamb.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/lamb.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/lars.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/lars.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/optimizer/nvme_optimizer.py` & `colossalai-nightly-2023.8.5/colossalai/nn/optimizer/nvme_optimizer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/data_parallel.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/data_parallel.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/base_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/cache_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/copyer.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/copyer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/embedding_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/cache_embedding/parallel_cached_embedding_tablewise_split_cache.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/colo_module.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/colo_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/linear.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/layers/module_utils.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/layers/module_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/nn/parallel/reducer.py` & `colossalai-nightly-2023.8.5/colossalai/nn/parallel/reducer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/layer_spec.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/layer_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/adaptor/fx.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/adaptor/fx.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/middleware/topo.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/middleware/topo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/pipelinable.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/pipelinable.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/pipeline_process_group.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/pipeline_process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_base.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/_pipeline_base.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/_pipeline_schedule.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/_pipeline_schedule.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/rpc/utils.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/rpc/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/pipeline/utils.py` & `colossalai-nightly-2023.8.5/colossalai/pipeline/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/registry/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/registry/registry.py` & `colossalai-nightly-2023.8.5/colossalai/registry/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/_operation.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/_operation.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/dropout.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/dropout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/embedding.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/embedding.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/linear.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/loss.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/loss.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/normalization.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/normalization.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/parallel_module.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/parallel_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/qkv_fused_linear.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/qkv_fused_linear.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/layer/utils.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/layer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/modeling/bloom.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/modeling/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/autopolicy.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/autopolicy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/basepolicy.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/basepolicy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bert.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/bloom.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/gpt2.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/llama.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/opt.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/t5.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/policies/vit.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/policies/vit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shard_config.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/shard/shard_config.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/shard/sharder.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/shard/sharder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/shardformer/shard/shardformer.py` & `colossalai-nightly-2023.8.5/colossalai/shardformer/shard/shardformer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/colo_parameter.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/colo_parameter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/colo_tensor.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/colo_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/comm_spec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/compute_spec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/compute_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/api.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/api.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/comm_spec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/comm_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/layout.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/layout_converter.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/layout_converter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/sharding_spec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/d_tensor/utils.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/d_tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/dist_spec_mgr.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/dist_spec_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/distspec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/distspec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/op_wrapper.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/op_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/param_op_hook.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/param_op_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/process_group.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/process_group.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/shape_consistency.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/shape_consistency.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/sharding_spec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/sharding_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/tensor_spec.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/tensor_spec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/tensor/utils.py` & `colossalai-nightly-2023.8.5/colossalai/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/testing/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/testing/comparison.py` & `colossalai-nightly-2023.8.5/colossalai/testing/comparison.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/testing/pytest_wrapper.py` & `colossalai-nightly-2023.8.5/colossalai/testing/pytest_wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/testing/random.py` & `colossalai-nightly-2023.8.5/colossalai/testing/random.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/testing/utils.py` & `colossalai-nightly-2023.8.5/colossalai/testing/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/_trainer.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/_trainer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/hooks/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_base_hook.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_base_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_checkpoint_hook.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_checkpoint_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_log_hook.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_log_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_lr_scheduler_hook.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_lr_scheduler_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/trainer/hooks/_metric_hook.py` & `colossalai-nightly-2023.8.5/colossalai/trainer/hooks/_metric_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/activation_checkpoint.py` & `colossalai-nightly-2023.8.5/colossalai/utils/activation_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/module_checkpoint.py` & `colossalai-nightly-2023.8.5/colossalai/utils/checkpoint/module_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/checkpoint/utils.py` & `colossalai-nightly-2023.8.5/colossalai/utils/checkpoint/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/checkpointing.py` & `colossalai-nightly-2023.8.5/colossalai/utils/checkpointing.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/common.py` & `colossalai-nightly-2023.8.5/colossalai/utils/common.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/cuda.py` & `colossalai-nightly-2023.8.5/colossalai/utils/cuda.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/data_sampler/data_parallel_sampler.py` & `colossalai-nightly-2023.8.5/colossalai/utils/data_sampler/data_parallel_sampler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/memory.py` & `colossalai-nightly-2023.8.5/colossalai/utils/memory.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/model/utils.py` & `colossalai-nightly-2023.8.5/colossalai/utils/model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/moe.py` & `colossalai-nightly-2023.8.5/colossalai/utils/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py` & `colossalai-nightly-2023.8.5/colossalai/utils/multi_tensor_apply/multi_tensor_apply.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/comm_profiler.py` & `colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/comm_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/pcie_profiler.py` & `colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/pcie_profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/profiler/legacy/prof_utils.py` & `colossalai-nightly-2023.8.5/colossalai/utils/profiler/legacy/prof_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/profiler/profiler.py` & `colossalai-nightly-2023.8.5/colossalai/utils/profiler/profiler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/profiler/stateful_tensor_mem_extention.py` & `colossalai-nightly-2023.8.5/colossalai/utils/profiler/stateful_tensor_mem_extention.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/rank_recorder/rank_recorder.py` & `colossalai-nightly-2023.8.5/colossalai/utils/rank_recorder/rank_recorder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/tensor_detector/tensor_detector.py` & `colossalai-nightly-2023.8.5/colossalai/utils/tensor_detector/tensor_detector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/utils/timer.py` & `colossalai-nightly-2023.8.5/colossalai/utils/timer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/zero/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/chunk.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/chunk.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/manager.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/manager.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/search_utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/search_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/chunk/utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/chunk/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/colo_init_context.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/colo_init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_ddp.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_hook.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_mgr.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/gemini_optimizer.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/gemini_optimizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # this code is inspired by the DeepSpeed library and implemented with our own design from scratch
 import copy
 import gc
 import math
 import warnings
-from typing import Any, Dict, Set, Tuple
+from typing import Any, Dict, Iterator, OrderedDict, Set, Tuple
 
 import torch
 import torch.distributed as dist
 from torch.nn import Parameter
 from torch.optim import Optimizer
 
 from colossalai.amp.naive_amp.mixed_precision_mixin import BF16MixedPrecisionMixin, FP16MixedPrecisionMixin
+from colossalai.checkpoint_io.utils import calculate_tensor_size
 from colossalai.logging import get_dist_logger
 from colossalai.nn.optimizer import ColossalaiOptimizer, CPUAdam, FusedAdam, HybridAdam
+from colossalai.tensor.d_tensor import is_distributed_tensor
 from colossalai.utils import disposable, get_current_device, is_ddp_ignored
 
 from .chunk import Chunk, ChunkManager
 from .gemini_ddp import ZeroDDP
 
 __all__ = ['ZeroOptimizer', 'GeminiAdamOptimizer']
 
@@ -356,18 +358,20 @@
         fake_param = self.id_to_fake_params[param_id]
         chunk = self.param_to_chunk32[fake_param].paired_chunk
         param = self.id_to_real_params[param_id]
         param_info = chunk.tensors_info[param]
 
         begin_in_chunk, end_in_chunk = self.param_to_range[fake_param]
         chunk_offset = begin_in_chunk
-        shard_offset = begin_in_chunk + chunk.shard_begin - param_info.offset
+        if chunk.keep_gathered:
+            shard_offset = 0
+        else:
+            shard_offset = begin_in_chunk + chunk.shard_begin - param_info.offset
         shard_size = end_in_chunk - begin_in_chunk
         assert chunk_offset >= 0 and shard_offset >= 0
-
         return chunk_offset, shard_offset, shard_size
 
     def collect_states(self, param_id: int, only_rank_0: bool = True) -> dict:
         """
         Args:
             param_id (int): id of the parameter whose state is to be gathered at master rank.
             only_rank_0(bool): if True, states will be collected only on master rank, otherwise collected on every rank.
@@ -423,15 +427,16 @@
                 for state_name in state_names:
                     if state_name == 'step':
                         # To keep aligned with pytorch, state 'step' is stored as a pytorch tensor with type float32.
                         collected_states[state_name] = torch.tensor(states['step'],
                                                                     dtype=torch.float32,
                                                                     requires_grad=False).cpu()
                     else:
-                        collected_states[state_name] = states[state_name].detach().clone().to(torch.float32).cpu()
+                        state_tensor = states[state_name].detach().clone().to(torch.float32).cpu()
+                        collected_states[state_name] = torch.reshape(state_tensor, param.shape)
             return collected_states
 
         # Check whether the param with given id is managed by current process.
         own_param = param_id in self.id_to_fake_params
 
         # Collector gets prepared for state collecting.
         if is_collector:
@@ -532,14 +537,39 @@
                                                              requires_grad=False).cpu()
                 next_state_offset += 1
             else:
                 target_segment = collected_states[state_name][shard_start:shard_end]
                 target_segment.copy_(compacted_states[next_state_offset:next_state_offset + shard_size])
                 next_state_offset += shard_size
 
+    def get_param_groups_for_saving(self) -> list:
+        '''
+        Return the param_groups in Pytorch format when saving to checkpoint.
+        '''
+
+        param_groups = copy.deepcopy(self.param_groups_backup)
+
+        # To be compatible with pytorch checkpointing,
+        # store extra hyperparameters used by pytorch Adam optimizer.
+        torch_special_hyperparameters = {
+            'amsgrad': False,
+            'maximize': False,
+            'foreach': None,
+            'capturable': False,
+            'differentiable': False,
+            'fused': False
+        }
+
+        for group in param_groups:
+            for k, v in torch_special_hyperparameters.items():
+                if k not in group:
+                    group[k] = v
+
+        return param_groups
+
     def state_dict(self, only_rank_0: bool = True) -> dict:
         """
         Args:
             only_rank_0 (bool): a boolean value indicating whether the state_dict is collected
             only on rank 0, dafault to True.
 
         Returns:
@@ -551,29 +581,15 @@
             * param_groups - a list containing all parameter groups where each
                 parameter group is a dict.
 
         Warning: This method will gather and return the whole optimizer state_dict,
                  so it should be called only when memory resources are abundant.
         """
         state_dict = {}
-        state_dict['param_groups'] = copy.deepcopy(self.param_groups_backup)
-
-        torch_special_hyperparameters = {
-            'amsgrad': False,
-            'maximize': False,
-            'foreach': None,
-            'capturable': False,
-            'differentiable': False,
-            'fused': False
-        }
-
-        for group in state_dict['param_groups']:
-            for k, v in torch_special_hyperparameters.items():
-                if k not in group:
-                    group[k] = v
+        state_dict['param_groups'] = self.get_param_groups_for_saving()
 
         # Collect optimizer states.
         state_dict['state'] = dict()
         for param_id in self.id_to_real_params.keys():
             dist.barrier()
             state_dict['state'][param_id] = self.collect_states(param_id=param_id, only_rank_0=only_rank_0)
         return state_dict
@@ -630,34 +646,104 @@
         # Copy states assigned to param (and cast tensors to appropriate types).
         updated_states = dict()
         for k, v in saved_states.items():
             updated_states[k] = cast(fake_param, state_range, v, k)
             del v    # clean loaded states
         self.optim.state[fake_param].update(updated_states)
 
+    def load_param_states(self, param_states: dict):
+        """Loads param states from a state_dict. The param_states can be complete or sharded.
+           During loading, filter out the part of states not considered by current process.
+
+        Args:
+            param_states (dict): A mapping from param_id to its states.
+        """
+        for param_id, states in param_states.items():
+            if param_id in self.id_to_fake_params:
+                self.load_single_param_states(param_id, states)
+
+    def optimizer_loading_epilogue(self):
+        # Epilogue when loading state_dict to pytorch optimizer.
+        self.optim._hook_for_profile()    # To support multiprocessing pickle/unpickle.
+        self.optim.defaults.setdefault('differentiable', False)
+
     def load_state_dict(self, state_dict: dict):
-        """Loads optimizer state from whole optimizer state_dict.
+        """Loads optimizer state from complete optimizer state_dict.
            During loading, filter out the part of states not considered by current process.
 
         Args:
             state_dict (dict): optimizer state. Should be an object returned
                 from a call to :meth:`state_dict`.
         """
         assert 'param_groups' in state_dict
+        assert 'state' in state_dict
         self.load_param_groups(state_dict['param_groups'])
+        self.load_param_states(state_dict['state'])
+        self.optimizer_loading_epilogue()
 
-        state = state_dict['state']
+    def state_shard(self,
+                    prefix: str = '',
+                    max_shard_size: int = 1024,
+                    only_rank_0: bool = True) -> Iterator[Tuple[OrderedDict, int]]:
+        """Returns dictionaries containing shards of optimizer states one by one.
+           The max size of each dictionary shard is specified by ``max_shard_size``.
 
-        for param_id, param_states in state.items():
-            if param_id in self.id_to_fake_params:
-                self.load_single_param_states(param_id, param_states)
+        Args:
+            prefix (str, optional): the prefix for states. Default to ''.
+            max_shard_size (int, optional): max size of state dict shard (in MB). Defaults to 1024.
+            only_rank_0 (bool, optional): a boolean value indicating whether the state_dict is collected
+                                          only on rank 0, dafault to True.
 
-        # Epilogue for pytorch optimizer.
-        self.optim._hook_for_profile()    # To support multiprocessing pickle/unpickle.
-        self.optim.defaults.setdefault('differentiable', False)
+        Yields:
+            Iterator[OrderedDict]: A generator of state dict shard of optimizer states.
+        """
+
+        current_block = {}
+        current_block_size = 0
+
+        for param_id in self.id_to_real_params.keys():
+
+            dist.barrier()
+            state = self.collect_states(param_id=param_id, only_rank_0=only_rank_0)
+
+            ret_block = None
+            ret_block_size = 0
+
+            # A state might contain more than one tensors.
+            # e.g. each Adam state includes: 'step', 'exp_avg', 'exp_avg_sq'
+            state_size = 0
+            isDTensor = False
+            for state_tensor in state.values():
+
+                # When state_tensor is not of Tensor class,
+                # e.g., a SGD optimizer with momentum set to 0 can have None as state
+                # The calculation of tensor size should be skipped to avoid error.
+                if not isinstance(state_tensor, torch.Tensor):
+                    continue
+
+                # If the states are stored as DTensors, mark isDTensor as true.
+                if is_distributed_tensor(state_tensor):
+                    isDTensor = True
+                state_size += calculate_tensor_size(state_tensor)
+
+            if not isDTensor:
+
+                if current_block_size + state_size > max_shard_size and current_block_size > 0:
+                    ret_block = current_block
+                    ret_block_size = current_block_size
+                    current_block = {}
+                    current_block_size = 0
+
+                current_block[param_id] = state
+                current_block_size += state_size
+
+            if ret_block != None:
+                yield ret_block, ret_block_size
+
+        yield current_block, current_block_size
 
 
 class GeminiAdamOptimizer(ZeroOptimizer):
 
     def __init__(self, model: torch.nn.Module, **defaults: Any) -> None:
         optimizer = HybridAdam(model.parameters(), **defaults)
         super().__init__(optimizer, model, **defaults)
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/chunk_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_monitor.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/memory_monitor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memory_stats.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/memory_stats.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/memstats_collector.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/param_runtime_order.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/param_runtime_order.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/runtime_mem_tracer.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/static_memstats_collector.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/memory_tracer/utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/memory_tracer/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/placement_policy.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/gemini/utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/gemini/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/__init__.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/gemini_context.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/gemini_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/_shard_grad_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/_shard_param_ophook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/runtime_mem_tracer_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/ophooks/utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/ophooks/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/paramhooks/_param_hookmgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/stateful_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/stateful_tensor_mgr.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_placement_policy.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/tensor_placement_policy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/gemini/tensor_utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/gemini/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/init_ctx/init_context.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/init_ctx/init_context.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/base_shard_strategy.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/base_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/bucket_tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/commons.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/commons.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/shard_utils/tensor_shard_strategy.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/reduce_scatter.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/reduce_scatter.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/sharded_model_v2.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/sharded_model_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_model/zero_hook.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_model/zero_hook.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_optim/sharded_optim_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_param.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_param/sharded_param.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/legacy/sharded_param/sharded_tensor.py` & `colossalai-nightly-2023.8.5/colossalai/zero/legacy/sharded_param/sharded_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/low_level/_utils.py` & `colossalai-nightly-2023.8.5/colossalai/zero/low_level/_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import math
 from typing import Optional
 
 import torch
 import torch.distributed as dist
-from torch import inf
+from torch import Tensor, inf
 from torch._utils import _flatten_dense_tensors, _unflatten_dense_tensors
+from torch.distributed import ProcessGroup
 
 from colossalai.tensor import ColoParameter
 from colossalai.utils import is_model_parallel_parameter
 
 
 def flatten(input_):
     return _flatten_dense_tensors(input_)
@@ -190,74 +191,61 @@
     """
     total_norm = 0.0
     for norm in norm_list:
         total_norm += norm**2.0
     return math.sqrt(total_norm)
 
 
-def compute_norm(gradients, params, dp_group, mp_group, norm_type=2):
+def compute_norm(gradients: Tensor, dp_group: ProcessGroup, tp_group: ProcessGroup, norm_type: int = 2) -> int:
     """Clips gradient norm of an iterable of parameters.
     This is adapted from torch.nn.utils.clip_grad.clip_grad_norm_ and
-    added functionality to handle model parallel parameters. Note that
-    the gradients are modified in place.
-    Arguments:
-        parameters (Iterable[Tensor] or Tensor): an iterable of Tensors or a
-            single Tensor that will have gradients normalized
-        max_norm (float or int): max norm of the gradients
-        norm_type (float or int): type of the used p-norm. Can be ``'inf'`` for
-            infinity norm.
+    added functionality to handle model parallel parameters.
+
+    Args:
+        gradients (Tensor): The gradients to compute norm
+        dp_group (ProcessGroup): The process group of ZeRO Data Parallelism
+        tp_group (ProcessGroup): The process group of Tensor Parallelism
+        norm_type (int, optional): type of the used p-norm, Can be ``'inf'`` for infinity norm. Defaults to 2.
+
     Returns:
-        Total norm of the parameters (viewed as a single vector).
+        int: The total norm of given gradients
     """
 
-    if mp_group is None:
-        mp_rank = 0
-    else:
-        mp_rank = dist.get_rank(mp_group)
-
     norm_type = float(norm_type)
     if norm_type == inf:
         total_norm = max(g.data.abs().max() for g in gradients)
         total_norm_cuda = torch.cuda.FloatTensor([float(total_norm)])
         dist.all_reduce(total_norm_cuda, op=torch.distributed.ReduceOp.MAX, group=dp_group)
 
         # Take max across all GPUs.
-        if mp_group is not None:
+        if tp_group is not None:
             dist.all_reduce(tensor=total_norm_cuda, op=torch.distributed.ReduceOp.MAX)
         total_norm = total_norm_cuda[0].item()
     else:
         total_norm = 0.0
-        # if dist.get_rank() == 0:
-        #    logger.info(f"Total Norm beginning {total_norm}")
-
-        for g, p in zip(gradients, params):
-            # Pipeline parallelism may replicate parameters. Avoid multi-counting.
-            tp_param_flag = False
-            if is_model_parallel_parameter(p) or (isinstance(p, ColoParameter) and not p.is_replicate()):
-                tp_param_flag = True
-            if tp_param_flag or mp_rank == 0:
-                param_norm = g.data.double().norm(2)
-                total_norm += param_norm.item()**2
+        for g in gradients:
+            param_norm = g.data.double().norm(2)
+            total_norm += param_norm.item()**2
 
         # Sum across all model parallel GPUs.
         total_norm_cuda = torch.cuda.FloatTensor([float(total_norm)])
         torch.distributed.all_reduce(total_norm_cuda, op=torch.distributed.ReduceOp.SUM, group=dp_group)
 
-        if mp_group is not None:
-            dist.all_reduce(tensor=total_norm_cuda, op=torch.distributed.ReduceOp.SUM, group=mp_group)
+        if tp_group is not None:
+            dist.all_reduce(tensor=total_norm_cuda, op=torch.distributed.ReduceOp.SUM, group=tp_group)
 
         total_norm = total_norm_cuda[0].item()**(1. / norm_type)
 
     if total_norm == float('inf') or total_norm == -float('inf') or total_norm != total_norm:
         total_norm = -1
 
     return total_norm
 
 
-def sync_param(flat_tensor, tensor_list):
+def sync_tensor(flat_tensor, tensor_list):
     """
     Synchronize the flattened tensor and unflattened tensor list. When
     a list of tensor are flattened with `torch._utils._unflatten_dense_tensors`,
     a new tensor is created. Thus, the flat tensor and original tensor list do not
     share the same memory space. This function will update the tensor list so that
     they point to the same value.
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/low_level/bookkeeping/tensor_bucket.py` & `colossalai-nightly-2023.8.5/colossalai/zero/low_level/bookkeeping/tensor_bucket.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/low_level/low_level_optim.py` & `colossalai-nightly-2023.8.5/colossalai/zero/low_level/low_level_optim.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 # this code is inspired by the DeepSpeed library and implemented with our own design from scratch
+import copy
+from contextlib import contextmanager
 from functools import partial
-from typing import Optional
+from typing import Dict, Iterator, Optional, Tuple
 
 import torch
 import torch.distributed as dist
+from torch.distributed import ProcessGroup
 from torch.optim import Optimizer
 
 from colossalai.amp.naive_amp.mixed_precision_mixin import (
     BF16MixedPrecisionMixin,
     FP16MixedPrecisionMixin,
     MixedPrecisionMixin,
 )
-from colossalai.context import ParallelMode
-from colossalai.core import global_context as gpc
+from colossalai.interface import OptimizerWrapper
 from colossalai.logging import get_dist_logger
-from colossalai.nn.optimizer import ColossalaiOptimizer
-from colossalai.tensor import ColoParameter, ProcessGroup
+# from colossalai.tensor import ColoParameter, ProcessGroup
 from colossalai.utils.cuda import get_current_device
 
 from ._utils import (
     calculate_global_norm_from_list,
     compute_norm,
     flatten,
     has_inf_or_nan,
-    reduce_tensor_dp_group,
     release_param_grad,
-    split_by_dtype,
-    sync_param,
+    sync_tensor,
 )
-from .bookkeeping import BucketStore, GradientStore, ParameterStore, TensorBucket
+from .bookkeeping import BucketStore, GradientStore, ParameterStore
 
 
 class LowLevelZeroFP16MixedPrecisionMixin(FP16MixedPrecisionMixin):
 
     def __init__(self,
                  num_working_param_groups: int,
                  grad_store: GradientStore,
@@ -46,21 +45,21 @@
         super().__init__(initial_scale, min_scale, growth_factor, backoff_factor, growth_interval, hysteresis,
                          max_scale)
         self.num_working_param_groups = num_working_param_groups
         self.grad_store = grad_store
 
     def check_local_overflow(self) -> bool:
         for group_id in range(self.num_working_param_groups):
-            for avg_grad in self.grad_store.get_averaged_gradients_by_group(group_id):
+            for avg_grad in self.grad_store.get_working_grads_by_group_id(group_id):
                 if avg_grad is not None and has_inf_or_nan(avg_grad):
                     return True
         return False
 
 
-class LowLevelZeroOptimizer(ColossalaiOptimizer):
+class LowLevelZeroOptimizer(OptimizerWrapper):
     """Optimizer used for ZeRO-1 and ZeRO-2.
     """
 
     def __init__(
             self,
             optimizer: Optimizer,
             initial_scale: int = 2**16,    # grad scaler config
@@ -73,60 +72,44 @@
             clip_grad_norm: float = 0.0,    # grad clipping
             verbose: bool = False,
             reduce_bucket_size: int = 1024 * 1024,    # communication
             communication_dtype: Optional[torch.dtype] = None,
             overlap_communication: bool = False,
             partition_grad: bool = False,    # stage 2 flag
             cpu_offload: bool = False,    # cpu offload
+            dp_process_group: Optional[ProcessGroup] = None,    # the dp pg for comm
+            tp_process_group: Optional[ProcessGroup] = None,    # if using tp
             forced_dtype: Optional[torch.dtype] = None):
 
-        # TODO: add support for
-        # 1. fp16 master weights
-        # 2. contiguous gradients
-        # 3. cpu offload
-        # 4. support when some parameters requires_grad = False
-        # 5. support layer drop
+        # TODO:
+        # 1. state_dict for checkpoint IO
+
         super(LowLevelZeroOptimizer, self).__init__(optim=optimizer)
         self._dtype = self.optim.param_groups[0]['params'][0].dtype
         self._logger = get_dist_logger()
         self._verbose = verbose
 
         # stage 2
         self._partition_grads = partition_grad
 
         self._cpu_offload = cpu_offload
 
-        colo_pg = self._search_colo_process_group()
-        if isinstance(colo_pg, ProcessGroup):
-            self._local_rank = colo_pg.dp_local_rank()
-            self._world_size = colo_pg.dp_world_size()
-            self._dp_global_ranks = colo_pg.get_ranks_in_dp()
-            self._dp_torch_group = colo_pg.dp_process_group()
-            self._mp_torch_group = None
-            if colo_pg.tp_world_size() > 1:
-                self._mp_torch_group = colo_pg.tp_process_group()
-        elif colo_pg is None:
-            dp_parallel_mode = ParallelMode.DATA
-            mp_parallel_mode = ParallelMode.MODEL
-
-            self._dp_parallel_mode = dp_parallel_mode
-            self._mp_parallel_mode = mp_parallel_mode
-            self._local_rank = gpc.get_local_rank(dp_parallel_mode)
-            self._world_size = gpc.get_world_size(dp_parallel_mode)
-            self._dp_global_ranks = gpc.get_ranks_in_group(dp_parallel_mode)
-            self._dp_torch_group = gpc.get_group(dp_parallel_mode)
-            self._mp_torch_group = None
-            if gpc.is_initialized(mp_parallel_mode) and gpc.get_world_size(mp_parallel_mode) > 1:
-                self._mp_torch_group = gpc.get_group(mp_parallel_mode)
-        else:
-            raise NotImplementedError
+        # grad accumulation
+        self.require_grad_sync = True
+
+        # if process_group is none, will use the default one
+        self.dp_pg = dp_process_group
+        self._local_rank = dist.get_rank(group=self.dp_pg)
+        self._world_size = dist.get_world_size(group=self.dp_pg)
+
+        self.tp_pg = tp_process_group
 
         # working and master params for mixed precision training
         self._working_param_groups = dict()
-        self._master_flat_param_groups_of_current_rank = dict()
+        self._master_param_groups_of_current_rank = dict()
 
         # communication params
         self._overlap_communication = overlap_communication
         self._reduce_bucket_size = reduce_bucket_size
         self._communication_dtype = communication_dtype
 
         # gradient clipping
@@ -140,79 +123,41 @@
             self._dtype = forced_dtype
 
         # check argument conflict
         self._sanity_checks()
 
         # ParameterStore will manage the tensor buffers used for zero
         # it will not manage the tensors used by mixed precision training
-        self._param_store = ParameterStore(self._dp_torch_group)
-        self._grad_store = GradientStore(self._dp_torch_group)
-        self._bucket_store = BucketStore(self._dp_torch_group)
+        self._param_store = ParameterStore(self.dp_pg)
+        self._grad_store = GradientStore(self.dp_pg, partition_grad=partition_grad)
+        self._bucket_store = BucketStore(self.dp_pg)
 
         # iterate over the param group in the optimizer
         # partition these param groups for data parallel training
         # and add buffers to parameter store for future access
         for group_id, param_group in enumerate(self.optim.param_groups):
             group_params = list()
             for param in param_group['params']:
                 if param.requires_grad:
                     group_params.append(param)
 
             # add the working params to working_param_groups for bookkeeping
             self._working_param_groups[group_id] = group_params
 
-            # assign parameters to ranks
-            # the params in the list are sorted
-            params_per_rank = self._partition_param_list(group_params)
-
-            # store the mapping between param to rank
-            # each param should belong to only one rank
-            for rank, params in enumerate(params_per_rank):
-                self._param_store.add_param_list_by_rank_group(rank, group_id, params)
-                for param in params:
-                    self._param_store.set_param_to_rank(param, rank)
+            master_param_current_rank = self._create_master_param_current_rank(group_params)
 
-            # move to cpu to make room to create the flat tensor
-            # move_tensor(params, device='cpu')
-            for param in group_params:
-                param.data = param.data.cpu()
-
-            # flatten the reordered tensors
-            for rank in range(self._world_size):
-                tensor_list = self._param_store.get_params_by_rank_group(rank, group_id)
-                with torch.no_grad():
-                    flat_tensor = flatten(tensor_list)
-                flat_tensor = flat_tensor.data.cuda()
-                self._param_store.add_flat_param_by_rank_group(rank, group_id, flat_tensor)
-
-            # sync parameters
-            for rank in range(self._world_size):
-                flat_tensor = self._param_store.get_flat_param_by_rank_group(rank, group_id)
-                tensor_list = self._param_store.get_params_by_rank_group(rank, group_id)
-                sync_param(flat_tensor=flat_tensor, tensor_list=tensor_list)
-
-            # create a copy of fp32 master weights of the parameters for which this rank is responsible
-            working_flat_current_rank = self._param_store.get_flat_param_by_rank_group(self._local_rank, group_id)
-            master_flat_current_rank = working_flat_current_rank.float()
-            device = 'cpu' if self._cpu_offload else get_current_device()
-            master_flat_current_rank = master_flat_current_rank.to(device)
-            master_flat_current_rank.requires_grad = True
-            self._master_flat_param_groups_of_current_rank[group_id] = master_flat_current_rank
+            self._master_param_groups_of_current_rank[group_id] = master_param_current_rank
 
             # need to replace the params in the `params` field in the optimizer
             # so that when the optimizer calls step(), it only updates the tensors
             # managed by this data parallel rank
-            param_group['params'] = [master_flat_current_rank]
+            param_group['params'] = master_param_current_rank
 
-            # set reduction state
-            for param in self._working_param_groups[group_id]:
-                self._param_store.set_param_reduction_state(param, False)
-
-        # initialize communication stream for
-        # communication-computation overlapping
+        # intialize communication stream for
+        # communication-compuation overlapping
         if self._overlap_communication:
             self._comm_stream = torch.cuda.Stream()
 
         # reduction hook is only used if overlapping communication
         # or stage 2 is used
         # if it is stage 1 without overlapping, no hook will be attached
         if self._overlap_communication or self._partition_grads:
@@ -245,205 +190,143 @@
         assert torch.cuda.is_available(), 'CUDA is required'
         for param_group in self.optim.param_groups:
             group_params = param_group['params']
             for param in group_params:
                 assert param.dtype == self._dtype, \
                     f"Parameters are expected to have the same dtype `{self._dtype}`, but got `{param.dtype}`"
 
-    def _search_colo_process_group(self):
-        colo_flag = False
-        colo_pg = None
-        for param_group in self.optim.param_groups:
-            group_params = param_group['params']
-            for param in group_params:
-                if isinstance(param, ColoParameter):
-                    colo_flag = True
-                    if colo_pg is None:
-                        colo_pg = param.get_process_group()
-                    else:
-                        assert colo_pg == param.get_process_group(), "All parameters should be in a same process group"
-                elif colo_flag:
-                    raise RuntimeError("All parameters should be ColoParameter if you use ColoParameter.")
-        return colo_pg
-
-    def _partition_param_list(self, param_list):
-        params_per_rank = [[] for _ in range(self._world_size)]
-        numel_per_rank = [0 for _ in range(self._world_size)]
-
-        # partition the parameters in a greedy fashion
-        sorted_params = sorted(param_list, key=lambda x: x.numel(), reverse=True)
-        for param in sorted_params:
-            # allocate this parameter to the rank with
-            # the smallest numel for load balancing purpose
-            rank_to_go = numel_per_rank.index(min(numel_per_rank))
-            params_per_rank[rank_to_go].append(param)
-            numel_per_rank[rank_to_go] += param.numel()
-
-        if self._verbose:
-            self._logger.info(f'Number of elements on ranks: {numel_per_rank}', ranks=[0])
-        return params_per_rank
+    def _create_master_param_current_rank(self, param_list):
+        # split each param evenly by world size
+        params_current_rank = []
+        device = 'cpu' if self._cpu_offload else get_current_device()
+
+        for param in param_list:
+            padding_size = (self._world_size - param.numel() % self._world_size) % self._world_size
+            self._param_store.record_param_padding_size(param, padding_size)
+
+            with torch.no_grad():
+                if padding_size > 0:
+                    padding_param = torch.nn.functional.pad(param.data.view(-1), [0, padding_size])
+                else:
+                    padding_param = param.data.view(-1)
+                splited_params = padding_param.split(padding_param.numel() // self._world_size)
+
+                splited_param_current_rank = splited_params[self._local_rank].detach().float().to(device)
+                params_current_rank.append(splited_param_current_rank)
+                self._param_store.link_master_and_working_param(splited_param_current_rank, param)
+
+        return params_current_rank
 
     ###########################
     # Backward Reduction Hook #
     ###########################
 
-    def _grad_handler(self, param, grad, reduce_rank):
-        self._add_to_reduction_bucket(param, reduce_rank)
+    def _grad_handler(self, param, group_id, grad):
+        # if run with no_sync context, would not sync grad when backward
+        if self.require_grad_sync:
+            self._add_to_bucket(param, group_id)
         return grad
 
     def _attach_reduction_hook(self):
         # we iterate over the working params
         # on each param, we register a hook to its AccumulateGrad object
         for group_id in range(self.num_param_groups):
             param_group = self._working_param_groups[group_id]
             for param in param_group:
                 if param.requires_grad:
-                    # determines the reduction destination rank
-                    # this is only valid for stage 2
-                    # dst_rank = None means using all-reduce
-                    # else using reduce
-                    if self._partition_grads:
-                        reduce_rank = self._param_store.get_param_rank(param)
-                    else:
-                        reduce_rank = None
-
-                    param.register_hook(partial(self._grad_handler, param, reduce_rank=reduce_rank))
-
-    def _reduce_tensor_bucket(self, bucket: TensorBucket, reduce_rank):
-        if self._overlap_communication:
-            torch.cuda.synchronize()
-            self._param_store.clear_grads_of_previous_reduced_params()
-            stream = self._comm_stream
-        else:
-            stream = torch.cuda.current_stream()
-
-        with torch.cuda.stream(stream):
-            flat = bucket.flatten()
-            reduce_global_rank = None
-            if reduce_rank is not None:
-                reduce_global_rank = self._dp_global_ranks[reduce_rank]
-            reduced_flat = reduce_tensor_dp_group(tensor=flat,
-                                                  dtype=self._communication_dtype,
-                                                  dst_local_rank=reduce_rank,
-                                                  dst_global_rank=reduce_global_rank,
-                                                  group=self._dp_torch_group)
-
-            # update the reduced tensor
-            if reduce_rank is None or reduce_rank == self._local_rank:
-                bucket.unflatten_and_copy(reduced_flat)
-
-    def _reduce_tensor_list_with_one_dtype(self, tensor_list, bucket_size, reduce_rank):
-        param_bucket = TensorBucket(size=bucket_size)
-
-        for tensor in tensor_list:
-            param_bucket.add_to_bucket(tensor, allow_oversize=True)
-
-            if param_bucket.is_full_or_oversized():
-                self._reduce_tensor_bucket(bucket=param_bucket, reduce_rank=reduce_rank)
-                param_bucket.empty()
-
-        if not param_bucket.is_empty():
-            self._reduce_tensor_bucket(bucket=param_bucket, reduce_rank=reduce_rank)
-
-    def _reduce_grads(self, reduce_rank, grads, bucket_size):
-        grad_buckets_by_dtype = split_by_dtype(grads)
-
-        for tensor_list in grad_buckets_by_dtype:
-            self._reduce_tensor_list_with_one_dtype(tensor_list=tensor_list,
-                                                    bucket_size=bucket_size,
-                                                    reduce_rank=reduce_rank)
+                    param.register_hook(partial(self._grad_handler, param, group_id))
 
     #######################
     # Reduction Functions #
     #######################
 
-    def _run_reduction(self, reduce_rank=None):
-        # reduce grads
-        self._reduce_grads(reduce_rank=reduce_rank,
-                           grads=self._bucket_store.get_grad(reduce_rank=reduce_rank),
-                           bucket_size=self._bucket_store.num_elements_in_bucket(reduce_rank))
-
-        # use communication stream if overlapping
-        # communication with computation
-        if self._overlap_communication:
-            stream = self._comm_stream
-        else:
-            stream = torch.cuda.current_stream()
+    def _run_reduction(self):
+        if self._bucket_store.num_elements_in_bucket() > 0:
+            self._bucket_store.build_grad_in_bucket()
+            flat_grads = self._bucket_store.get_flatten_grad()
+            flat_grads /= self._world_size
+            if self._overlap_communication:
+                stream = self._comm_stream
+            else:
+                stream = torch.cuda.current_stream()
+
+            with torch.cuda.stream(stream):
+                group_id = self._bucket_store.current_group_id
+
+                grad_dtype = flat_grads.dtype
+                if self._communication_dtype is not None:
+                    flat_grads = flat_grads.to(self._communication_dtype)
+
+                if not self._partition_grads:
+                    dist.all_reduce(flat_grads, group=self.dp_pg)
+                    if flat_grads.dtype != grad_dtype:
+                        flat_grads = flat_grads.to(grad_dtype)
+
+                    flat_grads_per_rank = flat_grads.split(flat_grads.numel() // self._world_size)
+                    grad_in_bucket = self._bucket_store.get_grad()
+
+                    for rank, grad_list in grad_in_bucket.items():
+                        sync_tensor(flat_grads_per_rank[rank], grad_list)
+                        for grad in grad_list:
+                            param_id = self._bucket_store.get_param_id_of_grad(grad)
+                            self._grad_store.append_gradients_by_param_id(grad, group_id, param_id)
 
-        with torch.cuda.stream(stream):
-            params_in_bucket = self._bucket_store.get_param(reduce_rank=reduce_rank)
-
-            for param in params_in_bucket:
-                # the is_param_reduced flag should be False showing that
-                # this param is not reduced before calling self._reduce_grads_by_rank
-                is_param_reduced = self._param_store.is_param_reduced(param)
-
-                if is_param_reduced:
-                    msg = f'Parameter of size ({param.size()}) has been reduced, ' + \
-                          'duplicate reduction will lead to arithmetic incorrectness'
-                    raise RuntimeError(msg)
-
-                # update the flag
-                self._param_store.set_param_reduction_state(param, True)
-
-                # if partition grads = True
-                # we do not keep the gradient after reduction
-                if self._partition_grads and not self._param_store.belongs_to_current_rank(param):
-                    if self._overlap_communication:
-                        # we need to keep this gradient for now as reduction may
-                        # be completed yet since it is using a different cuda stream
-                        self._param_store.add_previous_reduced_param(param)
-                    else:
-                        param.grad = None
+                else:
+                    flat_grads_list = list(flat_grads.split(len(flat_grads) // self._world_size))
+                    recieved_grad = torch.zeros_like(flat_grads_list[0])
+                    dist.reduce_scatter(recieved_grad, flat_grads_list, group=self.dp_pg)
+
+                    if recieved_grad.dtype != grad_dtype:
+                        recieved_grad = recieved_grad.to(grad_dtype)
+
+                    grad_in_bucket_current_rank = self._bucket_store.get_grad()[self._local_rank]
+                    sync_tensor(recieved_grad, grad_in_bucket_current_rank)
+                    for grad in grad_in_bucket_current_rank:
+                        param_id = self._bucket_store.get_param_id_of_grad(grad)
+                        self._grad_store.append_gradients_by_param_id(grad, group_id, param_id)
 
-        self._bucket_store.reset_by_rank(reduce_rank)
+                self._bucket_store.reset()
 
-    def _add_to_reduction_bucket(self, param, reduce_rank=None):
+    def _add_to_bucket(self, param, group_id):
         param_size = param.numel()
 
         # check if the bucket is full
         # if full, will reduce the grads already in the bucket
+        # or got a grad of param from another group
         # after reduction, the bucket will be empty
-        if self._bucket_store.num_elements_in_bucket(reduce_rank) + param_size > self._reduce_bucket_size:
-            self._run_reduction(reduce_rank)
+        if self._bucket_store.num_elements_in_bucket() + param_size > self._reduce_bucket_size or \
+            group_id != self._bucket_store.current_group_id:
+            self._run_reduction()
 
-        # the param must not be reduced to ensure correctness
-        is_param_reduced = self._param_store.is_param_reduced(param)
-        if is_param_reduced:
-            msg = f'Parameter of size ({param.size()}) has already been reduced, ' \
-                  + 'duplicate reduction will lead to arithmetic incorrectness'
-            raise RuntimeError(msg)
-
-        self._bucket_store.add_num_elements_in_bucket(param_size, reduce_rank)
-        self._bucket_store.add_param(param, reduce_rank)
+        padding_size = self._param_store.get_param_padding_size(param)
+        self._bucket_store.add_param_grad(group_id, param, padding_size)
 
     ################################
     # torch.optim.Optimizer methods
     ################################
 
-    def backward(self, loss, retain_graph=False, sync_grad=True):
+    def backward(self, loss, retain_graph=False):
+        assert not(self._partition_grads and not self.require_grad_sync), \
+            "ZeRO2(partition_grads) and gradient accumulation(no_sync) are not compatible"
+
         if self.mixed_precision_mixin is not None:
             loss = self.mixed_precision_mixin.pre_backward(loss)
+
         loss.backward(retain_graph=retain_graph)
 
-        # finish gradient reduction
-        if not self._partition_grads:
-            self._reduce_grad_stage1()
-        else:
-            # TODO: support async comm in reduce
-            self._reduce_grad_stage2()
+        if not self.require_grad_sync:
+            return
+
+        self._reduce_grad(self._partition_grads)
 
         # clear reduced grads
         if self._overlap_communication:
             torch.cuda.synchronize()
-            self._param_store.clear_grads_of_previous_reduced_params()
 
-        # gradient synchronization
-        if sync_grad:
-            self._sync_grad()
+        self.zero_grad()
 
     def zero_grad(self, set_to_none=True):
         """
         Set parameter gradients to zero. If set_to_none = True, gradient
         will be set to None to save memory.
 
         :param set_to_none: Whether set the gradient to None. Default value is True.
@@ -463,76 +346,88 @@
     ####################
     # Update Parameter #
     ####################
 
     def step(self, closure=None):
         assert closure is None, 'closure is not supported by step()'
 
+        if not self.require_grad_sync:
+            return
+
         if self.mixed_precision_mixin is not None and self.mixed_precision_mixin.should_skip_step():
-            self._grad_store.reset_all_average_gradients()
+            self._grad_store.reset_all_gradients()
             if self._verbose:
                 self._logger.info(f'Found overflow. Skip step')
             self.zero_grad()
             return
 
-        # copy the grad of working param to master param
-        single_grad_partition_groups = []
+        # record all grads for unscale and clip
+        grad_partition_groups = []
         norm_groups = []
 
+        # sometimes not all params are 'really' working
+        # for instance, when layer drop, the dropped layer has no grad
+        # and should not be updated
+        real_working_params = dict()
+        real_master_params = dict()
+
+        grad_index = 0 if self._partition_grads else self._local_rank
+
         for group_id in range(self.num_param_groups):
+            master_params = self._master_param_groups_of_current_rank[group_id]
+            real_working_params[group_id] = []
+            real_master_params[group_id] = []
+            for splited_param in master_params:
+                working_param = self._param_store.master_to_working_param[id(splited_param)]
+                # if a working param requires grad and has no grad
+                # it is not 'really' working, e.g. the droped layer
+                # else the splited grad should be attached to the splited param
+                grads = self._grad_store.get_partitioned_gradients_by_param_id(group_id, id(working_param))
+                if len(grads) > 0:
+                    real_working_params[group_id].append(working_param)
+                    grad = grads[grad_index].to(splited_param.dtype).to(splited_param.device)
+                    splited_param.grad = grad
+                    grad_partition_groups.append(grad)
+                    real_master_params[group_id].append(splited_param)
+
             # compute norm
-            norm_group = compute_norm(gradients=self._grad_store.get_averaged_gradients_by_group(group_id),
-                                      params=self._param_store.get_params_by_rank_group(group_id=group_id,
-                                                                                        rank=self._local_rank),
-                                      dp_group=self._dp_torch_group,
-                                      mp_group=self._mp_torch_group)
+            working_grads = self._grad_store.get_working_grads_by_group_id(group_id)
+            norm_group = compute_norm(gradients=working_grads, dp_group=self.dp_pg, tp_group=self.tp_pg)
             norm_groups.append(norm_group)
 
-            # create flat gradient for the flat fp32 master params
-            working_avg_grads = self._grad_store.get_averaged_gradients_by_group(group_id)
-            flat_working_avg_grads = flatten(working_avg_grads)
-
-            dtype = self._master_flat_param_groups_of_current_rank[group_id].dtype
-            flat_master_avg_grads = flat_working_avg_grads.to(dtype)
-
-            param_shape = self._master_flat_param_groups_of_current_rank[group_id].shape
-            assert param_shape == flat_master_avg_grads.shape, \
-                f'fp32 param and grad have different shape {param_shape} vs {flat_master_avg_grads.shape}'
-
-            single_grad_partition_groups.append(flat_master_avg_grads)
-            device = self._master_flat_param_groups_of_current_rank[group_id].device
-            self._master_flat_param_groups_of_current_rank[group_id].grad = flat_master_avg_grads.to(device)
-            self._grad_store.reset_average_gradients_by_group(group_id)
+            self._grad_store.reset_grads_by_group_id(group_id)
+
+            # update the params in the optimizer
+            self.optim.param_groups[group_id]['params'] = real_master_params[group_id]
 
         # unscale and clip grads
         global_norm = calculate_global_norm_from_list(norm_list=norm_groups)
-        self._unscale_and_clip_grads(single_grad_partition_groups, global_norm)
+        self._unscale_and_clip_grads(grad_partition_groups, global_norm)
 
         # update the parameters
         self.optim.step()
-        # release the master grad
-        release_param_grad(self._master_flat_param_groups_of_current_rank.values())
 
-        # update working partition updated by the current rank
-        for group_id in range(len(self._working_param_groups)):
-            working_param = self._param_store.get_flat_param_by_rank_group(rank=self._local_rank, group_id=group_id)
-            master_param = self._master_flat_param_groups_of_current_rank[group_id]
-            working_param.data.copy_(master_param)
+        # release the grad
+        grad_partition_groups = []
+        for group_id in range(self.num_param_groups):
+            release_param_grad(self._master_param_groups_of_current_rank[group_id])
 
-        # broadcast the updated model weights
-        handles = []
+        # update working partition updated by the current rank
+        dtype = real_working_params[0][0].dtype
         for group_id in range(self.num_param_groups):
-            for index in range(self._world_size):
-                rank = self._dp_global_ranks[index]
-                working_param = self._param_store.get_flat_param_by_rank_group(rank=index, group_id=group_id)
-                handle = dist.broadcast(working_param, src=rank, group=self._dp_torch_group, async_op=True)
-                handles.append(handle)
+            master_working_param = self.optim.param_groups[group_id]['params']
+            for idx, splited_param in enumerate(master_working_param):
+                working_param = real_working_params[group_id][idx]
+                all_splited_param = [
+                    torch.zeros(splited_param.shape, device="cuda", dtype=dtype) for _ in range(self._world_size)
+                ]
+                dist.all_gather(all_splited_param, splited_param.cuda().to(dtype), group=self.dp_pg)
+                working_param.data.copy_(flatten(all_splited_param)[:working_param.numel()].reshape_as(working_param))
 
-        for handle in handles:
-            handle.wait()
+            self.optim.param_groups[group_id]['params'] = self._master_param_groups_of_current_rank[group_id]
 
     #############################
     # Mixed Precision Utilities #
     #############################
 
     def _unscale_and_clip_grads(self, grad_groups_flat, total_norm):
         # compute combined scale factor for this group
@@ -549,53 +444,143 @@
         for grad in grad_groups_flat:
             grad.data.mul_(1. / div_scale)
 
     ############################
     # Gradient Synchronization #
     ############################
 
-    def _sync_grad(self):
-        # update param already reduced flag
-        reduction_states = self._param_store.get_param_reduction_states()
-        for tensor, _ in reduction_states.items():
-            reduction_states[tensor] = False
-
-        # accumulate gradient
+    # this method is used to sync gradient manually
+    def sync_grad(self):
         for group_id in range(self.num_param_groups):
-            param_group = self._param_store.get_params_by_rank_group(self._local_rank, group_id)
-
-            avg_gradients_group = self._grad_store.get_averaged_gradients_by_group(group_id)
-
-            param_idx = 0
+            param_group = self._working_param_groups[group_id]
             for param in param_group:
-                if param.grad is not None:
-                    if len(avg_gradients_group) == param_idx:
-                        self._grad_store.append_average_gradient_by_group(group_id, param.grad)
-                    else:
-                        self._grad_store.add_average_gradient_by_group(group_id, param_idx, param.grad)
-                    param_idx += 1
+                if param.requires_grad and param.grad is not None:
+                    self._add_to_bucket(param, group_id)
 
-        # the gradients needed are stored in the avg_gradients buffer
-        # thus, can clear this
-        self.zero_grad()
+        self._run_reduction()
 
-    def _reduce_grad_stage1(self):
-        # if not overlapping communication (no reduction hook is attached)
+    def _reduce_grad(self, partition_grad):
+        # if not overlapping communication (no reduction hook is attached) when zero1
         # we need to manually reduce these gradients
-        if not self._overlap_communication:
-            for group_id in range(len(self._working_param_groups)):
-                param_group = self._working_param_groups[group_id]
-                for param in param_group:
-                    if param.grad is not None:
-                        self._add_to_reduction_bucket(param)
+        if not partition_grad and not self._overlap_communication:
+            self.sync_grad()
+        else:
+            self._run_reduction()
 
-        # we need to reduce the gradients
-        # left in the communication bucket
-        self._run_reduction()
+    # this context comes from pytorch DDP
+    @contextmanager
+    def no_sync(self):
+        old_require_grad_sync = self.require_grad_sync
+        self.require_grad_sync = False
+        try:
+            yield
+        finally:
+            self.require_grad_sync = old_require_grad_sync
+
+    ##############
+    # State Dict #
+    ##############
+
+    def _pack_state(self, state: Dict) -> Dict:
+        # comes from pytorch optimizer.state_dict()
+        param_mappings = {}
+        start_index = 0
+
+        def pack_group(group):
+            nonlocal start_index
+            packed = {k: v for k, v in group.items() if k != 'params'}
+            param_mappings.update(
+                {id(p): i for i, p in enumerate(group['params'], start_index) if id(p) not in param_mappings})
+            packed['params'] = [param_mappings[id(p)] for p in group['params']]
+            start_index += len(packed['params'])
+            return packed
+
+        param_groups = [pack_group(g) for g in self.optim.param_groups]
+        # Remap state to use order indices as keys
+        packed_state = {(param_mappings[id(k)] if isinstance(k, torch.Tensor) else k): v for k, v in state.items()}
+
+        return {'state': packed_state, 'param_groups': param_groups}
+
+    def state_dict(self) -> Dict:
+        """Return a state_dict same with DDP
+
+        Returns:
+            Dict: the pytorch form state_dict
+        """
+        zero_state = dict()
+        for param, state in self.optim.state.items():
+            zero_state[param] = copy.deepcopy(state)
+            for k, v in state.items():
+                if isinstance(v, torch.Tensor) and k != 'step':
+                    working_param = self._param_store.master_to_working_param[id(param)]
+                    gather_tensor = [torch.zeros_like(v) for _ in range(self._world_size)]
+                    dist.all_gather(gather_tensor, v, group=self.dp_pg)
+                    param_state = torch.stack(gather_tensor).view(-1)[:working_param.numel()].reshape_as(working_param)
+                    zero_state[param][k] = param_state
+
+        states_dict = self._pack_state(zero_state)
+
+        return states_dict
+
+    def load_state_dict(self, state_dict: Dict):
+        """Load state dict, requires the state_dict be the pytorch form
+
+        Args:
+            state_dict (dict): A pytorch form state_dict
+        """
+        zero_state_dict = copy.deepcopy(state_dict)
+        for param_idx, state in zero_state_dict['state'].items():
+            for k, v in state.items():
+                if isinstance(v, torch.Tensor) and k != 'step':
+                    padding_size = (self._world_size - v.numel() % self._world_size) % self._world_size
+                    with torch.no_grad():
+                        v = v.flatten()
+                        if padding_size > 0:
+                            v = torch.nn.functional.pad(v, [0, padding_size])
+                        v_list = v.split(v.numel() // self._world_size)
+                        zero_state_dict['state'][param_idx][k] = v_list[self._local_rank].detach()
+
+        self.optim.load_state_dict(zero_state_dict)
+        zero_state_dict = dict()
+
+    def state_dict_shard(self, max_shard_size: int = 1024) -> Iterator[Tuple[Dict, int]]:
+        """Returns dictionaries containing a whole state of the module one by one. The max size of dictionary shard is specified by ``max_shard_size``.
+           Only include the 'state' in state_dict.
+
+        Args:
+            max_shard_size (int, optional): max size of state shard (in MB). Defaults to 1024.
+
+        Yields:
+            Iterator[OrderedDict]: A generator of state dict shard
+        """
+        ret_block = dict()
+        ret_block_size = 0
+
+        local_states = self.optim.state_dict()['state']
+        for param_idx, states in local_states.items():
+            current_block_size = 0
+            current_block = copy.deepcopy(states)
+
+            # find the working param of current param_id
+            for group_id, pg in self._master_param_groups_of_current_rank.items():
+                if (group_id + 1) * len(pg) < param_idx:
+                    continue
+                master_param = pg[param_idx - (group_id) * len(pg)]
+                working_param = self._param_store.master_to_working_param[id(master_param)]
+
+            for k, v in states.items():
+                if isinstance(v, torch.Tensor) and k != 'step':
+                    state_tensor = [torch.zeros_like(v) for _ in range(self._world_size)]
+                    dist.all_gather(state_tensor, v, group=self.dp_pg)
+                    state_tensor = torch.stack(state_tensor).view(-1)[:working_param.numel()].reshape_as(working_param)
+                    current_block_size += state_tensor.numel()
+                    current_block[k] = state_tensor
+
+            if ret_block_size + current_block_size > max_shard_size and len(ret_block) > 0:
+                yield ret_block, ret_block_size
+                ret_block = dict()
+                ret_block_size = 0
+
+            ret_block[param_idx] = current_block
+            ret_block_size += current_block_size
 
-    def _reduce_grad_stage2(self):
-        # when partition_grads is True, reduction hooks
-        # are attached in the __init__ function, so we
-        # only need to reduce the gradients
-        # left in the communication bucket
-        for reduce_rank in range(self._world_size):
-            self._run_reduction(reduce_rank)
+        yield ret_block, ret_block_size
```

### Comparing `colossalai-nightly-2023.7.8/colossalai/zero/wrapper.py` & `colossalai-nightly-2023.8.5/colossalai/zero/wrapper.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/PKG-INFO` & `colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colossalai-nightly
-Version: 2023.7.8
+Version: 2023.8.5
 Summary: An integrated large-scale model training system with efficient parallelization techniques
 Home-page: https://www.colossalai.org
 License: Apache Software License 2.0
 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/discussions
 Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/issues
 Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io
@@ -32,22 +32,23 @@
         
         
            | [English](README.md) | [中文](docs/README-zh-Hans.md) |
         
         </div>
         
         ## Latest News
+        * [2023/07] [HPC-AI Tech Raises 22 Million USD in Series A Funding](https://www.hpc-ai.tech/blog/hpc-ai-tech-raises-22-million-usd-in-series-a-funding-to-fuel-team-expansion-and-business-growth)
+        * [2023/07] [65B Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
         * [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-5edf08fb538b)
         * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction](https://www.hpc-ai.tech/blog/intel-habana)
         * [2023/03] [AWS and Google Fund Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-fund-colossal-ai-with-startup-cloud-programs)
         * [2023/02] [Open Source Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt)
         * [2023/01] [Hardware Savings Up to 46 Times for AIGC and  Automatic Parallelism](https://medium.com/pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-savings-up-to-46x-for-stable-1453b48f3f02)
         * [2022/11] [Diffusion Pretraining and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper)
         * [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding)
-        * [2022/09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https://www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-fundraising-led-by-bluerun-ventures-in-the)
         
         ## Table of Contents
         <ul>
          <li><a href="#Why-Colossal-AI">Why Colossal-AI</a> </li>
          <li><a href="#Features">Features</a> </li>
          <li>
            <a href="#Colossal-AI-in-the-Real-World">Colossal-AI for Real World Applications</a>
@@ -56,14 +57,15 @@
              <li><a href="#AIGC">AIGC: Acceleration of Stable Diffusion</a></li>
              <li><a href="#Biomedicine">Biomedicine: Acceleration of AlphaFold Protein Structure</a></li>
            </ul>
          </li>
          <li>
            <a href="#Parallel-Training-Demo">Parallel Training Demo</a>
            <ul>
+             <li><a href="#LLaMA">LLaMA</a></li>
              <li><a href="#GPT-3">GPT-3</a></li>
              <li><a href="#GPT-2">GPT-2</a></li>
              <li><a href="#BERT">BERT</a></li>
              <li><a href="#PaLM">PaLM</a></li>
              <li><a href="#OPT">OPT</a></li>
              <li><a href="#ViT">ViT</a></li>
              <li><a href="#Recommendation-System-Models">Recommendation System Models</a></li>
@@ -223,14 +225,23 @@
         - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer): accelerating structure prediction of protein monomers and multimer by 11x.
         
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
         ## Parallel Training Demo
         
+        ### LLaMA
+        <p align="center">
+        <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/images/LLaMA_pretraining.png" width=600/>
+        </p>
+        
+        - 65-billion-parameter large model pretraining accelerated by 38%
+        [[code]](https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/llama)
+        [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining)
+        
         ### GPT-3
         <p align="center">
         <img src="https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT3-v5.png" width=700/>
         </p>
         
         - Save 50% GPU resources and 10.7% acceleration
         
@@ -459,15 +470,16 @@
           title={Colossal-AI: A Unified Deep Learning System For Large-Scale Parallel Training},
           author={Bian, Zhengda and Liu, Hongxin and Wang, Boxiang and Huang, Haichen and Li, Yongbin and Wang, Chuanrui and Cui, Fan and You, Yang},
           journal={arXiv preprint arXiv:2110.14883},
           year={2021}
         }
         ```
         
-        Colossal-AI has been accepted as official tutorial by top conferences [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/Conferences/AAAI-23/), [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), etc.
+        Colossal-AI has been accepted as official tutorial by top conferences [NeurIPS](https://nips.cc/), [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/Conferences/AAAI-23/), 
+        [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), [NVIDIA GTC](https://www.nvidia.com/en-us/on-demand/session/gtcspring23-S51482/) ,etc.
         
         <p align="right">(<a href="#top">back to top</a>)</p>
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Environment :: GPU :: NVIDIA CUDA
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.7.8 Summary: An
+Metadata-Version: 2.1 Name: colossalai-nightly Version: 2023.8.5 Summary: An
 integrated large-scale model training system with efficient parallelization
 techniques Home-page: https://www.colossalai.org License: Apache Software
 License 2.0 Project-URL: Forum, https://github.com/hpcaitech/ColossalAI/
 discussions Project-URL: Bug Tracker, https://github.com/hpcaitech/ColossalAI/
 issues Project-URL: Examples, https://github.com/hpcaitech/ColossalAI-Examples
 Project-URL: Documentation, http://colossalai.readthedocs.io Project-URL:
 Github, https://github.com/hpcaitech/ColossalAI Description: # Colossal-AI
@@ -22,43 +22,47 @@
  (https://img.shields.io/badge/%F0%9F%A4%97HuggingFace-Join-yellow)](https://
 huggingface.co/hpcai-tech) [![slack badge](https://img.shields.io/badge/Slack-
   join-blueviolet?logo=slack&)](https://join.slack.com/t/colossalaiworkspace/
   shared_invite/zt-z7b26eeb-CBp7jouvu~r0~lcFzX832w) [![WeChat badge](https://
        img.shields.io/badge/å¾®ä¿¡-å å¥-green?logo=wechat&)](https://
     raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
     WeChat.png) | [English](README.md) | [ä¸­æ](docs/README-zh-Hans.md) |
-## Latest News * [2023/03] [ColossalChat: An Open-Source Solution for Cloning
-ChatGPT With a Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/
-colossalchat-an-open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-
-pipeline-5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver
-Cost-Efficient Open-Source Solution for Protein Folding Structure Prediction]
-(https://www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund
-Colossal-AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-
-google-fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source
-Solution Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU
-Memory](https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
+## Latest News * [2023/07] [HPC-AI Tech Raises 22 Million USD in Series A
+Funding](https://www.hpc-ai.tech/blog/hpc-ai-tech-raises-22-million-usd-in-
+series-a-funding-to-fuel-team-expansion-and-business-growth) * [2023/07] [65B
+Model Pretraining Accelerated by 38%, Best Practices for Building LLaMA-Like
+Base Models Open-Source](https://www.hpc-ai.tech/blog/large-model-pretraining)
+* [2023/03] [ColossalChat: An Open-Source Solution for Cloning ChatGPT With a
+Complete RLHF Pipeline](https://medium.com/@yangyou_berkeley/colossalchat-an-
+open-source-solution-for-cloning-chatgpt-with-a-complete-rlhf-pipeline-
+5edf08fb538b) * [2023/03] [Intel and Colossal-AI Partner to Deliver Cost-
+Efficient Open-Source Solution for Protein Folding Structure Prediction](https:
+//www.hpc-ai.tech/blog/intel-habana) * [2023/03] [AWS and Google Fund Colossal-
+AI with Startup Cloud Programs](https://www.hpc-ai.tech/blog/aws-and-google-
+fund-colossal-ai-with-startup-cloud-programs) * [2023/02] [Open Source Solution
+Replicates ChatGPT Training Process! Ready to go with only 1.6GB GPU Memory]
+(https://www.hpc-ai.tech/blog/colossal-ai-chatgpt) * [2023/01] [Hardware
 Savings Up to 46 Times for AIGC and Automatic Parallelism](https://medium.com/
 pytorch/latest-colossal-ai-boasts-novel-automatic-parallelism-and-offers-
 savings-up-to-46x-for-stable-1453b48f3f02) * [2022/11] [Diffusion Pretraining
 and Hardware Fine-Tuning Can Be Almost 7X Cheaper](https://www.hpc-ai.tech/
 blog/diffusion-pretraining-and-hardware-fine-tuning-can-be-almost-7x-cheaper) *
 [2022/10] [Use a Laptop to Analyze 90% of Proteins, With a Single-GPU Inference
 Sequence Exceeding 10,000](https://www.hpc-ai.tech/blog/use-a-laptop-to-
-analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) * [2022/
-09] [HPC-AI Tech Completes $6 Million Seed and Angel Round Fundraising](https:/
-/www.hpc-ai.tech/blog/hpc-ai-tech-completes-6-million-seed-and-angel-round-
-fundraising-led-by-bluerun-ventures-in-the) ## Table of Contents
+analyze-90-of-proteins-with-a-single-gpu-inference-sequence-exceeding) ## Table
+of Contents
     * Why_Colossal-AI
     * Features
     * Colossal-AI_for_Real_World_Applications
           o ColossalChat:_An_Open-Source_Solution_for_Cloning_ChatGPT_With_a
             Complete_RLHF_Pipeline
           o AIGC:_Acceleration_of_Stable_Diffusion
           o Biomedicine:_Acceleration_of_AlphaFold_Protein_Structure
     * Parallel_Training_Demo
+          o LLaMA
           o GPT-3
           o GPT-2
           o BERT
           o PaLM
           o OPT
           o ViT
           o Recommendation_System_Models
@@ -151,15 +155,20 @@
 - [FastFold with Intel](https://github.com/hpcaitech/FastFold): 3x inference
 acceleration and 39% cost reduce.
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                            xTrimoMultimer_Table.jpg]
 - [xTrimoMultimer](https://github.com/biomap-research/xTrimoMultimer):
 accelerating structure prediction of protein monomers and multimer by 11x.
                                                                   (back_to_top)
-## Parallel Training Demo ### GPT-3
+## Parallel Training Demo ### LLaMA
+   [https://raw.githubusercontent.com/hpcaitech/public_assets/main/examples/
+                         images/LLaMA_pretraining.png]
+- 65-billion-parameter large model pretraining accelerated by 38% [[code]]
+(https://github.com/hpcaitech/ColossalAI/tree/example/llama/examples/language/
+llama) [[blog]](https://www.hpc-ai.tech/blog/large-model-pretraining) ### GPT-3
 [https://raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/
                                  GPT3-v5.png]
 - Save 50% GPU resources and 10.7% acceleration ### GPT-2 [https://
 raw.githubusercontent.com/hpcaitech/public_assets/main/colossalai/img/GPT2.png]
 - 11x lower GPU memory consumption, and superlinear scaling efficiency with
 Tensor Parallelism [https://raw.githubusercontent.com/hpcaitech/public_assets/
 main/colossalai/img/(updated)GPT-2.png] - 24x larger model size on the same
@@ -281,16 +290,18 @@
 like to credit these amazing projects as listed in the [Reference List](./docs/
 REFERENCE.md). To cite this project, you can use the following BibTeX citation.
 ``` @article{bian2021colossal, title={Colossal-AI: A Unified Deep Learning
 System For Large-Scale Parallel Training}, author={Bian, Zhengda and Liu,
 Hongxin and Wang, Boxiang and Huang, Haichen and Li, Yongbin and Wang, Chuanrui
 and Cui, Fan and You, Yang}, journal={arXiv preprint arXiv:2110.14883}, year=
 {2021} } ``` Colossal-AI has been accepted as official tutorial by top
-conferences [SC](https://sc22.supercomputing.org/), [AAAI](https://aaai.org/
-Conferences/AAAI-23/), [PPoPP](https://ppopp23.sigplan.org/), [CVPR](https://
-cvpr2023.thecvf.com/), [ISC](https://www.isc-hpc.com/), etc.
+conferences [NeurIPS](https://nips.cc/), [SC](https://sc22.supercomputing.org/
+), [AAAI](https://aaai.org/Conferences/AAAI-23/), [PPoPP](https://
+ppopp23.sigplan.org/), [CVPR](https://cvpr2023.thecvf.com/), [ISC](https://
+www.isc-hpc.com/), [NVIDIA GTC](https://www.nvidia.com/en-us/on-demand/session/
+gtcspring23-S51482/) ,etc.
                                                                   (back_to_top)
 Platform: UNKNOWN Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Apache Software License Classifier: Environment ::
 GPU :: NVIDIA CUDA Classifier: Topic :: Scientific/Engineering :: Artificial
 Intelligence Classifier: Topic :: System :: Distributed Computing Requires-
 Python: >=3.6 Description-Content-Type: text/markdown
```

### Comparing `colossalai-nightly-2023.7.8/colossalai_nightly.egg-info/SOURCES.txt` & `colossalai-nightly-2023.8.5/colossalai_nightly.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -321,15 +321,14 @@
 colossalai/fx/tracer/meta_patch/patched_module/pooling.py
 colossalai/fx/tracer/meta_patch/patched_module/rnn.py
 colossalai/interface/__init__.py
 colossalai/interface/model.py
 colossalai/interface/optimizer.py
 colossalai/kernel/__init__.py
 colossalai/kernel/cuda_native/__init__.py
-colossalai/kernel/cuda_native/flash_attention.py
 colossalai/kernel/cuda_native/layer_norm.py
 colossalai/kernel/cuda_native/multihead_attention.py
 colossalai/kernel/cuda_native/scaled_softmax.py
 colossalai/kernel/cuda_native/csrc/colossal_C_frontend.cpp
 colossalai/kernel/cuda_native/csrc/compat.h
 colossalai/kernel/cuda_native/csrc/cpu_adam.cpp
 colossalai/kernel/cuda_native/csrc/cpu_adam.h
@@ -368,14 +367,19 @@
 colossalai/kernel/cuda_native/csrc/kernels/include/dropout.h
 colossalai/kernel/cuda_native/csrc/kernels/include/feed_forward.h
 colossalai/kernel/cuda_native/csrc/kernels/include/kernels.h
 colossalai/kernel/cuda_native/csrc/kernels/include/ls_cub.cuh
 colossalai/kernel/cuda_native/csrc/kernels/include/normalize_layer.h
 colossalai/kernel/cuda_native/csrc/kernels/include/softmax.h
 colossalai/kernel/cuda_native/csrc/kernels/include/strided_batch_gemm.h
+colossalai/kernel/cuda_native/mha/__init__.py
+colossalai/kernel/cuda_native/mha/flash_attn_2.py
+colossalai/kernel/cuda_native/mha/mem_eff_attn.py
+colossalai/kernel/cuda_native/mha/mha.py
+colossalai/kernel/cuda_native/mha/utils.py
 colossalai/kernel/jit/__init__.py
 colossalai/kernel/jit/bias_dropout_add.py
 colossalai/kernel/jit/bias_gelu.py
 colossalai/kernel/jit/option.py
 colossalai/kernel/op_builder/__init__.py
 colossalai/kernel/op_builder/builder.py
 colossalai/kernel/op_builder/cpu_adam.py
@@ -577,24 +581,14 @@
 colossalai/utils/cuda.py
 colossalai/utils/memory.py
 colossalai/utils/moe.py
 colossalai/utils/timer.py
 colossalai/utils/checkpoint/__init__.py
 colossalai/utils/checkpoint/module_checkpoint.py
 colossalai/utils/checkpoint/utils.py
-colossalai/utils/checkpoint_io/__init__.py
-colossalai/utils/checkpoint_io/backend.py
-colossalai/utils/checkpoint_io/constant.py
-colossalai/utils/checkpoint_io/convertor.py
-colossalai/utils/checkpoint_io/distributed.py
-colossalai/utils/checkpoint_io/io.py
-colossalai/utils/checkpoint_io/meta.py
-colossalai/utils/checkpoint_io/reader.py
-colossalai/utils/checkpoint_io/utils.py
-colossalai/utils/checkpoint_io/writer.py
 colossalai/utils/data_sampler/__init__.py
 colossalai/utils/data_sampler/base_sampler.py
 colossalai/utils/data_sampler/data_parallel_sampler.py
 colossalai/utils/model/__init__.py
 colossalai/utils/model/utils.py
 colossalai/utils/multi_tensor_apply/__init__.py
 colossalai/utils/multi_tensor_apply/multi_tensor_apply.py
```

### Comparing `colossalai-nightly-2023.7.8/op_builder/__init__.py` & `colossalai-nightly-2023.8.5/op_builder/__init__.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/builder.py` & `colossalai-nightly-2023.8.5/op_builder/builder.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/cpu_adam.py` & `colossalai-nightly-2023.8.5/op_builder/cpu_adam.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/fused_optim.py` & `colossalai-nightly-2023.8.5/op_builder/fused_optim.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/layernorm.py` & `colossalai-nightly-2023.8.5/op_builder/layernorm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/moe.py` & `colossalai-nightly-2023.8.5/op_builder/moe.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/multi_head_attn.py` & `colossalai-nightly-2023.8.5/op_builder/multi_head_attn.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/scaled_masked_softmax.py` & `colossalai-nightly-2023.8.5/op_builder/scaled_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/scaled_upper_triangle_masked_softmax.py` & `colossalai-nightly-2023.8.5/op_builder/scaled_upper_triangle_masked_softmax.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/op_builder/utils.py` & `colossalai-nightly-2023.8.5/op_builder/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/requirements/requirements-test.txt` & `colossalai-nightly-2023.8.5/requirements/requirements-test.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 diffusers
 fbgemm-gpu==0.2.0
 pytest
 coverage==7.2.3
 git+https://github.com/hpcaitech/pytest-testmon
 torchvision
-transformers
+transformers==4.30.2
 timm
 titans
 torchaudio
 torchx-nightly==2022.6.29 # torchrec 0.2.0 requires torchx-nightly. This package is updated every day. We fix the version to a specific date to avoid breaking changes.
 torchrec==0.2.0
 contexttimer
 einops
```

### Comparing `colossalai-nightly-2023.7.8/setup.py` & `colossalai-nightly-2023.8.5/setup.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/albert.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/beit.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/beit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/bert.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/gpt2.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/hanging_param_model.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/hanging_param_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/inline_op_model.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/inline_op_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/nested_model.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/nested_model.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/registry.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/repeated_computed_layers.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/repeated_computed_layers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/resnet.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/resnet.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/simple_net.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/simple_net.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/components_to_test/utils/executor.py` & `colossalai-nightly-2023.8.5/tests/components_to_test/utils/executor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/diffusers/diffusers.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/diffusers/diffusers.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/registry.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/registry.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/timm/timm.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/timm/timm.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchaudio/torchaudio.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchaudio/torchaudio.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchrec/torchrec.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchrec/torchrec.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/torchvision/torchvision.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/torchvision/torchvision.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/albert.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/albert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bert.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/bloom.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/gpt.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/gpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/llama.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/opt.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/kit/model_zoo/transformers/t5.py` & `colossalai-nightly-2023.8.5/tests/kit/model_zoo/transformers/t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_bias_addition.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_bias_addition.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_mod_dir.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_mod_dir.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_nested_ckpt.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_nested_ckpt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_shape_prop.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_shape_prop.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/test_symbolic_profile.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/test_symbolic_profile.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_fx/zoo.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_fx/zoo.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_aten.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/test_aten.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_flop_tensor.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/test_flop_tensor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_analyzer/test_subclasses/test_meta_mode.py` & `colossalai-nightly-2023.8.5/tests/test_analyzer/test_subclasses/test_meta_mode.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_node_converting_pass.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_pass/test_node_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_pass/test_size_value_converting_pass.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_bias_addition_forward.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_broadcast.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_ddp.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_compatibility_with_gemini.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_find_repeat_block.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_runtime_with_gpt_modules.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_gpt/test_solver_with_gpt_module.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_liveness_analysis.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addbmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_addmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_batch_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_function_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bias_linear_module_node.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_binary_elementwise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_bmm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_conv_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_default_reshape_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_embedding_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getattr_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_getitem_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_layer_norm_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_linear_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_matmul_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_norm_pooling_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_output_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_permute_and_transpose_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_placeholder_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_shard_option.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_softmax_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_split_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_sum_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_tensor_constructor.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_unary_element_wise_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_view_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/test_where_handler.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_node_handler/utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py` & `colossalai-nightly-2023.8.5/tests/test_auto_parallel/test_tensor_shard/test_solver_with_resnet_v2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/_utils.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/_utils.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bert.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_bert.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_bloom.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_bloom.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_gpt2.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_gpt2.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_llama.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_llama.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_opt.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_opt.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_t5.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_t5.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_model/test_shard_vit.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_model/test_shard_vit.py`

 * *Files identical despite different names*

### Comparing `colossalai-nightly-2023.7.8/tests/test_shardformer/test_with_torch_ddp.py` & `colossalai-nightly-2023.8.5/tests/test_shardformer/test_with_torch_ddp.py`

 * *Files identical despite different names*

