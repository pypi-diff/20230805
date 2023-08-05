# Comparing `tmp/sklearn2pmml-0.97.0.tar.gz` & `tmp/sklearn2pmml-0.97.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sklearn2pmml-0.97.0.tar", last modified: Thu Aug  3 12:57:47 2023, max compression
+gzip compressed data, was "dist/sklearn2pmml-0.97.1.tar", last modified: Sat Aug  5 16:19:21 2023, max compression
```

## Comparing `sklearn2pmml-0.97.0.tar` & `sklearn2pmml-0.97.1.tar`

### file list

```diff
@@ -1,79 +1,79 @@
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.0/setup.cfg
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.0/LICENSE.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1403 2023-07-16 18:17:01.000000 sklearn2pmml-0.97.0/setup.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/PKG-INFO
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/h2o.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/ruleset/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/ruleset/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/pipeline/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/pipeline/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/tpot.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    12365 2023-07-31 06:07:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/decoration/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/decoration/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/neural_network/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/neural_network/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/pycaret.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/util/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/util/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/xgboost.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/text/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/text/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/ensemble/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/ensemble/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/statsmodels.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_selection/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/feature_selection/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/postprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/postprocessing/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   474695 2023-08-03 12:40:49.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-1.7.34.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  3041245 2023-07-18 12:18:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/guava-32.1.1-jre.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    51724 2023-07-22 06:57:40.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-h2o-1.2.9.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jcommander-1.72.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   198931 2023-07-20 20:18:17.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-converter-1.5.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    68200 2023-07-21 08:53:01.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     6242 2023-08-03 12:40:52.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.34.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-0.1.8.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   283367 2023-07-21 09:00:16.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/gson-2.10.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   442631 2023-07-30 05:41:05.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      818 2023-08-03 12:46:00.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/classpath.txt
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-30 05:41:05.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     4888 2023-08-03 12:46:01.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   209112 2023-07-21 07:47:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-python-1.1.17.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7357 2023-08-03 12:40:52.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.34.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/serpent-1.40.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7767 2023-08-03 12:40:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.34.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    84465 2023-08-03 12:40:51.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.34.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     7977 2023-08-03 12:40:52.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.34.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    30899 2023-07-21 19:03:56.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pickle-1.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-07-21 09:07:53.000000 sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-08-03 12:45:30.000000 sklearn2pmml-0.97.0/sklearn2pmml/metadata.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/h2o.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/__init__.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/xgboost.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/lightgbm.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/tree/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/tree/chaid.py
--rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/tree/__init__.py
-drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-03 12:57:47.000000 sklearn2pmml-0.97.0/sklearn2pmml/expression/
--rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.0/sklearn2pmml/expression/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)       40 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.1/setup.cfg
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    34520 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.1/LICENSE.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1403 2023-07-16 18:17:01.000000 sklearn2pmml-0.97.1/setup.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      739 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/PKG-INFO
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      840 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/h2o.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/ruleset/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      888 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/ruleset/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/pipeline/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6005 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/pipeline/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      769 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/tpot.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    12365 2023-07-31 06:07:51.000000 sklearn2pmml-0.97.1/sklearn2pmml/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/decoration/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16924 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/decoration/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/neural_network/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      777 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/neural_network/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      640 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/pycaret.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/util/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7471 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/util/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1108 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/xgboost.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/feature_extraction/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2018-03-12 15:29:56.000000 sklearn2pmml-0.97.1/sklearn2pmml/feature_extraction/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/feature_extraction/text/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1123 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/feature_extraction/text/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/ensemble/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     9294 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/ensemble/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4574 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/statsmodels.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/feature_selection/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      846 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/feature_selection/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/postprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1740 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/postprocessing/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1300 2020-10-11 20:49:33.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8245 2023-08-05 16:08:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.35.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  3041245 2023-07-18 12:18:27.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/guava-32.1.1-jre.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   139727 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      297 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    41125 2022-02-16 09:19:19.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    84465 2023-08-05 16:08:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.35.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    51724 2023-07-22 06:57:40.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-h2o-1.2.9.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    75714 2022-07-22 17:55:51.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    69254 2018-02-17 21:50:20.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/jcommander-1.72.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   198931 2023-07-20 20:18:17.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-converter-1.5.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    68200 2023-07-21 08:53:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)  1138813 2022-08-01 13:09:48.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-model-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2235 2022-05-06 18:22:34.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4708 2022-08-01 13:10:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   476817 2023-08-05 16:08:00.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-1.7.35.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    39662 2022-05-06 18:22:34.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/ubjson-0.1.8.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   283367 2023-07-21 09:00:16.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/gson-2.10.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   442631 2023-07-30 05:41:05.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      818 2023-08-05 16:16:43.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/classpath.txt
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4526 2023-07-30 05:41:05.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7863 2023-08-05 16:08:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-h2o-1.7.35.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     4887 2023-08-05 16:16:45.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/sklearn2pmml-1.0-SNAPSHOT.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   209112 2023-07-21 07:47:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-python-1.1.17.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     8436 2022-02-16 09:19:19.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   913701 2021-10-23 18:57:29.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    44790 2021-06-01 08:00:08.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/serpent-1.40.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    29896 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    62154 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)   128941 2021-10-23 18:57:27.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     7608 2023-08-05 16:08:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.35.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    30899 2023-07-21 19:03:56.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    54294 2023-06-11 07:47:11.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pickle-1.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    72620 2023-07-21 09:07:53.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     6844 2023-08-05 16:08:01.000000 sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.35.jar
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      144 2023-08-05 16:16:33.000000 sklearn2pmml-0.97.1/sklearn2pmml/metadata.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)      880 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/h2o.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)    16423 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/__init__.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1724 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/xgboost.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1868 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/lightgbm.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/tree/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     1941 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/tree/chaid.py
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)        0 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/tree/__init__.py
+drwxrwxr-x   0 vfed      (1000) vfed      (1000)        0 2023-08-05 16:19:21.000000 sklearn2pmml-0.97.1/sklearn2pmml/expression/
+-rw-rw-r--   0 vfed      (1000) vfed      (1000)     2944 2023-06-02 16:05:54.000000 sklearn2pmml-0.97.1/sklearn2pmml/expression/__init__.py
```

### Comparing `sklearn2pmml-0.97.0/LICENSE.txt` & `sklearn2pmml-0.97.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/setup.py` & `sklearn2pmml-0.97.1/setup.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/PKG-INFO` & `sklearn2pmml-0.97.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: sklearn2pmml
-Version: 0.97.0
+Version: 0.97.1
 Summary: Python library for converting Scikit-Learn pipelines to PMML
 Home-page: https://github.com/jpmml/sklearn2pmml
 Author: Villu Ruusmann
 Author-email: villu.ruusmann@gmail.com
 License: GNU Affero General Public License (AGPL) version 3.0
-Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.97.0.tar.gz
+Download-URL: https://github.com/jpmml/sklearn2pmml/archive/0.97.1.tar.gz
 Description: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/h2o.py` & `sklearn2pmml-0.97.1/sklearn2pmml/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/ruleset/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/ruleset/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/pipeline/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/tpot.py` & `sklearn2pmml-0.97.1/sklearn2pmml/tpot.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/decoration/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/decoration/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/neural_network/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/neural_network/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/pycaret.py` & `sklearn2pmml-0.97.1/sklearn2pmml/pycaret.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/util/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/util/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/xgboost.py` & `sklearn2pmml-0.97.1/sklearn2pmml/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/feature_extraction/text/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/feature_extraction/text/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/ensemble/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/statsmodels.py` & `sklearn2pmml-0.97.1/sklearn2pmml/statsmodels.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/feature_selection/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/feature_selection/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/postprocessing/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/postprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/h2o-tree-api-0.3.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-1.7.34.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-1.7.35.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,412 +1,416 @@
