# Comparing `tmp/chiapos-2.0.0b5.tar.gz` & `tmp/chiapos-2.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chiapos-2.0.0b5.tar", last modified: Mon Jul 17 20:54:14 2023, max compression
+gzip compressed data, was "chiapos-2.0.0rc1.tar", last modified: Sat Jul 22 05:12:56 2023, max compression
```

## Comparing `chiapos-2.0.0b5.tar` & `chiapos-2.0.0rc1.tar`

### file list

```diff
@@ -1,190 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.348793 chiapos-2.0.0b5/
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.clang-format
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.284793 chiapos-2.0.0b5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.296793 chiapos-2.0.0b5/.github/actions/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2491 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/actions/fetch_bladebit_harvester.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.300793 chiapos-2.0.0b5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/build-test-cplusplus.yml
--rw-r--r--   0 runner    (1001) docker     (123)    10236 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/build-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/doc-html-pdf.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/manual-plot.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/plot-k27-no-bitfield.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/plot-k27.yaml
--rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.github/workflows/stale-issue.yml
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/CMakeLists.txt
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-17 20:54:14.348793 chiapos-2.0.0b5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.300793 chiapos-2.0.0b5/chiapos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-07-17 20:54:14.000000 chiapos-2.0.0b5/chiapos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-17 20:54:14.000000 chiapos-2.0.0b5/chiapos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:54:14.000000 chiapos-2.0.0b5/chiapos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 20:54:13.000000 chiapos-2.0.0b5/chiapos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-17 20:54:14.000000 chiapos-2.0.0b5/chiapos.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/docker-build.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/docker-test.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.304793 chiapos-2.0.0b5/documents/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/bucket_graph.pdf
--rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/code_documentation.pdf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.304793 chiapos-2.0.0b5/documents/images/
--rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/images/aesctr.png
--rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/images/beyondhellman.png
--rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/images/beyondhellman2.png
--rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/images/pointerformat.png
--rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/images/proofofspace.png
--rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/proof_of_space.html
--rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/documents/proof_of_space.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.312793 chiapos-2.0.0b5/hellman_example/
--rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/Hellman attacks.pdf
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/aes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/cxxopts.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/hellman.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/sort_on_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/hellman_example/verifier.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lgtm.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.288793 chiapos-2.0.0b5/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.312793 chiapos-2.0.0b5/lib/FiniteStateEntropy/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.288793 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.312793 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.312793 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE/
--rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
--rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.316793 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.316793 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/libfse/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
--rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
--rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.324793 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.324793 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/Archives/
--rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/Archives/hufx6.h
--rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/bitstream.h
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/compiler.h
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/debug.c
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/debug.h
--rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/entropy_common.c
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/error_private.h
--rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/error_public.h
--rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fse.h
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fseU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fseU16.h
--rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fse_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fse_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/hist.c
--rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/hist.h
--rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/huf.h
--rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/huf_compress.c
--rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/huf_decompress.c
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/mem.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.328793 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/COPYING
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/bench.c
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/bench.h
--rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/commandline.c
--rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/cpu.h
--rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fileio.c
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fileio.h
--rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fseDist.c
--rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fseDist.h
--rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fullbench.c
--rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fuzzer.c
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
--rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fuzzerU16.c
--rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/probaGenerator.c
--rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/xxhash.c
--rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/xxhash.h
--rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/zlibh.c
--rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/zlibh.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.332793 chiapos-2.0.0b5/lib/include/
--rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/lib/include/picosha2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/mypi.ini
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.332793 chiapos-2.0.0b5/python-bindings/
--rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/python-bindings/chiapos.cpp
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 20:54:14.348793 chiapos-2.0.0b5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.340793 chiapos-2.0.0b5/src/
--rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b17phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b17phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b17phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b17sort_manager.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.344793 chiapos-2.0.0b5/src/b3/
--rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3.c
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3.h
--rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_avx2.c
--rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_avx2_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_avx512.c
--rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_avx512_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_dispatch.c
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_impl.h
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_portable.c
--rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_sse41.c
--rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/b3/blake3_sse41_x86-64_unix.S
--rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/bitfield.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/bitfield_index.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/bits.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/calculate_bucket.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/chacha8.c
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/chacha8.h
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/chia_filesystem.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/cli.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/encoding.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/entry_sizes.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/exceptions.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/phase1.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/phase2.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/phase3.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/phase4.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/phases.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/plotter_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/pos_constants.hpp
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/progress.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    49812 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/prover_disk.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/quicksort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/serialize.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/sort_manager.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/threading.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/uniformsort.hpp
--rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/util.hpp
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/src/verifier.hpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.348793 chiapos-2.0.0b5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tests/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tests/plot-resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tests/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tests/test_python_bindings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.348793 chiapos-2.0.0b5/tools/
--rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tools/disk.gnuplot
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/tools/parse_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 20:54:14.348793 chiapos-2.0.0b5/uint128_t/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/endianness.h
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/uint128_t.build
--rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/uint128_t.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/uint128_t.h
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/uint128_t.include
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-17 20:54:04.000000 chiapos-2.0.0b5/uint128_t/uint128_t_config.include
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.571741 chiapos-2.0.0rc1/
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.clang-format
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.523742 chiapos-2.0.0rc1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.531741 chiapos-2.0.0rc1/.github/actions/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/actions/fetch_bladebit_harvester.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.535741 chiapos-2.0.0rc1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2149 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/build-test-cplusplus.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    10051 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/build-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/doc-html-pdf.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/manual-plot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/plot-k27-no-bitfield.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/plot-k27.yaml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1330 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.github/workflows/stale-issue.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     7285 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-22 05:12:56.571741 chiapos-2.0.0rc1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3833 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.535741 chiapos-2.0.0rc1/chiapos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4178 2023-07-22 05:12:56.000000 chiapos-2.0.0rc1/chiapos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4709 2023-07-22 05:12:56.000000 chiapos-2.0.0rc1/chiapos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:12:56.000000 chiapos-2.0.0rc1/chiapos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 05:12:56.000000 chiapos-2.0.0rc1/chiapos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-22 05:12:56.000000 chiapos-2.0.0rc1/chiapos.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)       41 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/docker-build.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)       57 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/docker-test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.539741 chiapos-2.0.0rc1/documents/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   224153 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/bucket_graph.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)   116670 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/code_documentation.pdf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.539741 chiapos-2.0.0rc1/documents/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    13861 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/images/aesctr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    62757 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/images/beyondhellman.png
+-rw-r--r--   0 runner    (1001) docker     (123)    67446 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/images/beyondhellman2.png
+-rw-r--r--   0 runner    (1001) docker     (123)   146667 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/images/pointerformat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    40389 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/images/proofofspace.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1368315 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/proof_of_space.html
+-rw-r--r--   0 runner    (1001) docker     (123)    75267 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/documents/proof_of_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.543741 chiapos-2.0.0rc1/hellman_example/
+-rw-r--r--   0 runner    (1001) docker     (123)    85217 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/Hellman attacks.pdf
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/aes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    22632 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    15920 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    41970 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/cxxopts.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6187 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13236 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/hellman.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    78714 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    28580 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34630 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/sort_on_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5474 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/hellman_example/verifier.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lgtm.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.527742 chiapos-2.0.0rc1/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.547741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3636 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.523742 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.547741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.547741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/
+-rw-r--r--   0 runner    (1001) docker     (123)    10066 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)     2821 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.547741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.547741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc
+-rw-r--r--   0 runner    (1001) docker     (123)    10601 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj
+-rw-r--r--   0 runner    (1001) docker     (123)     5026 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.551741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.551741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/
+-rw-r--r--   0 runner    (1001) docker     (123)     2928 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6.h
+-rw-r--r--   0 runner    (1001) docker     (123)    18735 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    18204 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/bitstream.h
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/compiler.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.h
+-rw-r--r--   0 runner    (1001) docker     (123)     9599 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/entropy_common.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_private.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2434 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_public.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32982 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse.h
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.h
+-rw-r--r--   0 runner    (1001) docker     (123)    27523 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11179 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4327 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19479 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32593 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_compress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    45802 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_decompress.c
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/mem.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.555741 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/COPYING
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    29002 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12301 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/commandline.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4444 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/cpu.h
+-rw-r--r--   0 runner    (1001) docker     (123)    22894 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19607 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.h
+-rw-r--r--   0 runner    (1001) docker     (123)    44827 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fullbench.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzer.c
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerHuff0.c
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerU16.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4406 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/probaGenerator.c
+-rw-r--r--   0 runner    (1001) docker     (123)    28510 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.c
+-rw-r--r--   0 runner    (1001) docker     (123)    12352 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.h
+-rw-r--r--   0 runner    (1001) docker     (123)    68887 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.c
+-rw-r--r--   0 runner    (1001) docker     (123)     4817 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.555741 chiapos-2.0.0rc1/lib/include/
+-rw-r--r--   0 runner    (1001) docker     (123)    13016 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/lib/include/picosha2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/mypi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.555741 chiapos-2.0.0rc1/python-bindings/
+-rw-r--r--   0 runner    (1001) docker     (123)     7575 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/python-bindings/chiapos.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 05:12:56.571741 chiapos-2.0.0rc1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     7842 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.563741 chiapos-2.0.0rc1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)    21159 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b17phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    21395 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b17phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b17phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11996 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b17sort_manager.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.567741 chiapos-2.0.0rc1/src/b3/
+-rw-r--r--   0 runner    (1001) docker     (123)    26722 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12411 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_avx2.c
+-rw-r--r--   0 runner    (1001) docker     (123)    65803 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_avx2_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)    47960 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_avx512.c
+-rw-r--r--   0 runner    (1001) docker     (123)    89081 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_avx512_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_dispatch.c
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_impl.h
+-rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_portable.c
+-rw-r--r--   0 runner    (1001) docker     (123)    20772 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_sse41.c
+-rw-r--r--   0 runner    (1001) docker     (123)    60859 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/b3/blake3_sse41_x86-64_unix.S
+-rw-r--r--   0 runner    (1001) docker     (123)     2144 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/bitfield.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/bitfield_index.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19655 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/bits.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11224 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/calculate_bucket.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/chacha8.c
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/chacha8.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/chia_filesystem.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11919 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/cli.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    16417 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     7635 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/encoding.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/entry_sizes.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/exceptions.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    32661 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/phase1.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11324 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/phase2.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    23014 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/phase3.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     8587 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/phase4.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/phases.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    19059 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/plotter_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/pos_constants.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/progress.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    49706 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/prover_disk.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     3272 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/quicksort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/serialize.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11844 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/sort_manager.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/threading.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     4253 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/uniformsort.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)    10882 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/util.hpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/src/verifier.hpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.567741 chiapos-2.0.0rc1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tests/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6367 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tests/plot-resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42154 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tests/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tests/test_python_bindings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.567741 chiapos-2.0.0rc1/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      879 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tools/disk.gnuplot
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/tools/parse_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 05:12:56.571741 chiapos-2.0.0rc1/uint128_t/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1385 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/endianness.h
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/uint128_t.build
+-rw-r--r--   0 runner    (1001) docker     (123)    13671 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/uint128_t.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/uint128_t.h
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/uint128_t.include
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-07-22 05:12:45.000000 chiapos-2.0.0rc1/uint128_t/uint128_t_config.include
```

### Comparing `chiapos-2.0.0b5/.github/actions/fetch_bladebit_harvester.sh` & `chiapos-2.0.0rc1/.github/actions/fetch_bladebit_harvester.sh`

 * *Files 14% similar despite different names*

```diff
@@ -18,22 +18,22 @@
 
 if [[ "${host_arch}" != "arm64" ]] && [[ "${host_arch}" != "x86-64" ]]; then
   echo >&2 "Unkonwn Architecture '${host_arch}'"
   exit 1
 fi
 
 ## Change this before releasing 2.0.0
