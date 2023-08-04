# Comparing `tmp/gwdetchar-2.1.2.tar.gz` & `tmp/gwdetchar-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gwdetchar-2.1.2.tar", last modified: Fri Aug  4 18:21:26 2023, max compression
+gzip compressed data, was "gwdetchar-2.1.3.tar", last modified: Fri Aug  4 22:14:23 2023, max compression
```

## Comparing `gwdetchar-2.1.2.tar` & `gwdetchar-2.1.3.tar`

### file list

```diff
@@ -1,141 +1,141 @@
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.024246 gwdetchar-2.1.2/
--rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/.codecov.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/.flake8
--rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/.gitattributes
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.946317 gwdetchar-2.1.2/.github/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.961251 gwdetchar-2.1.2/.github/workflows/
--rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/.github/workflows/build.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/.github/workflows/docs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.1.2/.github/workflows/lint.yml
--rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/.gitignore
--rw-r--r--   0 egoetz     (501) staff       (20)      525 2023-06-28 17:53:22.000000 gwdetchar-2.1.2/.readthedocs.yml
--rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/CONTRIBUTING.md
--rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/LICENSE
--rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/MANIFEST.in
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 18:21:26.023736 gwdetchar-2.1.2/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/README.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.961965 gwdetchar-2.1.2/ci/
--rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/ci/test-cli.sh
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.964130 gwdetchar-2.1.2/docs/
--rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/Makefile
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.946886 gwdetchar-2.1.2/docs/_static/
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.964870 gwdetchar-2.1.2/docs/_static/css/
--rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/_static/css/custom.css
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.965452 gwdetchar-2.1.2/docs/api/
--rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/api/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/conf.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.966035 gwdetchar-2.1.2/docs/conlog/
--rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/conlog/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.966874 gwdetchar-2.1.2/docs/daq/
--rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/daq/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.967657 gwdetchar-2.1.2/docs/data/
--rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/data/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.968366 gwdetchar-2.1.2/docs/html/
--rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/html/index.rst
--rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.969025 gwdetchar-2.1.2/docs/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/lasso/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.969601 gwdetchar-2.1.2/docs/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/docs/nagios/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.970204 gwdetchar-2.1.2/docs/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/omega/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.970992 gwdetchar-2.1.2/docs/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/saturation/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.971668 gwdetchar-2.1.2/docs/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/docs/scattering/index.rst
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.980805 gwdetchar-2.1.2/gwdetchar/
--rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar/_version.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.2/gwdetchar/cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.2/gwdetchar/condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/conftest.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.2/gwdetchar/const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/daq.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.986868 gwdetchar-2.1.2/gwdetchar/io/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/io/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/gwdetchar/io/datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/io/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/gwdetchar/io/ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.990483 gwdetchar-2.1.2/gwdetchar/io/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/io/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/io/tests/test_datafind.py
--rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/io/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/gwdetchar/io/tests/test_ligolw.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.994512 gwdetchar-2.1.2/gwdetchar/lasso/
--rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    50279 2023-08-04 18:20:44.000000 gwdetchar-2.1.2/gwdetchar/lasso/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.2/gwdetchar/lasso/old.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.997247 gwdetchar-2.1.2/gwdetchar/lasso/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/lasso/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/mct.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.998922 gwdetchar-2.1.2/gwdetchar/nagios/
--rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.999883 gwdetchar-2.1.2/gwdetchar/nagios/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/nagios/tests/test_main.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.004146 gwdetchar-2.1.2/gwdetchar/omega/
--rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.1.2/gwdetchar/omega/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.2/gwdetchar/omega/batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/config.py
--rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.008335 gwdetchar-2.1.2/gwdetchar/omega/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_batch.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_config.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_html.py
--rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/omega/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/overflow.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/plot.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.010323 gwdetchar-2.1.2/gwdetchar/saturation/
--rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/core.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.011479 gwdetchar-2.1.2/gwdetchar/saturation/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/saturation/tests/test_saturation.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.014534 gwdetchar-2.1.2/gwdetchar/scattering/
--rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/__main__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.017710 gwdetchar-2.1.2/gwdetchar/scattering/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_core.py
--rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_main.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/scattering/tests/test_simple.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:26.022945 gwdetchar-2.1.2/gwdetchar/tests/
--rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/__init__.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_cds.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_cli.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.2/gwdetchar/tests/test_condor.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_conlog.py
--rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_const.py
--rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_daq.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_plot.py
--rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/tests/test_utils.py
--rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.2/gwdetchar/utils.py
-drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 18:21:25.984146 gwdetchar-2.1.2/gwdetchar.egg-info/
--rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/PKG-INFO
--rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/SOURCES.txt
--rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/dependency_links.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/entry_points.txt
--rw-r--r--   0 egoetz     (501) staff       (20)      348 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/requires.txt
--rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-08-04 18:21:25.000000 gwdetchar-2.1.2/gwdetchar.egg-info/top_level.txt
--rw-r--r--   0 egoetz     (501) staff       (20)     3457 2023-06-19 18:12:55.000000 gwdetchar-2.1.2/pyproject.toml
--rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-08-04 18:21:26.024377 gwdetchar-2.1.2/setup.cfg
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.508633 gwdetchar-2.1.3/
+-rw-r--r--   0 egoetz     (501) staff       (20)      184 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/.codecov.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      134 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/.flake8
+-rw-r--r--   0 egoetz     (501) staff       (20)       35 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/.gitattributes
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.440055 gwdetchar-2.1.3/.github/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.454956 gwdetchar-2.1.3/.github/workflows/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2885 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/.github/workflows/build.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1334 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/.github/workflows/docs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     1377 2023-06-28 17:53:22.000000 gwdetchar-2.1.3/.github/workflows/lint.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)      617 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/.gitignore
+-rw-r--r--   0 egoetz     (501) staff       (20)      525 2023-06-28 17:53:22.000000 gwdetchar-2.1.3/.readthedocs.yml
+-rw-r--r--   0 egoetz     (501) staff       (20)     2638 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/CONTRIBUTING.md
+-rw-r--r--   0 egoetz     (501) staff       (20)    35147 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/LICENSE
+-rw-r--r--   0 egoetz     (501) staff       (20)       69 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/MANIFEST.in
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 22:14:23.508179 gwdetchar-2.1.3/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2328 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/README.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.455667 gwdetchar-2.1.3/ci/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1135 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/ci/test-cli.sh
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.457642 gwdetchar-2.1.3/docs/
+-rw-r--r--   0 egoetz     (501) staff       (20)     6857 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/Makefile
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.440757 gwdetchar-2.1.3/docs/_static/
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.458463 gwdetchar-2.1.3/docs/_static/css/
+-rw-r--r--   0 egoetz     (501) staff       (20)     4997 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/_static/css/custom.css
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.458943 gwdetchar-2.1.3/docs/api/
+-rw-r--r--   0 egoetz     (501) staff       (20)       54 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/api/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)    10994 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/conf.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.459526 gwdetchar-2.1.3/docs/conlog/
+-rw-r--r--   0 egoetz     (501) staff       (20)      964 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/conlog/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.460354 gwdetchar-2.1.3/docs/daq/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1807 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/daq/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.460951 gwdetchar-2.1.3/docs/data/
+-rw-r--r--   0 egoetz     (501) staff       (20)      863 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/data/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.461486 gwdetchar-2.1.3/docs/html/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1488 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/html/index.rst
+-rw-r--r--   0 egoetz     (501) staff       (20)     2968 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.462069 gwdetchar-2.1.3/docs/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1439 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/lasso/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.462613 gwdetchar-2.1.3/docs/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      941 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/docs/nagios/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.463143 gwdetchar-2.1.3/docs/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3035 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/omega/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.463539 gwdetchar-2.1.3/docs/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1638 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/saturation/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.463922 gwdetchar-2.1.3/docs/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     2926 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/docs/scattering/index.rst
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.470661 gwdetchar-2.1.3/gwdetchar/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1408 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)      160 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar/_version.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3732 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4738 2023-05-16 23:56:26.000000 gwdetchar-2.1.3/gwdetchar/cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2773 2023-04-25 15:49:41.000000 gwdetchar-2.1.3/gwdetchar/condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2703 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/conftest.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7363 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2997 2023-05-17 00:05:55.000000 gwdetchar-2.1.3/gwdetchar/const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7440 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/daq.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.475402 gwdetchar-2.1.3/gwdetchar/io/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/io/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7584 2023-06-19 18:12:55.000000 gwdetchar-2.1.3/gwdetchar/io/datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    41413 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/io/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3764 2023-06-19 18:12:55.000000 gwdetchar-2.1.3/gwdetchar/io/ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.478542 gwdetchar-2.1.3/gwdetchar/io/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      827 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/io/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4834 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/io/tests/test_datafind.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    24146 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/io/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2451 2023-06-19 18:12:55.000000 gwdetchar-2.1.3/gwdetchar/io/tests/test_ligolw.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.483087 gwdetchar-2.1.3/gwdetchar/lasso/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1063 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    50279 2023-08-04 18:20:44.000000 gwdetchar-2.1.3/gwdetchar/lasso/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6652 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20595 2022-10-03 17:36:21.000000 gwdetchar-2.1.3/gwdetchar/lasso/old.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4946 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.486941 gwdetchar-2.1.3/gwdetchar/lasso/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3984 2023-04-27 00:53:55.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1549 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2142 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/lasso/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6744 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/mct.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.488297 gwdetchar-2.1.3/gwdetchar/nagios/
+-rw-r--r--   0 egoetz     (501) staff       (20)      887 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2959 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2166 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.489067 gwdetchar-2.1.3/gwdetchar/nagios/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2131 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/nagios/tests/test_main.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.492846 gwdetchar-2.1.3/gwdetchar/omega/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1188 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    14012 2023-08-04 18:20:44.000000 gwdetchar-2.1.3/gwdetchar/omega/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    12682 2023-05-16 23:56:26.000000 gwdetchar-2.1.3/gwdetchar/omega/batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    15875 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    10365 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    20699 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8871 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.496633 gwdetchar-2.1.3/gwdetchar/omega/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      830 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3689 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_batch.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6970 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_config.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5493 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13502 2023-06-16 22:43:20.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_html.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     9824 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2702 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/omega/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    17732 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/overflow.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2244 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/plot.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.498553 gwdetchar-2.1.3/gwdetchar/saturation/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1039 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    13870 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     7654 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/core.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.499333 gwdetchar-2.1.3/gwdetchar/saturation/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3510 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/saturation/tests/test_saturation.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.501452 gwdetchar-2.1.3/gwdetchar/scattering/
+-rw-r--r--   0 egoetz     (501) staff       (20)     1983 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)    32277 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/__main__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     6413 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5282 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     8523 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.503507 gwdetchar-2.1.3/gwdetchar/scattering/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      835 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2238 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_core.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     5520 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_main.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1831 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3156 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/scattering/tests/test_simple.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.507641 gwdetchar-2.1.3/gwdetchar/tests/
+-rw-r--r--   0 egoetz     (501) staff       (20)      826 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/__init__.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3276 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_cds.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3181 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_cli.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1918 2023-04-25 15:49:41.000000 gwdetchar-2.1.3/gwdetchar/tests/test_condor.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4819 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_conlog.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     1928 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_const.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     3306 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_daq.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2077 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_plot.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     2831 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/tests/test_utils.py
+-rw-r--r--   0 egoetz     (501) staff       (20)     4531 2022-08-23 18:11:03.000000 gwdetchar-2.1.3/gwdetchar/utils.py
+drwxr-xr-x   0 egoetz     (501) staff       (20)        0 2023-08-04 22:14:23.473016 gwdetchar-2.1.3/gwdetchar.egg-info/
+-rw-r--r--   0 egoetz     (501) staff       (20)     3726 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/PKG-INFO
+-rw-r--r--   0 egoetz     (501) staff       (20)     2832 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/SOURCES.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)        1 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/dependency_links.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      591 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/entry_points.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)      356 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/requires.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)       10 2023-08-04 22:14:23.000000 gwdetchar-2.1.3/gwdetchar.egg-info/top_level.txt
+-rw-r--r--   0 egoetz     (501) staff       (20)     3465 2023-08-04 22:13:43.000000 gwdetchar-2.1.3/pyproject.toml
+-rw-r--r--   0 egoetz     (501) staff       (20)       38 2023-08-04 22:14:23.508761 gwdetchar-2.1.3/setup.cfg
```

### Comparing `gwdetchar-2.1.2/.github/workflows/build.yml` & `gwdetchar-2.1.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/.github/workflows/docs.yml` & `gwdetchar-2.1.3/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/.github/workflows/lint.yml` & `gwdetchar-2.1.3/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/.gitignore` & `gwdetchar-2.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/.readthedocs.yml` & `gwdetchar-2.1.3/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/CONTRIBUTING.md` & `gwdetchar-2.1.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/LICENSE` & `gwdetchar-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/PKG-INFO` & `gwdetchar-2.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.2
+Version: 2.1.3
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.2/README.rst` & `gwdetchar-2.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/ci/test-cli.sh` & `gwdetchar-2.1.3/ci/test-cli.sh`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/Makefile` & `gwdetchar-2.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/_static/css/custom.css` & `gwdetchar-2.1.3/docs/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/conf.py` & `gwdetchar-2.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/conlog/index.rst` & `gwdetchar-2.1.3/docs/conlog/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/daq/index.rst` & `gwdetchar-2.1.3/docs/daq/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/data/index.rst` & `gwdetchar-2.1.3/docs/data/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/html/index.rst` & `gwdetchar-2.1.3/docs/html/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/index.rst` & `gwdetchar-2.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/lasso/index.rst` & `gwdetchar-2.1.3/docs/lasso/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/nagios/index.rst` & `gwdetchar-2.1.3/docs/nagios/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/omega/index.rst` & `gwdetchar-2.1.3/docs/omega/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/saturation/index.rst` & `gwdetchar-2.1.3/docs/saturation/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/docs/scattering/index.rst` & `gwdetchar-2.1.3/docs/scattering/index.rst`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/__init__.py` & `gwdetchar-2.1.3/gwdetchar/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/cds.py` & `gwdetchar-2.1.3/gwdetchar/cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/cli.py` & `gwdetchar-2.1.3/gwdetchar/cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/condor.py` & `gwdetchar-2.1.3/gwdetchar/condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/conftest.py` & `gwdetchar-2.1.3/gwdetchar/conftest.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/conlog.py` & `gwdetchar-2.1.3/gwdetchar/conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/const.py` & `gwdetchar-2.1.3/gwdetchar/const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/daq.py` & `gwdetchar-2.1.3/gwdetchar/daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/__init__.py` & `gwdetchar-2.1.3/gwdetchar/io/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/datafind.py` & `gwdetchar-2.1.3/gwdetchar/io/datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/html.py` & `gwdetchar-2.1.3/gwdetchar/io/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/ligolw.py` & `gwdetchar-2.1.3/gwdetchar/io/ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/io/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/tests/test_datafind.py` & `gwdetchar-2.1.3/gwdetchar/io/tests/test_datafind.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/tests/test_html.py` & `gwdetchar-2.1.3/gwdetchar/io/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/io/tests/test_ligolw.py` & `gwdetchar-2.1.3/gwdetchar/io/tests/test_ligolw.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/__init__.py` & `gwdetchar-2.1.3/gwdetchar/lasso/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/__main__.py` & `gwdetchar-2.1.3/gwdetchar/lasso/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/core.py` & `gwdetchar-2.1.3/gwdetchar/lasso/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/old.py` & `gwdetchar-2.1.3/gwdetchar/lasso/old.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/plot.py` & `gwdetchar-2.1.3/gwdetchar/lasso/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/lasso/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/tests/test_core.py` & `gwdetchar-2.1.3/gwdetchar/lasso/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/tests/test_main.py` & `gwdetchar-2.1.3/gwdetchar/lasso/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/lasso/tests/test_plot.py` & `gwdetchar-2.1.3/gwdetchar/lasso/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/mct.py` & `gwdetchar-2.1.3/gwdetchar/mct.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/nagios/__init__.py` & `gwdetchar-2.1.3/gwdetchar/nagios/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/nagios/__main__.py` & `gwdetchar-2.1.3/gwdetchar/nagios/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/nagios/core.py` & `gwdetchar-2.1.3/gwdetchar/nagios/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/nagios/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/nagios/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/nagios/tests/test_main.py` & `gwdetchar-2.1.3/gwdetchar/nagios/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/__init__.py` & `gwdetchar-2.1.3/gwdetchar/omega/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/__main__.py` & `gwdetchar-2.1.3/gwdetchar/omega/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/batch.py` & `gwdetchar-2.1.3/gwdetchar/omega/batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/config.py` & `gwdetchar-2.1.3/gwdetchar/omega/config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/core.py` & `gwdetchar-2.1.3/gwdetchar/omega/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/html.py` & `gwdetchar-2.1.3/gwdetchar/omega/html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/plot.py` & `gwdetchar-2.1.3/gwdetchar/omega/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/test_batch.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/test_batch.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/test_config.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/test_core.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/test_html.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/test_main.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/omega/tests/test_plot.py` & `gwdetchar-2.1.3/gwdetchar/omega/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/overflow.py` & `gwdetchar-2.1.3/gwdetchar/overflow.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/plot.py` & `gwdetchar-2.1.3/gwdetchar/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/saturation/__init__.py` & `gwdetchar-2.1.3/gwdetchar/saturation/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/saturation/__main__.py` & `gwdetchar-2.1.3/gwdetchar/saturation/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/saturation/core.py` & `gwdetchar-2.1.3/gwdetchar/saturation/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/saturation/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/saturation/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/saturation/tests/test_saturation.py` & `gwdetchar-2.1.3/gwdetchar/saturation/tests/test_saturation.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/__init__.py` & `gwdetchar-2.1.3/gwdetchar/scattering/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/__main__.py` & `gwdetchar-2.1.3/gwdetchar/scattering/__main__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/core.py` & `gwdetchar-2.1.3/gwdetchar/scattering/core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/plot.py` & `gwdetchar-2.1.3/gwdetchar/scattering/plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/simple.py` & `gwdetchar-2.1.3/gwdetchar/scattering/simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/scattering/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_core.py` & `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_main.py` & `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_plot.py` & `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/scattering/tests/test_simple.py` & `gwdetchar-2.1.3/gwdetchar/scattering/tests/test_simple.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/__init__.py` & `gwdetchar-2.1.3/gwdetchar/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_cds.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_cds.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_cli.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_condor.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_condor.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_conlog.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_conlog.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_const.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_const.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_daq.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_daq.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_plot.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/tests/test_utils.py` & `gwdetchar-2.1.3/gwdetchar/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar/utils.py` & `gwdetchar-2.1.3/gwdetchar/utils.py`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar.egg-info/PKG-INFO` & `gwdetchar-2.1.3/gwdetchar.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gwdetchar
-Version: 2.1.2
+Version: 2.1.3
 Summary: A python package for gravitational-wave detector characterisation
 Author-email: Alex Urban <alex.urban@ligo.org>, Duncan Macleod <duncan.macleod@ligo.org>
 Maintainer-email: Evan Goetz <evan.goetz@ligo.org>
 License: GPL-3.0-or-later
 Project-URL: Documentation, https://gwdetchar.readthedocs.io
 Project-URL: Source Code, https://github.com/gwdetchar/gwdetchar
 Project-URL: Bug Tracker, https://github.com/gwdetchar/gwdetchar/issues
```

### Comparing `gwdetchar-2.1.2/gwdetchar.egg-info/SOURCES.txt` & `gwdetchar-2.1.3/gwdetchar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/gwdetchar.egg-info/entry_points.txt` & `gwdetchar-2.1.3/gwdetchar.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `gwdetchar-2.1.2/pyproject.toml` & `gwdetchar-2.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,15 @@
   "gwdatafind",
   "gwpy >=3.0.0",
   "gwtrigfind",
   "lalsuite",
   "ligo-segments",
   "lxml",
   "MarkupPy >=1.14",
-  "matplotlib >=3.1.0",
+  "matplotlib >=3.1.0,<=3.7.1",
   "numpy >=1.16",
   "pandas",
   "pycondor",
   "pygments >=2.7.3",
   "python-ligo-lw",
   "pytz",
   "scikit-learn",
```

