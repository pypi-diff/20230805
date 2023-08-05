# Comparing `tmp/pysme-astro-0.4.99.tar.gz` & `tmp/pysme-astro-5.74.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysme-astro-0.4.99.tar", last modified: Thu Nov 18 13:17:28 2021, max compression
+gzip compressed data, was "dist/pysme-astro-5.74.9.tar", last modified: Thu Dec  3 10:59:28 2020, max compression
```

## Comparing `pysme-astro-0.4.99.tar` & `pysme-astro-5.74.9.tar`

### file list

```diff
@@ -1,72 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.477668 pysme-astro-0.4.99/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      298 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-11-18 13:17:28.477668 pysme-astro-0.4.99/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1652 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      174 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      227 2021-11-18 13:17:28.477668 pysme-astro-0.4.99/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3135 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.469668 pysme-astro-0.4.99/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.477668 pysme-astro-0.4.99/src/pysme/
--rw-r--r--   0 runner    (1001) docker     (121)     1373 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1546 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      498 2021-11-18 13:17:28.477668 pysme-astro-0.4.99/src/pysme/_version.py
--rw-r--r--   0 runner    (1001) docker     (121)    21508 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/abund.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.473668 pysme-astro-0.4.99/src/pysme/atmosphere/
--rw-r--r--   0 runner    (1001) docker     (121)      135 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/atmosphere/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10534 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/atmosphere/atmosphere.py
--rw-r--r--   0 runner    (1001) docker     (121)    37746 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/atmosphere/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/atmosphere/krzfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     7355 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/atmosphere/savfile.py
--rw-r--r--   0 runner    (1001) docker     (121)     8143 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/broadening.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/config.py
--rw-r--r--   0 runner    (1001) docker     (121)      381 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/config_default.json
--rw-r--r--   0 runner    (1001) docker     (121)    36661 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/continuum_and_radial_velocity.py
--rw-r--r--   0 runner    (1001) docker     (121)    27670 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/cwrapper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7082 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/data_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      917 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/datafiles_atmospheres.json
--rw-r--r--   0 runner    (1001) docker     (121)     3261 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/datafiles_nlte.json
--rw-r--r--   0 runner    (1001) docker     (121)     7918 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/echelle.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.473668 pysme-astro-0.4.99/src/pysme/gui/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      745 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/gui/plot_colors.py
--rw-r--r--   0 runner    (1001) docker     (121)    18939 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/gui/plot_plotly.py
--rw-r--r--   0 runner    (1001) docker     (121)     9529 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/gui/plot_pyplot.py
--rw-r--r--   0 runner    (1001) docker     (121)    11353 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/iliffe_vector.py
--rw-r--r--   0 runner    (1001) docker     (121)     7997 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/large_file_storage.py
--rw-r--r--   0 runner    (1001) docker     (121)     2789 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/libtools.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.473668 pysme-astro-0.4.99/src/pysme/linelist/
--rw-r--r--   0 runner    (1001) docker     (121)   397072 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/linelist/VALD3_ref.bib
--rw-r--r--   0 runner    (1001) docker     (121)      111 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/linelist/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2857 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/linelist/ges.py
--rw-r--r--   0 runner    (1001) docker     (121)    17287 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/linelist/linelist.py
--rw-r--r--   0 runner    (1001) docker     (121)    17666 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/linelist/vald.py
--rw-r--r--   0 runner    (1001) docker     (121)    41149 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/nlte.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/nso.py
--rw-r--r--   0 runner    (1001) docker     (121)    16382 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/persistence.py
--rw-r--r--   0 runner    (1001) docker     (121)    31173 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/sme.py
--rw-r--r--   0 runner    (1001) docker     (121)    26116 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/sme_synth.py
--rw-r--r--   0 runner    (1001) docker     (121)    29488 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/solve.py
--rw-r--r--   0 runner    (1001) docker     (121)    35357 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/synthesize.py
--rw-r--r--   0 runner    (1001) docker     (121)     3445 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (121)    11266 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/src/pysme/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.473668 pysme-astro-0.4.99/src/pysme_astro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2769 2021-11-18 13:17:28.000000 pysme-astro-0.4.99/src/pysme_astro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2021-11-18 13:17:28.000000 pysme-astro-0.4.99/src/pysme_astro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-18 13:17:28.000000 pysme-astro-0.4.99/src/pysme_astro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       71 2021-11-18 13:17:28.000000 pysme-astro-0.4.99/src/pysme_astro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2021-11-18 13:17:28.000000 pysme-astro-0.4.99/src/pysme_astro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-18 13:17:28.477668 pysme-astro-0.4.99/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4816 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_abund.py
--rw-r--r--   0 runner    (1001) docker     (121)     1773 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_atmospheres.py
--rw-r--r--   0 runner    (1001) docker     (121)     3715 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_continuum_and_rv.py
--rw-r--r--   0 runner    (1001) docker     (121)     4478 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_dll.py
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_largefilestorage.py
--rw-r--r--   0 runner    (1001) docker     (121)     4719 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_nlte.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_plotting.py
--rw-r--r--   0 runner    (1001) docker     (121)     3340 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_sme_structure.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_solver.py
--rw-r--r--   0 runner    (1001) docker     (121)     1412 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_synthesis.py
--rw-r--r--   0 runner    (1001) docker     (121)       52 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_uncertainties.py
--rw-r--r--   0 runner    (1001) docker     (121)     3427 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/test/test_vald.py
--rw-r--r--   0 runner    (1001) docker     (121)    68818 2021-11-18 13:15:07.000000 pysme-astro-0.4.99/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/
+-rw-r--r--   0 runner    (1001) docker     (116)      260 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     2771 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1654 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)      227 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)     3131 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.950674 pysme-astro-5.74.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/src/pysme/
+-rw-r--r--   0 runner    (1001) docker     (116)     1210 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      498 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/src/pysme/_version.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20771 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/abund.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.950674 pysme-astro-5.74.9/src/pysme/atmosphere/
+-rw-r--r--   0 runner    (1001) docker     (116)      111 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/atmosphere/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8308 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/atmosphere/atmosphere.py
+-rw-r--r--   0 runner    (1001) docker     (116)    37693 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/atmosphere/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3091 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/atmosphere/krzfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3770 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/atmosphere/savfile.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8089 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/broadening.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1098 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/config.py
+-rw-r--r--   0 runner    (1001) docker     (116)    25611 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/continuum_and_radial_velocity.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11215 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/cwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (116)     6703 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/data_structure.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2697 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/datafiles_atmospheres.json
+-rw-r--r--   0 runner    (1001) docker     (116)     7014 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/datafiles_nlte.json
+-rw-r--r--   0 runner    (1001) docker     (116)     7897 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/echelle.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.950674 pysme-astro-5.74.9/src/pysme/gui/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      497 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/gui/plot_colors.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15213 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/gui/plot_plotly.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9388 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/gui/plot_pyplot.py
+-rw-r--r--   0 runner    (1001) docker     (116)    12940 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/iliffe_vector.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10541 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/large_file_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/src/pysme/linelist/
+-rw-r--r--   0 runner    (1001) docker     (116)   224665 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/linelist/VALD3_ref.bib
+-rw-r--r--   0 runner    (1001) docker     (116)       87 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/linelist/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14693 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/linelist/linelist.py
+-rw-r--r--   0 runner    (1001) docker     (116)    17137 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/linelist/vald.py
+-rw-r--r--   0 runner    (1001) docker     (116)    38573 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/nlte.py
+-rw-r--r--   0 runner    (1001) docker     (116)    15209 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/persistence.py
+-rw-r--r--   0 runner    (1001) docker     (116)    29489 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/sme.py
+-rw-r--r--   0 runner    (1001) docker     (116)    24115 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/sme_synth.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23509 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/solve.py
+-rw-r--r--   0 runner    (1001) docker     (116)    28880 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/synthesize.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3420 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11251 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/src/pysme/util.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/src/pysme_astro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     2771 2020-12-03 10:59:28.000000 pysme-astro-5.74.9/src/pysme_astro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     1447 2020-12-03 10:59:28.000000 pysme-astro-5.74.9/src/pysme_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-03 10:59:28.000000 pysme-astro-5.74.9/src/pysme_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       80 2020-12-03 10:59:28.000000 pysme-astro-5.74.9/src/pysme_astro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        6 2020-12-03 10:59:28.000000 pysme-astro-5.74.9/src/pysme_astro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-03 10:59:28.954674 pysme-astro-5.74.9/test/
+-rw-r--r--   0 runner    (1001) docker     (116)     4811 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_abund.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1783 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_atmospheres.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2228 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_continuum_and_rv.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4468 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_dll.py
+-rw-r--r--   0 runner    (1001) docker     (116)      971 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_largefilestorage.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4770 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_nlte.py
+-rw-r--r--   0 runner    (1001) docker     (116)       84 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_plotting.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3322 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_sme_structure.py
+-rw-r--r--   0 runner    (1001) docker     (116)      956 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_solver.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1388 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_synthesis.py
+-rw-r--r--   0 runner    (1001) docker     (116)       29 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_uncertainties.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3439 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/test/test_vald.py
+-rw-r--r--   0 runner    (1001) docker     (116)    68751 2020-12-03 10:56:56.000000 pysme-astro-5.74.9/versioneer.py
```

### Comparing `pysme-astro-0.4.99/PKG-INFO` & `pysme-astro-5.74.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pysme-astro
-Version: 0.4.99
+Version: 5.74.9
 Summary: Spectroscopy Made Easy
 Home-page: https://github.com/AWehrhahn/SME/
 Author: Ansgar Wehrhahn, Jeff A. Valenti
 Author-email: ansgar.wehrhahn@physics.uu.se, valenti@stsci.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AWehrhahn/SME/issues
 Project-URL: Documentation, https://pysme-astro.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/AWehrhahn/SME/