-Zip file size: 474695 bytes, number of entries: 410
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
--rw-r--r--  2.0 unx      159 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn_pandas/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 chaid/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 stop_words/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/calibration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/dummy/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/svm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/impute/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/naive_bayes/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/logistic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/ridge/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/glm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/compose/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/model_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/decomposition/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/neighbors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/multioutput/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/isotonic/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/metrics/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/bagging/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/stacking/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/forest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/iforest/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/voting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/ensemble/weight_boosting/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/loss/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/discriminant_analysis/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/tree/visitors/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/cluster/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn/multiclass/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/ruleset/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/decoration/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/neural_network/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/util/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/feature_extraction/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/feature_extraction/text/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/ensemble/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/feature_selection/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/postprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/preprocessing/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/tree/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/expression/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/jpmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/jpmml/sklearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 org/jpmml/sklearn/testing/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn/
--rw-rw-r--  2.0 unx    16829 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2287 b- defN 23-Aug-03 15:40 sklearn_pandas/CategoricalImputer.class
--rw-rw-r--  2.0 unx      656 b- defN 23-Aug-03 15:40 sklearn_pandas/TransformerPipeline.class
--rw-rw-r--  2.0 unx     1154 b- defN 23-Aug-03 15:40 sklearn_pandas/DataFrameMapper$2.class
--rw-rw-r--  2.0 unx     6280 b- defN 23-Aug-03 15:40 sklearn_pandas/DataFrameMapper.class
--rw-rw-r--  2.0 unx     1126 b- defN 23-Aug-03 15:40 sklearn_pandas/DataFrameMapper$1.class
--rw-rw-r--  2.0 unx      609 b- defN 23-Aug-03 15:40 chaid/ContinuousColumn.class
--rw-rw-r--  2.0 unx      925 b- defN 23-Aug-03 15:40 chaid/Node.class
--rw-rw-r--  2.0 unx      467 b- defN 23-Aug-03 15:40 chaid/Column.class
--rw-rw-r--  2.0 unx     3283 b- defN 23-Aug-03 15:40 chaid/Split.class
--rw-rw-r--  2.0 unx      401 b- defN 23-Aug-03 15:40 chaid/InvalidSplitReason.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Aug-03 15:40 chaid/NominalColumn.class
--rw-rw-r--  2.0 unx     1912 b- defN 23-Aug-03 15:40 stop_words/english.txt
--rw-rw-r--  2.0 unx      147 b- defN 23-Aug-03 15:40 sklearn/HasHead.class
--rw-rw-r--  2.0 unx     1728 b- defN 23-Aug-03 15:40 sklearn/StepUtil.class
--rw-rw-r--  2.0 unx    12045 b- defN 23-Aug-03 15:40 sklearn/calibration/CalibratedClassifier.class
--rw-rw-r--  2.0 unx     2953 b- defN 23-Aug-03 15:40 sklearn/calibration/SigmoidCalibration.class
--rw-rw-r--  2.0 unx      683 b- defN 23-Aug-03 15:40 sklearn/calibration/CalibratedClassifier$1.class
--rw-rw-r--  2.0 unx     3672 b- defN 23-Aug-03 15:40 sklearn/calibration/CalibratedClassifierCV.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineTransformer.class
--rw-rw-r--  2.0 unx     1697 b- defN 23-Aug-03 15:40 sklearn/pipeline/Pipeline$2.class
--rw-rw-r--  2.0 unx     2536 b- defN 23-Aug-03 15:40 sklearn/pipeline/FeatureUnion.class
--rw-rw-r--  2.0 unx     5599 b- defN 23-Aug-03 15:40 sklearn/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx     2327 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineRegressor.class
--rw-rw-r--  2.0 unx     1742 b- defN 23-Aug-03 15:40 sklearn/pipeline/Pipeline$1.class
--rw-rw-r--  2.0 unx     1111 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineUtil.class
--rw-rw-r--  2.0 unx     2589 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineClassifier.class
--rw-rw-r--  2.0 unx     2435 b- defN 23-Aug-03 15:40 sklearn/pipeline/PipelineClusterer.class
--rw-rw-r--  2.0 unx     5027 b- defN 23-Aug-03 15:40 sklearn/dummy/DummyClassifier.class
--rw-rw-r--  2.0 unx     2174 b- defN 23-Aug-03 15:40 sklearn/dummy/DummyRegressor.class
--rw-rw-r--  2.0 unx      512 b- defN 23-Aug-03 15:40 sklearn/SkLearnFields.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Aug-03 15:40 sklearn/SkLearnOutlierTransformation.class
--rw-rw-r--  2.0 unx      240 b- defN 23-Aug-03 15:40 sklearn/HasEstimator.class
--rw-rw-r--  2.0 unx     3421 b- defN 23-Aug-03 15:40 sklearn/OutlierDetectorUtil.class
--rw-rw-r--  2.0 unx     1236 b- defN 23-Aug-03 15:40 sklearn/HasMultiApplyField.class
--rw-rw-r--  2.0 unx     2393 b- defN 23-Aug-03 15:40 sklearn/svm/SupportVectorMachineUtil.class
--rw-rw-r--  2.0 unx     1109 b- defN 23-Aug-03 15:40 sklearn/svm/LinearSVC.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Aug-03 15:40 sklearn/svm/LibSVMClassifier.class
--rw-rw-r--  2.0 unx      966 b- defN 23-Aug-03 15:40 sklearn/svm/SupportVectorMachineUtil$1.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Aug-03 15:40 sklearn/svm/OneClassSVM.class
--rw-rw-r--  2.0 unx     3594 b- defN 23-Aug-03 15:40 sklearn/svm/LibSVMRegressor.class
--rw-rw-r--  2.0 unx     3007 b- defN 23-Aug-03 15:40 sklearn/InitializerUtil$1.class
--rw-rw-r--  2.0 unx      735 b- defN 23-Aug-03 15:40 sklearn/Estimator$1.class
--rw-rw-r--  2.0 unx      342 b- defN 23-Aug-03 15:40 sklearn/HasOutlierField.class
--rw-rw-r--  2.0 unx      214 b- defN 23-Aug-03 15:40 sklearn/HasNumberOfFeatures.class
--rw-rw-r--  2.0 unx      660 b- defN 23-Aug-03 15:40 sklearn/MultiTransformer.class
--rw-rw-r--  2.0 unx     2110 b- defN 23-Aug-03 15:40 sklearn/neural_network/MLPRegressor.class
--rw-rw-r--  2.0 unx     2555 b- defN 23-Aug-03 15:40 sklearn/neural_network/MLPClassifier.class
--rw-rw-r--  2.0 unx      759 b- defN 23-Aug-03 15:40 sklearn/neural_network/MultilayerPerceptronUtil$1.class
--rw-rw-r--  2.0 unx     8927 b- defN 23-Aug-03 15:40 sklearn/neural_network/MultilayerPerceptronUtil.class
--rw-rw-r--  2.0 unx     1761 b- defN 23-Aug-03 15:40 sklearn/Step.class
--rw-rw-r--  2.0 unx      168 b- defN 23-Aug-03 15:40 sklearn/HasDefaultValue.class
--rw-rw-r--  2.0 unx       99 b- defN 23-Aug-03 15:40 sklearn/Proxy.class
--rw-rw-r--  2.0 unx     2936 b- defN 23-Aug-03 15:40 sklearn/impute/MissingIndicator.class
--rw-rw-r--  2.0 unx     4027 b- defN 23-Aug-03 15:40 sklearn/impute/ImputerUtil.class
--rw-rw-r--  2.0 unx     5703 b- defN 23-Aug-03 15:40 sklearn/impute/SimpleImputer.class
--rw-rw-r--  2.0 unx     6948 b- defN 23-Aug-03 15:40 sklearn/naive_bayes/GaussianNB.class
--rw-rw-r--  2.0 unx      233 b- defN 23-Aug-03 15:40 sklearn/HasFeatureNamesIn.class
--rw-rw-r--  2.0 unx     4446 b- defN 23-Aug-03 15:40 sklearn/linear_model/LinearRegressor.class
--rw-rw-r--  2.0 unx     5037 b- defN 23-Aug-03 15:40 sklearn/linear_model/LinearClassifier.class
--rw-rw-r--  2.0 unx     7645 b- defN 23-Aug-03 15:40 sklearn/linear_model/logistic/LogisticRegression.class
--rw-rw-r--  2.0 unx     1042 b- defN 23-Aug-03 15:40 sklearn/linear_model/ridge/RidgeClassifier.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Aug-03 15:40 sklearn/linear_model/glm/DistributionBoundary.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Aug-03 15:40 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
--rw-rw-r--  2.0 unx      947 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/Hinge.class
--rw-rw-r--  2.0 unx     2440 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
--rw-rw-r--  2.0 unx      461 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/LossFunction.class
--rw-rw-r--  2.0 unx      452 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/Log.class
--rw-rw-r--  2.0 unx     1165 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
--rw-rw-r--  2.0 unx      482 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
--rw-rw-r--  2.0 unx      968 b- defN 23-Aug-03 15:40 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
--rw-rw-r--  2.0 unx     1746 b- defN 23-Aug-03 15:40 sklearn/compose/ColumnTransformer$1.class
--rw-rw-r--  2.0 unx     3239 b- defN 23-Aug-03 15:40 sklearn/compose/TransformedTargetRegressor.class
--rw-rw-r--  2.0 unx     3649 b- defN 23-Aug-03 15:40 sklearn/compose/ColumnTransformer.class
--rw-rw-r--  2.0 unx     1534 b- defN 23-Aug-03 15:40 sklearn/compose/TransformedTargetRegressor$1.class
--rw-rw-r--  2.0 unx      894 b- defN 23-Aug-03 15:40 sklearn/IdentityTransformer.class
--rw-rw-r--  2.0 unx     4089 b- defN 23-Aug-03 15:40 sklearn/Classifier.class
--rw-rw-r--  2.0 unx     1457 b- defN 23-Aug-03 15:40 sklearn/model_selection/EstimatorSearcher.class
--rw-rw-r--  2.0 unx     1685 b- defN 23-Aug-03 15:40 sklearn/Selector.class
--rw-rw-r--  2.0 unx      419 b- defN 23-Aug-03 15:40 sklearn/decomposition/IncrementalPCA.class
--rw-rw-r--  2.0 unx     3471 b- defN 23-Aug-03 15:40 sklearn/decomposition/TruncatedSVD.class
--rw-rw-r--  2.0 unx     4759 b- defN 23-Aug-03 15:40 sklearn/decomposition/PCA.class
--rw-rw-r--  2.0 unx      911 b- defN 23-Aug-03 15:40 sklearn/decomposition/BasePCA.class
--rw-rw-r--  2.0 unx      336 b- defN 23-Aug-03 15:40 sklearn/HasPredictField.class
--rw-rw-r--  2.0 unx     3018 b- defN 23-Aug-03 15:40 sklearn/neighbors/NearestNeighbors.class
--rw-rw-r--  2.0 unx     4505 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsClassifier.class
--rw-rw-r--  2.0 unx     3794 b- defN 23-Aug-03 15:40 sklearn/neighbors/NearestCentroid.class
--rw-rw-r--  2.0 unx     2061 b- defN 23-Aug-03 15:40 sklearn/neighbors/BinaryTree.class
--rw-rw-r--  2.0 unx     1266 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsUtil$1.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Aug-03 15:40 sklearn/neighbors/HasMetric.class
--rw-rw-r--  2.0 unx    10745 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsUtil.class
--rw-rw-r--  2.0 unx     4387 b- defN 23-Aug-03 15:40 sklearn/neighbors/KNeighborsRegressor.class
--rw-rw-r--  2.0 unx     1068 b- defN 23-Aug-03 15:40 sklearn/neighbors/DistanceMetric.class
--rw-rw-r--  2.0 unx      351 b- defN 23-Aug-03 15:40 sklearn/neighbors/HasTrainingData.class
--rw-rw-r--  2.0 unx      176 b- defN 23-Aug-03 15:40 sklearn/neighbors/HasNumberOfNeighbors.class
--rw-rw-r--  2.0 unx     2666 b- defN 23-Aug-03 15:40 sklearn/multioutput/MultiOutputUtil.class
--rw-rw-r--  2.0 unx     3522 b- defN 23-Aug-03 15:40 sklearn/multioutput/ChainUtil.class
--rw-rw-r--  2.0 unx     1601 b- defN 23-Aug-03 15:40 sklearn/multioutput/RegressorChain.class
--rw-rw-r--  2.0 unx     1316 b- defN 23-Aug-03 15:40 sklearn/multioutput/MultiOutputClassifier.class
--rw-rw-r--  2.0 unx     1310 b- defN 23-Aug-03 15:40 sklearn/multioutput/MultiOutputRegressor.class
--rw-rw-r--  2.0 unx     1745 b- defN 23-Aug-03 15:40 sklearn/multioutput/ClassifierChain.class
--rw-rw-r--  2.0 unx     4450 b- defN 23-Aug-03 15:40 sklearn/isotonic/IsotonicRegression.class
--rw-rw-r--  2.0 unx      326 b- defN 23-Aug-03 15:40 sklearn/HasApplyField.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Aug-03 15:40 sklearn/HasEstimatorEnsemble.class
--rw-rw-r--  2.0 unx     2094 b- defN 23-Aug-03 15:40 sklearn/Transformer$1.class
--rw-rw-r--  2.0 unx      953 b- defN 23-Aug-03 15:40 sklearn/LabelEncoderClassifier.class
--rw-rw-r--  2.0 unx      451 b- defN 23-Aug-03 15:40 sklearn/PassThrough.class
--rw-rw-r--  2.0 unx      181 b- defN 23-Aug-03 15:40 sklearn/HasPriorProbability.class
--rw-rw-r--  2.0 unx      230 b- defN 23-Aug-03 15:40 sklearn/SkLearnSteps.class
--rw-rw-r--  2.0 unx     5693 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/TfidfVectorizer.class
--rw-rw-r--  2.0 unx      809 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/TfidfVectorizer$1.class
--rw-rw-r--  2.0 unx      675 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/Tokenizer.class
--rw-rw-r--  2.0 unx    13329 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/CountVectorizer.class
--rw-rw-r--  2.0 unx     2129 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/CountVectorizer$1.class
--rw-rw-r--  2.0 unx     1433 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/text/TfidfTransformer.class
--rw-rw-r--  2.0 unx     4030 b- defN 23-Aug-03 15:40 sklearn/feature_extraction/DictVectorizer.class
--rw-rw-r--  2.0 unx      762 b- defN 23-Aug-03 15:40 sklearn/Clusterer.class
--rw-rw-r--  2.0 unx     1411 b- defN 23-Aug-03 15:40 sklearn/metrics/DistanceMetric.class
--rw-rw-r--  2.0 unx     1069 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleUtil.class
--rw-rw-r--  2.0 unx     2112 b- defN 23-Aug-03 15:40 sklearn/ensemble/bagging/BaggingRegressor.class
--rw-rw-r--  2.0 unx     3293 b- defN 23-Aug-03 15:40 sklearn/ensemble/bagging/BaggingUtil.class
--rw-rw-r--  2.0 unx     3031 b- defN 23-Aug-03 15:40 sklearn/ensemble/bagging/BaggingClassifier.class
--rw-rw-r--  2.0 unx     1409 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleRegressor.class
--rw-rw-r--  2.0 unx     3485 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingClassifier.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
--rw-rw-r--  2.0 unx     3109 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingRegressor.class
--rw-rw-r--  2.0 unx     3862 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingUtil.class
--rw-rw-r--  2.0 unx     2524 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingClassifier$1.class
--rw-rw-r--  2.0 unx     2254 b- defN 23-Aug-03 15:40 sklearn/ensemble/stacking/StackingRegressor$1.class
--rw-rw-r--  2.0 unx      495 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
--rw-rw-r--  2.0 unx     1440 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
--rw-rw-r--  2.0 unx     1862 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
--rw-rw-r--  2.0 unx     2563 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
--rw-rw-r--  2.0 unx      858 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/LossFunction.class
--rw-rw-r--  2.0 unx     1588 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
--rw-rw-r--  2.0 unx     1317 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
--rw-rw-r--  2.0 unx     7945 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
--rw-rw-r--  2.0 unx      960 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/MeanEstimator.class
--rw-rw-r--  2.0 unx     1265 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
--rw-rw-r--  2.0 unx     1578 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
--rw-rw-r--  2.0 unx      811 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
--rw-rw-r--  2.0 unx     3003 b- defN 23-Aug-03 15:40 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
--rw-rw-r--  2.0 unx     1148 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleUtil$1.class
--rw-rw-r--  2.0 unx     3059 b- defN 23-Aug-03 15:40 sklearn/ensemble/forest/ForestUtil.class
--rw-rw-r--  2.0 unx     2528 b- defN 23-Aug-03 15:40 sklearn/ensemble/forest/ForestRegressor.class
--rw-rw-r--  2.0 unx     2987 b- defN 23-Aug-03 15:40 sklearn/ensemble/forest/ForestClassifier.class
--rw-rw-r--  2.0 unx     1752 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest$3.class
--rw-rw-r--  2.0 unx     2206 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest$1.class
--rw-rw-r--  2.0 unx     1716 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest$2.class
--rw-rw-r--  2.0 unx     8225 b- defN 23-Aug-03 15:40 sklearn/ensemble/iforest/IsolationForest.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Aug-03 15:40 sklearn/ensemble/voting/VotingClassifier.class
--rw-rw-r--  2.0 unx     3716 b- defN 23-Aug-03 15:40 sklearn/ensemble/voting/VotingRegressor.class
--rw-rw-r--  2.0 unx     2814 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
--rw-rw-r--  2.0 unx     1247 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
--rw-rw-r--  2.0 unx     3041 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
--rw-rw-r--  2.0 unx     6152 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
--rw-rw-r--  2.0 unx      505 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
--rw-rw-r--  2.0 unx      490 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
--rw-rw-r--  2.0 unx     1572 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
--rw-rw-r--  2.0 unx     6374 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
--rw-rw-r--  2.0 unx     8868 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
--rw-rw-r--  2.0 unx      441 b- defN 23-Aug-03 15:40 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
--rw-rw-r--  2.0 unx     1418 b- defN 23-Aug-03 15:40 sklearn/ensemble/EnsembleClassifier.class
--rw-rw-r--  2.0 unx     3564 b- defN 23-Aug-03 15:40 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
--rw-rw-r--  2.0 unx     6362 b- defN 23-Aug-03 15:40 sklearn/Transformer.class
--rw-rw-r--  2.0 unx      859 b- defN 23-Aug-03 15:40 sklearn/Transformer$1$1.class
--rw-rw-r--  2.0 unx      981 b- defN 23-Aug-03 15:40 sklearn/Drop.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-03 15:40 sklearn/feature_selection/SelectKBest$Entry.class
--rw-rw-r--  2.0 unx     3486 b- defN 23-Aug-03 15:40 sklearn/feature_selection/SelectFromModel.class
--rw-rw-r--  2.0 unx     2922 b- defN 23-Aug-03 15:40 sklearn/feature_selection/SelectKBest.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Aug-03 15:40 sklearn/feature_selection/PySelector.class
--rw-rw-r--  2.0 unx      607 b- defN 23-Aug-03 15:40 sklearn/Transformer$2.class
--rw-rw-r--  2.0 unx     2216 b- defN 23-Aug-03 15:40 sklearn/SkLearnUtil.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Aug-03 15:40 sklearn/loss/HalfMultinomialLoss.class
--rw-rw-r--  2.0 unx      602 b- defN 23-Aug-03 15:40 sklearn/loss/CyLossFunction.class
--rw-rw-r--  2.0 unx      403 b- defN 23-Aug-03 15:40 sklearn/loss/HalfBinomialLoss.class
--rw-rw-r--  2.0 unx      387 b- defN 23-Aug-03 15:40 sklearn/loss/BaseLoss.class
--rw-rw-r--  2.0 unx      381 b- defN 23-Aug-03 15:40 sklearn/HasDecisionFunctionField.class
--rw-rw-r--  2.0 unx      338 b- defN 23-Aug-03 15:40 sklearn/SkLearnMethods.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Aug-03 15:40 sklearn/OutlierDetectorUtil$1.class
--rw-rw-r--  2.0 unx      195 b- defN 23-Aug-03 15:40 sklearn/HasClasses.class
--rw-rw-r--  2.0 unx     4682 b- defN 23-Aug-03 15:40 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
--rw-rw-r--  2.0 unx      696 b- defN 23-Aug-03 15:40 sklearn/EstimatorUtil$1.class
--rw-rw-r--  2.0 unx     3817 b- defN 23-Aug-03 15:40 sklearn/Composite.class
--rw-rw-r--  2.0 unx     1194 b- defN 23-Aug-03 15:40 sklearn/preprocessing/KBinsDiscretizer$1.class
--rw-rw-r--  2.0 unx     4567 b- defN 23-Aug-03 15:40 sklearn/preprocessing/PowerTransformer.class
--rw-rw-r--  2.0 unx     2381 b- defN 23-Aug-03 15:40 sklearn/preprocessing/LabelEncoder.class
--rw-rw-r--  2.0 unx     4924 b- defN 23-Aug-03 15:40 sklearn/preprocessing/LabelBinarizer.class
--rw-rw-r--  2.0 unx     1158 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$3.class
--rw-rw-r--  2.0 unx      389 b- defN 23-Aug-03 15:40 sklearn/preprocessing/Scaler.class
--rw-rw-r--  2.0 unx      797 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MultiOneHotEncoder$1.class
--rw-rw-r--  2.0 unx     3242 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MaxAbsScaler.class
--rw-rw-r--  2.0 unx     2948 b- defN 23-Aug-03 15:40 sklearn/preprocessing/FunctionTransformer.class
--rw-rw-r--  2.0 unx     3291 b- defN 23-Aug-03 15:40 sklearn/preprocessing/BaseEncoder.class
--rw-rw-r--  2.0 unx     1270 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$1.class
--rw-rw-r--  2.0 unx     4549 b- defN 23-Aug-03 15:40 sklearn/preprocessing/StandardScaler.class
--rw-rw-r--  2.0 unx     9005 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil.class
--rw-rw-r--  2.0 unx     6343 b- defN 23-Aug-03 15:40 sklearn/preprocessing/PolynomialFeatures.class
--rw-rw-r--  2.0 unx     8486 b- defN 23-Aug-03 15:40 sklearn/preprocessing/KBinsDiscretizer.class
--rw-rw-r--  2.0 unx     4671 b- defN 23-Aug-03 15:40 sklearn/preprocessing/OneHotEncoder.class
--rw-rw-r--  2.0 unx      729 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$4.class
--rw-rw-r--  2.0 unx     2553 b- defN 23-Aug-03 15:40 sklearn/preprocessing/Binarizer.class
--rw-rw-r--  2.0 unx     1054 b- defN 23-Aug-03 15:40 sklearn/preprocessing/EncoderUtil$2.class
--rw-rw-r--  2.0 unx     3595 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MinMaxScaler.class
--rw-rw-r--  2.0 unx     4467 b- defN 23-Aug-03 15:40 sklearn/preprocessing/RobustScaler.class
--rw-rw-r--  2.0 unx     3740 b- defN 23-Aug-03 15:40 sklearn/preprocessing/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      957 b- defN 23-Aug-03 15:40 sklearn/preprocessing/Imputer.class
--rw-rw-r--  2.0 unx     2033 b- defN 23-Aug-03 15:40 sklearn/preprocessing/PolynomialFeatures$1.class
--rw-rw-r--  2.0 unx    10333 b- defN 23-Aug-03 15:40 sklearn/preprocessing/MultiOneHotEncoder.class
--rw-rw-r--  2.0 unx     2153 b- defN 23-Aug-03 15:40 sklearn/tree/TreeClassifier.class
--rw-rw-r--  2.0 unx     3111 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$1.class
--rw-rw-r--  2.0 unx     2664 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$4.class
--rw-rw-r--  2.0 unx     4805 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelFlattener.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelCompactor$1.class
--rw-rw-r--  2.0 unx     5431 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelCompactor.class
--rw-rw-r--  2.0 unx     2988 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelPruner.class
--rw-rw-r--  2.0 unx      739 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelFlattener$1.class
--rw-rw-r--  2.0 unx      730 b- defN 23-Aug-03 15:40 sklearn/tree/visitors/TreeModelPruner$1.class
--rw-rw-r--  2.0 unx      915 b- defN 23-Aug-03 15:40 sklearn/tree/RegressionCriterion.class
--rw-rw-r--  2.0 unx     1151 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$5.class
--rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-03 15:40 sklearn/tree/PresortBestSplitter.class
--rw-rw-r--  2.0 unx     1589 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$6.class
--rw-rw-r--  2.0 unx     1764 b- defN 23-Aug-03 15:40 sklearn/tree/TreeRegressor.class
--rw-rw-r--  2.0 unx     1489 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$7.class
--rw-rw-r--  2.0 unx    19425 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil.class
--rw-rw-r--  2.0 unx     1123 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$3.class
--rw-rw-r--  2.0 unx     1373 b- defN 23-Aug-03 15:40 sklearn/tree/HasTreeOptions.class
--rw-rw-r--  2.0 unx     2293 b- defN 23-Aug-03 15:40 sklearn/tree/Tree.class
--rw-rw-r--  2.0 unx      754 b- defN 23-Aug-03 15:40 sklearn/tree/TreeUtil$2.class
--rw-rw-r--  2.0 unx      150 b- defN 23-Aug-03 15:40 sklearn/tree/HasTree.class
--rw-rw-r--  2.0 unx     1967 b- defN 23-Aug-03 15:40 sklearn/InitializerUtil.class
--rw-rw-r--  2.0 unx      570 b- defN 23-Aug-03 15:40 sklearn/Regressor.class
--rw-rw-r--  2.0 unx      211 b- defN 23-Aug-03 15:40 sklearn/HasNumberOfOutputs.class
--rw-rw-r--  2.0 unx      534 b- defN 23-Aug-03 15:40 sklearn/OutlierDetector.class
--rw-rw-r--  2.0 unx     2808 b- defN 23-Aug-03 15:40 sklearn/Calibrator.class
--rw-rw-r--  2.0 unx      273 b- defN 23-Aug-03 15:40 sklearn/HasClassifierOptions.class
--rw-rw-r--  2.0 unx     7080 b- defN 23-Aug-03 15:40 sklearn/EstimatorUtil.class
--rw-rw-r--  2.0 unx      199 b- defN 23-Aug-03 15:40 sklearn/HasType.class
--rw-rw-r--  2.0 unx      678 b- defN 23-Aug-03 15:40 sklearn/cluster/MiniBatchKMeans.class
--rw-rw-r--  2.0 unx     5086 b- defN 23-Aug-03 15:40 sklearn/cluster/KMeans.class
--rw-rw-r--  2.0 unx    14149 b- defN 23-Aug-03 15:40 sklearn/Estimator.class
--rw-rw-r--  2.0 unx     1624 b- defN 23-Aug-03 15:40 sklearn/Initializer.class
--rw-rw-r--  2.0 unx     4595 b- defN 23-Aug-03 15:40 sklearn/multiclass/OneVsRestClassifier.class
--rw-rw-r--  2.0 unx     5157 b- defN 23-Aug-03 15:40 sklearn2pmml/ruleset/RuleSetClassifier.class
--rw-rw-r--  2.0 unx     1187 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
--rw-rw-r--  2.0 unx      980 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$3.class
--rw-rw-r--  2.0 unx     1023 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$4.class
--rw-rw-r--  2.0 unx    27315 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline.class
--rw-rw-r--  2.0 unx     1421 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$2.class
--rw-rw-r--  2.0 unx     1346 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipeline$1.class
--rw-rw-r--  2.0 unx     1593 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/PMMLPipelineUtil.class
--rw-rw-r--  2.0 unx     1811 b- defN 23-Aug-03 15:40 sklearn2pmml/pipeline/Verification.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/MultiDomain.class
--rw-rw-r--  2.0 unx     1152 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/ContinuousDomainEraser.class
--rw-rw-r--  2.0 unx     1654 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Alias.class
--rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/TemporalDomain.class
--rw-rw-r--  2.0 unx      779 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/ContinuousDomain$1.class
--rw-rw-r--  2.0 unx    11878 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain.class
--rw-rw-r--  2.0 unx     1416 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/MultiAlias.class
--rw-rw-r--  2.0 unx     5055 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DiscreteDomain.class
--rw-rw-r--  2.0 unx     1952 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/CategoricalDomain.class
--rw-rw-r--  2.0 unx     1453 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DomainEraser.class
--rw-rw-r--  2.0 unx      613 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DateTimeDomain.class
--rw-rw-r--  2.0 unx     7764 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/ContinuousDomain.class
--rw-rw-r--  2.0 unx     1077 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DiscreteDomainEraser.class
--rw-rw-r--  2.0 unx     1590 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/TransformerWrapper.class
--rw-rw-r--  2.0 unx     1045 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$2.class
--rw-rw-r--  2.0 unx      596 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DateDomain.class
--rw-rw-r--  2.0 unx     2374 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/DomainUtil.class
--rw-rw-r--  2.0 unx     1033 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$1.class
--rw-rw-r--  2.0 unx     1577 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/OrdinalDomain.class
--rw-rw-r--  2.0 unx      672 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$4.class
--rw-rw-r--  2.0 unx      799 b- defN 23-Aug-03 15:40 sklearn2pmml/decoration/Domain$3.class
--rw-rw-r--  2.0 unx     7879 b- defN 23-Aug-03 15:40 sklearn2pmml/neural_network/MLPTransformer.class
--rw-rw-r--  2.0 unx      391 b- defN 23-Aug-03 15:40 sklearn2pmml/SkLearn2PMMLFields.class
--rw-rw-r--  2.0 unx     1160 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Evaluatable.class
--rw-rw-r--  2.0 unx     1196 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Expression.class
--rw-rw-r--  2.0 unx     1189 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Predicate.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Reshaper.class
--rw-rw-r--  2.0 unx     3392 b- defN 23-Aug-03 15:40 sklearn2pmml/util/EvaluatableUtil.class
--rw-rw-r--  2.0 unx     1658 b- defN 23-Aug-03 15:40 sklearn2pmml/util/Slicer.class
--rw-rw-r--  2.0 unx     2418 b- defN 23-Aug-03 15:40 sklearn2pmml/feature_extraction/text/Splitter.class
--rw-rw-r--  2.0 unx     3184 b- defN 23-Aug-03 15:40 sklearn2pmml/feature_extraction/text/Matcher.class
--rw-rw-r--  2.0 unx     1262 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/SelectFirstRegressor.class
--rw-rw-r--  2.0 unx     2083 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTUtil$2.class
--rw-rw-r--  2.0 unx     1934 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTLMRegressor.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTUtil$1.class
--rw-rw-r--  2.0 unx     7410 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/EstimatorChain.class
--rw-rw-r--  2.0 unx     6582 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTUtil.class
--rw-rw-r--  2.0 unx     3995 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/Link.class
--rw-rw-r--  2.0 unx     4360 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/SelectFirstUtil.class
--rw-rw-r--  2.0 unx     4249 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/GBDTLRClassifier.class
--rw-rw-r--  2.0 unx     2608 b- defN 23-Aug-03 15:40 sklearn2pmml/ensemble/SelectFirstClassifier.class
--rw-rw-r--  2.0 unx     1438 b- defN 23-Aug-03 15:40 sklearn2pmml/EstimatorProxy$1.class
--rw-rw-r--  2.0 unx      946 b- defN 23-Aug-03 15:40 sklearn2pmml/feature_selection/SelectUnique.class
--rw-rw-r--  2.0 unx     6477 b- defN 23-Aug-03 15:40 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
--rw-rw-r--  2.0 unx      791 b- defN 23-Aug-03 15:40 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
--rw-rw-r--  2.0 unx     1197 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PatternTransformer.class
--rw-rw-r--  2.0 unx     2908 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/ReplaceTransformer.class
--rw-rw-r--  2.0 unx     1844 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/WordCountTransformer.class
--rw-rw-r--  2.0 unx      597 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DateTimeFormatter.class
--rw-rw-r--  2.0 unx     1288 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
--rw-rw-r--  2.0 unx     4621 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DurationTransformer.class
--rw-rw-r--  2.0 unx      444 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
--rw-rw-r--  2.0 unx     2777 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/FilterLookupTransformer.class
--rw-rw-r--  2.0 unx     2545 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/Formatter.class
--rw-rw-r--  2.0 unx     3424 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/CastTransformer.class
--rw-rw-r--  2.0 unx     2758 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/MatchesTransformer.class
--rw-rw-r--  2.0 unx      589 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/NumberFormatter.class
--rw-rw-r--  2.0 unx     4149 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/MultiLookupTransformer.class
--rw-rw-r--  2.0 unx     3871 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/StringNormalizer.class
--rw-rw-r--  2.0 unx     7145 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/ExpressionTransformer.class
--rw-rw-r--  2.0 unx      635 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
--rw-rw-r--  2.0 unx     3604 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/DataFrameConstructor.class
--rw-rw-r--  2.0 unx     2847 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/ConcatTransformer.class
--rw-rw-r--  2.0 unx     5993 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/CutTransformer.class
--rw-rw-r--  2.0 unx     7025 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/BSplineTransformer.class
--rw-rw-r--  2.0 unx     6410 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/LookupTransformer.class
--rw-rw-r--  2.0 unx     3236 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/SubstringTransformer.class
--rw-rw-r--  2.0 unx     3181 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
--rw-rw-r--  2.0 unx     2132 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
--rw-rw-r--  2.0 unx     3328 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/Aggregator.class
--rw-rw-r--  2.0 unx      647 b- defN 23-Aug-03 15:40 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
--rw-rw-r--  2.0 unx     1639 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDRegressor.class
--rw-rw-r--  2.0 unx    10719 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDUtil.class
--rw-rw-r--  2.0 unx     2032 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDClassifier.class
--rw-rw-r--  2.0 unx     1417 b- defN 23-Aug-03 15:40 sklearn2pmml/tree/CHAIDUtil$1.class
--rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-03 15:40 sklearn2pmml/EstimatorProxy.class
--rw-rw-r--  2.0 unx     1479 b- defN 23-Aug-03 15:40 sklearn2pmml/SelectorProxy.class
--rw-rw-r--  2.0 unx     2046 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionUtil.class
--rw-rw-r--  2.0 unx     3799 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionRegressor.class
--rw-rw-r--  2.0 unx      990 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionClassifier$1.class
--rw-rw-r--  2.0 unx     8687 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionClassifier.class
--rw-rw-r--  2.0 unx      948 b- defN 23-Aug-03 15:40 sklearn2pmml/expression/ExpressionUtil$1.class
--rw-rw-r--  2.0 unx     1774 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
--rw-rw-r--  2.0 unx     2764 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
--rw-rw-r--  2.0 unx     3549 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
--rw-rw-r--  2.0 unx    15476 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/SkLearnEncoder.class
--rw-rw-r--  2.0 unx      194 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/FieldNames.class
--rw-rw-r--  2.0 unx      171 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/HasSkLearnOptions.class
--rw-rw-r--  2.0 unx     1179 b- defN 23-Aug-03 15:40 org/jpmml/sklearn/SkLearnEncoder$1.class
--rw-rw-r--  2.0 unx     1822 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
--rw-rw-r--  2.0 unx       57 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
-410 files, 933938 bytes uncompressed, 411785 bytes compressed:  55.9%
+Zip file size: 476817 bytes, number of entries: 414
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/
+-rw-r--r--  2.0 unx      159 b- defN 23-Aug-05 19:08 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn_pandas/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 chaid/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 stop_words/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/calibration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/dummy/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/svm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/impute/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/naive_bayes/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/linear_model/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/linear_model/logistic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/linear_model/ridge/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/linear_model/glm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/compose/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/model_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/decomposition/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/neighbors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/multioutput/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/isotonic/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/metrics/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/bagging/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/stacking/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/forest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/iforest/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/voting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/ensemble/weight_boosting/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/loss/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/discriminant_analysis/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/tree/visitors/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/cluster/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn/multiclass/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/ruleset/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/decoration/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/neural_network/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/util/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/feature_extraction/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/feature_extraction/text/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/ensemble/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/feature_selection/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/postprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/preprocessing/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/tree/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 sklearn2pmml/expression/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 org/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 org/jpmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 org/jpmml/sklearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:07 org/jpmml/sklearn/testing/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn/
+-rw-rw-r--  2.0 unx    16829 b- defN 23-Aug-05 19:07 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2287 b- defN 23-Aug-05 19:07 sklearn_pandas/CategoricalImputer.class
+-rw-rw-r--  2.0 unx      656 b- defN 23-Aug-05 19:07 sklearn_pandas/TransformerPipeline.class
+-rw-rw-r--  2.0 unx     1154 b- defN 23-Aug-05 19:07 sklearn_pandas/DataFrameMapper$2.class
+-rw-rw-r--  2.0 unx     6280 b- defN 23-Aug-05 19:07 sklearn_pandas/DataFrameMapper.class
+-rw-rw-r--  2.0 unx     1126 b- defN 23-Aug-05 19:07 sklearn_pandas/DataFrameMapper$1.class
+-rw-rw-r--  2.0 unx      609 b- defN 23-Aug-05 19:07 chaid/ContinuousColumn.class
+-rw-rw-r--  2.0 unx      925 b- defN 23-Aug-05 19:07 chaid/Node.class
+-rw-rw-r--  2.0 unx      467 b- defN 23-Aug-05 19:07 chaid/Column.class
+-rw-rw-r--  2.0 unx     3283 b- defN 23-Aug-05 19:07 chaid/Split.class
+-rw-rw-r--  2.0 unx      401 b- defN 23-Aug-05 19:07 chaid/InvalidSplitReason.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Aug-05 19:07 chaid/NominalColumn.class
+-rw-rw-r--  2.0 unx     1912 b- defN 23-Aug-05 19:07 stop_words/english.txt
+-rw-rw-r--  2.0 unx      147 b- defN 23-Aug-05 19:07 sklearn/HasHead.class
+-rw-rw-r--  2.0 unx     1728 b- defN 23-Aug-05 19:07 sklearn/StepUtil.class
+-rw-rw-r--  2.0 unx    12045 b- defN 23-Aug-05 19:07 sklearn/calibration/CalibratedClassifier.class
+-rw-rw-r--  2.0 unx     2953 b- defN 23-Aug-05 19:07 sklearn/calibration/SigmoidCalibration.class
+-rw-rw-r--  2.0 unx      683 b- defN 23-Aug-05 19:07 sklearn/calibration/CalibratedClassifier$1.class
+-rw-rw-r--  2.0 unx     3672 b- defN 23-Aug-05 19:07 sklearn/calibration/CalibratedClassifierCV.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Aug-05 19:07 sklearn/HasPMMLOptions.class
+-rw-rw-r--  2.0 unx     2216 b- defN 23-Aug-05 19:07 sklearn/VersionUtil.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Aug-05 19:07 sklearn/pipeline/PipelineTransformer.class
+-rw-rw-r--  2.0 unx     1697 b- defN 23-Aug-05 19:07 sklearn/pipeline/Pipeline$2.class
+-rw-rw-r--  2.0 unx     2536 b- defN 23-Aug-05 19:07 sklearn/pipeline/FeatureUnion.class
+-rw-rw-r--  2.0 unx     6463 b- defN 23-Aug-05 19:07 sklearn/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx     2327 b- defN 23-Aug-05 19:07 sklearn/pipeline/PipelineRegressor.class
+-rw-rw-r--  2.0 unx     1742 b- defN 23-Aug-05 19:07 sklearn/pipeline/Pipeline$1.class
+-rw-rw-r--  2.0 unx     1111 b- defN 23-Aug-05 19:07 sklearn/pipeline/PipelineUtil.class
+-rw-rw-r--  2.0 unx     2589 b- defN 23-Aug-05 19:07 sklearn/pipeline/PipelineClassifier.class
+-rw-rw-r--  2.0 unx     2435 b- defN 23-Aug-05 19:07 sklearn/pipeline/PipelineClusterer.class
+-rw-rw-r--  2.0 unx     5027 b- defN 23-Aug-05 19:07 sklearn/dummy/DummyClassifier.class
+-rw-rw-r--  2.0 unx     2174 b- defN 23-Aug-05 19:07 sklearn/dummy/DummyRegressor.class
+-rw-rw-r--  2.0 unx      512 b- defN 23-Aug-05 19:07 sklearn/SkLearnFields.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Aug-05 19:07 sklearn/SkLearnOutlierTransformation.class
+-rw-rw-r--  2.0 unx      240 b- defN 23-Aug-05 19:07 sklearn/HasEstimator.class
+-rw-rw-r--  2.0 unx     3421 b- defN 23-Aug-05 19:07 sklearn/OutlierDetectorUtil.class
+-rw-rw-r--  2.0 unx     1236 b- defN 23-Aug-05 19:07 sklearn/HasMultiApplyField.class
+-rw-rw-r--  2.0 unx     2393 b- defN 23-Aug-05 19:07 sklearn/svm/SupportVectorMachineUtil.class
+-rw-rw-r--  2.0 unx     1109 b- defN 23-Aug-05 19:07 sklearn/svm/LinearSVC.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Aug-05 19:07 sklearn/svm/LibSVMClassifier.class
+-rw-rw-r--  2.0 unx      966 b- defN 23-Aug-05 19:07 sklearn/svm/SupportVectorMachineUtil$1.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Aug-05 19:07 sklearn/svm/OneClassSVM.class
+-rw-rw-r--  2.0 unx     3594 b- defN 23-Aug-05 19:07 sklearn/svm/LibSVMRegressor.class
+-rw-rw-r--  2.0 unx     3007 b- defN 23-Aug-05 19:07 sklearn/InitializerUtil$1.class
+-rw-rw-r--  2.0 unx      735 b- defN 23-Aug-05 19:07 sklearn/Estimator$1.class
+-rw-rw-r--  2.0 unx      342 b- defN 23-Aug-05 19:07 sklearn/HasOutlierField.class
+-rw-rw-r--  2.0 unx      214 b- defN 23-Aug-05 19:07 sklearn/HasNumberOfFeatures.class
+-rw-rw-r--  2.0 unx      660 b- defN 23-Aug-05 19:07 sklearn/MultiTransformer.class
+-rw-rw-r--  2.0 unx     2110 b- defN 23-Aug-05 19:07 sklearn/neural_network/MLPRegressor.class
+-rw-rw-r--  2.0 unx     2555 b- defN 23-Aug-05 19:07 sklearn/neural_network/MLPClassifier.class
+-rw-rw-r--  2.0 unx      759 b- defN 23-Aug-05 19:07 sklearn/neural_network/MultilayerPerceptronUtil$1.class
+-rw-rw-r--  2.0 unx     8927 b- defN 23-Aug-05 19:07 sklearn/neural_network/MultilayerPerceptronUtil.class
+-rw-rw-r--  2.0 unx     1761 b- defN 23-Aug-05 19:07 sklearn/Step.class
+-rw-rw-r--  2.0 unx      168 b- defN 23-Aug-05 19:07 sklearn/HasDefaultValue.class
+-rw-rw-r--  2.0 unx       99 b- defN 23-Aug-05 19:07 sklearn/Proxy.class
+-rw-rw-r--  2.0 unx     2936 b- defN 23-Aug-05 19:07 sklearn/impute/MissingIndicator.class
+-rw-rw-r--  2.0 unx     4027 b- defN 23-Aug-05 19:07 sklearn/impute/ImputerUtil.class
+-rw-rw-r--  2.0 unx     5703 b- defN 23-Aug-05 19:07 sklearn/impute/SimpleImputer.class
+-rw-rw-r--  2.0 unx     6948 b- defN 23-Aug-05 19:07 sklearn/naive_bayes/GaussianNB.class
+-rw-rw-r--  2.0 unx      233 b- defN 23-Aug-05 19:07 sklearn/HasFeatureNamesIn.class
+-rw-rw-r--  2.0 unx     4446 b- defN 23-Aug-05 19:07 sklearn/linear_model/LinearRegressor.class
+-rw-rw-r--  2.0 unx     5037 b- defN 23-Aug-05 19:07 sklearn/linear_model/LinearClassifier.class
+-rw-rw-r--  2.0 unx     7645 b- defN 23-Aug-05 19:07 sklearn/linear_model/logistic/LogisticRegression.class
+-rw-rw-r--  2.0 unx     1042 b- defN 23-Aug-05 19:07 sklearn/linear_model/ridge/RidgeClassifier.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Aug-05 19:07 sklearn/linear_model/glm/DistributionBoundary.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Aug-05 19:07 sklearn/linear_model/glm/GeneralizedLinearRegressor.class
+-rw-rw-r--  2.0 unx      947 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/Hinge.class
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/SGDOneClassSVM.class
+-rw-rw-r--  2.0 unx      461 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/LossFunction.class
+-rw-rw-r--  2.0 unx      452 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/Log.class
+-rw-rw-r--  2.0 unx     1165 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/SGDClassifier.class
+-rw-rw-r--  2.0 unx      482 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/ModifiedHuber.class
+-rw-rw-r--  2.0 unx      968 b- defN 23-Aug-05 19:07 sklearn/linear_model/stochastic_gradient/SquaredHinge.class
+-rw-rw-r--  2.0 unx     1746 b- defN 23-Aug-05 19:07 sklearn/compose/ColumnTransformer$1.class
+-rw-rw-r--  2.0 unx     3239 b- defN 23-Aug-05 19:07 sklearn/compose/TransformedTargetRegressor.class
+-rw-rw-r--  2.0 unx     3649 b- defN 23-Aug-05 19:07 sklearn/compose/ColumnTransformer.class
+-rw-rw-r--  2.0 unx     1534 b- defN 23-Aug-05 19:07 sklearn/compose/TransformedTargetRegressor$1.class
+-rw-rw-r--  2.0 unx      894 b- defN 23-Aug-05 19:07 sklearn/IdentityTransformer.class
+-rw-rw-r--  2.0 unx     4089 b- defN 23-Aug-05 19:07 sklearn/Classifier.class
+-rw-rw-r--  2.0 unx     1457 b- defN 23-Aug-05 19:07 sklearn/model_selection/EstimatorSearcher.class
+-rw-rw-r--  2.0 unx     1685 b- defN 23-Aug-05 19:07 sklearn/Selector.class
+-rw-rw-r--  2.0 unx      419 b- defN 23-Aug-05 19:07 sklearn/decomposition/IncrementalPCA.class
+-rw-rw-r--  2.0 unx     3471 b- defN 23-Aug-05 19:07 sklearn/decomposition/TruncatedSVD.class
+-rw-rw-r--  2.0 unx     4759 b- defN 23-Aug-05 19:07 sklearn/decomposition/PCA.class
+-rw-rw-r--  2.0 unx      911 b- defN 23-Aug-05 19:07 sklearn/decomposition/BasePCA.class
+-rw-rw-r--  2.0 unx      336 b- defN 23-Aug-05 19:07 sklearn/HasPredictField.class
+-rw-rw-r--  2.0 unx     3018 b- defN 23-Aug-05 19:07 sklearn/neighbors/NearestNeighbors.class
+-rw-rw-r--  2.0 unx     4505 b- defN 23-Aug-05 19:07 sklearn/neighbors/KNeighborsClassifier.class
+-rw-rw-r--  2.0 unx     3794 b- defN 23-Aug-05 19:07 sklearn/neighbors/NearestCentroid.class
+-rw-rw-r--  2.0 unx     2061 b- defN 23-Aug-05 19:07 sklearn/neighbors/BinaryTree.class
+-rw-rw-r--  2.0 unx     1266 b- defN 23-Aug-05 19:07 sklearn/neighbors/KNeighborsUtil$1.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Aug-05 19:07 sklearn/neighbors/HasMetric.class
+-rw-rw-r--  2.0 unx    10745 b- defN 23-Aug-05 19:07 sklearn/neighbors/KNeighborsUtil.class
+-rw-rw-r--  2.0 unx     4387 b- defN 23-Aug-05 19:07 sklearn/neighbors/KNeighborsRegressor.class
+-rw-rw-r--  2.0 unx     1068 b- defN 23-Aug-05 19:07 sklearn/neighbors/DistanceMetric.class
+-rw-rw-r--  2.0 unx      351 b- defN 23-Aug-05 19:07 sklearn/neighbors/HasTrainingData.class
+-rw-rw-r--  2.0 unx      176 b- defN 23-Aug-05 19:07 sklearn/neighbors/HasNumberOfNeighbors.class
+-rw-rw-r--  2.0 unx     2666 b- defN 23-Aug-05 19:07 sklearn/multioutput/MultiOutputUtil.class
+-rw-rw-r--  2.0 unx     3522 b- defN 23-Aug-05 19:07 sklearn/multioutput/ChainUtil.class
+-rw-rw-r--  2.0 unx     1601 b- defN 23-Aug-05 19:07 sklearn/multioutput/RegressorChain.class
+-rw-rw-r--  2.0 unx     1316 b- defN 23-Aug-05 19:07 sklearn/multioutput/MultiOutputClassifier.class
+-rw-rw-r--  2.0 unx     1310 b- defN 23-Aug-05 19:07 sklearn/multioutput/MultiOutputRegressor.class
+-rw-rw-r--  2.0 unx     1745 b- defN 23-Aug-05 19:07 sklearn/multioutput/ClassifierChain.class
+-rw-rw-r--  2.0 unx     4450 b- defN 23-Aug-05 19:07 sklearn/isotonic/IsotonicRegression.class
+-rw-rw-r--  2.0 unx      326 b- defN 23-Aug-05 19:07 sklearn/HasApplyField.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Aug-05 19:07 sklearn/HasEstimatorEnsemble.class
+-rw-rw-r--  2.0 unx     2094 b- defN 23-Aug-05 19:07 sklearn/Transformer$1.class
+-rw-rw-r--  2.0 unx      953 b- defN 23-Aug-05 19:07 sklearn/LabelEncoderClassifier.class
+-rw-rw-r--  2.0 unx      451 b- defN 23-Aug-05 19:07 sklearn/PassThrough.class
+-rw-rw-r--  2.0 unx      181 b- defN 23-Aug-05 19:07 sklearn/HasPriorProbability.class
+-rw-rw-r--  2.0 unx      230 b- defN 23-Aug-05 19:07 sklearn/SkLearnSteps.class
+-rw-rw-r--  2.0 unx     5693 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/text/TfidfVectorizer.class
+-rw-rw-r--  2.0 unx      809 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/text/TfidfVectorizer$1.class
+-rw-rw-r--  2.0 unx      675 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/text/Tokenizer.class
+-rw-rw-r--  2.0 unx    13329 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/text/CountVectorizer.class
+-rw-rw-r--  2.0 unx     2129 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/text/CountVectorizer$1.class
+-rw-rw-r--  2.0 unx     1433 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/text/TfidfTransformer.class
+-rw-rw-r--  2.0 unx     4030 b- defN 23-Aug-05 19:07 sklearn/feature_extraction/DictVectorizer.class
+-rw-rw-r--  2.0 unx      762 b- defN 23-Aug-05 19:07 sklearn/Clusterer.class
+-rw-rw-r--  2.0 unx     1411 b- defN 23-Aug-05 19:07 sklearn/metrics/DistanceMetric.class
+-rw-rw-r--  2.0 unx     1069 b- defN 23-Aug-05 19:07 sklearn/ensemble/EnsembleUtil.class
+-rw-rw-r--  2.0 unx     2112 b- defN 23-Aug-05 19:07 sklearn/ensemble/bagging/BaggingRegressor.class
+-rw-rw-r--  2.0 unx     3293 b- defN 23-Aug-05 19:07 sklearn/ensemble/bagging/BaggingUtil.class
+-rw-rw-r--  2.0 unx     3031 b- defN 23-Aug-05 19:07 sklearn/ensemble/bagging/BaggingClassifier.class
+-rw-rw-r--  2.0 unx     1409 b- defN 23-Aug-05 19:07 sklearn/ensemble/EnsembleRegressor.class
+-rw-rw-r--  2.0 unx     3485 b- defN 23-Aug-05 19:07 sklearn/ensemble/stacking/StackingClassifier.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Aug-05 19:07 sklearn/ensemble/stacking/StackingUtil$PredictFunction.class
+-rw-rw-r--  2.0 unx     3109 b- defN 23-Aug-05 19:07 sklearn/ensemble/stacking/StackingRegressor.class
+-rw-rw-r--  2.0 unx     3862 b- defN 23-Aug-05 19:07 sklearn/ensemble/stacking/StackingUtil.class
+-rw-rw-r--  2.0 unx     2524 b- defN 23-Aug-05 19:07 sklearn/ensemble/stacking/StackingClassifier$1.class
+-rw-rw-r--  2.0 unx     2254 b- defN 23-Aug-05 19:07 sklearn/ensemble/stacking/StackingRegressor$1.class
+-rw-rw-r--  2.0 unx      495 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/ScaledLogOddsEstimator.class
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$GradientBoostingClassifierProxy.class
+-rw-rw-r--  2.0 unx     1862 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/MultinomialDeviance.class
+-rw-rw-r--  2.0 unx     2563 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/GradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx      858 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/LossFunction.class
+-rw-rw-r--  2.0 unx     1588 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/ExponentialLoss.class
+-rw-rw-r--  2.0 unx     1317 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/PriorProbabilityEstimator.class
+-rw-rw-r--  2.0 unx     7945 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/LogOddsEstimator.class
+-rw-rw-r--  2.0 unx      960 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/MeanEstimator.class
+-rw-rw-r--  2.0 unx     1265 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/GradientBoostingClassifier$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/QuantileEstimator.class
+-rw-rw-r--  2.0 unx     1578 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/BinomialDeviance.class
+-rw-rw-r--  2.0 unx      811 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/ZeroEstimator.class
+-rw-rw-r--  2.0 unx     3003 b- defN 23-Aug-05 19:07 sklearn/ensemble/gradient_boosting/GradientBoostingUtil.class
+-rw-rw-r--  2.0 unx     1148 b- defN 23-Aug-05 19:07 sklearn/ensemble/EnsembleUtil$1.class
+-rw-rw-r--  2.0 unx     3059 b- defN 23-Aug-05 19:07 sklearn/ensemble/forest/ForestUtil.class
+-rw-rw-r--  2.0 unx     2528 b- defN 23-Aug-05 19:07 sklearn/ensemble/forest/ForestRegressor.class
+-rw-rw-r--  2.0 unx     2987 b- defN 23-Aug-05 19:07 sklearn/ensemble/forest/ForestClassifier.class
+-rw-rw-r--  2.0 unx     1752 b- defN 23-Aug-05 19:07 sklearn/ensemble/iforest/IsolationForest$3.class
+-rw-rw-r--  2.0 unx     2206 b- defN 23-Aug-05 19:07 sklearn/ensemble/iforest/IsolationForest$1.class
+-rw-rw-r--  2.0 unx     1716 b- defN 23-Aug-05 19:07 sklearn/ensemble/iforest/IsolationForest$2.class
+-rw-rw-r--  2.0 unx     8225 b- defN 23-Aug-05 19:07 sklearn/ensemble/iforest/IsolationForest.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Aug-05 19:07 sklearn/ensemble/voting/VotingClassifier.class
+-rw-rw-r--  2.0 unx     3716 b- defN 23-Aug-05 19:07 sklearn/ensemble/voting/VotingRegressor.class
+-rw-rw-r--  2.0 unx     2814 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingRegressor.class
+-rw-rw-r--  2.0 unx     1247 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/BinMapper$1.class
+-rw-rw-r--  2.0 unx     3041 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/TreePredictor.class
+-rw-rw-r--  2.0 unx     6152 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingUtil.class
+-rw-rw-r--  2.0 unx      505 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/CategoricalCrossEntropy.class
+-rw-rw-r--  2.0 unx      490 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/BinaryCrossEntropy.class
+-rw-rw-r--  2.0 unx     1572 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/BinMapper.class
+-rw-rw-r--  2.0 unx     6374 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/HistGradientBoostingClassifier.class
+-rw-rw-r--  2.0 unx     8868 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/TreePredictorUtil.class
+-rw-rw-r--  2.0 unx      441 b- defN 23-Aug-05 19:07 sklearn/ensemble/hist_gradient_boosting/BaseLoss.class
+-rw-rw-r--  2.0 unx     1418 b- defN 23-Aug-05 19:07 sklearn/ensemble/EnsembleClassifier.class
+-rw-rw-r--  2.0 unx     3564 b- defN 23-Aug-05 19:07 sklearn/ensemble/weight_boosting/AdaBoostRegressor.class
+-rw-rw-r--  2.0 unx     6362 b- defN 23-Aug-05 19:07 sklearn/Transformer.class
+-rw-rw-r--  2.0 unx      859 b- defN 23-Aug-05 19:07 sklearn/Transformer$1$1.class
+-rw-rw-r--  2.0 unx      981 b- defN 23-Aug-05 19:07 sklearn/Drop.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-05 19:07 sklearn/feature_selection/SelectKBest$Entry.class
+-rw-rw-r--  2.0 unx     3486 b- defN 23-Aug-05 19:07 sklearn/feature_selection/SelectFromModel.class
+-rw-rw-r--  2.0 unx     2922 b- defN 23-Aug-05 19:07 sklearn/feature_selection/SelectKBest.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Aug-05 19:07 sklearn/feature_selection/PySelector.class
+-rw-rw-r--  2.0 unx      607 b- defN 23-Aug-05 19:07 sklearn/Transformer$2.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Aug-05 19:07 sklearn/loss/HalfMultinomialLoss.class
+-rw-rw-r--  2.0 unx      602 b- defN 23-Aug-05 19:07 sklearn/loss/CyLossFunction.class
+-rw-rw-r--  2.0 unx      403 b- defN 23-Aug-05 19:07 sklearn/loss/HalfBinomialLoss.class
+-rw-rw-r--  2.0 unx      387 b- defN 23-Aug-05 19:07 sklearn/loss/BaseLoss.class
+-rw-rw-r--  2.0 unx      381 b- defN 23-Aug-05 19:07 sklearn/HasDecisionFunctionField.class
+-rw-rw-r--  2.0 unx      338 b- defN 23-Aug-05 19:07 sklearn/SkLearnMethods.class
+-rw-rw-r--  2.0 unx     1515 b- defN 23-Aug-05 19:07 sklearn/OutlierDetectorUtil$1.class
+-rw-rw-r--  2.0 unx      195 b- defN 23-Aug-05 19:07 sklearn/HasClasses.class
+-rw-rw-r--  2.0 unx     4682 b- defN 23-Aug-05 19:07 sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class
+-rw-rw-r--  2.0 unx      696 b- defN 23-Aug-05 19:07 sklearn/EstimatorUtil$1.class
+-rw-rw-r--  2.0 unx     3817 b- defN 23-Aug-05 19:07 sklearn/Composite.class
+-rw-rw-r--  2.0 unx     1194 b- defN 23-Aug-05 19:07 sklearn/preprocessing/KBinsDiscretizer$1.class
+-rw-rw-r--  2.0 unx     4567 b- defN 23-Aug-05 19:07 sklearn/preprocessing/PowerTransformer.class
+-rw-rw-r--  2.0 unx     2381 b- defN 23-Aug-05 19:07 sklearn/preprocessing/LabelEncoder.class
+-rw-rw-r--  2.0 unx     4924 b- defN 23-Aug-05 19:07 sklearn/preprocessing/LabelBinarizer.class
+-rw-rw-r--  2.0 unx     1158 b- defN 23-Aug-05 19:07 sklearn/preprocessing/EncoderUtil$3.class
+-rw-rw-r--  2.0 unx      389 b- defN 23-Aug-05 19:07 sklearn/preprocessing/Scaler.class
+-rw-rw-r--  2.0 unx      797 b- defN 23-Aug-05 19:07 sklearn/preprocessing/MultiOneHotEncoder$1.class
+-rw-rw-r--  2.0 unx     3242 b- defN 23-Aug-05 19:07 sklearn/preprocessing/MaxAbsScaler.class
+-rw-rw-r--  2.0 unx     2948 b- defN 23-Aug-05 19:07 sklearn/preprocessing/FunctionTransformer.class
+-rw-rw-r--  2.0 unx     3291 b- defN 23-Aug-05 19:07 sklearn/preprocessing/BaseEncoder.class
+-rw-rw-r--  2.0 unx     1270 b- defN 23-Aug-05 19:07 sklearn/preprocessing/EncoderUtil$1.class
+-rw-rw-r--  2.0 unx     4549 b- defN 23-Aug-05 19:07 sklearn/preprocessing/StandardScaler.class
+-rw-rw-r--  2.0 unx     9005 b- defN 23-Aug-05 19:07 sklearn/preprocessing/EncoderUtil.class
+-rw-rw-r--  2.0 unx     6343 b- defN 23-Aug-05 19:07 sklearn/preprocessing/PolynomialFeatures.class
+-rw-rw-r--  2.0 unx     8486 b- defN 23-Aug-05 19:07 sklearn/preprocessing/KBinsDiscretizer.class
+-rw-rw-r--  2.0 unx     4671 b- defN 23-Aug-05 19:07 sklearn/preprocessing/OneHotEncoder.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Aug-05 19:07 sklearn/preprocessing/EncoderUtil$4.class
+-rw-rw-r--  2.0 unx     2553 b- defN 23-Aug-05 19:07 sklearn/preprocessing/Binarizer.class
+-rw-rw-r--  2.0 unx     1054 b- defN 23-Aug-05 19:07 sklearn/preprocessing/EncoderUtil$2.class
+-rw-rw-r--  2.0 unx     3595 b- defN 23-Aug-05 19:07 sklearn/preprocessing/MinMaxScaler.class
+-rw-rw-r--  2.0 unx     4467 b- defN 23-Aug-05 19:07 sklearn/preprocessing/RobustScaler.class
+-rw-rw-r--  2.0 unx     3740 b- defN 23-Aug-05 19:07 sklearn/preprocessing/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      957 b- defN 23-Aug-05 19:07 sklearn/preprocessing/Imputer.class
+-rw-rw-r--  2.0 unx     2033 b- defN 23-Aug-05 19:07 sklearn/preprocessing/PolynomialFeatures$1.class
+-rw-rw-r--  2.0 unx    10333 b- defN 23-Aug-05 19:07 sklearn/preprocessing/MultiOneHotEncoder.class
+-rw-rw-r--  2.0 unx     2153 b- defN 23-Aug-05 19:07 sklearn/tree/TreeClassifier.class
+-rw-rw-r--  2.0 unx     3111 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$1.class
+-rw-rw-r--  2.0 unx     2664 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$4.class
+-rw-rw-r--  2.0 unx     4805 b- defN 23-Aug-05 19:07 sklearn/tree/visitors/TreeModelFlattener.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Aug-05 19:07 sklearn/tree/visitors/TreeModelCompactor$1.class
+-rw-rw-r--  2.0 unx     5431 b- defN 23-Aug-05 19:07 sklearn/tree/visitors/TreeModelCompactor.class
+-rw-rw-r--  2.0 unx     2988 b- defN 23-Aug-05 19:07 sklearn/tree/visitors/TreeModelPruner.class
+-rw-rw-r--  2.0 unx      739 b- defN 23-Aug-05 19:07 sklearn/tree/visitors/TreeModelFlattener$1.class
+-rw-rw-r--  2.0 unx      730 b- defN 23-Aug-05 19:07 sklearn/tree/visitors/TreeModelPruner$1.class
+-rw-rw-r--  2.0 unx      915 b- defN 23-Aug-05 19:07 sklearn/tree/RegressionCriterion.class
+-rw-rw-r--  2.0 unx     1151 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$5.class
+-rw-rw-r--  2.0 unx     1014 b- defN 23-Aug-05 19:07 sklearn/tree/PresortBestSplitter.class
+-rw-rw-r--  2.0 unx     1589 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$6.class
+-rw-rw-r--  2.0 unx     1764 b- defN 23-Aug-05 19:07 sklearn/tree/TreeRegressor.class
+-rw-rw-r--  2.0 unx     1489 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$7.class
+-rw-rw-r--  2.0 unx    19425 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil.class
+-rw-rw-r--  2.0 unx     1123 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$3.class
+-rw-rw-r--  2.0 unx     1373 b- defN 23-Aug-05 19:07 sklearn/tree/HasTreeOptions.class
+-rw-rw-r--  2.0 unx     2293 b- defN 23-Aug-05 19:07 sklearn/tree/Tree.class
+-rw-rw-r--  2.0 unx      754 b- defN 23-Aug-05 19:07 sklearn/tree/TreeUtil$2.class
+-rw-rw-r--  2.0 unx      150 b- defN 23-Aug-05 19:07 sklearn/tree/HasTree.class
+-rw-rw-r--  2.0 unx     1967 b- defN 23-Aug-05 19:07 sklearn/InitializerUtil.class
+-rw-rw-r--  2.0 unx      570 b- defN 23-Aug-05 19:07 sklearn/Regressor.class
+-rw-rw-r--  2.0 unx      211 b- defN 23-Aug-05 19:07 sklearn/HasNumberOfOutputs.class
+-rw-rw-r--  2.0 unx      534 b- defN 23-Aug-05 19:07 sklearn/OutlierDetector.class
+-rw-rw-r--  2.0 unx     2808 b- defN 23-Aug-05 19:07 sklearn/Calibrator.class
+-rw-rw-r--  2.0 unx      273 b- defN 23-Aug-05 19:07 sklearn/HasClassifierOptions.class
+-rw-rw-r--  2.0 unx     7080 b- defN 23-Aug-05 19:07 sklearn/EstimatorUtil.class
+-rw-rw-r--  2.0 unx      199 b- defN 23-Aug-05 19:07 sklearn/HasType.class
+-rw-rw-r--  2.0 unx      678 b- defN 23-Aug-05 19:07 sklearn/cluster/MiniBatchKMeans.class
+-rw-rw-r--  2.0 unx     5086 b- defN 23-Aug-05 19:07 sklearn/cluster/KMeans.class
+-rw-rw-r--  2.0 unx    14377 b- defN 23-Aug-05 19:07 sklearn/Estimator.class
+-rw-rw-r--  2.0 unx     1624 b- defN 23-Aug-05 19:07 sklearn/Initializer.class
+-rw-rw-r--  2.0 unx     4595 b- defN 23-Aug-05 19:07 sklearn/multiclass/OneVsRestClassifier.class
+-rw-rw-r--  2.0 unx     5157 b- defN 23-Aug-05 19:07 sklearn2pmml/ruleset/RuleSetClassifier.class
+-rw-rw-r--  2.0 unx     1187 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipelineUtil$1.class
+-rw-rw-r--  2.0 unx      980 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipeline$3.class
+-rw-rw-r--  2.0 unx     1023 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipeline$4.class
+-rw-rw-r--  2.0 unx    27427 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipeline.class
+-rw-rw-r--  2.0 unx     1421 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipeline$2.class
+-rw-rw-r--  2.0 unx     1346 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipeline$1.class
+-rw-rw-r--  2.0 unx     1593 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/PMMLPipelineUtil.class
+-rw-rw-r--  2.0 unx     1811 b- defN 23-Aug-05 19:07 sklearn2pmml/pipeline/Verification.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/MultiDomain.class
+-rw-rw-r--  2.0 unx     1152 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/ContinuousDomainEraser.class
+-rw-rw-r--  2.0 unx     1654 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/Alias.class
+-rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/TemporalDomain.class
+-rw-rw-r--  2.0 unx      779 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/ContinuousDomain$1.class
+-rw-rw-r--  2.0 unx    11878 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/Domain.class
+-rw-rw-r--  2.0 unx     1416 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/MultiAlias.class
+-rw-rw-r--  2.0 unx     5055 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/DiscreteDomain.class
+-rw-rw-r--  2.0 unx     1952 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/CategoricalDomain.class
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/DomainEraser.class
+-rw-rw-r--  2.0 unx      613 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/DateTimeDomain.class
+-rw-rw-r--  2.0 unx     7764 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/ContinuousDomain.class
+-rw-rw-r--  2.0 unx     1077 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/DiscreteDomainEraser.class
+-rw-rw-r--  2.0 unx     1590 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     1045 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/Domain$2.class
+-rw-rw-r--  2.0 unx      596 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/DateDomain.class
+-rw-rw-r--  2.0 unx     2374 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/DomainUtil.class
+-rw-rw-r--  2.0 unx     1033 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/Domain$1.class
+-rw-rw-r--  2.0 unx     1577 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/OrdinalDomain.class
+-rw-rw-r--  2.0 unx      672 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/Domain$4.class
+-rw-rw-r--  2.0 unx      799 b- defN 23-Aug-05 19:07 sklearn2pmml/decoration/Domain$3.class
+-rw-rw-r--  2.0 unx     7879 b- defN 23-Aug-05 19:07 sklearn2pmml/neural_network/MLPTransformer.class
+-rw-rw-r--  2.0 unx      391 b- defN 23-Aug-05 19:07 sklearn2pmml/SkLearn2PMMLFields.class
+-rw-rw-r--  2.0 unx     1160 b- defN 23-Aug-05 19:07 sklearn2pmml/util/Evaluatable.class
+-rw-rw-r--  2.0 unx     1196 b- defN 23-Aug-05 19:07 sklearn2pmml/util/Expression.class
+-rw-rw-r--  2.0 unx     1189 b- defN 23-Aug-05 19:07 sklearn2pmml/util/Predicate.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Aug-05 19:07 sklearn2pmml/util/Reshaper.class
+-rw-rw-r--  2.0 unx     3392 b- defN 23-Aug-05 19:07 sklearn2pmml/util/EvaluatableUtil.class
+-rw-rw-r--  2.0 unx     1658 b- defN 23-Aug-05 19:07 sklearn2pmml/util/Slicer.class
+-rw-rw-r--  2.0 unx     2418 b- defN 23-Aug-05 19:07 sklearn2pmml/feature_extraction/text/Splitter.class
+-rw-rw-r--  2.0 unx     3184 b- defN 23-Aug-05 19:07 sklearn2pmml/feature_extraction/text/Matcher.class
+-rw-rw-r--  2.0 unx     1262 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/SelectFirstRegressor.class
+-rw-rw-r--  2.0 unx     2083 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/GBDTUtil$2.class
+-rw-rw-r--  2.0 unx     1934 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/GBDTLMRegressor.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/GBDTUtil$1.class
+-rw-rw-r--  2.0 unx     7410 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/EstimatorChain.class
+-rw-rw-r--  2.0 unx     6582 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/GBDTUtil.class
+-rw-rw-r--  2.0 unx     3995 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/Link.class
+-rw-rw-r--  2.0 unx     4360 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/SelectFirstUtil.class
+-rw-rw-r--  2.0 unx     4249 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/GBDTLRClassifier.class
+-rw-rw-r--  2.0 unx     2608 b- defN 23-Aug-05 19:07 sklearn2pmml/ensemble/SelectFirstClassifier.class
+-rw-rw-r--  2.0 unx     1438 b- defN 23-Aug-05 19:07 sklearn2pmml/EstimatorProxy$1.class
+-rw-rw-r--  2.0 unx      946 b- defN 23-Aug-05 19:07 sklearn2pmml/feature_selection/SelectUnique.class
+-rw-rw-r--  2.0 unx     6477 b- defN 23-Aug-05 19:07 sklearn2pmml/postprocessing/BusinessDecisionTransformer.class
+-rw-rw-r--  2.0 unx      791 b- defN 23-Aug-05 19:07 sklearn2pmml/postprocessing/BusinessDecisionTransformer$1.class
+-rw-rw-r--  2.0 unx     1197 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/PatternTransformer.class
+-rw-rw-r--  2.0 unx     2908 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/ReplaceTransformer.class
+-rw-rw-r--  2.0 unx     1844 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/WordCountTransformer.class
+-rw-rw-r--  2.0 unx      597 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/DateTimeFormatter.class
+-rw-rw-r--  2.0 unx     1288 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/PMMLLabelBinarizer.class
+-rw-rw-r--  2.0 unx     4621 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/DurationTransformer.class
+-rw-rw-r--  2.0 unx      444 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/PMMLLabelEncoder.class
+-rw-rw-r--  2.0 unx     2777 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/FilterLookupTransformer.class
+-rw-rw-r--  2.0 unx     2545 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/Formatter.class
+-rw-rw-r--  2.0 unx     3424 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/CastTransformer.class
+-rw-rw-r--  2.0 unx     2758 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/MatchesTransformer.class
+-rw-rw-r--  2.0 unx      589 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/NumberFormatter.class
+-rw-rw-r--  2.0 unx     4149 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/MultiLookupTransformer.class
+-rw-rw-r--  2.0 unx     3871 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/StringNormalizer.class
+-rw-rw-r--  2.0 unx     7145 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/ExpressionTransformer.class
+-rw-rw-r--  2.0 unx      635 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/DaysSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     3604 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/DataFrameConstructor.class
+-rw-rw-r--  2.0 unx     2847 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/ConcatTransformer.class
+-rw-rw-r--  2.0 unx     5993 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/CutTransformer.class
+-rw-rw-r--  2.0 unx     7025 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/BSplineTransformer.class
+-rw-rw-r--  2.0 unx     6410 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/LookupTransformer.class
+-rw-rw-r--  2.0 unx     3236 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/SubstringTransformer.class
+-rw-rw-r--  2.0 unx     3181 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/SecondsSinceMidnightTransformer.class
+-rw-rw-r--  2.0 unx     2132 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/PowerFunctionTransformer.class
+-rw-rw-r--  2.0 unx     3328 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/Aggregator.class
+-rw-rw-r--  2.0 unx      647 b- defN 23-Aug-05 19:07 sklearn2pmml/preprocessing/SecondsSinceYearTransformer.class
+-rw-rw-r--  2.0 unx     1639 b- defN 23-Aug-05 19:07 sklearn2pmml/tree/CHAIDRegressor.class
+-rw-rw-r--  2.0 unx    10719 b- defN 23-Aug-05 19:07 sklearn2pmml/tree/CHAIDUtil.class
+-rw-rw-r--  2.0 unx     2032 b- defN 23-Aug-05 19:07 sklearn2pmml/tree/CHAIDClassifier.class
+-rw-rw-r--  2.0 unx     1417 b- defN 23-Aug-05 19:07 sklearn2pmml/tree/CHAIDUtil$1.class
+-rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-05 19:07 sklearn2pmml/EstimatorProxy.class
+-rw-rw-r--  2.0 unx     1479 b- defN 23-Aug-05 19:07 sklearn2pmml/SelectorProxy.class
+-rw-rw-r--  2.0 unx     2046 b- defN 23-Aug-05 19:07 sklearn2pmml/expression/ExpressionUtil.class
+-rw-rw-r--  2.0 unx     3799 b- defN 23-Aug-05 19:07 sklearn2pmml/expression/ExpressionRegressor.class
+-rw-rw-r--  2.0 unx      990 b- defN 23-Aug-05 19:07 sklearn2pmml/expression/ExpressionClassifier$1.class
+-rw-rw-r--  2.0 unx     8687 b- defN 23-Aug-05 19:07 sklearn2pmml/expression/ExpressionClassifier.class
+-rw-rw-r--  2.0 unx      948 b- defN 23-Aug-05 19:07 sklearn2pmml/expression/ExpressionUtil$1.class
+-rw-rw-r--  2.0 unx      162 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/Encodable.class
+-rw-rw-r--  2.0 unx     1774 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
+-rw-rw-r--  2.0 unx     2902 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
+-rw-rw-r--  2.0 unx     3549 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
+-rw-rw-r--  2.0 unx    15476 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/SkLearnEncoder.class
+-rw-rw-r--  2.0 unx      729 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/EncodableUtil.class
+-rw-rw-r--  2.0 unx      194 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/FieldNames.class
+-rw-rw-r--  2.0 unx      171 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/HasSkLearnOptions.class
+-rw-rw-r--  2.0 unx      664 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/SkLearnUtil.class
+-rw-rw-r--  2.0 unx     1179 b- defN 23-Aug-05 19:07 org/jpmml/sklearn/SkLearnEncoder$1.class
+-rw-rw-r--  2.0 unx     1822 b- defN 23-Aug-05 19:07 META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
+-rw-rw-r--  2.0 unx       57 b- defN 23-Aug-05 19:07 META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
+414 files, 937224 bytes uncompressed, 413337 bytes compressed:  55.9%
```

#### zipnote «TEMP»/diffoscope_y9tsz13i_/tmpwisa9iil_.zip

```diff
@@ -246,14 +246,20 @@
 
 Filename: sklearn/calibration/CalibratedClassifier$1.class
 Comment: 
 
 Filename: sklearn/calibration/CalibratedClassifierCV.class
 Comment: 
 