-artifact_ver="v3.0.0-alpha4"
-artifact_base_url="https://github.com/harold-b/bladebit-test/releases/download/v3-alpha4-fixes"
+artifact_ver="v3.0.0-rc1"
+artifact_base_url="https://github.com/Chia-Network/bladebit/releases/download/v3.0.0-rc1"
 
-linux_arm_sha256="d6f4fc6014a0faa4a5735980a4c12753e205e6429a9d92ea1d32831e475df357"
-linux_x86_sha256="98c0efb464935455595d7a573027613c46a7921a95d3f9216b27814f84a1ac31"
-macos_arm_sha256="713849aa5d01df9ccfcec259920d86a4ddec83cc3bbc30860852dcf9ac793978"
-macos_x86_sha256="67885e4f95b11a115f37138309cc9fd92785229f76adefe6d23e15c45625c92f"
-windows_sha256="2a951daa19c65574808537007b874a29d9001bc4387c162633646b0f546676ca"
+linux_arm_sha256="d0af989049f077be726cf5cbc9b5e138defe7891214c23457bd6925fded68b3d"
+linux_x86_sha256="d7cb5525e11b27d386523730fcde4dfc099681ccddbd5861cf9c7ba7fbda9676"
+macos_arm_sha256="b63b8611791a02395ad3fa31f78f2983335301e8cf3352729026fb0aec9b8e3c"
+macos_x86_sha256="8b4ba2cb40a041ba64025f933eecb59942c5d85447d0fef7ded8e8e4527a0573"
+windows_sha256="bcfef83e1d9664308d8571b76af57f5a7e4b0fdc14a380deeb21b186b02b2356"
 ## End changes
 
 artifact_ext="tar.gz"
 sha_bin="sha256sum"
 expected_sha256=
 
 if [[ "$OSTYPE" == "darwin"* ]]; then
