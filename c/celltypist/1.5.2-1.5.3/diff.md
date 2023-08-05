# Comparing `tmp/celltypist-1.5.2.tar.gz` & `tmp/celltypist-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/celltypist-1.5.2.tar", last modified: Thu Jun  8 09:15:34 2023, max compression
+gzip compressed data, was "dist/celltypist-1.5.3.tar", last modified: Mon Jul 10 10:41:47 2023, max compression
```

## Comparing `celltypist-1.5.2.tar` & `celltypist-1.5.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:34.972307 celltypist-1.5.2/
--rw-r--r--   0 cx1      (20436) team205   (1403)      256 2022-01-08 15:31:17.000000 celltypist-1.5.2/.gitignore
--rw-r--r--   0 cx1      (20436) team205   (1403)     2471 2023-06-08 09:07:11.000000 celltypist-1.5.2/CHANGELOG.md
--rw-r--r--   0 cx1      (20436) team205   (1403)     5120 2022-06-20 15:29:01.000000 celltypist-1.5.2/CITATION.cff
--rw-r--r--   0 cx1      (20436) team205   (1403)      579 2022-05-31 18:44:35.000000 celltypist-1.5.2/Dockerfile
--rw-r--r--   0 cx1      (20436) team205   (1403)     1056 2021-05-01 12:32:36.000000 celltypist-1.5.2/LICENSE
--rw-r--r--   0 cx1      (20436) team205   (1403)      153 2021-12-25 19:53:33.000000 celltypist-1.5.2/MANIFEST.in
--rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-06-08 09:15:34.965232 celltypist-1.5.2/PKG-INFO
--rw-r--r--   0 cx1      (20436) team205   (1403)    71919 2023-05-16 08:14:33.000000 celltypist-1.5.2/README.md
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:33.613467 celltypist-1.5.2/celltypist/
--rw-r--r--   0 cx1      (20436) team205   (1403)      342 2023-06-08 09:05:19.000000 celltypist-1.5.2/celltypist/__init__.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     6109 2022-08-22 09:17:16.000000 celltypist-1.5.2/celltypist/annotate.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    27443 2023-06-08 09:04:11.000000 celltypist-1.5.2/celltypist/classifier.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     7421 2022-01-26 22:00:20.000000 celltypist-1.5.2/celltypist/command_line.py
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:33.887861 celltypist-1.5.2/celltypist/contro/
--rw-r--r--   0 cx1      (20436) team205   (1403)        0 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/contro/__init__.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    33894 2023-05-15 20:57:38.000000 celltypist-1.5.2/celltypist/contro/align.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    26363 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/contro/distance.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    11379 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/contro/distances.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     8310 2023-05-15 21:15:07.000000 celltypist-1.5.2/celltypist/contro/harmonize.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    15932 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/contro/integrate.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     9960 2023-05-26 14:15:16.000000 celltypist-1.5.2/celltypist/contro/pct.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    30047 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/contro/plot.py
--rw-r--r--   0 cx1      (20436) team205   (1403)      109 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/contro/symbols.py
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:33.160016 celltypist-1.5.2/celltypist/data/
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:33.937214 celltypist-1.5.2/celltypist/data/samples/
--rw-r--r--   0 cx1      (20436) team205   (1403)   557901 2022-01-27 10:03:11.000000 celltypist-1.5.2/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv
--rw-r--r--   0 cx1      (20436) team205   (1403) 53473636 2021-05-01 12:32:37.000000 celltypist-1.5.2/celltypist/data/samples/sample_cell_by_gene.csv
--rw-r--r--   0 cx1      (20436) team205   (1403)      226 2021-05-01 12:32:37.000000 celltypist-1.5.2/celltypist/logger.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    21018 2023-06-08 09:04:11.000000 celltypist-1.5.2/celltypist/models.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    10071 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/plot.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     4157 2022-08-22 08:57:00.000000 celltypist-1.5.2/celltypist/samples.py
--rw-r--r--   0 cx1      (20436) team205   (1403)    19188 2023-05-02 08:46:42.000000 celltypist-1.5.2/celltypist/train.py
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:33.723428 celltypist-1.5.2/celltypist.egg-info/
--rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-06-08 09:15:17.000000 celltypist-1.5.2/celltypist.egg-info/PKG-INFO
--rw-r--r--   0 cx1      (20436) team205   (1403)     1921 2023-06-08 09:15:22.000000 celltypist-1.5.2/celltypist.egg-info/SOURCES.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)        1 2023-06-08 09:15:17.000000 celltypist-1.5.2/celltypist.egg-info/dependency_links.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)       61 2023-06-08 09:15:17.000000 celltypist-1.5.2/celltypist.egg-info/entry_points.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-06-08 09:15:17.000000 celltypist-1.5.2/celltypist.egg-info/requires.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)       11 2023-06-08 09:15:17.000000 celltypist-1.5.2/celltypist.egg-info/top_level.txt
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:34.307488 celltypist-1.5.2/docs/
--rw-r--r--   0 cx1      (20436) team205   (1403)      638 2021-05-01 12:32:37.000000 celltypist-1.5.2/docs/Makefile
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:34.423135 celltypist-1.5.2/docs/notebook/
--rw-r--r--   0 cx1      (20436) team205   (1403)   376236 2022-08-23 10:52:31.000000 celltypist-1.5.2/docs/notebook/celltypist_tutorial.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)   552805 2022-08-23 13:32:51.000000 celltypist-1.5.2/docs/notebook/celltypist_tutorial_cv.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)  1512368 2023-05-16 11:01:52.000000 celltypist-1.5.2/docs/notebook/celltypist_tutorial_harmonisation.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)  3075328 2023-05-16 19:05:14.000000 celltypist-1.5.2/docs/notebook/celltypist_tutorial_integration.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)   629323 2022-08-23 12:38:41.000000 celltypist-1.5.2/docs/notebook/celltypist_tutorial_ml.ipynb
--rw-r--r--   0 cx1      (20436) team205   (1403)      225 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/requirements.txt
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:34.896508 celltypist-1.5.2/docs/source/
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:33.194198 celltypist-1.5.2/docs/source/_static/
-drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-06-08 09:15:34.934831 celltypist-1.5.2/docs/source/_static/img/
--rw-r--r--   0 cx1      (20436) team205   (1403)    67929 2021-11-02 03:08:25.000000 celltypist-1.5.2/docs/source/_static/img/logo_celltypist.png
--rw-r--r--   0 cx1      (20436) team205   (1403)       83 2022-08-05 12:50:13.000000 celltypist-1.5.2/docs/source/celltypist.annotate.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      156 2022-08-05 13:11:23.000000 celltypist-1.5.2/docs/source/celltypist.classifier.AnnotationResult.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      153 2022-08-05 13:12:18.000000 celltypist-1.5.2/docs/source/celltypist.classifier.Classifier.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      162 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.contro.align.DistanceAlignment.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      154 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.contro.distance.Distance.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      161 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.contro.pct.PredictiveClusteringTree.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       80 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.dotplot.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       87 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.harmonize.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       85 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.integrate.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      139 2022-08-05 13:13:01.000000 celltypist-1.5.2/docs/source/celltypist.models.Model.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 13:30:15.000000 celltypist-1.5.2/docs/source/celltypist.models.download_models.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 12:49:53.000000 celltypist-1.5.2/docs/source/celltypist.samples.downsample_adata.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       86 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.sankeyplot.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       78 2022-08-05 12:50:03.000000 celltypist-1.5.2/docs/source/celltypist.train.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)       82 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/celltypist.treeplot.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)     2872 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/conf.py
--rw-r--r--   0 cx1      (20436) team205   (1403)     1602 2023-05-02 08:46:43.000000 celltypist-1.5.2/docs/source/index.rst
--rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-05-02 08:46:43.000000 celltypist-1.5.2/requirements.txt
--rw-r--r--   0 cx1      (20436) team205   (1403)       38 2023-06-08 09:15:34.976713 celltypist-1.5.2/setup.cfg
--rw-r--r--   0 cx1      (20436) team205   (1403)     1519 2023-05-02 08:46:43.000000 celltypist-1.5.2/setup.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:47.727285 celltypist-1.5.3/
+-rw-r--r--   0 cx1      (20436) team205   (1403)      256 2022-01-08 15:31:17.000000 celltypist-1.5.3/.gitignore
+-rw-r--r--   0 cx1      (20436) team205   (1403)     2757 2023-07-10 10:27:13.000000 celltypist-1.5.3/CHANGELOG.md
+-rw-r--r--   0 cx1      (20436) team205   (1403)     5120 2022-06-20 15:29:01.000000 celltypist-1.5.3/CITATION.cff
+-rw-r--r--   0 cx1      (20436) team205   (1403)      579 2022-05-31 18:44:35.000000 celltypist-1.5.3/Dockerfile
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1056 2021-05-01 12:32:36.000000 celltypist-1.5.3/LICENSE
+-rw-r--r--   0 cx1      (20436) team205   (1403)      153 2021-12-25 19:53:33.000000 celltypist-1.5.3/MANIFEST.in
+-rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-07-10 10:41:47.723554 celltypist-1.5.3/PKG-INFO
+-rw-r--r--   0 cx1      (20436) team205   (1403)    71919 2023-05-16 08:14:33.000000 celltypist-1.5.3/README.md
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:44.761697 celltypist-1.5.3/celltypist/
+-rw-r--r--   0 cx1      (20436) team205   (1403)      342 2023-07-10 10:23:27.000000 celltypist-1.5.3/celltypist/__init__.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     6109 2022-08-22 09:17:16.000000 celltypist-1.5.3/celltypist/annotate.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    27443 2023-06-08 09:04:11.000000 celltypist-1.5.3/celltypist/classifier.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     7421 2022-01-26 22:00:20.000000 celltypist-1.5.3/celltypist/command_line.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:45.099509 celltypist-1.5.3/celltypist/contro/
+-rw-r--r--   0 cx1      (20436) team205   (1403)        0 2023-05-02 08:46:42.000000 celltypist-1.5.3/celltypist/contro/__init__.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    33894 2023-05-15 20:57:38.000000 celltypist-1.5.3/celltypist/contro/align.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    26363 2023-05-02 08:46:42.000000 celltypist-1.5.3/celltypist/contro/distance.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    11379 2023-05-02 08:46:42.000000 celltypist-1.5.3/celltypist/contro/distances.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     8310 2023-05-15 21:15:07.000000 celltypist-1.5.3/celltypist/contro/harmonize.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    16008 2023-07-03 12:37:18.000000 celltypist-1.5.3/celltypist/contro/integrate.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     9960 2023-05-26 14:15:16.000000 celltypist-1.5.3/celltypist/contro/pct.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    30047 2023-05-02 08:46:42.000000 celltypist-1.5.3/celltypist/contro/plot.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)      109 2023-05-02 08:46:42.000000 celltypist-1.5.3/celltypist/contro/symbols.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:44.263873 celltypist-1.5.3/celltypist/data/
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:45.281242 celltypist-1.5.3/celltypist/data/samples/
+-rw-r--r--   0 cx1      (20436) team205   (1403)   557901 2022-01-27 10:03:11.000000 celltypist-1.5.3/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv
+-rw-r--r--   0 cx1      (20436) team205   (1403) 53473636 2021-05-01 12:32:37.000000 celltypist-1.5.3/celltypist/data/samples/sample_cell_by_gene.csv
+-rw-r--r--   0 cx1      (20436) team205   (1403)      226 2021-05-01 12:32:37.000000 celltypist-1.5.3/celltypist/logger.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    21018 2023-06-08 09:04:11.000000 celltypist-1.5.3/celltypist/models.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    10265 2023-07-10 10:06:31.000000 celltypist-1.5.3/celltypist/plot.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     4157 2022-08-22 08:57:00.000000 celltypist-1.5.3/celltypist/samples.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)    19188 2023-05-02 08:46:42.000000 celltypist-1.5.3/celltypist/train.py
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:44.860734 celltypist-1.5.3/celltypist.egg-info/
+-rw-r--r--   0 cx1      (20436) team205   (1403)    79562 2023-07-10 10:41:36.000000 celltypist-1.5.3/celltypist.egg-info/PKG-INFO
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1921 2023-07-10 10:41:40.000000 celltypist-1.5.3/celltypist.egg-info/SOURCES.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)        1 2023-07-10 10:41:36.000000 celltypist-1.5.3/celltypist.egg-info/dependency_links.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)       61 2023-07-10 10:41:36.000000 celltypist-1.5.3/celltypist.egg-info/entry_points.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-07-10 10:41:36.000000 celltypist-1.5.3/celltypist.egg-info/requires.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)       11 2023-07-10 10:41:36.000000 celltypist-1.5.3/celltypist.egg-info/top_level.txt
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:46.254289 celltypist-1.5.3/docs/
+-rw-r--r--   0 cx1      (20436) team205   (1403)      638 2021-05-01 12:32:37.000000 celltypist-1.5.3/docs/Makefile
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:46.846002 celltypist-1.5.3/docs/notebook/
+-rw-r--r--   0 cx1      (20436) team205   (1403)   376236 2022-08-23 10:52:31.000000 celltypist-1.5.3/docs/notebook/celltypist_tutorial.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)   552805 2022-08-23 13:32:51.000000 celltypist-1.5.3/docs/notebook/celltypist_tutorial_cv.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)  1512368 2023-05-16 11:01:52.000000 celltypist-1.5.3/docs/notebook/celltypist_tutorial_harmonisation.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)  3075328 2023-05-16 19:05:14.000000 celltypist-1.5.3/docs/notebook/celltypist_tutorial_integration.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)   629323 2022-08-23 12:38:41.000000 celltypist-1.5.3/docs/notebook/celltypist_tutorial_ml.ipynb
+-rw-r--r--   0 cx1      (20436) team205   (1403)      225 2023-07-10 09:52:58.000000 celltypist-1.5.3/docs/requirements.txt
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:47.645507 celltypist-1.5.3/docs/source/
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:44.285217 celltypist-1.5.3/docs/source/_static/
+drwxr-sr-x   0 cx1      (20436) team205   (1403)        0 2023-07-10 10:41:47.661254 celltypist-1.5.3/docs/source/_static/img/
+-rw-r--r--   0 cx1      (20436) team205   (1403)    67929 2021-11-02 03:08:25.000000 celltypist-1.5.3/docs/source/_static/img/logo_celltypist.png
+-rw-r--r--   0 cx1      (20436) team205   (1403)       83 2022-08-05 12:50:13.000000 celltypist-1.5.3/docs/source/celltypist.annotate.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      156 2022-08-05 13:11:23.000000 celltypist-1.5.3/docs/source/celltypist.classifier.AnnotationResult.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      153 2022-08-05 13:12:18.000000 celltypist-1.5.3/docs/source/celltypist.classifier.Classifier.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      162 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.contro.align.DistanceAlignment.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      154 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.contro.distance.Distance.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      161 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.contro.pct.PredictiveClusteringTree.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       80 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.dotplot.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       87 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.harmonize.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       85 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.integrate.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      139 2022-08-05 13:13:01.000000 celltypist-1.5.3/docs/source/celltypist.models.Model.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 13:30:15.000000 celltypist-1.5.3/docs/source/celltypist.models.download_models.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      101 2022-08-05 12:49:53.000000 celltypist-1.5.3/docs/source/celltypist.samples.downsample_adata.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       86 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.sankeyplot.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       78 2022-08-05 12:50:03.000000 celltypist-1.5.3/docs/source/celltypist.train.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)       82 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/celltypist.treeplot.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)     2872 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/conf.py
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1602 2023-05-02 08:46:43.000000 celltypist-1.5.3/docs/source/index.rst
+-rw-r--r--   0 cx1      (20436) team205   (1403)      140 2023-07-10 09:52:45.000000 celltypist-1.5.3/requirements.txt
+-rw-r--r--   0 cx1      (20436) team205   (1403)       38 2023-07-10 10:41:47.730116 celltypist-1.5.3/setup.cfg
+-rw-r--r--   0 cx1      (20436) team205   (1403)     1519 2023-05-02 08:46:43.000000 celltypist-1.5.3/setup.py
```

### Comparing `celltypist-1.5.2/CHANGELOG.md` & `celltypist-1.5.3/CHANGELOG.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 # Changelog
 *********************************