+Filename: sklearn/HasPMMLOptions.class
+Comment: 
+
+Filename: sklearn/VersionUtil.class
+Comment: 
+
 Filename: sklearn/pipeline/PipelineTransformer.class
 Comment: 
 
 Filename: sklearn/pipeline/Pipeline$2.class
 Comment: 
 
 Filename: sklearn/pipeline/FeatureUnion.class
@@ -711,17 +717,14 @@
 
 Filename: sklearn/feature_selection/PySelector.class
 Comment: 
 
 Filename: sklearn/Transformer$2.class
 Comment: 
 
-Filename: sklearn/SkLearnUtil.class
-Comment: 
-
 Filename: sklearn/loss/HalfMultinomialLoss.class
 Comment: 
 
 Filename: sklearn/loss/CyLossFunction.class
 Comment: 
 
 Filename: sklearn/loss/HalfBinomialLoss.class
@@ -1197,32 +1200,41 @@
 
 Filename: sklearn2pmml/expression/ExpressionClassifier.class
 Comment: 
 
 Filename: sklearn2pmml/expression/ExpressionUtil$1.class
 Comment: 
 
+Filename: org/jpmml/sklearn/Encodable.class
+Comment: 
+
 Filename: org/jpmml/sklearn/testing/SkLearnEncoderBatchTest$1.class
 Comment: 
 
 Filename: org/jpmml/sklearn/testing/SkLearnEncoderBatch.class
 Comment: 
 
 Filename: org/jpmml/sklearn/testing/SkLearnEncoderBatchTest.class
 Comment: 
 
 Filename: org/jpmml/sklearn/SkLearnEncoder.class
 Comment: 
 