```

### Comparing `chiapos-2.0.0b5/.github/workflows/build-test-cplusplus.yml` & `chiapos-2.0.0rc1/.github/workflows/build-test-cplusplus.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/.github/workflows/build-wheels.yml` & `chiapos-2.0.0rc1/.github/workflows/build-wheels.yml`

 * *Files 2% similar despite different names*

```diff
@@ -38,20 +38,14 @@
               arm: [Linux, ARM64]
               intel: [ubuntu-latest]
           - name: Windows
             matrix: windows
             runs-on:
               intel: [windows-latest]
         python:
-          - major-dot-minor: '3.7'
-            cibw-build: 'cp37-*'
-            manylinux:
-              arm: manylinux2014
-              intel: manylinux2014
-            matrix: '3.7'
           - major-dot-minor: '3.8'
             cibw-build: 'cp38-*'
             manylinux:
               arm: manylinux2014
               intel: manylinux2014
             matrix: '3.8'
           - major-dot-minor: '3.9'
@@ -93,17 +87,17 @@
           - os:
               name: macOS
               matrix: macos
               runs-on:
                 arm: [macOS, ARM64]
                 intel: [macos-latest]
             python:
-              major-dot-minor: '3.7'
-              cibw-build: 'cp37-*'
-              matrix: '3.7'
+              major-dot-minor: '3.8'
+              cibw-build: 'cp38-*'
+              matrix: '3.8'
             arch:
               name: ARM
               matrix: arm
 
     steps:
     - name: Clean workspace
       uses: Chia-Network/actions/clean-workspace@main
