# Comparing `tmp/botocore-a-la-carte-ec2-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-ec2-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-ec2-1.31.8.tar", last modified: Fri Jul 21 01:21:26 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-ec2-1.31.9.tar", last modified: Sat Jul 22 01:20:29 2023, max compression
```

## Comparing `botocore-a-la-carte-ec2-1.31.8.tar` & `botocore-a-la-carte-ec2-1.31.9.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.611026 botocore-a-la-carte-ec2-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:26.000000 botocore-a-la-carte-ec2-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-21 01:21:26.611026 botocore-a-la-carte-ec2-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.599025 botocore-a-la-carte-ec2-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.599025 botocore-a-la-carte-ec2-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.599025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.603025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   539923 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.603025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   566499 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.603025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   588390 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.603025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   715324 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.607025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   847080 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.607025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   109914 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   878250 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.607025 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/
--rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   110174 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   891280 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.611026 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   147949 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)  2872499 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-07-21 01:21:06.000000 botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:26.611026 botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-21 01:21:26.000000 botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-21 01:21:26.000000 botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:26.000000 botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:26.000000 botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:26.611026 botocore-a-la-carte-ec2-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-21 01:21:26.000000 botocore-a-la-carte-ec2-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.156983 botocore-a-la-carte-ec2-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:28.000000 botocore-a-la-carte-ec2-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-22 01:20:29.156983 botocore-a-la-carte-ec2-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.144983 botocore-a-la-carte-ec2-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.144983 botocore-a-la-carte-ec2-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.144983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.144983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   539923 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8548 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.144983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   566499 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.144983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   588390 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11040 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.148983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   715324 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11546 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.148983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   847080 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14823 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.148983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109914 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   878250 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15259 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.152983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    14695 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   110174 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   891280 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14875 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.156983 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   147949 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    26102 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/paginators-1.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2872499 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)    17748 2023-07-22 01:20:09.000000 botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:29.156983 botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-22 01:20:29.000000 botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-22 01:20:29.000000 botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:29.000000 botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:29.000000 botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:29.156983 botocore-a-la-carte-ec2-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-22 01:20:28.000000 botocore-a-la-carte-ec2-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-ec2-1.31.8/LICENSE.txt` & `botocore-a-la-carte-ec2-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/PKG-INFO` & `botocore-a-la-carte-ec2-1.31.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.31.8
+Version: 1.31.9
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-09-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-09-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2014-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2014-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-03-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-03-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-04-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-04-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2015-10-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2015-10-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/examples-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-04-01/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-04-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/examples-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-09-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-09-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/examples-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/paginators-1.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/service-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore/data/ec2/2016-11-15/waiters-2.json` & `botocore-a-la-carte-ec2-1.31.9/botocore/data/ec2/2016-11-15/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/PKG-INFO` & `botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-ec2
-Version: 1.31.8
+Version: 1.31.9
 Summary: ec2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-ec2-1.31.8/botocore_a_la_carte_ec2.egg-info/SOURCES.txt` & `botocore-a-la-carte-ec2-1.31.9/botocore_a_la_carte_ec2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-ec2-1.31.8/setup.py` & `botocore-a-la-carte-ec2-1.31.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-ec2',
-    version="1.31.8",
+    version="1.31.9",
     description='ec2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/ec2/*/*.json'],
```