+Filename: org/jpmml/sklearn/EncodableUtil.class
+Comment: 
+
 Filename: org/jpmml/sklearn/FieldNames.class
 Comment: 
 
 Filename: org/jpmml/sklearn/HasSkLearnOptions.class
 Comment: 
 
+Filename: org/jpmml/sklearn/SkLearnUtil.class
+Comment: 
+
 Filename: org/jpmml/sklearn/SkLearnEncoder$1.class
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-sklearn/pom.xml
 Comment: 
 
 Filename: META-INF/maven/org.jpmml/pmml-sklearn/pom.properties
```

#### META-INF/MANIFEST.MF

```diff
@@ -1,6 +1,6 @@
 Manifest-Version: 1.0
 Implementation-Title: JPMML-SkLearn library
-Implementation-Version: 1.7.34
+Implementation-Version: 1.7.35
 Build-Jdk-Spec: 1.8
 Created-By: Maven JAR Plugin 3.3.0
```

#### sklearn/pipeline/Pipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3c4fe13554c603f6527e4d65f5043d460f481e2cfe6e497e090218b4cf4a9c84
+  SHA-256 checksum 676f3f723b4f956820fa3bdd348f4bb6ce13f028fd733ea73f67e24f9e7ced6e
   Compiled from "Pipeline.java"
 class sklearn.pipeline.Pipeline$2 extends org.jpmml.python.CastFunction<E>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #16                         // sklearn/pipeline/Pipeline$2
   super_class: #17                        // org/jpmml/python/CastFunction
@@ -102,15 +102,15 @@
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/pipeline/Pipeline;
          5: aload_0
          6: aload_2
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 134: 0
+        line 136: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn/pipeline/Pipeline$2;
             0      11     1 this$0   Lsklearn/pipeline/Pipeline;
             0      11     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -129,17 +129,17 @@
         10: areturn
         11: aload_0
         12: aload_1
         13: invokespecial #6                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         16: checkcast     #7                  // class sklearn/Estimator
         19: areturn
       LineNumberTable:
-        line 139: 0
-        line 140: 9
-        line 143: 11
+        line 141: 0
+        line 142: 9
+        line 145: 11
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      20     0  this   Lsklearn/pipeline/Pipeline$2;
             0      20     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 11 /* same */
     Signature: #38                          // (Ljava/lang/Object;)TE;
@@ -158,15 +158,15 @@
         13: invokestatic  #12                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
         16: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         19: ldc           #13                 // String ) is not a supported Estimator
         21: invokevirtual #11                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         24: invokevirtual #14                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         27: areturn
       LineNumberTable:
-        line 148: 0
+        line 150: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lsklearn/pipeline/Pipeline$2;
             0      28     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
@@ -174,15 +174,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #15                 // Method apply:(Ljava/lang/Object;)Lsklearn/Estimator;
          5: areturn
       LineNumberTable:
-        line 134: 0
+        line 136: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/pipeline/Pipeline$2;
 }
 Signature: #42                          // Lorg/jpmml/python/CastFunction<TE;>;
 SourceFile: "Pipeline.java"
 EnclosingMethod: #46.#47                // sklearn.pipeline.Pipeline.getFinalEstimator
```