```

### Comparing `chiapos-2.0.0b5/.github/workflows/doc-html-pdf.yml` & `chiapos-2.0.0rc1/.github/workflows/doc-html-pdf.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/.github/workflows/manual-plot.yml` & `chiapos-2.0.0rc1/.github/workflows/manual-plot.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/.github/workflows/plot-k27-no-bitfield.yaml` & `chiapos-2.0.0rc1/.github/workflows/plot-k27-no-bitfield.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/.github/workflows/plot-k27.yaml` & `chiapos-2.0.0rc1/.github/workflows/plot-k27.yaml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/.github/workflows/stale-issue.yml` & `chiapos-2.0.0rc1/.github/workflows/stale-issue.yml`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/CMakeLists.txt` & `chiapos-2.0.0rc1/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/Dockerfile` & `chiapos-2.0.0rc1/Dockerfile`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/LICENSE` & `chiapos-2.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/PKG-INFO` & `chiapos-2.0.0rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 2.0.0b5
+Version: 2.0.0rc1
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chiapos-2.0.0b5/README.md` & `chiapos-2.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/chiapos.egg-info/PKG-INFO` & `chiapos-2.0.0rc1/chiapos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chiapos
-Version: 2.0.0b5
+Version: 2.0.0rc1
 Summary: Chia proof of space plotting, proving, and verifying (wraps C++)
 Home-page: https://github.com/Chia-Network/chiapos
 Author: Mariano Sorgente
 Author-email: mariano@chia.net
 License: Apache License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `chiapos-2.0.0b5/chiapos.egg-info/SOURCES.txt` & `chiapos-2.0.0rc1/chiapos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/bucket_graph.pdf` & `chiapos-2.0.0rc1/documents/bucket_graph.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/code_documentation.pdf` & `chiapos-2.0.0rc1/documents/code_documentation.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/images/aesctr.png` & `chiapos-2.0.0rc1/documents/images/aesctr.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/images/beyondhellman.png` & `chiapos-2.0.0rc1/documents/images/beyondhellman.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/images/beyondhellman2.png` & `chiapos-2.0.0rc1/documents/images/beyondhellman2.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/images/pointerformat.png` & `chiapos-2.0.0rc1/documents/images/pointerformat.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/images/proofofspace.png` & `chiapos-2.0.0rc1/documents/images/proofofspace.png`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/proof_of_space.html` & `chiapos-2.0.0rc1/documents/proof_of_space.html`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/documents/proof_of_space.md` & `chiapos-2.0.0rc1/documents/proof_of_space.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/Hellman attacks.pdf` & `chiapos-2.0.0rc1/hellman_example/Hellman attacks.pdf`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/aes.hpp` & `chiapos-2.0.0rc1/hellman_example/aes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/bits.hpp` & `chiapos-2.0.0rc1/hellman_example/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/calculate_bucket.hpp` & `chiapos-2.0.0rc1/hellman_example/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/cli.cpp` & `chiapos-2.0.0rc1/hellman_example/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/cxxopts.hpp` & `chiapos-2.0.0rc1/hellman_example/cxxopts.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/encoding.hpp` & `chiapos-2.0.0rc1/hellman_example/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/hellman.hpp` & `chiapos-2.0.0rc1/hellman_example/hellman.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/picosha2.hpp` & `chiapos-2.0.0rc1/hellman_example/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/plotter_disk.hpp` & `chiapos-2.0.0rc1/hellman_example/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/pos_constants.hpp` & `chiapos-2.0.0rc1/hellman_example/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/prover_disk.hpp` & `chiapos-2.0.0rc1/hellman_example/prover_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/sort_on_disk.hpp` & `chiapos-2.0.0rc1/hellman_example/sort_on_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/util.hpp` & `chiapos-2.0.0rc1/hellman_example/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/hellman_example/verifier.hpp` & `chiapos-2.0.0rc1/hellman_example/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/LICENSE` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/README.md` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/FSE.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE/fse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/FSE.sln`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/fuzzer/fuzzer.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.rc`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/Visual/VC2012/libfse/libfse.vcxproj`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/fetch-content-CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/Archives/hufx6.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/Archives/hufx6_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/README.md` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/bitstream.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/bitstream.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/compiler.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/compiler.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/debug.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/debug.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/debug.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/entropy_common.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/entropy_common.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/error_private.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_private.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/error_public.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/error_public.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fse.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fseU16.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fseU16.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fseU16.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fse_compress.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/fse_decompress.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/fse_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/hist.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/hist.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/hist.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/huf.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/huf_compress.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_compress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/huf_decompress.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/huf_decompress.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/lib/mem.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/lib/mem.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/COPYING` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/COPYING`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/bench.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/bench.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/bench.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/commandline.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/commandline.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/cpu.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/cpu.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fileio.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fileio.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fileio.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fseDist.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fseDist.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fseDist.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fullbench.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fullbench.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fuzzer.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzer.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fuzzerHuff0.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerHuff0.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/fuzzerU16.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/fuzzerU16.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/probaGenerator.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/probaGenerator.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/xxhash.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/xxhash.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/xxhash.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/zlibh.c` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/FiniteStateEntropy/programs/zlibh.h` & `chiapos-2.0.0rc1/lib/FiniteStateEntropy/programs/zlibh.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/lib/include/picosha2.hpp` & `chiapos-2.0.0rc1/lib/include/picosha2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/python-bindings/chiapos.cpp` & `chiapos-2.0.0rc1/python-bindings/chiapos.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/setup.py` & `chiapos-2.0.0rc1/setup.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b17phase2.hpp` & `chiapos-2.0.0rc1/src/b17phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b17phase3.hpp` & `chiapos-2.0.0rc1/src/b17phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b17phase4.hpp` & `chiapos-2.0.0rc1/src/b17phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b17sort_manager.hpp` & `chiapos-2.0.0rc1/src/b17sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3.c` & `chiapos-2.0.0rc1/src/b3/blake3.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3.h` & `chiapos-2.0.0rc1/src/b3/blake3.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_avx2.c` & `chiapos-2.0.0rc1/src/b3/blake3_avx2.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_avx2_x86-64_unix.S` & `chiapos-2.0.0rc1/src/b3/blake3_avx2_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_avx512.c` & `chiapos-2.0.0rc1/src/b3/blake3_avx512.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_avx512_x86-64_unix.S` & `chiapos-2.0.0rc1/src/b3/blake3_avx512_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_dispatch.c` & `chiapos-2.0.0rc1/src/b3/blake3_dispatch.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_impl.h` & `chiapos-2.0.0rc1/src/b3/blake3_impl.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_portable.c` & `chiapos-2.0.0rc1/src/b3/blake3_portable.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_sse41.c` & `chiapos-2.0.0rc1/src/b3/blake3_sse41.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/b3/blake3_sse41_x86-64_unix.S` & `chiapos-2.0.0rc1/src/b3/blake3_sse41_x86-64_unix.S`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/bitfield.hpp` & `chiapos-2.0.0rc1/src/bitfield.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/bitfield_index.hpp` & `chiapos-2.0.0rc1/src/bitfield_index.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/bits.hpp` & `chiapos-2.0.0rc1/src/bits.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/calculate_bucket.hpp` & `chiapos-2.0.0rc1/src/calculate_bucket.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/chacha8.c` & `chiapos-2.0.0rc1/src/chacha8.c`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/chia_filesystem.hpp` & `chiapos-2.0.0rc1/src/chia_filesystem.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/cli.cpp` & `chiapos-2.0.0rc1/src/cli.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/disk.hpp` & `chiapos-2.0.0rc1/src/disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/encoding.hpp` & `chiapos-2.0.0rc1/src/encoding.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/entry_sizes.hpp` & `chiapos-2.0.0rc1/src/entry_sizes.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/exceptions.hpp` & `chiapos-2.0.0rc1/src/exceptions.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/phase1.hpp` & `chiapos-2.0.0rc1/src/phase1.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/phase2.hpp` & `chiapos-2.0.0rc1/src/phase2.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/phase3.hpp` & `chiapos-2.0.0rc1/src/phase3.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/phase4.hpp` & `chiapos-2.0.0rc1/src/phase4.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/phases.hpp` & `chiapos-2.0.0rc1/src/phases.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/plotter_disk.hpp` & `chiapos-2.0.0rc1/src/plotter_disk.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/pos_constants.hpp` & `chiapos-2.0.0rc1/src/pos_constants.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/prover_disk.hpp` & `chiapos-2.0.0rc1/src/prover_disk.hpp`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 #endif
 #include <stdio.h>
 
 #include <algorithm>  // std::min
 #include <fstream>
 #include <future>
 #include <iostream>
