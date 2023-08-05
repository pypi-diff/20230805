# Comparing `tmp/botocore-a-la-carte-rds-1.31.8.tar.gz` & `tmp/botocore-a-la-carte-rds-1.31.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-rds-1.31.8.tar", last modified: Fri Jul 21 01:21:48 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-rds-1.31.9.tar", last modified: Sat Jul 22 01:20:49 2023, max compression
```

## Comparing `botocore-a-la-carte-rds-1.31.8.tar` & `botocore-a-la-carte-rds-1.31.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.219428 botocore-a-la-carte-rds-1.31.8/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-21 01:21:48.000000 botocore-a-la-carte-rds-1.31.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-21 01:21:48.219428 botocore-a-la-carte-rds-1.31.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.215428 botocore-a-la-carte-rds-1.31.8/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.215428 botocore-a-la-carte-rds-1.31.8/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.215428 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.215428 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/
--rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   326067 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.219428 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/
--rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)    57903 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   969933 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/service-2.sdk-extras.json
--rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-21 01:21:06.000000 botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-21 01:21:48.219428 botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-21 01:21:48.000000 botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-21 01:21:48.000000 botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-21 01:21:48.000000 botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-21 01:21:48.000000 botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-21 01:21:48.219428 botocore-a-la-carte-rds-1.31.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-21 01:21:48.000000 botocore-a-la-carte-rds-1.31.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-22 01:20:49.000000 botocore-a-la-carte-rds-1.31.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/
+-rw-r--r--   0 runner    (1001) docker     (123)    20411 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   326067 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/
+-rw-r--r--   0 runner    (1001) docker     (123)    19575 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57903 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6308 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   970766 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/service-2.sdk-extras.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9673 2023-07-22 01:20:09.000000 botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-22 01:20:49.000000 botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-22 01:20:49.000000 botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 01:20:49.000000 botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-22 01:20:49.000000 botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-22 01:20:49.477296 botocore-a-la-carte-rds-1.31.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-22 01:20:49.000000 botocore-a-la-carte-rds-1.31.9/setup.py
```

### Comparing `botocore-a-la-carte-rds-1.31.8/LICENSE.txt` & `botocore-a-la-carte-rds-1.31.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/PKG-INFO` & `botocore-a-la-carte-rds-1.31.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rds
-Version: 1.31.8
+Version: 1.31.9
 Summary: rds data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/paginators-1.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/service-2.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-09-01/waiters-2.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-09-01/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/examples-1.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/examples-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/paginators-1.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/service-2.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998749927503237%*

 * *Differences: {"'operations'": "{'DeleteBlueGreenDeployment': {'documentation': '<p>Deletes a blue/green "*

 * *                 'deployment.</p> <p>For more information, see <a '*

 * *                 'href="https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html">Using '*

 * *                 'Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS '*

 * *                 'User Guide</i> and <a '*

 * *                 'href="https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-gre […]*

```diff
@@ -1026,15 +1026,15 @@
             "name": "CreateOptionGroup",
             "output": {
                 "resultWrapper": "CreateOptionGroupResult",
                 "shape": "CreateOptionGroupResult"
             }
         },
         "DeleteBlueGreenDeployment": {
-            "documentation": "<p>Deletes a blue/green deployment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\"> Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
+            "documentation": "<p>Deletes a blue/green deployment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "BlueGreenDeploymentNotFoundFault"
                 },
                 {
                     "shape": "InvalidBlueGreenDeploymentStateFault"
                 }
@@ -1468,15 +1468,15 @@
             "name": "DescribeAccountAttributes",
             "output": {
                 "resultWrapper": "DescribeAccountAttributesResult",
                 "shape": "AccountAttributesMessage"
             }
         },
         "DescribeBlueGreenDeployments": {
-            "documentation": "<p>Returns information about blue/green deployments.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\"> Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
+            "documentation": "<p>Describes one or more blue/green deployments.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\"> Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "BlueGreenDeploymentNotFoundFault"
                 }
             ],
             "http": {
                 "method": "POST",
@@ -4020,15 +4020,15 @@
             "name": "StopDBInstanceAutomatedBackupsReplication",
             "output": {
                 "resultWrapper": "StopDBInstanceAutomatedBackupsReplicationResult",
                 "shape": "StopDBInstanceAutomatedBackupsReplicationResult"
             }
         },
         "SwitchoverBlueGreenDeployment": {
-            "documentation": "<p>Switches over a blue/green deployment.</p> <p>Before you switch over, production traffic is routed to the databases in the blue environment. After you switch over, production traffic is routed to the databases in the green environment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\"> Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
+            "documentation": "<p>Switches over a blue/green deployment.</p> <p>Before you switch over, production traffic is routed to the databases in the blue environment. After you switch over, production traffic is routed to the databases in the green environment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
             "errors": [
                 {
                     "shape": "BlueGreenDeploymentNotFoundFault"
                 },
                 {
                     "shape": "InvalidBlueGreenDeploymentStateFault"
                 }
@@ -4451,38 +4451,38 @@
                 "senderFault": true
             },
             "exception": true,
             "members": {},
             "type": "structure"
         },
         "BlueGreenDeployment": {
-            "documentation": "<p>Contains the details about a blue/green deployment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\"> Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
+            "documentation": "<p>Details about a blue/green deployment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
             "members": {
                 "BlueGreenDeploymentIdentifier": {
-                    "documentation": "<p>The system-generated identifier of the blue/green deployment.</p>",
+                    "documentation": "<p>The unique identifier of the blue/green deployment.</p>",
                     "shape": "BlueGreenDeploymentIdentifier"
                 },
                 "BlueGreenDeploymentName": {
                     "documentation": "<p>The user-supplied name of the blue/green deployment.</p>",
                     "shape": "BlueGreenDeploymentName"
                 },
                 "CreateTime": {
-                    "documentation": "<p>Specifies the time when the blue/green deployment was created, in Universal Coordinated Time (UTC).</p>",
+                    "documentation": "<p>The time when the blue/green deployment was created, in Universal Coordinated Time (UTC).</p>",
                     "shape": "TStamp"
                 },
                 "DeleteTime": {
-                    "documentation": "<p>Specifies the time when the blue/green deployment was deleted, in Universal Coordinated Time (UTC).</p>",
+                    "documentation": "<p>The time when the blue/green deployment was deleted, in Universal Coordinated Time (UTC).</p>",
                     "shape": "TStamp"
                 },
                 "Source": {
                     "documentation": "<p>The source database for the blue/green deployment.</p> <p>Before switchover, the source database is the production database in the blue environment.</p>",
                     "shape": "DatabaseArn"
                 },
                 "Status": {
-                    "documentation": "<p>The status of the blue/green deployment.</p> <p>Values:</p> <ul> <li> <p> <code>PROVISIONING</code> - Resources are being created in the green environment.</p> </li> <li> <p> <code>AVAILABLE</code> - Resources are available in the green environment.</p> </li> <li> <p> <code>SWITCHOVER_IN_PROGRESS</code> - The deployment is being switched from the blue environment to the green environment.</p> </li> <li> <p> <code>SWITCHOVER_COMPLETED</code> - Switchover from the blue environment to the green environment is complete.</p> </li> <li> <p> <code>INVALID_CONFIGURATION</code> - Resources in the green environment are invalid, so switchover isn't possible.</p> </li> <li> <p> <code>SWITCHOVER_FAILED</code> - Switchover was attempted but failed.</p> </li> <li> <p> <code>DELETING</code> - The blue/green deployment is being deleted.</p> </li> </ul>",
+                    "documentation": "<p>The status of the blue/green deployment.</p> <p>Valid Values:</p> <ul> <li> <p> <code>PROVISIONING</code> - Resources are being created in the green environment.</p> </li> <li> <p> <code>AVAILABLE</code> - Resources are available in the green environment.</p> </li> <li> <p> <code>SWITCHOVER_IN_PROGRESS</code> - The deployment is being switched from the blue environment to the green environment.</p> </li> <li> <p> <code>SWITCHOVER_COMPLETED</code> - Switchover from the blue environment to the green environment is complete.</p> </li> <li> <p> <code>INVALID_CONFIGURATION</code> - Resources in the green environment are invalid, so switchover isn't possible.</p> </li> <li> <p> <code>SWITCHOVER_FAILED</code> - Switchover was attempted but failed.</p> </li> <li> <p> <code>DELETING</code> - The blue/green deployment is being deleted.</p> </li> </ul>",
                     "shape": "BlueGreenDeploymentStatus"
                 },
                 "StatusDetails": {
                     "documentation": "<p>Additional information about the status of the blue/green deployment.</p>",
                     "shape": "BlueGreenDeploymentStatusDetails"
                 },
                 "SwitchoverDetails": {
@@ -4546,22 +4546,22 @@
         "BlueGreenDeploymentStatus": {
             "type": "string"
         },
         "BlueGreenDeploymentStatusDetails": {
             "type": "string"
         },
         "BlueGreenDeploymentTask": {
-            "documentation": "<p>Contains the details about a task for a blue/green deployment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\"> Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
+            "documentation": "<p>Details about a task for a blue/green deployment.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon RDS User Guide</i> and <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/AuroraUserGuide/blue-green-deployments.html\">Using Amazon RDS Blue/Green Deployments for database updates</a> in the <i>Amazon Aurora User Guide</i>.</p>",
             "members": {
                 "Name": {
                     "documentation": "<p>The name of the blue/green deployment task.</p>",
                     "shape": "BlueGreenDeploymentTaskName"
                 },
                 "Status": {
-                    "documentation": "<p>The status of the blue/green deployment task.</p> <p>Values:</p> <ul> <li> <p> <code>PENDING</code> - The resources are being prepared for deployment.</p> </li> <li> <p> <code>IN_PROGRESS</code> - The resource is being deployed.</p> </li> <li> <p> <code>COMPLETED</code> - The resource has been deployed.</p> </li> <li> <p> <code>FAILED</code> - Deployment of the resource failed.</p> </li> </ul>",
+                    "documentation": "<p>The status of the blue/green deployment task.</p> <p>Valid Values:</p> <ul> <li> <p> <code>PENDING</code> - The resource is being prepared for deployment.</p> </li> <li> <p> <code>IN_PROGRESS</code> - The resource is being deployed.</p> </li> <li> <p> <code>COMPLETED</code> - The resource has been deployed.</p> </li> <li> <p> <code>FAILED</code> - Deployment of the resource failed.</p> </li> </ul>",
                     "shape": "BlueGreenDeploymentTaskStatus"
                 }
             },
             "type": "structure"
         },
         "BlueGreenDeploymentTaskList": {
             "member": {
@@ -5471,29 +5471,33 @@
                     "shape": "String"
                 },
                 "DBInstanceIdentifier": {
                     "documentation": "<p>The identifier for this DB instance. This parameter is stored as a lowercase string.</p> <p>Constraints:</p> <ul> <li> <p>Must contain from 1 to 63 letters, numbers, or hyphens.</p> </li> <li> <p>First character must be a letter.</p> </li> <li> <p>Can't end with a hyphen or contain two consecutive hyphens.</p> </li> </ul> <p>Example: <code>mydbinstance</code> </p>",
                     "shape": "String"
                 },
                 "DBName": {
-                    "documentation": "<p>The meaning of this parameter differs depending on the database engine.</p> <dl> <dt>Amazon Aurora MySQL</dt> <dd> <p>The name of the database to create when the primary DB instance of the Aurora MySQL DB cluster is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB cluster.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 alphanumeric characters.</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>Amazon Aurora PostgreSQL</dt> <dd> <p>The name of the database to create when the primary DB instance of the Aurora PostgreSQL DB cluster is created.</p> <p>Default: <code>postgres</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 alphanumeric characters.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0 to 9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>Amazon RDS Custom for Oracle</dt> <dd> <p>The Oracle System ID (SID) of the created RDS Custom DB instance.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 8 alphanumeric characters.</p> </li> <li> <p>Must contain a letter.</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>Amazon RDS Custom for SQL Server</dt> <dd> <p>Not applicable. Must be null.</p> </dd> <dt>RDS for MariaDB</dt> <dd> <p>The name of the database to create when the DB instance is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>RDS for MySQL</dt> <dd> <p>The name of the database to create when the DB instance is created. If you don't specify a value, Amazon RDS doesn't create a database in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>RDS for Oracle</dt> <dd> <p>The Oracle System ID (SID) of the created DB instance.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 8 characters.</p> </li> <li> <p>Can't be a word reserved by the database engine, such as the string <code>NULL</code>.</p> </li> </ul> </dd> <dt>RDS for PostgreSQL</dt> <dd> <p>The name of the database to create when the DB instance is created.</p> <p>Default: <code>postgres</code> </p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 letters, numbers, or underscores.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the database engine.</p> </li> </ul> </dd> <dt>RDS for SQL Server</dt> <dd> <p>Not applicable. Must be null.</p> </dd> </dl>",
+                    "documentation": "<p>The meaning of this parameter differs according to the database engine you use.</p> <p> <b>MySQL</b> </p> <p>The name of the database to create when the DB instance is created. If this parameter isn't specified, no database is created in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the specified database engine</p> </li> </ul> <p> <b>MariaDB</b> </p> <p>The name of the database to create when the DB instance is created. If this parameter isn't specified, no database is created in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 64 letters or numbers.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the specified database engine</p> </li> </ul> <p> <b>PostgreSQL</b> </p> <p>The name of the database to create when the DB instance is created. If this parameter isn't specified, a database named <code>postgres</code> is created in the DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must contain 1 to 63 letters, numbers, or underscores.</p> </li> <li> <p>Must begin with a letter. Subsequent characters can be letters, underscores, or digits (0-9).</p> </li> <li> <p>Can't be a word reserved by the specified database engine</p> </li> </ul> <p> <b>Oracle</b> </p> <p>The Oracle System ID (SID) of the created DB instance. If you don't specify a value, the default value is <code>ORCL</code>. You can't specify the string <code>null</code>, or any other reserved word, for <code>DBName</code>.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>Can't be longer than 8 characters</p> </li> </ul> <p> <b>Amazon RDS Custom for Oracle</b> </p> <p>The Oracle System ID (SID) of the created RDS Custom DB instance. If you don't specify a value, the default value is <code>ORCL</code> for non-CDBs and <code>RDSCDB</code> for CDBs.</p> <p>Default: <code>ORCL</code> </p> <p>Constraints:</p> <ul> <li> <p>It must contain 1 to 8 alphanumeric characters.</p> </li> <li> <p>It must contain a letter.</p> </li> <li> <p>It can't be a word reserved by the database engine.</p> </li> </ul> <p> <b>Amazon RDS Custom for SQL Server</b> </p> <p>Not applicable. Must be null.</p> <p> <b>SQL Server</b> </p> <p>Not applicable. Must be null.</p> <p> <b>Amazon Aurora MySQL</b> </p> <p>The name of the database to create when the primary DB instance of the Aurora MySQL DB cluster is created. If this parameter isn't specified for an Aurora MySQL DB cluster, no database is created in the DB cluster.</p> <p>Constraints:</p> <ul> <li> <p>It must contain 1 to 64 alphanumeric characters.</p> </li> <li> <p>It can't be a word reserved by the database engine.</p> </li> </ul> <p> <b>Amazon Aurora PostgreSQL</b> </p> <p>The name of the database to create when the primary DB instance of the Aurora PostgreSQL DB cluster is created. If this parameter isn't specified for an Aurora PostgreSQL DB cluster, a database named <code>postgres</code> is created in the DB cluster.</p> <p>Constraints:</p> <ul> <li> <p>It must contain 1 to 63 alphanumeric characters.</p> </li> <li> <p>It must begin with a letter. Subsequent characters can be letters, underscores, or digits (0 to 9).</p> </li> <li> <p>It can't be a word reserved by the database engine.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "DBParameterGroupName": {
                     "documentation": "<p>The name of the DB parameter group to associate with this DB instance. If you don't specify a value, then Amazon RDS uses the default DB parameter group for the specified DB engine and version.</p> <p>This setting doesn't apply to RDS Custom DB instances.</p> <p>Constraints:</p> <ul> <li> <p>Must be 1 to 255 letters, numbers, or hyphens.</p> </li> <li> <p>The first character must be a letter.</p> </li> <li> <p>Can't end with a hyphen or contain two consecutive hyphens.</p> </li> </ul>",
                     "shape": "String"
                 },
                 "DBSecurityGroups": {
                     "documentation": "<p>A list of DB security groups to associate with this DB instance.</p> <p>This setting applies to the legacy EC2-Classic platform, which is no longer used to create new DB instances. Use the <code>VpcSecurityGroupIds</code> setting instead.</p>",
                     "shape": "DBSecurityGroupNameList"
                 },
                 "DBSubnetGroupName": {
                     "documentation": "<p>A DB subnet group to associate with this DB instance.</p> <p>Constraints:</p> <ul> <li> <p>Must match the name of an existing DB subnet group.</p> </li> <li> <p>Must not be <code>default</code>.</p> </li> </ul> <p>Example: <code>mydbsubnetgroup</code> </p>",
                     "shape": "String"
                 },
+                "DBSystemId": {
+                    "documentation": "<p>The Oracle system identifier (SID), which is the name of the Oracle database instance that manages your database files. In this context, the term \"Oracle database instance\" refers exclusively to the system global area (SGA) and Oracle background processes. If you don't specify a SID, the value defaults to <code>RDSCDB</code>. The Oracle SID is also the name of your CDB.</p>",
+                    "shape": "String"
+                },
                 "DeletionProtection": {
                     "documentation": "<p>Specifies whether the DB instance has deletion protection enabled. The database can't be deleted when deletion protection is enabled. By default, deletion protection isn't enabled. For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/USER_DeleteInstance.html\"> Deleting a DB Instance</a>.</p> <p>This setting doesn't apply to Amazon Aurora DB instances. You can enable or disable deletion protection for the DB cluster. For more information, see <code>CreateDBCluster</code>. DB instances in a DB cluster can be deleted even when deletion protection is enabled for the DB cluster.</p>",
                     "shape": "BooleanOptional"
                 },
                 "Domain": {
                     "documentation": "<p>The Active Directory directory ID to create the DB instance in. Currently, only Microsoft SQL Server, MySQL, Oracle, and PostgreSQL DB instances can be created in an Active Directory Domain.</p> <p>For more information, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/kerberos-authentication.html\"> Kerberos Authentication</a> in the <i>Amazon RDS User Guide</i>.</p> <p>This setting doesn't apply to the following DB instances:</p> <ul> <li> <p>Amazon Aurora (The domain is managed by the DB cluster.)</p> </li> <li> <p>RDS Custom</p> </li> </ul>",
                     "shape": "String"
@@ -7468,15 +7472,15 @@
                     "shape": "String"
                 },
                 "DBInstanceStatus": {
                     "documentation": "<p>The current state of this database.</p> <p>For information about DB instance statuses, see <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/accessing-monitoring.html#Overview.DBInstance.Status\">Viewing DB instance status</a> in the <i>Amazon RDS User Guide.</i> </p>",
                     "shape": "String"
                 },
                 "DBName": {
-                    "documentation": "<p>The meaning of this parameter differs depending on the database engine.</p> <ul> <li> <p>For RDS for MariaDB, Microsoft SQL Server, MySQL, and PostgreSQL - The name of the initial database specified for this DB instance when it was created, if one was provided. This same name is returned for the life of the DB instance.</p> </li> <li> <p>For RDS for Oracle - The Oracle System ID (SID) of the created DB instance. This value is only returned when the object returned is an Oracle DB instance.</p> </li> </ul>",
+                    "documentation": "<p>Contains the initial database name that you provided (if required) when you created the DB instance. This name is returned for the life of your DB instance. For an RDS for Oracle CDB instance, the name identifies the PDB rather than the CDB.</p>",
                     "shape": "String"
                 },
                 "DBParameterGroups": {
                     "documentation": "<p>The list of DB parameter groups applied to this DB instance.</p>",
                     "shape": "DBParameterGroupStatusList"
                 },
                 "DBSecurityGroups": {
@@ -8626,14 +8630,18 @@
                     "documentation": "<p>The Amazon Resource Name (ARN) for the DB snapshot.</p>",
                     "shape": "String"
                 },
                 "DBSnapshotIdentifier": {
                     "documentation": "<p>Specifies the identifier for the DB snapshot.</p>",
                     "shape": "String"
                 },
+                "DBSystemId": {
+                    "documentation": "<p>The Oracle system identifier (SID), which is the name of the Oracle database instance that manages your database files. The Oracle SID is also the name of your CDB.</p>",
+                    "shape": "String"
+                },
                 "DbiResourceId": {
                     "documentation": "<p>The identifier for the source DB instance, which can't be changed and which is unique to an Amazon Web Services Region.</p>",
                     "shape": "String"
                 },
                 "Encrypted": {
                     "documentation": "<p>Specifies whether the DB snapshot is encrypted.</p>",
                     "shape": "Boolean"
@@ -8963,19 +8971,19 @@
             "min": 1,
             "pattern": "^arn:[A-Za-z][0-9A-Za-z-:._]*",
             "type": "string"
         },
         "DeleteBlueGreenDeploymentRequest": {
             "members": {
                 "BlueGreenDeploymentIdentifier": {
-                    "documentation": "<p>The blue/green deployment identifier of the deployment to be deleted. This parameter isn't case-sensitive.</p> <p>Constraints: </p> <ul> <li> <p>Must match an existing blue/green deployment identifier.</p> </li> </ul>",
+                    "documentation": "<p>The unique identifier of the blue/green deployment to delete. This parameter isn't case-sensitive.</p> <p>Constraints: </p> <ul> <li> <p>Must match an existing blue/green deployment identifier.</p> </li> </ul>",
                     "shape": "BlueGreenDeploymentIdentifier"
                 },
                 "DeleteTarget": {
-                    "documentation": "<p>A value that indicates whether to delete the resources in the green environment. You can't specify this option if the blue/green deployment <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/APIReference/API_BlueGreenDeployment.html\">status</a> is <code>SWITCHOVER_COMPLETED</code>.</p>",
+                    "documentation": "<p>Specifies whether to delete the resources in the green environment. You can't specify this option if the blue/green deployment <a href=\"https://docs.aws.amazon.com/AmazonRDS/latest/APIReference/API_BlueGreenDeployment.html\">status</a> is <code>SWITCHOVER_COMPLETED</code>.</p>",
                     "shape": "BooleanOptional"
                 }
             },
             "required": [
                 "BlueGreenDeploymentIdentifier"
             ],
             "type": "structure"
@@ -9323,40 +9331,40 @@
             "documentation": "<p/>",
             "members": {},
             "type": "structure"
         },
         "DescribeBlueGreenDeploymentsRequest": {
             "members": {
                 "BlueGreenDeploymentIdentifier": {
-                    "documentation": "<p>The blue/green deployment identifier. If this parameter is specified, information from only the specific blue/green deployment is returned. This parameter isn't case-sensitive.</p> <p>Constraints:</p> <ul> <li> <p>If supplied, must match an existing blue/green deployment identifier.</p> </li> </ul>",
+                    "documentation": "<p>The blue/green deployment identifier. If you specify this parameter, the response only includes information about the specific blue/green deployment. This parameter isn't case-sensitive.</p> <p>Constraints:</p> <ul> <li> <p>Must match an existing blue/green deployment identifier.</p> </li> </ul>",
                     "shape": "BlueGreenDeploymentIdentifier"
                 },
                 "Filters": {
-                    "documentation": "<p>A filter that specifies one or more blue/green deployments to describe.</p> <p>Supported filters:</p> <ul> <li> <p> <code>blue-green-deployment-identifier</code> - Accepts system-generated identifiers for blue/green deployments. The results list only includes information about the blue/green deployments with the specified identifiers.</p> </li> <li> <p> <code>blue-green-deployment-name</code> - Accepts user-supplied names for blue/green deployments. The results list only includes information about the blue/green deployments with the specified names.</p> </li> <li> <p> <code>source</code> - Accepts source databases for a blue/green deployment. The results list only includes information about the blue/green deployments with the specified source databases.</p> </li> <li> <p> <code>target</code> - Accepts target databases for a blue/green deployment. The results list only includes information about the blue/green deployments with the specified target databases.</p> </li> </ul>",
+                    "documentation": "<p>A filter that specifies one or more blue/green deployments to describe.</p> <p>Valid Values:</p> <ul> <li> <p> <code>blue-green-deployment-identifier</code> - Accepts system-generated identifiers for blue/green deployments. The results list only includes information about the blue/green deployments with the specified identifiers.</p> </li> <li> <p> <code>blue-green-deployment-name</code> - Accepts user-supplied names for blue/green deployments. The results list only includes information about the blue/green deployments with the specified names.</p> </li> <li> <p> <code>source</code> - Accepts source databases for a blue/green deployment. The results list only includes information about the blue/green deployments with the specified source databases.</p> </li> <li> <p> <code>target</code> - Accepts target databases for a blue/green deployment. The results list only includes information about the blue/green deployments with the specified target databases.</p> </li> </ul>",
                     "shape": "FilterList"
                 },
                 "Marker": {
-                    "documentation": "<p>An optional pagination token provided by a previous <code>DescribeBlueGreenDeployments</code> request. If this parameter is specified, the response includes only records beyond the marker, up to the value specified by <code>MaxRecords</code>.</p>",
+                    "documentation": "<p>An optional pagination token provided by a previous <code>DescribeBlueGreenDeployments</code> request. If you specify this parameter, the response only includes records beyond the marker, up to the value specified by <code>MaxRecords</code>.</p>",
                     "shape": "String"
                 },
                 "MaxRecords": {
-                    "documentation": "<p>The maximum number of records to include in the response. If more records exist than the specified <code>MaxRecords</code> value, a pagination token called a marker is included in the response so you can retrieve the remaining results.</p> <p>Default: 100</p> <p>Constraints: Minimum 20, maximum 100.</p>",
+                    "documentation": "<p>The maximum number of records to include in the response. If more records exist than the specified <code>MaxRecords</code> value, a pagination token called a marker is included in the response so you can retrieve the remaining results.</p> <p>Default: 100</p> <p>Constraints:</p> <ul> <li> <p>Must be a minimum of 20.</p> </li> <li> <p>Can't exceed 100.</p> </li> </ul>",
                     "shape": "MaxRecords"
                 }
             },
             "type": "structure"
         },
         "DescribeBlueGreenDeploymentsResponse": {
             "members": {
                 "BlueGreenDeployments": {
-                    "documentation": "<p>Contains a list of blue/green deployments for the user.</p>",
+                    "documentation": "<p>A list of blue/green deployments in the current account and Amazon Web Services Region.</p>",
                     "shape": "BlueGreenDeploymentList"
                 },
                 "Marker": {
-                    "documentation": "<p>A pagination token that can be used in a later DescribeBlueGreenDeployments request.</p>",
+                    "documentation": "<p>A pagination token that can be used in a later <code>DescribeBlueGreenDeployments</code> request.</p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "DescribeCertificatesMessage": {
             "documentation": "<p/>",
@@ -15918,19 +15926,19 @@
                 "shape": "Timezone"
             },
             "type": "list"
         },
         "SwitchoverBlueGreenDeploymentRequest": {
             "members": {
                 "BlueGreenDeploymentIdentifier": {
-                    "documentation": "<p>The blue/green deployment identifier.</p> <p>Constraints:</p> <ul> <li> <p>Must match an existing blue/green deployment identifier.</p> </li> </ul>",
+                    "documentation": "<p>The unique identifier of the blue/green deployment.</p> <p>Constraints:</p> <ul> <li> <p>Must match an existing blue/green deployment identifier.</p> </li> </ul>",
                     "shape": "BlueGreenDeploymentIdentifier"
                 },
                 "SwitchoverTimeout": {
-                    "documentation": "<p>The amount of time, in seconds, for the switchover to complete. The default is 300.</p> <p>If the switchover takes longer than the specified duration, then any changes are rolled back, and no changes are made to the environments.</p>",
+                    "documentation": "<p>The amount of time, in seconds, for the switchover to complete.</p> <p>Default: 300</p> <p>If the switchover takes longer than the specified duration, then any changes are rolled back, and no changes are made to the environments.</p>",
                     "shape": "SwitchoverTimeout"
                 }
             },
             "required": [
                 "BlueGreenDeploymentIdentifier"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/service-2.sdk-extras.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/service-2.sdk-extras.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore/data/rds/2014-10-31/waiters-2.json` & `botocore-a-la-carte-rds-1.31.9/botocore/data/rds/2014-10-31/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/PKG-INFO` & `botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-rds
-Version: 1.31.8
+Version: 1.31.9
 Summary: rds data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-rds-1.31.8/botocore_a_la_carte_rds.egg-info/SOURCES.txt` & `botocore-a-la-carte-rds-1.31.9/botocore_a_la_carte_rds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-rds-1.31.8/setup.py` & `botocore-a-la-carte-rds-1.31.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-rds',
-    version="1.31.8",
+    version="1.31.9",
     description='rds data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/rds/*/*.json'],
```