#### sklearn/pipeline/Pipeline.class

##### procyon -ec {}

```diff
@@ -1,26 +1,28 @@
 
 package sklearn.pipeline;
 
 import sklearn.Clusterer;
+import java.util.Map;
 import sklearn.Regressor;
 import sklearn.Classifier;
 import org.jpmml.python.CastFunction;
 import com.google.common.base.Function;
 import com.google.common.collect.Lists;
 import sklearn.Transformer;
 import org.jpmml.python.CastUtil;
 import sklearn.Estimator;
 import org.jpmml.python.TupleUtil;
 import java.util.List;
+import sklearn.HasPMMLOptions;
 import sklearn.HasHead;
 import org.jpmml.python.Castable;
 import sklearn.Composite;
 
-public class Pipeline extends Composite implements Castable, HasHead
+public class Pipeline extends Composite implements Castable, HasHead, HasPMMLOptions<Pipeline>
 {
     public Pipeline() {
         this("sklearn.pipeline", "Pipeline");
     }
     
     public Pipeline(final String module, final String name) {
         super(module, name);
@@ -91,14 +93,30 @@
         Estimator estimator = null;
         if (this.hasFinalEstimator()) {
             estimator = this.getFinalEstimator();
         }
         return PipelineUtil.getHead((List)transformers, estimator);
     }
     
+    public Map<String, ?> getPMMLOptions() {
+        if (this.hasFinalEstimator()) {
+            final Estimator estimator = this.getFinalEstimator();
+            return estimator.getPMMLOptions();
+        }
+        return null;
+    }
+    
+    public Pipeline setPMMLOptions(final Map<String, ?> pmmlOptions) {
+        if (this.hasFinalEstimator()) {
+            final Estimator estimator = this.getFinalEstimator();
+            estimator.setPMMLOptions((Map)pmmlOptions);
+        }
+        return this;
+    }
+    
     public Transformer toTransformer() {
         if (this.hasFinalEstimator()) {
             final Estimator estimator = this.getFinalEstimator();
             if (estimator != null) {
                 throw new IllegalArgumentException("The pipeline ends with an estimator object");
             }
         }
```

#### sklearn/pipeline/Pipeline$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 3b513eee5a1485ec18be204f6679c9edb7c2c7b0fba4166446677bbcb5fb2115
+  SHA-256 checksum f8d59166f6d78b871d2f31a4d738856935531ee1929faf8e17aac7a9f8ba9d1c
   Compiled from "Pipeline.java"
 class sklearn.pipeline.Pipeline$1 extends org.jpmml.python.CastFunction<sklearn.Transformer>
   minor version: 0
   major version: 52
   flags: (0x0020) ACC_SUPER
   this_class: #17                         // sklearn/pipeline/Pipeline$1
   super_class: #18                        // org/jpmml/python/CastFunction
@@ -107,15 +107,15 @@
          1: aload_1
          2: putfield      #1                  // Field this$0:Lsklearn/pipeline/Pipeline;
          5: aload_0
          6: aload_2
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 97: 0
+        line 99: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn/pipeline/Pipeline$1;
             0      11     1 this$0   Lsklearn/pipeline/Pipeline;
             0      11     2    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
@@ -136,17 +136,17 @@
         16: areturn
         17: aload_0
         18: aload_1
         19: invokespecial #7                  // Method org/jpmml/python/CastFunction.apply:(Ljava/lang/Object;)Ljava/lang/Object;
         22: checkcast     #8                  // class sklearn/Transformer
         25: areturn
       LineNumberTable:
-        line 102: 0
-        line 103: 13
-        line 106: 17
+        line 104: 0
+        line 105: 13
+        line 108: 17
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      26     0  this   Lsklearn/pipeline/Pipeline$1;
             0      26     1 object   Ljava/lang/Object;
       StackMapTable: number_of_entries = 2
         frame_type = 13 /* same */
         frame_type = 3 /* same */
@@ -165,15 +165,15 @@
         13: invokestatic  #13                 // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
         16: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         19: ldc           #14                 // String ) is not a supported Transformer
         21: invokevirtual #12                 // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         24: invokevirtual #15                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         27: areturn
       LineNumberTable:
-        line 111: 0
+        line 113: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      28     0  this   Lsklearn/pipeline/Pipeline$1;
             0      28     1 object   Ljava/lang/Object;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
@@ -181,15 +181,15 @@
     Code:
       stack=2, locals=2, args_size=2
          0: aload_0
          1: aload_1
          2: invokevirtual #16                 // Method apply:(Ljava/lang/Object;)Lsklearn/Transformer;
          5: areturn
       LineNumberTable:
-        line 97: 0
+        line 99: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       6     0  this   Lsklearn/pipeline/Pipeline$1;
 }
 Signature: #42                          // Lorg/jpmml/python/CastFunction<Lsklearn/Transformer;>;
 SourceFile: "Pipeline.java"
 EnclosingMethod: #46.#47                // sklearn.pipeline.Pipeline.getTransformers
