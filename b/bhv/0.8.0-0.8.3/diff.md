# Comparing `tmp/bhv-0.8.0.tar.gz` & `tmp/bhv-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.8.0.tar", last modified: Tue Aug  1 14:31:08 2023, max compression
+gzip compressed data, was "bhv-0.8.3.tar", last modified: Fri Aug  4 23:11:29 2023, max compression
```

## Comparing `bhv-0.8.0.tar` & `bhv-0.8.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.800197 bhv-0.8.0/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       47 2023-05-13 14:44:39.000000 bhv-0.8.0/.gitignore
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.8.0/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)       50 2023-06-25 20:42:11.000000 bhv-0.8.0/MANIFEST.in
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-08-01 14:31:08.800197 bhv-0.8.0/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6987 2023-07-27 10:41:19.000000 bhv-0.8.0/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.783529 bhv-0.8.0/benchmarks/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2158 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/exact_synthesis.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1879 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/layerwise_random_execution.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1829 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/lookup.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1307 2023-07-27 10:41:19.000000 bhv-0.8.0/benchmarks/majority.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2635 2023-06-25 20:42:11.000000 bhv-0.8.0/benchmarks/random_network.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.786863 bhv-0.8.0/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.8.0/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    17267 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/abstract.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.790196 bhv-0.8.0/bhv/cnative/
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.790196 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/
--rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512-config.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    18986 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2183 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-SnP.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.inc
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2406 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/align.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/brg_endian.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/config.h
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.793530 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    22154 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-64.macros
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2383 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-SnP.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64-config.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    19024 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9730 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-unrolling.macros
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.inc
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6272 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/SnP-Relaned.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2408 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/align.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/brg_endian.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/config.h
--rwxr-xr-x   0 adamv     (1000) adamv     (1000)  1202008 2023-08-01 13:51:25.000000 bhv-0.8.0/bhv/cnative/a.out
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35552 2023-08-01 14:05:51.000000 bhv-0.8.0/bhv/cnative/benchmark.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)    14176 2023-08-01 14:12:36.000000 bhv-0.8.0/bhv/cnative/bindings.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2708 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/core.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    10024 2023-07-31 19:36:17.000000 bhv-0.8.0/bhv/cnative/distance.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)      124 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/hash.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     7813 2023-08-01 11:07:04.000000 bhv-0.8.0/bhv/cnative/majority.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6296 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/permutation.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2267 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/plain_test.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)     9955 2023-07-31 19:36:17.000000 bhv-0.8.0/bhv/cnative/random.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)   107227 2023-07-28 00:14:59.000000 bhv-0.8.0/bhv/cnative/random_experiments.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1428 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/representative.h
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.793530 bhv-0.8.0/bhv/cnative/results/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15710 2023-07-27 15:32:26.000000 bhv-0.8.0/bhv/cnative/results/2-4Mop-128Wavefront-DualScalar.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    16196 2023-07-27 12:26:54.000000 bhv-0.8.0/bhv/cnative/results/2-8Mop-DualScalar.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15728 2023-07-27 15:07:54.000000 bhv-0.8.0/bhv/cnative/results/4-Bit-Unified-Wavefront-AVX-512.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15735 2023-07-27 15:26:42.000000 bhv-0.8.0/bhv/cnative/results/4Mop-256Wavefront-AVX.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15721 2023-07-27 15:22:28.000000 bhv-0.8.0/bhv/cnative/results/4Mop-512-Wavefront.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15726 2023-07-27 15:13:50.000000 bhv-0.8.0/bhv/cnative/results/4Mop.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    16198 2023-07-27 12:19:02.000000 bhv-0.8.0/bhv/cnative/results/8-Bit-Unified-Wavefront-AVX-512.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15311 2023-07-27 15:37:51.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Parsimonious-Scalar.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15712 2023-07-27 19:46:41.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-AVX-512.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15695 2023-07-27 15:44:08.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-AVX2.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15339 2023-07-27 15:39:40.000000 bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-Scalar.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    31555 2023-08-01 14:04:19.000000 bhv-0.8.0/bhv/cnative/results/all_avx2.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15799 2023-07-27 15:07:32.000000 bhv-0.8.0/bhv/cnative/results/negative_tree_avx512.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    16189 2023-07-27 13:48:36.000000 bhv-0.8.0/bhv/cnative/results/sparse_tree.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    15775 2023-07-28 00:02:07.000000 bhv-0.8.0/bhv/cnative/results/ternary_tree.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)    39644 2023-07-27 15:49:27.000000 bhv-0.8.0/bhv/cnative/results.zip
--rwxr-xr-x   0 adamv     (1000) adamv     (1000)      255 2023-08-01 14:05:16.000000 bhv-0.8.0/bhv/cnative/run.sh
--rw-r--r--   0 adamv     (1000) adamv     (1000)      396 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/shared.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8457 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/cnative/simdpcg.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)    46933 2023-08-01 11:05:34.000000 bhv-0.8.0/bhv/cnative/ternary.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     5189 2023-07-28 01:18:44.000000 bhv-0.8.0/bhv/cnative/testing.cpp
--rw-r--r--   0 adamv     (1000) adamv     (1000)    38396 2023-08-01 14:05:51.000000 bhv-0.8.0/bhv/cnative/threshold.h
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.8.0/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     4208 2023-06-25 20:42:11.000000 bhv-0.8.0/bhv/lookup.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2608 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/native.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    13110 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-05-27 17:35:51.000000 bhv-0.8.0/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.8.0/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8455 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3588 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.8.0/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    27835 2023-07-28 01:18:57.000000 bhv-0.8.0/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.8.0/bhv/unification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3839 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     6602 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/variants.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2069 2023-07-27 10:41:19.000000 bhv-0.8.0/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.786863 bhv-0.8.0/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3478 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       44 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-08-01 14:31:08.000000 bhv-0.8.0/bhv.egg-info/top_level.txt
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.796863 bhv-0.8.0/examples/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    23765 2023-05-14 01:00:15.000000 bhv-0.8.0/examples/Kanerva09.ipynb
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11380 2023-05-14 01:00:15.000000 bhv-0.8.0/examples/Metric_Picker.ipynb
--rw-r--r--   0 adamv     (1000) adamv     (1000)      903 2023-07-11 12:00:53.000000 bhv-0.8.0/examples/ca_rules.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1843 2023-05-13 14:46:42.000000 bhv-0.8.0/examples/grandmother_example.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    13478 2023-05-13 15:07:15.000000 bhv-0.8.0/examples/kanerva09.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      389 2023-07-27 10:41:19.000000 bhv-0.8.0/examples/majority_classification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2414 2023-07-27 10:41:19.000000 bhv-0.8.0/examples/reasoning_by_analogy_adiabatic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2726 2023-07-27 10:41:19.000000 bhv-0.8.0/examples/reasoning_by_analogy_linear.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1169 2023-05-13 15:04:14.000000 bhv-0.8.0/examples/state_machine.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      294 2023-05-13 15:04:14.000000 bhv-0.8.0/examples/viz_distances.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      686 2023-05-13 15:07:15.000000 bhv-0.8.0/examples/winnow_classification.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-08-01 14:31:08.800197 bhv-0.8.0/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2050 2023-08-01 14:27:17.000000 bhv-0.8.0/setup.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-01 14:31:08.796863 bhv-0.8.0/tests/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3196 2023-05-15 19:48:48.000000 bhv-0.8.0/tests/blocklsynth.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3981 2023-06-25 20:42:11.000000 bhv-0.8.0/tests/composites.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      837 2023-04-11 14:49:00.000000 bhv-0.8.0/tests/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3037 2023-06-12 22:49:54.000000 bhv-0.8.0/tests/fiestal.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1193 2023-07-27 10:41:19.000000 bhv-0.8.0/tests/inspect_random.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    13700 2023-07-27 10:41:19.000000 bhv-0.8.0/tests/laws.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1253 2023-06-28 14:28:44.000000 bhv-0.8.0/tests/lsynthesis.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1437 2023-06-26 20:59:59.000000 bhv-0.8.0/tests/marshalling.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      332 2023-06-12 22:49:54.000000 bhv-0.8.0/tests/metrics.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      913 2023-08-01 11:05:34.000000 bhv-0.8.0/tests/native_test.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      835 2023-05-23 15:42:03.000000 bhv-0.8.0/tests/reconstruct_program.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      998 2023-07-28 01:19:06.000000 bhv-0.8.0/tests/sym.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     7032 2023-05-23 17:58:09.000000 bhv-0.8.0/tests/sym_laws.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      715 2023-06-25 20:42:11.000000 bhv-0.8.0/tests/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      927 2023-03-28 11:00:31.000000 bhv-0.8.0/tests/test_pytorch.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.413800 bhv-0.8.3/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       47 2023-05-13 14:44:39.000000 bhv-0.8.3/.gitignore
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.8.3/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       50 2023-06-25 20:42:11.000000 bhv-0.8.3/MANIFEST.in
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-08-04 23:11:29.410466 bhv-0.8.3/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6987 2023-07-27 10:41:19.000000 bhv-0.8.3/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.393798 bhv-0.8.3/benchmarks/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2158 2023-06-25 20:42:11.000000 bhv-0.8.3/benchmarks/exact_synthesis.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2390 2023-08-04 17:43:45.000000 bhv-0.8.3/benchmarks/layerwise_random_execution.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1829 2023-06-25 20:42:11.000000 bhv-0.8.3/benchmarks/lookup.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1307 2023-07-27 10:41:19.000000 bhv-0.8.3/benchmarks/majority.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2635 2023-06-25 20:42:11.000000 bhv-0.8.3/benchmarks/random_network.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.393798 bhv-0.8.3/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.8.3/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    17267 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/abstract.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.400466 bhv-0.8.3/bhv/cnative/
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.403799 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512-config.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    18986 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2183 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-SnP.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.inc
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2406 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/align.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/brg_endian.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/config.h
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.403799 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    22154 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-64.macros
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2383 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-SnP.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      186 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64-config.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    19024 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9730 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-unrolling.macros
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2537 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakSponge.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2811 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakSponge.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11249 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakSponge.inc
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6272 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/SnP-Relaned.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2408 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1673 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      873 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/align.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     5638 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/brg_endian.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      136 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/config.h
+-rwxr-xr-x   0 adamv     (1000) adamv     (1000)  1202008 2023-08-01 13:51:25.000000 bhv-0.8.3/bhv/cnative/a.out
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35552 2023-08-01 14:05:51.000000 bhv-0.8.3/bhv/cnative/benchmark.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15048 2023-08-04 15:59:28.000000 bhv-0.8.3/bhv/cnative/bindings.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2708 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/core.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    10024 2023-07-31 19:36:17.000000 bhv-0.8.3/bhv/cnative/distance.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      124 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/hash.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     7813 2023-08-01 11:07:04.000000 bhv-0.8.3/bhv/cnative/majority.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6296 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/cnative/permutation.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2267 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/plain_test.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     9955 2023-07-31 19:36:17.000000 bhv-0.8.3/bhv/cnative/random.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)   107227 2023-07-28 00:14:59.000000 bhv-0.8.3/bhv/cnative/random_experiments.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1428 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/cnative/representative.h
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.407132 bhv-0.8.3/bhv/cnative/results/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15710 2023-07-27 15:32:26.000000 bhv-0.8.3/bhv/cnative/results/2-4Mop-128Wavefront-DualScalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    16196 2023-07-27 12:26:54.000000 bhv-0.8.3/bhv/cnative/results/2-8Mop-DualScalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15728 2023-07-27 15:07:54.000000 bhv-0.8.3/bhv/cnative/results/4-Bit-Unified-Wavefront-AVX-512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15735 2023-07-27 15:26:42.000000 bhv-0.8.3/bhv/cnative/results/4Mop-256Wavefront-AVX.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15721 2023-07-27 15:22:28.000000 bhv-0.8.3/bhv/cnative/results/4Mop-512-Wavefront.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15726 2023-07-27 15:13:50.000000 bhv-0.8.3/bhv/cnative/results/4Mop.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    16198 2023-07-27 12:19:02.000000 bhv-0.8.3/bhv/cnative/results/8-Bit-Unified-Wavefront-AVX-512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15311 2023-07-27 15:37:51.000000 bhv-0.8.3/bhv/cnative/results/Single-Bit-Parsimonious-Scalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15712 2023-07-27 19:46:41.000000 bhv-0.8.3/bhv/cnative/results/Single-Bit-Single-Buffer-AVX-512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15695 2023-07-27 15:44:08.000000 bhv-0.8.3/bhv/cnative/results/Single-Bit-Single-Buffer-AVX2.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15339 2023-07-27 15:39:40.000000 bhv-0.8.3/bhv/cnative/results/Single-Bit-Single-Buffer-Scalar.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    31555 2023-08-01 14:04:19.000000 bhv-0.8.3/bhv/cnative/results/all_avx2.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15799 2023-07-27 15:07:32.000000 bhv-0.8.3/bhv/cnative/results/negative_tree_avx512.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    16189 2023-07-27 13:48:36.000000 bhv-0.8.3/bhv/cnative/results/sparse_tree.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    15775 2023-07-28 00:02:07.000000 bhv-0.8.3/bhv/cnative/results/ternary_tree.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    39644 2023-07-27 15:49:27.000000 bhv-0.8.3/bhv/cnative/results.zip
+-rwxr-xr-x   0 adamv     (1000) adamv     (1000)      255 2023-08-01 14:05:16.000000 bhv-0.8.3/bhv/cnative/run.sh
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      396 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/cnative/shared.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8457 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/cnative/simdpcg.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    46933 2023-08-01 11:05:34.000000 bhv-0.8.3/bhv/cnative/ternary.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     5189 2023-07-28 01:18:44.000000 bhv-0.8.3/bhv/cnative/testing.cpp
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    38396 2023-08-01 14:05:51.000000 bhv-0.8.3/bhv/cnative/threshold.h
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.8.3/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     4208 2023-06-25 20:42:11.000000 bhv-0.8.3/bhv/lookup.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2995 2023-08-04 17:43:04.000000 bhv-0.8.3/bhv/native.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13110 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-05-27 17:35:51.000000 bhv-0.8.3/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.8.3/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8455 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3588 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.8.3/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    27835 2023-07-28 01:18:57.000000 bhv-0.8.3/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.8.3/bhv/unification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3839 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     6602 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/variants.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2069 2023-07-27 10:41:19.000000 bhv-0.8.3/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.397132 bhv-0.8.3/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1054 2023-08-04 23:11:29.000000 bhv-0.8.3/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3478 2023-08-04 23:11:29.000000 bhv-0.8.3/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-08-04 23:11:29.000000 bhv-0.8.3/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       44 2023-08-04 23:11:29.000000 bhv-0.8.3/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-08-04 23:11:29.000000 bhv-0.8.3/bhv.egg-info/top_level.txt
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.407132 bhv-0.8.3/examples/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    23765 2023-05-14 01:00:15.000000 bhv-0.8.3/examples/Kanerva09.ipynb
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11380 2023-05-14 01:00:15.000000 bhv-0.8.3/examples/Metric_Picker.ipynb
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      903 2023-07-11 12:00:53.000000 bhv-0.8.3/examples/ca_rules.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1843 2023-05-13 14:46:42.000000 bhv-0.8.3/examples/grandmother_example.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13478 2023-05-13 15:07:15.000000 bhv-0.8.3/examples/kanerva09.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      389 2023-07-27 10:41:19.000000 bhv-0.8.3/examples/majority_classification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2414 2023-07-27 10:41:19.000000 bhv-0.8.3/examples/reasoning_by_analogy_adiabatic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2726 2023-07-27 10:41:19.000000 bhv-0.8.3/examples/reasoning_by_analogy_linear.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1169 2023-05-13 15:04:14.000000 bhv-0.8.3/examples/state_machine.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      294 2023-05-13 15:04:14.000000 bhv-0.8.3/examples/viz_distances.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      686 2023-05-13 15:07:15.000000 bhv-0.8.3/examples/winnow_classification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-08-04 23:11:29.413800 bhv-0.8.3/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2050 2023-08-04 15:49:05.000000 bhv-0.8.3/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-08-04 23:11:29.410466 bhv-0.8.3/tests/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3196 2023-05-15 19:48:48.000000 bhv-0.8.3/tests/blocklsynth.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3981 2023-06-25 20:42:11.000000 bhv-0.8.3/tests/composites.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      837 2023-04-11 14:49:00.000000 bhv-0.8.3/tests/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3037 2023-06-12 22:49:54.000000 bhv-0.8.3/tests/fiestal.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1193 2023-07-27 10:41:19.000000 bhv-0.8.3/tests/inspect_random.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    13700 2023-07-27 10:41:19.000000 bhv-0.8.3/tests/laws.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1253 2023-06-28 14:28:44.000000 bhv-0.8.3/tests/lsynthesis.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1437 2023-06-26 20:59:59.000000 bhv-0.8.3/tests/marshalling.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      332 2023-06-12 22:49:54.000000 bhv-0.8.3/tests/metrics.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      913 2023-08-01 11:05:34.000000 bhv-0.8.3/tests/native_test.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      835 2023-05-23 15:42:03.000000 bhv-0.8.3/tests/reconstruct_program.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      998 2023-07-28 01:19:06.000000 bhv-0.8.3/tests/sym.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     7032 2023-05-23 17:58:09.000000 bhv-0.8.3/tests/sym_laws.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      715 2023-06-25 20:42:11.000000 bhv-0.8.3/tests/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      927 2023-03-28 11:00:31.000000 bhv-0.8.3/tests/test_pytorch.py
```

### Comparing `bhv-0.8.0/LICENSE` & `bhv-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/PKG-INFO` & `bhv-0.8.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.8.0
+Version: 0.8.3
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bhv-0.8.0/README.md` & `bhv-0.8.3/README.md`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/benchmarks/exact_synthesis.py` & `bhv-0.8.3/benchmarks/exact_synthesis.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/benchmarks/layerwise_random_execution.py` & `bhv-0.8.3/benchmarks/layerwise_random_execution.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 # N-input M-output stack of random computation (from different families)
 # NOTE: can fail due to tight bounds on the probabilistic properties, run multiple times
 # from bhv.np import NumPyPacked64BHV as BHV
-from bhv.native import CNativePackedBHV as BHV
+from bhv.native import NativePackedBHV as BHV
 
 from time import monotonic
 from random import shuffle, random, randrange, sample
 from statistics import pstdev, fmean
 from multiprocessing import Pool
 
 
 repeat_pipeline = 3
 
-I = 50
-O = 50
-sizes = [2000]*20 + [O]
-vat_type: '"MAJ3" | "XOR NOT", "SELECT EQ"' = "MAJ3"
+I = 500
+O = 500
+sizes = [10000]*100 + [O]
+vat_type: '"MAJ3" | "XOR NOT" | "SELECT EQ" | "TERNARY"' = "MAJ3"
 
 
 if vat_type == "MAJ3":
     def execute(_):
         i, j, k = sample(values[-1], k=3)
         return BHV.majority([
                 i if random() < 2/3 else ~i,
@@ -38,15 +38,20 @@
         r = random()
         if r < 1/3:
             i, j, k = sample(values[-1], k=3)
             return BHV.select(i, j, k)
         else:
             i, j = sample(values[-1], k=2)
             return ~(i ^ j)
-
+elif vat_type == "TERNARY":
+    OPS = [15, 23, 27, 29, 30, 39, 43, 45, 46, 51, 53, 54, 57, 58, 60, 71, 75, 77, 78, 83, 85, 86, 89, 90, 92, 99, 101, 102, 105, 106, 108, 113, 114, 116, 120, 135, 139, 141, 142, 147, 149, 150, 153, 154, 156, 163, 165, 166, 169, 170, 172, 177, 178, 180, 184, 195, 197, 198, 201, 202, 204, 209, 210, 212, 216, 225, 226, 228, 232, 240]
+    def execute(_):
+        op, = sample(OPS, k=1)
+        i, j, k = sample(values[-1], k=3)
+        return BHV.ternary(i, j, k, op)
 
 execution_times = []
 
 for _ in range(repeat_pipeline):
     t_exec = monotonic()
 
     value = [BHV.rand() for _ in range(I)]
```

