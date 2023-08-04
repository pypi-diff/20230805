# Comparing `tmp/spec_plots-1.35.0.tar.gz` & `tmp/spec_plots-1.35.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spec_plots-1.35.0.tar", last modified: Mon Jul 31 17:43:58 2023, max compression
+gzip compressed data, was "spec_plots-1.35.1.tar", last modified: Fri Aug  4 21:55:43 2023, max compression
```

## Comparing `spec_plots-1.35.0.tar` & `spec_plots-1.35.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.949343 spec_plots-1.35.0/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      285 2023-07-31 17:43:58.949172 spec_plots-1.35.0/PKG-INFO
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      362 2023-07-31 15:04:45.000000 spec_plots-1.35.0/README.md
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       38 2023-07-31 17:43:58.949400 spec_plots-1.35.0/setup.cfg
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1175 2023-07-31 16:18:05.000000 spec_plots-1.35.0/setup.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.941427 spec_plots-1.35.0/spec_plots/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      231 2023-07-31 15:05:19.000000 spec_plots-1.35.0/spec_plots/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1613 2018-03-16 03:24:26.000000 spec_plots-1.35.0/spec_plots/__main__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1648 2018-03-16 03:24:26.000000 spec_plots-1.35.0/spec_plots/__main_jwst__.py
--rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    20169 2020-04-05 18:34:12.000000 spec_plots-1.35.0/spec_plots/make_hst_spec_previews.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    16259 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/make_html.py
--rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    14959 2018-03-19 16:55:13.000000 spec_plots-1.35.0/spec_plots/make_jwst_spec_previews.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.943238 spec_plots-1.35.0/spec_plots/utils/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      180 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/__init__.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.945834 spec_plots-1.35.0/spec_plots/utils/specutils/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1336 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2333 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/avoidregion.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4601 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils/calc_covering_fraction.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3797 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/calc_plot_metrics.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4890 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/debug_oplot.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1957 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/dq_has_flag.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    15392 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/edge_trim.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1693 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/get_flux_stats.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1880 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils/is_bad_dq.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1035 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/rms.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4836 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_xrange.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4587 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_yrange.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1253 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils/specutilserror.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7916 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils/stitch_components.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.947299 spec_plots-1.35.0/spec_plots/utils/specutils_cos/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      837 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3125 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/check_segments.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7256 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/cosspectrum.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3579 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/extract_subspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1204 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/get_segment_names.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     5388 2018-01-24 21:18:54.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/make_fits.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17530 2023-07-31 16:00:45.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/plotspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    12465 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_cos/readspec.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.948009 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      483 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1491 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/jwstspectrum.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    13340 2023-07-31 16:09:30.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/plotspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2523 2016-11-28 23:11:25.000000 spec_plots-1.35.0/spec_plots/utils/specutils_jwst/readspec.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.948924 spec_plots-1.35.0/spec_plots/utils/specutils_stis/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      685 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/__init__.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1201 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/get_association_indices.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17349 2023-07-31 15:57:11.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/plotspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2302 2016-11-28 23:02:15.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/readspec.py
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4897 2016-09-30 20:32:23.000000 spec_plots-1.35.0/spec_plots/utils/specutils_stis/stis1dspectrum.py
-drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-07-31 17:43:58.943037 spec_plots-1.35.0/spec_plots.egg-info/
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      285 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/PKG-INFO
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1860 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/SOURCES.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/dependency_links.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      124 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/entry_points.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2014-12-12 18:16:09.000000 spec_plots-1.35.0/spec_plots.egg-info/not-zip-safe
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       62 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/requires.txt
--rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       11 2023-07-31 17:43:58.000000 spec_plots-1.35.0/spec_plots.egg-info/top_level.txt
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.781545 spec_plots-1.35.1/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      283 2023-08-04 21:55:43.781421 spec_plots-1.35.1/PKG-INFO
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      362 2023-07-31 15:04:45.000000 spec_plots-1.35.1/README.md
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       38 2023-08-04 21:55:43.781595 spec_plots-1.35.1/setup.cfg
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1173 2023-08-04 21:53:57.000000 spec_plots-1.35.1/setup.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.774912 spec_plots-1.35.1/spec_plots/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      231 2023-08-04 19:21:09.000000 spec_plots-1.35.1/spec_plots/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1613 2018-03-16 03:24:26.000000 spec_plots-1.35.1/spec_plots/__main__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1648 2018-03-16 03:24:26.000000 spec_plots-1.35.1/spec_plots/__main_jwst__.py
+-rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    20169 2020-04-05 18:34:12.000000 spec_plots-1.35.1/spec_plots/make_hst_spec_previews.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    16259 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/make_html.py
+-rwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)    14959 2018-03-19 16:55:13.000000 spec_plots-1.35.1/spec_plots/make_jwst_spec_previews.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.776064 spec_plots-1.35.1/spec_plots/utils/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      180 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/__init__.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.778391 spec_plots-1.35.1/spec_plots/utils/specutils/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1336 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2333 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/avoidregion.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4601 2018-01-24 21:18:54.000000 spec_plots-1.35.1/spec_plots/utils/specutils/calc_covering_fraction.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3797 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/calc_plot_metrics.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4890 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/debug_oplot.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1957 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/dq_has_flag.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    15392 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/edge_trim.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1693 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/get_flux_stats.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1880 2016-11-28 23:11:25.000000 spec_plots-1.35.1/spec_plots/utils/specutils/is_bad_dq.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1035 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/rms.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4836 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/set_plot_xrange.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4587 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/set_plot_yrange.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1253 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils/specutilserror.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7916 2018-01-24 21:18:54.000000 spec_plots-1.35.1/spec_plots/utils/specutils/stitch_components.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.779749 spec_plots-1.35.1/spec_plots/utils/specutils_cos/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      837 2018-01-24 21:18:54.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3125 2016-11-28 23:11:25.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/check_segments.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     7256 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/cosspectrum.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     3579 2016-11-28 23:11:25.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/extract_subspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1204 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/get_segment_names.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     5388 2018-01-24 21:18:54.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/make_fits.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17530 2023-07-31 16:00:45.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/plotspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    12465 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils_cos/readspec.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.780408 spec_plots-1.35.1/spec_plots/utils/specutils_jwst/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      483 2016-11-28 23:11:25.000000 spec_plots-1.35.1/spec_plots/utils/specutils_jwst/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1491 2016-11-28 23:11:25.000000 spec_plots-1.35.1/spec_plots/utils/specutils_jwst/jwstspectrum.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    13538 2023-08-04 21:36:36.000000 spec_plots-1.35.1/spec_plots/utils/specutils_jwst/plotspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2700 2023-08-04 20:03:14.000000 spec_plots-1.35.1/spec_plots/utils/specutils_jwst/readspec.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.781239 spec_plots-1.35.1/spec_plots/utils/specutils_stis/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      685 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils_stis/__init__.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1201 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils_stis/get_association_indices.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)    17349 2023-07-31 15:57:11.000000 spec_plots-1.35.1/spec_plots/utils/specutils_stis/plotspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     2302 2016-11-28 23:02:15.000000 spec_plots-1.35.1/spec_plots/utils/specutils_stis/readspec.py
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     4897 2016-09-30 20:32:23.000000 spec_plots-1.35.1/spec_plots/utils/specutils_stis/stis1dspectrum.py
+drwxr-xr-x   0 fleming   (4340) STSCI\science  (1031)        0 2023-08-04 21:55:43.775917 spec_plots-1.35.1/spec_plots.egg-info/
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      283 2023-08-04 21:55:43.000000 spec_plots-1.35.1/spec_plots.egg-info/PKG-INFO
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)     1860 2023-08-04 21:55:43.000000 spec_plots-1.35.1/spec_plots.egg-info/SOURCES.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2023-08-04 21:55:43.000000 spec_plots-1.35.1/spec_plots.egg-info/dependency_links.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)      124 2023-08-04 21:55:43.000000 spec_plots-1.35.1/spec_plots.egg-info/entry_points.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)        1 2014-12-12 18:16:09.000000 spec_plots-1.35.1/spec_plots.egg-info/not-zip-safe
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       62 2023-08-04 21:55:43.000000 spec_plots-1.35.1/spec_plots.egg-info/requires.txt
+-rw-r--r--   0 fleming   (4340) STSCI\science  (1031)       11 2023-08-04 21:55:43.000000 spec_plots-1.35.1/spec_plots.egg-info/top_level.txt
```

### Comparing `spec_plots-1.35.0/setup.py` & `spec_plots-1.35.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from __future__ import absolute_import
 from setuptools import setup
 from spec_plots import __version__
 
 setup(name="spec_plots",
       version=__version__,
       description="Create preview plots of HST or JWST spectra.",
-      classifiers=["Programming Language :: Python :: 3.9"],
+      classifiers=["Programming Language :: Python :: 3"],
       url="https://github.com/spacetelescope/spec_plots",
       author="Scott W. Fleming",
       author_email="fleming@stsci.edu",
       license="MIT",
       packages=["spec_plots", "spec_plots.utils", "spec_plots.utils.specutils",
                 "spec_plots.utils.specutils_cos",
                 "spec_plots.utils.specutils_jwst",
```

### Comparing `spec_plots-1.35.0/spec_plots/__main__.py` & `spec_plots-1.35.1/spec_plots/__main__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/__main_jwst__.py` & `spec_plots-1.35.1/spec_plots/__main_jwst__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/make_hst_spec_previews.py` & `spec_plots-1.35.1/spec_plots/make_hst_spec_previews.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/make_html.py` & `spec_plots-1.35.1/spec_plots/make_html.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/make_jwst_spec_previews.py` & `spec_plots-1.35.1/spec_plots/make_jwst_spec_previews.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/__init__.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/__init__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/avoidregion.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/avoidregion.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/calc_covering_fraction.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/calc_covering_fraction.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/calc_plot_metrics.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/calc_plot_metrics.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/debug_oplot.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/debug_oplot.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/dq_has_flag.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/dq_has_flag.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/edge_trim.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/edge_trim.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/get_flux_stats.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/get_flux_stats.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/is_bad_dq.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/is_bad_dq.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/rms.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/rms.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_xrange.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/set_plot_xrange.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/set_plot_yrange.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/set_plot_yrange.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/specutilserror.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/specutilserror.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils/stitch_components.py` & `spec_plots-1.35.1/spec_plots/utils/specutils/stitch_components.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/__init__.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/__init__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/check_segments.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/check_segments.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/cosspectrum.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/cosspectrum.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/extract_subspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/extract_subspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/get_segment_names.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/get_segment_names.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/make_fits.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/make_fits.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/plotspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/plotspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_cos/readspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_cos/readspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_jwst/jwstspectrum.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_jwst/jwstspectrum.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_jwst/plotspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_jwst/plotspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -233,15 +233,16 @@
         max_wl = numpy.nanmax(all_wls)
         xplot_buffer = (max_wl - min_wl) * 0.05
         this_plotarea.set_xlim([min_wl-xplot_buffer, max_wl+xplot_buffer])
 
         # Only use two tick labels (min and max wavelengths) for
         # thumbnails, because there isn't enough space otherwise.
         if not is_bigplot:
-            rc('font', size=10)
+            this_plotarea.tick_params(labelsize=6., labelrotation=45.,
+                                          axis='y', pad=0.)
             minwl = numpy.nanmin(all_wls)
             maxwl = numpy.nanmax(all_wls)
             this_plotarea.set_xticks([minwl, maxwl])
             this_plotarea.set_xticklabels(this_plotarea.get_xticks(),
                                           rotation=25.)
             this_plotarea.xaxis.set_major_formatter(FormatStrFormatter(
                 "%6.1f"))
@@ -271,15 +272,16 @@
         # `special` plot.  Turn off y-tick labels.
         this_plotarea.set_facecolor("lightgrey")
         this_plotarea.set_yticklabels([])
 
         # Configure the plot units, text size, and other markings based
         # on whether this is a large or thumbnail-sized plot.
         if not is_bigplot:
-            rc('font', size=10)
+            this_plotarea.tick_params(labelsize=6., labelrotation=45.,
+                                          axis='y', pad=0.)
             minwl = numpy.nanmin(all_wls)
             maxwl = numpy.nanmax(all_wls)
             this_plotarea.set_xticks([minwl, maxwl])
             this_plotarea.set_xticklabels(this_plotarea.get_xticks(),
                                           rotation=25.)
             this_plotarea.xaxis.set_major_formatter(FormatStrFormatter(
                 "%6.1f"))
```

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_jwst/readspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_jwst/readspec.py`

 * *Files 3% similar despite different names*

```diff
@@ -59,17 +59,21 @@
             print("*** MAKE_JWST_SPEC_PREVIEWS ERROR: FLUX column not found in"
                   " first extension's binary table.")
             exit(1)
 
         try:
             fluxerr_table = jwst_tabledata.field("ERROR")
         except KeyError:
-            print("*** MAKE_JWST_SPEC_PREVIEWS ERROR: ERROR column not found"
-                  " in first extension's binary table.")
-            exit(1)
+            try:
+                fluxerr_table = jwst_tabledata.field("FLUX_ERROR")
+            except KeyError:
+                print("*** MAKE_JWST_SPEC_PREVIEWS ERROR: neither ERROR "
+                          "nor FLUX_ERROR column found in first "
+                          "extension's binary table.")
+                exit(1)
 
         try:
             dq_table = jwst_tabledata.field("DQ")
         except KeyError:
             print("*** MAKE_JWST_SPEC_PREVIEWS ERROR: DQ column not found"
                   " in first extension's binary table.")
             exit(1)
```

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_stis/__init__.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_stis/__init__.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_stis/get_association_indices.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_stis/get_association_indices.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_stis/plotspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_stis/plotspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_stis/readspec.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_stis/readspec.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots/utils/specutils_stis/stis1dspectrum.py` & `spec_plots-1.35.1/spec_plots/utils/specutils_stis/stis1dspectrum.py`

 * *Files identical despite different names*

### Comparing `spec_plots-1.35.0/spec_plots.egg-info/SOURCES.txt` & `spec_plots-1.35.1/spec_plots.egg-info/SOURCES.txt`

 * *Files identical despite different names*