```

#### sklearn/Step.class

##### procyon -ec {}

```diff
@@ -7,15 +7,15 @@
 {
     public Step(final String module, final String name) {
         super(module, name);
     }
     
     public void checkVersion() {
         final String sklearnVersion = this.getSkLearnVersion();
-        if (sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "1.2.2") > 0) {
+        if (sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "1.2.2") > 0) {
             final String message = "This converter version does not know about Scikit-Learn version " + sklearnVersion + " artifacts. Please upgrade the converter to the latest version, or downgrade Scikit-Learn to version 1.2.2";
             throw new IllegalArgumentException(message);
         }
     }
     
     public String getPMMLName() {
         return this.getOptionalString("pmml_name_");
```

#### sklearn/linear_model/logistic/LogisticRegression.class

##### procyon -ec {}

```diff
@@ -22,30 +22,30 @@
 import org.jpmml.converter.CMatrixUtil;
 import org.jpmml.converter.Label;
 import org.jpmml.converter.DiscreteLabel;
 import org.jpmml.converter.SchemaUtil;
 import org.jpmml.converter.CategoricalLabel;
 import net.razorvine.pickle.objects.ClassDict;
 import org.jpmml.python.ClassDictUtil;
-import sklearn.SkLearnUtil;
+import sklearn.VersionUtil;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import sklearn.linear_model.LinearClassifier;
 
 public class LogisticRegression extends LinearClassifier
 {
     public LogisticRegression(final String module, final String name) {
         super(module, name);
     }
     
     public Model encodeModel(final Schema schema) {
         final String sklearnVersion = this.getSkLearnVersion();
         String multiClass = this.getMultiClass();
         final String solver = this.getSolver();
-        if ("auto".equals(multiClass) && sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.22") >= 0) {
+        if ("auto".equals(multiClass) && sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "0.22") >= 0) {
             final int[] shape = this.getCoefShape();
             multiClass = getAutoMultiClass(solver, shape);
         }
         if ("auto".equals(multiClass)) {
             throw new IllegalArgumentException("Attribute '" + ClassDictUtil.formatMember((ClassDict)this, "multi_class") + "' must be explicitly set to the 'ovr' or 'multinomial' value");
         }
         if ("multinomial".equals(multiClass)) {
@@ -65,15 +65,15 @@
         final List<? extends Number> coef = this.getCoef();
         final List<? extends Number> intercept = this.getIntercept();
         final PMMLEncoder encoder = schema.getEncoder();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
         if (numberOfClasses == 1) {
             SchemaUtil.checkSize(2, (DiscreteLabel)categoricalLabel);
-            final boolean corrected = sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.20") >= 0;
+            final boolean corrected = sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "0.20") >= 0;
             if (!corrected) {
                 return this.encodeOvRModel(schema);
             }
             final Schema segmentSchema = schema.toRelabeledSchema((Label)null);
             final Model firstModel = (Model)RegressionModelUtil.createRegression((List)features, CMatrixUtil.getRow((List)coef, 1, numberOfFeatures, 0), (Number)intercept.get(0), (RegressionModel.NormalizationMethod)null, segmentSchema).setOutput(ModelUtil.createPredictedOutput("decisionFunction", OpType.CONTINUOUS, DataType.DOUBLE, new Transformation[0]));
             final Feature feature = (Feature)new ContinuousFeature(encoder, "decisionFunction", DataType.DOUBLE);
             final RegressionTable passiveRegressionTable = RegressionModelUtil.createRegressionTable((List)Collections.singletonList(feature), (List)Collections.singletonList(Double.valueOf(-1.0)), (Number)Double.valueOf(0.0)).setTargetCategory(categoricalLabel.getValue(0));
```

#### sklearn/ensemble/gradient_boosting/GradientBoostingClassifier.class

##### procyon -ec {}

```diff
@@ -13,15 +13,15 @@
 import org.jpmml.converter.Transformation;
 import org.dmg.pmml.OpType;
 import org.jpmml.converter.FieldNameUtil;
 import sklearn.Estimator;
 import org.jpmml.converter.DiscreteLabel;
 import org.jpmml.converter.SchemaUtil;
 import org.jpmml.converter.CategoricalLabel;
-import sklearn.SkLearnUtil;
+import sklearn.VersionUtil;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import org.dmg.pmml.DataType;
 import sklearn.tree.HasTreeOptions;
 import sklearn.tree.TreeRegressor;
 import sklearn.HasEstimatorEnsemble;
 import sklearn.Classifier;
@@ -46,15 +46,15 @@
     public MiningModel encodeModel(final Schema schema) {
         final String sklearnVersion = this.getSkLearnVersion();
         final LossFunction loss = this.getLoss();
         final int numberOfClasses = (int)loss.getK();
         final HasPriorProbability init = this.getInit();
         final Number learningRate = this.getLearningRate();
         IntFunction<Number> initialPredictions = init::getPriorProbability;
-        if (sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.21") >= 0) {
+        if (sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "0.21") >= 0) {
             final List<? extends Number> computedInitialPredictions = loss.computeInitialPredictions(init);
             initialPredictions = computedInitialPredictions::get;
         }
         final Schema segmentSchema = schema.toAnonymousRegressorSchema(DataType.DOUBLE);
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         MiningModel miningModel;
         if (numberOfClasses == 1) {
```

#### sklearn/ensemble/iforest/IsolationForest.class

##### procyon -ec {}

```diff
@@ -22,15 +22,15 @@
 import com.google.common.primitives.Ints;
 import java.util.List;
 import sklearn.Regressor;
 import org.dmg.pmml.tree.TreeModel;
 import java.util.ArrayList;
 import org.jpmml.converter.ScoreDistributionManager;
 import org.jpmml.converter.PredicateManager;
-import sklearn.SkLearnUtil;
+import sklearn.VersionUtil;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import sklearn.OutlierDetector;
 import sklearn.tree.HasTreeOptions;
 import sklearn.ensemble.EnsembleRegressor;
 
 public class IsolationForest extends EnsembleRegressor implements HasTreeOptions, OutlierDetector
@@ -43,16 +43,16 @@
         return false;
     }
     
     public MiningModel encodeModel(final Schema schema) {
         final String sklearnVersion = this.getSkLearnVersion();
         final List<? extends Regressor> estimators = this.getEstimators();
         final List<List<Integer>> estimatorsFeatures = this.getEstimatorsFeatures();
-        final boolean corrected = sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.19") >= 0;
-        final boolean nodeSampleCorrected = sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.21") >= 0;
+        final boolean corrected = sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "0.19") >= 0;
+        final boolean nodeSampleCorrected = sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "0.21") >= 0;
         final Boolean numeric = (Boolean)this.getOption("numeric", (Object)Boolean.TRUE);
         final PredicateManager predicateManager = new PredicateManager();
         final ScoreDistributionManager scoreDistributionManager = new ScoreDistributionManager();
         final Schema segmentSchema = schema.toAnonymousSchema();
         final List<TreeModel> treeModels = new ArrayList<TreeModel>();
         for (int i = 0; i < estimators.size(); ++i) {
             final Regressor estimator = (Regressor)estimators.get(i);
```

#### sklearn/discriminant_analysis/LinearDiscriminantAnalysis.class

##### procyon -ec {}

```diff
@@ -12,15 +12,15 @@
 import org.dmg.pmml.regression.RegressionModel;
 import java.util.List;
 import org.jpmml.converter.CMatrixUtil;
 import java.util.ArrayList;
 import org.dmg.pmml.DataType;
 import org.jpmml.converter.DiscreteLabel;
 import org.jpmml.converter.SchemaUtil;
-import sklearn.SkLearnUtil;
+import sklearn.VersionUtil;
 import org.jpmml.converter.CategoricalLabel;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import sklearn.linear_model.LinearClassifier;
 
 public class LinearDiscriminantAnalysis extends LinearClassifier
 {
@@ -47,15 +47,15 @@
         final int[] shape = this.getCoefShape();
         final int numberOfClasses = shape[0];
         final int numberOfFeatures = shape[1];
         final List<? extends Number> coef = this.getCoef();
         final List<? extends Number> intercept = this.getIntercept();
         final CategoricalLabel categoricalLabel = (CategoricalLabel)schema.getLabel();
         final List<? extends Feature> features = schema.getFeatures();
-        final boolean corrected = sklearnVersion != null && SkLearnUtil.compareVersion(sklearnVersion, "0.21") >= 0;
+        final boolean corrected = sklearnVersion != null && VersionUtil.compareVersion(sklearnVersion, "0.21") >= 0;
         if (!corrected) {
             return super.encodeModel(schema);
         }
         if (numberOfClasses >= 3) {
             SchemaUtil.checkSize(numberOfClasses, (DiscreteLabel)categoricalLabel);
             final Schema segmentSchema = schema.toAnonymousRegressorSchema(DataType.DOUBLE).toEmptySchema();
             final List<Model> models = new ArrayList<Model>();
```

#### sklearn/Estimator.class

##### procyon -ec {}

```diff
@@ -25,15 +25,15 @@
 import org.dmg.pmml.OpType;
 import java.util.List;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
 import org.dmg.pmml.MiningFunction;
 import org.slf4j.Logger;
 
-public abstract class Estimator extends Step implements HasNumberOfOutputs
+public abstract class Estimator extends Step implements HasNumberOfOutputs, HasPMMLOptions<Estimator>
 {
     public static final String FIELD_APPLY = "apply";
     public static final String FIELD_DECISION_FUNCTION = "decisionFunction";
     public static final String FIELD_PREDICT = "predict";
     private static final Logger logger;
     
     public Estimator(final String module, final String name) {
```

#### sklearn2pmml/pipeline/PMMLPipeline$3.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 572b3193c38934b75fa208b24f1365819741f1268017177b3cdc4f63aa233ca9
+  SHA-256 checksum 01ce355a793639a3619110df7419f0188f0a99e536ff3295afaad19512e979d7
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$3 extends java.lang.Object implements com.google.common.base.Function<java.lang.Object, java.lang.Object>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #4                          // sklearn2pmml/pipeline/PMMLPipeline$3
   super_class: #5                         // java/lang/Object
@@ -56,15 +56,15 @@
     flags: (0x0000)
     Code:
       stack=1, locals=1, args_size=1
          0: aload_0
          1: invokespecial #1                  // Method java/lang/Object."<init>":()V
          4: return
       LineNumberTable:
-        line 717: 0
+        line 726: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0       5     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$3;
 
   public java.lang.Object apply(java.lang.Object);
     descriptor: (Ljava/lang/Object;)Ljava/lang/Object;
     flags: (0x0001) ACC_PUBLIC
@@ -77,18 +77,18 @@
          6: invokestatic  #3                  // Method org/jpmml/converter/ValueUtil.isNaN:(Ljava/lang/Object;)Z
          9: ifeq          14
         12: aconst_null
         13: areturn
         14: aload_1
         15: areturn
       LineNumberTable:
-        line 721: 0
-        line 723: 5
-        line 724: 12
-        line 727: 14
+        line 730: 0
+        line 732: 5
+        line 733: 12
+        line 736: 14
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      16     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$3;
             0      16     1 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 14 /* same */
 }
```

#### sklearn2pmml/pipeline/PMMLPipeline$4.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 95ff94f650595d2fb6ef2af9dd77ccfbec9a253afe6fe705c22a950889aff80c
+  SHA-256 checksum 397297c3182397c368c94e20bd1726b6b698e0772af16ec8e84784443391c566
   Compiled from "PMMLPipeline.java"
 class sklearn2pmml.pipeline.PMMLPipeline$4
   minor version: 0
   major version: 52
   flags: (0x1020) ACC_SUPER, ACC_SYNTHETIC
   this_class: #13                         // sklearn2pmml/pipeline/PMMLPipeline$4
   super_class: #14                        // java/lang/Object
@@ -129,16 +129,16 @@
          from    to  target type
              9    20    23   Class java/lang/NoSuchFieldError
             24    35    38   Class java/lang/NoSuchFieldError
             39    50    53   Class java/lang/NoSuchFieldError
             63    74    77   Class java/lang/NoSuchFieldError
             78    89    92   Class java/lang/NoSuchFieldError
       LineNumberTable:
-        line 571: 0
-        line 333: 54
+        line 580: 0
+        line 342: 54
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
       StackMapTable: number_of_entries = 10
         frame_type = 87 /* same_locals_1_stack_item */
           stack = [ class java/lang/NoSuchFieldError ]
         frame_type = 0 /* same */
         frame_type = 77 /* same_locals_1_stack_item */
```

#### sklearn2pmml/pipeline/PMMLPipeline.class

##### procyon -ec {}

```diff
@@ -23,15 +23,14 @@
 import org.dmg.pmml.Header;
 import org.jpmml.converter.PMMLUtil;
 import org.dmg.pmml.Extension;
 import org.dmg.pmml.MiningBuildTask;
 import java.util.Iterator;
 import org.dmg.pmml.Output;
 import org.dmg.pmml.DataField;
-import org.jpmml.converter.Schema;
 import org.jpmml.python.PythonObject;
 import org.jpmml.converter.Label;
 import sklearn.Estimator;
 import sklearn.Transformer;
 import java.util.Map;
 import sklearn2pmml.decoration.Domain;
 import sklearn.Classifier;
@@ -47,28 +46,30 @@
 import org.dmg.pmml.OutputField;
 import org.jpmml.converter.ScalarLabelUtil;
 import org.jpmml.converter.ModelUtil;
 import org.jpmml.converter.mining.MiningModelUtil;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.converter.WildcardFeature;
 import java.util.Collection;
-import org.dmg.pmml.Model;
 import sklearn.Step;
 import sklearn.Initializer;
 import java.util.ArrayList;
 import sklearn.pipeline.PipelineUtil;
 import org.dmg.pmml.PMML;
+import org.dmg.pmml.Model;
+import org.jpmml.converter.Schema;
 import org.jpmml.python.ClassDictUtil;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Feature;
 import java.util.List;
 import org.slf4j.Logger;
+import org.jpmml.sklearn.Encodable;
 import sklearn.pipeline.Pipeline;
 
-public class PMMLPipeline extends Pipeline
+public class PMMLPipeline extends Pipeline implements Encodable
 {
     private static final Logger logger;
     
     public PMMLPipeline() {
         this("sklearn2pmml", "PMMLPipeline");
     }
     
@@ -77,15 +78,20 @@
     }
     
     public List<Feature> encodeFeatures(final List<Feature> features, final SkLearnEncoder encoder) {
         PMMLPipeline.logger.warn(ClassDictUtil.formatClass((Object)this) + " should be replaced with " + ClassDictUtil.formatClass((Object)new Pipeline()) + " in nested workflows");
         return super.encodeFeatures((List)features, encoder);
     }
     
-    public PMML encodePMML(final SkLearnEncoder encoder) {
+    public Model encodeModel(final Schema schema) {
+        return super.encodeModel(schema);
+    }
+    
+    public PMML encodePMML() {
+        final SkLearnEncoder encoder = new SkLearnEncoder();
         final List<? extends Transformer> transformers = this.getTransformers();
         Estimator estimator = null;
         if (this.hasFinalEstimator()) {
             estimator = this.getFinalEstimator();
         }
         final Map<?, ?> header = this.getHeader();
         final Transformer predictTransformer = this.getPredictTransformer();
```

#### sklearn2pmml/pipeline/PMMLPipeline$2.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum eb0ca6cf9c387cae56fae3aadff956e8b28d6fc40c57c4d2239af16f777cc8c8
+  SHA-256 checksum 7cfda5e80077f3646fd8022d3b5959e6a2ef39d6f088bb8860d710a1b0aee526
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$2 extends org.jpmml.converter.visitors.AbstractExtender
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #9                          // sklearn2pmml/pipeline/PMMLPipeline$2
   super_class: #10                        // org/jpmml/converter/visitors/AbstractExtender
@@ -89,15 +89,15 @@
          1: aload_2
          2: putfield      #1                  // Field val$values:Ljava/util/Map;
          5: aload_0
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/converter/visitors/AbstractExtender."<init>":(Ljava/lang/String;)V
         10: return
       LineNumberTable:
-        line 668: 0
+        line 677: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
             0      11     1    x0   Ljava/lang/String;
 
   public org.dmg.pmml.VisitorAction visit(org.dmg.pmml.Value);
     descriptor: (Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
@@ -121,19 +121,19 @@
         26: invokestatic  #6                  // Method org/jpmml/converter/ValueUtil.asString:(Ljava/lang/Object;)Ljava/lang/String;
         29: invokevirtual #7                  // Method addExtension:(Lorg/dmg/pmml/PMMLObject;Ljava/lang/String;)V
         32: aload_0
         33: aload_1
         34: invokespecial #8                  // Method org/jpmml/converter/visitors/AbstractExtender.visit:(Lorg/dmg/pmml/Value;)Lorg/dmg/pmml/VisitorAction;
         37: areturn
       LineNumberTable:
-        line 672: 0
-        line 674: 14
-        line 675: 18
-        line 677: 23
-        line 680: 32
+        line 681: 0
+        line 683: 14
+        line 684: 18
+        line 686: 23
+        line 689: 32
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      38     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$2;
             0      38     1 pmmlValue   Lorg/dmg/pmml/Value;
            14      24     2 value   Ljava/lang/Object;
       StackMapTable: number_of_entries = 1
         frame_type = 252 /* append */
```

#### sklearn2pmml/pipeline/PMMLPipeline$1.class

##### javap -verbose -constants -s -l -private {}

```diff
@@ -1,8 +1,8 @@
-  SHA-256 checksum 8e06ac2621148ef2f077c68371e735e95127dcc9f1c3a18e1aa0a351c66670a5
+  SHA-256 checksum 1a97440e0f23c6184c03ae9fbb620ea646adab7e64eee1184a33a6f0f5525bee
   Compiled from "PMMLPipeline.java"
 final class sklearn2pmml.pipeline.PMMLPipeline$1 extends org.jpmml.python.CastFunction<java.util.List<?>>
   minor version: 0
   major version: 52
   flags: (0x0030) ACC_FINAL, ACC_SUPER
   this_class: #11                         // sklearn2pmml/pipeline/PMMLPipeline$1
   super_class: #12                        // org/jpmml/python/CastFunction
@@ -83,15 +83,15 @@
          1: aload_2
          2: putfield      #1                  // Field val$targetField:Ljava/lang/String;
          5: aload_0
          6: aload_1
          7: invokespecial #2                  // Method org/jpmml/python/CastFunction."<init>":(Ljava/lang/Class;)V
         10: return
       LineNumberTable:
-        line 592: 0
+        line 601: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      11     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      11     1    x0   Ljava/lang/Class;
       LocalVariableTypeTable:
         Start  Length  Slot  Name   Signature
             0      11     1    x0   Ljava/lang/Class<+Ljava/util/List<*>;>;
@@ -115,15 +115,15 @@
         25: invokestatic  #8                  // Method org/jpmml/python/ClassDictUtil.formatClass:(Ljava/lang/Object;)Ljava/lang/String;
         28: invokevirtual #6                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         31: ldc           #9                  // String ) is not supported
         33: invokevirtual #6                  // Method java/lang/StringBuilder.append:(Ljava/lang/String;)Ljava/lang/StringBuilder;
         36: invokevirtual #10                 // Method java/lang/StringBuilder.toString:()Ljava/lang/String;
         39: areturn
       LineNumberTable:
-        line 596: 0
+        line 605: 0
       LocalVariableTable:
         Start  Length  Slot  Name   Signature
             0      40     0  this   Lsklearn2pmml/pipeline/PMMLPipeline$1;
             0      40     1 object   Ljava/lang/Object;
 }
 Signature: #32                          // Lorg/jpmml/python/CastFunction<Ljava/util/List<*>;>;
 SourceFile: "PMMLPipeline.java"
```

#### org/jpmml/sklearn/testing/SkLearnEncoderBatch.class

##### procyon -ec {}

```diff
@@ -1,16 +1,18 @@
 
 package org.jpmml.sklearn.testing;
 
+import org.jpmml.sklearn.SkLearnUtil;
 import org.jpmml.converter.testing.ModelEncoderBatchTest;
 import org.jpmml.python.testing.PythonEncoderBatchTest;
-import sklearn.Estimator;
+import org.jpmml.sklearn.Encodable;
 import java.util.Map;
-import sklearn2pmml.pipeline.PMMLPipeline;
-import org.jpmml.sklearn.SkLearnEncoder;
+import sklearn.HasPMMLOptions;
+import org.jpmml.sklearn.EncodableUtil;
+import sklearn.Step;
 import org.dmg.pmml.PMML;
 import com.google.common.base.Equivalence;
 import org.jpmml.evaluator.ResultField;
 import java.util.function.Predicate;
 import org.jpmml.python.testing.PythonEncoderBatch;
 
 public abstract class SkLearnEncoderBatch extends PythonEncoderBatch
@@ -18,31 +20,35 @@
     public SkLearnEncoderBatch(final String algorithm, final String dataset, final Predicate<ResultField> columnFilter, final Equivalence<Object> equivalence) {
         super(algorithm, dataset, (Predicate)columnFilter, (Equivalence)equivalence);
     }
     
     public abstract SkLearnEncoderBatchTest getArchiveBatchTest();
     
     public PMML getPMML() throws Exception {
-        final SkLearnEncoder encoder = new SkLearnEncoder();
-        final PMMLPipeline pipeline = (PMMLPipeline)this.loadPickle((Class)PMMLPipeline.class);
-        this.activate(pipeline);
+        final Map<String, ?> options = this.getOptions();
+        final Step step = (Step)this.loadPickle((Class)Step.class);
+        this.activate(step);
         try {
-            final PMML pmml = pipeline.encodePMML(encoder);
+            final Encodable encodable = EncodableUtil.toEncodable((Object)step);
+            if (options != null && !options.isEmpty()) {
+                final HasPMMLOptions<?> hasPmmlOptions = (HasPMMLOptions<?>)encodable;
+                hasPmmlOptions.setPMMLOptions((Map)options);
+            }
+            final PMML pmml = encodable.encodePMML();
             this.validatePMML(pmml);
             return pmml;
         }
         finally {
-            this.deactivate(pipeline);
+            this.deactivate(step);
         }
     }
     
-    protected void activate(final PMMLPipeline pipeline) throws Exception {
-        final Map<String, ?> options = this.getOptions();
-        final Estimator estimator = pipeline.getFinalEstimator();
-        if (!options.isEmpty()) {
-            estimator.putOptions((Map)options);
-        }
+    protected void activate(final Object object) throws Exception {
+    }
+    
+    protected void deactivate(final Object object) throws Exception {
     }
     
-    protected void deactivate(final PMMLPipeline pipeline) throws Exception {
+    static {
+        SkLearnUtil.initOnce();
     }
 }
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.34</version>
+    <version>1.7.35</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn converter</name>
   <description>JPMML Scikit-Learn to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn/pom.properties

```diff
@@ -1,3 +1,3 @@
 artifactId=pmml-sklearn
 groupId=org.jpmml
-version=1.7.34
+version=1.7.35
```

#### Comparing `sklearn/SkLearnUtil.class` & `sklearn/VersionUtil.class`

 * *Files 7% similar despite different names*

##### procyon -ec {}

```diff
@@ -2,20 +2,20 @@
 package sklearn;
 
 import java.util.regex.Matcher;
 import java.util.ArrayList;
 import java.util.List;
 import java.util.regex.Pattern;
 
-public class SkLearnUtil
+public class VersionUtil
 {
     private static final String PEP440_REGEX = "(\\d+)\\.(\\d+)(?:(?:a|b|rc)\\d)?(?:\\.(?:(\\d)|(?:(?:post|dev)?\\d?)))*";
     private static final Pattern PEP440_VERSION;
     
-    private SkLearnUtil() {
+    private VersionUtil() {
     }
     
     public static int compareVersion(final String left, final String right) {
         final List<Integer> leftTokens = parseVersion(left);
         final List<Integer> rightTokens = parseVersion(right);
         for (int i = 0; i < Math.min(leftTokens.size(), rightTokens.size()); ++i) {
             final int diff = Integer.compare(Integer.valueOf(leftTokens.get(i)), Integer.valueOf(rightTokens.get(i)));
@@ -26,15 +26,15 @@
         if (leftTokens.size() < rightTokens.size() && Integer.valueOf(rightTokens.get(leftTokens.size())) != 0) {
             return -1;
         }
         return 0;
     }
     
     public static List<Integer> parseVersion(final String string) {
-        final Matcher matcher = SkLearnUtil.PEP440_VERSION.matcher(string);
+        final Matcher matcher = VersionUtil.PEP440_VERSION.matcher(string);
         if (!matcher.matches()) {
             throw new IllegalArgumentException(string);
         }
         final List<Integer> tokens = new ArrayList<Integer>();
         for (int i = 1; i <= 3; ++i) {
             final String token = matcher.group(i);
             if (token == null) {
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/guava-32.1.1-jre.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/guava-32.1.1-jre.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-core-3.0.2.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/jaxb-core-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-api-1.7.36.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/slf4j-api-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-h2o-1.2.9.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-h2o-1.2.9.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/jackson-annotations-2.13.3.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/jackson-annotations-2.13.3.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/jcommander-1.72.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/jcommander-1.72.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-converter-1.5.5.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-converter-1.5.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-lightgbm-1.4.6.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-1.6.4.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-model-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-gson-0.1.8.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/ubjson-gson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-model-metro-1.6.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.34.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-statsmodels-1.7.35.jar`

 * *Files 22% similar despite different names*

#### zipinfo {}

```diff
@@ -1,16 +1,17 @@
-Zip file size: 6242 bytes, number of entries: 14
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklearn2pmml/statsmodels/
--rw-rw-r--  2.0 unx      152 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2079 b- defN 23-Aug-03 15:40 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
--rw-rw-r--  2.0 unx     1515 b- defN 23-Aug-03 15:40 sklearn2pmml/statsmodels/StatsModelsClassifier.class
--rw-rw-r--  2.0 unx     1920 b- defN 23-Aug-03 15:40 sklearn2pmml/statsmodels/StatsModelsUtil.class
--rw-rw-r--  2.0 unx     1511 b- defN 23-Aug-03 15:40 sklearn2pmml/statsmodels/StatsModelsRegressor.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
--rw-rw-r--  2.0 unx     1331 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
--rw-rw-r--  2.0 unx      120 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
-14 files, 8758 bytes uncompressed, 4120 bytes compressed:  53.0%
+Zip file size: 6844 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-05 19:08 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 sklearn2pmml/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 sklearn2pmml/statsmodels/
+-rw-rw-r--  2.0 unx      152 b- defN 23-Aug-05 19:08 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2079 b- defN 23-Aug-05 19:08 sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
+-rw-rw-r--  2.0 unx     1744 b- defN 23-Aug-05 19:08 sklearn2pmml/statsmodels/StatsModelsClassifier.class
+-rw-rw-r--  2.0 unx      180 b- defN 23-Aug-05 19:08 sklearn2pmml/statsmodels/HasResults.class
+-rw-rw-r--  2.0 unx     2352 b- defN 23-Aug-05 19:08 sklearn2pmml/statsmodels/StatsModelsUtil.class
+-rw-rw-r--  2.0 unx     1740 b- defN 23-Aug-05 19:08 sklearn2pmml/statsmodels/StatsModelsRegressor.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/
+-rw-rw-r--  2.0 unx     1331 b- defN 23-Aug-05 19:07 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml
+-rw-rw-r--  2.0 unx      120 b- defN 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties
+15 files, 9828 bytes uncompressed, 4564 bytes compressed:  53.6%
```

#### zipnote «TEMP»/diffoscope_y9tsz13i_/tmpw06bwxjs_.zip

```diff
@@ -15,14 +15,17 @@
 
 Filename: sklearn2pmml/statsmodels/StatsModelsOrdinalClassifier.class
 Comment: 
 
 Filename: sklearn2pmml/statsmodels/StatsModelsClassifier.class
 Comment: 
 
+Filename: sklearn2pmml/statsmodels/HasResults.class
+Comment: 
+
 Filename: sklearn2pmml/statsmodels/StatsModelsUtil.class
 Comment: 
 
 Filename: sklearn2pmml/statsmodels/StatsModelsRegressor.class
 Comment: 
 
 Filename: META-INF/maven/
```

#### sklearn2pmml/statsmodels/StatsModelsClassifier.class

##### procyon -ec {}

```diff
@@ -1,30 +1,37 @@
 
 package sklearn2pmml.statsmodels;
 
+import sklearn.Estimator;
+import org.dmg.pmml.PMML;
 import statsmodels.ResultsWrapper;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
+import org.jpmml.sklearn.Encodable;
 import sklearn.Classifier;
 
-public class StatsModelsClassifier extends Classifier
+public class StatsModelsClassifier extends Classifier implements HasResults, Encodable
 {
     public StatsModelsClassifier(final String module, final String name) {
         super(module, name);
     }
     
     public Model encodeModel(Schema schema) {
         final Boolean fitIntercept = this.getFitIntercept();
         final ResultsWrapper results = this.getResults();
         if ((boolean)fitIntercept) {
             schema = StatsModelsUtil.addConstant(schema);
         }
         return results.encodeModel(schema);
     }
     
+    public PMML encodePMML() {
+        return StatsModelsUtil.encodePMML((Estimator)this);
+    }
+    
     public Boolean getFitIntercept() {
         return this.getBoolean("fit_intercept");
     }
     
     public ResultsWrapper getResults() {
         return (ResultsWrapper)this.get("results_", (Class)ResultsWrapper.class);
     }
```

#### sklearn2pmml/statsmodels/StatsModelsUtil.class

##### procyon -ec {}

```diff
@@ -1,27 +1,36 @@
 
 package sklearn2pmml.statsmodels;
 
-import org.jpmml.python.PickleUtil;
 import org.jpmml.converter.Label;
 import java.util.List;
 import org.jpmml.converter.Feature;
 import org.jpmml.converter.PMMLEncoder;
 import org.jpmml.statsmodels.InterceptFeature;
 import org.dmg.pmml.DataType;
 import org.jpmml.sklearn.SkLearnEncoder;
 import org.jpmml.converter.Schema;
+import statsmodels.ResultsWrapper;
+import org.jpmml.statsmodels.StatsModelsEncoder;
+import org.dmg.pmml.PMML;
+import sklearn.Estimator;
 
 public class StatsModelsUtil
 {
     private static boolean initialized;
     
     private StatsModelsUtil() {
     }
     
+    public static <E extends Estimator & HasResults> PMML encodePMML(final E estimator) {
+        final StatsModelsEncoder encoder = new StatsModelsEncoder();
+        final ResultsWrapper resultsWrapper = ((E)estimator).getResults();
+        return resultsWrapper.encodePMML(encoder);
+    }
+    
     public static Schema addConstant(final Schema schema) {
         final SkLearnEncoder encoder = (SkLearnEncoder)schema.getEncoder();
         final Label label = schema.getLabel();
         final List<Feature> features = schema.getFeatures();
         features.add(0, (Feature)new InterceptFeature((PMMLEncoder)encoder, "const", DataType.DOUBLE));
         return new Schema((PMMLEncoder)encoder, label, (List)features);
     }
@@ -30,15 +39,14 @@
         if (!StatsModelsUtil.initialized) {
             init();
             StatsModelsUtil.initialized = true;
         }
     }
     
     private static void init() {
-        final ClassLoader clazzLoader = SkLearnEncoder.class.getClassLoader();
-        PickleUtil.init(clazzLoader, "statsmodels2pmml.properties");
+        final StatsModelsEncoder encoder = new StatsModelsEncoder();
     }
     
     static {
         StatsModelsUtil.initialized = false;
     }
 }
```

#### sklearn2pmml/statsmodels/StatsModelsRegressor.class

##### procyon -ec {}

```diff
@@ -1,30 +1,37 @@
 
 package sklearn2pmml.statsmodels;
 
+import sklearn.Estimator;
+import org.dmg.pmml.PMML;
 import statsmodels.ResultsWrapper;
 import org.dmg.pmml.Model;
 import org.jpmml.converter.Schema;
+import org.jpmml.sklearn.Encodable;
 import sklearn.Regressor;
 
-public class StatsModelsRegressor extends Regressor
+public class StatsModelsRegressor extends Regressor implements HasResults, Encodable
 {
     public StatsModelsRegressor(final String module, final String name) {
         super(module, name);
     }
     
     public Model encodeModel(Schema schema) {
         final Boolean fitIntercept = this.getFitIntercept();
         final ResultsWrapper results = this.getResults();
         if ((boolean)fitIntercept) {
             schema = StatsModelsUtil.addConstant(schema);
         }
         return results.encodeModel(schema);
     }
     
+    public PMML encodePMML() {
+        return StatsModelsUtil.encodePMML((Estimator)this);
+    }
+    
     public Boolean getFitIntercept() {
         return this.getBoolean("fit_intercept");
     }
     
     public ResultsWrapper getResults() {
         return (ResultsWrapper)this.get("results_", (Class)ResultsWrapper.class);
     }
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.34</version>
+    <version>1.7.35</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-statsmodels</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn StatsModels converter</name>
   <description>JPMML Scikit-Learn StatsModels to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-statsmodels/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Thu Aug 03 15:40:52 EEST 2023
-version=1.7.34
+#Sat Aug 05 19:08:01 EEST 2023
+version=1.7.35
 groupId=org.jpmml
 artifactId=pmml-sklearn-statsmodels
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/ubjson-0.1.8.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/ubjson-0.1.8.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/gson-2.10.1.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/gson-2.10.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/h2o-genmodel-3.42.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/classpath.txt` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/classpath.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,20 +14,20 @@
 pickle-1.4.jar
 pmml-converter-1.5.5.jar
 pmml-h2o-1.2.9.jar
 pmml-lightgbm-1.4.6.jar
 pmml-model-1.6.4.jar
 pmml-model-metro-1.6.4.jar
 pmml-python-1.1.17.jar
-pmml-sklearn-1.7.34.jar
-pmml-sklearn-extension-1.7.34.jar
-pmml-sklearn-h2o-1.7.34.jar
-pmml-sklearn-lightgbm-1.7.34.jar
-pmml-sklearn-statsmodels-1.7.34.jar
-pmml-sklearn-xgboost-1.7.34.jar
+pmml-sklearn-1.7.35.jar
+pmml-sklearn-extension-1.7.35.jar
+pmml-sklearn-h2o-1.7.35.jar
+pmml-sklearn-lightgbm-1.7.35.jar
+pmml-sklearn-statsmodels-1.7.35.jar
+pmml-sklearn-xgboost-1.7.35.jar
 pmml-statsmodels-1.0.5.jar
 pmml-xgboost-1.7.4.jar
 serpent-1.40.jar
 slf4j-api-1.7.36.jar
 slf4j-jdk14-1.7.36.jar
 ubjson-0.1.8.jar
 ubjson-gson-0.1.8.jar
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/h2o-logger-3.42.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-python-1.1.17.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-python-1.1.17.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.34.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-lightgbm-1.7.35.jar`

 * *Files 20% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7357 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 lightgbm/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 lightgbm/sklearn/
--rw-rw-r--  2.0 unx      177 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      170 b- defN 23-Aug-03 15:40 lightgbm/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2047 b- defN 23-Aug-03 15:40 lightgbm/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2102 b- defN 23-Aug-03 15:40 lightgbm/sklearn/LGBMRegressor.class
--rw-rw-r--  2.0 unx     2126 b- defN 23-Aug-03 15:40 lightgbm/sklearn/LGBMClassifier.class
--rw-rw-r--  2.0 unx     3298 b- defN 23-Aug-03 15:40 lightgbm/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
--rw-rw-r--  2.0 unx     1319 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
--rw-rw-r--  2.0 unx      117 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
-15 files, 11486 bytes uncompressed, 5277 bytes compressed:  54.1%
+Zip file size: 7608 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-05 19:08 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 lightgbm/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 lightgbm/sklearn/
+-rw-rw-r--  2.0 unx      177 b- defN 23-Aug-05 19:08 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      170 b- defN 23-Aug-05 19:08 lightgbm/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2047 b- defN 23-Aug-05 19:08 lightgbm/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2288 b- defN 23-Aug-05 19:08 lightgbm/sklearn/LGBMRegressor.class
+-rw-rw-r--  2.0 unx     2312 b- defN 23-Aug-05 19:08 lightgbm/sklearn/LGBMClassifier.class
+-rw-rw-r--  2.0 unx     3797 b- defN 23-Aug-05 19:08 lightgbm/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/
+-rw-rw-r--  2.0 unx     1319 b- defN 23-Aug-05 19:07 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml
+-rw-rw-r--  2.0 unx      117 b- defN 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties
+15 files, 12357 bytes uncompressed, 5528 bytes compressed:  55.3%
```

#### lightgbm/sklearn/LGBMRegressor.class

##### procyon -ec {}

```diff
@@ -1,21 +1,23 @@
 
 package lightgbm.sklearn;
 
 import org.dmg.pmml.Model;
+import org.dmg.pmml.PMML;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import org.jpmml.lightgbm.ObjectiveFunction;
 import org.jpmml.lightgbm.Regression;
 import org.jpmml.converter.Label;
 import sklearn.Estimator;
+import org.jpmml.sklearn.Encodable;
 import org.jpmml.lightgbm.HasLightGBMOptions;
 import sklearn.Regressor;
 
-public class LGBMRegressor extends Regressor implements HasBooster, HasLightGBMOptions
+public class LGBMRegressor extends Regressor implements HasBooster, HasLightGBMOptions, Encodable
 {
     public LGBMRegressor(final String module, final String name) {
         super(module, name);
     }
     
     public int getNumberOfFeatures() {
         return BoosterUtil.getNumberOfFeatures((Estimator)this);
@@ -29,11 +31,15 @@
         }
     }
     
     public MiningModel encodeModel(final Schema schema) {
         return BoosterUtil.encodeModel((Estimator)this, schema);
     }
     
+    public PMML encodePMML() {
+        return BoosterUtil.encodePMML((Estimator)this);
+    }
+    
     public Booster getBooster() {
         return (Booster)this.get("_Booster", (Class)Booster.class);
     }
 }
```

#### lightgbm/sklearn/LGBMClassifier.class

##### procyon -ec {}

```diff
@@ -1,21 +1,23 @@
 
 package lightgbm.sklearn;
 
 import org.dmg.pmml.Model;
+import org.dmg.pmml.PMML;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import org.jpmml.lightgbm.ObjectiveFunction;
 import org.jpmml.lightgbm.Classification;
 import org.jpmml.converter.Label;
 import sklearn.Estimator;
+import org.jpmml.sklearn.Encodable;
 import org.jpmml.lightgbm.HasLightGBMOptions;
 import sklearn.LabelEncoderClassifier;
 
-public class LGBMClassifier extends LabelEncoderClassifier implements HasBooster, HasLightGBMOptions
+public class LGBMClassifier extends LabelEncoderClassifier implements HasBooster, HasLightGBMOptions, Encodable
 {
     public LGBMClassifier(final String module, final String name) {
         super(module, name);
     }
     
     public int getNumberOfFeatures() {
         return BoosterUtil.getNumberOfFeatures((Estimator)this);
@@ -29,11 +31,15 @@
         }
     }
     
     public MiningModel encodeModel(final Schema schema) {
         return BoosterUtil.encodeModel((Estimator)this, schema);
     }
     
+    public PMML encodePMML() {
+        return BoosterUtil.encodePMML((Estimator)this);
+    }
+    
     public Booster getBooster() {
         return (Booster)this.get("_Booster", (Class)Booster.class);
     }
 }
```

#### lightgbm/sklearn/BoosterUtil.class

##### procyon -ec {}

```diff
@@ -1,10 +1,12 @@
 
 package lightgbm.sklearn;
 
+import java.util.List;
+import org.dmg.pmml.PMML;
 import org.dmg.pmml.Model;
 import java.util.Map;
 import org.jpmml.converter.ModelEncoder;
 import java.util.LinkedHashMap;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.lightgbm.HasLightGBMOptions;
 import org.jpmml.converter.Schema;
@@ -39,12 +41,18 @@
         final ModelEncoder encoder = (ModelEncoder)schema.getEncoder();
         final Schema lgbmSchema = gbdt.toLightGBMSchema(schema);
         final MiningModel miningModel = gbdt.encodeMiningModel((Map)options, lgbmSchema);
         encoder.transferFeatureImportances((Model)null, (Model)miningModel);
         return miningModel;
     }
     
+    public static <E extends Estimator & HasBooster & HasLightGBMOptions> PMML encodePMML(final E estimator) {
+        final GBDT gbdt = getGBDT(estimator);
+        final Map<String, ?> options = ((E)estimator).getNativeConfiguration();
+        return gbdt.encodePMML((Map)options, (String)null, (List)null);
+    }
+    
     private static GBDT getGBDT(final HasBooster hasBooster) {
         final Booster booster = hasBooster.getBooster();
         return booster.getGBDT();
     }
 }
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.34</version>
+    <version>1.7.35</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-lightgbm</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn LightGBM converter</name>
   <description>JPMML Scikit-Learn LightGBM to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-lightgbm/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Thu Aug 03 15:40:51 EEST 2023
-version=1.7.34
+#Sat Aug 05 19:08:01 EEST 2023
+version=1.7.35
 groupId=org.jpmml
 artifactId=pmml-sklearn-lightgbm
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/slf4j-jdk14-1.7.36.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/jaxb-runtime-3.0.2.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/serpent-1.40.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/serpent-1.40.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/istack-commons-runtime-4.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.activation-2.0.1.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/jakarta.activation-2.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/jakarta.xml.bind-api-3.0.1.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-extension-1.7.34.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-extension-1.7.35.jar`

 * *Files 10% similar despite different names*

#### zipinfo {}

```diff
@@ -1,67 +1,67 @@
 Zip file size: 84465 bytes, number of entries: 65
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 pycaret/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 pycaret/pipeline/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 pycaret/preprocess/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 tpot/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 tpot/builtins/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 optbinning/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 optbinning/scorecard/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 imblearn/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 category_encoders/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklego/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 sklego/meta/
--rw-rw-r--  2.0 unx     4312 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx     2928 b- defN 23-Aug-03 15:40 pycaret/pipeline/Pipeline.class
--rw-rw-r--  2.0 unx      412 b- defN 23-Aug-03 15:40 pycaret/preprocess/FixImbalancer.class
--rw-rw-r--  2.0 unx     2818 b- defN 23-Aug-03 15:40 pycaret/preprocess/RemoveMulticollinearity.class
--rw-rw-r--  2.0 unx      421 b- defN 23-Aug-03 15:40 pycaret/preprocess/CleanColumnNames.class
--rw-rw-r--  2.0 unx     1332 b- defN 23-Aug-03 15:40 pycaret/preprocess/RemoveOutliers$1.class
--rw-rw-r--  2.0 unx     2747 b- defN 23-Aug-03 15:40 pycaret/preprocess/RareCategoryGrouping.class
--rw-rw-r--  2.0 unx     3125 b- defN 23-Aug-03 15:40 pycaret/preprocess/RemoveOutliers.class
--rw-rw-r--  2.0 unx     7826 b- defN 23-Aug-03 15:40 pycaret/preprocess/TransformerWrapper.class
--rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-03 15:40 pycaret/preprocess/TransformerWrapperWithInverse.class
--rw-rw-r--  2.0 unx      720 b- defN 23-Aug-03 15:40 tpot/builtins/StackingEstimator$1.class
--rw-rw-r--  2.0 unx     4530 b- defN 23-Aug-03 15:40 tpot/builtins/StackingEstimator.class
--rw-rw-r--  2.0 unx     2433 b- defN 23-Aug-03 15:40 optbinning/BinnedFeature.class
--rw-rw-r--  2.0 unx     8333 b- defN 23-Aug-03 15:40 optbinning/scorecard/Scorecard.class
--rw-rw-r--  2.0 unx     2133 b- defN 23-Aug-03 15:40 optbinning/OptimalBinningUtil.class
--rw-rw-r--  2.0 unx     6372 b- defN 23-Aug-03 15:40 optbinning/BinningProcess.class
--rw-rw-r--  2.0 unx     2274 b- defN 23-Aug-03 15:40 optbinning/ContinuousOptimalBinning.class
--rw-rw-r--  2.0 unx     3917 b- defN 23-Aug-03 15:40 optbinning/MulticlassOptimalBinning.class
--rw-rw-r--  2.0 unx     1240 b- defN 23-Aug-03 15:40 optbinning/BinningProcess$1.class
--rw-rw-r--  2.0 unx    14050 b- defN 23-Aug-03 15:40 optbinning/OptimalBinning.class
--rw-rw-r--  2.0 unx      374 b- defN 23-Aug-03 15:40 imblearn/Sampler.class
--rw-rw-r--  2.0 unx     1916 b- defN 23-Aug-03 15:40 category_encoders/MapEncoder.class
--rw-rw-r--  2.0 unx     8449 b- defN 23-Aug-03 15:40 category_encoders/MapFeature.class
--rw-rw-r--  2.0 unx      527 b- defN 23-Aug-03 15:40 category_encoders/TargetEncoder.class
--rw-rw-r--  2.0 unx     1451 b- defN 23-Aug-03 15:40 category_encoders/CountEncoder$1.class
--rw-rw-r--  2.0 unx      515 b- defN 23-Aug-03 15:40 category_encoders/WOEEncoder.class
--rw-rw-r--  2.0 unx     8474 b- defN 23-Aug-03 15:40 category_encoders/MeanEncoder.class
--rw-rw-r--  2.0 unx     8520 b- defN 23-Aug-03 15:40 category_encoders/CountEncoder.class
--rw-rw-r--  2.0 unx    12815 b- defN 23-Aug-03 15:40 category_encoders/BaseNFeature.class
--rw-rw-r--  2.0 unx     1481 b- defN 23-Aug-03 15:40 category_encoders/OrdinalMapEncoder$1.class
--rw-rw-r--  2.0 unx     1445 b- defN 23-Aug-03 15:40 category_encoders/MeanEncoder$1.class
--rw-rw-r--  2.0 unx     2119 b- defN 23-Aug-03 15:40 category_encoders/OrdinalEncoder$Mapping.class
--rw-rw-r--  2.0 unx     1323 b- defN 23-Aug-03 15:40 category_encoders/LeaveOneOutEncoder$1.class
--rw-rw-r--  2.0 unx     8108 b- defN 23-Aug-03 15:40 category_encoders/OrdinalMapEncoder.class
--rw-rw-r--  2.0 unx     9241 b- defN 23-Aug-03 15:40 category_encoders/BaseNEncoder.class
--rw-rw-r--  2.0 unx     1334 b- defN 23-Aug-03 15:40 category_encoders/BinaryEncoder.class
--rw-rw-r--  2.0 unx     3547 b- defN 23-Aug-03 15:40 category_encoders/OneHotEncoder.class
--rw-rw-r--  2.0 unx     1325 b- defN 23-Aug-03 15:40 category_encoders/CatBoostEncoder.class
--rw-rw-r--  2.0 unx     2062 b- defN 23-Aug-03 15:40 category_encoders/CategoryEncoderUtil.class
--rw-rw-r--  2.0 unx     1564 b- defN 23-Aug-03 15:40 category_encoders/OrdinalEncoder$1.class
--rw-rw-r--  2.0 unx     1047 b- defN 23-Aug-03 15:40 category_encoders/LeaveOneOutEncoder.class
--rw-rw-r--  2.0 unx     4690 b- defN 23-Aug-03 15:40 category_encoders/OrdinalEncoder.class
--rw-rw-r--  2.0 unx      742 b- defN 23-Aug-03 15:40 category_encoders/MeanEncoder$MeanFunction.class
--rw-rw-r--  2.0 unx     1378 b- defN 23-Aug-03 15:40 category_encoders/CatBoostEncoder$1.class
--rw-rw-r--  2.0 unx     2162 b- defN 23-Aug-03 15:40 category_encoders/CategoryEncoder.class
--rw-rw-r--  2.0 unx      725 b- defN 23-Aug-03 15:40 sklego/meta/EstimatorTransformer$1.class
--rw-rw-r--  2.0 unx     7272 b- defN 23-Aug-03 15:40 sklego/meta/EstimatorTransformer.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-extension/
--rw-rw-r--  2.0 unx     1226 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
--rw-rw-r--  2.0 unx      118 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-05 19:08 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 pycaret/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 pycaret/pipeline/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 pycaret/preprocess/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 tpot/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 tpot/builtins/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 optbinning/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 optbinning/scorecard/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 imblearn/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 category_encoders/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 sklego/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 sklego/meta/
+-rw-rw-r--  2.0 unx     4312 b- defN 23-Aug-05 19:08 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx     2928 b- defN 23-Aug-05 19:08 pycaret/pipeline/Pipeline.class
+-rw-rw-r--  2.0 unx      412 b- defN 23-Aug-05 19:08 pycaret/preprocess/FixImbalancer.class
+-rw-rw-r--  2.0 unx     2818 b- defN 23-Aug-05 19:08 pycaret/preprocess/RemoveMulticollinearity.class
+-rw-rw-r--  2.0 unx      421 b- defN 23-Aug-05 19:08 pycaret/preprocess/CleanColumnNames.class
+-rw-rw-r--  2.0 unx     1332 b- defN 23-Aug-05 19:08 pycaret/preprocess/RemoveOutliers$1.class
+-rw-rw-r--  2.0 unx     2747 b- defN 23-Aug-05 19:08 pycaret/preprocess/RareCategoryGrouping.class
+-rw-rw-r--  2.0 unx     3125 b- defN 23-Aug-05 19:08 pycaret/preprocess/RemoveOutliers.class
+-rw-rw-r--  2.0 unx     7826 b- defN 23-Aug-05 19:08 pycaret/preprocess/TransformerWrapper.class
+-rw-rw-r--  2.0 unx     4170 b- defN 23-Aug-05 19:08 pycaret/preprocess/TransformerWrapperWithInverse.class
+-rw-rw-r--  2.0 unx      720 b- defN 23-Aug-05 19:08 tpot/builtins/StackingEstimator$1.class
+-rw-rw-r--  2.0 unx     4530 b- defN 23-Aug-05 19:08 tpot/builtins/StackingEstimator.class
+-rw-rw-r--  2.0 unx     2433 b- defN 23-Aug-05 19:08 optbinning/BinnedFeature.class
+-rw-rw-r--  2.0 unx     8333 b- defN 23-Aug-05 19:08 optbinning/scorecard/Scorecard.class
+-rw-rw-r--  2.0 unx     2133 b- defN 23-Aug-05 19:08 optbinning/OptimalBinningUtil.class
+-rw-rw-r--  2.0 unx     6372 b- defN 23-Aug-05 19:08 optbinning/BinningProcess.class
+-rw-rw-r--  2.0 unx     2274 b- defN 23-Aug-05 19:08 optbinning/ContinuousOptimalBinning.class
+-rw-rw-r--  2.0 unx     3917 b- defN 23-Aug-05 19:08 optbinning/MulticlassOptimalBinning.class
+-rw-rw-r--  2.0 unx     1240 b- defN 23-Aug-05 19:08 optbinning/BinningProcess$1.class
+-rw-rw-r--  2.0 unx    14050 b- defN 23-Aug-05 19:08 optbinning/OptimalBinning.class
+-rw-rw-r--  2.0 unx      374 b- defN 23-Aug-05 19:08 imblearn/Sampler.class
+-rw-rw-r--  2.0 unx     1916 b- defN 23-Aug-05 19:08 category_encoders/MapEncoder.class
+-rw-rw-r--  2.0 unx     8449 b- defN 23-Aug-05 19:08 category_encoders/MapFeature.class
+-rw-rw-r--  2.0 unx      527 b- defN 23-Aug-05 19:08 category_encoders/TargetEncoder.class
+-rw-rw-r--  2.0 unx     1451 b- defN 23-Aug-05 19:08 category_encoders/CountEncoder$1.class
+-rw-rw-r--  2.0 unx      515 b- defN 23-Aug-05 19:08 category_encoders/WOEEncoder.class
+-rw-rw-r--  2.0 unx     8474 b- defN 23-Aug-05 19:08 category_encoders/MeanEncoder.class
+-rw-rw-r--  2.0 unx     8520 b- defN 23-Aug-05 19:08 category_encoders/CountEncoder.class
+-rw-rw-r--  2.0 unx    12815 b- defN 23-Aug-05 19:08 category_encoders/BaseNFeature.class
+-rw-rw-r--  2.0 unx     1481 b- defN 23-Aug-05 19:08 category_encoders/OrdinalMapEncoder$1.class
+-rw-rw-r--  2.0 unx     1445 b- defN 23-Aug-05 19:08 category_encoders/MeanEncoder$1.class
+-rw-rw-r--  2.0 unx     2119 b- defN 23-Aug-05 19:08 category_encoders/OrdinalEncoder$Mapping.class
+-rw-rw-r--  2.0 unx     1323 b- defN 23-Aug-05 19:08 category_encoders/LeaveOneOutEncoder$1.class
+-rw-rw-r--  2.0 unx     8108 b- defN 23-Aug-05 19:08 category_encoders/OrdinalMapEncoder.class
+-rw-rw-r--  2.0 unx     9241 b- defN 23-Aug-05 19:08 category_encoders/BaseNEncoder.class
+-rw-rw-r--  2.0 unx     1334 b- defN 23-Aug-05 19:08 category_encoders/BinaryEncoder.class
+-rw-rw-r--  2.0 unx     3547 b- defN 23-Aug-05 19:08 category_encoders/OneHotEncoder.class
+-rw-rw-r--  2.0 unx     1325 b- defN 23-Aug-05 19:08 category_encoders/CatBoostEncoder.class
+-rw-rw-r--  2.0 unx     2062 b- defN 23-Aug-05 19:08 category_encoders/CategoryEncoderUtil.class
+-rw-rw-r--  2.0 unx     1564 b- defN 23-Aug-05 19:08 category_encoders/OrdinalEncoder$1.class
+-rw-rw-r--  2.0 unx     1047 b- defN 23-Aug-05 19:08 category_encoders/LeaveOneOutEncoder.class
+-rw-rw-r--  2.0 unx     4690 b- defN 23-Aug-05 19:08 category_encoders/OrdinalEncoder.class
+-rw-rw-r--  2.0 unx      742 b- defN 23-Aug-05 19:08 category_encoders/MeanEncoder$MeanFunction.class
+-rw-rw-r--  2.0 unx     1378 b- defN 23-Aug-05 19:08 category_encoders/CatBoostEncoder$1.class
+-rw-rw-r--  2.0 unx     2162 b- defN 23-Aug-05 19:08 category_encoders/CategoryEncoder.class
+-rw-rw-r--  2.0 unx      725 b- defN 23-Aug-05 19:08 sklego/meta/EstimatorTransformer$1.class
+-rw-rw-r--  2.0 unx     7272 b- defN 23-Aug-05 19:08 sklego/meta/EstimatorTransformer.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-extension/
+-rw-rw-r--  2.0 unx     1226 b- defN 23-Aug-05 19:07 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml
+-rw-rw-r--  2.0 unx      118 b- defN 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties
 65 files, 172173 bytes uncompressed, 75151 bytes compressed:  56.4%
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.34</version>
+    <version>1.7.35</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-extension</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn extensions converter</name>
   <description>JPMML Scikit-Learn extension packages to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-extension/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Thu Aug 03 15:40:51 EEST 2023
-version=1.7.34
+#Sat Aug 05 19:08:01 EEST 2023
+version=1.7.35
 groupId=org.jpmml
 artifactId=pmml-sklearn-extension
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.34.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-sklearn-xgboost-1.7.35.jar`

 * *Files 25% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 7977 bytes, number of entries: 15
-drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/
--rw-r--r--  2.0 unx      130 b- defN 23-Aug-03 15:40 META-INF/MANIFEST.MF
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 xgboost/
-drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-03 15:40 xgboost/sklearn/
--rw-rw-r--  2.0 unx      364 b- defN 23-Aug-03 15:40 META-INF/sklearn2pmml.properties
--rw-rw-r--  2.0 unx      168 b- defN 23-Aug-03 15:40 xgboost/sklearn/HasBooster.class
--rw-rw-r--  2.0 unx     2270 b- defN 23-Aug-03 15:40 xgboost/sklearn/XGBClassifier.class
--rw-rw-r--  2.0 unx     2210 b- defN 23-Aug-03 15:40 xgboost/sklearn/Booster.class
--rw-rw-r--  2.0 unx     2246 b- defN 23-Aug-03 15:40 xgboost/sklearn/XGBRegressor.class
--rw-rw-r--  2.0 unx     4204 b- defN 23-Aug-03 15:40 xgboost/sklearn/BoosterUtil.class
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/
-?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
--rw-rw-r--  2.0 unx     1453 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
--rw-rw-r--  2.0 unx      116 b- defN 23-Aug-03 15:40 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
-15 files, 13161 bytes uncompressed, 5921 bytes compressed:  55.0%
+Zip file size: 8245 bytes, number of entries: 15
+drwxr-xr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/
+-rw-r--r--  2.0 unx      130 b- defN 23-Aug-05 19:08 META-INF/MANIFEST.MF
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 xgboost/
+drwxrwxr-x  2.0 unx        0 b- stor 23-Aug-05 19:08 xgboost/sklearn/
+-rw-rw-r--  2.0 unx      364 b- defN 23-Aug-05 19:08 META-INF/sklearn2pmml.properties
+-rw-rw-r--  2.0 unx      168 b- defN 23-Aug-05 19:08 xgboost/sklearn/HasBooster.class
+-rw-rw-r--  2.0 unx     2440 b- defN 23-Aug-05 19:08 xgboost/sklearn/XGBClassifier.class
+-rw-rw-r--  2.0 unx     2210 b- defN 23-Aug-05 19:08 xgboost/sklearn/Booster.class
+-rw-rw-r--  2.0 unx     2416 b- defN 23-Aug-05 19:08 xgboost/sklearn/XGBRegressor.class
+-rw-rw-r--  2.0 unx     4855 b- defN 23-Aug-05 19:08 xgboost/sklearn/BoosterUtil.class
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/
+?rwsrwsrwt  2.0 unx        0 b- stor 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/
+-rw-rw-r--  2.0 unx     1453 b- defN 23-Aug-05 19:07 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml
+-rw-rw-r--  2.0 unx      116 b- defN 23-Aug-05 19:08 META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties
+15 files, 14152 bytes uncompressed, 6189 bytes compressed:  56.3%
```

#### xgboost/sklearn/XGBClassifier.class

##### procyon -ec {}

```diff
@@ -1,22 +1,24 @@
 
 package xgboost.sklearn;
 
 import org.dmg.pmml.Model;
+import org.dmg.pmml.PMML;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import org.jpmml.xgboost.ObjFunction;
 import org.jpmml.xgboost.Classification;
 import org.jpmml.converter.Label;
 import org.dmg.pmml.DataType;
 import sklearn.Estimator;
+import org.jpmml.sklearn.Encodable;
 import org.jpmml.xgboost.HasXGBoostOptions;
 import sklearn.LabelEncoderClassifier;
 
-public class XGBClassifier extends LabelEncoderClassifier implements HasBooster, HasXGBoostOptions
+public class XGBClassifier extends LabelEncoderClassifier implements HasBooster, HasXGBoostOptions, Encodable
 {
     public XGBClassifier(final String module, final String name) {
         super(module, name);
     }
     
     public int getNumberOfFeatures() {
         return BoosterUtil.getNumberOfFeatures((Estimator)this);
@@ -31,14 +33,18 @@
         super.checkLabel(label);
         if (objFunction != null && !(objFunction instanceof Classification)) {
             throw new IllegalArgumentException("Expected a classification-type objective function, got '" + objFunction.getName() + "'");
         }
     }
     
     public MiningModel encodeModel(final Schema schema) {
-        return BoosterUtil.encodeBooster((Estimator)this, schema);
+        return BoosterUtil.encodeModel((Estimator)this, schema);
+    }
+    
+    public PMML encodePMML() {
+        return BoosterUtil.encodePMML((Estimator)this);
     }
     
     public Booster getBooster() {
         return (Booster)this.get("_Booster", (Class)Booster.class);
     }
 }
```

#### xgboost/sklearn/XGBRegressor.class

##### procyon -ec {}

```diff
@@ -1,22 +1,24 @@
 
 package xgboost.sklearn;
 
 import org.dmg.pmml.Model;
+import org.dmg.pmml.PMML;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import org.jpmml.xgboost.ObjFunction;
 import org.jpmml.xgboost.Regression;
 import org.jpmml.converter.Label;
 import org.dmg.pmml.DataType;
 import sklearn.Estimator;
+import org.jpmml.sklearn.Encodable;
 import org.jpmml.xgboost.HasXGBoostOptions;
 import sklearn.Regressor;
 
-public class XGBRegressor extends Regressor implements HasBooster, HasXGBoostOptions
+public class XGBRegressor extends Regressor implements HasBooster, HasXGBoostOptions, Encodable
 {
     public XGBRegressor(final String module, final String name) {
         super(module, name);
     }
     
     public int getNumberOfFeatures() {
         return BoosterUtil.getNumberOfFeatures((Estimator)this);
@@ -31,14 +33,18 @@
         super.checkLabel(label);
         if (objFunction != null && !(objFunction instanceof Regression)) {
             throw new IllegalArgumentException("Expected a regression-type objective function, got '" + objFunction.getName() + "'");
         }
     }
     
     public MiningModel encodeModel(final Schema schema) {
-        return BoosterUtil.encodeBooster((Estimator)this, schema);
+        return BoosterUtil.encodeModel((Estimator)this, schema);
+    }
+    
+    public PMML encodePMML() {
+        return BoosterUtil.encodePMML((Estimator)this);
     }
     
     public Booster getBooster() {
         return (Booster)this.get("_Booster", (Class)Booster.class);
     }
 }
```

#### xgboost/sklearn/BoosterUtil.class

##### procyon -ec {}

```diff
@@ -1,12 +1,15 @@
 
 package xgboost.sklearn;
 
 import org.jpmml.xgboost.ByteOrderUtil;
 import java.nio.ByteOrder;
+import org.jpmml.xgboost.FeatureMap;
+import java.util.List;
+import org.dmg.pmml.PMML;
 import org.jpmml.xgboost.GBTree;
 import java.util.Map;
 import java.util.LinkedHashMap;
 import org.dmg.pmml.mining.MiningModel;
 import org.jpmml.converter.Schema;
 import org.jpmml.xgboost.ObjFunction;
 import org.jpmml.xgboost.Learner;
@@ -24,15 +27,15 @@
     }
     
     public static <E extends Estimator & HasBooster & HasXGBoostOptions> ObjFunction getObjFunction(final E estimator) {
         final Learner learner = getLearner(estimator);
         return learner.obj();
     }
     
-    public static <E extends Estimator & HasBooster & HasXGBoostOptions> MiningModel encodeBooster(final E estimator, final Schema schema) {
+    public static <E extends Estimator & HasBooster & HasXGBoostOptions> MiningModel encodeModel(final E estimator, final Schema schema) {
         final Booster booster = ((E)estimator).getBooster();
         Integer bestNTreeLimit = booster.getBestNTreeLimit();
         final Learner learner = getLearner(estimator);
         final GBTree gbtree = learner.gbtree();
         if (bestNTreeLimit == null) {
             bestNTreeLimit = (Integer)estimator.getOptionalScalar("best_ntree_limit");
         }
@@ -48,14 +51,21 @@
         options.put("prune", prune);
         options.put("ntree_limit", ntreeLimit);
         final Schema xgbSchema = learner.toXGBoostSchema((boolean)numeric, schema);
         final MiningModel miningModel = learner.encodeMiningModel((Map)options, xgbSchema);
         return miningModel;
     }
     
+    public static <E extends Estimator & HasBooster & HasXGBoostOptions> PMML encodePMML(final E estimator) {
+        final Learner learner = getLearner(estimator);
+        final FeatureMap featureMap = learner.encodeFeatureMap();
+        final Map<String, ?> options = ((E)estimator).getNativeConfiguration();
+        return learner.encodePMML((Map)options, (String)null, (List)null, featureMap);
+    }
+    
     private static <E extends Estimator & HasBooster & HasXGBoostOptions> Learner getLearner(final E estimator) {
         final Booster booster = ((E)estimator).getBooster();
         final String byteOrder = (String)estimator.getOption("byte_order", (Object)ByteOrder.nativeOrder().toString());
         final String charset = (String)estimator.getOption("charset", (Object)null);
         return booster.getLearner(ByteOrderUtil.forValue(byteOrder), charset);
     }
 }
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

##### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.xml

```diff
@@ -1,14 +1,14 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project xmlns="http://maven.apache.org/POM/4.0.0" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
   <modelVersion>4.0.0</modelVersion>
   <parent>
     <groupId>org.jpmml</groupId>
     <artifactId>jpmml-sklearn</artifactId>
-    <version>1.7.34</version>
+    <version>1.7.35</version>
   </parent>
   <groupId>org.jpmml</groupId>
   <artifactId>pmml-sklearn-xgboost</artifactId>
   <packaging>jar</packaging>
   <name>JPMML SkLearn XGBoost converter</name>
   <description>JPMML Scikit-Learn XGBoost to PMML converter</description>
   <licenses>
```

#### META-INF/maven/org.jpmml/pmml-sklearn-xgboost/pom.properties

```diff
@@ -1,5 +1,5 @@
 #Generated by Maven
-#Thu Aug 03 15:40:52 EEST 2023
-version=1.7.34
+#Sat Aug 05 19:08:01 EEST 2023
+version=1.7.35
 groupId=org.jpmml
 artifactId=pmml-sklearn-xgboost
```

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-statsmodels-1.0.5.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pickle-1.4.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pickle-1.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar` & `sklearn2pmml-0.97.1/sklearn2pmml/resources/pmml-xgboost-1.7.4.jar`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/h2o.py` & `sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/h2o.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/xgboost.py` & `sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/xgboost.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/preprocessing/lightgbm.py` & `sklearn2pmml-0.97.1/sklearn2pmml/preprocessing/lightgbm.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/tree/chaid.py` & `sklearn2pmml-0.97.1/sklearn2pmml/tree/chaid.py`

 * *Files identical despite different names*

### Comparing `sklearn2pmml-0.97.0/sklearn2pmml/expression/__init__.py` & `sklearn2pmml-0.97.1/sklearn2pmml/expression/__init__.py`

 * *Files identical despite different names*