-#include <mutex>
 #include <string>
 #include <utility>
 #include <vector>
 #include <mutex>
 #include <condition_variable>
 
 #include "../lib/include/picosha2.hpp"
@@ -179,26 +178,23 @@
     }
 
     GreenReaperContext* pop() {
         std::unique_lock<std::mutex> lock(mutex);
         while (queue.empty()) {
             condition.wait(lock);
         }
-        dequeue_lock.lock();
         GreenReaperContext* gr = queue.front();
         queue.pop();
-        dequeue_lock.unlock();
         return gr;
     }
 
 private:
     std::queue<GreenReaperContext*> queue;
     std::mutex mutex;
     std::condition_variable condition;
-    std::mutex dequeue_lock;
 };
 
 class ProofCache {
     static constexpr uint32_t MAX_ENTRIES = 64;
 
     struct Entry {
         alignas(16) uint8_t challenge[32];
```

### Comparing `chiapos-2.0.0b5/src/quicksort.hpp` & `chiapos-2.0.0rc1/src/quicksort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/serialize.hpp` & `chiapos-2.0.0rc1/src/serialize.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/sort_manager.hpp` & `chiapos-2.0.0rc1/src/sort_manager.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/threading.hpp` & `chiapos-2.0.0rc1/src/threading.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/uniformsort.hpp` & `chiapos-2.0.0rc1/src/uniformsort.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/util.hpp` & `chiapos-2.0.0rc1/src/util.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/src/verifier.hpp` & `chiapos-2.0.0rc1/src/verifier.hpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/tests/plot-resources.py` & `chiapos-2.0.0rc1/tests/plot-resources.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/tests/test.cpp` & `chiapos-2.0.0rc1/tests/test.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/tests/test_python_bindings.py` & `chiapos-2.0.0rc1/tests/test_python_bindings.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/tools/disk.gnuplot` & `chiapos-2.0.0rc1/tools/disk.gnuplot`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/tools/parse_disk.py` & `chiapos-2.0.0rc1/tools/parse_disk.py`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/uint128_t/LICENSE` & `chiapos-2.0.0rc1/uint128_t/LICENSE`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/uint128_t/README.md` & `chiapos-2.0.0rc1/uint128_t/README.md`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/uint128_t/endianness.h` & `chiapos-2.0.0rc1/uint128_t/endianness.h`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/uint128_t/uint128_t.cpp` & `chiapos-2.0.0rc1/uint128_t/uint128_t.cpp`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/uint128_t/uint128_t.include` & `chiapos-2.0.0rc1/uint128_t/uint128_t.include`

 * *Files identical despite different names*

### Comparing `chiapos-2.0.0b5/uint128_t/uint128_t_config.include` & `chiapos-2.0.0rc1/uint128_t/uint128_t_config.include`

 * *Files identical despite different names*

