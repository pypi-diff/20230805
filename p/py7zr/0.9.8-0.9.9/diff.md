# Comparing `tmp/py7zr-0.9.8.tar.gz` & `tmp/py7zr-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/tmp/tmph_7_ysfi/tmpbhjabuqa/py7zr-0.9.8.tar", last modified: Sun Oct  4 07:20:13 2020, max compression
+gzip compressed data, was "/tmp/tmp6fvih5dr/tmpyk3k7rls/py7zr-0.9.9.tar", last modified: Sun Oct  4 08:36:28 2020, max compression
```

## Comparing `py7zr-0.9.8.tar` & `py7zr-0.9.9.tar`

### file list

```diff
@@ -1,143 +1,145 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/.github/
--rw-r--r--   0 runner    (1001) docker     (116)      676 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/FUNDING.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (116)     1002 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (116)      595 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/ISSUE_TEMPLATE/feature_request.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     1218 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/workflows/publish-to-test-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (116)      755 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/workflows/release-note.yml
--rw-r--r--   0 runner    (1001) docker     (116)     1375 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/workflows/run-tox-tests.yml
--rw-r--r--   0 runner    (1001) docker     (116)      635 2020-10-04 07:20:00.000000 py7zr-0.9.8/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (116)      172 2020-10-04 07:20:00.000000 py7zr-0.9.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)      194 2020-10-04 07:20:00.000000 py7zr-0.9.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)      375 2020-10-04 07:20:00.000000 py7zr-0.9.8/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (116)    20499 2020-10-04 07:20:00.000000 py7zr-0.9.8/Changelog.rst
--rw-r--r--   0 runner    (1001) docker     (116)    26530 2020-10-04 07:20:00.000000 py7zr-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      576 2020-10-04 07:20:00.000000 py7zr-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)    41614 2020-10-04 07:20:13.000000 py7zr-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)    10481 2020-10-04 07:20:00.000000 py7zr-0.9.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      630 2020-10-04 07:20:00.000000 py7zr-0.9.8/azure-pipelines.yml
--rw-r--r--   0 runner    (1001) docker     (116)      429 2020-10-04 07:20:00.000000 py7zr-0.9.8/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (116)      414 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (116)     7659 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (116)       28 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/_config.yml
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     5298 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/_static/logo.png
--rw-r--r--   0 runner    (1001) docker     (116)    11475 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)    32115 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/archive_format.rst
--rw-r--r--   0 runner    (1001) docker     (116)     9847 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)     4600 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/contribution.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/docs/diagrams/
--rw-r--r--   0 runner    (1001) docker     (116)      305 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/diagrams/abstractio.dot
--rw-r--r--   0 runner    (1001) docker     (116)      379 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/diagrams/callbacks.dot
--rw-r--r--   0 runner    (1001) docker     (116)     9766 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/diagrams/classes.dot
--rw-r--r--   0 runner    (1001) docker     (116)     3135 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/diagrams/compressor_classes.dot
--rw-r--r--   0 runner    (1001) docker     (116)     3504 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/diagrams/header_classes.dot
--rw-r--r--   0 runner    (1001) docker     (116)     1548 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/diagrams/packages.dot
--rw-r--r--   0 runner    (1001) docker     (116)     4096 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/glossary.rst
--rw-r--r--   0 runner    (1001) docker     (116)      316 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)     6991 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/docs/presentations/
--rw-r--r--   0 runner    (1001) docker     (116)   741861 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/presentations/Introduction_of_py7zr.odp
--rw-r--r--   0 runner    (1001) docker     (116)   471731 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/presentations/Introduction_of_py7zr.pdf
--rw-r--r--   0 runner    (1001) docker     (116)     2688 2020-10-04 07:20:00.000000 py7zr-0.9.8/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (116)     5097 2020-10-04 07:20:00.000000 py7zr-0.9.8/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr/
--rw-r--r--   0 runner    (1001) docker     (116)     2491 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      988 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    39961 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/archiveinfo.py
--rw-r--r--   0 runner    (1001) docker     (116)     2043 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (116)    15506 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)    41051 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/compressor.py
--rw-r--r--   0 runner    (1001) docker     (116)     1292 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)    11687 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     5676 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/properties.py
--rw-r--r--   0 runner    (1001) docker     (116)    50753 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/py7zr.py
--rw-r--r--   0 runner    (1001) docker     (116)     7759 2020-10-04 07:20:00.000000 py7zr-0.9.8/py7zr/win32compat.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)    41614 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2940 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       47 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      454 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-04 07:20:13.000000 py7zr-0.9.8/py7zr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)      393 2020-10-04 07:20:00.000000 py7zr-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     1801 2020-10-04 07:20:13.000000 py7zr-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      113 2020-10-04 07:20:00.000000 py7zr-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      762 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)    12800 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/bcj.bin
--rw-r--r--   0 runner    (1001) docker     (116)    16206 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/bugzilla_4.7z
--rw-r--r--   0 runner    (1001) docker     (116)   272671 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/bzip2_2.7z
--rw-r--r--   0 runner    (1001) docker     (116)      239 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/copy.7z
--rw-r--r--   0 runner    (1001) docker     (116)     1313 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/copy_2.7z
--rw-r--r--   0 runner    (1001) docker     (116)      805 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/crc_corrupted.7z
--rw-r--r--   0 runner    (1001) docker     (116)      226 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/deflate.7z
--rw-r--r--   0 runner    (1001) docker     (116)      227 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/deflate64.7z
--rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/empty.7z
--rw-r--r--   0 runner    (1001) docker     (116)      251 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/encrypted_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)    54676 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/encrypted_2.7z
--rw-r--r--   0 runner    (1001) docker     (116)      711 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/encrypted_3.7z
--rw-r--r--   0 runner    (1001) docker     (116)    13465 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/encrypted_4.7z
--rw-r--r--   0 runner    (1001) docker     (116)      166 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/filename_encryption.7z
--rw-r--r--   0 runner    (1001) docker     (116)      121 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/github_14.7z
--rw-r--r--   0 runner    (1001) docker     (116)      203 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/github_14_multi.7z
--rw-r--r--   0 runner    (1001) docker     (116)   197268 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/issue_218.7z
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/tests/data/lib/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/tests/data/lib/aarch64-linux-gnu/
--rw-r--r--   0 runner    (1001) docker     (116)   150136 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lib/aarch64-linux-gnu/liblzma.so.0
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/tests/data/lib/powerpc64le-linux-gnu/
--rw-r--r--   0 runner    (1001) docker     (116)   199232 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lib/powerpc64le-linux-gnu/liblzma.so.0
--rw-r--r--   0 runner    (1001) docker     (116)     1079 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/longpath.7z
--rw-r--r--   0 runner    (1001) docker     (116)      800 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lz4.7z
--rw-r--r--   0 runner    (1001) docker     (116)      657 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2_bcj_arm.7z
--rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2_bcj_armt.7z
--rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2_bcj_ia64.7z
--rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2_bcj_ppc.7z
--rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2_bcj_sparc.7z
--rw-r--r--   0 runner    (1001) docker     (116)    52337 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2bcj.7z
--rw-r--r--   0 runner    (1001) docker     (116)    51169 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2bcj2.7z
--rw-r--r--   0 runner    (1001) docker     (116)      175 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma2delta_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)      159 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)      222 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_bcj2_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)    20474 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_bcj_arm.7z
--rw-r--r--   0 runner    (1001) docker     (116)    28957 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_bcj_armt.7z
--rw-r--r--   0 runner    (1001) docker     (116)    20164 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_bcj_ppc.7z
--rw-r--r--   0 runner    (1001) docker     (116)    18794 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_bcj_sparc.7z
--rw-r--r--   0 runner    (1001) docker     (116)    11456 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/lzma_bcj_x86.7z
--rw-r--r--   0 runner    (1001) docker     (116)   631690 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/mblock_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)   222788 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/p7zip-zstd.7z
--rw-r--r--   0 runner    (1001) docker     (116)      228 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/ppmd.7z
--rw-r--r--   0 runner    (1001) docker     (116)      233 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/solid.7z
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 07:20:13.000000 py7zr-0.9.8/tests/data/src/
--rw-r--r--   0 runner    (1001) docker     (116)       11 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/src/bra.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1758 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/symlink.7z
--rw-r--r--   0 runner    (1001) docker     (116)       33 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test1.txt
--rw-r--r--   0 runner    (1001) docker     (116)      657 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_1.7z
--rw-r--r--   0 runner    (1001) docker     (116)     1663 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_2.7z
--rw-r--r--   0 runner    (1001) docker     (116)     9055 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_3.7z
--rw-r--r--   0 runner    (1001) docker     (116)      225 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_5.7z
--rw-r--r--   0 runner    (1001) docker     (116)    11600 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_6.7z
--rw-r--r--   0 runner    (1001) docker     (116)      199 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_folder.7z
--rw-r--r--   0 runner    (1001) docker     (116)      250 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/test_lzma2bcj2.7z
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/umlaut-non_solid.7z
--rw-r--r--   0 runner    (1001) docker     (116)      163 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/umlaut-solid.7z
--rw-r--r--   0 runner    (1001) docker     (116)    12800 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/x86.bin
--rw-r--r--   0 runner    (1001) docker     (116)      177 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/zerosize.7z
--rw-r--r--   0 runner    (1001) docker     (116)      652 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/data/zstd.7z
--rw-r--r--   0 runner    (1001) docker     (116)    42789 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_archive.py
--rw-r--r--   0 runner    (1001) docker     (116)    23897 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_basic.py
--rw-r--r--   0 runner    (1001) docker     (116)     1968 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (116)     4042 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_concurrent.py
--rw-r--r--   0 runner    (1001) docker     (116)     8771 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_encryption.py
--rw-r--r--   0 runner    (1001) docker     (116)     8124 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_extra_codecs.py
--rw-r--r--   0 runner    (1001) docker     (116)    19376 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_extract.py
--rw-r--r--   0 runner    (1001) docker     (116)     4101 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_info.py
--rw-r--r--   0 runner    (1001) docker     (116)    26295 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_unit.py
--rw-r--r--   0 runner    (1001) docker     (116)     4083 2020-10-04 07:20:00.000000 py7zr-0.9.8/tests/test_win32compat.py
--rw-r--r--   0 runner    (1001) docker     (116)     2040 2020-10-04 07:20:00.000000 py7zr-0.9.8/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/.github/
+-rw-r--r--   0 runner    (1001) docker     (116)      676 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/FUNDING.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (116)     1002 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (116)      595 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/ISSUE_TEMPLATE/feature_request.md
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1218 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/workflows/publish-to-test-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      755 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/workflows/release-note.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1375 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/workflows/run-tox-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      635 2020-10-04 08:36:12.000000 py7zr-0.9.9/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      172 2020-10-04 08:36:12.000000 py7zr-0.9.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)      194 2020-10-04 08:36:12.000000 py7zr-0.9.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      375 2020-10-04 08:36:12.000000 py7zr-0.9.9/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (116)    20698 2020-10-04 08:36:12.000000 py7zr-0.9.9/Changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    26530 2020-10-04 08:36:12.000000 py7zr-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      576 2020-10-04 08:36:12.000000 py7zr-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    41885 2020-10-04 08:36:28.000000 py7zr-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    10481 2020-10-04 08:36:12.000000 py7zr-0.9.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      630 2020-10-04 08:36:12.000000 py7zr-0.9.9/azure-pipelines.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      429 2020-10-04 08:36:12.000000 py7zr-0.9.9/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)      414 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     7659 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (116)       28 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/_config.yml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (116)     5298 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/_static/logo.png
+-rw-r--r--   0 runner    (1001) docker     (116)    11475 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (116)    32115 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/archive_format.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     9847 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4600 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/contribution.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/docs/diagrams/
+-rw-r--r--   0 runner    (1001) docker     (116)      305 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/diagrams/abstractio.dot
+-rw-r--r--   0 runner    (1001) docker     (116)      379 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/diagrams/callbacks.dot
+-rw-r--r--   0 runner    (1001) docker     (116)     9766 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/diagrams/classes.dot
+-rw-r--r--   0 runner    (1001) docker     (116)     3135 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/diagrams/compressor_classes.dot
+-rw-r--r--   0 runner    (1001) docker     (116)     3504 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/diagrams/header_classes.dot
+-rw-r--r--   0 runner    (1001) docker     (116)     1548 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/diagrams/packages.dot
+-rw-r--r--   0 runner    (1001) docker     (116)     4096 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/glossary.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      316 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     6991 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/docs/presentations/
+-rw-r--r--   0 runner    (1001) docker     (116)   741861 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/presentations/Introduction_of_py7zr.odp
+-rw-r--r--   0 runner    (1001) docker     (116)   471731 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/presentations/Introduction_of_py7zr.pdf
+-rw-r--r--   0 runner    (1001) docker     (116)     2688 2020-10-04 08:36:12.000000 py7zr-0.9.9/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     5097 2020-10-04 08:36:12.000000 py7zr-0.9.9/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/py7zr/
+-rw-r--r--   0 runner    (1001) docker     (116)     2491 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      988 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    39961 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/archiveinfo.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2043 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15506 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/cli.py
+-rw-r--r--   0 runner    (1001) docker     (116)    41322 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/compressor.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1292 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11687 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5676 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/properties.py
+-rw-r--r--   0 runner    (1001) docker     (116)    50753 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/py7zr.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7759 2020-10-04 08:36:12.000000 py7zr-0.9.9/py7zr/win32compat.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/py7zr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    41885 2020-10-04 08:36:27.000000 py7zr-0.9.9/py7zr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2984 2020-10-04 08:36:28.000000 py7zr-0.9.9/py7zr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-10-04 08:36:27.000000 py7zr-0.9.9/py7zr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       47 2020-10-04 08:36:27.000000 py7zr-0.9.9/py7zr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      454 2020-10-04 08:36:27.000000 py7zr-0.9.9/py7zr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-10-04 08:36:27.000000 py7zr-0.9.9/py7zr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      393 2020-10-04 08:36:12.000000 py7zr-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (116)     1801 2020-10-04 08:36:28.000000 py7zr-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      113 2020-10-04 08:36:12.000000 py7zr-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1831 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      762 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (116)    12800 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/bcj.bin
+-rw-r--r--   0 runner    (1001) docker     (116)    16206 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/bugzilla_4.7z
+-rw-r--r--   0 runner    (1001) docker     (116)   272671 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/bzip2_2.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      239 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/copy.7z
+-rw-r--r--   0 runner    (1001) docker     (116)     1313 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/copy_2.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    10130 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/copy_bcj_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      805 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/crc_corrupted.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      226 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/deflate.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/deflate64.7z
+-rw-r--r--   0 runner    (1001) docker     (116)       32 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/empty.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      251 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/encrypted_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    54676 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/encrypted_2.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      711 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/encrypted_3.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    13465 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/encrypted_4.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      166 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/filename_encryption.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      121 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/github_14.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      203 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/github_14_multi.7z
+-rw-r--r--   0 runner    (1001) docker     (116)   197268 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/issue_218.7z
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/tests/data/lib/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/tests/data/lib/aarch64-linux-gnu/
+-rw-r--r--   0 runner    (1001) docker     (116)   150136 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lib/aarch64-linux-gnu/liblzma.so.0
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/tests/data/lib/powerpc64le-linux-gnu/
+-rw-r--r--   0 runner    (1001) docker     (116)   199232 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lib/powerpc64le-linux-gnu/liblzma.so.0
+-rw-r--r--   0 runner    (1001) docker     (116)     1079 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/longpath.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      800 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lz4.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      657 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2_bcj_arm.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2_bcj_armt.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2_bcj_ia64.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2_bcj_ppc.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      243 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2_bcj_sparc.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    52337 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2bcj.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    51169 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2bcj2.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      175 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma2delta_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      159 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      222 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_bcj2_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    20474 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_bcj_arm.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    28957 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_bcj_armt.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    20164 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_bcj_ppc.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    18794 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_bcj_sparc.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    11456 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/lzma_bcj_x86.7z
+-rw-r--r--   0 runner    (1001) docker     (116)   631690 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/mblock_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)   222788 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/p7zip-zstd.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      228 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/ppmd.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      233 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/solid.7z
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-10-04 08:36:28.000000 py7zr-0.9.9/tests/data/src/
+-rw-r--r--   0 runner    (1001) docker     (116)       11 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/src/bra.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1758 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/symlink.7z
+-rw-r--r--   0 runner    (1001) docker     (116)       33 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test1.txt
+-rw-r--r--   0 runner    (1001) docker     (116)      657 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_1.7z
+-rw-r--r--   0 runner    (1001) docker     (116)     1663 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_2.7z
+-rw-r--r--   0 runner    (1001) docker     (116)     9055 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_3.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      225 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_5.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    11600 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_6.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      199 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_folder.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      250 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/test_lzma2bcj2.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/umlaut-non_solid.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      163 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/umlaut-solid.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    12800 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/x86.bin
+-rw-r--r--   0 runner    (1001) docker     (116)      177 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/zerosize.7z
+-rw-r--r--   0 runner    (1001) docker     (116)      652 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/data/zstd.7z
+-rw-r--r--   0 runner    (1001) docker     (116)    42789 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_archive.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23897 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_basic.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1968 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4042 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8771 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_encryption.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8124 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_extra_codecs.py
+-rw-r--r--   0 runner    (1001) docker     (116)    19376 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_extract.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4101 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_info.py
+-rw-r--r--   0 runner    (1001) docker     (116)      318 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26295 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_unit.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4083 2020-10-04 08:36:12.000000 py7zr-0.9.9/tests/test_win32compat.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2040 2020-10-04 08:36:12.000000 py7zr-0.9.9/tox.ini
```

### Comparing `py7zr-0.9.8/.github/FUNDING.yml` & `py7zr-0.9.9/.github/FUNDING.yml`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/.github/ISSUE_TEMPLATE/bug_report.md` & `py7zr-0.9.9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/.github/ISSUE_TEMPLATE/feature_request.md` & `py7zr-0.9.9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/.github/workflows/publish-to-test-pypi.yml` & `py7zr-0.9.9/.github/workflows/publish-to-test-pypi.yml`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/.github/workflows/release-note.yml` & `py7zr-0.9.9/.github/workflows/release-note.yml`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/.github/workflows/run-tox-tests.yml` & `py7zr-0.9.9/.github/workflows/run-tox-tests.yml`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/.github/workflows/stale.yml` & `py7zr-0.9.9/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/Changelog.rst` & `py7zr-0.9.9/Changelog.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,22 @@
 
 Removed
 -------
 
 Security
 --------
 