+## CellTypist 1.5.3 (July 10, 2023)
+- Fix DistanceMetric import for sklearn >= 1.3.0 [#73](https://github.com/Teichlab/celltypist/issues/73)
+- Detect input format for [celltypist.train](https://celltypist.readthedocs.io/en/latest/celltypist.train.html)
+- Require leidenalg >= 0.9.0
 ## CellTypist 1.5.2 (June 8, 2023)
-Patch log1p serialization issue and model download error
+- Patch log1p serialization issue and model download error
 ## CellTypist 1.5.1 (May 26, 2023)
-Fix error in not importing spmatrix in pct
+- Fix error in not importing spmatrix in pct
 ## CellTypist 1.5.0 (May 16, 2023)
 A more mature release before the formal CellTypist v2
 ## CellTypist 1.4.0 (May 2, 2023)
 - Add modules of cell type harmonisation and integration (a release before the formal CellTypist v2)
 ## CellTypist 1.3.0 (December 14, 2022)
 - Transfer numpy matrix to array during prediction for compatibility with sklearn >= 1.0 [#50](https://github.com/Teichlab/celltypist/issues/50)
 ## CellTypist 1.2.0 (August 22, 2022)
```

### Comparing `celltypist-1.5.2/CITATION.cff` & `celltypist-1.5.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/Dockerfile` & `celltypist-1.5.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/LICENSE` & `celltypist-1.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/PKG-INFO` & `celltypist-1.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celltypist
-Version: 1.5.2
+Version: 1.5.3
 Summary: A tool for semi-automatic cell type classification, harmonization and integration
 Home-page: https://github.com/Teichlab/celltypist
 Author: Chuan Xu
 Author-email: cx1@sanger.ac.uk
 License: UNKNOWN
 Description: <p align="left"><img src="https://github.com/Teichlab/celltypist/blob/main/docs/source/_static/img/logo_celltypist.png" width="250" height="85"></p>
```

### Comparing `celltypist-1.5.2/README.md` & `celltypist-1.5.3/README.md`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/annotate.py` & `celltypist-1.5.3/celltypist/annotate.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/classifier.py` & `celltypist-1.5.3/celltypist/classifier.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/command_line.py` & `celltypist-1.5.3/celltypist/command_line.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/contro/align.py` & `celltypist-1.5.3/celltypist/contro/align.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/contro/distance.py` & `celltypist-1.5.3/celltypist/contro/distance.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/contro/distances.py` & `celltypist-1.5.3/celltypist/contro/distances.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/contro/harmonize.py` & `celltypist-1.5.3/celltypist/contro/harmonize.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/contro/integrate.py` & `celltypist-1.5.3/celltypist/contro/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import numpy as np
 import pandas as pd
 from anndata import AnnData
 from typing import Optional, Union
 import types
 import sys
-from sklearn.neighbors import DistanceMetric
+try:
+    from sklearn.neighbors import DistanceMetric
+except ImportError:
+    from sklearn.metrics import DistanceMetric
 from sklearn.neighbors import KDTree
 from sklearn.metrics import pairwise_distances
 from .. import logger
 from .symbols import UNASSIGN
 from umap.umap_ import fuzzy_simplicial_set
 import pynndescent
 from annoy import AnnoyIndex
```

### Comparing `celltypist-1.5.2/celltypist/contro/pct.py` & `celltypist-1.5.3/celltypist/contro/pct.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/contro/plot.py` & `celltypist-1.5.3/celltypist/contro/plot.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv` & `celltypist-1.5.3/celltypist/data/samples/Ensembl105_Human2Mouse_Genes.csv`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/data/samples/sample_cell_by_gene.csv` & `celltypist-1.5.3/celltypist/data/samples/sample_cell_by_gene.csv`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/models.py` & `celltypist-1.5.3/celltypist/models.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/plot.py` & `celltypist-1.5.3/celltypist/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
                           prediction_order: Optional[Union[list, tuple, np.ndarray, pd.Series, pd.Index]] = None,
                           reference_order: Optional[Union[list, tuple, np.ndarray, pd.Series, pd.Index]] = None
                           ) -> tuple:
     """
     For internal use. Get the fraction and avg. probability data frames (predictions * truths) from AnnotationResult.
     """
     #prediction
+    if not isinstance(predictions, AnnotationResult):
+        raise TypeError(
+                f"🛑 Please provide a correct input - an `AnnotationResult` derived from `celltypist.annotate`")
     if use_as_prediction not in predictions.predicted_labels:
         if use_as_prediction == 'majority_voting':
             raise KeyError(
                     f"🛑 Did not find the column `majority_voting` in the `AnnotationResult.predicted_labels`, perform majority voting beforehand or use `use_as_prediction = 'predicted_labels'` instead")
         else:
             raise KeyError(
                     f"🛑 Did not find such column '{use_as_prediction}', should be one of `'majority_voting'` or `'predicted_labels'`")
```

### Comparing `celltypist-1.5.2/celltypist/samples.py` & `celltypist-1.5.3/celltypist/samples.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist/train.py` & `celltypist-1.5.3/celltypist/train.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/celltypist.egg-info/PKG-INFO` & `celltypist-1.5.3/celltypist.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: celltypist
-Version: 1.5.2
+Version: 1.5.3
 Summary: A tool for semi-automatic cell type classification, harmonization and integration
 Home-page: https://github.com/Teichlab/celltypist
 Author: Chuan Xu
 Author-email: cx1@sanger.ac.uk
 License: UNKNOWN
 Description: <p align="left"><img src="https://github.com/Teichlab/celltypist/blob/main/docs/source/_static/img/logo_celltypist.png" width="250" height="85"></p>
```

### Comparing `celltypist-1.5.2/celltypist.egg-info/SOURCES.txt` & `celltypist-1.5.3/celltypist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/Makefile` & `celltypist-1.5.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/notebook/celltypist_tutorial.ipynb` & `celltypist-1.5.3/docs/notebook/celltypist_tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/notebook/celltypist_tutorial_cv.ipynb` & `celltypist-1.5.3/docs/notebook/celltypist_tutorial_cv.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/notebook/celltypist_tutorial_harmonisation.ipynb` & `celltypist-1.5.3/docs/notebook/celltypist_tutorial_harmonisation.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/notebook/celltypist_tutorial_integration.ipynb` & `celltypist-1.5.3/docs/notebook/celltypist_tutorial_integration.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/notebook/celltypist_tutorial_ml.ipynb` & `celltypist-1.5.3/docs/notebook/celltypist_tutorial_ml.ipynb`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/source/_static/img/logo_celltypist.png` & `celltypist-1.5.3/docs/source/_static/img/logo_celltypist.png`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/source/conf.py` & `celltypist-1.5.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/docs/source/index.rst` & `celltypist-1.5.3/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `celltypist-1.5.2/setup.py` & `celltypist-1.5.3/setup.py`

 * *Files identical despite different names*