### Comparing `bhv-0.8.0/benchmarks/lookup.py` & `bhv-0.8.3/benchmarks/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/benchmarks/majority.py` & `bhv-0.8.3/benchmarks/majority.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/benchmarks/random_network.py` & `bhv-0.8.3/benchmarks/random_network.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/abstract.py` & `bhv-0.8.3/bhv/abstract.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512.cpp` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-AVX512.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-SnP.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakP-1600-SnP.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.cpp` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.inc` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/KeccakSponge.inc`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.cpp` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/TurboSHAKE.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/align.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/align.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_AVX512/brg_endian.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_AVX512/brg_endian.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-64.macros` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-64.macros`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-SnP.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-SnP.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-unrolling.macros` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakP-1600-unrolling.macros`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.cpp` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakSponge.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakSponge.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/KeccakSponge.inc` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/KeccakSponge.inc`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/SnP-Relaned.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/SnP-Relaned.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/TurboSHAKE.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/align.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/align.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/TurboSHAKE_opt/brg_endian.h` & `bhv-0.8.3/bhv/cnative/TurboSHAKE_opt/brg_endian.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/a.out` & `bhv-0.8.3/bhv/cnative/a.out`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/benchmark.cpp` & `bhv-0.8.3/bhv/cnative/benchmark.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/bindings.cpp` & `bhv-0.8.3/bhv/cnative/bindings.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -70,21 +70,21 @@
 static PyObject *BHV_and(PyObject * v1, PyObject * v2);
 static PyObject *BHV_or(PyObject * v1, PyObject * v2);
 static PyObject *BHV_invert(PyObject * v);
 
 static PyObject *BHV_hamming(BHV * v1, PyObject * args);
 
 static PyObject *BHV_to_bytes(BHV * x, PyObject * Py_UNUSED(ignored));