-Description: ![Python application](https://github.com/AWehrhahn/SME/workflows/Python%20application/badge.svg)
+Description: [![Build Status](https://travis-ci.com/AWehrhahn/SME.svg?branch=master)](https://travis-ci.com/AWehrhahn/SME)
         [![Documentation Status](https://readthedocs.org/projects/pysme-astro/badge/?version=latest)](https://pysme-astro.readthedocs.io/en/latest/?badge=latest)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5547527.svg)](https://doi.org/10.5281/zenodo.5547527)
+        [![DOI](https://zenodo.org/badge/150097199.svg)](https://zenodo.org/badge/latestdoi/150097199)
         
         
         
         # PySME
         
         Spectroscopy Made Easy (SME) is a software tool that fits an observed
         spectrum of a star with a model spectrum. Since its initial release in
```

### Comparing `pysme-astro-0.4.99/README.md` & `pysme-astro-5.74.9/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-![Python application](https://github.com/AWehrhahn/SME/workflows/Python%20application/badge.svg)
+[![Build Status](https://travis-ci.com/AWehrhahn/SME.svg?branch=master)](https://travis-ci.com/AWehrhahn/SME)
 [![Documentation Status](https://readthedocs.org/projects/pysme-astro/badge/?version=latest)](https://pysme-astro.readthedocs.io/en/latest/?badge=latest)
-[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5547527.svg)](https://doi.org/10.5281/zenodo.5547527)
+[![DOI](https://zenodo.org/badge/150097199.svg)](https://zenodo.org/badge/latestdoi/150097199)
 
 
 
 # PySME
 
 Spectroscopy Made Easy (SME) is a software tool that fits an observed
 spectrum of a star with a model spectrum. Since its initial release in
```

### Comparing `pysme-astro-0.4.99/setup.py` & `pysme-astro-5.74.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 import json
 import os
 from os.path import dirname, exists, expanduser, join
 from shutil import copy
 
 from setuptools import setup
@@ -75,14 +74,15 @@
     python_requires=">=3.6",
     install_requires=[
         "numpy",
         "scipy",
         "astropy",
         "pandas",
         "wget",
+        "requests",
         "tqdm",
         "colorlog",
         "emcee",
         "pybtex",
         "flex-format",
     ],
     url="https://github.com/AWehrhahn/SME/",
```

### Comparing `pysme-astro-0.4.99/src/pysme/__init__.py` & `pysme-astro-5.74.9/src/pysme/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-# -*- coding: utf-8 -*-
 __file_ending__ = ".sme"
 
 # Load correct version string
 from ._version import get_versions
 
 __version__ = get_versions()["version"]
 del get_versions
 
 # Add output to the console
 import logging
-
 import colorlog
 import tqdm
 
 
 class TqdmLoggingHandler(logging.Handler):
     def __init__(self, level=logging.NOTSET):
         super().__init__(level)
@@ -35,21 +33,16 @@
 console = TqdmLoggingHandler()
 console.setLevel(logging.INFO)
 console.setFormatter(
     colorlog.ColoredFormatter("%(log_color)s%(levelname)s - %(message)s")
 )
 logger.addHandler(console)
 
-# Download library if it does not exist
-import os.path
-
-from . import libtools
-
-if not os.path.exists(libtools.get_full_libfile()):
-    libtools.download_libsme()
+del logging
+del colorlog
 
 # Provide submodules to the outside
 __all__ = [
     "util",
     "abund",
     "atmosphere",
     "broadening",
```

### Comparing `pysme-astro-0.4.99/src/pysme/abund.py` & `pysme-astro-5.74.9/src/pysme/abund.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-# -*- coding: utf-8 -*-
 """
 Elemental abundance data handling module
 """
 import io
 import json
 import logging
 
 import numpy as np
 from flex.extensions.bindata import BinaryDataExtension
-
 from .persistence import IPersist
 
+
 logger = logging.getLogger(__name__)
 
 _citation_asplund2009 = r"""
 @ARTICLE{2009ARA&A..47..481A,
     author = {{Asplund}, Martin and {Grevesse}, Nicolas and {Sauval}, A. Jacques and
     {Scott}, Pat},
     title = "{The Chemical Composition of the Sun}",
@@ -97,24 +96,24 @@
     "Bi", "Po", "At", "Rn", "Fr", "Ra", "Ac", "Th",
     "Pa", "U" , "Np", "Pu", "Am", "Cm", "Bk", "Cf",
     "Es",)
 
 # index of each element in the pattern data array
 elements_dict = {el:i for i, el in enumerate(elements)}
 
-# Array of atomic weights
-# From Loss, R. D. 2003, Pure Appl. Chem., 75, 1107, "Atomic Weights
-# of the Elements 2001". The isotopic composition of the Sun and stars
-# may differ from the terrestrial values listed here!
-# For radionuclides that appear only in Table 3, we have adopted the
-# atomic mass of the longest lived isotope, rounding to at most two
-# digits after the decimal point. These elements are: 43_Tc_98,
-# 61_Pm_145, 85_At_210, 86_Rn_222, 87_Fr_223, 88_Ra_226, 89_Ac_227,
-# 93_Np_237, 94_Pu_244, 95_Am_243, 96_Cm_247, 97_Bk_247, 98_Cf_251,
-# 99_Es_252
+""" Array of atomic weights
+From Loss, R. D. 2003, Pure Appl. Chem., 75, 1107, "Atomic Weights
+of the Elements 2001". The isotopic composition of the Sun and stars
+may differ from the terrestrial values listed here!
+For radionuclides that appear only in Table 3, we have adopted the
+atomic mass of the longest lived isotope, rounding to at most two
+digits after the decimal point. These elements are: 43_Tc_98,
+61_Pm_145, 85_At_210, 86_Rn_222, 87_Fr_223, 88_Ra_226, 89_Ac_227,
+93_Np_237, 94_Pu_244, 95_Am_243, 96_Cm_247, 97_Bk_247, 98_Cf_251,
+99_Es_252 """
 
 _atom_weight = (
     1.00794, 4.002602,
     6.941, 9.012182, 10.811, 12.0107, 14.0067, 15.9994, 18.9984032, 20.1797,
     22.989770, 24.3050, 26.981538, 28.0855, 30.973761, 32.065, 35.453, 39.948,
     39.0983, 40.078, 44.955910, 47.867, 50.9415, 51.9961, 54.938049, 55.845,
     58.933200, 58.6934, 63.546, 65.409, 69.723, 72.64, 74.92160, 78.96,
@@ -124,16 +123,17 @@
     138.9055, 140.116, 140.90765, 144.24, 144.91, 150.36, 151.964, 157.25,
     158.92534, 162.500, 164.93032, 167.259, 168.93421, 173.04, 174.967, 178.49,
     180.9479, 183.84, 186.207, 190.23, 192.217, 195.078, 196.966, 200.59,
     204.3833, 207.2, 208.98038, 209.99, 222.02, 223.02, 226.03, 227.03,
     232.0381, 231.03588, 238.02891, 237.05, 244.06, 243.06, 247.07, 247.07,
     251.08, 252.08,)
 
-# Asplund, Grevesse, Sauval, Scott (2009,  Annual Review of Astronomy
-# and Astrophysics, 47, 481)
+"""Asplund, Grevesse, Sauval, Scott (2009,  Annual Review of Astronomy
+and Astrophysics, 47, 481)
+"""
 _asplund2009 = (
     12.00, 10.93,
     1.05, 1.38, 2.70, 8.43, 7.83, 8.69, 4.56,  7.93,
     6.24,  7.60,  6.45,  7.51,  5.41,  7.12,  5.50,  6.40,
     5.03,  6.34,  3.15,  4.95,  3.93,  5.64,  5.43,  7.50,
     4.99,  6.22,  4.19,  4.56,  3.04,  3.65,  2.30,  3.34,
     2.54,  3.25,  2.52,  2.87,  2.21,  2.58,  1.46,  1.88,
@@ -142,15 +142,16 @@
     0.72,  1.42,  None,  0.96,  0.52,  1.07,  0.30,  1.10,
     0.48,  0.92,  0.10,  0.84,  0.10,  0.85,  -0.12,  0.85,
     0.26,  1.40,  1.38,  1.62,  0.92,  1.17,  0.90,  1.75,
     0.65,  None,  None,  None,  None,  None,  None,  0.02,
     None,  -0.54,  None,  None,  None,  None,  None,  None,
     None,)
 
-# Grevesse, Asplund, Sauval (2007, Space Science Review, 130, 105)
+"""Grevesse, Asplund, Sauval (2007, Space Science Review, 130, 105)
+"""
 _grevesse2007 = (
     12.00, 10.93,
     1.05, 1.38, 2.70, 8.39, 7.78, 8.66, 4.56, 7.84,
     6.17, 7.53, 6.37, 7.51, 5.36, 7.14, 5.50, 6.18,
     5.08, 6.31, 3.17, 4.90, 4.00, 5.64, 5.39, 7.45,
     4.92, 6.23, 4.21, 4.60, 2.88, 3.58, 2.29, 3.33,
     2.56, 3.25, 2.60, 2.92, 2.21, 2.58, 1.42, 1.92,
@@ -159,15 +160,15 @@
     0.58, 1.45, None, 1.00, 0.52, 1.11, 0.28, 1.14,
     0.51, 0.93, 0.00, 1.08, 0.06, 0.88, -0.17, 1.11,
     0.23, 1.25, 1.38, 1.64, 1.01, 1.13, 0.90, 2.00,
     0.65, None, None, None, None, None, None, 0.06,
     None, -0.52, None, None, None, None, None, None,
     None,)
 
-# Lodders 2003 (ApJ, 591, 1220)
+""" Lodders 2003 (ApJ, 591, 1220) """
 _lodders2003 = (
     12, 10.899,
     3.28, 1.41, 2.78, 8.39, 7.83, 8.69, 4.46, 7.87,
     6.30, 7.55, 6.46, 7.54, 5.46, 7.19, 5.26, 6.55,
     5.11, 6.34, 3.07, 4.92, 4.00, 5.65, 5.50, 7.47,
     4.91, 6.22, 4.26, 4.63, 3.10, 3.62, 2.32, 3.36,
     2.59, 3.28, 2.36, 2.91, 2.20, 2.60, 1.42, 1.96,
@@ -230,15 +231,15 @@
         """Return abundances for all elements.
         Apply current [M/H] value to the current abundance pattern.
         Transform the resulting abundances to the requested abundance type.
         """
         pattern = np.copy(self._pattern)
         if self.monh is not None:
             pattern[2:] += self.monh
-        return self.totype(pattern, type, raw=raw, copy=False)
+        return self.totype(pattern, type, raw=raw)
 
     def __getitem__(self, elem):
         return self.get_element(elem)
 
     def __setitem__(self, elem, abund):
         self.update_pattern({elem: abund})
 
@@ -271,39 +272,23 @@
 
     def __repr__(self):
         return self.__str__()
 
     # These are there for the atmosphere interpolation
     # The internal format is always H=12, so that should be fine
     def __add__(self, other):
-        result = Abund(
-            monh=self.monh, pattern=np.copy(self._pattern), type=self._type_internal
-        )
         if isinstance(other, Abund):
-            result._pattern += other.get_pattern(self._type_internal, raw=True)
-            result.monh += other.monh
+            self._pattern += other._pattern
         else:
-            raise NotImplementedError
-        result.type = self.type
-        return result
-
-    def __radd__(self, other):
-        return self.__add__(other)
+            self._pattern += other
+        return self
 
     def __mul__(self, other):
-        result = Abund(
-            monh=self.monh, pattern=np.copy(self._pattern), type=self._type_internal
-        )
-        if isinstance(other, Abund):
-            raise NotImplementedError
-        else:
-            result._pattern *= other
-            result.monh *= other
-        result.type = self.type
-        return result
+        self._pattern *= other
+        return self
 
     def __rmul__(self, other):
         return self.__mul__(other)
 
     def _get_index(self, elem):
         try:
             return elements_dict[elem]
@@ -363,26 +348,24 @@
             )
         if raw:
             return abund
         else:
             return {el: abund[elements_dict[el]] for el in elements}
 
     @staticmethod
-    def totype(pattern, totype, raw=False, copy=True):
+    def totype(pattern, totype, raw=False):
         """Return a copy of the input abundance pattern, transformed from
         the 'H=12' type to the output type. Valid abundance pattern types
         are 'sme', 'n/nTot', 'n/nH', and 'H=12'.
         """
         if isinstance(pattern, dict):
             abund = [pattern[el] if el in pattern.keys() else np.nan for el in elements]
             abund = np.array(abund)
-        elif copy:
-            abund = np.copy(pattern)
         else:
-            abund = pattern
+            abund = np.copy(pattern)
 
         type = totype.lower()
 
         if type == "h=12":
             pass
         elif type == "sme":
             abund2 = 10 ** (abund - 12)
@@ -422,15 +405,15 @@
         """Return the standard abbreviation for each element.
         Use property so user will not redefine elements.
         """
         return elements
 
     @property
     def elem_dict(self):
-        """Return the position of each element in the raw array"""
+        """ Return the position of each element in the raw array """
         return elements_dict
 
     @property
     def monh(self):
         """float: Metallicity, the logarithmic offset added to
         the abundance pattern for all elements except hydrogen and helium."""
         return self._monh
@@ -526,15 +509,16 @@
         if type is None:
             type = self.type
         pattern = self(type, raw=True)
         i = self._get_index(elem)
         return pattern[i]
 
     def empty_pattern(self):
-        """Return an abundance pattern with value None for all elements."""
+        """Return an abundance pattern with value None for all elements.
+        """
         pattern = np.full(len(elements), np.nan)
         pattern[0] = 0
         return pattern
 
     def _save(self):
         header = {
             "monh": self.monh,
@@ -555,51 +539,44 @@
             pattern=pattern,
             type=header["type"],
             citation_info=header["citation_info"],
         )
         return abund
 
     def _save_v1(self, file, folder="abund"):
-        """Save the data to a file handler"""
+        """ Save the data to a file handler """
         if folder != "" or folder[-1] != "/":
             folder += "/"
 
         monh = float(self.monh) if self.monh is not None else None
-        info = {
-            "format": self.type,
-            "monh": monh,
-            "citation_info": self.citation_info,
-        }
+        info = {"format": self.type, "monh": monh, "citation_info": self.citation_info}
         file.writestr(f"{folder}info.json", json.dumps(info))
 
         b = io.BytesIO()
         np.save(b, self.get_pattern(raw=True))
         file.writestr(f"{folder}pattern.npy", b.getvalue())
 
     @staticmethod
     def _load_v1(file, names, folder=""):
-        """Load the data from a file handler"""
+        """ Load the data from a file handler """
         for name in names:
             if name.endswith("info.json"):
                 info = file.read(name)
                 info = json.loads(info)
 
                 abund_format = info["format"]
                 monh = info["monh"]
                 citation_info = info.get("citation_info", _citation_atomic_weights)
 
             elif name.endswith("pattern.npy"):
                 b = io.BytesIO(file.read(name))
                 pattern = np.load(b)
 
         return Abund(
-            monh=monh,
-            pattern=pattern,
-            type=abund_format,
-            citation_info=citation_info,
+            monh=monh, pattern=pattern, type=abund_format, citation_info=citation_info
         )
 
     @staticmethod
     def solar():
-        """Return solar abundances of asplund 2009"""
+        """ Return solar abundances of asplund 2009 """
         solar = Abund(pattern="solar", monh=0)
         return solar
```

### Comparing `pysme-astro-0.4.99/src/pysme/atmosphere/atmosphere.py` & `pysme-astro-5.74.9/src/pysme/atmosphere/atmosphere.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# -*- coding: utf-8 -*-
 """ Handles reading and interpolation of atmopshere (grid) data """
 import logging
 
 import numpy as np
+
 from flex.extensions.bindata import MultipleDataExtension
 
-from ..abund import Abund
 from ..data_structure import (
-    Collection,
     CollectionFactory,
+    Collection,
     absolute,
-    array,
+    this,
     asfloat,
     asstr,
     lowercase,
-    oneof,
-    this,
     uppercase,
+    oneof,
+    array,
 )
+from ..abund import Abund
 
 logger = logging.getLogger(__name__)
 
 
 class AtmosphereError(RuntimeError):
-    """Something went wrong with the atmosphere interpolation"""
+    """ Something went wrong with the atmosphere interpolation """
 
 
 @CollectionFactory
 class Atmosphere(Collection):
     """
     Atmosphere structure
     contains all information to describe the solar atmosphere
@@ -38,22 +38,22 @@
     # fmt: off
     _fields = [
         ("teff", 5770, asfloat, this, "float: effective temperature in Kelvin"),
         ("logg", 4.0, asfloat, this, "float: surface gravity in log10(cgs)"),
         ("abund", Abund.solar(), this, this, "Abund: elemental abundances"),
         ("vturb", 0, absolute, this, "float: turbulence velocity in km/s"),
         ("lonh", 0, asfloat, this, "float: ?"),
-        ("source", "marcs2014.sav", this, this, "str: datafile name of this data, or atmosphere grid/file"),
-        ("method", "grid", lowercase(oneof("grid", "embedded")), this,
+        ("source", None, asstr, this, "str: datafile name of this data"),
+        ("method", "grid", lowercase(oneof("grid", "embedded")), this, 
             "str: whether the data source is a grid or a fixed atmosphere"),
         ("geom", "PP", uppercase(oneof("PP", "SPH", None)), this,
             "str: the geometry of the atmopshere model"),
         ("radius", 0, asfloat, this, "float: radius of the spherical model"),
         ("height", None, array(None, "f8"), this, "array: height of the spherical model"),
-        ("opflag", [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1], array(20, int), this,
+        ("opflag", [1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 1, 0, 1, 0, 0, 0, 0, 0], array(20, int), this,
             "array of size (20,): opacity flags"),
         ("wlstd", 5000, asfloat, this, "float: wavelength standard deviation"),
         ("depth", None, uppercase(oneof(None, "RHOX", "TAU")), this,
             "str: flag that determines whether to use RHOX or TAU for calculations"),
         ("interp", None, uppercase(oneof(None, "RHOX", "TAU")), this,
             "str: flag that determines whether to use RHOX or TAU for interpolation"),
         ("rhox", None, array(None, "f8"), this,
@@ -69,20 +69,19 @@
         ("xne", None, array(None, "f8"), this,
             "array: number density of electrons in 1/cm**3"),
         ("citation_info", "", asstr, this, "str: citation for this atmosphere"),
     ]
     # fmt: on
 
     # TODO: pick the right geometry for the grid, based on whether it has height/radius values or not
-    def __init__(self, *args, **kwargs):
+
+    def __init__(self, **kwargs):
         monh = kwargs.pop("monh", kwargs.pop("feh", 0))
         abund = kwargs.pop("abund", "empty")
         abund_format = kwargs.pop("abund_format", "sme")
-        if "geom" in kwargs.keys() and kwargs["geom"] == "":
-            kwargs["geom"] = None
         super().__init__(**kwargs)
         self.abund = Abund(monh=monh, pattern=abund, type=abund_format)
 
     @property
     def monh(self):
         """float: metallicity"""
         return self.abund.monh
@@ -150,15 +149,15 @@
     of model atmospheres. Each entry represents one
     atmosphere model.
     """
 
     # fmt: off
     _fields = [
         ("source", None, asstr, this, "str: datafile name of this data"),
-        ("method", "grid", lowercase(oneof("grid", "embedded")), this,
+        ("method", "grid", lowercase(oneof("grid", "embedded")), this, 
             "str: whether the data source is a grid or a fixed atmosphere"),
         ("geom", None, uppercase(oneof(None, "PP", "SPH")), this,
             "str: the geometry of the atmopshere model"),
         ("depth", None, uppercase(oneof(None, "RHOX", "TAU")), this,
             "str: flag that determines whether to use RHOX or TAU for calculations"),
         ("interp", None, uppercase(oneof(None, "RHOX", "TAU")), this,
             "str: flag that determines whether to use RHOX or TAU for interpolation"),
@@ -187,122 +186,57 @@
             ("xna", f"({npoints},)f4"),
             ("xne", f"({npoints},)f4"),
         ]
 
         names = [s[0].lower() for s in dtype]
         titles = [s[0].upper() for s in dtype]
 
-        data = super().__new__(cls, (natmo,), dtype=dtype, names=names, titles=titles)
+        atmo_grid = np.recarray(natmo, dtype=dtype, names=names, titles=titles)
 
+        data = atmo_grid.view(cls)
         data.interp = "TAU"
         data.depth = "RHOX"
         data.method = "grid"
         data.geom = "PP"
         data.source = ""
         data.citation_info = ""
         data.abund_format = "sme"
-        data.info = ""
         return data
 
     def __array_finalize__(self, obj):
         if obj is None:
             return
-        self.interp = getattr(obj, "interp", "TAU")
-        self.depth = getattr(obj, "depth", "RHOX")
-        self.method = getattr(obj, "method", "grid")
-        self.geom = getattr(obj, "geom", "PP")
-        self.source = getattr(obj, "source", "")
-        self.citation_info = getattr(obj, "citation_info", "")
-        self.abund_format = getattr(obj, "abund_format", "sme")
-        self.info = getattr(obj, "info", "")
-
-    def __reduce__(self):
-        # Get the parent's __reduce__ tuple
-        pickled_state = super(AtmosphereGrid, self).__reduce__()
-        # Create our own tuple to pass to __setstate__
-        new_state = pickled_state[2] + (
-            self.interp,
-            self.depth,
-            self.source,
-            self.geom,
-            self.citation_info,
-            self.method,
-            self.abund_format,
-            self.info,
-        )
-        # Return a tuple that replaces the parent's __setstate__ tuple with our own
-        return (pickled_state[0], pickled_state[1], new_state)
-
-    def __setstate__(self, state):
-        self.interp = state[-8]
-        self.depth = state[-7]
-        self.source = state[-6]
-        self.geom = state[-5]
-        self.citation_info = state[-4]
-        self.method = state[-3]
-        self.abund_format = state[-2]
-        self.info = state[-1]
-
-        # Call the parent's __setstate__ with the other tuple elements.
-        super(AtmosphereGrid, self).__setstate__(state[0:-8])
+        self.interp = getattr(self, "interp", "TAU")
+        self.depth = getattr(self, "depth", "RHOX")
+        self.source = getattr(self, "source", "")
+        self.geom = getattr(self, "geom", "PP")
+        self.citation_info = getattr(self, "citation_info", "")
+        self.method = getattr(self, "method", "grid")
+        self.abund_format = getattr(self, "abund_format", "sme")
+        self.wlstd = getattr(self, "wlstd", 5000)
 
     def __getitem__(self, key):
-        """Overwrite the getitem routine, so we keep additional
+        """ Overwrite the getitem routine, so we keep additional
         properties and/or return an atmosphere object, when only
-        one record is returned"""
-        cls = self.__class__
+        one record is returned """
+        cls = type(self)
         value = super().__getitem__(key)
         if isinstance(value, cls) and value.size == 1:
             return value[0]
 
         if isinstance(value, np.record):
             kwargs = {s: value[s] for s in value.dtype.names}
             value = Atmosphere(**kwargs)
         if isinstance(value, (Atmosphere, cls)):
             for name in self._names:
                 setattr(value, name, getattr(self, name))
         return value
 
-    def __str__(self):
-        return self.source
-
-    def __repr__(self):
-        return str(self)
-
     def get(self, teff, logg, monh):
         mask = self.teff == teff
         mask &= self.logg == logg
         mask &= self.monh == monh
         return self[mask]
 
     @property
     def ndep(self):
         return self.shape[1]
-
-    def save(self, filename):
-        """Save the Atmopshere grid to a file using a numpy save format"""
-        header = {
-            "interp": self.interp,
-            "depth": self.depth,
-            "source": self.source,
-            "geom": self.geom,
-            "citation_info": self.citation_info,
-            "method": self.method,
-            "abund_format": self.abund_format,
-            "info": self.info,
-        }
-        names = list(header.keys())
-        values = [header[n] for n in names]
-        header = np.rec.array(values, names=names)
-        np.savez(filename, data=self, header=header)
-        return
-
-    @classmethod
-    def load(cls, filename):
-        """Load the atmosphere grid data from disk"""
-        data = np.load(filename)
-        self = data["data"].view(cls)
-        header = data["header"]
-        for k in header.dtype.names:
-            v = header[k][()]
-            setattr(self, k, v)
-        return self
```

### Comparing `pysme-astro-0.4.99/src/pysme/atmosphere/interpolation.py` & `pysme-astro-5.74.9/src/pysme/atmosphere/interpolation.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
 """ Handles reading and interpolation of atmopshere (grid) data """
 import itertools
 import logging
 
 import numpy as np
-from astropy import constants as const
 from scipy.interpolate import interp1d
 from scipy.optimize import curve_fit
 
-from ..large_file_storage import setup_atmo
-from .atmosphere import Atmosphere as Atmo
-from .atmosphere import AtmosphereError, AtmosphereGrid
+from astropy import constants as const
+
+from .atmosphere import Atmosphere as Atmo, AtmosphereError, AtmosphereGrid
 from .savfile import SavFile
+from ..large_file_storage import setup_atmo
 
 logger = logging.getLogger(__name__)
 
 # Radius and Surface Gravity of the Sun
 # Required for spherical models
 R_sun = const.R_sun.to_value("cm")
 g_sun = (const.G * const.M_sun / const.R_sun ** 2).to_value("cm/s**2")
@@ -63,17 +62,15 @@
         """
 
         # Internal parameters.
         if not isinstance(atmo_grid, AtmosphereGrid):
             if self.atmo_grid is None or self.source != atmo_grid:
                 atmo_file = self.lfs_atmo.get(atmo_grid)
                 self.source = atmo_grid
-                self.atmo_grid = SavFile(
-                    atmo_file, source=self.source, lfs=self.lfs_atmo
-                )
+                self.atmo_grid = SavFile(atmo_file)
         else:
             self.atmo_grid = atmo_grid
             self.source = atmo_grid.source
 
         if self.geom is not None:
             if self.geom == "PP":
                 atmo_grid = self.atmo_grid[self.atmo_grid.radius <= 1]
@@ -101,17 +98,15 @@
             if self.geom == "SPH":
                 raise AtmosphereError(
                     "Input ATMO.GEOM='%s' was requested but the model only supports PP (at this point)."
                     % self.geom
                 )
             else:
                 logger.info(
-                    "Input ATMO.GEOM='%s' overrides '%s' from grid.",
-                    self.geom,
-                    geom,
+                    "Input ATMO.GEOM='%s' overrides '%s' from grid.", self.geom, geom,
                 )
 
         # Add standard ATMO input fields, if they are missing from ATMO_IN.
         atmo.depth = depth
         atmo.interp = interp
         atmo.geom = geom
         if radius is not None:
@@ -123,26 +118,25 @@
 
     def interp_atmo_pair(self, atmo1, atmo2, frac, interpvar="RHOX", itop=0):
         """
         Interpolate between two model atmospheres, accounting for shifts in
         the mass column density or optical depth scale.
 
         How it works:
-
-        1. The second atmosphere is fitted onto the first, individually for
+        1) The second atmosphere is fitted onto the first, individually for
         each of the four atmospheric quantitites: T, xne, xna, rho.
         The fitting uses a linear shift in both the (log) depth parameter and
         in the (log) atmospheric quantity. For T, the midpoint of the two
         atmospheres is aligned for the initial guess. The result of this fit
         is used as initial guess for the other quantities. A penalty function
         is applied to each fit, to avoid excessively large shifts on the
         depth scale.
-        2. The mean of the horizontal shift in each parameter is used to
+        2) The mean of the horizontal shift in each parameter is used to
         construct the common output depth scale.
-        3. Each atmospheric quantity is interpolated after shifting the two
+        3) Each atmospheric quantity is interpolated after shifting the two
         corner models by the amount determined in step 1), rescaled by the
         interpolation fraction (frac).
 
         Parameters
         ------
         atmo1 : Atmosphere
             first atmosphere to interpolate
@@ -174,59 +168,59 @@
             .RHOX (vector[ndep]) mass column density (g/cm^2)
             .TAU  (vector[ndep]) reference optical depth (at 5000 Å)
             .temp (vector[ndep]) temperature (K)
             .xne  (vector[ndep]) electron number density (1/cm^3)
             .xna  (vector[ndep]) atomic number density (1/cm^3)
             .rho  (vector[ndep]) mass density (g/cm^3)
         """
-        # """
-        # History
-        # -------
-        # 2004-Apr-15 Valenti
-        #     Initial coding.
-        # MB
-        #     interpolation on TAU scale
-        # 2012-Oct-30 TN
-        #     Rewritten to use either column mass (RHOX) or
-        #     reference optical depth (TAU) as vertical scale. Shift-interpolation
-        #     algorithms have been improved for stability in cool dwarfs (<=3500 K).
-        #     The reference optical depth scale is preferred in terms of interpolation
-        #     accuracy across most of parameter space, with significant improvement for
-        #     both cool models (where depth vs temperature is rather flat) and hot
-        #     models (where depth vs temperature exhibits steep transitions).
-        #     Column mass depth is used by default for backward compatibility.
-        # 2013-May-17 Valenti
-        #     Use frac to weight the two shifted depth scales,
-        #     rather than simply averaging them. This change fixes discontinuities
-        #     when crossing grid nodes.
-        # 2013-Sep-10 Valenti
-        #     Now returns an atmosphere structure instead of a
-        #     [5,NDEP] atmosphere array. This was necessary to support interpolation
-        #     using one variable (e.g., TAU) and radiative transfer using a different
-        #     variable (e.g. RHOX). The atmosphere array could only store one depth
-        #     variable, meaning the radiative transfer variable had to be the same
-        #     as the interpolation variable. Returns atmo.RHOX if available and also
-        #     atmo.TAU if available. Since both depth variables are returned, if
-        #     available, this routine no longer needs to know which depth variable
-        #     will be used for radiative transfer. Only the interpolation variable
-        #     is important. Thus, the interpvar= keyword argument replaces the
-        #     type= keyword argument. Very similar code blocks for each atmospheric
-        #     quantity have been unified into a single code block inside a loop over
-        #     atmospheric quantities.
-        # 2013-Sep-21 Valenti
-        #     Fixed an indexing bug that affected the output depth
-        #     scale but not other atmosphere vectors. Itop clipping was not being
-        #     applied to the depth scale ('RHOX' or 'TAU'). Bug fixed by adding
-        #     interpvar to vtags. Now atmospheres interpolated with interp_atmo_grid
-        #     match output from revision 398. Revisions back to 399 were development
-        #     only, so no users should be affected.
-        # 2014-Mar-05 Piskunov
-        #     Replicated the removal of the bad top layers in models
-        #     for interpvar eq 'TAU'
-        # """
+        """
+        History
+        -------
+        2004-Apr-15 Valenti
+            Initial coding.
+        MB
+            interpolation on TAU scale
+        2012-Oct-30 TN
+            Rewritten to use either column mass (RHOX) or
+            reference optical depth (TAU) as vertical scale. Shift-interpolation
+            algorithms have been improved for stability in cool dwarfs (<=3500 K).
+            The reference optical depth scale is preferred in terms of interpolation
+            accuracy across most of parameter space, with significant improvement for
+            both cool models (where depth vs temperature is rather flat) and hot
+            models (where depth vs temperature exhibits steep transitions).
+            Column mass depth is used by default for backward compatibility.
+        2013-May-17 Valenti
+            Use frac to weight the two shifted depth scales,
+            rather than simply averaging them. This change fixes discontinuities
+            when crossing grid nodes.
+        2013-Sep-10 Valenti
+            Now returns an atmosphere structure instead of a
+            [5,NDEP] atmosphere array. This was necessary to support interpolation
+            using one variable (e.g., TAU) and radiative transfer using a different
+            variable (e.g. RHOX). The atmosphere array could only store one depth
+            variable, meaning the radiative transfer variable had to be the same
+            as the interpolation variable. Returns atmo.RHOX if available and also
+            atmo.TAU if available. Since both depth variables are returned, if
+            available, this routine no longer needs to know which depth variable
+            will be used for radiative transfer. Only the interpolation variable
+            is important. Thus, the interpvar= keyword argument replaces the
+            type= keyword argument. Very similar code blocks for each atmospheric
+            quantity have been unified into a single code block inside a loop over
+            atmospheric quantities.
+        2013-Sep-21 Valenti
+            Fixed an indexing bug that affected the output depth
+            scale but not other atmosphere vectors. Itop clipping was not being
+            applied to the depth scale ('RHOX' or 'TAU'). Bug fixed by adding
+            interpvar to vtags. Now atmospheres interpolated with interp_atmo_grid
+            match output from revision 398. Revisions back to 399 were development
+            only, so no users should be affected.
+        2014-Mar-05 Piskunov
+            Replicated the removal of the bad top layers in models
+            for interpvar eq 'TAU'
+        """
 
         # Internal program parameters.
         min_drhox = min_dtau = 0.01  # minimum fractional step in RHOX
         # min_dtau = 0.01  # minimum fractional step in TAU
         interpvar = interpvar.lower()
         ##
         ## Select interpolation variable (RHOX vs. TAU)
@@ -453,20 +447,18 @@
             # Create or add to output structure.
             atmo[tag] = value
         return atmo
 
     def determine_depth_scale(self, depth, atmo_grid):
         """
         Determine ATMO.DEPTH radiative transfer depth variable. Order of precedence:
-
-        1. Value of ATMO_IN.DEPTH, if it exists and is set
-        2. Value of ATMO_GRID[0].DEPTH, if it exists and is set
-        3. 'RHOX', if ATMO_GRID.RHOX exists (preferred over 'TAU' for depth)
-        4. 'TAU', if ATMO_GRID.TAU exists
-
+            1. Value of ATMO_IN.DEPTH, if it exists and is set
+            2. Value of ATMO_GRID[0].DEPTH, if it exists and is set
+            3. 'RHOX', if ATMO_GRID.RHOX exists (preferred over 'TAU' for depth)
+            4. 'TAU', if ATMO_GRID.TAU exists
         Check that INTERP is valid and the corresponding field exists in ATMO.
 
         Parameters
         ----------
         depth : {"RHOX", "TAU", None}
             requested value, or None for autoselection based in available grid
         atmo_grid : AtmosphereGrid
@@ -497,27 +489,25 @@
             raise AtmosphereError("no value for ATMO.DEPTH")
         if depth != "TAU" and depth != "RHOX":
             raise AtmosphereError(
                 "ATMO.DEPTH must be 'TAU' or 'RHOX', not '%s'" % depth
             )
         if depth.lower() not in gtags:
             raise AtmosphereError(
-                "ATMO.DEPTH='{}', but ATMO. {} does not exist".format(depth, depth)
+                "ATMO.DEPTH='%s', but ATMO. %s does not exist" % (depth, depth)
             )
         return depth
 
     def determine_interpolation_scale(self, interp, atmo_grid):
         """
         Determine ATMO.INTERP interpolation variable. Order of precedence:
-
-        1. Value of ATMO_IN.INTERP, if it exists and is set
-        2. Value of ATMO_GRID[0].INTERP, if it exists and is set
-        3. 'TAU', if ATMO_GRID.TAU exists (preferred over 'RHOX' for interpolation)
-        4. 'RHOX', if ATMO_GRID.RHOX exists
-
+            1. Value of ATMO_IN.INTERP, if it exists and is set
+            2. Value of ATMO_GRID[0].INTERP, if it exists and is set
+            3. 'TAU', if ATMO_GRID.TAU exists (preferred over 'RHOX' for interpolation)
+            4. 'RHOX', if ATMO_GRID.RHOX exists
         Check that INTERP is valid and the corresponding field exists in ATMO.
 
         Parameters
         ----------
         interp : {"RHOX", "TAU", None}
             requested interpolation axis, or None for autoselect
         atmo_grid : AtmosphereGrid
@@ -548,15 +538,15 @@
             raise AtmosphereError("no value for ATMO.INTERP")
         if interp not in ["TAU", "RHOX"]:
             raise AtmosphereError(
                 "ATMO.INTERP must be 'TAU' or 'RHOX', not '%s'" % interp
             )
         if interp.lower() not in gtags:
             raise AtmosphereError(
-                "ATMO.INTERP='{}', but ATMO. {} does not exist".format(interp, interp)
+                "ATMO.INTERP='%s', but ATMO. %s does not exist" % (interp, interp)
             )
         return interp
 
     def find_corner_models(self, teff, logg, monh, atmo_grid):
         """
         Find the models in the grid that bracket the given stellar parameters
 
@@ -649,19 +639,15 @@
                 gup = gmax
                 glo = np.max(glist[glist < gup])
             gb[i] = [glo, gup]  # store boundary values.
 
             # Trace diagnostics.
             if self.verbose >= 5:
                 logger.info(
-                    "log(g) at [M/H]=%.3f: %.3f < %.3f < %.3f",
-                    mb[i],
-                    glo,
-                    logg,
-                    gup,
+                    "log(g) at [M/H]=%.3f: %.3f < %.3f < %.3f", mb[i], glo, logg, gup
                 )
 
         # End of loop through [M/H] bracket values.
         # *** DETERMINATION OF TEFF BRACKETS AT [M/H] and LOG(G) BRACKET VALUES ***
         # Set up for loop through [M/H] and log(g) bounds.
         tb = np.zeros((nb, nb, nb))  # bounding temperatures
         for ig in range(nb):
@@ -788,37 +774,48 @@
 
         Returns
         -------
         atmo3: Atmosphere
             Interpolated atmosphere
         """
 
-        # We do this for every pair of atmosphere models
-        def interpolate(m0, m1, p, param, **kwargs):
+        # Interpolate 8 corner models to create 4 models at the desired [M/H].
+        atmo = np.empty((2, 2), dtype=object)
+        param = "monh"
+        p = monh
+
+        for (i, j) in np.ndindex(2, 2):
+            m0 = atmo_grid[icor[0, i, j]]
+            m1 = atmo_grid[icor[1, i, j]]
             p0 = getattr(m0, param)
             p1 = getattr(m1, param)
             pfrac = (p - p0) / (p1 - p0) if p0 != p1 else 0
-            return self.interp_atmo_pair(m0, m1, pfrac, interpvar=interp, **kwargs)
-
-        # Interpolate 8 corner models to create 4 models at the desired [M/H].
-        atmo = [[None, None], [None, None]]
-        for (i, j) in np.ndindex(2, 2):
-            m0 = atmo_grid[icor[0, j, i]]
-            m1 = atmo_grid[icor[1, j, i]]
-            atmo[i][j] = interpolate(m0, m1, monh, "monh", itop=itop)
+            atmo[i, j] = self.interp_atmo_pair(
+                m0, m1, pfrac, interpvar=interp, itop=itop
+            )
 
         # Interpolate 4 models at the desired [M/H] to create 2 models at desired
         # [M/H] and log(g).
         atmo2 = [None, None]
-        for k in range(2):
-            atmo2[k] = interpolate(atmo[k][0], atmo[k][1], logg, "logg")
+        param = "teff"
+        p = teff
+        for (k,) in np.ndindex(2):
+            m0 = atmo[0, k]
+            m1 = atmo[1, k]
+            p0 = getattr(m0, param)
+            p1 = getattr(m1, param)
+            pfrac = (p - p0) / (p1 - p0) if p0 != p1 else 0
+            atmo2[k] = self.interp_atmo_pair(m0, m1, pfrac, interpvar=interp)
 
         # Interpolate the 2 models at desired [M/H] and log(g) to create final
         # model at desired [M/H], log(g), and Teff
-        atmo3 = interpolate(atmo2[0], atmo2[1], teff, "teff")
+        t0 = atmo2[0].teff
+        t1 = atmo2[1].teff
+        tfrac = 0 if t0 == t1 else (teff - t0) / (t1 - t0)
+        atmo3 = self.interp_atmo_pair(atmo2[0], atmo2[1], tfrac, interpvar=interp)
 
         return atmo3
 
     def spherical_model_correction(self, atmo_grid, icor, logg):
         """
         Correct the radius of the model grids, for the stellar parameters if necessary
 
@@ -831,16 +828,15 @@
             2 * log(R / R_sol) = log g_sol - log g + log(M / M_sol)
 
         Parameters
         ----------
         atmo_grid : AtmosphereGrid
             complete atmosphere grid
         icor : array_like
-            indices for the corner models that were interpolated from the
-            atmosphere grid
+            indices for the corner models that were interpolated from the atmosphere grid
 
         Returns
         -------
         geom : {"PP", "SPH"}
             The geometry of the interpolated models
         radius : None, array
             The corrected radius of the models, if geom == "SPH". Otherwise None.
```

### Comparing `pysme-astro-0.4.99/src/pysme/broadening.py` & `pysme-astro-5.74.9/src/pysme/broadening.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 import logging
 
 import numpy as np
 from scipy.interpolate import interp1d
 from scipy.ndimage.filters import convolve
 
 logger = logging.getLogger(__name__)
@@ -17,21 +16,19 @@
     ipres : float
         instrument resolution
     x_seg : array (npoints,)
         x values (wavelength) of the spectrum to broaden
     y_seg : array (npoints,)
         y values (intensities) of the spectrum to broaden
     type : {str, None}, optional
-        broadening type to apply. Options are "gauss", "sinc", "table", None.
-        If None, will try to use sme.iptype to determine type. "table" requires
-        keyword sme to be passed as well. See functions the respective for details.
+        broadening type to apply. Options are "gauss", "sinc", "table", None. If None, will try to use sme.iptype to determine type.
+        "table" requires keyword sme to be passed as well. See functions the respective for details.
         (default: "gauss")
     sme : SME_Struct, optional
-        sme structure with instrument profile data, required only for
-        type="table" or type=None (default: None)
+        sme structure with instrument profile data, required only for type="table" or type=None (default: None)
 
     Raises
     ------
     AttributeError
         if type requires SME_Struct, but its missing
         passed type not recognized
 
@@ -41,15 +38,15 @@
         broadened intensity spectrum
     """
 
     if sme is None and type in ["table", None]:
         raise AttributeError(f"SME structure needs to be passed when using type={type}")
 
     # Using the log-linear wavelength grid requires using the first point
-    # for specifying the width of the instrumental profile
+    # for specifying the the width of the instrumental profile
     hwhm = 0.5 * x_seg[0] / ipres if ipres > 0 else 0
 
     if type is None:
         type = sme.iptype
     type = type.casefold()
 
     if type == "table":
@@ -161,31 +158,26 @@
         return s  # true: no broadening
 
     # Calculate (uniform) dispersion.
     nw = len(w)  ## points in spectrum
     wrange = w[-1] - w[0]
     dw = wrange / (nw - 1)  # wavelength change per pixel
 
-    # Make smoothing gaussian; extend to 4 sigma.
-    # 4.0 / sqrt(2.0 * alog(2.0)) = 3.3972872
-    # sqrt(alog(2.0)) = 0.83255461
-    # sqrt(alog(2.0) / pi) = 0.46971864
-    # (*1.0000632 to correct for >4 sigma wings)
+    # Make smoothing gaussian# extend to 4 sigma.
+    # 4.0 / sqrt(2.0*alog(2.0)) = 3.3972872 and sqrt(alog(2.0))=0.83255461
+    # sqrt(alog(2.0)/pi)=0.46971864 (*1.0000632 to correct for >4 sigma wings)
     if hwhm >= 5 * wrange:
         return np.full(nw, np.sum(s) / nw)
-    ## points in half gaussian
-    nhalf = int(3.3972872 * hwhm / dw)
-    ## points in gaussian (odd!)
-    ng = 2 * nhalf + 1
-    # wavelength scale of gaussian
-    wg = dw * (np.arange(ng, dtype=float) - (ng - 1) / 2)
-    # convenient absisca
-    xg = (0.83255461 / hwhm) * wg
-    # unit area gaussian w / FWHM
-    gpro = (0.46974832 * dw / hwhm) * np.exp(-xg * xg)
+    nhalf = int(3.3972872 * hwhm / dw)  ## points in half gaussian
+    ng = 2 * nhalf + 1  ## points in gaussian (odd!)
+    wg = dw * (
+        np.arange(ng, dtype=float) - (ng - 1) / 2
+    )  # wavelength scale of gaussian
+    xg = (0.83255461 / hwhm) * wg  # convenient absisca
+    gpro = (0.46974832 * dw / hwhm) * np.exp(-xg * xg)  # unit area gaussian w/ FWHM
     gpro = gpro / np.sum(gpro)
 
     # Pad spectrum ends to minimize impact of Fourier ringing.
     sout = convolve(s, gpro, mode="nearest")
 
     return sout
```

### Comparing `pysme-astro-0.4.99/src/pysme/config.py` & `pysme-astro-5.74.9/src/pysme/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
 """
 Handle the Json configuration file
 At the moment it is only used for the LargeFileStorage
 """
-import json
 import logging
-from os.path import dirname, exists, expanduser, join
+from os.path import expanduser
+import json
 
 logger = logging.getLogger(__name__)
 
 
 def _requires_load(func):
     def func_new(self, *args, **kwargs):
         if self._cfg is None:
@@ -20,20 +19,14 @@
 
 
 class Config:
     def __init__(self, fname="~/.sme/config.json"):
         self.filename = fname
         self._cfg = None
 
-        if not exists(self.filename):
-            logger.info(
-                f"No cconfiguration file found at {self.filename}, using default values instead"
-            )
-            self.filename = join(dirname(__file__), "config_default.json")
-
     @property
     def filename(self):
         return str(self._filename)
 
     @filename.setter
     def filename(self, value):
         self._filename = expanduser(value)
```

### Comparing `pysme-astro-0.4.99/src/pysme/data_structure.py` & `pysme-astro-5.74.9/src/pysme/data_structure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,28 @@
-# -*- coding: utf-8 -*-
 import logging
+import os.path
+import platform
+import sys
 from copy import copy
+from datetime import datetime as dt
 
 import numpy as np
-import pybtex
-from flex.extensions.bindata import MultipleDataExtension
+from flex.extensions.bindata import BinaryDataExtension
 from flex.flex import FlexExtension
+import pybtex
+
 
-from . import __file_ending__, __version__, persistence
+from . import __file_ending__, __version__, echelle, persistence
 from .iliffe_vector import Iliffe_vector
 
 logger = logging.getLogger(__name__)
 
 
 def this(self, x):
-    """This just returns the input"""
+    """ This just returns the input """
     return x
 
 
 def notNone(func):
     def f(self, value):
         return func(self, value) if value is not None else None
 
@@ -43,19 +47,17 @@
         except AttributeError:
             pass
         return func(self, value)
 
     return f
 
 
-def oneof(*options, astype=None):
+def oneof(*options):
     def f(self, value):
         if value not in options:
-            if astype is not None and astype(value) == value:
-                return astype(value)
             raise ValueError(f"Received {value} but expected one of {options}")
         return value
 
     return f
 
 
 def astype(func, allow_None=False):
@@ -117,26 +119,26 @@
     return f
 
 
 def vector(self, value):
     if value is None:
         return None
     elif np.isscalar(value):
-        wind = self.wave.sizes if self.wave is not None else None
+        wind = [0, *np.cumsum(self.wave.sizes)] if self.wave is not None else None
         values = np.full(self.wave.size, value)
-        value = Iliffe_vector.from_indices(values, self.wave.sizes)
+        value = Iliffe_vector(values=values, index=wind)
     elif isinstance(value, np.ndarray):
         value = np.require(value, requirements="W")
         if value.ndim == 1:
-            wind = self.wave.sizes if self.wave is not None else None
-            value = Iliffe_vector.from_indices(value, wind)
+            wind = [0, *np.cumsum(self.wave.sizes)] if self.wave is not None else None
+            value = Iliffe_vector(values=value, index=wind)
         else:
-            value = Iliffe_vector(value)
+            value = Iliffe_vector(nseg=len(value), values=[v for v in value])
     elif isinstance(value, list):
-        value = Iliffe_vector(value)
+        value = Iliffe_vector(nseg=len(value), values=value)
     elif isinstance(value, Iliffe_vector):
         pass
     elif isinstance(value, FlexExtension):
         value = Iliffe_vector._load(value)
     elif isinstance(value, np.lib.npyio.NpzFile):
         value = Iliffe_vector._load_v1(value)
     else:
@@ -165,38 +167,28 @@
     def f(self, value):
         setattr(self, name, func(self, value))
 
     return f
 
 
 def CollectionFactory(cls):
-    """Decorator that turns Collection _fields into properties"""
+    """ Decorator that turns Collection _fields into properties """
 
     # Add properties to the class
     for name, _, setter, getter, doc in cls._fields:
-        setattr(
-            cls,
-            name,
-            property(fget(name, getter), fset(name, setter), None, doc),
-        )
+        setattr(cls, name, property(fget(name, getter), fset(name, setter), None, doc))
     cls._names = [f[0] for f in cls._fields]
 
     return cls
 
 
 @CollectionFactory
 class Collection(persistence.IPersist):
     _fields = [
-        (
-            "citation_info",
-            "",
-            asstr,
-            this,
-            "str: Bibtex representation of the citation",
-        )
+        ("citation_info", "", asstr, this, "str: Bibtex representation of the citation")
     ]  # [("name", "default", str, this, "doc")]
 
     def __init__(self, **kwargs):
         for name, default, *_ in self._fields:
             setattr(self, name, copy(default))
 
         for key, value in kwargs.items():
@@ -241,28 +233,19 @@
         )
 
     def citation(self, output="string"):
         return self.create_citation(self.citation_info, output=output)
 
     def _save(self):
         header = {}
-        data = {}
+        data = None
 
         for name in self._names:
-            value = self[name]
-            if isinstance(value, np.ndarray) and value.size > 10:
-                data[name] = value
-            else:
-                header[name] = value
+            header[name] = self[name]
 
-        ext = MultipleDataExtension(header, data)
+        ext = BinaryDataExtension(header)
         return ext
 
     @classmethod
-    def _load(cls, ext: MultipleDataExtension):
-        header = ext.header
-        if isinstance(ext, MultipleDataExtension):
-            data = dict(ext.data)
-            header.update(data)
-
-        obj = cls(**header)
+    def _load(cls, ext: BinaryDataExtension):
+        obj = cls(**ext.header)
         return obj
```

### Comparing `pysme-astro-0.4.99/src/pysme/echelle.py` & `pysme-astro-5.74.9/src/pysme/echelle.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
-# -*- coding: utf-8 -*-
 """
 Contains functions to read and modify echelle structures, just as in reduce
 
 Mostly for compatibility reasons
 """
 
 import logging
-
 import astropy.io.fits as fits
 import numpy as np
 import scipy.constants
 
 logger = logging.getLogger(__name__)
 
 
@@ -102,15 +100,15 @@
 
     Parameters
     ----------
     ncol : int
         number of columns in the image
     poly : array[nord, ...]
         polynomial coefficients to expand, or already expanded data
-
+    
     Returns
     -------
     poly : array[nord, ncol]
         expanded data
     """
 
     if poly.ndim == 1:
```

### Comparing `pysme-astro-0.4.99/src/pysme/gui/plot_plotly.py` & `pysme-astro-5.74.9/src/pysme/gui/plot_plotly.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,78 +1,60 @@
-# -*- coding: utf-8 -*-
 """
 Provide Plotting utility for Jupyter Notebook using Plot.ly
 Can also be used just for Plot.ly, which will then generated html files
 """
-import json
-import logging
-from base64 import b64encode
-
 import numpy as np
-import plotly.graph_objs as go
 import plotly.offline as py
+import plotly.graph_objs as go
 from plotly.io import write_image
-from scipy.constants import speed_of_light
 
+from scipy.constants import speed_of_light
 from .plot_colors import PlotColors
 
 try:
     import ipywidgets as widgets
     from IPython import get_ipython
     from IPython.display import display
 
     cfg = get_ipython()
     in_notebook = cfg is not None
 except (AttributeError, ImportError, ModuleNotFoundError):
     in_notebook = False
 
-logger = logging.getLogger(__name__)
 clight = speed_of_light * 1e-3
 fmt = PlotColors()
 
-try:
-    import htmlmin
-except ImportError:
-    logger.info("Install htmlmin for minified html files")
-    htmlmin = None
-
 if in_notebook:
     py.init_notebook_mode()
 
 
 class FitPlot:
-    """Plot the sme solve fit, as iterations pass along"""
+    """ Plot the sme solve fit, as iterations pass along """
 
     def __init__(self, wave, spec):
         self.fig = go.FigureWidget()
         self.fig.layout["xaxis"]["title"] = "Wavelength [Å]"
         self.fig.layout["yaxis"]["title"] = "Intensity"
 
         self.fig.add_scatter(x=wave, y=spec, name="Observation")
 
     def add_synth(self, wave, synth, iteration=0):
-        """add a scatter plot to the plot"""
+        """ add a scatter plot to the plot """
         self.fig.add_scatter(x=wave, y=synth, name=f"Iteration {iteration}")
 
 
 class FinalPlot:
-    """Big plot that covers everything"""
+    """ Big plot that covers everything """
 
-    def __init__(self, sme, segment=0, orig=None, labels=None):
+    def __init__(self, sme, segment=0):
         self.sme = sme
         self.wave = sme.wave
         self.spec = sme.spec
         self.mask = sme.mask
         self.smod = sme.synth
-        self.orig = orig
-        self.labels = labels if labels is not None else {}
-        if sme.telluric is not None and self.smod is not None:
-            for i in range(sme.nseg):
-                if len(self.smod[i]) != 0:
-                    self.smod[i] = self.smod[i] * sme.telluric[i]
         self.nsegments = len(self.wave)
         self.segment = segment
         self.wran = sme.wran
         self.lines = sme.linelist
         self.vrad = sme.vrad
         self.vrad = [v if v is not None else 0 for v in self.vrad]
 
@@ -111,110 +93,63 @@
         }
         if in_notebook:
             self.fig = go.FigureWidget(data=data, layout=layout)
 
             # add selection callback
             self.fig.data[0].on_selection(self.selection_fn)
         else:
-            data = [go.Scattergl(d) for d in data]
-            self.fig = go.FigureWidget(data=data, layout=layout)
+            self.fig = go.Figure(data=data, layout=layout)
 
         # Add button to save figure
         if in_notebook:
             self.button_save = widgets.Button(description="Save")
             self.button_save.on_click(self.save)
 
             # Add buttons for Mask selection
             self.button_mask = widgets.ToggleButtons(
-                options=["Good", "Bad", "Continuum", "Line"],
-                description="Mask",
+                options=["Good", "Bad", "Continuum", "Line"], description="Mask"
             )
             self.button_mask.observe(self.on_toggle_click, "value")
 
             self.widget = widgets.VBox([self.button_mask, self.button_save, self.fig])
             display(self.widget)
 
     def save(self, _=None, filename="SME.html", **kwargs):
-        """save plot to html file"""
-        # Here we "hack" plotly to use base64 encoded data
-        # since we have a lot of data to look at
-        # this reduces the file size by about a factor 3
-        # zipping it would provide another factor 2
+        """ save plot to html file """
         if filename.endswith(".html"):
             self.fig.layout.dragmode = "zoom"
-            fig = self.fig.to_plotly_json()
-            # Convert the data to base64
-            for i in range(len(fig["data"])):
-                for ax in ["x", "y"]:
-                    data = np.asarray(fig["data"][i][ax]).astype("float32")
-                    b64data = b64encode(data).decode("utf8")
-                    fig["data"][i][ax] = {"data": b64data, "dtype": "float32"}
-
-            data = json.dumps(fig["data"])
-            layout = json.dumps(fig["layout"])
-            # This is the entire html as generated by self.fig.to_html
-            # except we replace the data and layout manually
-            # and transform it from base64 to TypedArrays
-            html = (
-                r"""<html><head><meta charset="utf-8" /></head><body><div>"""
-                r"""<script type="text/javascript">window.PlotlyConfig = {MathJaxConfig: 'local'};</script>"""
-                r"""<script src="https://cdn.plot.ly/plotly-latest.min.js"></script>"""
-                r"""<div id="56dedbe2-a786-4b0b-8232-b68dfd7b9eb5" class="plotly-graph-div" style="height:100%; width:100%;"></div>"""
-                r"""<script type="text/javascript">"""
-                r"""window.PLOTLYENV=window.PLOTLYENV || {};"""
-                r"""if (document.getElementById("56dedbe2-a786-4b0b-8232-b68dfd7b9eb5")) {"""
-                f"data = {data};"
-                f"layout = {layout};"
-                r"""const FromBase64 = function (str) {return new Uint8Array(atob(str).split('').map(function (c) { return c.charCodeAt(0); }));};"""
-                r"""for (let i = 0; i < data.length; i++){"""
-                r"""let data_x = data[i].x.data;"""
-                r"""let data_y = data[i].y.data;"""
-                r"""data[i].x = new Float32Array(FromBase64(data_x).buffer);"""
-                r"""data[i].y = new Float32Array(FromBase64(data_y).buffer);"""
-                r"""}"""
-                r"""Plotly.newPlot("56dedbe2-a786-4b0b-8232-b68dfd7b9eb5", data, layout, {"responsive": true})};"""
-                r"""</script></div></body></html>"""
-            )
-            # Finally try to minimize if possible
-            if htmlmin is not None:
-                html = htmlmin.minify(html, remove_empty_space=True)
-            with open(filename, "w") as f:
-                f.write(html)
-
+            py.plot(self.fig, filename=filename, **kwargs)
         else:
             write_image(self.fig, filename)
 
-    def show(self):
-        self.fig.show()
-
     def shift_mask(self, x, mask):
-        """shift the edges of the mask to the bottom of the plot,
-        so that the mask creates a shape with straight edges"""
+        """ shift the edges of the mask to the bottom of the plot,
+        so that the mask creates a shape with straight edges """
         for i in np.where(mask)[0]:
             try:
                 if mask[i] == mask[i + 1]:
                     x[i] = x[i - 1]
                 else:
                     x[i] = x[i + 1]
             except IndexError:
                 pass
 
         return x
 
     def create_mask_points(self, x, y, mask, value):
-        """Creates the points that define the outer edge of the mask region"""
+        """ Creates the points that define the outer edge of the mask region """
         mask = mask != value
         x = np.copy(x)
         y = np.copy(y)
         y[mask] = 0
         x = self.shift_mask(x, mask)
         return x, y
 
     def create_plot(self, current_segment):
-        """Generate the plot componentes (lines and masks) and line labels"""
+        """ Generate the plot componentes (lines and masks) and line labels """
 
         annotations = {}
         visible = []
         data = []
         line_mask_idx = {}
         cont_mask_idx = {}
 
@@ -243,15 +178,15 @@
                 data += [
                     dict(
                         x=x,
                         y=y,
                         fillcolor=fmt["LineMask"]["facecolor"],
                         fill="tozeroy",
                         mode="none",
-                        name=self.labels.get("linemask", "Line Mask"),
+                        name="Line Mask",
                         hoverinfo="none",
                         legendgroup=2,
                         visible=current_segment == seg,
                     )
                 ]
                 visible += [seg]
 
@@ -263,61 +198,49 @@
                 data += [
                     dict(
                         x=x,
                         y=y,
                         fillcolor=fmt["ContMask"]["facecolor"],
                         fill="tozeroy",
                         mode="none",
-                        name=self.labels.get("contmask", "Continuum Mask"),
+                        name="Continuum Mask",
                         hoverinfo="none",
                         legendgroup=2,
                         visible=current_segment == seg,
                     )
                 ]
                 visible += [seg]
 
             if self.spec is not None:
                 # Observation
                 data += [
                     dict(
                         x=self.wave[seg],
                         y=self.spec[seg],
                         line={"color": fmt["Obs"]["color"]},
-                        name=self.labels.get("obs", "Observation"),
+                        name="Observation",
                         legendgroup=0,
                         visible=current_segment == seg,
                     )
                 ]
                 visible += [seg]
 
             # Synthetic, if available
             if self.smod is not None:
                 data += [
                     dict(
                         x=self.wave[seg],
                         y=self.smod[seg],
-                        name=self.labels.get("synth", "Synthethic"),
+                        name="Synthethic",
                         line={"color": fmt["Syn"]["color"]},
                         legendgroup=1,
                         visible=current_segment == seg,
                     )
                 ]
                 visible += [seg]
-            if self.orig is not None:
-                data += [
-                    dict(
-                        x=self.wave[seg],
-                        y=self.orig[seg],
-                        name=self.labels.get("orig", "Original"),
-                        line={"color": fmt["Orig"]["color"], "dash": "dash"},
-                        legendgroup=1,
-                        visible=current_segment == seg,
-                    )
-                ]
-                visible += [seg]
 
             # mark important lines
             if self.lines is not None and len(self.lines) != 0:
                 seg_annotations = []
                 xlimits = self.wave[seg][[0, -1]]
                 xlimits *= 1 - self.vrad[seg] / clight
                 lines = (self.lines.wlcent > xlimits[0]) & (
@@ -356,18 +279,18 @@
                 #     lines.sort("depth", ascending=False)
                 #     lines = lines[:20]
                 # else:
                 #     idx = np.random.choice(len(lines), 20, replace=False)
                 #     lines = lines[idx]
 
                 x = wlcent * (1 + self.vrad[seg] / clight)
-                if self.smod is not None and len(self.smod[seg]) != 0:
-                    y = np.interp(x, self.wave[seg], self.smod[seg])
-                else:
+                if self.spec is not None:
                     y = np.interp(x, self.wave[seg], self.spec[seg])
+                else:
+                    y = np.interp(x, self.wave[seg], self.smod[seg])
 
                 if self.smod is not None and len(self.smod[seg]) > 0:
                     ytop = np.max(self.smod[seg])
                 elif self.spec is not None and len(self.spec[seg]) > 0:
                     ytop = np.max(self.spec[seg])
                 else:
                     ytop = 1
@@ -396,15 +319,15 @@
         self.visible = visible
         self.line_mask_idx = line_mask_idx
         self.cont_mask_idx = cont_mask_idx
 
         return data, annotations
 
     def selection_fn(self, trace, points, selector):
-        """Callback for area selection, changes the mask depending on selected mode"""
+        """ Callback for area selection, changes the mask depending on selected mode """
         self.segment = self.fig.layout["sliders"][0].active
         seg = self.segment
 
         xrange = selector.xrange
         wave = self.wave[seg]
         mask = self.mask[seg]
 
@@ -443,48 +366,48 @@
                 x, y = self.create_mask_points(
                     self.wave[seg], self.spec[seg], self.mask[seg], 2
                 )
                 self.fig.data[m].x = x
                 self.fig.data[m].y = y
 
     def on_toggle_click(self, change):
-        """Callback for mask mode selector buttons"""
+        """ Callback for mask mode selector buttons """
         change = change["new"]
         if change == "Good":
             self.set_mask_good()
         elif change == "Bad":
             self.set_mask_bad()
         elif change == "Continuum":
             self.set_mask_continuum()
         elif change == "Line":
             self.set_mask_line()
 
     def set_mask_good(self, _=None):
-        """Called by clicking the 'good' mask button"""
+        """ Called by clicking the 'good' mask button """
         self.set_mask_type("good")
 
     def set_mask_bad(self, _=None):
-        """Called by clicking the 'bad' mask button"""
+        """ Called by clicking the 'bad' mask button """
         self.set_mask_type("bad")
 
     def set_mask_line(self, _=None):
-        """Called by clicking the 'line' mask button"""
+        """ Called by clicking the 'line' mask button """
         self.set_mask_type("line")
 
     def set_mask_continuum(self, _=None):
-        """Called by clicking the 'continuum' mask button"""
+        """ Called by clicking the 'continuum' mask button """
         self.set_mask_type("cont")
 
     def set_mask_type(self, type):
-        """Changes the mask change mode and chooses the current interactive tool"""
+        """ Changes the mask change mode and chooses the current interactive tool """
         self.mask_type = type
         self.fig.layout["dragmode"] = "select"
 
     def add(self, x, y, label=""):
-        """adds a scatter plot to the image, and makes the necessary changes in the slider"""
+        """ adds a scatter plot to the image, and makes the necessary changes in the slider """
         self.fig.add_scatter(x=x, y=y, name=label, legendgroup=10)
         self.visible += [-1]
 
         # Update Sliders
         steps = []
         for i in range(self.nsegments):
             step_visible = [(v == i) or (v == -1) for v in self.visible]
```

### Comparing `pysme-astro-0.4.99/src/pysme/gui/plot_pyplot.py` & `pysme-astro-5.74.9/src/pysme/gui/plot_pyplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-# -*- coding: utf-8 -*-
+import numpy as np
 import matplotlib as mpl
+from matplotlib.widgets import SpanSelector, Button
 import matplotlib.pyplot as plt
-import numpy as np
-from matplotlib.widgets import Button, SpanSelector
+
+
 from scipy.constants import c
 
 clight = c * 1e-3
 
 # from ..sme.sme import SME_Struct
 
 from .plot_colors import PlotColors
 
 fmt = PlotColors()
 
 
 class MaskPlot:
-    """A plot that can be used to define the mask"""
+    """ A plot that can be used to define the mask """
 
     # Controls:
     # a, d keys: Switch between segments
     # Left, Right Mouse button: Select sections to change the mask depending on current mode
     #       mode == "good/bad" : left  -> line mask
     #                            right -> bad mask
     #                            Does not override existing good line mask
@@ -121,15 +122,15 @@
         self.section_select(min, max, mask_type)
 
     def section_continuum_callback(self, min, max):
         mask_type = "cont" if self.mode == "line/cont" else "bad"
         self.section_select(min, max, mask_type)
 
     def section_select(self, min, max, mask_type):
-        print("{} {:.3f} - {:.3f}".format(mask_type, min, max))
+        print("%s %.3f - %.3f" % (mask_type, min, max))
         # find points
         idx = (self.wave[self.segment] <= max) & (self.wave[self.segment] >= min)
 
         # update masks
         if mask_type == "line":
             mask_value = 1
         elif mask_type == "cont":
@@ -214,23 +215,19 @@
                         rotation="vertical",
                         horizontalalignment="right",
                         verticalalignment="top",
                         alpha=importance[i],
                     )
                     if self.spec is not None:
                         depth = np.interp(
-                            wl,
-                            self.wave[self.segment],
-                            self.spec[self.segment],
+                            wl, self.wave[self.segment], self.spec[self.segment]
                         )
                     else:
                         depth = np.interp(
-                            wl,
-                            self.wave[self.segment],
-                            self.smod[self.segment],
+                            wl, self.wave[self.segment], self.smod[self.segment]
                         )
                     self.line_plot[i][1] = self.im.vlines(
                         wl, ymin=depth, ymax=1.1, alpha=importance[i]
                     )
                 self.lock = False
         except ValueError:
             pass
@@ -274,7 +271,8 @@
             self.connect_axes()
 
     def next_segment(self, _=None):
         self.goto_segment(self.segment + 1)
 
     def previous_segment(self, _=None):
         self.goto_segment(self.segment - 1)
+
```

### Comparing `pysme-astro-0.4.99/src/pysme/linelist/linelist.py` & `pysme-astro-5.74.9/src/pysme/linelist/linelist.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# -*- coding: utf-8 -*-
 """
 Handles abstract LineList data
 Implementation of a specific source (e.g. Vald) should be in its own file
 
 Uses a pandas dataframe under the hood to handle the data
 """
 import io
 import json
 import logging
 
 import numpy as np
 import pandas as pd
+
 from flex.extensions.tabledata import JSONTableExtension
-from scipy import constants
 
 from ..persistence import IPersist
 from ..util import air2vac, vac2air
 
 logger = logging.getLogger(__name__)
 
 
 class LineListError(Exception):
     """Raise when attempt to read a line data file fails"""
 
 
 class LineList(IPersist):
-    """Atomic data for a list of spectral lines"""
+    """Atomic data for a list of spectral lines
+    """
 
     _base_columns = [
         "species",
         "wlcent",
         "excit",
         "gflog",
         "gamrad",
@@ -75,65 +75,39 @@
             "D+": 0.4,
             "D": 0.5,
             "D-": 0.6,
             "E": 0.7,
         }
         error = np.ones(len(error_flags), dtype=float)
         for i, (flag, _) in enumerate(zip(error_flags, values)):
-            if len(flag) == 0:
-                error[i] = 0.5
-            elif flag[0] in [" ", "_", "P"]:
+            if flag[0] in [" ", "_", "P"]:
                 # undefined or predicted
                 error[i] = 0.5
             elif flag[0] == "E":
                 # absolute error in dex
                 # TODO absolute?
                 error[i] = 10 ** float(flag[1:])
             elif flag[0] == "C":
                 # Cancellation Factor, i.e. relative error
-                try:
-                    error[i] = abs(float(flag[1:]))
-                except ValueError:
-                    error[i] = 0.5
+                error[i] = abs(float(flag[1:]))
             elif flag[0] == "N":
                 # NIST quality class
                 flag = flag[1:5].strip()
-                try:
-                    error[i] = nist[flag]
-                except KeyError:
-                    error[i] = 0.5
+                error[i] = nist[flag]
         return error
 
     @staticmethod
-    def guess_format(kwargs):
-        short_line_format = kwargs.pop(
-            "short_line_format", kwargs.pop("short_format", None)
-        )
-        if short_line_format is not None:
-            return short_line_format
-
-        keys = kwargs.keys()
-        if (
-            "line_extra" in keys
-            and "line_lulande" in keys
-            and "line_term_low" in keys
-            and "line_term_upp" in keys
-        ):
-            return 2
-        return 1
-
-    @classmethod
-    def from_IDL_SME(cls, **kwargs):
-        """extract LineList from IDL SME structure keywords"""
+    def from_IDL_SME(**kwargs):
+        """ extract LineList from IDL SME structure keywords """
         species = kwargs.pop("species").astype("U")
         atomic = np.asarray(kwargs.pop("atomic"), dtype="<f8")
         lande = np.asarray(kwargs.pop("lande"), dtype="<f8")
         depth = np.asarray(kwargs.pop("depth"), dtype="<f8")
         lineref = kwargs.pop("lineref").astype("U")
-        short_line_format = cls.guess_format(kwargs)
+        short_line_format = kwargs.pop("short_line_format")
         if short_line_format == 2:
             line_extra = np.asarray(kwargs.pop("line_extra"), dtype="<f8")
             line_lulande = np.asarray(kwargs.pop("line_lulande"), dtype="<f8")
             line_term_low = kwargs.pop("line_term_low").astype("U")
             line_term_upp = kwargs.pop("line_term_upp").astype("U")
 
         # If there is only one line, it is 1D in the IDL structure, but we expect 2D
@@ -239,37 +213,33 @@
     def __repr__(self):
         return self.__str__()
 
     def __iter__(self):
         return self._lines.itertuples(index=False)
 
     def __getitem__(self, index):
-        if isinstance(index, str) and hasattr(self, index):
-            return getattr(self, index)
         if isinstance(index, (list, str)):
             if len(index) == 0:
                 return LineList(
-                    self._lines.iloc[[]],
-                    lineformat=self.lineformat,
-                    medium=self.medium,
+                    self._lines.iloc[[]], lineformat=self.lineformat, medium=self.medium
                 )
             values = self._lines[index].values
             if index in self.string_columns:
                 values = values.astype(str)
             return values
         else:
             if isinstance(index, int):
                 index = slice(index, index + 1)
             # just pass on a subsection of the linelist data, but keep it a linelist object
             return LineList(
                 self._lines.iloc[index], self.lineformat, medium=self.medium
             )
 
     def __getattribute__(self, name):
-        if name[0] != "_" and name not in dir(self) and name in self._lines:
+        if name[0] != "_" and name not in dir(self):
             return self._lines[name].values
         return super().__getattribute__(name)
 
     @property
     def columns(self):
         return self._lines.columns
 
@@ -297,59 +267,57 @@
             else:
                 raise ValueError(
                     f"Type of medium not undertstood. Expected one of [vac, air], but got {value} instead"
                 )
 
     @property
     def species(self):
-        """list(str) of size (nlines,): Species name of each line"""
+        """list(str) of size (nlines,): Species name of each line """
         return self._lines["species"].values.astype("U")
 
     @property
     def lulande(self):
-        """list(float) of size (nlines, 2): Lower and Upper Lande factors"""
+        """list(float) of size (nlines, 2): Lower and Upper Lande factors """
         if self.lineformat == "short":
             raise AttributeError(
                 "Lower and Upper Lande Factors are only available in the long line format"
             )
 
             # additional data arrays for sme
         names = ["lande_lower", "lande_upper"]
         return self._lines.reindex(columns=names).values
 
     @property
     def extra(self):
-        """list(float) of size (nlines, 3): additional line level information for NLTE calculation"""
+        """list(float) of size (nlines, 3): additional line level information for NLTE calculation """
         if self.lineformat == "short":
             raise AttributeError("Extra is only available in the long line format")
         names = ["j_lo", "e_upp", "j_up"]
         return self._lines.reindex(columns=names).values
 
     @property
     def atomic(self):
-        """list(float) of size (nlines, 8): Data array passed to C library, should only be used for this purpose"""
+        """list(float) of size (nlines, 8): Data array passed to C library, should only be used for this purpose """
         names = [
             "atom_number",
             "ionization",
             "wlcent",
             "excit",
             "gflog",
             "gamrad",
             "gamqst",
             "gamvw",
         ]
         # Select fields
-        values = self._lines.reindex(columns=names).values
-        values = values.astype(float)
-        return values
+        return self._lines.reindex(columns=names).values
 
     def sort(self, field="wlcent", ascending=True):
         """Sort the linelist
 
-        The underlying datastructure will be replaced,
+        The underlying datastructure will be replaced, 
         i.e. any references will not be sorted or updated
 
         Parameters
         ----------
         field : str, optional
             Field to use for sorting (default: "wlcent")
         ascending : bool, optional
@@ -363,15 +331,15 @@
 
         self._lines = self._lines.sort_values(by=field, ascending=ascending)
         return self
 
     def add(self, species, wlcent, excit, gflog, gamrad, gamqst, gamvw):
         """Add a new line to the existing linelist
 
-        This replaces the underlying datastructure,
+        This replaces the underlying datastructure, 
         i.e. any references (atomic, etc.) will not be updated
 
         Parameters
         ----------
         species : str
             Name of the element and ionization
         wlcent : float
@@ -395,60 +363,14 @@
             "gflog": gflog,
             "gamrad": gamrad,
             "gamqst": gamqst,
             "gamvw": gamvw,
         }
         self._lines = self._lines.append([linedata])
 
-    def append(self, linelist: "LineList"):
-        """
-        Append a linelist to this one
-
-        Note this replaces the underlying data
-        and sorts the lines by wavelength
-
-        Parameters
-        ----------
-        linelist : LineList
-            other linelist to append
-
-        Returns
-        -------
-        self : LineList
-            this object, now with appended data
-        """
-        if self.medium != linelist.medium:
-            logger.warning(
-                "The appended linelist, has its wavelength in a different medium"
-            )
-        if self.lineformat != linelist.lineformat:
-            raise ValueError(
-                (
-                    "The formats of the linelists do not match. This linelist "
-                    "has format %s, but the other has format %s"
-                ),
-                self.lineformat,
-                linelist.lineformat,
-            )
-        self._lines = self._lines.append(linelist._lines)
-        self.sort()
-        return self
-
-    def trim(self, wave_min, wave_max, rvel=None):
-        if rvel is not None:
-            # Speed of light in km/s
-            c_light = constants.c * 1e3
-            wave_min *= np.sqrt((1 - rvel / c_light) / (1 + rvel / c_light))
-            wave_max *= np.sqrt((1 + rvel / c_light) / (1 - rvel / c_light))
-        selection = self._lines["wlcent"] > wave_min
-        selection &= self._lines["wlcent"] < wave_max
-        return LineList(
-            self._lines[selection], lineformat=self.lineformat, medium=self.medium
-        )
-
     def _save(self):
         header = {
             "lineformat": self.lineformat,
             "medium": self.medium,
             "citation_info": self.citation_info,
         }
         data = self._lines
@@ -497,12 +419,9 @@
                 linedata = pd.read_json(b, orient="records")
             elif name.endswith("data.npy"):
                 b = io.BytesIO(file.read(name))
                 linedata = np.load(b)
                 linedata = pd.DataFrame.from_records(linedata)
 
         return LineList(
-            linedata,
-            lineformat=lineformat,
-            medium=medium,
-            citation_info=citation_info,
+            linedata, lineformat=lineformat, medium=medium, citation_info=citation_info
         )
```

### Comparing `pysme-astro-0.4.99/src/pysme/linelist/vald.py` & `pysme-astro-5.74.9/src/pysme/linelist/vald.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-# -*- coding: utf-8 -*-
 """
 Module for handling linelist data from the VALD3 database (http://vald.astro.uu.se/).
 
 
 """
 import logging
 import re
 from io import StringIO
 from os.path import dirname, join
 
 import numpy as np
 import pandas as pd
-import pybtex.database
 from astropy import units as u
+import pybtex.database
+
 
 from ..abund import Abund
-from .linelist import LineList, LineListError
+from .linelist import LineListError, LineList
 
 logger = logging.getLogger(__name__)
 
 
 class ValdError(LineListError):
-    """Vald Data File Error"""
+    """ Vald Data File Error """
 
 
 class ValdFile(LineList):
-    """Atomic data for a list of spectral lines."""
+    """Atomic data for a list of spectral lines.
+    """
 
     citation_info = r"""
     @ARTICLE{2015PhyS...90e4005R,
         author = {{Ryabchikova}, T. and {Piskunov}, N. and {Kurucz}, R.~L. and
         {Stempels}, H.~C. and {Heiter}, U. and {Pakhomov}, Yu and
         {Barklem}, P.~S.},
         title = "{A major upgrade of the VALD database}",
@@ -141,15 +142,16 @@
         and whether it is in long or short format
 
         Parameters
         ----------
         lines : list(str)
             file contents
         """
-        header = lines[0].strip().split()
+        header = lines[0]
+        header = header.strip().split()
 
         if header[0] == "Damping":
             # short format extract all / extract element
             return "extract_all", "short"
         elif header[0] == "Lande":
             # long format extract all / extract element
             return "extract_all", "long"
@@ -166,19 +168,14 @@
 
     def loads(self, filename):
         logger.info("Loading VALD file %s", filename)
 
         with open(filename, "r") as file:
             lines = file.readlines()
 
-        # Check for Warnings
-        while lines[0].lstrip().startswith("WARNING"):
-            logger.warning(f"VALD {lines[0].lstrip()}")
-            lines = lines[1:]
-
         # Determine File type and format
         valdtype, fmt = self.identify_valdtype(lines)
 
         # Determine the number of lines in the file
         if valdtype == "extract_stellar":
             n = self.parse_header(lines[0])
             # Skip the info header if extract stellar
@@ -282,15 +279,15 @@
             raise ValueError(
                 "Could not determine the medium that the wavelength is based on (air or vacuum)"
             )
 
         if unit == "A":
             self.unit = u.AA
         elif unit == "nm":
-            self.unit = u.nm
+            self.unit = u.AA
         elif unit == "cm^-1":
             self.unit = 1 / u.cm
         else:
             raise ValueError("Could not determine the unit of the wavelength")
 
         if energy_unit == "eV":
             self.energy_unit = u.eV
@@ -410,16 +407,15 @@
 
             linelist["term_lower"] = term_lower
             linelist["term_upper"] = term_upper
 
             # extract error data
             error = np.array([s[:10].strip() for s in comment])
             error = LineList.parse_line_error(
-                error,
-                linelist["depth"] if valdtype == "extract_stellar" else None,
+                error, linelist["depth"] if valdtype == "extract_stellar" else None
             )
             linelist["error"] = error
 
         # Convert from whatever unit to Angstrom
         factor = self.unit.to(u.AA)
         linelist["wlcent"] *= factor
         self.unit = "Angstrom"
@@ -498,22 +494,14 @@
         ref = set(references)
         # Multiple references are seperated by '+'
         references = []
         for r in ref:
             references += r.split("+")
         # And make it unique again, if necessary
         references = set(references)
-        # some data entries are case sensitive, but bibtex is case insnsitive
-        # so remove those and replace them with fixed versions
-        if "LWb" in references:
-            references.add("LWb2")
-            references.remove("LWb")
-        if "LGb" in references:
-            references.add("LGb2")
-            references.remove("LGb")
 
         # Get references from bibtex file
         # TODO: only load this once? But then again, how often will we do this?
         bibdata = pybtex.database.parse_file(join(dirname(__file__), "VALD3_ref.bib"))
         entries = {}
         for r in references:
             try:
```

### Comparing `pysme-astro-0.4.99/src/pysme/nlte.py` & `pysme-astro-5.74.9/src/pysme/nlte.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,21 @@
-# -*- coding: utf-8 -*-
 """
 NLTE module of SME
 reads and interpolates departure coefficients from library files
 """
 
 import itertools
 import logging
 import warnings
 
 import numpy as np
 from scipy import interpolate
-from tqdm import tqdm
 
-from .abund import Abund
-from .abund import elements as abund_elem
-from .data_structure import Collection, CollectionFactory, array, astype, oneof, this
+from .abund import Abund, elements as abund_elem
+from .data_structure import Collection, CollectionFactory, astype, array, this, oneof
 
 logger = logging.getLogger(__name__)
 
 
 class DirectAccessFile:
     """
     This function reads a single record from binary file that has the following
@@ -53,15 +50,15 @@
         # Access data via brackets
         value = self.get(key)
         if value is None:
             raise KeyError(f"Key {key} not found")
         return value
 
     def get(self, key: str, alt=None) -> np.memmap:
-        """get field from file"""
+        """ get field from file """
         idx = np.where(self.key == key)[0]
 
         if idx.size == 0:
             return alt
         else:
             idx = idx[0]
 
@@ -132,22 +129,22 @@
         return typecode[dt]
 
     @staticmethod
     def get_dtypes(version):
         major, minor = version
         if major == 1 and minor == 00:
             header_dtype = np.dtype(
-                [("nblocks", "<u2"), ("dir_length", "<u2"), ("ndir", "<u2")]
+                [("nblocks", "<u2"), ("dir_length", "<u2"), ("ndir", "<u2"),]
             )
             dir_dtype = np.dtype(
                 [("key", "S256"), ("size", "<i4", 23), ("pointer", "<i8")]
             )
         elif major == 1 and minor >= 10:
             header_dtype = np.dtype(
-                [("nblocks", "<u8"), ("dir_length", "<i2"), ("ndir", "<u8")]
+                [("nblocks", "<u8"), ("dir_length", "<i2"), ("ndir", "<u8"),]
             )
             dir_dtype = np.dtype(
                 [("key", "S256"), ("size", "<i4", 23), ("pointer", "<i8")]
             )
         else:
             raise ValueError("DirectAccess File Version '{version}' not understood.")
         return header_dtype, dir_dtype
@@ -159,15 +156,15 @@
 
         major, minor = int(version_string[26]), int(version_string[28:30])
         version = (major, minor)
         return version
 
     @classmethod
     def read_header(cls, fname: str):
-        """parse Header data"""
+        """ parse Header data """
         with open(fname, "rb") as file:
             version_dtype = "S64"
             version = np.fromfile(file, version_dtype, count=1)
             version = cls.read_version(version[0])
             header_dtype, dir_dtype = cls.get_dtypes(version)
             header = np.fromfile(file, header_dtype, count=1)
             ndir = int(header["ndir"][0])
@@ -175,16 +172,15 @@
 
         # Decode bytes to strings
         key = directory["key"]
         key = np.char.strip(np.char.decode(key))
         # Get relevant info from size parameter
         # ndim, n1, n2, ..., typecode, size
         dtype = np.array(
-            [cls.idl_typecode(d[1 + d[0]]) for d in directory["size"]],
-            dtype="U5",
+            [cls.idl_typecode(d[1 + d[0]]) for d in directory["size"]], dtype="U5",
         )
         shape = np.empty(ndir, dtype=object)
         shape[:] = [tuple(d[1 : d[0] + 1]) for d in directory["size"]]
         # Pointer to data arrays
         pointer = directory["pointer"]
 
         # Bytes (which represent strings) get special treatment to get the dimensions right
@@ -247,15 +243,16 @@
             directory.tofile(file)
 
             for i, value in enumerate(kwargs.values()):
                 value.tofile(file)
 
 
 class Grid:
-    """NLTE Grid class that handles all NLTE data reading and interpolation"""
+    """NLTE Grid class that handles all NLTE data reading and interpolation
+    """
 
     def __init__(
         self,
         sme,
         elem,
         lfs_nlte,
         selection="energy",
@@ -265,18 +262,16 @@
     ):
         #:str: Element of the NLTE grid
         self.elem = elem
         #:LineList: Whole LineList that was passed to the C library
         self.linelist = sme.linelist
         #:array(str): Elemental Species Names for the linelist
         self.species = sme.linelist.species
-        #:str: Name of the grid
-        self.grid_name = sme.nlte.grids[elem]
         #:str: complete filename of the NLTE grid data file
-        self.fname = lfs_nlte.get(self.grid_name)
+        self.fname = lfs_nlte.get(sme.nlte.grids[elem])
         #:{"levels", "energy"}: Selection algorithm to match lines in grid with linelist
         self.selection = selection
         #:float: Minimum difference between energy levels to match, only relevant for selection=='energy'
         self.min_energy_diff = min_energy_diff
 
         #:DirectAccessFile: The NLTE data file
         self.directory = DirectAccessFile(self.fname)
@@ -294,16 +289,16 @@
         self._teff = self.directory["teff"]
         self._grav = self.directory["grav"]
         self._feh = self.directory["feh"]
         self._xfe = self.directory["abund"]
         # The position of the models in the datafile
         self._keys = self.directory["models"].astype("U")
 
-        depth_name = str.lower(sme.atmo.interp)
         try:
+            depth_name = str.lower(sme.atmo.interp)
             depth = self.directory[depth_name]
         except KeyError:
             other_depth_name = "tau" if depth_name == "rhox" else "rhox"
             depth = self.directory[other_depth_name]
             logger.warning(
                 f"No data for {depth_name} in NLTE grid for {self.elem} found, using {other_depth_name} instead."
             )
@@ -342,53 +337,42 @@
         self.lineindices = None
         #:array: Indices of the lines in the bgrid
         self.iused = None
 
         #:str: citations in bibtex format, if known
         self.citation_info = ""
 
-        self.first_warning = True
-
         conf = self.directory["conf"].astype("U")
         term = self.directory["term"].astype("U")
-        try:
-            species = self.directory["spec"].astype("U")
-        except KeyError:
-            logger.warning(
-                "Could not find 'species' field in NLTE file %s. Assuming they are all '%s 1'.",
-                self.grid_name,
-                self.elem,
-            )
-            species = np.full(conf.shape, "%s 1" % self.elem)
-            pass
+        species = self.directory["spec"].astype("U")
         rotnum = self.directory["J"]  # rotational number of the atomic state
         if self.version[0] == 1 and self.version[1] >= 10:
             energies = self.directory["energy"]  # energy in eV
             self.citation_info = self.directory["citation"][()].decode()
         else:
             self.citation_info = None
             if self.selection != "levels":
-                # logger.warning(
-                #     "NLTE grid file version %s only supports level selection, not %s",
-                #     self.version,
-                #     self.selection,
-                # )
+                logger.warning(
+                    "NLTE grid file version %s only supports level selection, not %s",
+                    self.version,
+                    self.selection,
+                )
                 self.selection = "levels"
 
         if self.selection == "levels":
             self.lineindices, self.linerefs, self.iused = self.select_levels(
                 conf, term, species, rotnum
             )
         elif self.selection == "energy":
             self.lineindices, self.linerefs, self.iused = self.select_energies(
                 conf, term, species, rotnum, energies
             )
 
     def solar_rel_abund(self, abund, elem):
-        """Get the abundance of elem relative to H, i.e. [X/H]"""
+        """ Get the abundance of elem relative to H, i.e. [X/H] """
         if self.abund_format == "H=12":
             # Its a bit more efficient, to simply use the values as is, instead of converting everything
             # just to end up back here
             idx = abund.elem_dict[elem]
             a = abund._pattern[idx]
             s = self.solar._pattern[idx]
             h = sh = 12
@@ -398,15 +382,15 @@
             s = self.solar.get_element(elem, type=self.abund_format)
             sh = self.solar.get_element("H", type=self.abund_format)
 
         rabund = (a - h) - (s - sh)
         return rabund
 
     def scaled_rel_abund(self, abund):
-        """Get the abundance of self.elem relative to Fe, i.e. [X/Fe]"""
+        """ Get the abundance of self.elem relative to Fe, i.e. [X/Fe] """
         sel = self.solar_rel_abund(abund, self.elem)
         sfe = self.solar_rel_abund(abund, "Fe")
         rabund = sel - sfe
         return rabund
 
     def get(self, abund, teff, logg, monh, atmo):
         rabund = self.scaled_rel_abund(abund)
@@ -418,15 +402,15 @@
             and (self.limits["feh"][0] <= monh <= self.limits["feh"][-1])
         ):
             _ = self.read_grid(rabund, teff, logg, monh)
 
         return self.interpolate(rabund, teff, logg, monh, atmo)
 
     def read_grid(self, rabund, teff, logg, monh):
-        """Read the NLTE coefficients from the nlte_grid files for the given element
+        """ Read the NLTE coefficients from the nlte_grid files for the given element
         The class will cache subgrid_size points around the target values as well
 
         Parameters
         ----------
         rabund : float
             relative (to solar) abundance of the element
         teff : float
@@ -462,19 +446,15 @@
         nabund = len(x)
         nteff = len(t)
         ngrav = len(g)
         nfeh = len(f)
 
         self.bgrid = np.zeros((ndepths, nlevel, nabund, nteff, ngrav, nfeh))
 
-        for i, j, k, l in tqdm(
-            np.ndindex(nabund, nteff, ngrav, nfeh),
-            desc="Loading NLTE %s" % self.elem,
-            total=nabund * nteff * ngrav * nfeh,
-        ):
+        for i, j, k, l in np.ndindex(nabund, nteff, ngrav, nfeh):
             model = self._keys[f[l], g[k], t[j], x[i]]
             try:
                 self.bgrid[:, :, i, j, k, l] = self.directory[model]
             except KeyError:
                 warnings.warn(
                     f"Missing Model for element {self.elem}: T={self._teff[t[j]]}, logg={self._grav[g[k]]}, feh={self._feh[f[l]]}, abund={self._xfe[x[i]]:.2f}"
                 )
@@ -488,20 +468,15 @@
         # Remap the previous indices into a collapsed sequence
         # level_labels = level_labels[iused]
         if self.iused is not None:
             self.bgrid = self.bgrid[self.iused, ...]
         else:
             self.bgrid = self.bgrid[False]
 
-        self._points = (
-            self._xfe[x],
-            self._teff[t],
-            self._grav[g],
-            self._feh[f],
-        )
+        self._points = (self._xfe[x], self._teff[t], self._grav[g], self._feh[f])
         self.limits = {
             "teff": self._points[1][[0, -1]],
             "grav": self._points[2][[0, -1]],
             "feh": self._points[3][[0, -1]],
             "xfe": self._points[0][[0, -1]],
         }
 
@@ -543,25 +518,23 @@
         iused : array of shape (nl,)
             Indices used in the subgrid
         """
 
         lineindices = np.asarray(self.species, "U")
         lineindices = np.char.startswith(lineindices, self.elem)
         if not np.any(lineindices):
-            logger.warning(f"No NLTE transitions for {self.elem} found")
+            warnings.warn(f"No NLTE transitions for {self.elem} found")
             return None, None, np.full(len(species), False)
 
         sme_species = self.species[lineindices]
 
         # Extract data from linelist
         low = self.linelist["term_lower"][lineindices]
         upp = self.linelist["term_upper"][lineindices]
         # Remove quotation marks (if any are there)
-        low = low.astype(str)
-        upp = upp.astype(str)
         low = np.char.replace(low, "'", "")
         upp = np.char.replace(upp, "'", "")
         # Get only the relevant part
         parts_low = np.char.partition(low, " ")[:, (0, 2)]
         parts_upp = np.char.partition(upp, " ")[:, (0, 2)]
 
         # Transform into term symbol J (2*S+1) ?
@@ -577,20 +550,18 @@
             ("species", sme_species.dtype),
             ("configuration", parts_upp.dtype),
             ("term", parts_upp.dtype),
             ("J", extra.dtype),
         ]
         level_labels = np.rec.fromarrays((species, conf, term, rotnum), dtype=dtype)
         line_label_low = np.rec.fromarrays(
-            (sme_species, parts_low[:, 0], parts_low[:, 1], extra[:, 0]),
-            dtype=dtype,
+            (sme_species, parts_low[:, 0], parts_low[:, 1], extra[:, 0]), dtype=dtype
         )
         line_label_upp = np.rec.fromarrays(
-            (sme_species, parts_upp[:, 0], parts_upp[:, 1], extra[:, 1]),
-            dtype=dtype,
+            (sme_species, parts_upp[:, 0], parts_upp[:, 1], extra[:, 1]), dtype=dtype
         )
 
         # Prepare arrays
         nlines = parts_low.shape[0]
         linerefs = np.full((nlines, 2), -1)
         iused = np.zeros(len(species), dtype=bool)
 
@@ -614,20 +585,20 @@
         return lineindices, linerefs, iused
 
     def select_energies(self, conf, term, species, rotnum, energies):
         lineindices = np.asarray(self.species, "U")
         lineindices = np.char.startswith(lineindices, self.elem)
         if not np.any(lineindices):
             logger.warning("No NLTE transitions for %s found", self.elem)
-            return None, None, np.full(len(species), False)
+            return [], [], []
         sme_species = self.species[lineindices]
 
         # Extract data from linelist
-        term_low = self.linelist["term_lower"][lineindices].astype(str)
-        term_upp = self.linelist["term_upper"][lineindices].astype(str)
+        term_low = self.linelist["term_lower"][lineindices]
+        term_upp = self.linelist["term_upper"][lineindices]
         # Remove quotation marks (if any are there)
         term_low = np.char.replace(term_low, "'", "")
         term_upp = np.char.replace(term_upp, "'", "")
         # Split the string into configuration and term
         term_low = np.char.partition(term_low, " ")
         term_upp = np.char.partition(term_upp, " ")
         # Remove whitespaces
@@ -669,15 +640,15 @@
             (sme_species, conf_upp, term_upp, j_upp, energy_upp), dtype=dtype
         )
 
         nlines = term_low.shape[0]  # np.count_nonzero(lineindices)
         linerefs = np.full((nlines, 2), -1)
         iused = np.zeros(len(species), dtype=bool)
 
-        idx_map = np.arange(len(species))
+        idx_map = np.arange(nlines)
         # Maximum energy in the grid
         max_energy = np.max(energies)
         # Maximum seperation between energy levels
         if self.min_energy_diff is None:
             diff = np.abs(np.diff(energies))
             energy_diff_limit = np.min(diff[diff != 0])
         else:
@@ -779,73 +750,45 @@
         # Interpolate the depth scale to the target depth, this is unstructured data
         # i.e. each combination of parameters has a different depth scale (given in depth)
         ndepths, _, *nparam = self.bgrid.shape
         target_depth = atmo[self.depth_name]
         target_depth = np.log10(target_depth)
         ntarget = len(target_depth)
 
-        param = [rabund, teff, logg, monh]
-        right = [
-            (self._points[i][-1] == p) and len(self._points[i] > 1)
-            for i, p in enumerate(param)
-        ]
-        iabund = np.digitize(rabund, self._points[0], right=right[0]) - 1
-        iteff = np.digitize(teff, self._points[1], right=right[1]) - 1
-        ilogg = np.digitize(logg, self._points[2], right=right[2]) - 1
-        imonh = np.digitize(monh, self._points[3], right=right[3]) - 1
+        # TODO: We only need to interpolate the closest 2**4 grids, and not all of them
+        grid = np.empty((*nparam, ntarget, ndepths), float)
+        for l, x, t, g, f in np.ndindex(ndepths, *nparam):
+            xp = self.depth[f, g, t, :]
+            yp = self.bgrid[l, :, x, t, g, f]
 
-        # Interpolate on the grid
-        # We only interpolate on the 2**4 points around the requested values
-        # self._points and self._grid are interpolated when reading the data in read_grid
-        target = (rabund, teff, logg, monh)
-        points = (
-            self._points[0][iabund : iabund + 2],
-            self._points[1][iteff : iteff + 2],
-            self._points[2][ilogg : ilogg + 2],
-            self._points[3][imonh : imonh + 2],
-        )
-        npoints = (
-            max(points[0].size, 1),
-            max(points[1].size, 1),
-            max(points[2].size, 1),
-            max(points[3].size, 1),
-        )
-
-        grid = np.empty((*npoints, ntarget, ndepths), float)
-        for l, x, t, g, f in np.ndindex(ndepths, *npoints):
-            xp = self.depth[imonh + f, ilogg + g, iteff + t, :]
-            yp = self.bgrid[l, :, iabund + x, iteff + t, ilogg + g, imonh + f]
             xp = np.log10(xp)
             grid[x, t, g, f, :, l] = interpolate.interp1d(
-                xp,
-                yp,
-                bounds_error=False,
-                fill_value="extrapolate",
-                kind="cubic",
+                xp, yp, bounds_error=False, fill_value="extrapolate", kind="cubic",
             )(target_depth)
 
+        # Interpolate on the grid
+        # self._points and self._grid are interpolated when reading the data in read_grid
+        target = (rabund, teff, logg, monh)
+        points = self._points
+
         # Check if we need to extrapolate
-        if any(
-            [t < min(p) or t > max(p) for t, p in zip(target, points) if len(p) > 0]
-        ):
-            if self.first_warning:
-                logger.warning(
-                    f"Extrapolate on the {self.elem} NLTE grid. Requested values of {target} on grid {points}"
-                )
-                self.first_warning = False
+        if any([t < min(p) or t > max(p) for t, p in zip(target, points)]):
+            logger.warning(
+                f"Extrapolate on the {self.elem} NLTE grid. Requested values of {target} on grid {points}"
+            )
 
         # Some grids have only one value in that direction
         # Usually in abundance. Then we need to remove that dimension
         # to avoid nan output
         mask = [len(p) > 1 for p in points]
         if not all(mask):
             points = [p for m, p in zip(mask, points) if m]
             target = [t for m, t in zip(mask, target) if m]
             idx = [slice(None, None) if m else 0 for m in mask]
-            grid = grid[tuple(idx)]
+            grid = grid[idx]
 
         method = "order"
         if method == "grid":
             # TODO: Interpolate with splines
             # Possibly in order of importance, since scipy doesn't have spline interpolation on a grid
             subgrid = interpolate.interpn(
                 points,
@@ -855,33 +798,29 @@
                 bounds_error=False,
                 fill_value=None,
             )
             subgrid = subgrid[0]
         elif method == "order":
             for p, t in zip(points, target):
                 grid = interpolate.interp1d(
-                    p,
-                    grid,
-                    axis=0,
-                    bounds_error=False,
-                    fill_value="extrapolate",
+                    p, grid, axis=0, bounds_error=False, fill_value="extrapolate",
                 )(t)
             subgrid = grid
         return subgrid
 
 
 @CollectionFactory
 class NLTE(Collection):
     # fmt: off
     _fields = Collection._fields + [
         ("elements", [], astype(list), this,
             "list: elements for which nlte calculations will be performed"),
         ("grids", {}, astype(dict), this,
             "dict: nlte grid datafiles for each element"),
-        ("subgrid_size", [3, 3, 3, 3], array(4, int), this,
+        ("subgrid_size", [2, 2, 2, 2], array(4, int), this,
             "array of shape (4,): defines size of nlte grid cache."
             "Each entry is for one parameter abund, teff, logg, monh"),
         ("flags", None, array(None, np.bool_), this,
             "array: contains a flag for each line, whether it was calculated in NLTE (True) or not (False)"),
         ("solar", None, this, this, "str: defines which default to use as the solar metallicitiies"),
         ("abund_format", "H=12", astype(str), this, "str: which abundance format to use for comparison"),
         ("selection", "energy", oneof("energy", "levels"), this, "str: which selection algorithm to use to match linelist and departure coefficients"),
@@ -905,15 +844,15 @@
         "H": "nlte_H_ama51_pysme.grd",
         "K": "nlte_K_ama51_pysme.grd",
         "Mn": "nlte_Mn_ama51_pysme.grd",
         "N": "nlte_N_ama51_pysme.grd",
     }
 
     def __init__(self, **kwargs):
-        super().__init__(**kwargs)
+        super().__init__()
         self.first = False
 
         if "solar" in kwargs.keys():
             self.solar = kwargs["solar"]
 
         # Convert IDL keywords to Python
         if "nlte_elem_flags" in kwargs.keys():
@@ -997,15 +936,15 @@
         return citations
 
     @_citation_info.setter
     def _citation_info(self, value):
         pass
 
     def update_coefficients(self, sme, dll, lfs_nlte):
-        """pass departure coefficients to C library"""
+        """ pass departure coefficients to C library """
 
         # Only print "Running in NLTE" message on the first run each time
         if np.all(self.grids == "") or np.size(self.elements) == 0:
             # No NLTE to do
             if self.first:
                 self.first = False
                 logger.info("Running in LTE")
@@ -1025,53 +964,37 @@
         dll.ResetNLTE()
 
         if self.first:
             self.first = False
             logger.info("Running in NLTE: %s", ", ".join(self.elements))
 
         # Call each element to update and return its set of departure coefficients
-        marked_for_removal = []
         for elem in self.elements:
             # Call function to retrieve interpolated NLTE departure coefficients
             # the abundances for NLTE are handled in the H-12 format
             grid = self.get_grid(sme, elem, lfs_nlte)
-            if not np.any(grid.iused):
-                # No lines are found for this element
-                # remove it from the elements after this loop
-                logger.warning(
-                    "No %s NLTE lines found, removing it from NLTE calculations",
-                    elem,
-                )
-                marked_for_removal += [elem]
-                continue
             bmat = grid.get(sme.abund, sme.teff, sme.logg, sme.monh, sme.atmo)
+
             if bmat is None or grid.linerefs.size == 0:
-                logger.warning(
-                    "No %s NLTE lines found, removing it from NLTE calculations",
-                    elem,
-                )
-                marked_for_removal += [elem]
-                continue
+                # no data were returned. Don't bother?
+                logger.warning(f"No NLTE transitions found for {elem}")
             else:
                 # Put corrections into the nlte_b matrix, don't cache the data
                 for lr, li in zip(grid.linerefs, grid.lineindices):
                     # loop through the list of relevant _lines_, substitute both their levels into the main b matrix
                     # Make sure both levels have corrections available
                     if lr[0] != -1 and lr[1] != -1:
-                        dll.InputNLTE(bmat[:, lr].T, li)
-
-        for elem in marked_for_removal:
-            self.remove_nlte(elem)
+                        dll.InputNLTE(bmat[:, lr], li)
 
         # flags = sme_synth.GetNLTEflags(sme.linelist)
 
         return sme
 
     def get_grid(self, sme, elem, lfs_nlte):
-        """Read and interpolate the NLTE grid for the current element and parameters"""
+        """ Read and interpolate the NLTE grid for the current element and parameters """
         if self.grids[elem] is None:
             raise ValueError(f"Element {elem} has not been prepared for NLTE")
 
         # The grids are cached in the NLTE object, but not saved
         if elem in self.grid_data.keys():
             grid = self.grid_data[elem]
         else:
@@ -1087,16 +1010,16 @@
             self.grid_data[elem] = grid
 
         return grid
 
 
 # These are kept here for compatibility, but it is recommended to use the functions of sme.nlte
 def nlte(sme, dll, elem, lfs_nlte):
-    """Read and interpolate the NLTE grid for the current element and parameters"""
+    """ Read and interpolate the NLTE grid for the current element and parameters """
     grid = sme.nlte.get_grid(sme, elem, lfs_nlte)
     subgrid = grid.get(sme.abund, sme.teff, sme.logg, sme.monh, sme.atmo)
     return subgrid, grid.linerefs, grid.lineindices
 
 
 def update_nlte_coefficients(sme, dll, lfs_nlte):
-    """pass departure coefficients to C library"""
+    """ pass departure coefficients to C library """
     return sme.nlte.update_coefficients(sme, dll, lfs_nlte)
```

### Comparing `pysme-astro-0.4.99/src/pysme/persistence.py` & `pysme-astro-5.74.9/src/pysme/persistence.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,32 @@
-# -*- coding: utf-8 -*-
 import io
-import json
-import logging
 import os
-import subprocess
-import sys
+import logging
+from zipfile import ZipFile, ZIP_STORED, ZIP_LZMA
+import json
 import tempfile
-from zipfile import ZIP_LZMA, ZIP_STORED, ZipFile
-
-import numpy as np
-from flex.flex import FlexExtension, FlexFile
+import sys
+import subprocess
 
+from flex.flex import FlexFile
 from . import __version__
 
+import numpy as np
+
 logger = logging.getLogger(__name__)
 
 
 def to_flex(sme):
     header = {}
     extensions = {}
 
     for name in sme._names:
         value = sme[name]
         if isinstance(value, IPersist):
             extensions[name] = value._save()
-        elif isinstance(value, FlexExtension):
-            extensions[name] = value
         elif value is not None:
             header[name] = value
 
     ff = FlexFile(header, extensions)
     return ff
 
 
@@ -38,59 +35,37 @@
     extensions = ff.extensions
     for name in sme._names:
         if name in updates.keys():
             name = updates[name]
         if name in header.keys():
             sme[name] = header[name]
         elif name in extensions.keys():
-            if sme[name] is not None and isinstance(sme[name], IPersist):
+            if sme[name] is not None:
                 sme[name] = sme[name]._load(extensions[name])
             else:
                 sme[name] = extensions[name]
     return sme
 
 
-def save(filename, sme, format="flex", _async=False):
+def save(fname, sme, compressed=False):
     """
     Create a folder structure inside a tarfile
     See flex-format for details
 
     Parameters
     ----------
     filename : str
         Filename of the final file
     sme : SME_Structure
         sme structure to save
     compressed : bool, optional
         whether to compress the output
     """
     ff = to_flex(sme)
-
-    if format == "flex":
-        file_ending = ".sme"
-    else:
-        file_ending = "." + format
-    if not filename.endswith(file_ending):
-        filename = filename + file_ending
-
-    if format == "flex":
-        if _async:
-            ff.write_async(filename)
-        else:
-            ff.write(filename)
-    elif format == "fits":
-        ff.to_fits(filename, overwrite=True)
-    elif format == "json":
-        ff.to_json(filename)
-    else:
-        raise ValueError(
-            "Format {!r} not understood, expected one of ['flex', 'fits', 'json'].".format(
-                format
-            )
-        )
+    ff.write(fname)
 
 
 def load(fname, sme):
     """
     Load the SME Structure from disk
 
     Parameters
@@ -278,15 +253,15 @@
     return data
 
 
 # IDL IO
 
 
 def get_typecode(dtype):
-    """Get the IDL typecode for a given dtype"""
+    """ Get the IDL typecode for a given dtype """
     if dtype.name[:5] == "bytes":
         return "1"
     if dtype.name == "int16":
         return "2"
     if dtype.name == "int32":
         return "3"
     if dtype.name == "float32":
@@ -304,18 +279,14 @@
 def save_as_binary(arr):
     global temps_to_clean
 
     with tempfile.NamedTemporaryFile("w+", suffix=".dat", delete=False) as temp:
         if arr.dtype.name[:3] == "str" or arr.dtype.name == "object":
             arr = arr.astype(bytes)
             shape = (arr.dtype.itemsize, len(arr))
-        elif np.issubdtype(arr.dtype, np.floating):
-            # SME expects double precision, so we assure that here
-            arr = arr.astype("float64")
-            shape = arr.shape[::-1]
         else:
             shape = arr.shape[::-1]
 
         # Most arrays should be in the native endianness anyway
         # But if not we swap it to the native representation
         endian = arr.dtype.str[0]
         if endian == "<":
@@ -344,38 +315,35 @@
             pass
 
     temps_to_clean = []
 
 
 def write_as_idl(sme):
     """
-    Write SME structure into and idl format
+    Write SME structure into and idl format 
     data arrays are stored in seperate temp files, and only the filename is passed to idl
     """
 
     vrad_flag = {"none": -2, "whole": -1, "each": 0, "fix": -2}[sme.vrad_flag]
-    # cscale_flag = {"none": -3, "fix": -3, "constant": 0, "linear": 1, "quadratic": 1, }[
-    #     sme.cscale_flag
-    # ]
-    # if not sme.normalize_by_continuum:
-    #     cscale_flag = -2
+    cscale_flag = {"none": -3, "fix": -3, "constant": 0, "linear": 1, "quadratic": 1,}[
+        sme.cscale_flag
+    ]
+    if not sme.normalize_by_continuum:
+        cscale_flag = -2
 
     abund = sme.abund.get_pattern(type="sme", raw=True)
     abund[np.isnan(abund)] = -99
 
     fitvars = ["TEFF", "GRAV", "FEH", "VMIC", "VMAC", "VSINI", "GAM6", "VRAD"]
     fitvars = [s.upper() for s in sme.fitparameters if s.upper() in fitvars]
     if "logg" in sme.fitparameters:
         fitvars += ["GRAV"]
     if "monh" in sme.fitparameters:
         fitvars += ["FEH"]
 
-    if sme.mask is None:
-        sme.mask = 1
-
     idl_fields = {
         "version": 5.1,
         "id": sme.id,
         "teff": sme.teff,
         "grav": sme.logg,
         "feh": sme.monh,
         "vmic": float(sme.vmic),
@@ -400,15 +368,15 @@
         "lande": save_as_binary(sme.linelist.lande),
         "lineref": save_as_binary(sme.linelist.reference),
         "short_line_format": {"short": 1, "long": 2}[sme.linelist.lineformat],
         "wran": sme.wran.tolist(),
         "mu": sme.mu.tolist() if sme.nmu > 1 else sme.mu[0],
         "obs_name": "",
         "obs_type": 0,
-        "glob_free": fitvars if len(fitvars) != 0 else "",
+        "glob_free": fitvars,
         "atmo": {
             "method": str(sme.atmo.method),
             "source": str(sme.atmo.source),
             "depth": str(sme.atmo.depth),
             "interp": str(sme.atmo.interp),
             "geom": str(sme.atmo.geom),
         },
@@ -426,22 +394,19 @@
         idl_fields["nlte"]["nlte_elem_flags"] = save_as_binary(flags)
         idl_fields["nlte"]["nlte_subgrid_size"] = save_as_binary(
             sme.nlte.subgrid_size.astype("int16")
         )
         idl_fields["nlte"]["nlte_grids"] = grids
         idl_fields["nlte"]["nlte_pro"] = "sme_nlte"
 
-    if sme.iptype is not None:
-        idl_fields["iptype"] = sme.iptype
-        idl_fields["ipres"] = sme.ipres[0]
-        # "ip_x": sme.ip_x,
-        # "ip_y": sme.ip_y,
-    else:
-        idl_fields["iptype"] = "gauss"
-        idl_fields["ipres"] = 0
+    # if sme.iptype is not None:
+    #     idl_fields["iptype"] = sme.iptype
+    #     idl_fields["ipres"] = sme.ipres
+    #     # "ip_x": sme.ip_x,
+    #     # "ip_y": sme.ip_y,
 
     if sme.wave is not None:
         wind = np.cumsum(sme.wave.shape[1]) - 1
         idl_fields["wave"] = save_as_binary(sme.wave.ravel())
         idl_fields["wind"] = wind.tolist()
     if sme.spec is not None:
         idl_fields["sob"] = save_as_binary(sme.spec.ravel())
@@ -468,15 +433,15 @@
         )
 
     sep = ""
     text = ""
 
     for key, value in idl_fields.items():
         if isinstance(value, dict):
-            text += f"{sep}{key!s}:{{{key!s},$\n"
+            text += f"{sep}{key!s}:{{$\n"
             sep = ""
             for key2, value2 in value.items():
                 text += f"{sep}{key2!s}:{value2!r}$\n"
                 sep = ","
             sep = ","
             text += "}$\n"
         else:
@@ -497,15 +462,15 @@
     structure need to be transformed into simple idl readable structures.
     All large arrays are stored in seperate binary files, for performance.
     The script then reads those files back into idl.
     """
     with tempfile.NamedTemporaryFile("w+", suffix=".pro") as temp:
         tempname = temp.name
         temp.write("print, 'Hello'\n")
-        temp.write("sme = {sme,")
+        temp.write("sme = {")
         # TODO: Save data as idl compatible data
         temp.write(write_as_idl(sme))
         temp.write("} \n")
         # This is the code that will be run in idl
         temp.write("print, 'there'\n")
         temp.write(
             """tags = tag_names(sme)
@@ -554,11 +519,10 @@
 sme = new_sme\n"""
         )
         temp.write(f'save, sme, filename="{fname}"\n')
         temp.write("end\n")
         temp.flush()
 
         # with open(os.devnull, 'w') as devnull:
-        print("IDL Script: ", tempname)
         subprocess.run(["idl", "-e", ".r %s" % tempname])
         # input("Wait for me...")
         clean_temps()
```

### Comparing `pysme-astro-0.4.99/src/pysme/sme.py` & `pysme-astro-5.74.9/src/pysme/sme.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-# -*- coding: utf-8 -*-
 import logging
 import os.path
 import platform
 import sys
+from copy import copy
 from datetime import datetime as dt
 
 import numpy as np
-from scipy.constants import speed_of_light
 from scipy.io import readsav
 
 from . import __file_ending__, __version__, echelle, persistence
-from .abund import Abund
-from .abund import elements as abund_elem
+from .abund import Abund, elements as abund_elem
 from .atmosphere.atmosphere import Atmosphere
-from .data_structure import *
 from .iliffe_vector import Iliffe_vector
 from .linelist.linelist import LineList
 from .nlte import NLTE
 
+from .data_structure import *
+
 logger = logging.getLogger(__name__)
 
 
 @CollectionFactory
 class Parameters(Collection):
     # fmt: off
     _fields = Collection._fields + [
@@ -48,18 +47,17 @@
 
     @_abund.setter
     def _abund(self, value):
         if isinstance(value, Abund):
             self.__abund = value
         else:
             logger.warning(
-                "Abundance set using just a pattern, assuming that "
-                "it has format %s. "
-                "If that is incorrect, try changing the format first.",
-                self.__abund.type,
+                "Abundance set using just a pattern, assuming that"
+                f"it has format {self.__abund.type}."
+                "If that is incorrect, try changing the format first."
             )
             self.__abund = Abund(monh=self.monh, pattern=value, type=self.__abund.type)
 
     @property
     def monh(self):
         """float: metallicity in log scale relative to the base abundances"""
         return self.abund.monh
@@ -87,44 +85,44 @@
     ]
     # fmt: on
 
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
     def update(self):
-        """Update version info with current machine data"""
+        """ Update version info with current machine data """
         self.arch = platform.machine()
         self.os = sys.platform
         self.os_family = platform.system()
         self.os_name = platform.version()
         self.release = platform.python_version()
         self.build_date = platform.python_build()[1]
         self.memory_bits = int(platform.architecture()[0][:2])
         self.host = platform.node()
 
 
 @CollectionFactory
 class Fitresults(Collection):
     # fmt: off
     _fields = Collection._fields + [
-        ("iterations", None, astype(int, allow_None=True), this, "int: maximum number of iterations in the solver"),
+        ("maxiter", None, astype(int, allow_None=True), this, "int: maximum number of iterations in the solver"),
         ("chisq", None, this, this, "float: reduced chi-square of the solution"),
         ("parameters", None, this, this, "list: parameter names"),
         ("values", None, array(None, float), this, "array: best fit values for the fit parameters"),
         ("uncertainties", None, array(None, float), this, "array of size(nfree,): uncertainties of the free parameters bases on SME statistics"),
         ("covariance", None, array(None, float), this, "array of size (nfree, nfree): covariance matrix"),
         ("gradient", None, array(None, float), this, "array of size (nfree,): final gradients of the free parameters on the cost function"),
         ("derivative", None, array(None, float), this, "array of size (npoints, nfree): final Jacobian of each point and each parameter"),
         ("residuals", None, array(None, float), this, "array of size (npoints,): final residuals of the fit"),
         ("fit_uncertainties", None, this, this, "array: uncertainties based solely on the least_squares fit")
     ]
     # fmt: on
 
     def clear(self):
-        """Reset all values to None"""
+        """ Reset all values to None """
         for name in self._names:
             default = [f[1] for f in self._fields if f[0] == name][0]
             setattr(self, name, default)
 
 
 @CollectionFactory
 class SME_Structure(Parameters):
@@ -138,55 +136,48 @@
 
             allowed values are:
                * "none": No radial velocity correction
                * "each": Determine radial velocity for each segment individually
                * "whole": Determine one radial velocity for the whole spectrum
             """),
         ("vrad", 0, array(None, float), this, "array of size (nseg,): radial velocity of each segment in km/s"),
-        ("vrad_limit", 500, asfloat, this, "float: radial velocity limit in km/s"),
-        ("cscale_flag", "none", lowercase(oneof("none", "fix", "constant", "linear", "quadratic", "cubic", "quintic", "quantic", astype=int)), this,
+        ("cscale_flag", "none", lowercase(oneof(-3, -2, -1, 0, 1, 2, 3, 4, 5, "none", "fix", "constant", "linear", "quadratic", "cubic", "quintic", "quantic")), this,
             """str: Flag that describes how to correct for the continuum
 
             allowed values are:
                 * "none": No continuum correction
                 * "fix": Use whatever continuum scale has been set, but don't change it
                 * "constant": Zeroth order polynomial, i.e. scale everything by a factor
                 * "linear": First order polynomial, i.e. approximate continuum by a straight line
                 * "quadratic": Second order polynomial, i.e. approximate continuum by a quadratic polynomial
             """),
-        ("cscale_type", "match+mask", lowercase(oneof("mcmc", "mask", "match", "match+mask", "matchlines", "matchlines+mask", "spline", "spline+mask")), this,
+        ("cscale_type", "whole", lowercase(oneof("whole", "mask")), this,
             """str: Flag that determines the algorithm to determine the continuum
 
             This is used in combination with cscale_flag, which determines the degree of the fit, if any.
 
             allowed values are:
               * "whole": Fit the whole synthetic spectrum to the observation to determine the best fit
               * "mask": Fit a polynomial to the pixels marked as continuum in the mask
             """),
-        ("cscale", None, this, this,
+        ("cscale", 1, array(None, float), this,
             """array of size (nseg, ndegree): Continumm polynomial coefficients for each wavelength segment
             The x coordinates of each polynomial are chosen so that x = 0, at the first wavelength point,
             i.e. x is shifted by wave[segment][0]
             """),
         ("normalize_by_continuum", True, asbool, this,
             "bool: Whether to normalize the synthetic spectrum by the synthetic continuum spectrum or not"),
         ("specific_intensities_only", False, asbool, this,
             "bool: Whether to keep the specific intensities or integrate them together"),
         ("gam6", 1, asfloat, this, "float: van der Waals scaling factor"),
         ("h2broad", True, asbool, this, "bool: Whether to use H2 broadening or not"),
         ("accwi", 3e-3, asfloat, this,
             "float: minimum accuracy for linear spectrum interpolation vs. wavelength."),
         ("accrt", 1e-4, asfloat, this,
             "float: minimum accuracy for synthethized spectrum at wavelength grid points in sme.wint."),
-        ("accxt", 1e-6, asfloat, this,
-            "float: minimum accuracy of the parameters in the fitting procedure"),
-        ("accft", 1e-3, asfloat, this,
-            "float: minimum accuracy of the best fit cost"),
-        ("accgt", 1e-4, asfloat, this,
-            "float: minimum accuracy of the gradient of the least squares fit"),
         ("iptype", None, lowercase(oneof(None, "gauss", "sinc", "table")), this, "str: instrumental broadening type"),
         ("ipres", 0, array(None, float), this, "float, array: Instrumental resolution for instrumental broadening"),
         ("ip_x", None, this, this, "array: Instrumental broadening table in x direction"),
         ("ip_y", None, this, this, "array: Instrumental broadening table in y direction"),
         ("mu", np.sqrt(0.5 * (2 * np.arange(7) + 1) / 7), array(None, float), this,
             """array of size (nmu,): Mu values to calculate radiative transfer at
             mu values describe the distance from the center of the stellar disk to the edge
@@ -197,15 +188,15 @@
             "array of size (nseg, 2): beginning and end wavelength points of each segment"),
         ("wave", None, vector, this,
             "Iliffe_vector of shape (nseg, ...): wavelength"),
         ("spec", None, vector, this,
             "Iliffe_vector of shape (nseg, ...): observed spectrum"),
         ("uncs", None, vector, this,
             "Iliffe_vector of shape (nseg, ...): uncertainties of the observed spectrum"),
-        ("telluric", None, vector, this,
+        ("telluric", None, vector, this, 
             "Illife_vector of shape (nseg, ...): telluric spectrum that is multiplied with synth during the fit"),
         ("mask", None, vector, this,
             "Iliffe_vector of shape (nseg, ...): mask defining good and bad points for the fit"),
         ("synth", None, vector, this,
             "Iliffe_vector of shape (nseg, ...): synthetic spectrum"),
         ("cont", None, vector, this,
             "Iliffe_vector of shape (nseg, ...): continuum intensities"),
@@ -229,16 +220,16 @@
         nlte = kwargs.pop("nlte", {})
         idlver = kwargs.pop("idlver", {})
         self.wave = None
         self.wran = None
         super().__init__(**kwargs)
 
         if wind is not None and self.wave is not None:
-            wind = wind + 1
-            self.wave = Iliffe_vector(self.wave.ravel(), offsets=wind)
+            wind = np.array([0, *(wind + 1)])
+            self.wave = Iliffe_vector(values=self.wave.ravel(), index=wind)
 
         self.spec = kwargs.get("sob", None)
         self.uncs = kwargs.get("uob", None)
         self.mask = kwargs.get("mob", None)
         self.synth = kwargs.get("smod", None)
 
         self.meta["object"] = kwargs.get("obs_name", "")
@@ -247,38 +238,36 @@
         except (KeyError, AttributeError):
             # TODO ignore the warning during loading of data
             logger.warning("No or incomplete linelist data present")
 
         # Parse free parameters into one list
         pname = kwargs.get("pname", [])
         glob_free = kwargs.get("glob_free", [])
-        if isinstance(glob_free, str):
-            glob_free = [glob_free]
         ab_free = kwargs.get("ab_free", [])
         if len(ab_free) != 0:
             ab_free = [f"abund {el}" for i, el in zip(ab_free, abund_elem) if i == 1]
         fitparameters = np.concatenate((pname, glob_free, ab_free)).astype("U")
         #:array of size (nfree): Names of the free parameters
         self.fitparameters = np.unique(fitparameters)
 
         self.fitresults = Fitresults(
-            iterations=kwargs.get("maxiter", None),
+            maxiter=kwargs.get("maxiter", None),
             chisq=kwargs.get("chisq", 0),
             uncertainties=kwargs.get("punc", None),
             covariance=kwargs.get("covar", None),
         )
 
         self.normalize_by_continuum = kwargs.get("cscale_flag", "") != "fix"
 
         self.system_info = Version(**idlver)
         atmo_abund = atmo.pop("abund", kwargs.get("abund", "empty"))
         atmo_monh = atmo.pop(
             "monh", atmo.pop("feh", kwargs.get("monh", kwargs.get("feh", 0)))
         )
-        self.atmo = Atmosphere(**atmo, abund=atmo_abund, monh=atmo_monh)
+        self.atmo = Atmosphere(**atmo, abund=atmo_abund, monh=atmo_monh,)
         self.nlte = NLTE(**nlte)
 
         self.citation_info = r"""
             @ARTICLE{2017A&A...597A..16P,
                 author = {{Piskunov}, Nikolai and {Valenti}, Jeff A.},
                 title = "{Spectroscopy Made Easy: Evolution}",
                 journal = {\aap},
@@ -412,17 +401,14 @@
 
     @property
     def _cscale(self):
         """array of size (nseg, ndegree): Continumm polynomial coefficients for each wavelength segment
         The x coordinates of each polynomial are chosen so that x = 0, at the first wavelength point,
         i.e. x is shifted by wave[segment][0]
         """
-        if self.cscale_type in ["spline", "spline+mask"]:
-            return self.__cscale
-
         nseg = self.nseg if self.nseg is not None else 1
 
         if self.__cscale is None:
             cs = np.zeros((nseg, self.cscale_degree + 1))
             cs[:, -1] = 1
             self.__cscale = cs
             return cs
@@ -451,47 +437,40 @@
         # since we might operate on that array
         self.__cscale = cs
 
         return self.__cscale
 
     @_cscale.setter
     def _cscale(self, value):
-        if self.cscale_type in ["spline", "spline+mask"]:
-            if not isinstance(value, Iliffe_vector):
-                self.__cscale = vector(self, value)
-            else:
-                self.__cscale = value
-        else:
-            self.__cscale = np.atleast_2d(value) if value is not None else None
+        self.__cscale = np.atleast_2d(value) if value is not None else None
 
     @property
     def _cscale_flag(self):
         try:
             _ = self.__cscale_flag
         except AttributeError:
             self.__cscale_flag = "none"
         return self.__cscale_flag
 
     @_cscale_flag.setter
     def _cscale_flag(self, value):
         if isinstance(value, (int, np.integer)):
-            try:
-                value = {
-                    -3: "none",
-                    -2: "fix",
-                    -1: "fix",
-                    0: "constant",
-                    1: "linear",
-                    2: "quadratic",
-                    3: "cubic",
-                    4: "quintic",
-                    5: "quantic",
-                }[value]
-            except KeyError:
-                value = value
+            value = {
+                -3: "none",
+                -2: "fix",
+                -1: "fix",
+                0: "constant",
+                1: "linear",
+                2: "quadratic",
+                3: "cubic",
+                4: "quintic",
+                5: "quantic",
+            }[value]
+        if value in ["quadratic", "cubic", "quintic", "quantic"]:
+            logger.warning(f"{value} continuum scale is experimental")
 
         self.__cscale_flag = value
 
     @property
     def _mu(self):
         return self.__mu
 
@@ -518,15 +497,15 @@
                 f"The instrument resolution must have 1 or {self.nseg} elements"
             )
         self.__ipres = value
 
     # Additional properties
     @property
     def nseg(self):
-        """int: Number of wavelength segments"""
+        """int: Number of wavelength segments """
         if self.wran is None:
             return 0
         else:
             return len(self.wran)
 
     @property
     def nmu(self):
@@ -558,52 +537,48 @@
     def mask_cont(self):
         if self.mask is None:
             return None
         return self.mask == self.mask_values["continuum"]
 
     @property
     def cscale_degree(self):
-        """int: Polynomial degree of the continuum as determined by cscale_flag"""
-        if self.cscale_type in ["spline", "spline+mask"]:
-            return self.wave.shape[1]
-        else:
-            if self.cscale_flag == "constant":
-                return 0
-            if self.cscale_flag == "linear":
-                return 1
-            if self.cscale_flag == "quadratic":
-                return 2
-            if self.cscale_flag == "cubic":
-                return 3
-            if self.cscale_flag == "quintic":
-                return 4
-            if self.cscale_flag == "quantic":
-                return 5
-            if self.cscale_flag == "fix":
-                # Use the underying element to avoid a loop
-                if self.__cscale is not None:
-                    return self.__cscale.shape[1] - 1
-                else:
-                    return 0
-            if self.cscale_flag == "none":
+        """int: Polynomial degree of the continuum as determined by cscale_flag """
+        if self.cscale_flag == "constant":
+            return 0
+        if self.cscale_flag == "linear":
+            return 1
+        if self.cscale_flag == "quadratic":
+            return 2
+        if self.cscale_flag == "cubic":
+            return 3
+        if self.cscale_flag == "quintic":
+            return 4
+        if self.cscale_flag == "quantic":
+            return 5
+        if self.cscale_flag == "fix":
+            # Use the underying element to avoid a loop
+            if self.__cscale is not None:
+                return self.__cscale.shape[1] - 1
+            else:
                 return 0
-            return self.cscale_flag
-            raise ValueError("This should never happen")
+        if self.cscale_flag == "none":
+            return 0
+        raise ValueError("This should never happen")
 
     @property
     def atomic(self):
         """array of size (nlines, 8): Atomic linelist data, usually passed to the C library
-        Use sme.linelist instead for other purposes"""
+        Use sme.linelist instead for other purposes """
         if self.linelist is None:
             return None
         return self.linelist.atomic
 
     @property
     def species(self):
-        """array of size (nlines,): Names of the species of each spectral line"""
+        """array of size (nlines,): Names of the species of each spectral line """
         if self.linelist is None:
             return None
         return self.linelist.species
 
     def __convert_cscale__(self):
         """
         Convert IDL SME continuum scale to regular polynomial coefficients
@@ -624,55 +599,39 @@
 
                 self.cscale[i] = [c0, c1]
         elif self.cscale_flag == "fix":
             self.cscale = self.cscale / np.sqrt(2)
         elif self.cscale_flag == "constant":
             self.cscale = np.sqrt(1 / self.cscale)
 
-    def import_mask(self, other, keep_bpm=False):
+    def import_mask(self, other):
         """
         Import the mask of another sme structure and apply it to this one
         Conversion is based on the wavelength
 
         Parameters
         ----------
         other : SME_Structure
             the sme structure to import the mask from
-
+        
         Returns
         -------
         self : SME_Structure
             this sme structure
         """
-        if self.mask is None:
-            self.mask = self.mask_values["line"]
-
-        c_light = speed_of_light * 1e-3  # speed of light in km/s
-        wave = other.wave.copy()
-        for i in range(len(wave)):
-            rvel = other.vrad[i]
-            rv_factor = np.sqrt((1 - rvel / c_light) / (1 + rvel / c_light))
-            wave[i] *= rv_factor
-        wave = wave.ravel()
-
+        wave = other.wave.ravel()
         line_mask = other.mask_line.ravel()
         cont_mask = other.mask_cont.ravel()
 
         for seg in range(self.nseg):
             # We simply interpolate between the masks, if most if the new pixel was
             # continuum / line mask then it will become that, otherwise bad
-            rvel = self.vrad[seg]
-            rv_factor = np.sqrt((1 - rvel / c_light) / (1 + rvel / c_light))
-            w = self.wave[seg] * rv_factor
+            w = self.wave[seg]
             cm = np.interp(w, wave, cont_mask) > 0.5
             lm = np.interp(w, wave, line_mask) > 0.5
-            if keep_bpm:
-                bpm = self.mask_bad[seg]
-                cm[bpm] = False
-                lm[bpm] = False
             self.mask[seg][cm] = self.mask_values["continuum"]
             self.mask[seg][lm] = self.mask_values["line"]
             self.mask[seg][~(cm | lm)] = self.mask_values["bad"]
         return self
 
     def citation(self, output="string"):
         """Create a citation string for use in papers, or
@@ -697,30 +656,32 @@
         citation += [self.abund.citation_info]
         citation += [self.linelist.citation_info]
         citation += [self.nlte.citation_info]
         citation = "\n".join(citation)
 
         return self.create_citation(citation, output=output)
 
-    def save(self, filename, format="flex", _async=False):
+    def save(self, filename, compressed=False):
         """Save the whole SME structure to disk.
 
         The file format is zip file, with one info.json
         file for simple values, and numpy save files for
         large arrays. Substructures (linelist, abundance, etc.)
         have their own folder within the zip file.
 
         Parameters
         ----------
         filename : str
             filename to save the structure at
         compressed : bool, optional
             whether to compress the output, by default False
         """
-        persistence.save(filename, self, format=format, _async=_async)
+        if not filename.endswith(__file_ending__):
+            filename = filename + __file_ending__
+        persistence.save(filename, self, compressed=compressed)
 
     @staticmethod
     def load(filename):
         """
         Load SME data from disk
 
         Currently supported file formats:
```

### Comparing `pysme-astro-0.4.99/src/pysme/sme_synth.py` & `pysme-astro-5.74.9/src/pysme/sme_synth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,23 @@
-# -*- coding: utf-8 -*-
 """ Wrapper for sme_synth.so C library """
-import logging
 import os
-from os.path import normpath
+from os.path import dirname, join
+import logging
 
 import numpy as np
 
-from .cwrapper import IDL_DLL, get_lib_name
-from .libtools import get_full_datadir
+from .cwrapper import get_lib_name, IDL_DLL
 
 logger = logging.getLogger(__name__)
 
 
 class SME_DLL:
-    """Object Oriented interface for the SME C library"""
+    """ Object Oriented interface for the SME C library """
 
-    def __init__(self, libfile=None, datadir=None, state=None):
+    def __init__(self, libfile=None, datadir=None):
         #:LineList: Linelist passed to the library
         self.linelist = None
         #:int: Number of mu points passed to the library
         self.nmu = None
         #:Abund: Elemental abundances passed to the library
         self.abund = None
         #:float: First wavelength of the current segment in Angstrom
@@ -35,69 +33,51 @@
         #:float: Surface gravity set in the model
         self.grav = None
         #:float: Turbulence velocity in the model in km/s
         self.vturb = None
         #:Atmo: Atmosphere structure in the model
         self.atmo = None
         #:dict: NLTE subgrids for nlte coefficient interpolation
-        self.nlte_grids = {}
+        self._nlte_grids = {}
         self.ion = None
 
         self.lib = IDL_DLL(libfile)
-
-        if self.interface == "Parallel":
-            self.parallel = True
-            if state is None:
-                self.state = self.NewState()
-            else:
-                self.state = state
-        else:
-            self.parallel = False
-            self.state = None
-
         self.SetLibraryPath(datadir)
-        self.check_data_files_exist()
 
-    def __del__(self):
-        # Free the memory from the state when this is closed
-        # self.FreeState()
-        pass
+        self.check_data_files_exist()
 
     @property
     def libfile(self):
         """str: Location of the library file"""
         return self.lib.libfile
 
     @property
-    def interface(self):
-        return self.lib.interface
+    def file(self):
+        """str: Location of the library file"""
+        # Deprecated
+        return self.libfile
 
     @property
     def datadir(self):
         """str: Expected directory of the data files"""
         return self.GetLibraryPath()
 
     @property
     def ndepth(self):
         """int: Number of depth layers in the atmosphere model"""
-        assert self.atmo is not None, "No model atmosphere has been set"
+        assert self.atmo is not None, f"No model atmosphere has been set"
         motype = self.atmo.depth
         return len(self.atmo[motype])
 
     @property
     def nlines(self):
         """int: number of lines in the linelist"""
-        assert self.linelist is not None, "No line list has been set"
+        assert self.linelist is not None, f"No line list has been set"
         return len(self.linelist)
 
-    @property
-    def file(self):
-        """str: (Expected) Location of the library file"""
-        return get_lib_name()
-
     def check_data_files_exist(self):
         """
         Checks if required data files for the SME library exist.
         If they dont exist, SME will just segfault, without any hint.
 
         Raises
         ------
@@ -106,89 +86,53 @@
         """
         names = self.GetDataFiles()
         directory = self.GetLibraryPath()
         for name in names:
             n = os.path.join(directory, name)
             if not os.path.exists(n):
                 raise FileNotFoundError(
-                    "Could not find required data file {name} in library directory {directory}".format(
-                        name=name, directory=directory
-                    )
+                    f"Could not find required data file {name} in library directory {directory}"
                 )
 
-    def NewState(self, delete_old=True):
-        # if delete_old and hasattr(self, "state") and self.state is not None:
-        #     self.FreeState()
-        self.state = self.lib.new_state()
-        return self.state
-
-    def FreeState(self):
-        pass
-        # if self.state is not None:
-        #     self.lib.free_state(self.state)
-        #     self.state = None
-
-    def CopyState(self):
-        if self.state is None:
-            return None
-        state = self.lib.copy_state(self.state)
-        return state
-
-    def copy(self):
-        return self.__copy__()
-
-    def __copy__(self):
-        cls = self.__class__
-        state = self.CopyState()
-        obj = cls(libfile=self.lib.libfile, datadir=self.datadir, state=state)
-        obj.parallel = self.parallel
-        obj.linelist = self.linelist
-        obj.nmu = self.nmu
-        obj.abund = self.abund
-        obj.wfirst = self.wfirst
-        obj.wlast = self.wlast
-        obj.vw_scale = self.vw_scale
-        obj.h2broad = self.h2broad
-        obj.teff = self.teff
-        obj.grav = self.grav
-        obj.vturb = self.vturb
-        obj.atmo = self.atmo
-        obj.nlte_grids = self.nlte_grids
-        obj.ion = self.ion
-        return obj
-
     def SMELibraryVersion(self):
         """
         Return SME library version
 
         Returns
         -------
         version : str
             SME library version
         """
-        version = self.lib.call(
-            "SMELibraryVersion", raise_error=False, state=self.state
-        )
+        version = self.lib.call("SMELibraryVersion", raise_error=False)
         return version
 
+    def SetLibraryPath(self, datadir=None):
+        """ Set the path to the library """
+        if datadir is None:
+            datadir = join(dirname(__file__), "share", "libsme")
+        datadir = str(datadir)
+        # Against all conventions, SME lib expects a "/" at the end of the path
+        if not datadir.endswith(os.sep):
+            datadir = datadir + os.sep
+        self.lib.SetLibraryPath(datadir, type="string")
+
     def GetLibraryPath(self):
-        """Get the data file directory"""
-        return self.lib.GetLibraryPath(raise_error=False, state=self.state)
+        """ Get the data file directory """
+        return self.lib.GetLibraryPath(raise_error=False)
 
     def GetDataFiles(self):
-        """Get the required data files"""
-        files = self.lib.GetDataFiles(raise_error=False, state=self.state)
-        return files.split(";")
-
-    def SetLibraryPath(self, libpath=None):
-        """Set the path to the library"""
-        if libpath is None:
-            libpath = get_full_datadir()
-        libpath = normpath(libpath) + os.sep
-        self.lib.SetLibraryPath(libpath, type="string", state=self.state)
+        """ Get the required data files """
+        files = self.lib.GetDataFiles(raise_error=False)
+        if files != "Using obsolete SME Library":
+            return files.split(";")
+        else:
+            logging.warning(
+                "Using obsolete SME Library. Cannot determine necessay data files"
+            )
+            return []
 
     def InputWaveRange(self, wfirst, wlast):
         """
         Read in Wavelength range
 
         Will raise an exception if wfirst is larger than wlast
 
@@ -198,42 +142,45 @@
             first wavelength of the segment
         wlast : float
             last wavelength of the segment
         """
         assert (
             wfirst < wlast
         ), "Input Wavelength range is wrong, first wavelength is larger than last"
-        self.lib.InputWaveRange(wfirst, wlast, type="double", state=self.state)
+        self.lib.InputWaveRange(wfirst, wlast, type="double")
 
         self.wfirst = wfirst
         self.wlast = wlast
 
     def SetVWscale(self, gamma6):
         """
         Set van der Waals scaling factor
 
         Parameters
         ----------
         gamma6 : float
             van der Waals scaling factor
         """
-        self.lib.SetVWscale(gamma6, type="double", state=self.state)
+        logger.debug("Setting Van der Waals scale in smelib")
+        self.lib.SetVWscale(gamma6, type="double")
         self.vw_scale = gamma6
 
     def SetH2broad(self, h2_flag=True):
-        """Set flag for H2 molecule"""
+        """ Set flag for H2 molecule """
+        logger.debug("Setting H2 broadening in smelib")
+
         if h2_flag:
-            self.lib.SetH2broad(state=self.state)
+            self.lib.SetH2broad()
             self.h2broad = True
         else:
             self.ClearH2broad()
 
     def ClearH2broad(self):
-        """Clear flag for H2 molecule"""
-        self.lib.ClearH2broad(state=self.state)
+        """ Clear flag for H2 molecule """
+        self.lib.ClearH2broad()
         self.h2broad = False
 
     def InputLineList(self, linelist):
         """
         Read in line list
 
         Parameters
@@ -241,43 +188,32 @@
         atomic : array of size (nlines, 8)
             atomic linelist data for each line
             fields are: atom_number, ionization, wlcent, excit, gflog, gamrad, gamqst, gamvw
         species : array(string) of size (nlines,)
             names of the elements (with Ionization level)
         """
         try:
-            atomic = linelist["atomic"].T
-            species = linelist["species"]
+            atomic = linelist.atomic.T
+            species = linelist.species
         except AttributeError:
             raise TypeError("linelist has to be a LineList type")
 
-        nlines = len(species)
+        nlines = len(linelist)
         species = np.asarray(species, "U8")
 
         assert (
             atomic.shape[1] == nlines
-        ), "Got wrong Linelist shape, expected ({nlines}, 8) but got {atomic}".format(
-            nlines=nlines, atomic=atomic.shape
-        )
+        ), f"Got wrong Linelist shape, expected ({nlines}, 8) but got {atomic.shape}"
         assert (
             atomic.shape[0] == 8
-        ), "Got wrong Linelist shape, expected ({nlines}, 8) but got {atomic}".format(
-            nlines=nlines, atomic=atomic.shape
-        )
-
-        if self.state is not None:
-            self.state.contents.free_linelist()
-            self.state.contents.free_opacities()
+        ), f"Got wrong Linelist shape, expected ({nlines}, 8) but got {atomic.shape}"
 
+        logger.debug("Passing linelist to smelib")
         self.lib.InputLineList(
-            nlines,
-            species,
-            atomic,
-            type=("int", "string", "double"),
-            state=self.state,
+            nlines, species, atomic, type=("int", "string", "double")
         )
 
         self.linelist = linelist
 
     def OutputLineList(self):
         """
         Return line list
@@ -286,17 +222,15 @@
         -------
         atomic : array of size (nlines, 6)
             relevant data of the linelist
             wlcent, excit, gflog, gamrad, gamqst, gamvw
         """
         nlines = self.nlines
         atomic = np.zeros((nlines, 6))
-        self.lib.OutputLineList(
-            nlines, atomic, type=("int", "double"), state=self.state
-        )
+        self.lib.OutputLineList(nlines, atomic, type=("int", "double"))
         return atomic
 
     def UpdateLineList(self, atomic, species, index):
         """
         Change line list parameters
 
         Parameters
@@ -308,38 +242,32 @@
             names of the elements (with Ionization level)
         index : array(int) of size (nlines,)
             indices of the lines to update relative to the overall linelist
         """
         nlines = atomic.shape[0]
         assert (
             atomic.shape[1] == 8
-        ), "Got wrong Linelist shape, expected ({nlines}, 8) but got {atomic}".format(
-            nlines=nlines, atomic=atomic.shape
-        )
+        ), f"Got wrong Linelist shape, expected ({nlines}, 8) but got {atomic.shape}"
 
         assert (
             len(index) == nlines
         ), "Inconsistent number if lines, between index and linelist"
         assert (
             len(species) == nlines
         ), "Inconsistent number if lines, between index and linelist"
 
         atomic = atomic.T
 
+        logger.debug("Updating linelist in smelib")
         self.lib.UpdateLineList(
-            nlines,
-            species,
-            atomic,
-            index,
-            type=("int", "str", "double", "short"),
-            state=self.state,
+            nlines, species, atomic, index, type=("int", "str", "double", "short")
         )
 
     def InputModel(self, teff, grav, vturb, atmo):
-        """Read in model atmosphere
+        """ Read in model atmosphere
 
         Parameters
         ---------
         teff : float
             effective Temperature in Kelvin
         grav : float
             surface gravity in log10(cgs)
@@ -351,24 +279,37 @@
 
         if teff <= 0:
             raise ValueError("Temperature must be positive (unit is Kelvin)")
         if vturb < 0:
             raise ValueError("Turbulence velocity must be positive or zero")
 
         try:
-            motype = atmo["depth"]
-            depth = atmo[motype]
+
+            #   MOTYPE==0   means depth scale is "Tau", plane-parralel
+            #   MOTYPE==1   means depth scale is "Rhox", plane-parralel
+            #   MOTYPE==3   means depth scale is "RhoX", spherical
+            #   MOTYPE==-1  fake value used with the call to OPMTRX get just
+            #               just the line opacities
+
+            if atmo.geom == "SPH":
+                # Spherical only supports RHOX
+                depth = atmo["RHOX"]
+                motype = "SPH"
+            else:
+                motype = atmo.depth
+                depth = atmo[motype]
+
             ndepth = len(depth)
-            t = atmo["temp"]
-            xne = atmo["xne"]
-            xna = atmo["xna"]
-            rho = atmo["rho"]
+            t = atmo.temp
+            xne = atmo.xne
+            xna = atmo.xna
+            rho = atmo.rho
             vt = np.full(ndepth, vturb) if np.size(vturb) == 1 else vturb
-            wlstd = atmo["wlstd"]
-            opflag = atmo["opflag"]
+            wlstd = atmo.wlstd
+            opflag = atmo.opflag
             args = [
                 ndepth,
                 teff,
                 grav,
                 wlstd,
                 motype,
                 opflag,
@@ -377,27 +318,25 @@
                 xne,
                 xna,
                 rho,
                 vt,
             ]
             type = "sdddusdddddd"  # s : short, d: double, u: unicode (string)
 
-            if atmo["geom"] == "SPH":
-                radius = atmo["radius"]
-                height = atmo["height"]
+            if atmo.geom == "SPH":
+                radius = atmo.radius
+                height = atmo.height
                 motype = "SPH"
                 args = args[:4] + [motype, radius] + args[5:] + [height]
-                type = type[:5] + "d" + type[5:] + "d"
+                type = type[:4] + "ud" + type[5:] + "d"
         except AttributeError as ae:
-            raise TypeError("atmo has to be an Atmo type, {ae}".format(ae=ae))
-
-        if self.state is not None:
-            self.state.contents.free_opacities()
+            raise TypeError(f"atmo has to be an Atmo type, {ae}")
 
-        self.lib.InputModel(*args, type=type, state=self.state)
+        logger.debug("Inputing atmosphere model to smelib")
+        self.lib.InputModel(*args, type=type)
 
         self.teff = teff
         self.grav = grav
         self.vturb = vturb
         self.atmo = atmo
 
     def InputAbund(self, abund):
@@ -414,20 +353,23 @@
         abund : Abund
             abundance structure to be passed (see Abund for more details)
         """
         # Convert abundances to the right format
         # metallicity is included in the abundance class, ignored in function call
         abund = abund("sme", raw=True)
         assert isinstance(abund, np.ndarray)
-        self.lib.InputAbund(abund, type="double", state=self.state)
+        abund[np.isnan(abund)] = -99
+
+        logger.debug("Inputing abundances to smelib")
+        self.lib.InputAbund(abund, type="double")
 
         self.abund = abund
 
     def Opacity(self, getData=False, motype=1):
-        """Calculate opacities
+        """ Calculate opacities
 
         Parameters
         ---------
         getData : bool
             if True copblu and copred (and copstd) will be returned
             requires that radiative transfer was run
         motype : int
@@ -452,15 +394,15 @@
             type = ["s", "d", "d"]
 
             if motype == 0:
                 copstd = np.zeros(nmu)
                 args += [copstd]
                 type += ["d"]
 
-        self.lib.Opacity(*args, type=type, state=self.state)
+        self.lib.Opacity(*args, type=type)
 
         return args[1:]
 
     def GetOpacity(self, switch, species=None, key=None):
         """
         Returns specific cont. opacity, different output depending on the input
 
@@ -501,15 +443,15 @@
                     args += [species, key]
                     type += ["u", "u"]
         elif switch == 9:
             if species is not None:
                 args += [species]
                 type += ["u"]
 
-        self.lib.GetOpacity(*args, type=type, state=self.state)
+        self.lib.GetOpacity(*args, type=type)
         return result
 
     def Ionization(self, ion=0):
         """
         Calculate ionization balance for current atmosphere and abundances.
         Ionization state is stored in the external library.
         Ion is a bit flag with values (add them together to use multiple):
@@ -523,66 +465,58 @@
         can affect line shape, e.g. shape of hydrogen lines.
 
         Parameters
         ----------
         ion : int
             flag that determines the behaviour of the C function
         """
-        if self.state is not None:
-            self.state.contents.free_ionization()
-
-        self.lib.Ionization(
-            ion,
-            type="short",
-            raise_error=False,
-            raise_warning=True,
-            state=self.state,
-        )
+        logger.debug("Calculating ionization in smelib")
+        self.lib.Ionization(ion, type="short", raise_error=False, raise_warning=True)
         self.ion = ion
 
     def GetDensity(self):
         """
         Retrieve density in each layer
 
         Returns
         -------
         density : array of size (ndepth,)
             Density of the atmosphere in each layer
         """
         length = self.ndepth
         array = np.zeros(length, dtype=float)
-        self.lib.GetDensity(length, array, type="sd", state=self.state)
+        self.lib.GetDensity(length, array, type="sd")
         return array
 
     def GetNatom(self):
         """
         Get XNA
 
         Returns
         -------
         XNA : array of size (ndepth,)
             XNA in each layer
         """
         length = self.ndepth
         array = np.zeros(length, dtype=float)
-        self.lib.GetNatom(length, array, type="sd", state=self.state)
+        self.lib.GetNatom(length, array, type="sd")
         return array
 
     def GetNelec(self):
         """
         Get XNE (Electron number density) for each layer in the atmosphere
 
         Returns
         -------
         XNE : array of size (ndepth,)
             XNE in each layer
         """
         length = self.ndepth
         array = np.zeros(length, dtype=float)
-        self.lib.GetNelec(length, array, type="sd", state=self.state)
+        self.lib.GetNelec(length, array, type="sd")
         return array
 
     def Transf(
         self,
         mu,
         accrt,
         accwi,
@@ -639,37 +573,36 @@
 
         mu = np.asarray(mu)
         nmu = np.size(mu)
 
         # Prepare data:
         sint_seg = np.zeros((nwmax, nmu))  # line+continuum intensities
         cint_seg = np.zeros((nwmax, nmu))  # all continuum intensities
-        cintr_seg = np.zeros(nmu)  # red continuum intensity
+        cintr_seg = np.zeros((nmu))  # red continuum intensity
+        nw = np.array([nw])
 
         type = "sdddiiddddss"  # s: short, d:double, i:int, u:unicode (string)
 
+        logger.debug("Starting radiative Transfer calculations in smelib")
         self.lib.Transf(
             nmu,
             mu,
             cint_seg,
             cintr_seg,
             nwmax,
             nw,
             wint_seg,
             sint_seg,
             accrt,
             accwi,
             keep_lineop,
             long_continuum,
             type=type,
-            state=self.state,
         )
-
-        if nw == 0:
-            nw = np.count_nonzero(wint_seg)
+        nw = nw[0]
 
         wint_seg = wint_seg[:nw]
         sint_seg = sint_seg[:nw, :].T
         cint_seg = cint_seg[:nw, :].T
 
         sint_seg = np.nan_to_num(sint_seg, copy=False)
         cint_seg = np.nan_to_num(cint_seg, copy=False)
@@ -697,17 +630,15 @@
             Centeral depth (i.e. specific intensity) of each line
         """
 
         nmu = np.size(mu)
         nwsize = self.nlines
         table = np.zeros(nwsize)
 
-        self.lib.CentralDepth(
-            nmu, mu, nwsize, table, accrt, type="idifd", state=self.state
-        )
+        self.lib.CentralDepth(nmu, mu, nwsize, table, accrt, type="idifd")
         self.nmu = nmu
 
         return table
 
     def GetLineOpacity(self, wave):
         """
         Retrieve line opacity data from the C library
@@ -726,28 +657,26 @@
         scr : array
             Scatter
         tsf : array
             Total source function
         csf : array
             Continuum source function
         """
-        nmu = self.ndepth
+        nmu = self.nmu
         lop = np.zeros(nmu)
         cop = np.zeros(nmu)
         scr = np.zeros(nmu)
         tsf = np.zeros(nmu)
         csf = np.zeros(nmu)
         type = "dsddddd"
-        self.lib.GetLineOpacity(
-            wave, nmu, lop, cop, scr, tsf, csf, type=type, state=self.state
-        )
+        self.lib.GetLineOpacity(wave, nmu, lop, cop, scr, tsf, csf, type=type)
         return lop, cop, scr, tsf, csf
 
     def GetLineRange(self):
-        """Get the effective wavelength range for each line
+        """ Get the effective wavelength range for each line
         i.e. the wavelengths for which the line has significant impact
 
         Parameters
         ----------
         nlines : int
             number of lines in the linelist
 
@@ -755,17 +684,15 @@
         -------
         linerange : array of size (nlines, 2)
             lower and upper wavelength for each spectral line
         """
         nlines = self.nlines
         linerange = np.zeros((nlines, 2))
 
-        self.lib.GetLineRange(
-            linerange, nlines, type=("double", "int"), state=self.state
-        )
+        self.lib.GetLineRange(linerange, nlines, type=("double", "int"))
 
         return linerange
 
     def InputNLTE(self, bmat, lineindex):
         """
         Input NLTE departure coefficients
 
@@ -779,43 +706,35 @@
         ndepth = self.ndepth
         nlines = self.nlines
 
         if not isinstance(bmat, (list, np.ndarray)):
             raise TypeError("Departure coefficient matrix is not an array")
 
         bmat = np.atleast_2d(bmat)
-        if bmat.shape[0] != 2:
+        if bmat.shape[1] != 2:
             raise ValueError(
-                "Departure coefficient matrix has the wrong shape, expected (2, {ndepth}) but got {bmat} instead".format(
-                    ndepth=ndepth, bmat=bmat.shape
-                )
+                f"Departure coefficient matrix has the wrong shape, expected ({ndepth}, 2) but got {bmat.shape} instead"
             )
-        if bmat.shape[1] != ndepth:
+        if bmat.shape[0] != ndepth:
             raise ValueError(
-                "Departure coefficient matrix has the wrong shape, expected (2, {ndepth}) but got {bmat} instead".format(
-                    ndepth=ndepth, bmat=bmat.shape
-                )
+                f"Departure coefficient matrix has the wrong shape, expected ({ndepth}, 2) but got {bmat.shape} instead"
             )
 
         if not isinstance(lineindex, (int, np.integer)):
             raise TypeError("Lineindex is not an integer type")
 
         if not 0 <= lineindex < nlines:
             raise ValueError(
-                "Lineindex out of range, expected value between 0 and {nlines}, but got {lineindex} instead".format(
-                    nlines=nlines, lineindex=lineindex
-                )
+                f"Lineindex out of range, expected value between 0 and {nlines}, but got {lineindex} instead"
             )
 
-        self.lib.InputDepartureCoefficients(
-            bmat, lineindex, type=("double", "int"), state=self.state
-        )
+        self.lib.InputDepartureCoefficients(bmat, lineindex, type=("double", "int"))
 
     def GetNLTE(self, line):
-        """Get the NLTE departure coefficients as stored in the C library
+        """ Get the NLTE departure coefficients as stored in the C library
 
         Parameters
         ----------
         line : int
             requested line index, i.e. between 0 and number of lines
 
         Returns
@@ -823,21 +742,21 @@
         bmat : array of size (2, nrhox)
             departure coefficients for the given line index
         """
         nrhox = self.ndepth
 
         bmat = np.full((2, nrhox), -1.0, dtype=float)
         self.lib.GetDepartureCoefficients(
-            bmat, nrhox, line, type=("double", "int", "int"), state=self.state
+            bmat, nrhox, line, type=("double", "int", "int")
         )
         return bmat
 
     def ResetNLTE(self):
-        """Reset departure coefficients from any previous call, to ensure LTE as default"""
-        self.lib.ResetDepartureCoefficients(state=self.state)
+        """ Reset departure coefficients from any previous call, to ensure LTE as default """
+        self.lib.ResetDepartureCoefficients()
 
     def GetNLTEflags(self):
         """Get an array that tells us which lines have been used with NLTE correction
 
         Parameters
         ----------
         linelist : int
@@ -847,12 +766,10 @@
         -------
         nlte_flags : array(bool) of size (nlines,)
             True if line was used with NLTE, False if line is only LTE
         """
         nlines = self.nlines
         nlte_flags = np.zeros(nlines, dtype=np.int16)
 
-        self.lib.GetNLTEflags(
-            nlte_flags, nlines, type=("short", "int"), state=self.state
-        )
+        self.lib.GetNLTEflags(nlte_flags, nlines, type=("short", "int"))
 
         return nlte_flags.astype(bool)
```

### Comparing `pysme-astro-0.4.99/src/pysme/solve.py` & `pysme-astro-5.74.9/src/pysme/solve.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,98 +1,76 @@
-# -*- coding: utf-8 -*-
 """
 Calculates the spectrum, based on a set of stellar parameters
 And also determines the best fit parameters
 """
 
-import json
 import logging
 import warnings
 from os.path import splitext
+import contextlib
+import sys
+import builtins
 
 import numpy as np
+from tqdm import tqdm
 from scipy.constants import speed_of_light
-from scipy.optimize import OptimizeWarning, least_squares
+from scipy.optimize import OptimizeWarning, least_squares, curve_fit
 from scipy.optimize._numdiff import approx_derivative
-from scipy.stats import norm
-from tqdm import tqdm
+from scipy.special import erf
+from scipy.stats import gennorm
 
-from . import __file_ending__
+from . import __file_ending__, broadening
 from .abund import Abund
 from .atmosphere.atmosphere import AtmosphereError
-from .atmosphere.krzfile import KrzFile
 from .atmosphere.savfile import SavFile
+from .atmosphere.krzfile import KrzFile
+from .config import Config
+from .continuum_and_radial_velocity import match_rv_continuum
 from .large_file_storage import setup_lfs
-from .nlte import DirectAccessFile
-from .synthesize import Synthesizer
+from .iliffe_vector import Iliffe_vector
+from .sme_synth import SME_DLL
+from .uncertainties import uncertainties
 from .util import print_to_log
+from .synthesize import Synthesizer
+from .nlte import DirectAccessFile
 
 logger = logging.getLogger(__name__)
 
 clight = speed_of_light * 1e-3  # km/s
 warnings.filterwarnings("ignore", category=OptimizeWarning)
 
 
 class SME_Solver:
-    def __init__(self, filename=None, restore=False):
+    def __init__(self, filename=None):
+        self.dll = SME_DLL()
         self.config, self.lfs_atmo, self.lfs_nlte = setup_lfs()
         self.synthesizer = Synthesizer(
             config=self.config,
             lfs_atmo=self.lfs_atmo,
             lfs_nlte=self.lfs_nlte,
+            dll=self.dll,
         )
 
         # Various parameters to keep track of during solving
         self.filename = filename
         self.iteration = 0
         self.parameter_names = []
         self.update_linelist = False
         self._latest_residual = None
-        self._latest_jacobian = None
-        self.restore = restore
 
         # For displaying the progressbars
+        self.fig = None
         self.progressbar = None
         self.progressbar_jacobian = None
 
     @property
     def nparam(self):
         return len(self.parameter_names)
 
-    def restore_func(self, sme):
-        fname = self.filename.rsplit(".", 1)[0]
-        fname = f"{fname}_iter.json"
-        try:
-            with open(fname) as f:
-                data = json.load(f)
-            # The keys are string, but we want the max in int, so we need to convert back and forth
-            iteration = str(max(int(i) for i in data.keys()))
-            for fp in self.parameter_names:
-                sme[fp] = data[iteration].get(fp, sme[fp])
-            logger.warning(f"Restoring existing backup data from {fname}")
-        except:
-            pass
-        return sme
-
-    def backup(self, sme):
-        fname = self.filename.rsplit(".", 1)[0]
-        fname = f"{fname}_iter.json"
-        try:
-            with open(fname) as f:
-                data = json.load(f)
-        except:
-            data = {}
-        data[self.iteration] = {fp: sme[fp] for fp in self.parameter_names}
-        try:
-            with open(fname, "w") as f:
-                json.dump(data, f)
-        except:
-            pass
-
-    def _residuals(
+    def __residuals(
         self, param, sme, spec, uncs, mask, segments="all", isJacobian=False, **_
     ):
         """
         Calculates the synthetic spectrum with sme_func and
         returns the residuals between observation and synthetic spectrum
 
         residual = (obs - synth) / uncs
@@ -122,121 +100,119 @@
 
         Returns
         -------
         resid : array(float) of size (m,)
             residuals of the synthetic spectrum
         """
         update = not isJacobian
-        save = not isJacobian and self.filename is not None
+        save = not isJacobian
         reuse_wavelength_grid = isJacobian
         radial_velocity_mode = "robust" if not isJacobian else "fast"
-        # method = "parallel" if isJacobian else "sequential"
-        method = "sequential"
 
         # change parameters
         for name, value in zip(self.parameter_names, param):
             sme[name] = value
         # run spectral synthesis
         try:
             result = self.synthesizer.synthesize_spectrum(
                 sme,
                 updateStructure=update,
                 reuse_wavelength_grid=reuse_wavelength_grid,
                 segments=segments,
                 passLineList=False,
                 updateLineList=self.update_linelist,
                 radial_velocity_mode=radial_velocity_mode,
-                method=method,
             )
         except AtmosphereError as ae:
             # Something went wrong (left the grid? Don't go there)
             # If returned value is not finite, the fit algorithm will not go there
             logger.debug(ae)
-            return np.full(spec.size, np.inf)
+            return np.inf
+
+        # Also save intermediary results, because we can
+        if save and self.filename is not None:
+            if self.filename.endswith(__file_ending__):
+                fname = self.filename[:-4]
+            else:
+                fname = self.filename
+            fname = f"{fname}_tmp{__file_ending__}"
+            sme.save(fname)
 
         segments = Synthesizer.check_segments(sme, segments)
 
         # Get the correct results for the comparison
         synth = sme.synth if update else result[1]
         synth = synth[segments]
         synth = synth[mask] if mask is not None else synth
 
         if sme.telluric is not None:
             tell = sme.telluric[segments]
             tell = tell[mask] if mask is not None else tell
-            synth = synth * tell
+            synth *= tell
+
+        # TODO: update based on lineranges
+        uncs_linelist = 0
 
-        resid = (synth - spec) / (uncs)
+        resid = (synth - spec) / (uncs + uncs_linelist)
         resid = resid.ravel()
         resid = np.nan_to_num(resid, copy=False)
 
         # Update progress bars
         if isJacobian:
             self.progressbar_jacobian.update(1)
         else:
             self.progressbar.total += 1
             self.progressbar.update(1)
 
         if not isJacobian:
             # Save result for jacobian
             self._latest_residual = resid
             self.iteration += 1
-        logger.debug("%s", {n: f"{v:.3f}" for n, v in zip(self.parameter_names, param)})
-
-        # Also save intermediary results, because we can
-        if save:
-            self.backup(sme)
+            logger.debug("%s", {n: v for n, v in zip(self.parameter_names, param)})
+            # Plot
+            # if fig is not None:
+            #     wave = sme2.wave
+            #     try:
+            #         fig.add(wave, synth, f"Iteration {self.iteration}")
+            #     except AttributeError:
+            #         warnings.warn(f"Figure {repr(fig)} doesn't have a 'add' method")
+            #     except Exception as e:
+            #         warnings.warn(f"Error during Plotting: {e.message}")
 
         return resid
 
-    def _jacobian(
-        self,
-        param,
-        *args,
-        bounds=None,
-        segments="all",
-        step_sizes=None,
-        method="2-point",
-        **_,
-    ):
+    def __jacobian(self, param, *args, bounds=None, segments="all", **_):
         """
         Approximate the jacobian numerically
-        The calculation is the same as "2-point"
-        but we can tell residuals that we are within a jacobian.
-
-        Note that when we reuse the wavelength grid, the results are
-        slightly different for reasons(?). Therefore the step size should
-        be larger than those differences, which is why we specify the
-        step size for each parameter.
+        The calculation is the same as "3-point"
+        but we can tell residuals that we are within a jacobian
         """
         self.progressbar_jacobian.reset()
-
-        # Here we replace the scipy version of approx_derivative with our own
-        # The only difference being that we use Multiprocessing for the jacobian
         g = approx_derivative(
-            self._residuals,
+            self.__residuals,
             param,
-            method=method,
+            method="3-point",
             # This feels pretty bad, passing the latest synthetic spectrum
             # by reference as a parameter of the residuals function object
             f0=self._latest_residual,
-            abs_step=step_sizes,
             bounds=bounds,
             args=args,
             kwargs={"isJacobian": True, "segments": segments},
         )
 
         if not np.all(np.isfinite(g)):
             g[~np.isfinite(g)] = 0
             logger.warning(
                 "Some derivatives are non-finite, setting them to zero. "
                 "Final uncertainties will be inaccurate. "
                 "You might be running into the boundary of the grid"
             )
-        self._latest_jacobian = np.copy(g)
+
+        self._last_jac = np.copy(g)
+
         return g
 
     def get_bounds(self, sme):
         """
         Create Bounds based on atmosphere grid and general rules
 
         Note that bounds define by definition a cube in the parameter space,
@@ -250,16 +226,15 @@
             names of the parameters to vary
         sme : SME_Structure
             sme structure to get bounds for
 
         Raises
         ------
         IOError
-            If the atmosphere file can't be read, allowed types
-            are IDL savefiles (.sav), and .krz files
+            If the atmosphere file can't be read, allowed types are IDL savefiles (.sav), and .krz files
 
         Returns
         -------
         bounds : dict
             Bounds for the given parameters
         """
 
@@ -267,58 +242,44 @@
 
         # Create bounds based on atmosphere grid
         if (
             "teff" in self.parameter_names
             or "logg" in self.parameter_names
             or "monh" in self.parameter_names
         ):
-            if sme.atmo.method == "grid":
-                atmo_source = sme.atmo.source
-                _, ext = splitext(atmo_source)
-                atmo_file = self.lfs_atmo.get(atmo_source)
-
-                if ext == ".sav":
-                    atmo_grid = SavFile(
-                        atmo_file, source=atmo_source, lfs=self.lfs_atmo
-                    )
-
-                    teff = np.unique(atmo_grid.teff)
-                    teff = np.min(teff), np.max(teff)
-                    bounds["teff"] = teff
-
-                    logg = np.unique(atmo_grid.logg)
-                    logg = np.min(logg), np.max(logg) * 1.5
-                    bounds["logg"] = logg
-
-                    monh = np.unique(atmo_grid.monh)
-                    monh = np.min(monh), np.max(monh) * 1.5
-                    bounds["monh"] = monh
-                elif ext == ".krz":
-                    # krz atmospheres are fixed to one parameter set
-                    # allow just "small" area around that
-                    atmo = KrzFile(atmo_file, source=atmo_source)
-                    bounds["teff"] = atmo.teff - 500, atmo.teff + 500
-                    bounds["logg"] = atmo.logg - 1, atmo.logg + 1
-                    bounds["monh"] = atmo.monh - 1, atmo.monh + 1
-                else:
-                    raise IOError(f"File extension {ext} not recognized")
-            if sme.atmo.method == "embedded":
-                atmo = sme.atmo
+            atmo_file = sme.atmo.source
+            _, ext = splitext(atmo_file)
+            atmo_file = self.lfs_atmo.get(atmo_file)
+
+            if ext == ".sav":
+                atmo_grid = SavFile(atmo_file)
+
+                teff = np.unique(atmo_grid.teff)
+                teff = np.min(teff), np.max(teff)
+                bounds["teff"] = teff
+
+                logg = np.unique(atmo_grid.logg)
+                logg = np.min(logg), np.inf
+                bounds["logg"] = logg
+
+                monh = np.unique(atmo_grid.monh)
+                monh = np.min(monh), np.inf
+                bounds["monh"] = monh
+            elif ext == ".krz":
+                # krz atmospheres are fixed to one parameter set
+                # allow just "small" area around that
+                atmo = KrzFile(atmo_file)
                 bounds["teff"] = atmo.teff - 500, atmo.teff + 500
                 bounds["logg"] = atmo.logg - 1, atmo.logg + 1
                 bounds["monh"] = atmo.monh - 1, atmo.monh + 1
+            else:
+                raise IOError(f"File extension {ext} not recognized")
+
         # Add generic bounds
-        bounds.update(
-            {
-                "vmic": [0, clight],
-                "vmac": [0, clight],
-                "vsini": [0, clight],
-                "ipres": [1, 500_000],
-            }
-        )
+        bounds.update({"vmic": [0, clight], "vmac": [0, clight], "vsini": [0, clight]})
         # bounds.update({"abund %s" % el: [-10, 11] for el in abund_elem})
 
         result = np.array([[-np.inf, np.inf]] * self.nparam)
         solar = Abund.solar()
         for i, name in enumerate(self.parameter_names):
             if name[:5].lower() == "abund":
                 element = name[5:].strip().capitalize()
@@ -368,52 +329,26 @@
         scales = {"teff": 1000}
         scales = [
             scales[name] if name in scales.keys() else 1
             for name in self.parameter_names
         ]
         return scales
 
-    def get_step_sizes(self, parameter_names):
-        steps = {
-            "teff": 10,
-            "logg": 0.01,
-            "monh": 0.01,
-            "vmic": 0.01,
-            "vmac": 0.1,
-            "vsini": 0.05,
-            "vrad": 0.05,
-            "gam6": 0.02,
-            "ipres": 1000,
-        }
-        step_sizes = []
-        for param in parameter_names:
-            if param in steps.keys():
-                step_sizes += [steps[param]]
-            elif param.startswith("Abund"):
-                step_sizes += [0.01]
-            elif param.startswith("linelist"):
-                step_sizes += [0.02]
-            else:
-                step_sizes += [0.001]
-        step_sizes = np.asarray(step_sizes)
-        return step_sizes
-
     def get_default_values(self, sme):
-        """Default parameter values for each name"""
+        """ Default parameter values for each name """
         d = {"teff": 5778, "logg": 4.4, "monh": 0, "vmac": 1, "vmic": 1}
         d.update({f"{el} abund": v for el, v in Abund.solar()().items()})
 
         def default(name):
             logger.info("No value for %s set, using default value %s", name, d[name])
             return d[name]
 
-        values = [
+        return [
             sme[s] if sme[s] is not None else default(s) for s in self.parameter_names
         ]
-        return np.array(values)
 
     def estimate_uncertainties(self, unc, resid, deriv):
         """
         Estimate the uncertainties by fitting the cumulative distribution of
         derivative / uncertainties vs. residual / derivative
         with the generalized normal distribution and use the 68% percentile
         as the 1 sigma approximation for a normally distributed variable
@@ -433,44 +368,35 @@
             uncertainties for each free paramater, in the same order as self.parameter_names
         """
 
         freep_name = self.parameter_names
         nparameters = len(freep_name)
         freep_unc = np.zeros(nparameters)
 
-        chi2 = np.sum(resid ** 2) / (resid.size - nparameters)
-
         # Cumulative distribution function of the normal distribution
         # cdf = lambda x, mu, sig: 0.5 * (1 + erf((x - mu) / (np.sqrt(2) * sig)))
         # std = lambda mu, sig: sig
 
-        def cdf(x, mu, alpha):
+        def cdf(x, mu, alpha, beta):
             """
             Cumulative distribution function of the generalized normal distribution
             the factor sqrt(2) is a conversion between generalized and regular normal distribution
             """
-            # return gennorm.cdf(x, beta, loc=mu, scale=alpha * np.sqrt(2))
-            return norm.cdf(x, loc=mu, scale=alpha)
+            return gennorm.cdf(x, beta, loc=mu, scale=alpha * np.sqrt(2))
 
-        def std(mu, alpha):
-            """1 sigma (68.27 %) quantile, assuming symmetric distribution"""
-            # interval = gennorm.interval(0.6827, beta, loc=mu, scale=alpha * np.sqrt(2))
-            interval = norm.interval(0.6827, loc=mu, scale=alpha)
+        def std(mu, alpha, beta):
+            """ 1 sigma (68.27 %) quantile, assuming symmetric distribution """
+            interval = gennorm.interval(0.6827, beta, loc=mu, scale=alpha * np.sqrt(2))
             sigma = (interval[1] - interval[0]) / 2
             return sigma
 
-        for i, pname in enumerate(freep_name):
-            pder = deriv[:, i] / np.sqrt(chi2)
-            idx = pder != 0
-            # idx &= np.abs(resid) < 5 * unc / unc_median
-
-            med = np.median(np.abs(pder))
-            mad = np.median(np.abs(np.abs(pder) - med))
-            idx &= np.abs(pder) < med + 20 * mad
-
+        for i in range(nparameters):
+            pder = deriv[:, i]
+            gradlim = np.median(np.abs(pder))
+            idx = np.abs(pder) > gradlim
             if np.count_nonzero(idx) <= 5:
                 logger.warning(
                     "Not enough data points with a suitable derivative to determine the uncertainties of %s",
                     freep_name[i],
                 )
                 continue
             # Sort pixels according to the change of the i
@@ -480,64 +406,26 @@
             # Weights of the individual pixels also sorted
             ch_y = np.abs(pder[idx][idx_sort]) / unc[idx][idx_sort]
             # Cumulative weights
             ch_y = np.cumsum(ch_y)
             # Normalized cumulative weights
             ch_y /= ch_y[-1]
 
-            hmed = np.interp(0.5, ch_y, ch_x)
-            interval = np.interp([0.16, 0.84], ch_y, ch_x)
-            sigma_estimate = (interval[1] - interval[0]) / 2
-
-            # # Fit the distribution
-            # try:
-            #     sopt, _ = curve_fit(cdf, ch_x, ch_y)
-            # except RuntimeError:
-            #     # Fit failed, use dogbox instead
-            #     try:
-            #         sopt, _ = curve_fit(cdf, ch_x, ch_y, method="dogbox")
-            #     except RuntimeError:
-            #         sopt = [0, 0, 0]
+            # Fit the distribution
+            sopt, _ = curve_fit(cdf, ch_x, ch_y)
 
-            # hmed = sopt[0]
-            # sigma_estimate = std(*sopt)
+            hmed = sopt[0]
+            sigma_estimate = std(*sopt)
             freep_unc[i] = sigma_estimate
 
-            # # Debug plots
-            # import matplotlib.pyplot as plt
-
-            # # Plot 1 (cumulative distribution)
-            # r = (sopt[0] - 20 * sopt[1], sopt[0] + 20 * sopt[1])
-            # x = np.linspace(ch_x.min(), ch_x.max(), ch_x.size * 10)
-            # plt.plot(ch_x, ch_y, "+", label="measured")
-            # plt.plot(x, cdf(x, *sopt), label="fit")
-            # plt.xlabel(freep_name[i])
-            # plt.ylabel("cumulative probability")
-            # plt.show()
-            # # Plot 2 (density distribution)
-            # x = np.linspace(r[0], r[-1], ch_x.size * 10)
-            # plt.hist(
-            #     ch_x,
-            #     bins="auto",
-            #     density=True,
-            #     histtype="step",
-            #     range=r,
-            #     label="measured",
-            # )
-            # plt.plot(x, norm.pdf(x, loc=sopt[0], scale=sopt[1]), label="fit")
-            # plt.xlabel(freep_name[i])
-            # plt.ylabel("probability")
-            # plt.xlim(r)
-            # plt.show()
-
-            logger.debug(f"{pname}: {hmed}, {sigma_estimate}")
+            logger.debug(f"{freep_name[i]}: {hmed}, {sigma_estimate}")
 
         return freep_unc
 
-    def update_fitresults(self, sme, result, segments):
+    def update_fitresults(self, sme, result):
         # Update SME structure
         sme.fitresults.clear()
 
         popt = result.x
         sme.fitresults.values = popt
         sme.fitresults.parameters = self.parameter_names
 
@@ -551,32 +439,24 @@
         sme.fitresults.covariance = covar
         sme.fitresults.gradient = result.grad
         sme.fitresults.derivative = result.jac
         sme.fitresults.residuals = result.fun
         sme.fitresults.chisq = (
             result.cost * 2 / (sme.spec.size - len(self.parameter_names))
         )
-        sme.fitresults.iterations = self.iteration
 
         sme.fitresults.fit_uncertainties = [np.nan for _ in self.parameter_names]
         for i in range(len(self.parameter_names)):
             # Errors based on covariance matrix
             sme.fitresults.fit_uncertainties[i] = sig[i]
 
-        try:
-            mask = sme.mask_good[segments]
-            unc = sme.uncs[segments]
-            unc = unc[mask] if mask is not None else unc
-            unc = unc.ravel()
-            sme.fitresults.uncertainties = self.estimate_uncertainties(
-                unc, result.fun, result.jac
-            )
-        except:
-            sme.fitresults.uncertainties = sme.fitresults.fit_uncertainties
-        # sme.fitresults.uncertainties = sme.fitresults.fit_uncertainties
+        unc = np.concatenate(sme.uncs[sme.mask_good])
+        sme.fitresults.uncertainties = self.estimate_uncertainties(
+            unc, result.fun, result.jac
+        )
 
         return sme
 
     def sanitize_parameter_names(self, sme, param_names):
         # Sanitize parameter names
         param_names = [p.casefold() for p in param_names]
         param_names = [p.capitalize() if p[:5] == "abund" else p for p in param_names]
@@ -605,15 +485,15 @@
                 sme.cscale_flag = "linear"
                 logger.info(
                     "Removed fit parameter 'cont', instead set continuum flag to %s",
                     sme.cscale_flag,
                 )
         return param_names
 
-    def solve(self, sme, param_names=None, segments="all", bounds=None):
+    def solve(self, sme, param_names=None, segments="all"):
         """
         Find the least squares fit parameters to an observed spectrum
 
         NOTE: intermediary results will be saved in filename ("sme.npy")
 
         Parameters
         ----------
@@ -629,26 +509,14 @@
         sme : SME_Struct
             same sme structure with fit results in sme.fitresults, and best fit spectrum in sme.smod
         """
 
         assert "wave" in sme, "SME Structure has no wavelength"
         assert "spec" in sme, "SME Structure has no observation"
 
-        if self.restore and self.filename is not None:
-            fname = self.filename.rsplit(".", 1)[0]
-            fname = f"{fname}_iter.json"
-            try:
-                with open(fname) as f:
-                    data = json.load(f)
-                for fp in param_names:
-                    sme[fp] = data[fp]
-                logger.warning(f"Restoring existing backup data from {fname}")
-            except:
-                pass
-
         if "uncs" not in sme:
             sme.uncs = np.ones(sme.spec.size)
             logger.warning("SME Structure has no uncertainties, using all ones instead")
         if "mask" not in sme:
             sme.mask = np.full(sme.wave.size, sme.mask_values["line"])
 
         segments = Synthesizer.check_segments(sme, segments)
@@ -666,111 +534,86 @@
         self.update_linelist = False
         for name in self.parameter_names:
             if name[:8] == "linelist":
                 self.update_linelist = True
                 break
 
         # Create appropiate bounds
-        if bounds is None:
-            bounds = self.get_bounds(sme)
-        # scales = self.get_scale()
-        step_sizes = self.get_step_sizes(self.parameter_names)
+        bounds = self.get_bounds(sme)
+        scales = self.get_scale()
         # Starting values
         p0 = self.get_default_values(sme)
         if np.any((p0 < bounds[0]) | (p0 > bounds[1])):
             logger.warning(
                 "Initial values are incompatible with the bounds, clipping initial values"
             )
             p0 = np.clip(p0, bounds[0], bounds[1])
-        # Restore backup
-        if self.restore:
-            sme = self.restore_func(sme)
 
         # Get constant data from sme structure
-        for seg in segments:
-            sme.mask[seg, sme.uncs[seg] == 0] = sme.mask_values["bad"]
-        # sme.mask[segments][sme.uncs[segments] == 0] = sme.mask_values["bad"]
+        sme.mask[segments][sme.uncs[segments] == 0] = 0
         mask = sme.mask_good[segments]
         spec = sme.spec[segments][mask]
         uncs = sme.uncs[segments][mask]
 
-        # This is the expected range of the uncertainty
-        # if the residuals are larger, they are dampened by log(1 + z)
-        f_scale = 0.1 * np.nanmean(spec.ravel()) / np.nanmean(uncs.ravel())
-
         # Divide the uncertainties by the spectrum, to improve the fit in the continuum
         # Just as in IDL SME, this increases the relative error for points inside lines
-        # uncs /= spec
+        uncs /= spec
 
         logger.info("Fitting Spectrum with Parameters: %s", ",".join(param_names))
         logger.debug("Initial values: %s", p0)
         logger.debug("Bounds: %s", bounds)
 
         if (
-            sme.wran.min() * (1 - 100 / clight) > sme.linelist.wlcent.min()
-            or sme.wran.max() * (1 + 100 / clight) < sme.linelist.wlcent.max()
+            sme.wran.min() * (1 - 100 / 3e5) > sme.linelist.wlcent.min()
+            or sme.wran.max() * (1 + 100 / 3e5) < sme.linelist.wlcent.max()
         ):
             logger.warning(
                 "The linelist extends far beyond the requested wavelength range."
-                " This will slow down the calculation, consider using only relevant lines\n"
+                " This will slow down the calculation, consider using only relevant lines"
+            )
+            logger.warning(
                 f"Wavelength range: {sme.wran.min()} - {sme.wran.max()} Å"
                 f" ; Linelist range: {sme.linelist.wlcent.min()} - {sme.linelist.wlcent.max()} Å"
             )
 
         # Setup LineList only once
-        dll = self.synthesizer.get_dll()
-        dll.SetLibraryPath()
-        dll.InputLineList(sme.linelist)
+        self.dll.SetLibraryPath()
+        self.dll.InputLineList(sme.linelist)
 
         # Do the heavy lifting
         if self.nparam > 0:
             self.progressbar = tqdm(desc="Iteration", total=0)
-            self.progressbar_jacobian = tqdm(desc="Jacobian", total=len(p0))
+            self.progressbar_jacobian = tqdm(desc="Jacobian", total=len(p0) * 2)
             with print_to_log():
                 res = least_squares(
-                    self._residuals,
-                    jac=self._jacobian,
+                    self.__residuals,
                     x0=p0,
+                    jac=self.__jacobian,
                     bounds=bounds,
-                    loss="cauchy",
-                    f_scale=f_scale,
-                    method="dogbox",
-                    # x_scale="jac",
-                    # These control the tolerance, for early termination
-                    # since each iteration is quite expensive
-                    xtol=sme.accxt,
-                    ftol=sme.accft,
-                    gtol=sme.accgt,
+                    x_scale="jac",
+                    loss="soft_l1",
+                    method="trf",
                     verbose=2,
+                    max_nfev=sme.fitresults.maxiter,
                     args=(sme, spec, uncs, mask),
-                    kwargs={
-                        "bounds": bounds,
-                        "segments": segments,
-                        "step_sizes": step_sizes,
-                        "method": "2-point",
-                    },
+                    kwargs={"bounds": bounds, "segments": segments},
                 )
-                # The jacobian is altered by the loss function
-                # This lets us keep the original for our uncertainty estimate
-                res.jac = self._latest_jacobian
-
             self.progressbar.close()
             self.progressbar_jacobian.close()
+            # The returned jacobian is "scaled for robust loss function"
+            res.jac = self._last_jac
             for i, name in enumerate(self.parameter_names):
                 sme[name] = res.x[i]
-            sme = self.update_fitresults(sme, res, segments)
+            sme = self.update_fitresults(sme, res)
             logger.debug("Reduced chi square: %.3f", sme.fitresults.chisq)
-            try:
-                for name, value, unc in zip(
-                    self.parameter_names, res.x, sme.fitresults.uncertainties
-                ):
-                    logger.info("%s\t%.5f +- %.5g", name.ljust(10), value, unc)
-                logger.info("%s\t%s +- %s", "v_rad".ljust(10), sme.vrad, sme.vrad_unc)
-            except:
-                pass
+            for name, value, unc in zip(
+                self.parameter_names, res.x, sme.fitresults.uncertainties
+            ):
+                logger.info("%s\t%.5f +- %.5g", name.ljust(10), value, unc)
+            logger.info("%s\t%s +- %s", "v_rad".ljust(10), sme.vrad, sme.vrad_unc)
         elif len(param_names) > 0:
             # This happens when vrad and/or cscale are given as parameters but nothing else
             # We could try to reuse the already calculated synthetic spectrum (if it already exists)
             # However it is much lower resolution then the newly synthethized one (usually)
             # Therefore the radial velocity wont be as good as when redoing the whole thing
             sme = self.synthesizer.synthesize_spectrum(sme, segments)
         else:
@@ -778,12 +621,10 @@
 
         if self.filename is not None:
             sme.save(self.filename)
 
         return sme
 
 
-def solve(
-    sme, param_names=None, segments="all", filename=None, restore=False, **kwargs
-):
-    solver = SME_Solver(filename=filename, restore=restore)
-    return solver.solve(sme, param_names, segments, **kwargs)
+def solve(sme, param_names=None, segments="all", filename=None):
+    solver = SME_Solver(filename=filename)
+    return solver.solve(sme, param_names, segments)
```

### Comparing `pysme-astro-0.4.99/src/pysme/synthesize.py` & `pysme-astro-5.74.9/src/pysme/synthesize.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,53 +1,46 @@
-# -*- coding: utf-8 -*-
 """
 Spectral Synthesis Module of SME
 """
 import logging
-import uuid
+import warnings
 
 import numpy as np
+from tqdm import tqdm
 from scipy.constants import speed_of_light
-from scipy.interpolate import interp1d
 from scipy.ndimage.filters import convolve
-from tqdm import tqdm
+from scipy.interpolate import interp1d
+
 
 from . import broadening
 from .atmosphere.interpolation import AtmosphereInterpolator
-from .continuum_and_radial_velocity import (
-    apply_radial_velocity_and_continuum,
-    match_rv_continuum,
-    null_result,
-)
-from .iliffe_vector import Iliffe_vector
+from .continuum_and_radial_velocity import match_rv_continuum
 from .large_file_storage import setup_lfs
+from .iliffe_vector import Iliffe_vector
+from .nlte import update_nlte_coefficients
 from .sme_synth import SME_DLL
 
 logger = logging.getLogger(__name__)
 
 clight = speed_of_light * 1e-3  # km/s
 
-__DLL_DICT__ = {}
-__DLL_IDS__ = {}
-
 
 class Synthesizer:
     def __init__(self, config=None, lfs_atmo=None, lfs_nlte=None, dll=None):
         self.config, self.lfs_atmo, self.lfs_nlte = setup_lfs(
             config, lfs_atmo, lfs_nlte
         )
         # dict: internal storage of the adaptive wavelength grid
         self.wint = {}
         # dll: the smelib object used for the radiative transfer calculation
         self.dll = dll if dll is not None else SME_DLL()
-        self.dll = self.get_dll_id()
         self.atmosphere_interpolator = None
         # This stores a reference to the currently used sme structure, so we only log it once
         self.known_sme = None
-        logger.info("Don't forget to cite your sources. Use sme.citation()")
+        logger.critical("Don't forget to cite your sources. Use sme.citation()")
 
     def get_atmosphere(self, sme):
         """
         Return an atmosphere based on specification in an SME structure
 
         sme.atmo.method defines mode of action:
             "grid"
@@ -71,15 +64,15 @@
         # Handle atmosphere grid or user routine.
         atmo = sme.atmo
 
         if atmo.method == "grid":
             if self.atmosphere_interpolator is None:
                 self.atmosphere_interpolator = AtmosphereInterpolator(
                     depth=atmo.depth,
-                    interp=atmo.interp,
+                    interp=atmo.depth,
                     geom=atmo.geom,
                     lfs_atmo=self.lfs_atmo,
                 )
             else:
                 self.atmosphere_interpolator.depth = atmo.depth
                 self.atmosphere_interpolator.interp = atmo.interp
                 self.atmosphere_interpolator.geom = atmo.geom
@@ -94,32 +87,30 @@
             pass
         else:
             raise AttributeError("Source must be 'grid', 'routine', or 'embedded'")
 
         sme.atmo = atmo
         return sme
 
-    @staticmethod
-    def get_wavelengthrange(wran, vrad, vsini):
+    def get_wavelengthrange(self, wran, vrad, vsini):
         """
         Determine wavelengthrange that needs to be calculated
         to include all lines within velocity shift vrad + vsini
         """
         # 30 km/s == maximum barycentric velocity
         vrad_pad = 30.0 + 0.5 * np.clip(vsini, 0, None)  # km/s
         vbeg = vrad_pad + np.clip(vrad, 0, None)  # km/s
         vend = vrad_pad - np.clip(vrad, None, 0)  # km/s
 
         wbeg = wran[0] * (1 - vbeg / clight)
         wend = wran[1] * (1 + vend / clight)
         return wbeg, wend
 
-    @staticmethod
-    def new_wavelength_grid(wint):
-        """Generate new wavelength grid within bounds of wint"""
+    def new_wavelength_grid(self, wint):
+        """ Generate new wavelength grid within bounds of wint"""
         # Determine step size for a new model wavelength scale, which must be uniform
         # to facilitate convolution with broadening kernels. The uniform step size
         # is the larger of:
         #
         # [1] smallest wavelength step in WINT_SEG, which has variable step size
         # [2] 10% the mean dispersion of WINT_SEG
         # [3] 0.05 km/s, which is 1% the width of solar line profiles
@@ -167,28 +158,31 @@
             segments = [
                 seg
                 for seg in segments
                 if not np.all(sme.mask[seg] == sme.mask_values["bad"])
             ]
         return segments
 
-    @staticmethod
     def apply_radial_velocity_and_continuum(
-        wave, spec, wmod, smod, cmod, vrad, cscale, cscale_type, segments
+        self, wave, wmod, smod, cmod, vrad, cscale, segments
     ):
-        smod = apply_radial_velocity_and_continuum(
-            wave, wmod, smod, vrad, cscale, cscale_type, segments
-        )
-        cmod = apply_radial_velocity_and_continuum(
-            wave, wmod, cmod, vrad, None, None, segments
-        )
-        return smod, cmod
+        for il in segments:
+            if vrad[il] is not None:
+                rv_factor = np.sqrt((1 + vrad[il] / clight) / (1 - vrad[il] / clight))
+                wmod[il] *= rv_factor
+            smod[il] = np.interp(wave[il], wmod[il], smod[il])
+            if cmod is not None:
+                cmod[il] = np.interp(wave[il], wmod[il], cmod[il])
+
+            if cscale[il] is not None and not np.all(cscale[il] == 0):
+                x = wave[il] - wave[il][0]
+                smod[il] *= np.polyval(cscale[il], x)
+        return smod
 
-    @staticmethod
-    def integrate_flux(mu, inten, deltav, vsini, vrt, osamp=None):
+    def integrate_flux(self, mu, inten, deltav, vsini, vrt, osamp=1):
         """
         Produces a flux profile by integrating intensity profiles (sampled
         at various mu angles) over the visible stellar surface.
 
         Intensity profiles are weighted by the fraction of the projected
         stellar surface they represent, apportioning the area between
         adjacent MU points equally. Additional weights (such as those
@@ -275,57 +269,46 @@
         # Make local copies of various input variables, which will be altered below.
         # Force vsini and especially vmac to be scalars. Otherwise mu dependence fails.
 
         if np.size(vsini) > 1:
             vsini = vsini[0]
         if np.size(vrt) > 1:
             vrt = vrt[0]
-        nmu = np.size(mu)  # number of radii
+
+        # Determine oversampling factor.
+        os = round(np.clip(osamp, 1, None))  # force integral value > 1
 
         # Convert input MU to projected radii, R, of annuli for a star of unit radius
         #  (which is just sine, rather than cosine, of the angle between the outward
         #  normal and the line of sight).
         rmu = np.sqrt(1 - mu ** 2)  # use simple trig identity
-        if nmu > 1:
-            r = np.sqrt(
-                0.5 * (rmu[:-1] ** 2 + rmu[1:] ** 2)
-            )  # area midpoints between rmu
-            r = np.concatenate(([0], r, [1]))
-        else:
-            r = np.array([0, 1])
-
-        # Determine oversampling factor.
-        if osamp is None:
-            if vsini == 0:
-                os = 2
-            else:
-                os = deltav / (vsini * r[r != 0])
-                os = np.max(os[np.isfinite(os)])
-                os = int(np.ceil(os)) + 1
-        else:
-            os = osamp
-        # force integral value > 1
-        os = round(np.clip(os, 2, 10))
 
         # Sort the projected radii and corresponding intensity spectra into ascending
         #  order (i.e. from disk center to the limb), which is equivalent to sorting
         #  MU in descending order.
         isort = np.argsort(rmu)
         rmu = rmu[isort]  # reorder projected radii
-        if nmu == 1 and vsini != 0:
-            logger.warning(
-                "Vsini is non-zero, but only one projected radius (mu value) is set. No rotational broadening will be performed."
-            )
-            vsini = 0  # ignore vsini if only 1 mu
+        nmu = np.size(mu)  # number of radii
+        if nmu == 1:
+            if vsini != 0:
+                logger.warning(
+                    "Vsini is non-zero, but only one projected radius (mu value) is set. No rotational broadening will be performed."
+                )
+                vsini = 0  # ignore vsini if only 1 mu
 
         # Calculate projected radii for boundaries of disk integration annuli.  The n+1
         # boundaries are selected such that r(i+1) exactly bisects the area between
         # rmu(i) and rmu(i+1). The in!=rmost boundary, r(0) is set to 0 (disk center)
         # and the outermost boundary, r(nmu) is set to 1 (limb).
-        if nmu > 1:  # really want disk integration
+        if nmu > 1 or vsini != 0:  # really want disk integration
+            r = np.sqrt(
+                0.5 * (rmu[:-1] ** 2 + rmu[1:] ** 2)
+            )  # area midpoints between rmu
+            r = np.concatenate(([0], r, [1]))
+
             # Calculate integration weights for each disk integration annulus.  The weight
             # is just given by the relative area of each annulus, normalized such that
             # the sum of all weights is unity.  Weights for limb darkening are included
             # explicitly in the intensity profiles, so they aren't needed here.
             wt = r[1:] ** 2 - r[:-1] ** 2  # weights = relative areas
         else:
             wt = np.array([1.0])  # single mu value, full weight
@@ -348,25 +331,18 @@
         for imu in range(nmu):  # loop thru integration annuli
 
             #  Use external cubic spline routine (adapted from Numerical Recipes) to make
             #  an oversampled version of the intensity profile for the current annulus.
             ypix = inten[isort[imu]]  # extract intensity profile
             if os == 1:
                 # just copy (use) original profile
-                yfine = np.copy(ypix)
+                yfine = ypix
             else:
                 # spline onto fine wavelength scale
-                try:
-                    yfine = interp1d(
-                        xpix, ypix, kind="cubic", fill_value="extrapolate"
-                    )(xfine)
-                except ValueError:
-                    yfine = interp1d(
-                        xpix, ypix, kind="linear", fill_value="extrapolate"
-                    )(xfine)
+                yfine = interp1d(xpix, ypix, kind="cubic")(xfine)
 
             # Construct the convolution kernel which describes the distribution of
             # rotational velocities present in the current annulus. The distribution has
             # been derived analytically for annuli of arbitrary thickness in a rigidly
             # rotating star. The kernel is constructed in two pieces: o!= piece for
             # radial velocities less than the maximum velocity along the inner edge of
             # the annulus, and one piece for velocities greater than this limit.
@@ -390,16 +366,19 @@
                     (vsini * r2) ** 2 - v[j2] ** 2
                 )  # generate distribution
 
                 rkern = rkern / np.sum(rkern)  # normalize kernel
 
                 # Convolve the intensity profile with the rotational velocity kernel for this
                 # annulus. Pad each end of the profile with as many points as are in the
-                # convolution kernel. This reduces Fourier ringing.
-                yfine = convolve(yfine, rkern, mode="nearest")
+                # convolution kernel. This reduces Fourier ringing. The convolution may also
+                # be do!= with a routi!= called "externally" from IDL, which efficiently
+                # shifts and adds.
+                if nrk > 3:
+                    yfine = convolve(yfine, rkern, mode="nearest")
 
             # Calculate projected sigma for radial and tangential velocity distributions.
             muval = mu[isort[imu]]  # current value of mu
             sigma = os * vrt / np.sqrt(2) / deltav  # standard deviation in points
             sigr = sigma * muval  # reduce by current mu value
             sigt = sigma * np.sqrt(1.0 - muval ** 2)  # reduce by np.sqrt(1-mu**2)
 
@@ -430,169 +409,36 @@
             # Sum the radial and tangential components, weighted by surface area.
             area_r = 0.5  # assume equal areas
             area_t = 0.5  # ar+at must equal 1
             mkern = area_r * mrkern + area_t * mtkern  # add both components
 
             # Convolve the total flux profiles, again padding the spectrum on both ends to
             # protect against Fourier ringing.
-            yfine = convolve(yfine, mkern, mode="nearest")
+            yfine = convolve(
+                yfine, mkern, mode="nearest"
+            )  # add the padding and convolve
 
             # Add contribution from current annulus to the running total.
             flux = flux + wt[imu] * yfine  # add profile to running total
 
         flux = np.reshape(flux, (npts, os))  # convert to an array
         flux = np.pi * np.sum(flux, axis=1) / os  # sum, normalize
         return flux
 
-    def sequential_synthesize_segments(
-        self,
-        sme,
-        segments,
-        wmod,
-        smod,
-        cmod,
-        reuse_wavelength_grid,
-        dll_id=None,
-    ):
-        for il in tqdm(segments, desc="Segments", leave=False):
-            wmod[il], smod[il], cmod[il] = self.synthesize_segment(
-                sme,
-                il,
-                reuse_wavelength_grid,
-                il != segments[0],
-                dll_id=dll_id,
-            )
-        return wmod, smod, cmod
-
-    def get_dll_id(self, dll=None):
-        if dll is None:
-            dll = self.dll
-        if dll in __DLL_IDS__:
-            dll_id = __DLL_IDS__[dll]
-        elif dll in __DLL_DICT__:
-            dll_id = dll
-        else:
-            dll_id = uuid.uuid4()
-            __DLL_DICT__[dll_id] = dll
-            __DLL_IDS__[dll] = dll_id
-        return dll_id
-
-    def get_dll(self, dll_id=None):
-        if dll_id is None:
-            dll_id = self.dll
-        if dll_id in __DLL_DICT__:
-            return __DLL_DICT__[dll_id]
-        else:
-            return dll_id
-
-    def parallel_synthesize_segments(
-        self,
-        sme,
-        segments,
-        wmod,
-        smod,
-        cmod,
-        reuse_wavelength_grid,
-        dll_id=None,
-    ):
-        # Make sure the dll is recorded in the global variables
-        dll = self.get_dll(dll_id)
-        dll_id = self.get_dll_id(dll)
-
-        # We calculate the first segment sequentially
-        with tqdm(desc="Segments", total=len(segments), leave=False) as progress:
-            il = segments[0]
-            wmod[il], smod[il], cmod[il] = self.synthesize_segment(
-                sme, il, reuse_wavelength_grid, False, dll_id=dll_id
-            )
-            progress.update(1)
-            # and then all others in parrallel
-            # since we can keep the line opacities from the calculation of the first segment
-            # TODO: do the line opacities also in parallel?
-
-            # For multiple Processes we need to pickle all the components
-            # BUT we can not pickle the smelib, since it has pointers (in the state)
-            # Therefore we cheat by putting the library in a global variable
-            # but only with a unqiue id, that should be unique to this library
-
-            def parallel(il):
-                return self.synthesize_segment(
-                    sme,
-                    il,
-                    reuse_wavelength_grid,
-                    True,
-                    method="parallel",
-                    dll_id=dll_id,
-                )
-
-            # Sequential version for debugging
-            data = [None for _ in segments[1:]]
-            for i, seg in enumerate(segments[1:]):
-                data[i] = self.synthesize_segment(
-                    sme,
-                    seg,
-                    reuse_wavelength_grid,
-                    True,
-                    method="sequential",
-                    dll_id=dll_id,
-                )
-                progress.update(1)
-
-        # data_seq = [None for _ in segments[1:]]
-        # What is sticking around in the library that is not part of the state?
-        # for seg in segments[1:]:
-        #     i = seg-1
-        #     data_seq[i] = self.synthesize_segment(
-        #         sme,
-        #         seg,
-        #         reuse_wavelength_grid,
-        #         True,
-        #         method="sequential",
-        #         dll_id=dll_id,
-        #     )
-
-        #     if not np.all(data[i][0] == data_seq[i][0]):
-        #         print("What")
-        #     if not np.all(data[i][1] == data_seq[i][1]):
-        #         print("The")
-        #     if not np.all(data[i][2] == data_seq[i][2]):
-        #         print("Hell")
-
-        # Pathos version crashes for some reason
-        # with ThreadPool() as pool:
-        #     data = pool.map(parallel, segments[1:])
-
-        # Use "default" ThreadPool instead
-        # data = [None for _ in segments[1:]]
-        # with ThreadPoolExecutor() as executor:
-        #     futures = {executor.submit(parallel, il): il for il in segments[1:]}
-        #     for future in as_completed(futures):
-        #         il = futures[future] - 1
-        #         data[il] = future.result()
-
-        for i, seg in enumerate(segments[1:]):
-            wmod[seg] = data[i][0]
-            smod[seg] = data[i][1]
-            cmod[seg] = data[i][2]
-
-        return wmod, smod, cmod
-
     def synthesize_spectrum(
         self,
         sme,
         segments="all",
         passLineList=True,
         passAtmosphere=True,
         passNLTE=True,
         updateStructure=True,
         updateLineList=False,
         reuse_wavelength_grid=False,
         radial_velocity_mode="robust",
-        method="sequential",
-        dll_id=None,
     ):
         """
         Calculate the synthetic spectrum based on the parameters passed in the SME structure
         The wavelength range of each segment is set in sme.wran
         The specific wavelength grid is given by sme.wave, or is generated on the fly if sme.wave is None
 
         Will try to fit radial velocity RV and continuum to observed spectrum, depending on vrad_flag and cscale_flag
@@ -632,103 +478,70 @@
         if "spec" not in sme:
             sme.vrad_flag = "none"
             sme.cscale_flag = "none"
         else:
             if "mask" not in sme:
                 sme.mask = np.full(sme.spec.size, sme.mask_values["line"])
             for i in range(sme.nseg):
-                mask = ~np.isfinite(sme.spec[i])
-                mask |= sme.uncs[i] == 0
-                sme.mask[i][mask] = sme.mask_values["bad"]
+                sme.mask[i, ~np.isfinite(sme.spec[i])] = 0
 
         if radial_velocity_mode != "robust" and (
             "cscale" not in sme or "vrad" not in sme
         ):
             radial_velocity_mode = "robust"
 
-        segments = self.check_segments(sme, segments)
+        segments = Synthesizer.check_segments(sme, segments)
 
         # Prepare arrays
-        vrad, _, cscale, _ = null_result(sme.nseg, sme.cscale_degree, sme.cscale_type)
+        vrad = np.zeros(n_segments)
+        cscale = np.zeros((n_segments, cscale_degree + 1))
+        cscale[:, -1] = 1
 
         wave = [np.zeros(0) for _ in range(n_segments)]
         smod = [[] for _ in range(n_segments)]
         cmod = [[] for _ in range(n_segments)]
         wmod = [[] for _ in range(n_segments)]
 
         # If wavelengths are already defined use those as output
         if "wave" in sme:
             wave = [w for w in sme.wave]
 
-        if method == "parallel" and not self.get_dll(dll_id).parallel:
-            # display only once
-            if (
-                not hasattr(self, "_warning_parallel_mode")
-                or not self._warning_parallel_mode
-            ):
-                self._warning_parallel_mode = True
-                logger.warning(
-                    "Parallel mode was requested, but the library in use is a sequential version. Running in sequential mode instead"
-                )
-            method = "sequential"
-
-        if method == "parallel":
-            dll = self.get_dll(dll_id).copy()
-            dll_id = self.get_dll_id(dll)
-        else:
-            dll = self.get_dll(dll_id)
-
         # Input Model data to C library
-        dll.SetLibraryPath()
+        self.dll.SetLibraryPath()
         if passLineList:
-            dll.InputLineList(sme.linelist)
+            self.dll.InputLineList(sme.linelist)
         if updateLineList:
             # TODO Currently Updates the whole linelist, could be improved to only change affected lines
-            dll.UpdateLineList(sme.atomic, sme.species, np.arange(len(sme.linelist)))
+            self.dll.UpdateLineList(
+                sme.atomic, sme.species, np.arange(len(sme.linelist))
+            )
         if passAtmosphere:
             sme = self.get_atmosphere(sme)
-            dll.InputModel(sme.teff, sme.logg, sme.vmic, sme.atmo)
-            dll.InputAbund(sme.abund)
-            dll.Ionization(0)
-            dll.SetVWscale(sme.gam6)
-            dll.SetH2broad(sme.h2broad)
+            self.dll.InputModel(sme.teff, sme.logg, sme.vmic, sme.atmo)
+            self.dll.InputAbund(sme.abund)
+            self.dll.Ionization(0)
+            self.dll.SetVWscale(sme.gam6)
+            self.dll.SetH2broad(sme.h2broad)
         if passNLTE:
-            sme.nlte.update_coefficients(sme, dll, self.lfs_nlte)
+            sme.nlte.update_coefficients(sme, self.dll, self.lfs_nlte)
 
         # Loop over segments
         #   Input Wavelength range and Opacity
         #   Calculate spectral synthesis for each
         #   Interpolate onto geomspaced wavelength grid
         #   Apply instrumental and turbulence broadening
 
         # TODO Parallelization
         # This requires changes in the C code however, since SME uses global parameters
         # for the wavelength range (and opacities) which change within each segment
-        if dll.parallel:
-            wmod, smod, cmod = self.parallel_synthesize_segments(
-                sme,
-                segments,
-                wmod,
-                smod,
-                cmod,
-                reuse_wavelength_grid,
-                dll_id=dll,
-            )
-        else:
-            wmod, smod, cmod = self.sequential_synthesize_segments(
-                sme,
-                segments,
-                wmod,
-                smod,
-                cmod,
-                reuse_wavelength_grid,
-                dll_id=dll,
+        for il in tqdm(segments, desc="Segment", leave=False):
+            wmod[il], smod[il], cmod[il] = self.synthesize_segment(
+                sme, il, reuse_wavelength_grid, il != segments[0]
             )
 
-        for il in segments:
             if "wave" not in sme or len(sme.wave[il]) == 0:
                 # trim padding
                 wbeg, wend = sme.wran[il]
                 itrim = (wmod[il] > wbeg) & (wmod[il] < wend)
                 # Force endpoints == wavelength range
                 wave[il] = np.concatenate(([wbeg], wmod[il][itrim], [wend]))
 
@@ -744,24 +557,16 @@
             logger.debug("Radial velocity: %s", str(vrad))
             logger.debug("Continuum coefficients: %s", str(cscale))
         elif radial_velocity_mode == "fast":
             cscale, vrad = sme.cscale, sme.vrad
         else:
             raise ValueError("Radial Velocity mode not understood")
 
-        smod, cmod = self.apply_radial_velocity_and_continuum(
-            wave,
-            sme.spec,
-            wmod,
-            smod,
-            cmod,
-            vrad,
-            cscale,
-            sme.cscale_type,
-            segments,
+        smod = self.apply_radial_velocity_and_continuum(
+            wave, wmod, smod, cmod, vrad, cscale, segments
         )
 
         # Merge all segments
         # if sme already has a wavelength this should be the same
         if updateStructure:
             if "wave" not in sme:
                 # TODO: what if not all segments are there?
@@ -772,45 +577,31 @@
                 sme.cont = cmod
 
             for s in segments:
                 sme.wave[s] = wave[s]
                 sme.synth[s] = smod[s]
                 sme.cont[s] = cmod[s]
 
-            if sme.cscale_type in ["spline", "spline+mask"]:
-                sme.cscale = np.asarray(cscale)
-                sme.cscale_unc = np.asarray(cscale_unc)
-            elif sme.cscale_flag not in ["fix", "none"]:
-                for s in np.arange(sme.nseg):
-                    if s not in segments:
-                        cscale[s] = sme.cscale[s]
-                sme.cscale = np.asarray(cscale)
-                sme.cscale_unc = np.asarray(cscale_unc)
+            if sme.cscale_flag not in ["fix", "none"]:
+                for s in segments:
+                    sme.cscale[s] = cscale[s]
+                sme.cscale_unc = cscale_unc
 
             sme.vrad = np.asarray(vrad)
             sme.vrad_unc = np.asarray(vrad_unc)
-            sme.nlte.flags = dll.GetNLTEflags()
-            result = sme
+            sme.nlte.flags = self.dll.GetNLTEflags()
+            return sme
         else:
             wave = Iliffe_vector(values=wave)
             smod = Iliffe_vector(values=smod)
             cmod = Iliffe_vector(values=cmod)
-            result = wave, smod, cmod
-
-        # Cleanup
-        return result
+            return wave, smod, cmod
 
     def synthesize_segment(
-        self,
-        sme,
-        segment,
-        reuse_wavelength_grid=False,
-        keep_line_opacity=False,
-        method="sequential",
-        dll_id=None,
+        self, sme, segment, reuse_wavelength_grid=False, keep_line_opacity=False
     ):
         """Create the synthetic spectrum of a single segment
 
         Parameters
         ----------
         sme : SME_Struct
             The SME strcuture containing all relevant parameters
@@ -829,43 +620,37 @@
             Wavelength grid of the synthesized spectrum
         flux : array of shape (npoints,)
             The Flux of the synthesized spectrum
         cont_flux : array of shape (npoints,)
             The continuum Flux of the synthesized spectrum
         """
         logger.debug("Segment %i out of %i", segment, sme.nseg)
-        if method == "parallel":
-            dll = self.get_dll(dll_id).copy()
-            dll_id = self.get_dll_id(dll)
-        else:
-            dll = self.get_dll(dll_id)
 
         # Input Wavelength range and Opacity
         vrad_seg = sme.vrad[segment] if sme.vrad[segment] is not None else 0
         wbeg, wend = self.get_wavelengthrange(sme.wran[segment], vrad_seg, sme.vsini)
 
-        dll.InputWaveRange(wbeg, wend)
-        dll.Opacity()
+        self.dll.InputWaveRange(wbeg, wend)
+        self.dll.Opacity()
 
         # Reuse adaptive wavelength grid in the jacobians
         if reuse_wavelength_grid and segment in self.wint.keys():
             wint_seg = self.wint[segment]
         else:
             wint_seg = None
 
         # Only calculate line opacities in the first segment
         #   Calculate spectral synthesis for each
-        _, wint, sint, cint = dll.Transf(
+        _, wint, sint, cint = self.dll.Transf(
             sme.mu,
             sme.accrt,  # threshold line opacity / cont opacity
             sme.accwi,
             keep_lineop=keep_line_opacity,
             wave=wint_seg,
         )
-
         # Store the adaptive wavelength grid for the future
         # if it was newly created
         if wint_seg is None:
             self.wint[segment] = wint
 
         if not sme.specific_intensities_only:
             # Create new geomspaced wavelength grid, to be used for intermediary steps
@@ -884,21 +669,21 @@
 
             # Turbulence broadening
             # Apply macroturbulent and rotational broadening while integrating intensities
             # over the stellar disk to produce flux spectrum Y.
             sint = self.integrate_flux(sme.mu, y_integrated, vstep, sme.vsini, sme.vmac)
             wint = wgrid
 
-            # instrument broadening
-            if "iptype" in sme:
-                logger.debug("Apply detector broadening")
-                ipres = sme.ipres if np.size(sme.ipres) == 1 else sme.ipres[segment]
-                sint = broadening.apply_broadening(
-                    ipres, wint, sint, type=sme.iptype, sme=sme
-                )
+        # instrument broadening
+        if "iptype" in sme:
+            logger.debug("Apply detector broadening")
+            ipres = sme.ipres if np.size(sme.ipres) == 1 else sme.ipres[segment]
+            sint = broadening.apply_broadening(
+                ipres, wint, sint, type=sme.iptype, sme=sme
+            )
 
         # Divide calculated spectrum by continuum
         if sme.normalize_by_continuum:
             sint /= cint
 
         return wint, sint, cint
```

### Comparing `pysme-astro-0.4.99/src/pysme/uncertainties.py` & `pysme-astro-5.74.9/src/pysme/uncertainties.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-# -*- coding: utf-8 -*-
 import logging
-
 import numpy as np
 from scipy.optimize import curve_fit
 
 logger = logging.getLogger(__name__)
 
 
 def uncertainties(pder, resid, unc, freep_name, plot=False):
```

### Comparing `pysme-astro-0.4.99/src/pysme/util.py` & `pysme-astro-5.74.9/src/pysme/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
 """
 Utility functions for SME
 
 safe interpolation
 """
 
 import argparse
+import logging
+from functools import wraps
+from platform import python_version
+import sys
 import builtins
 import contextlib
-import logging
 import os
 import subprocess
-import sys
-from functools import wraps
-from platform import python_version
 
 import numpy as np
 from numpy import __version__ as npversion
 from pandas import __version__ as pdversion
 from scipy import __version__ as spversion
 from scipy.interpolate import interp1d
+from tqdm import tqdm
 
 from . import __version__ as smeversion
 from .sme_synth import SME_DLL
 
 logger = logging.getLogger(__name__)
 
 
@@ -31,15 +31,15 @@
 def print_to_log():
     original_print = builtins.print
 
     def logprint(*args, file=None, **kwargs):
         # The debugger freaks out if we dont give it what it wants
         if file is not None:
             original_print(*args, **kwargs, file=file)
-        elif len(args) != 0:
+        else:
             logger.info(*args, **kwargs)
 
     builtins.print = logprint
     try:
         yield None
     finally:
         builtins.print = original_print
@@ -315,15 +315,15 @@
     if x_new is not None:
         return interpolator(x_new)
     else:
         return interpolator
 
 
 def log_version():
-    """For Debug purposes"""
+    """ For Debug purposes """
     dll = SME_DLL()
     logger.debug("----------------------")
     logger.debug("Python version: %s", python_version())
     try:
         logger.debug("SME CLib version: %s", dll.SMELibraryVersion())
     except OSError:
         logger.debug("SME CLib version: ???")
```

### Comparing `pysme-astro-0.4.99/src/pysme_astro.egg-info/PKG-INFO` & `pysme-astro-5.74.9/src/pysme_astro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: pysme-astro
-Version: 0.4.99
+Version: 5.74.9
 Summary: Spectroscopy Made Easy
 Home-page: https://github.com/AWehrhahn/SME/
 Author: Ansgar Wehrhahn, Jeff A. Valenti
 Author-email: ansgar.wehrhahn@physics.uu.se, valenti@stsci.edu
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/AWehrhahn/SME/issues
 Project-URL: Documentation, https://pysme-astro.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/AWehrhahn/SME/
-Description: ![Python application](https://github.com/AWehrhahn/SME/workflows/Python%20application/badge.svg)
+Description: [![Build Status](https://travis-ci.com/AWehrhahn/SME.svg?branch=master)](https://travis-ci.com/AWehrhahn/SME)
         [![Documentation Status](https://readthedocs.org/projects/pysme-astro/badge/?version=latest)](https://pysme-astro.readthedocs.io/en/latest/?badge=latest)
-        [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.5547527.svg)](https://doi.org/10.5281/zenodo.5547527)
+        [![DOI](https://zenodo.org/badge/150097199.svg)](https://zenodo.org/badge/latestdoi/150097199)
         
         
         
         # PySME
         
         Spectroscopy Made Easy (SME) is a software tool that fits an observed
         spectrum of a star with a model spectrum. Since its initial release in
```

### Comparing `pysme-astro-0.4.99/src/pysme_astro.egg-info/SOURCES.txt` & `pysme-astro-5.74.9/src/pysme_astro.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,26 @@
-LICENSE
 MANIFEST.in
 README.md
-pyproject.toml
 setup.cfg
 setup.py
 versioneer.py
 src/pysme/__init__.py
-src/pysme/__main__.py
 src/pysme/_version.py
 src/pysme/abund.py
 src/pysme/broadening.py
 src/pysme/config.py
-src/pysme/config_default.json
 src/pysme/continuum_and_radial_velocity.py
 src/pysme/cwrapper.py
 src/pysme/data_structure.py
 src/pysme/datafiles_atmospheres.json
 src/pysme/datafiles_nlte.json
 src/pysme/echelle.py
 src/pysme/iliffe_vector.py
 src/pysme/large_file_storage.py
-src/pysme/libtools.py
 src/pysme/nlte.py
-src/pysme/nso.py
 src/pysme/persistence.py
 src/pysme/sme.py
 src/pysme/sme_synth.py
 src/pysme/solve.py
 src/pysme/synthesize.py
 src/pysme/uncertainties.py
 src/pysme/util.py
@@ -37,15 +31,14 @@
 src/pysme/atmosphere/savfile.py
 src/pysme/gui/__init__.py
 src/pysme/gui/plot_colors.py
 src/pysme/gui/plot_plotly.py
 src/pysme/gui/plot_pyplot.py
 src/pysme/linelist/VALD3_ref.bib
 src/pysme/linelist/__init__.py
-src/pysme/linelist/ges.py
 src/pysme/linelist/linelist.py
 src/pysme/linelist/vald.py
 src/pysme_astro.egg-info/PKG-INFO
 src/pysme_astro.egg-info/SOURCES.txt
 src/pysme_astro.egg-info/dependency_links.txt
 src/pysme_astro.egg-info/requires.txt
 src/pysme_astro.egg-info/top_level.txt
```

### Comparing `pysme-astro-0.4.99/test/test_abund.py` & `pysme-astro-5.74.9/test/test_abund.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-# -*- coding: utf-8 -*-
 from collections import OrderedDict
 
 import numpy as np
 import pytest
-
 from pysme.abund import Abund
 
 pattern_names = ["Asplund2009", "Grevesse2007", "Empty"]
 types = ["H=12", "n/nH", "n/nTot", "SME"]
 
 
 def test_init_with_too_few_args():
-    """Test that __init__ raise an error if too few arguments are passed."""
+    """Test that __init__ raise an error if too few arguments are passed.
+    """
     Abund()
     Abund(monh=0)
     Abund(pattern="asplund2009")
     Abund(type="H=12")
 
 
 def test_init_using_pattern_names():
-    """Test handling of abundance pattern name passed to __init__()."""
+    """Test handling of abundance pattern name passed to __init__().
+    """
     # Each abundance pattern name yields an Abund object.
     for pattern_name in pattern_names:
         assert isinstance(Abund(pattern=pattern_name, monh=0), Abund)
 
     # The 'Empty' abundance pattern has a value of None for all elements.
     abund = Abund(monh=0, pattern="Empty")
     pattern = abund.get_pattern(raw=True)
@@ -49,15 +49,16 @@
     the specified element or list of elements.
     """
     abund = Abund(pattern=pattern_names[0], monh=0)
     assert abund["H"] == 12
 
 
 def test_monh_property_set_and_get():
-    """Test setting and getting monh property. Set converts input to float."""
+    """Test setting and getting monh property. Set converts input to float.
+    """
     # Input str convertable to float yields a float with the specified value.
     abund = Abund(pattern=pattern_names[0], monh="-6e-1")
     assert isinstance(abund.monh, float)
     assert abund.monh == -0.6
 
     # Input int yields a float with the specified value.
     abund.monh = -2
@@ -75,15 +76,16 @@
 
     # Input that is not a string or a number raises an error.
     with pytest.raises(TypeError):
         abund.monh = []
 
 
 def test_pattern_property_set_and_get():
-    """Test setting and getting pattern property. Set is not allowed."""
+    """Test setting and getting pattern property. Set is not allowed.
+    """
     # Raise error is user tries to set pattern
     abund = Abund(pattern="Empty", monh=0)
     with pytest.raises(AttributeError):
         abund.pattern = 0.0
 
 
 def test_update_pattern():
```

### Comparing `pysme-astro-0.4.99/test/test_atmospheres.py` & `pysme-astro-5.74.9/test/test_atmospheres.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-# -*- coding: utf-8 -*-
 # TODO implement atmosphere tests
-import numpy as np
 import pytest
-
+import numpy as np
 from pysme.atmosphere.atmosphere import Atmosphere
-from pysme.atmosphere.interpolation import AtmosphereInterpolator
 from pysme.atmosphere.savfile import SavFile
+from pysme.atmosphere.interpolation import AtmosphereInterpolator
+from pysme.large_file_storage import setup_atmo
 
-from .test_largefilestorage import lfs_atmo, skipif_lfs
+from .test_largefilestorage import skipif_lfs, lfs_atmo
 
 
 @pytest.fixture
 def atmosphere_name():
     # TODO iterate over all possible options
     return "marcs2012p_t1.0.sav"
 
@@ -34,15 +33,15 @@
     return interp
 
 
 @pytest.fixture
 @pytest.mark.usefixtures("lfs_atmo")
 def atmosphere_grid(atmosphere_name, lfs_atmo):
     name = lfs_atmo.get(atmosphere_name)
-    atmo = SavFile(name, source=name)
+    atmo = SavFile(name)
     return atmo
 
 
 @skipif_lfs
 @pytest.mark.usefixtures("lfs_atmo")
 def test_grid_point(atmosphere_name, atmosphere_grid, lfs_atmo, interpolator):
     # TODO: get this values from the grid
```

### Comparing `pysme-astro-0.4.99/test/test_continuum_and_rv.py` & `pysme-astro-5.74.9/test/test_continuum_and_rv.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,121 +1,68 @@
-# -*- coding: utf-8 -*-
 # TODO implement continuum and radial velocity tests
 
-from itertools import product
+from os.path import dirname
 
-import numpy as np
 import pytest
+import numpy as np
 
-from pysme.continuum_and_radial_velocity import (
-    apply_radial_velocity_and_continuum,
-    match_rv_continuum,
-)
+from pysme.sme import SME_Structure as SME_Struct
+from pysme.continuum_and_radial_velocity import determine_rv_and_cont
 
 
 def test_match_both(testcase1):
     sme, x_syn, y_syn, rv = testcase1
 
     # Fix random results of the MCMC
     np.random.seed(0)
 
-    vrad_options = ["none", "fix", "each", "whole"]
-    cscale_options = ["none", "fix", "constant", "linear"]  # quadratic
-    cscale_types = [
-        "mask",
-        "match",
-        "match+mask",
-        "mcmc",
-        "spline",
-        "spline+mask",
-    ]
-
-    # vrad_options = ["whole"]
-    # cscale_options = ["linear"]  # quadratic
-    # cscale_types = ["spline", "spline+mask"]
-    segments = [[0], range(sme.nseg)]
-
-    for voption, coption, ctype, segment in product(
-        vrad_options, cscale_options, cscale_types, segments
-    ):
-        sme.vrad_flag = voption
-        sme.cscale_flag = coption
-        sme.cscale_type = ctype
-        sme.vrad = None
-        sme.cscale = None
-
-        # Determine the radial velocity and the continuum
-        cscale, cunc, vrad, vunc = match_rv_continuum(
-            sme, segment, x_syn[segment], y_syn[segment]
-        )
-
-        # check that it can be applied
-        smod = apply_radial_velocity_and_continuum(
-            sme.wave, x_syn, y_syn, vrad, cscale, ctype, segment, copy=True
-        )
-
-        assert vrad is not None
-        assert vunc is not None
-        assert cscale is not None
-        assert cunc is not None
-
-        assert vrad.ndim == 1
-        assert vrad.shape[0] == sme.nseg
-        assert vunc.ndim == 2
-        assert vunc.shape[0] == sme.nseg
-        assert vunc.shape[1] == 2
-
-        assert cscale.ndim == 2
-        assert cscale.shape[0] == sme.nseg
-        if ctype in ["mask", "match", "match+mask", "mcmc"]:
-            assert cscale.shape[1] == sme.cscale_degree + 1
-        elif ctype in ["spline", "spline+mask"]:
-            assert np.allclose(cscale.shape[1], sme.cscale_degree)
-        else:
-            pass
-
-        if ctype in ["mask", "match", "match+mask", "mcmc"]:
-            assert cunc.ndim == 3
-            assert cunc.shape[0] == sme.nseg
-            assert cunc.shape[1] == sme.cscale_degree + 1
-            assert cunc.shape[2] == 2
-        elif ctype in ["spline", "spline+mask"]:
-            assert cunc.ndim == 2
-            assert cunc.shape[0] == sme.nseg
-            assert np.allclose(cunc.shape[1], sme.cscale_degree)
-        else:
-            pass
-
-        if voption in ["none", "fix"]:
-            assert np.all(vrad == 0)
-        else:
-            for seg in range(sme.nseg):
-                if seg in segment:
-                    assert np.allclose(vrad[seg], rv, atol=1)
+    vrad_options = ["fix", "none", "each", "whole"]
+    cscale_options = ["fix", "none", "constant", "linear"]  # quadratic
+
+    for voption in vrad_options:
+        for coption in cscale_options:
+            for segment in [[0], range(sme.nseg)]:
+                sme.vrad_flag = voption
+                sme.cscale_flag = coption
+                sme.vrad = None
+                sme.cscale = None
+
+                vrad, vunc, cscale, cunc = determine_rv_and_cont(
+                    sme, segment, x_syn[segment], y_syn[segment]
+                )
+
+                assert vrad is not None
+                assert vunc is not None
+                assert cscale is not None
+                assert cunc is not None
+
+                assert vrad.ndim == 1
+                assert vrad.shape[0] == len(segment)
+                assert vunc.ndim == 2
+                assert vunc.shape[0] == len(segment)
+                assert vunc.shape[1] == 2
+                assert cscale.ndim == 2
+                assert cscale.shape[0] == len(segment)
+                assert cscale.shape[1] == sme.cscale_degree + 1
+                assert cunc.ndim == 3
+                assert cunc.shape[0] == len(segment)
+                assert cunc.shape[1] == sme.cscale_degree + 1
+                assert cunc.shape[2] == 2
+
+                if voption in ["none", "fix"]:
+                    assert np.all(vrad == 0)
                 else:
-                    assert vrad[seg] == 0
+                    assert np.allclose(vrad, rv, atol=1)
 
-        if ctype in ["mask", "match", "match+mask", "mcmc"]:
-            if coption in ["none", "fix"]:
-                assert np.all(cscale[:, -1] == 1)
-                assert np.all(cscale[:, :-1] == 0)
-            else:
                 assert np.allclose(cscale[:, -1], 1, atol=1e-1)
                 assert np.allclose(cscale[:, :-1], 0, atol=1e-1)
-        elif ctype in ["spline", "spline+mask"]:
-            if coption in ["none", "fix"]:
-                assert np.all(cscale == 1)
-            else:
-                pass
-        else:
-            pass
-
-
-# def test_nomask(testcase1):
-#     sme, x_syn, y_syn, rv = testcase1
-#     sme.cscale_flag = "constant"
-#     sme.vrad_flag = "each"
-#     sme.cscale_type = "mask"
-
-#     sme.mask = 0
-#     with pytest.warns(UserWarning):
-#         rvel, vunc, cscale, cunc = match_rv_continuum(sme, 0, x_syn, y_syn)
+
+
+def test_nomask(testcase1):
+    sme, x_syn, y_syn, rv = testcase1
+    sme.cscale_flag = "constant"
+    sme.vrad_flag = "each"
+
+    sme.mask = 0
+    with pytest.warns(UserWarning):
+        rvel, vunc, cscale, cunc = determine_rv_and_cont(sme, 0, x_syn[0], y_syn[0])
+
```

### Comparing `pysme-astro-0.4.99/test/test_dll.py` & `pysme-astro-5.74.9/test/test_dll.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-# -*- coding: utf-8 -*-
 from os.path import dirname
 
-import numpy as np
 import pytest
+import numpy as np
 
+from pysme.sme import SME_Structure as SME_Struct
 from pysme.abund import Abund
 from pysme.atmosphere.krzfile import KrzFile
 from pysme.linelist.linelist import LineList
 from pysme.sme_synth import SME_DLL
-
+from pysme.nlte import nlte
 
 # Create Objects to pass to library
 # Their functionality is tested in other test files, so we assume it works
 @pytest.fixture
 def cwd():
     return dirname(__file__)
 
@@ -83,37 +83,31 @@
 
 @pytest.fixture
 def abund():
     return Abund(monh=0, pattern="Asplund2009")
 
 
 def test_basic(libsme, wfirst, wlast, vw_scale):
-    """Test instantiation of library object and some basic functions"""
+    """ Test instantiation of library object and some basic functions """
     print(libsme.SMELibraryVersion())
     libsme.InputWaveRange(wfirst, wlast)
     libsme.SetVWscale(vw_scale)
     libsme.SetH2broad()
 
-    print(
-        libsme.file,
-        libsme.wfirst,
-        libsme.wlast,
-        libsme.vw_scale,
-        libsme.h2broad,
-    )
+    print(libsme.file, libsme.wfirst, libsme.wlast, libsme.vw_scale, libsme.h2broad)
 
     # assert libsme.file
     assert libsme.wfirst == wfirst
     assert libsme.wlast == wlast
     assert libsme.vw_scale == vw_scale
     assert libsme.h2broad
 
 
 def test_linelist(libsme, linelist):
-    """Test linelist behaviour"""
+    """ Test linelist behaviour """
     libsme.InputLineList(linelist)
     outlist = libsme.OutputLineList()
 
     print(libsme.linelist)
     fmt = "  Out: {0:10.4f},{2:7.4f},{1:7.3f},{3:5.2f},{4:6.2f},{5:8.3f}"
     for i in range(len(linelist)):
         outline = [x for x in outlist[i]]
@@ -124,15 +118,15 @@
     # libsme.UpdateLineList()
 
     with pytest.raises(TypeError):
         libsme.InputLineList(None)
 
 
 def test_atmosphere(libsme, atmo, teff, grav, vturb):
-    """Test atmosphere behaviour"""
+    """ Test atmosphere behaviour """
 
     libsme.InputModel(teff, grav, vturb, atmo)
 
     # TODO test different geometries
 
     assert libsme.teff == teff
     assert libsme.grav == grav
@@ -146,15 +140,15 @@
         libsme.InputModel(teff, grav, -10, atmo)
 
     with pytest.raises(TypeError):
         libsme.InputModel(teff, grav, vturb, None)
 
 
 def test_abund(libsme, abund):
-    """Test abundance behaviour"""
+    """ Test abundance behaviour """
     libsme.InputAbund(abund)
 
     # TODO: What should be the expected behaviour?
     empty = Abund(monh=0, pattern="empty")
     empty.update_pattern({"H": 12})
     libsme.InputAbund(empty)
 
@@ -173,15 +167,15 @@
     vw_scale,
     wfirst,
     wlast,
     mu,
     accrt,
     accwt,
 ):
-    """Test radiative transfer"""
+    """ Test radiative transfer """
     libsme.SetLibraryPath()
 
     libsme.InputLineList(linelist)
     libsme.InputModel(teff, grav, vturb, atmo)
     libsme.InputAbund(abund)
     libsme.Ionization(0)
     libsme.SetVWscale(vw_scale)
@@ -210,9 +204,8 @@
     print(atmo.xne)
     assert np.allclose(xna, atmo.xna, rtol=1e-1)
 
     libsme.GetLineOpacity(linelist.wlcent[0])
     libsme.GetLineRange()
     for switch in range(-3, 13):
         if switch != 8:
-            print(switch)
             libsme.GetOpacity(switch)
```

### Comparing `pysme-astro-0.4.99/test/test_nlte.py` & `pysme-astro-5.74.9/test/test_nlte.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,40 @@
-# -*- coding: utf-8 -*-
 # TODO implement NLTE tests
 
+import pytest
+
 import os
-import tempfile
 from os.path import dirname
+import tempfile
 
 import numpy as np
-import pytest
 
-from pysme.abund import Abund
-from pysme.linelist.vald import ValdFile
-from pysme.nlte import DirectAccessFile, nlte
 from pysme.sme import SME_Structure as SME_Struct
+from pysme.iliffe_vector import Iliffe_vector
+from pysme.linelist.vald import ValdFile
 from pysme.sme_synth import SME_DLL
+from pysme.nlte import nlte, DirectAccessFile
 from pysme.synthesize import Synthesizer, synthesize_spectrum
+from pysme.config import Config
+from pysme.abund import Abund
 
-from .test_largefilestorage import lfs_atmo, lfs_nlte, skipif_lfs
+from .test_largefilestorage import skipif_lfs, lfs_nlte, lfs_atmo
 
 cwd = dirname(__file__)
 
 
 def make_minimum_structure():
     sme = SME_Struct()
     sme.teff = 5000
     sme.logg = 4.4
     sme.vmic = 1
     sme.vmac = 1
     sme.vsini = 1
     sme.abund = Abund.solar()
-    sme.linelist = ValdFile("{}/testcase3.lin".format(cwd))
+    sme.linelist = ValdFile("{}/testcase3.lin".format((cwd)))
     sme.atmo.source = "marcs2012p_t2.0.sav"
     sme.atmo.method = "grid"
 
     sme.wran = [[6436, 6444]]
 
     return sme
 
@@ -113,15 +115,15 @@
 
     # This is essentially what update_depcoefs does, just for one element
     counter = 0
     bmat, linerefs, lineindices = nlte(sme, libsme, elem, lfs_nlte)
     for lr, li in zip(linerefs, lineindices):
         if lr[0] != -1 and lr[1] != -1:
             counter += 1
-            libsme.InputNLTE(bmat[:, lr].T, li)
+            libsme.InputNLTE(bmat[:, lr], li)
 
     flags = libsme.GetNLTEflags()
     assert np.any(flags)
     assert np.count_nonzero(flags) == counter
     assert len(flags) == len(sme.linelist)
 
     idx = np.where(flags)[0][0]
@@ -134,21 +136,21 @@
     assert not np.any(flags)
     assert len(flags) == len(sme.linelist)
 
     with pytest.raises(TypeError):
         libsme.InputNLTE(None, 0)
 
     with pytest.raises(TypeError):
-        libsme.InputNLTE(bmat[:, [0, 1]].T, 0.1)
+        libsme.InputNLTE(bmat[:, [0, 1]], 0.1)
 
     with pytest.raises(ValueError):
         libsme.InputNLTE([0, 1], 10)
 
     with pytest.raises(ValueError):
-        libsme.InputNLTE(bmat[:, [0, 1]].T, -10)
+        libsme.InputNLTE(bmat[:, [0, 1]], -10)
 
 
 @pytest.fixture
 def temp():
     file = tempfile.NamedTemporaryFile(delete=False)
     yield file.name
     try:
```

### Comparing `pysme-astro-0.4.99/test/test_sme_structure.py` & `pysme-astro-5.74.9/test/test_sme_structure.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,33 @@
-# -*- coding: utf-8 -*-
-from os import remove
-from os.path import dirname
+import pytest
 
 import numpy as np
-import pytest
+from os.path import dirname
+from os import remove
 
 from pysme.sme import SME_Structure as SME_Struct
 
 
 @pytest.fixture
 def cwd():
     return dirname(__file__)
 
 
 @pytest.fixture
 def filename(cwd):
-    fname = "{}/__test.sme".format(cwd)
+    fname = "{}/__test.sme".format((cwd))
     yield fname
     try:
         remove(fname)
     except:
         pass
 
 
 def test_empty_structure():
-    """Test that all properties behave well when nothing is set"""
+    """ Test that all properties behave well when nothing is set """
     empty = SME_Struct()
 
     assert isinstance(empty.version, str)
     assert empty.teff is not None
     assert empty.logg is not None
     assert empty.vmic == 0
     assert empty.vmac == 0
@@ -100,15 +99,15 @@
     sme = SME_Struct.load(filename)
     assert np.all(sme.wave[0] == data)
     assert np.all(sme.spec[0] == data)
     assert sme.nseg == 1
 
 
 def test_load_idl_savefile(cwd):
-    filename = "{}/testcase1.inp".format(cwd)
+    filename = "{}/testcase1.inp".format((cwd))
     sme = SME_Struct.load(filename)
 
     assert sme.teff == 5770
     assert sme.wave is not None
 
     assert sme.nseg == 1
     assert sme.cscale_flag == "linear"
```

### Comparing `pysme-astro-0.4.99/test/test_solver.py` & `pysme-astro-5.74.9/test/test_solver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
+import pytest
 from os.path import dirname
 
 import numpy as np
-import pytest
 
-from pysme.sme import SME_Structure as SME_Struct
 from pysme.solve import solve
+from pysme.sme import SME_Structure as SME_Struct
 
 cwd = dirname(__file__)
-filename = "{}/testcase1.inp".format(cwd)
+filename = "{}/testcase1.inp".format((cwd))
 
 
 def test_simple():
     sme = SME_Struct.load(filename)
     sme2 = solve(sme, ["teff"])
 
     assert sme2.synth is not None
```

### Comparing `pysme-astro-0.4.99/test/test_synthesis.py` & `pysme-astro-5.74.9/test/test_synthesis.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-# -*- coding: utf-8 -*-
 # TODO implement synthesis tests
-import numpy as np
 import pytest
+import numpy as np
 
-from pysme.iliffe_vector import Iliffe_vector
 from pysme.synthesize import synthesize_spectrum
+from pysme.iliffe_vector import Iliffe_vector
 
 
 def test_synthesis_simple(sme_2segments):
     sme = sme_2segments
     sme2 = synthesize_spectrum(sme)
 
     # Check if a result is there it has the expected data type
```

### Comparing `pysme-astro-0.4.99/test/test_vald.py` & `pysme-astro-5.74.9/test/test_vald.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,43 @@
-# -*- coding: utf-8 -*-
 from os.path import dirname, join
-
 import numpy as np
 import pytest
 
-from pysme.abund import Abund
 from pysme.linelist.linelist import LineList
-from pysme.linelist.vald import ValdFile
+from pysme.linelist.vald import ValdFile, ValdError
+from pysme.abund import Abund
+
 
 species = "Fe 1"
 wlcent = 5502.9931
 excit = 0.9582
 gflog = -3.047
 gamrad = 7.19
 gamqst = -6.22
 gamvw = 239.249
 linedata = [species, wlcent, excit, gflog, gamrad, gamqst, gamvw]
 
 
 def test_line_init():
-    """Test that property values equal line data passed to __init__()."""
+    """Test that property values equal line data passed to __init__().
+    """
     line = LineList(linedata)
     assert isinstance(line, LineList)
     assert line.species[0] == species
     assert line.wlcent[0] == wlcent
     assert line.excit[0] == excit
     assert line.gflog[0] == gflog
     assert line.gamrad[0] == gamrad
     assert line.gamqst[0] == gamqst
     assert line.gamvw[0] == gamvw
 
 
 def test_linelist_add_and_len():
-    """Test that len() returns the number of lines (including 0) in list."""
+    """Test that len() returns the number of lines (including 0) in list.
+    """
     linelist = LineList()
     assert isinstance(linelist, LineList)
     assert len(linelist) == 0
     for iline in range(3):
         print(len(linelist._lines))
         print(linelist._lines)
         assert len(linelist) == iline
@@ -62,29 +63,31 @@
         print(linelist._lines)
         assert isinstance(prop, np.ndarray)
         assert len(prop) == 1
         assert prop[0] == linedata[iprop]
 
 
 def test_valdfile():
-    """Test class to read a VALD line data file."""
+    """Test class to read a VALD line data file.
+    """
     testdir = dirname(__file__)
     linelist = ValdFile(join(testdir, "testcase1.lin"))
 
     assert len(linelist) == 44
     assert linelist.lineformat == "short"
     assert linelist.medium == "air"
     assert linelist[0].species == "V 1"
 
     with pytest.raises(IOError):
-        ValdFile(join(testdir, "testcase1.npy"))
+        vf = ValdFile(join(testdir, "testcase1.npy"))
 
 
 def test_medium():
-    """Test class to read a VALD line data file."""
+    """Test class to read a VALD line data file.
+    """
     testdir = dirname(__file__)
     vf = ValdFile(join(testdir, "testcase1.lin"), medium="vac")
 
     assert vf.medium == "vac"
 
 
 def test_short_format():
```

### Comparing `pysme-astro-0.4.99/versioneer.py` & `pysme-astro-5.74.9/versioneer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Version: 0.18
 
 """The Versioneer - like a rocketeer, but for versions.
 
 The Versioneer
 ==============
 
@@ -411,30 +410,30 @@
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
-            print("unable to find command, tried {}".format(commands))
+            print("unable to find command, tried %s" % (commands,))
         return None, None
     stdout = p.communicate()[0].strip()
     if sys.version_info[0] >= 3:
         stdout = stdout.decode()
     if p.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
 LONG_VERSION_PY[
     "git"
-] = r'''
+] = '''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -997,28 +996,28 @@
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = {r.strip() for r in refnames.strip("()").split(",")}
+    refs = set([r.strip() for r in refnames.strip("()").split(",")])
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
+    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = {r for r in refs if re.search(r"\d", r)}
+        tags = set([r for r in refs if re.search(r"\d", r)])
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
@@ -1113,15 +1112,15 @@
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '{}' doesn't start with prefix '{}'".format(
+            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
                 full_tag,
                 tag_prefix,
             )
             return pieces
         pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
@@ -1236,37 +1235,33 @@
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
     except EnvironmentError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(
-        r"version_json = '''\n(.*)'''  # END VERSION_JSON",
-        contents,
-        re.M | re.S,
+        r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
     )
     if not mo:
         mo = re.search(
-            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON",
-            contents,
-            re.M | re.S,
+            r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
         )
     if not mo:
         raise NotThisMethod("no version_json in _version.py")
     return json.loads(mo.group(1))
 
 
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
-    print("set {} to '{}'".format(filename, versions["version"]))
+    print("set %s to '%s'" % (filename, versions["version"]))
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
@@ -1483,15 +1478,15 @@
             return ver
         except NotThisMethod:
             pass
 
     try:
         ver = versions_from_file(versionfile_abs)
         if verbose:
-            print("got version from file {} {}".format(versionfile_abs, ver))
+            print("got version from file %s %s" % (versionfile_abs, ver))
         return ver
     except NotThisMethod:
         pass
 
     from_vcs_f = handlers.get("pieces_from_vcs")
     if from_vcs_f:
         try:
```