+`v0.9.9`_
+=========
+
+Fixed
+-----
+
+* (backport) Fix BCJ filter issue failing a certain data when LZMA+BCJ compression(#240, #250)
+
 `v0.9.8`_
 =========
 
 Changed
 -------
 
 * Avoid re-read header data from fike, otherwise calculate CRC32 when writing header.(#246)
@@ -770,15 +778,16 @@
 Changed
 -------
 
 * refactoring all the code.
 
 
 .. History links
-.. _Unreleased: https://github.com/miurahr/py7zr/compare/v0.9.8...HEAD
+.. _Unreleased: https://github.com/miurahr/py7zr/compare/v0.9.9...HEAD
+.. _v0.9.9: https://github.com/miurahr/py7zr/compare/v0.9.8...v0.9.9
 .. _v0.9.8: https://github.com/miurahr/py7zr/compare/v0.9.7...v0.9.8
 .. _v0.9.7: https://github.com/miurahr/py7zr/compare/v0.9.6...v0.9.7
 .. _v0.9.6: https://github.com/miurahr/py7zr/compare/v0.9.5...v0.9.6
 .. _v0.9.5: https://github.com/miurahr/py7zr/compare/v0.9.4...v0.9.5
 .. _v0.9.4: https://github.com/miurahr/py7zr/compare/v0.9.3...v0.9.4
 .. _v0.9.3: https://github.com/miurahr/py7zr/compare/v0.9.2...v0.9.3
 .. _v0.9.2: https://github.com/miurahr/py7zr/compare/v0.9.1...v0.9.2
```

### Comparing `py7zr-0.9.8/LICENSE` & `py7zr-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/MANIFEST.in` & `py7zr-0.9.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/PKG-INFO` & `py7zr-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py7zr
-Version: 0.9.8
+Version: 0.9.9
 Summary: Pure python 7-zip library
 Home-page: https://github.com/miurahr/py7zr
 Author: Hiroshi Miura
 Author-email: miurahr@linux.com
 License: LGPL-2.1+
 Description: ======================================
         |logo| py7zr -- a 7z library on python
@@ -389,14 +389,22 @@
         
         Removed
         -------
         
         Security
         --------
         
+        `v0.9.9`_
+        =========
+        
+        Fixed
+        -----
+        
+        * (backport) Fix BCJ filter issue failing a certain data when LZMA+BCJ compression(#240, #250)
+        
         `v0.9.8`_
         =========
         
         Changed
         -------
         
         * Avoid re-read header data from fike, otherwise calculate CRC32 when writing header.(#246)
@@ -1138,15 +1146,16 @@
         Changed
         -------
         
         * refactoring all the code.
         
         
         .. History links
-        .. _Unreleased: https://github.com/miurahr/py7zr/compare/v0.9.8...HEAD
+        .. _Unreleased: https://github.com/miurahr/py7zr/compare/v0.9.9...HEAD
+        .. _v0.9.9: https://github.com/miurahr/py7zr/compare/v0.9.8...v0.9.9
         .. _v0.9.8: https://github.com/miurahr/py7zr/compare/v0.9.7...v0.9.8
         .. _v0.9.7: https://github.com/miurahr/py7zr/compare/v0.9.6...v0.9.7
         .. _v0.9.6: https://github.com/miurahr/py7zr/compare/v0.9.5...v0.9.6
         .. _v0.9.5: https://github.com/miurahr/py7zr/compare/v0.9.4...v0.9.5
         .. _v0.9.4: https://github.com/miurahr/py7zr/compare/v0.9.3...v0.9.4
         .. _v0.9.3: https://github.com/miurahr/py7zr/compare/v0.9.2...v0.9.3
         .. _v0.9.2: https://github.com/miurahr/py7zr/compare/v0.9.1...v0.9.2
```

### Comparing `py7zr-0.9.8/README.rst` & `py7zr-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/azure-pipelines.yml` & `py7zr-0.9.9/azure-pipelines.yml`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/Makefile` & `py7zr-0.9.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/_static/logo.png` & `py7zr-0.9.9/docs/_static/logo.png`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/api.rst` & `py7zr-0.9.9/docs/api.rst`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/archive_format.rst` & `py7zr-0.9.9/docs/archive_format.rst`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/conf.py` & `py7zr-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/contribution.rst` & `py7zr-0.9.9/docs/contribution.rst`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/diagrams/classes.dot` & `py7zr-0.9.9/docs/diagrams/classes.dot`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/diagrams/compressor_classes.dot` & `py7zr-0.9.9/docs/diagrams/compressor_classes.dot`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/diagrams/header_classes.dot` & `py7zr-0.9.9/docs/diagrams/header_classes.dot`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/diagrams/packages.dot` & `py7zr-0.9.9/docs/diagrams/packages.dot`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/glossary.rst` & `py7zr-0.9.9/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/make.bat` & `py7zr-0.9.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/presentations/Introduction_of_py7zr.odp` & `py7zr-0.9.9/docs/presentations/Introduction_of_py7zr.odp`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/presentations/Introduction_of_py7zr.pdf` & `py7zr-0.9.9/docs/presentations/Introduction_of_py7zr.pdf`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/docs/user_guide.rst` & `py7zr-0.9.9/docs/user_guide.rst`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/logo.svg` & `py7zr-0.9.9/logo.svg`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/__init__.py` & `py7zr-0.9.9/py7zr/__init__.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/__main__.py` & `py7zr-0.9.9/py7zr/__main__.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/archiveinfo.py` & `py7zr-0.9.9/py7zr/archiveinfo.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/callbacks.py` & `py7zr-0.9.9/py7zr/callbacks.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/cli.py` & `py7zr-0.9.9/py7zr/cli.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/compressor.py` & `py7zr-0.9.9/py7zr/compressor.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,19 @@
                     dest = (src - distance) >> 2
                 self.buffer[i:i + 3] = struct.pack('<L', dest & 0xFFFFFF)[:3]
             i += 4
         self.current_position += i
         return i
 
     def _x86_code(self) -> int:
+        """
+        The code algorithm from liblzma/simple/x86.c
+        It is slightly different from LZMA-SDK's bra86.c
+        :return: buffer position
+        """
         size = len(self.buffer)
         if size < 5:
             return 0
         if self.current_position - self.prev_pos > 5:
             self.prev_pos = self.current_position - 5
         view = memoryview(self.buffer)
         limit = size - 5
@@ -425,14 +430,16 @@
                 write_view[0:3] = (dest & 0xFFFFFF).to_bytes(3, 'little')
                 write_view[3:4] = [b'\x00', b'\xff'][(dest >> 24) & 1]  # (~(((dest >> 24) & 1) - 1)) & 0xFF
                 buffer_pos += 5
                 self.prev_mask = 0
             else:
                 buffer_pos += 1
                 self.prev_mask |= 1
+                if self.buffer[buffer_pos + 3] in [0, 0xff]:
+                    self.prev_mask |= 0x10
         self.current_position += buffer_pos
         return buffer_pos
 
     def _decompress(self, data: Union[bytes, bytearray, memoryview], max_length: int = -1) -> bytes:
         self.buffer.extend(data)
         pos = self._method()
         if self.current_position > self.stream_size - self._readahead:
```

### Comparing `py7zr-0.9.8/py7zr/exceptions.py` & `py7zr-0.9.9/py7zr/exceptions.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/helpers.py` & `py7zr-0.9.9/py7zr/helpers.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/properties.py` & `py7zr-0.9.9/py7zr/properties.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/py7zr.py` & `py7zr-0.9.9/py7zr/py7zr.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr/win32compat.py` & `py7zr-0.9.9/py7zr/win32compat.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/py7zr.egg-info/PKG-INFO` & `py7zr-0.9.9/py7zr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py7zr
-Version: 0.9.8
+Version: 0.9.9
 Summary: Pure python 7-zip library
 Home-page: https://github.com/miurahr/py7zr
 Author: Hiroshi Miura
 Author-email: miurahr@linux.com
 License: LGPL-2.1+
 Description: ======================================
         |logo| py7zr -- a 7z library on python
@@ -389,14 +389,22 @@
         
         Removed
         -------
         
         Security
         --------
         
+        `v0.9.9`_
+        =========
+        
+        Fixed
+        -----
+        
+        * (backport) Fix BCJ filter issue failing a certain data when LZMA+BCJ compression(#240, #250)
+        
         `v0.9.8`_
         =========
         
         Changed
         -------
         
         * Avoid re-read header data from fike, otherwise calculate CRC32 when writing header.(#246)
@@ -1138,15 +1146,16 @@
         Changed
         -------
         
         * refactoring all the code.
         
         
         .. History links
-        .. _Unreleased: https://github.com/miurahr/py7zr/compare/v0.9.8...HEAD
+        .. _Unreleased: https://github.com/miurahr/py7zr/compare/v0.9.9...HEAD
+        .. _v0.9.9: https://github.com/miurahr/py7zr/compare/v0.9.8...v0.9.9
         .. _v0.9.8: https://github.com/miurahr/py7zr/compare/v0.9.7...v0.9.8
         .. _v0.9.7: https://github.com/miurahr/py7zr/compare/v0.9.6...v0.9.7
         .. _v0.9.6: https://github.com/miurahr/py7zr/compare/v0.9.5...v0.9.6
         .. _v0.9.5: https://github.com/miurahr/py7zr/compare/v0.9.4...v0.9.5
         .. _v0.9.4: https://github.com/miurahr/py7zr/compare/v0.9.3...v0.9.4
         .. _v0.9.3: https://github.com/miurahr/py7zr/compare/v0.9.2...v0.9.3
         .. _v0.9.2: https://github.com/miurahr/py7zr/compare/v0.9.1...v0.9.2
```

### Comparing `py7zr-0.9.8/py7zr.egg-info/SOURCES.txt` & `py7zr-0.9.9/py7zr.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -62,21 +62,23 @@
 tests/test_basic.py
 tests/test_benchmark.py
 tests/test_concurrent.py
 tests/test_encryption.py
 tests/test_extra_codecs.py
 tests/test_extract.py
 tests/test_info.py
+tests/test_misc.py
 tests/test_unit.py
 tests/test_win32compat.py
 tests/data/bcj.bin
 tests/data/bugzilla_4.7z
 tests/data/bzip2_2.7z
 tests/data/copy.7z
 tests/data/copy_2.7z
+tests/data/copy_bcj_1.7z
 tests/data/crc_corrupted.7z
 tests/data/deflate.7z
 tests/data/deflate64.7z
 tests/data/empty.7z
 tests/data/encrypted_1.7z
 tests/data/encrypted_2.7z
 tests/data/encrypted_3.7z
```

### Comparing `py7zr-0.9.8/setup.cfg` & `py7zr-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/__init__.py` & `py7zr-0.9.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/conftest.py` & `py7zr-0.9.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/bcj.bin` & `py7zr-0.9.9/tests/data/bcj.bin`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/bugzilla_4.7z` & `py7zr-0.9.9/tests/data/bugzilla_4.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/bzip2_2.7z` & `py7zr-0.9.9/tests/data/bzip2_2.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/copy_2.7z` & `py7zr-0.9.9/tests/data/copy_2.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/crc_corrupted.7z` & `py7zr-0.9.9/tests/data/crc_corrupted.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/encrypted_2.7z` & `py7zr-0.9.9/tests/data/encrypted_2.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/encrypted_3.7z` & `py7zr-0.9.9/tests/data/encrypted_3.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/encrypted_4.7z` & `py7zr-0.9.9/tests/data/encrypted_4.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/issue_218.7z` & `py7zr-0.9.9/tests/data/issue_218.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lib/aarch64-linux-gnu/liblzma.so.0` & `py7zr-0.9.9/tests/data/lib/aarch64-linux-gnu/liblzma.so.0`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lib/powerpc64le-linux-gnu/liblzma.so.0` & `py7zr-0.9.9/tests/data/lib/powerpc64le-linux-gnu/liblzma.so.0`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/longpath.7z` & `py7zr-0.9.9/tests/data/longpath.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lz4.7z` & `py7zr-0.9.9/tests/data/lz4.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma2_1.7z` & `py7zr-0.9.9/tests/data/lzma2_1.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma2bcj.7z` & `py7zr-0.9.9/tests/data/lzma2bcj.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma2bcj2.7z` & `py7zr-0.9.9/tests/data/lzma2bcj2.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma_bcj_arm.7z` & `py7zr-0.9.9/tests/data/lzma_bcj_arm.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma_bcj_armt.7z` & `py7zr-0.9.9/tests/data/lzma_bcj_armt.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma_bcj_ppc.7z` & `py7zr-0.9.9/tests/data/lzma_bcj_ppc.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma_bcj_sparc.7z` & `py7zr-0.9.9/tests/data/lzma_bcj_sparc.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/lzma_bcj_x86.7z` & `py7zr-0.9.9/tests/data/lzma_bcj_x86.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/mblock_1.7z` & `py7zr-0.9.9/tests/data/mblock_1.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/p7zip-zstd.7z` & `py7zr-0.9.9/tests/data/p7zip-zstd.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/symlink.7z` & `py7zr-0.9.9/tests/data/symlink.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/test_1.7z` & `py7zr-0.9.9/tests/data/test_1.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/test_2.7z` & `py7zr-0.9.9/tests/data/test_2.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/test_3.7z` & `py7zr-0.9.9/tests/data/test_3.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/test_6.7z` & `py7zr-0.9.9/tests/data/test_6.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/x86.bin` & `py7zr-0.9.9/tests/data/x86.bin`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/data/zstd.7z` & `py7zr-0.9.9/tests/data/zstd.7z`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_archive.py` & `py7zr-0.9.9/tests/test_archive.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_basic.py` & `py7zr-0.9.9/tests/test_basic.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_benchmark.py` & `py7zr-0.9.9/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_concurrent.py` & `py7zr-0.9.9/tests/test_concurrent.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_encryption.py` & `py7zr-0.9.9/tests/test_encryption.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_extra_codecs.py` & `py7zr-0.9.9/tests/test_extra_codecs.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_extract.py` & `py7zr-0.9.9/tests/test_extract.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_info.py` & `py7zr-0.9.9/tests/test_info.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_unit.py` & `py7zr-0.9.9/tests/test_unit.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tests/test_win32compat.py` & `py7zr-0.9.9/tests/test_win32compat.py`

 * *Files identical despite different names*

### Comparing `py7zr-0.9.8/tox.ini` & `py7zr-0.9.9/tox.ini`

 * *Files identical despite different names*