-
 static PyObject *BHV_from_bytes(PyTypeObject *type, PyObject *args);
 
+static PyObject *__getstate__(BHV *x, PyObject *Py_UNUSED(ignored));
+static PyObject *__setstate__(BHV *x, PyObject *args);
+
 static PyObject *BHV_active(BHV * v, PyObject * Py_UNUSED(ignored)) {
-return Py_BuildValue("i",
-bhv::active(v
-->data));
+    return Py_BuildValue("i", bhv::active(v->data));
 }
 
 static PyMemberDef BHV_members[] = {
         {nullptr}
 };
 
 static PyMethodDef BHV_methods[] = {
@@ -120,27 +120,31 @@
                 "Hamming distance between two BHVs"},
         {"active",            (PyCFunction) BHV_active,            METH_NOARGS,
                 "Count the number of active bits"},
         {"to_bytes",          (PyCFunction) BHV_to_bytes,          METH_NOARGS,
                 "Bytes normalized form"},
         {"from_bytes",        (PyCFunction) BHV_from_bytes,        METH_CLASS | METH_VARARGS,
                 "Construct from bytes normalized form"},
+        {"__getstate__",      (PyCFunction) __getstate__,          METH_NOARGS,
+                "Pickle the vector"},
+        {"__setstate__",      (PyCFunction) __setstate__,          METH_VARARGS,
+                "Un-pickle the vector"},
         {nullptr}
 };
 
 static PyNumberMethods BHV_nb_methods = {
         .nb_invert = (unaryfunc) BHV_invert,
         .nb_and = (binaryfunc) BHV_and,
         .nb_xor = (binaryfunc) BHV_xor,
         .nb_or = (binaryfunc) BHV_or,
 };
 
 static PyTypeObject BHVType = {
         .ob_base = PyVarObject_HEAD_INIT(nullptr, 0)
-        .tp_name = "bhv.CNativePackedBHV",
+        .tp_name = "bhv.cnative.CNativePackedBHV",
         .tp_basicsize = sizeof(BHV),
         .tp_itemsize = 0,
         .tp_dealloc = (destructor) BHV_dealloc,
         .tp_as_number = &BHV_nb_methods,
         .tp_flags = Py_TPFLAGS_DEFAULT | Py_TPFLAGS_BASETYPE,
         .tp_doc = "Packed, native implementation of Boolean Hypervectors",
         .tp_richcompare = BHV_richcompare,
@@ -289,15 +293,15 @@
 }
 
 static PyObject *BHV_ternary(BHV * x, PyObject * args) {
     BHV * y;
     BHV * z;
     uint8_t op;
 
-    if (!PyArg_ParseTuple(args, "O!O!i", &BHVType, &y, &BHVType, &z, &op))
+    if (!PyArg_ParseTuple(args, "O!O!b", &BHVType, &y, &BHVType, &z, &op))
         return nullptr;
 
     PyObject * ret = BHV_new(&BHVType, nullptr, nullptr);
     bhv::dynamic_ternary_into(x->data, y->data, z->data, ((BHV *) ret)->data, op);
     return ret;
 }
 
