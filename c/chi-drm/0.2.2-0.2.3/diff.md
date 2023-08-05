# Comparing `tmp/chi-drm-0.2.2.tar.gz` & `tmp/chi-drm-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chi-drm-0.2.2.tar", last modified: Mon Dec 12 10:13:48 2022, max compression
+gzip compressed data, was "chi-drm-0.2.3.tar", last modified: Sat Aug  5 15:35:20 2023, max compression
```

## Comparing `chi-drm-0.2.2.tar` & `chi-drm-0.2.3.tar`

### file list

```diff
@@ -1,84 +1,46 @@
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.303083 chi-drm-0.2.2/
--rw-r--r--   0 david      (502) staff       (20)       64 2022-03-22 12:34:29.000000 chi-drm-0.2.2/.coveragerc
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.248771 chi-drm-0.2.2/.github/
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.258201 chi-drm-0.2.2/.github/workflows/
--rw-r--r--   0 david      (502) staff       (20)      617 2021-07-30 11:00:43.000000 chi-drm-0.2.2/.github/workflows/copyright-test.yml
--rw-r--r--   0 david      (502) staff       (20)      932 2021-07-30 11:00:43.000000 chi-drm-0.2.2/.github/workflows/coverage-test.yml
--rw-r--r--   0 david      (502) staff       (20)      776 2022-03-22 12:34:29.000000 chi-drm-0.2.2/.github/workflows/docs-test.yml
--rw-r--r--   0 david      (502) staff       (20)      650 2021-07-30 11:00:43.000000 chi-drm-0.2.2/.github/workflows/style-test.yml
--rw-r--r--   0 david      (502) staff       (20)     1040 2021-12-10 12:58:34.000000 chi-drm-0.2.2/.github/workflows/unit-test-os-versions.yml
--rw-r--r--   0 david      (502) staff       (20)      858 2021-12-10 12:58:34.000000 chi-drm-0.2.2/.github/workflows/unit-test-python-versions.yml
--rw-r--r--   0 david      (502) staff       (20)     1998 2022-01-06 11:19:29.000000 chi-drm-0.2.2/.gitignore
--rw-r--r--   0 david      (502) staff       (20)     1522 2022-01-06 11:19:29.000000 chi-drm-0.2.2/LICENSE.md
--rw-r--r--   0 david      (502) staff       (20)       98 2021-12-10 12:58:34.000000 chi-drm-0.2.2/MANIFEST.in
--rw-r--r--   0 david      (502) staff       (20)     3381 2022-12-12 10:13:48.302800 chi-drm-0.2.2/PKG-INFO
--rw-r--r--   0 david      (502) staff       (20)     2398 2022-04-03 13:41:32.000000 chi-drm-0.2.2/README.md
--rw-r--r--   0 david      (502) staff       (20)       16 2020-12-20 13:29:04.000000 chi-drm-0.2.2/apt.txt
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.266104 chi-drm-0.2.2/chi/
--rw-r--r--   0 david      (502) staff       (20)     1700 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/__init__.py
--rw-r--r--   0 david      (502) staff       (20)    13128 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/_covariate_models.py
--rw-r--r--   0 david      (502) staff       (20)    71339 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/_error_models.py
--rw-r--r--   0 david      (502) staff       (20)    30391 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/_inference.py
--rw-r--r--   0 david      (502) staff       (20)    80085 2022-12-12 10:10:17.000000 chi-drm-0.2.2/chi/_log_pdfs.py
--rw-r--r--   0 david      (502) staff       (20)    42891 2022-12-06 17:50:55.000000 chi-drm-0.2.2/chi/_mechanistic_models.py
--rw-r--r--   0 david      (502) staff       (20)    36107 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/_population_filters.py
--rw-r--r--   0 david      (502) staff       (20)   150485 2022-12-12 10:10:17.000000 chi-drm-0.2.2/chi/_population_models.py
--rw-r--r--   0 david      (502) staff       (20)    56002 2022-12-06 17:50:55.000000 chi-drm-0.2.2/chi/_predictive_models.py
--rw-r--r--   0 david      (502) staff       (20)    33370 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/_problems.py
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.268733 chi-drm-0.2.2/chi/library/
--rw-r--r--   0 david      (502) staff       (20)      332 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/library/__init__.py
--rw-r--r--   0 david      (502) staff       (20)     4897 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/library/_data_library_api.py
--rw-r--r--   0 david      (502) staff       (20)     5529 2022-03-22 12:34:29.000000 chi-drm-0.2.2/chi/library/_model_library_api.py
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.271650 chi-drm-0.2.2/chi/library/data_library/
--rw-r--r--   0 david      (502) staff       (20)     6836 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/library/data_library/lxf_control_growth.csv
--rw-r--r--   0 david      (502) staff       (20)    13662 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/library/data_library/lxf_high_erlotinib_dose.csv
--rw-r--r--   0 david      (502) staff       (20)    29264 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/library/data_library/lxf_low_erlotinib_dose.csv
--rw-r--r--   0 david      (502) staff       (20)    24931 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/library/data_library/lxf_medium_erlotinib_dose.csv
--rw-r--r--   0 david      (502) staff       (20)     3125 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/library/data_library/lxf_single_erlotinib_dose.csv
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.273610 chi-drm-0.2.2/chi/library/model_library/
--rw-r--r--   0 david      (502) staff       (20)     1749 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/library/model_library/pk_one_comp.xml
--rw-r--r--   0 david      (502) staff       (20)     3677 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/library/model_library/temporary_full_pkpd_model.xml
--rw-r--r--   0 david      (502) staff       (20)     3083 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/library/model_library/tgi_Koch_2009.xml
--rw-r--r--   0 david      (502) staff       (20)     2904 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/library/model_library/tgi_Koch_2009_reparametrised.xml
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.276264 chi-drm-0.2.2/chi/plots/
--rw-r--r--   0 david      (502) staff       (20)      633 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/plots/__init__.py
--rw-r--r--   0 david      (502) staff       (20)     6391 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/plots/_base.py
--rw-r--r--   0 david      (502) staff       (20)     5775 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/plots/_optimisation.py
--rw-r--r--   0 david      (502) staff       (20)    10702 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/plots/_residuals.py
--rw-r--r--   0 david      (502) staff       (20)     6710 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/plots/_sampling.py
--rw-r--r--   0 david      (502) staff       (20)    43633 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/plots/_time_series.py
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.289266 chi-drm-0.2.2/chi/tests/
--rw-r--r--   0 david      (502) staff       (20)    10875 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/tests/test_covariate_models.py
--rw-r--r--   0 david      (502) staff       (20)     7299 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/tests/test_data_library_api.py
--rw-r--r--   0 david      (502) staff       (20)    56910 2021-12-10 12:58:34.000000 chi-drm-0.2.2/chi/tests/test_error_models.py
--rw-r--r--   0 david      (502) staff       (20)    41208 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/tests/test_inference.py
--rw-r--r--   0 david      (502) staff       (20)   135618 2022-12-12 10:10:17.000000 chi-drm-0.2.2/chi/tests/test_log_pdfs.py
--rw-r--r--   0 david      (502) staff       (20)    36378 2022-03-22 12:34:29.000000 chi-drm-0.2.2/chi/tests/test_mechanistic_models.py
--rw-r--r--   0 david      (502) staff       (20)     6505 2022-03-22 12:34:29.000000 chi-drm-0.2.2/chi/tests/test_model_library_api.py
--rw-r--r--   0 david      (502) staff       (20)     5681 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/tests/test_plots_optimisation.py
--rw-r--r--   0 david      (502) staff       (20)     5798 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/tests/test_plots_residuals.py
--rw-r--r--   0 david      (502) staff       (20)     3919 2021-07-30 11:00:43.000000 chi-drm-0.2.2/chi/tests/test_plots_sampling.py
--rw-r--r--   0 david      (502) staff       (20)    28724 2022-01-06 11:19:29.000000 chi-drm-0.2.2/chi/tests/test_plots_time_series.py
--rw-r--r--   0 david      (502) staff       (20)   187649 2022-12-12 10:10:17.000000 chi-drm-0.2.2/chi/tests/test_population_models.py
--rw-r--r--   0 david      (502) staff       (20)    89629 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/tests/test_predictive_models.py
--rw-r--r--   0 david      (502) staff       (20)    49670 2022-09-21 10:17:12.000000 chi-drm-0.2.2/chi/tests/test_problems.py
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.291998 chi-drm-0.2.2/chi_drm.egg-info/
--rw-r--r--   0 david      (502) staff       (20)     3381 2022-12-12 10:13:48.000000 chi-drm-0.2.2/chi_drm.egg-info/PKG-INFO
--rw-r--r--   0 david      (502) staff       (20)     2047 2022-12-12 10:13:48.000000 chi-drm-0.2.2/chi_drm.egg-info/SOURCES.txt
--rw-r--r--   0 david      (502) staff       (20)        1 2022-12-12 10:13:48.000000 chi-drm-0.2.2/chi_drm.egg-info/dependency_links.txt
--rw-r--r--   0 david      (502) staff       (20)      162 2022-12-12 10:13:48.000000 chi-drm-0.2.2/chi_drm.egg-info/requires.txt
--rw-r--r--   0 david      (502) staff       (20)        4 2022-12-12 10:13:48.000000 chi-drm-0.2.2/chi_drm.egg-info/top_level.txt
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.293572 chi-drm-0.2.2/docs/
--rw-r--r--   0 david      (502) staff       (20)      605 2021-07-30 11:00:43.000000 chi-drm-0.2.2/docs/Makefile
--rw-r--r--   0 david      (502) staff       (20)      811 2021-07-30 11:00:43.000000 chi-drm-0.2.2/docs/make.bat
--rw-r--r--   0 david      (502) staff       (20)       47 2022-03-22 12:34:29.000000 chi-drm-0.2.2/docs/requirements.txt
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.296186 chi-drm-0.2.2/docs/source/
-drwxr-xr-x   0 david      (502) staff       (20)        0 2022-12-12 10:13:48.301426 chi-drm-0.2.2/docs/source/_static/
--rw-r--r--   0 david      (502) staff       (20)      108 2020-11-11 14:15:36.000000 chi-drm-0.2.2/docs/source/_static/custom.css
--rw-r--r--   0 david      (502) staff       (20)    11601 2021-07-30 10:54:20.000000 chi-drm-0.2.2/docs/source/_static/logo.png
--rw-r--r--   0 david      (502) staff       (20)   107595 2021-07-30 11:00:43.000000 chi-drm-0.2.2/docs/source/_static/logo_social_media.png
--rw-r--r--   0 david      (502) staff       (20)     5156 2022-09-21 10:17:12.000000 chi-drm-0.2.2/docs/source/conf.py
--rw-r--r--   0 david      (502) staff       (20)     1251 2022-03-22 12:34:29.000000 chi-drm-0.2.2/docs/source/index.rst
--rw-r--r--   0 david      (502) staff       (20)    11524 2022-03-22 12:34:29.000000 chi-drm-0.2.2/run-tests.py
--rw-r--r--   0 david      (502) staff       (20)       38 2022-12-12 10:13:48.303168 chi-drm-0.2.2/setup.cfg
--rw-r--r--   0 david      (502) staff       (20)     1156 2022-12-12 10:10:17.000000 chi-drm-0.2.2/setup.py
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.872946 chi-drm-0.2.3/
+-rw-r--r--   0 DAUGU      (502) staff       (20)     1522 2023-08-05 15:34:34.000000 chi-drm-0.2.3/LICENSE.md
+-rw-r--r--   0 DAUGU      (502) staff       (20)       98 2023-08-05 13:40:13.000000 chi-drm-0.2.3/MANIFEST.in
+-rw-r--r--   0 DAUGU      (502) staff       (20)     2751 2023-08-05 15:35:20.872694 chi-drm-0.2.3/PKG-INFO
+-rw-r--r--   0 DAUGU      (502) staff       (20)     2398 2023-08-05 13:40:13.000000 chi-drm-0.2.3/README.md
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.841624 chi-drm-0.2.3/chi/
+-rw-r--r--   0 DAUGU      (502) staff       (20)     1700 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/__init__.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    13128 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/_covariate_models.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    71335 2023-08-05 15:34:34.000000 chi-drm-0.2.3/chi/_error_models.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    30391 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/_inference.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    80121 2023-08-05 15:34:34.000000 chi-drm-0.2.3/chi/_log_pdfs.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    42887 2023-08-05 15:34:34.000000 chi-drm-0.2.3/chi/_mechanistic_models.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    36107 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/_population_filters.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)   150481 2023-08-05 15:34:34.000000 chi-drm-0.2.3/chi/_population_models.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    56002 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/_predictive_models.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    33370 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/_problems.py
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.843158 chi-drm-0.2.3/chi/library/
+-rw-r--r--   0 DAUGU      (502) staff       (20)      332 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/__init__.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)     4897 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/_data_library_api.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)     5529 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/_model_library_api.py
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.845922 chi-drm-0.2.3/chi/library/data_library/
+-rw-r--r--   0 DAUGU      (502) staff       (20)     6836 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/data_library/lxf_control_growth.csv
+-rw-r--r--   0 DAUGU      (502) staff       (20)    13662 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/data_library/lxf_high_erlotinib_dose.csv
+-rw-r--r--   0 DAUGU      (502) staff       (20)    29264 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/data_library/lxf_low_erlotinib_dose.csv
+-rw-r--r--   0 DAUGU      (502) staff       (20)    24931 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/data_library/lxf_medium_erlotinib_dose.csv
+-rw-r--r--   0 DAUGU      (502) staff       (20)     3125 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/data_library/lxf_single_erlotinib_dose.csv
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.847870 chi-drm-0.2.3/chi/library/model_library/
+-rw-r--r--   0 DAUGU      (502) staff       (20)     1749 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/model_library/pk_one_comp.xml
+-rw-r--r--   0 DAUGU      (502) staff       (20)     3677 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/model_library/temporary_full_pkpd_model.xml
+-rw-r--r--   0 DAUGU      (502) staff       (20)     3083 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/model_library/tgi_Koch_2009.xml
+-rw-r--r--   0 DAUGU      (502) staff       (20)     2904 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/library/model_library/tgi_Koch_2009_reparametrised.xml
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.865389 chi-drm-0.2.3/chi/plots/
+-rw-r--r--   0 DAUGU      (502) staff       (20)      633 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/plots/__init__.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)     6391 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/plots/_base.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)     5775 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/plots/_optimisation.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    10702 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/plots/_residuals.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)     6710 2023-08-05 13:40:13.000000 chi-drm-0.2.3/chi/plots/_sampling.py
+-rw-r--r--   0 DAUGU      (502) staff       (20)    43645 2023-08-05 15:34:34.000000 chi-drm-0.2.3/chi/plots/_time_series.py
+drwxr-xr-x   0 DAUGU      (502) staff       (20)        0 2023-08-05 15:35:20.872213 chi-drm-0.2.3/chi_drm.egg-info/
+-rw-r--r--   0 DAUGU      (502) staff       (20)     2751 2023-08-05 15:35:20.000000 chi-drm-0.2.3/chi_drm.egg-info/PKG-INFO
+-rw-r--r--   0 DAUGU      (502) staff       (20)     1111 2023-08-05 15:35:20.000000 chi-drm-0.2.3/chi_drm.egg-info/SOURCES.txt
+-rw-r--r--   0 DAUGU      (502) staff       (20)        1 2023-08-05 15:35:20.000000 chi-drm-0.2.3/chi_drm.egg-info/dependency_links.txt
+-rw-r--r--   0 DAUGU      (502) staff       (20)      162 2023-08-05 15:35:20.000000 chi-drm-0.2.3/chi_drm.egg-info/requires.txt
+-rw-r--r--   0 DAUGU      (502) staff       (20)        4 2023-08-05 15:35:20.000000 chi-drm-0.2.3/chi_drm.egg-info/top_level.txt
+-rw-r--r--   0 DAUGU      (502) staff       (20)       38 2023-08-05 15:35:20.873014 chi-drm-0.2.3/setup.cfg
+-rw-r--r--   0 DAUGU      (502) staff       (20)     1156 2023-08-05 15:34:34.000000 chi-drm-0.2.3/setup.py
```

### Comparing `chi-drm-0.2.2/LICENSE.md` & `chi-drm-0.2.3/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, David Augustin
+Copyright (c) 2023, David Augustin
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `chi-drm-0.2.2/PKG-INFO` & `chi-drm-0.2.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 Metadata-Version: 2.1
 Name: chi-drm
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package to model dose response dynamics
 Home-page: https://chi.readthedocs.io
 Maintainer: David Augustin
 Maintainer-email: david.augustin@cs.ox.ac.uk
 License: BSD 3-clause license
-Description: # Chi
-        
-        [![Unit tests on multiple python versions](https://github.com/DavAug/chi/workflows/Unit%20tests%20(python%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
-        [![Unit tests on multiple operating systems](https://github.com/DavAug/chi/workflows/Unit%20tests%20(OS%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
-        [![codecov](https://codecov.io/gh/DavAug/chi/branch/main/graph/badge.svg)](https://codecov.io/gh/DavAug/chi)
-        [![Documentation Status](https://readthedocs.org/projects/chi/badge/?version=latest)](https://chi.readthedocs.io/en/latest/?badge=latest)
-        
-        ## About
-        
-        **Chi** is an open source Python package hosted on GitHub,
-        which can be used to model dose response dynamics.
-        
-        All features of the software are described in detail in the
-        [full API documentation](https://chi.readthedocs.io/en/latest/).
-        
-        ## Getting started
-        ### Installation
-        
-        1. Install sundials
-        
-        Chi uses the open source package Myokit to solve ordinary differential equations
-        and compute their sensitivities efficiently. Myokit does this using sundials' CVODESS,
-        which needs to be installed with:
-        
-        - On Ubuntu:
-        ```bash
-        apt-get install libsundials-dev
-        ```
-        
-        - On MacOS:
-        ```bash
-        brew install sundials
-        ```
-        
-        - On Windows: No action required. Myokit will install sundial automatically.
-        
-        2. Install chi
-        ```bash
-        pip install chi-drm
-        ```
-        
-         You can now use chi's functionality by importing it
-         ```python
-        import chi
-         ```
-         
-         ### Tutorials
-        
-         Tutorials and more detailed explanations on how to use chi can be found in the [documentation's getting started](https://chi.readthedocs.io/en/latest/getting_started/index.html) section.
-         
-        ## Citation
-        
-        If you use this software in your work, please cite it using the following metadata:
-        
-        #### APA
-        ```
-        Augustin, D. (2021). Chi - An open source python package for treatment response modelling (Version 0.1.0) [Computer software]. https://github.com/DavAug/chi
-        ```
-        
-        #### BibTeX
-        ```
-        @software{Augustin_Chi_-_An_2021,
-        author = {Augustin, David},
-        month = {12},
-        title = {{Chi - An open source python package for treatment response modelling}},
-        url = {https://github.com/DavAug/chi},
-        version = {0.1.0},
-        year = {2021}
-        }
-        ```
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        Please make sure to update tests as appropriate.
-        
-        ## License
-        [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: notebooks
+License-File: LICENSE.md
+
+# Chi
+
+[![Unit tests on multiple python versions](https://github.com/DavAug/chi/workflows/Unit%20tests%20(python%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
+[![Unit tests on multiple operating systems](https://github.com/DavAug/chi/workflows/Unit%20tests%20(OS%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
+[![codecov](https://codecov.io/gh/DavAug/chi/branch/main/graph/badge.svg)](https://codecov.io/gh/DavAug/chi)
+[![Documentation Status](https://readthedocs.org/projects/chi/badge/?version=latest)](https://chi.readthedocs.io/en/latest/?badge=latest)
+
+## About
+
+**Chi** is an open source Python package hosted on GitHub,
+which can be used to model dose response dynamics.
+
+All features of the software are described in detail in the
+[full API documentation](https://chi.readthedocs.io/en/latest/).
+
+## Getting started
+### Installation
+
+1. Install sundials
+
+Chi uses the open source package Myokit to solve ordinary differential equations
+and compute their sensitivities efficiently. Myokit does this using sundials' CVODESS,
+which needs to be installed with:
+
+- On Ubuntu:
+```bash
+apt-get install libsundials-dev
+```
+
+- On MacOS:
+```bash
+brew install sundials
+```
+
+- On Windows: No action required. Myokit will install sundial automatically.
+
+2. Install chi
+```bash
+pip install chi-drm
+```
+
+ You can now use chi's functionality by importing it
+ ```python
+import chi
+ ```
+ 
+ ### Tutorials
+
+ Tutorials and more detailed explanations on how to use chi can be found in the [documentation's getting started](https://chi.readthedocs.io/en/latest/getting_started/index.html) section.
+ 
+## Citation
+
+If you use this software in your work, please cite it using the following metadata:
+
+#### APA
+```
+Augustin, D. (2021). Chi - An open source python package for treatment response modelling (Version 0.1.0) [Computer software]. https://github.com/DavAug/chi
+```
+
+#### BibTeX
+```
+@software{Augustin_Chi_-_An_2021,
+author = {Augustin, David},
+month = {12},
+title = {{Chi - An open source python package for treatment response modelling}},
+url = {https://github.com/DavAug/chi},
+version = {0.1.0},
+year = {2021}
+}
+```
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+[BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)
```

### Comparing `chi-drm-0.2.2/README.md` & `chi-drm-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/__init__.py` & `chi-drm-0.2.3/chi/__init__.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/_covariate_models.py` & `chi-drm-0.2.3/chi/_covariate_models.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/_error_models.py` & `chi-drm-0.2.3/chi/_error_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1787,15 +1787,15 @@
                 continue
 
             # Fix parameter if value is not None, else unfix it
             self._fixed_params_mask[index] = value is not None
             self._fixed_params_values[index] = value
 
         # If all parameters are free, set mask and values to None again
-        if np.alltrue(~self._fixed_params_mask):
+        if np.all(~self._fixed_params_mask):
             self._fixed_params_mask = None
             self._fixed_params_values = None
 
     def get_error_model(self):
         """
         Returns the original error model.
         """
```

### Comparing `chi-drm-0.2.2/chi/_inference.py` & `chi-drm-0.2.3/chi/_inference.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/_log_pdfs.py` & `chi-drm-0.2.3/chi/_log_pdfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -126,16 +126,16 @@
             )
 
         # Compute population model score
         score = self._population_model.compute_log_likelihood(
             top_parameters, bottom_parameters, covariates=self._covariates)
 
         # Return if values already lead to a rejection
-        if np.isinf(score):
-            return score
+        if np.isinf(score):  # noqa: no cover
+            return score  # noqa: no cover
 
         # Transform bottom-level parameters
         # Identity, if model does not tranform parameters
         bottom_parameters = \
             self._population_model.compute_individual_parameters(
                 top_parameters, bottom_parameters, self._covariates)
```

### Comparing `chi-drm-0.2.2/chi/_mechanistic_models.py` & `chi-drm-0.2.3/chi/_mechanistic_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -982,15 +982,15 @@
                 continue
 
             # Fix parameter if value is not None, else unfix it
             self._fixed_params_mask[index] = value is not None
             self._fixed_params_values[index] = value
 
         # If all parameters are free, set mask and values to None again
-        if np.alltrue(~self._fixed_params_mask):
+        if np.all(~self._fixed_params_mask):
             self._fixed_params_mask = None
             self._fixed_params_values = None
 
         # Remove sensitivities for fixed parameters
         if self.has_sensitivities() is True:
             self.enable_sensitivities(True)
```

### Comparing `chi-drm-0.2.2/chi/_population_filters.py` & `chi-drm-0.2.3/chi/_population_filters.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/_population_models.py` & `chi-drm-0.2.3/chi/_population_models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3270,15 +3270,15 @@
                 continue
 
             # Fix parameter if value is not None, else unfix it
             self._fixed_params_mask[index] = value is not None
             self._fixed_params_values[index] = value
 
         # If all parameters are free, set mask and values to None again
-        if np.alltrue(~self._fixed_params_mask):
+        if np.all(~self._fixed_params_mask):
             self._fixed_params_mask = None
             self._fixed_params_values = None
 
     def get_covariate_names(self):
         """
         Returns the names of the covariates. If name is
         not set, defaults are returned.
```

### Comparing `chi-drm-0.2.2/chi/_predictive_models.py` & `chi-drm-0.2.3/chi/_predictive_models.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/_problems.py` & `chi-drm-0.2.3/chi/_problems.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/_data_library_api.py` & `chi-drm-0.2.3/chi/library/_data_library_api.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/_model_library_api.py` & `chi-drm-0.2.3/chi/library/_model_library_api.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/data_library/lxf_control_growth.csv` & `chi-drm-0.2.3/chi/library/data_library/lxf_control_growth.csv`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/data_library/lxf_high_erlotinib_dose.csv` & `chi-drm-0.2.3/chi/library/data_library/lxf_high_erlotinib_dose.csv`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/data_library/lxf_low_erlotinib_dose.csv` & `chi-drm-0.2.3/chi/library/data_library/lxf_low_erlotinib_dose.csv`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/data_library/lxf_medium_erlotinib_dose.csv` & `chi-drm-0.2.3/chi/library/data_library/lxf_medium_erlotinib_dose.csv`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/data_library/lxf_single_erlotinib_dose.csv` & `chi-drm-0.2.3/chi/library/data_library/lxf_single_erlotinib_dose.csv`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/model_library/pk_one_comp.xml` & `chi-drm-0.2.3/chi/library/model_library/pk_one_comp.xml`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/model_library/temporary_full_pkpd_model.xml` & `chi-drm-0.2.3/chi/library/model_library/temporary_full_pkpd_model.xml`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/model_library/tgi_Koch_2009.xml` & `chi-drm-0.2.3/chi/library/model_library/tgi_Koch_2009.xml`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/library/model_library/tgi_Koch_2009_reparametrised.xml` & `chi-drm-0.2.3/chi/library/model_library/tgi_Koch_2009_reparametrised.xml`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/plots/__init__.py` & `chi-drm-0.2.3/chi/plots/__init__.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/plots/_base.py` & `chi-drm-0.2.3/chi/plots/_base.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/plots/_optimisation.py` & `chi-drm-0.2.3/chi/plots/_optimisation.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/plots/_residuals.py` & `chi-drm-0.2.3/chi/plots/_residuals.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/plots/_sampling.py` & `chi-drm-0.2.3/chi/plots/_sampling.py`

 * *Files identical despite different names*

### Comparing `chi-drm-0.2.2/chi/plots/_time_series.py` & `chi-drm-0.2.3/chi/plots/_time_series.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,19 +145,19 @@
                 mask = percentile_df <= lower
                 biom_lower = reduced_data[mask][sample_key].max()
 
                 mask = percentile_df >= upper
                 biom_upper = reduced_data[mask][sample_key].min()
 
                 # Append percentiles to container
-                container = container.append(pd.DataFrame({
+                container = pd.concat([container, pd.DataFrame({
                     'Time': [time],
                     'Lower': [biom_lower],
                     'Upper': [biom_upper],
-                    'Bulk probability': [str(bulk_prob)]}))
+                    'Bulk probability': [str(bulk_prob)]})])
 
         return container
 
     def add_data(
             self, data, observable=None, id_key='ID', time_key='Time',
             obs_key='Observable', value_key='Value'):
         """
@@ -534,19 +534,19 @@
                 mask = percentile_df <= lower
                 biom_lower = reduced_data[mask][sample_key].max()
 
                 mask = percentile_df >= upper
                 biom_upper = reduced_data[mask][sample_key].min()
 
                 # Append percentiles to container
-                container = container.append(pd.DataFrame({
+                container = pd.concat([container, pd.DataFrame({
                     'Time': [time],
                     'Lower': [biom_lower],
                     'Upper': [biom_upper],
-                    'Bulk probability': [str(bulk_prob)]}))
+                    'Bulk probability': [str(bulk_prob)]})])
 
         return container
 
     def add_data(
             self, data, observable=None, id_key='ID', time_key='Time',
             obs_key='Observable', value_key='Value', dose_key='Dose',
             dose_duration_key='Duration'):
```

### Comparing `chi-drm-0.2.2/chi_drm.egg-info/PKG-INFO` & `chi-drm-0.2.3/chi_drm.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,91 +1,91 @@
 Metadata-Version: 2.1
 Name: chi-drm
-Version: 0.2.2
+Version: 0.2.3
 Summary: Package to model dose response dynamics
 Home-page: https://chi.readthedocs.io
 Maintainer: David Augustin
 Maintainer-email: david.augustin@cs.ox.ac.uk
 License: BSD 3-clause license
-Description: # Chi
-        
-        [![Unit tests on multiple python versions](https://github.com/DavAug/chi/workflows/Unit%20tests%20(python%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
-        [![Unit tests on multiple operating systems](https://github.com/DavAug/chi/workflows/Unit%20tests%20(OS%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
-        [![codecov](https://codecov.io/gh/DavAug/chi/branch/main/graph/badge.svg)](https://codecov.io/gh/DavAug/chi)
-        [![Documentation Status](https://readthedocs.org/projects/chi/badge/?version=latest)](https://chi.readthedocs.io/en/latest/?badge=latest)
-        
-        ## About
-        
-        **Chi** is an open source Python package hosted on GitHub,
-        which can be used to model dose response dynamics.
-        
-        All features of the software are described in detail in the
-        [full API documentation](https://chi.readthedocs.io/en/latest/).
-        
-        ## Getting started
-        ### Installation
-        
-        1. Install sundials
-        
-        Chi uses the open source package Myokit to solve ordinary differential equations
-        and compute their sensitivities efficiently. Myokit does this using sundials' CVODESS,
-        which needs to be installed with:
-        
-        - On Ubuntu:
-        ```bash
-        apt-get install libsundials-dev
-        ```
-        
-        - On MacOS:
-        ```bash
-        brew install sundials
-        ```
-        
-        - On Windows: No action required. Myokit will install sundial automatically.
-        
-        2. Install chi
-        ```bash
-        pip install chi-drm
-        ```
-        
-         You can now use chi's functionality by importing it
-         ```python
-        import chi
-         ```
-         
-         ### Tutorials
-        
-         Tutorials and more detailed explanations on how to use chi can be found in the [documentation's getting started](https://chi.readthedocs.io/en/latest/getting_started/index.html) section.
-         
-        ## Citation
-        
-        If you use this software in your work, please cite it using the following metadata:
-        
-        #### APA
-        ```
-        Augustin, D. (2021). Chi - An open source python package for treatment response modelling (Version 0.1.0) [Computer software]. https://github.com/DavAug/chi
-        ```
-        
-        #### BibTeX
-        ```
-        @software{Augustin_Chi_-_An_2021,
-        author = {Augustin, David},
-        month = {12},
-        title = {{Chi - An open source python package for treatment response modelling}},
-        url = {https://github.com/DavAug/chi},
-        version = {0.1.0},
-        year = {2021}
-        }
-        ```
-        
-        ## Contributing
-        Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
-        
-        Please make sure to update tests as appropriate.
-        
-        ## License
-        [BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)
-        
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: notebooks
+License-File: LICENSE.md
+
+# Chi
+
+[![Unit tests on multiple python versions](https://github.com/DavAug/chi/workflows/Unit%20tests%20(python%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
+[![Unit tests on multiple operating systems](https://github.com/DavAug/chi/workflows/Unit%20tests%20(OS%20versions)/badge.svg)](https://github.com/DavAug/chi/actions)
+[![codecov](https://codecov.io/gh/DavAug/chi/branch/main/graph/badge.svg)](https://codecov.io/gh/DavAug/chi)
+[![Documentation Status](https://readthedocs.org/projects/chi/badge/?version=latest)](https://chi.readthedocs.io/en/latest/?badge=latest)
+
+## About
+
+**Chi** is an open source Python package hosted on GitHub,
+which can be used to model dose response dynamics.
+
+All features of the software are described in detail in the
+[full API documentation](https://chi.readthedocs.io/en/latest/).
+
+## Getting started
+### Installation
+
+1. Install sundials
+
+Chi uses the open source package Myokit to solve ordinary differential equations
+and compute their sensitivities efficiently. Myokit does this using sundials' CVODESS,
+which needs to be installed with:
+
+- On Ubuntu:
+```bash
+apt-get install libsundials-dev
+```
+
+- On MacOS:
+```bash
+brew install sundials
+```
+
+- On Windows: No action required. Myokit will install sundial automatically.
+
+2. Install chi
+```bash
+pip install chi-drm
+```
+
+ You can now use chi's functionality by importing it
+ ```python
+import chi
+ ```
+ 
+ ### Tutorials
+
+ Tutorials and more detailed explanations on how to use chi can be found in the [documentation's getting started](https://chi.readthedocs.io/en/latest/getting_started/index.html) section.
+ 
+## Citation
+
+If you use this software in your work, please cite it using the following metadata:
+
+#### APA
+```
+Augustin, D. (2021). Chi - An open source python package for treatment response modelling (Version 0.1.0) [Computer software]. https://github.com/DavAug/chi
+```
+
+#### BibTeX
+```
+@software{Augustin_Chi_-_An_2021,
+author = {Augustin, David},
+month = {12},
+title = {{Chi - An open source python package for treatment response modelling}},
+url = {https://github.com/DavAug/chi},
+version = {0.1.0},
+year = {2021}
+}
+```
+
+## Contributing
+Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
+
+Please make sure to update tests as appropriate.
+
+## License
+[BSD-3-Clause](https://opensource.org/licenses/BSD-3-Clause)
```

### Comparing `chi-drm-0.2.2/chi_drm.egg-info/SOURCES.txt` & `chi-drm-0.2.3/chi_drm.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,11 @@
-.coveragerc
-.gitignore
 LICENSE.md
 MANIFEST.in
 README.md
-apt.txt
-run-tests.py
 setup.py
-.github/workflows/copyright-test.yml
-.github/workflows/coverage-test.yml
-.github/workflows/docs-test.yml
-.github/workflows/style-test.yml
-.github/workflows/unit-test-os-versions.yml
-.github/workflows/unit-test-python-versions.yml
 chi/__init__.py
 chi/_covariate_models.py
 chi/_error_models.py
 chi/_inference.py
 chi/_log_pdfs.py
 chi/_mechanistic_models.py
 chi/_population_filters.py
@@ -36,34 +26,12 @@
 chi/library/model_library/tgi_Koch_2009_reparametrised.xml
 chi/plots/__init__.py
 chi/plots/_base.py
 chi/plots/_optimisation.py
 chi/plots/_residuals.py
 chi/plots/_sampling.py
 chi/plots/_time_series.py
-chi/tests/test_covariate_models.py
-chi/tests/test_data_library_api.py
-chi/tests/test_error_models.py
-chi/tests/test_inference.py
-chi/tests/test_log_pdfs.py
-chi/tests/test_mechanistic_models.py
-chi/tests/test_model_library_api.py
-chi/tests/test_plots_optimisation.py
-chi/tests/test_plots_residuals.py
-chi/tests/test_plots_sampling.py
-chi/tests/test_plots_time_series.py
-chi/tests/test_population_models.py
-chi/tests/test_predictive_models.py
-chi/tests/test_problems.py
 chi_drm.egg-info/PKG-INFO
 chi_drm.egg-info/SOURCES.txt
 chi_drm.egg-info/dependency_links.txt
 chi_drm.egg-info/requires.txt
-chi_drm.egg-info/top_level.txt
-docs/Makefile
-docs/make.bat
-docs/requirements.txt
-docs/source/conf.py
-docs/source/index.rst
-docs/source/_static/custom.css
-docs/source/_static/logo.png
-docs/source/_static/logo_social_media.png
+chi_drm.egg-info/top_level.txt
```

### Comparing `chi-drm-0.2.2/setup.py` & `chi-drm-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = f.read()
 
 
 # Go!
 setup(
     # Module name
     name='chi-drm',
-    version='0.2.2',
+    version='0.2.3',
     description='Package to model dose response dynamics',
     long_description=readme,
     long_description_content_type="text/markdown",
     url="https://chi.readthedocs.io",
 
     # License name
     license='BSD 3-clause license',
@@ -27,15 +27,15 @@
         include=('chi', 'chi.*'),
         exclude=('chi/tests',)),
     include_package_data=True,
 
     # List of dependencies
     install_requires=[
         'arviz>=0.11',
-        'myokit>=1.33',
+        'myokit>=1.34',
         'numpy>=1.17',
         'pandas>=0.24',
         'pints>=0.4',
         'plotly>=4.8.1',
         'tqdm>=4.46.1',
         'xarray>=0.19'
     ],
```