@@ -384,14 +388,34 @@
         return nullptr;
     }
 
     memcpy(((BHV *) ret)->data, buf, BYTES);
     return ret;
 }
 
+static PyObject *__getstate__(BHV *x, PyObject *Py_UNUSED(ignored)) {
+    return PyBytes_FromStringAndSize((char*)x->data, BYTES);
+}
+
+static PyObject *__setstate__(BHV *x, PyObject *args) {
+    char *buf;
+    size_t size;
+
+    if (!PyArg_ParseTuple(args, "s#", &buf, &size))
+        return nullptr;
+
+    if (size != BYTES) {
+        PyErr_SetString(PyExc_TypeError, "Bytes object didn't have the right size");
+        return nullptr;
+    }
+
+    memcpy(x->data, buf, BYTES);
+    Py_RETURN_NONE;
+}
+
 static PyObject *dimension(PyObject * self, PyObject * args, PyObject * kwds) {
     return PyLong_FromLong(BITS);
 }
 
 
 static PyMethodDef module_methods[] = {
         {"_DIMENSION", (PyCFunction) dimension, METH_NOARGS,
```

### Comparing `bhv-0.8.0/bhv/cnative/core.h` & `bhv-0.8.3/bhv/cnative/core.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/distance.h` & `bhv-0.8.3/bhv/cnative/distance.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/majority.h` & `bhv-0.8.3/bhv/cnative/majority.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/permutation.h` & `bhv-0.8.3/bhv/cnative/permutation.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/plain_test.cpp` & `bhv-0.8.3/bhv/cnative/plain_test.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/random.h` & `bhv-0.8.3/bhv/cnative/random.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/random_experiments.h` & `bhv-0.8.3/bhv/cnative/random_experiments.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/representative.h` & `bhv-0.8.3/bhv/cnative/representative.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/2-4Mop-128Wavefront-DualScalar.txt` & `bhv-0.8.3/bhv/cnative/results/2-4Mop-128Wavefront-DualScalar.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/2-8Mop-DualScalar.txt` & `bhv-0.8.3/bhv/cnative/results/2-8Mop-DualScalar.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/4-Bit-Unified-Wavefront-AVX-512.txt` & `bhv-0.8.3/bhv/cnative/results/4-Bit-Unified-Wavefront-AVX-512.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/4Mop-256Wavefront-AVX.txt` & `bhv-0.8.3/bhv/cnative/results/4Mop-256Wavefront-AVX.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/4Mop-512-Wavefront.txt` & `bhv-0.8.3/bhv/cnative/results/4Mop-512-Wavefront.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/4Mop.txt` & `bhv-0.8.3/bhv/cnative/results/4Mop.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/8-Bit-Unified-Wavefront-AVX-512.txt` & `bhv-0.8.3/bhv/cnative/results/8-Bit-Unified-Wavefront-AVX-512.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/Single-Bit-Parsimonious-Scalar.txt` & `bhv-0.8.3/bhv/cnative/results/Single-Bit-Parsimonious-Scalar.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-AVX-512.txt` & `bhv-0.8.3/bhv/cnative/results/Single-Bit-Single-Buffer-AVX-512.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-AVX2.txt` & `bhv-0.8.3/bhv/cnative/results/Single-Bit-Single-Buffer-AVX2.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/Single-Bit-Single-Buffer-Scalar.txt` & `bhv-0.8.3/bhv/cnative/results/Single-Bit-Single-Buffer-Scalar.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/all_avx2.txt` & `bhv-0.8.3/bhv/cnative/results/all_avx2.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/negative_tree_avx512.txt` & `bhv-0.8.3/bhv/cnative/results/negative_tree_avx512.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/sparse_tree.txt` & `bhv-0.8.3/bhv/cnative/results/sparse_tree.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results/ternary_tree.txt` & `bhv-0.8.3/bhv/cnative/results/ternary_tree.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/results.zip` & `bhv-0.8.3/bhv/cnative/results.zip`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/simdpcg.h` & `bhv-0.8.3/bhv/cnative/simdpcg.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/ternary.h` & `bhv-0.8.3/bhv/cnative/ternary.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/testing.cpp` & `bhv-0.8.3/bhv/cnative/testing.cpp`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/cnative/threshold.h` & `bhv-0.8.3/bhv/cnative/threshold.h`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/embedding.py` & `bhv-0.8.3/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/lookup.py` & `bhv-0.8.3/bhv/lookup.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/native.py` & `bhv-0.8.3/bhv/native.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,25 @@
 
     def __invert__(self):
         return NativePackedBHV(~self.ins)
 
     def select(self, when1, when0):
         return NativePackedBHV(self.ins.select(when1.ins, when0.ins))
 
+    def ternary(self, y, z, op):
+        return NativePackedBHV(self.ins.ternary(y.ins, z.ins, op))
+
     @classmethod
     def majority(cls, xs):
         return NativePackedBHV(CNativePackedBHV.majority([x.ins for x in xs]))
 
+    @classmethod
+    def representative(cls, xs):
+        return NativePackedBHV(CNativePackedBHV.representative([x.ins for x in xs]))
+
     def active(self):
         return self.ins.active()
 
     def hamming(self, other):
         return self.ins.hamming(other.ins)
 
     def permute_words(self, permutation_id: int):
@@ -76,11 +83,17 @@
     @classmethod
     def from_bytes(cls, bs):
         return NativePackedBHV(CNativePackedBHV.from_bytes(bs))
 
     def to_bytes(self):
         return self.ins.to_bytes()
 
+    def __getstate__(self):
+        return self.to_bytes()
+
+    def __setstate__(self, state):
+        self.ins = CNativePackedBHV.from_bytes(state)
+
 NativePackedBHV.ZERO = NativePackedBHV(CNativePackedBHV.ZERO)
 NativePackedBHV.ONE = NativePackedBHV(CNativePackedBHV.ONE)
 NativePackedBHV.HALF = NativePackedBHV(CNativePackedBHV.HALF)
 NativePackedBHV._FEISTAL_SUBKEYS = NativePackedBHV.nrand2(NativePackedBHV._FEISTAL_ROUNDS, 4)
```

### Comparing `bhv-0.8.0/bhv/np.py` & `bhv-0.8.3/bhv/np.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/poibin.py` & `bhv-0.8.3/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/positions.py` & `bhv-0.8.3/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/pytorch.py` & `bhv-0.8.3/bhv/pytorch.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/shared.py` & `bhv-0.8.3/bhv/shared.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/slice.py` & `bhv-0.8.3/bhv/slice.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/symbolic.py` & `bhv-0.8.3/bhv/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/unification.py` & `bhv-0.8.3/bhv/unification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/vanilla.py` & `bhv-0.8.3/bhv/vanilla.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/variants.py` & `bhv-0.8.3/bhv/variants.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv/visualization.py` & `bhv-0.8.3/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/bhv.egg-info/PKG-INFO` & `bhv-0.8.3/bhv.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.8.0
+Version: 0.8.3
 Summary: Boolean Hypervectors
 Home-page: https://github.com/Adam-Vandervorst/PyBHV
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bhv-0.8.0/bhv.egg-info/SOURCES.txt` & `bhv-0.8.3/bhv.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/Kanerva09.ipynb` & `bhv-0.8.3/examples/Kanerva09.ipynb`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/Metric_Picker.ipynb` & `bhv-0.8.3/examples/Metric_Picker.ipynb`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/ca_rules.py` & `bhv-0.8.3/examples/ca_rules.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/grandmother_example.py` & `bhv-0.8.3/examples/grandmother_example.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/kanerva09.py` & `bhv-0.8.3/examples/kanerva09.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/reasoning_by_analogy_adiabatic.py` & `bhv-0.8.3/examples/reasoning_by_analogy_adiabatic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/reasoning_by_analogy_linear.py` & `bhv-0.8.3/examples/reasoning_by_analogy_linear.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/state_machine.py` & `bhv-0.8.3/examples/state_machine.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/examples/winnow_classification.py` & `bhv-0.8.3/examples/winnow_classification.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/setup.py` & `bhv-0.8.3/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages, Extension
 
-VERSION = '0.8.0'
+VERSION = '0.8.3'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 native = Extension("bhv.cnative",
                    sources=['bhv/cnative/bindings.cpp',
                             'bhv/cnative/TurboSHAKE_opt/TurboSHAKE.cpp',
                             'bhv/cnative/TurboSHAKE_opt/KeccakP-1600-opt64.cpp',
```

### Comparing `bhv-0.8.0/tests/blocklsynth.py` & `bhv-0.8.3/tests/blocklsynth.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/composites.py` & `bhv-0.8.3/tests/composites.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/embedding.py` & `bhv-0.8.3/tests/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/fiestal.py` & `bhv-0.8.3/tests/fiestal.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/inspect_random.py` & `bhv-0.8.3/tests/inspect_random.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/laws.py` & `bhv-0.8.3/tests/laws.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/lsynthesis.py` & `bhv-0.8.3/tests/lsynthesis.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/marshalling.py` & `bhv-0.8.3/tests/marshalling.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/native_test.py` & `bhv-0.8.3/tests/native_test.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/reconstruct_program.py` & `bhv-0.8.3/tests/reconstruct_program.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/sym.py` & `bhv-0.8.3/tests/sym.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/sym_laws.py` & `bhv-0.8.3/tests/sym_laws.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/symbolic.py` & `bhv-0.8.3/tests/symbolic.py`

 * *Files identical despite different names*

### Comparing `bhv-0.8.0/tests/test_pytorch.py` & `bhv-0.8.3/tests/test_pytorch.py`

 * *Files identical despite different names*

