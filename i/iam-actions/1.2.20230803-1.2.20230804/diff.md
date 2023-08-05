# Comparing `tmp/iam_actions-1.2.20230803.tar.gz` & `tmp/iam_actions-1.2.20230804.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230803.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230804.tar", max compression
```

## Comparing `iam_actions-1.2.20230803.tar` & `iam_actions-1.2.20230804.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/LICENSE
--rw-r--r--   0        0        0     2302 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/README.md
--rw-r--r--   0        0        0      228 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/__init__.py
--rw-r--r--   0        0        0  4387612 2023-08-03 02:23:51.836879 iam_actions-1.2.20230803/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-08-03 02:21:56.527093 iam_actions-1.2.20230803/iam_actions/generate/services.py
--rw-r--r--   0        0        0   565944 2023-08-03 02:23:51.836879 iam_actions-1.2.20230803/iam_actions/policies.json
--rw-r--r--   0        0        0   196374 2023-08-03 02:23:51.836879 iam_actions-1.2.20230803/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   548980 2023-08-03 02:23:51.836879 iam_actions-1.2.20230803/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-08-03 02:23:52.656891 iam_actions-1.2.20230803/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230803/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230803/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/LICENSE
+-rw-r--r--   0        0        0     2302 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/README.md
+-rw-r--r--   0        0        0      228 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4389954 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-08-04 02:23:00.878126 iam_actions-1.2.20230804/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   566190 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/policies.json
+-rw-r--r--   0        0        0   196525 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   549219 2023-08-04 02:24:39.268079 iam_actions-1.2.20230804/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-08-04 02:24:40.140096 iam_actions-1.2.20230804/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230804/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230804/PKG-INFO
```

### Comparing `iam_actions-1.2.20230803/LICENSE` & `iam_actions-1.2.20230804/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/README.md` & `iam_actions-1.2.20230804/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/actions.json` & `iam_actions-1.2.20230804/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998188151397268%*

 * *Differences: {"'connect'": "{'SearchResourceTags': {'description': 'Grants permission to search tags that are "*

 * *              "used in an Amazon Connect instance'}}",*

 * * "'datasync'": "{'DescribeLocationAzureBlob': OrderedDict([('access_level', 'Undocumented'), "*

 * *               "('action', 'DescribeLocationAzureBlob'), ('condition_keys', []), ('description', "*

 * *               "'Not Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *               "'CreateLocationAzureBlob': OrderedDict([('access_level', 'Undocu […]*

```diff
@@ -32215,15 +32215,15 @@
         "SearchResourceTags": {
             "access_level": "List",
             "action": "SearchResourceTags",
             "condition_keys": [
                 "aws:ResourceTag/${TagKey}",
                 "connect:InstanceId"
             ],
-            "description": "Grants permission to search tags used in an Amazon Connect instance",
+            "description": "Grants permission to search tags that are used in an Amazon Connect instance",
             "orphan": false,
             "resources": [
                 "instance"
             ]
         },
         "SearchRoutingProfiles": {
             "access_level": "Read",
@@ -34798,14 +34798,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to activate an agent that you have deployed on your host",
             "orphan": false,
             "resources": []
         },
+        "CreateLocationAzureBlob": {
+            "access_level": "Undocumented",
+            "action": "CreateLocationAzureBlob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateLocationEfs": {
             "access_level": "Write",
             "action": "CreateLocationEfs",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -34972,14 +34980,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe metadata about a discovery job",
             "orphan": false,
             "resources": [
                 "discoveryjob"
             ]
         },
+        "DescribeLocationAzureBlob": {
+            "access_level": "Undocumented",
+            "action": "DescribeLocationAzureBlob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeLocationEfs": {
             "access_level": "Read",
             "action": "DescribeLocationEfs",
             "condition_keys": [],
             "description": "Grants permission to view metadata, such as the path information about an Amazon EFS sync location",
             "orphan": false,
             "resources": [
@@ -35298,14 +35314,22 @@
             "condition_keys": [],
             "description": "Grants permission to update a discovery job",
             "orphan": false,
             "resources": [
                 "discoveryjob"
             ]
         },
+        "UpdateLocationAzureBlob": {
+            "access_level": "Undocumented",
+            "action": "UpdateLocationAzureBlob",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "UpdateLocationHdfs": {
             "access_level": "Write",
             "action": "UpdateLocationHdfs",
             "condition_keys": [],
             "description": "Grants permission to update an HDFS sync Location",
             "orphan": false,
             "resources": [
@@ -75493,18 +75517,18 @@
             "action": "BatchGetCodeSnippet",
             "condition_keys": [],
             "description": "Grants permission to retrieve code snippet information about one or more code vulnerability findings",
             "orphan": false,
             "resources": []
         },
         "BatchGetFindingDetails": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "BatchGetFindingDetails",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to let a customer get enhanced vulnerability intelligence details for findings",
             "orphan": false,
             "resources": []
         },
         "BatchGetFreeTrialInfo": {
             "access_level": "Read",
             "action": "BatchGetFreeTrialInfo",
             "condition_keys": [],
@@ -92823,14 +92847,15 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a model that is trained on a dataset",
             "orphan": false,
             "resources": [
                 "dataset",
+                "label-group",
                 "model"
             ]
         },
         "DeleteDataset": {
             "access_level": "Write",
             "action": "DeleteDataset",
             "condition_keys": [],
@@ -92877,20 +92902,24 @@
             "description": "Grants permission to delete a model",
             "orphan": false,
             "resources": [
                 "model"
             ]
         },
         "DeleteResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete a resource policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset",
+                "model",
+                "model-version"
+            ]
         },
         "DescribeDataIngestionJob": {
             "access_level": "Read",
             "action": "DescribeDataIngestionJob",
             "condition_keys": [],
             "description": "Grants permission to describe a data ingestion job",
             "orphan": false,
@@ -92933,54 +92962,72 @@
             "description": "Grants permission to describe a model",
             "orphan": false,
             "resources": [
                 "model"
             ]
         },
         "DescribeModelVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeModelVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a model version",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "model-version"
+            ]
         },
         "DescribeResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "DescribeResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to describe a resource policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset",
+                "model",
+                "model-version"
+            ]
         },
         "Describelabel": {
             "access_level": "Read",
             "action": "Describelabel",
             "condition_keys": [],
             "description": "Grants permission to describe a label",
             "orphan": false,
             "resources": [
                 "label-group"
             ]
         },
         "ImportDataset": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportDataset",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to import a dataset",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset"
+            ]
         },
         "ImportModelVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "ImportModelVersion",
-            "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "condition_keys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:TagKeys"
+            ],
+            "description": "Grants permission to import a model version",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset",
+                "label-group",
+                "model"
+            ]
         },
         "ListDataIngestionJobs": {
             "access_level": "List",
             "action": "ListDataIngestionJobs",
             "condition_keys": [],
             "description": "Grants permission to list the data ingestion jobs in your account or for a particular dataset",
             "orphan": false,
@@ -93041,20 +93088,22 @@
             "description": "Grants permission to list the labels in your account",
             "orphan": false,
             "resources": [
                 "label-group"
             ]
         },
         "ListModelVersions": {
-            "access_level": "Undocumented",
+            "access_level": "List",
             "action": "ListModelVersions",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to list the model versions in your account",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "model"
+            ]
         },
         "ListModels": {
             "access_level": "List",
             "action": "ListModels",
             "condition_keys": [],
             "description": "Grants permission to list the models in your account",
             "orphan": false,
@@ -93076,24 +93125,29 @@
             "condition_keys": [],
             "description": "Grants permission to list the tags for a resource",
             "orphan": false,
             "resources": [
                 "dataset",
                 "inference-scheduler",
                 "label-group",
-                "model"
+                "model",
+                "model-version"
             ]
         },
         "PutResourcePolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutResourcePolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to put a resource policy",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "dataset",
+                "model",
+                "model-version"
+            ]
         },
         "StartDataIngestionJob": {
             "access_level": "Write",
             "action": "StartDataIngestionJob",
             "condition_keys": [],
             "description": "Grants permission to start a data ingestion job for a dataset",
             "orphan": false,
@@ -93130,39 +93184,44 @@
             ],
             "description": "Grants permission to tag a resource",
             "orphan": false,
             "resources": [
                 "dataset",
                 "inference-scheduler",
                 "label-group",
-                "model"
+                "model",
+                "model-version"
             ]
         },
         "UntagResource": {
             "access_level": "Tagging",
             "action": "UntagResource",
             "condition_keys": [
                 "aws:TagKeys"
             ],
             "description": "Grants permission to untag a resource",
             "orphan": false,
             "resources": [
                 "dataset",
                 "inference-scheduler",
                 "label-group",
-                "model"
+                "model",
+                "model-version"
             ]
         },
         "UpdateActiveModelVersion": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "UpdateActiveModelVersion",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to set the active model version for a given machine learning model",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "model",
+                "model-version"
+            ]
         },
         "UpdateInferenceScheduler": {
             "access_level": "Write",
             "action": "UpdateInferenceScheduler",
             "condition_keys": [],
             "description": "Grants permission to update an inference scheduler",
             "orphan": false,
@@ -93889,18 +93948,18 @@
             "description": "Grants permission to retrieve a runtime environment",
             "orphan": false,
             "resources": [
                 "Environment"
             ]
         },
         "GetSignedBluinsightsUrl": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetSignedBluinsightsUrl",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to create a signed Bluinsights url",
             "orphan": false,
             "resources": []
         },
         "ListApplicationVersions": {
             "access_level": "Read",
             "action": "ListApplicationVersions",
             "condition_keys": [],
@@ -114967,14 +115026,22 @@
             "description": "Grants permission to delete a previously provisioned DB cluster",
             "orphan": false,
             "resources": [
                 "cluster",
                 "cluster-snapshot"
             ]
         },
+        "DeleteDBClusterAutomatedBackup": {
+            "access_level": "Undocumented",
+            "action": "DeleteDBClusterAutomatedBackup",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteDBClusterEndpoint": {
             "access_level": "Write",
             "action": "DeleteDBClusterEndpoint",
             "condition_keys": [],
             "description": "Grants permission to delete a custom endpoint and removes it from an Amazon Aurora DB cluster",
             "orphan": false,
             "resources": [
@@ -115144,14 +115211,22 @@
             "access_level": "List",
             "action": "DescribeCertificates",
             "condition_keys": [],
             "description": "Grants permission to list the set of CA certificates provided by Amazon RDS for this AWS account",
             "orphan": false,
             "resources": []
         },
+        "DescribeDBClusterAutomatedBackups": {
+            "access_level": "Undocumented",
+            "action": "DescribeDBClusterAutomatedBackups",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DescribeDBClusterBacktracks": {
             "access_level": "List",
             "action": "DescribeDBClusterBacktracks",
             "condition_keys": [],
             "description": "Grants permission to return information about backtracks for a DB cluster",
             "orphan": false,
             "resources": [
@@ -119187,14 +119262,22 @@
             "condition_keys": [],
             "description": "Grants permission to add draft application version resource mappings",
             "orphan": false,
             "resources": [
                 "application"
             ]
         },
+        "BatchUpdateRecommendationStatus": {
+            "access_level": "Undocumented",
+            "action": "BatchUpdateRecommendationStatus",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "CreateApp": {
             "access_level": "Write",
             "action": "CreateApp",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -119422,14 +119505,22 @@
             "condition_keys": [],
             "description": "Grants permission to list alarm recommendation",
             "orphan": false,
             "resources": [
                 "application"
             ]
         },
+        "ListAppAssessmentComplianceDrifts": {
+            "access_level": "Undocumented",
+            "action": "ListAppAssessmentComplianceDrifts",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "ListAppAssessments": {
             "access_level": "List",
             "action": "ListAppAssessments",
             "condition_keys": [],
             "description": "Grants permission to list application assessment",
             "orphan": false,
             "resources": []
@@ -150882,15 +150973,14 @@
         "GetSampledRequests": {
             "access_level": "Read",
             "action": "GetSampledRequests",
             "condition_keys": [],
             "description": "Grants permission to retrieve detailed information about a sample set of web requests",
             "orphan": false,
             "resources": [
-                "rule",
                 "webacl"
             ]
         },
         "GetSizeConstraintSet": {
             "access_level": "Read",
             "action": "GetSizeConstraintSet",
             "condition_keys": [],
@@ -151668,15 +151758,14 @@
         "GetSampledRequests": {
             "access_level": "Read",
             "action": "GetSampledRequests",
             "condition_keys": [],
             "description": "Grants permission to retrieve detailed information for a sample set of web requests",
             "orphan": false,
             "resources": [
-                "rule",
                 "webacl"
             ]
         },
         "GetSizeConstraintSet": {
             "access_level": "Read",
             "action": "GetSizeConstraintSet",
             "condition_keys": [],
```

### Comparing `iam_actions-1.2.20230803/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230804/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230804/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/generate/generate.py` & `iam_actions-1.2.20230804/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230804/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230804/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/generate/services.py` & `iam_actions-1.2.20230804/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230803/iam_actions/policies.json` & `iam_actions-1.2.20230804/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9994798321048322%*

 * *Differences: {"'serviceMap'": "{'Amazon RDS': {'Actions': {insert: [(34, 'DeleteDBClusterAutomatedBackup'), "*

 * *                 "(53, 'DescribeDBClusterAutomatedBackups')]}}, 'AWS DataSync': {'Actions': "*

 * *                 "{insert: [(3, 'CreateLocationAzureBlob'), (20, 'DescribeLocationAzureBlob'), "*

 * *                 "(52, 'UpdateLocationAzureBlob')]}}, 'AWS Resilience Hub': "*

 * *                 "OrderedDict([('StringPrefix', 'resiliencehub'), ('Actions', "*

 * *                 "['AddDraftAppVersionResourceMappings', 'BatchUpd […]*

```diff
@@ -2624,14 +2624,15 @@
         "AWS DataSync": {
             "ARNFormat": "arn:aws:datasync:${Region}:${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:datasync:.+",
             "Actions": [
                 "AddStorageSystem",
                 "CancelTaskExecution",
                 "CreateAgent",
+                "CreateLocationAzureBlob",
                 "CreateLocationEfs",
                 "CreateLocationFsxLustre",
                 "CreateLocationFsxOntap",
                 "CreateLocationFsxOpenZfs",
                 "CreateLocationFsxWindows",
                 "CreateLocationHdfs",
                 "CreateLocationNfs",
@@ -2640,14 +2641,15 @@
                 "CreateLocationSmb",
                 "CreateTask",
                 "DeleteAgent",
                 "DeleteLocation",
                 "DeleteTask",
                 "DescribeAgent",
                 "DescribeDiscoveryJob",
+                "DescribeLocationAzureBlob",
                 "DescribeLocationEfs",
                 "DescribeLocationFsxLustre",
                 "DescribeLocationFsxOntap",
                 "DescribeLocationFsxOpenZfs",
                 "DescribeLocationFsxWindows",
                 "DescribeLocationHdfs",
                 "DescribeLocationNfs",
@@ -2671,14 +2673,15 @@
                 "StartDiscoveryJob",
                 "StartTaskExecution",
                 "StopDiscoveryJob",
                 "TagResource",
                 "UntagResource",
                 "UpdateAgent",
                 "UpdateDiscoveryJob",
+                "UpdateLocationAzureBlob",
                 "UpdateLocationHdfs",
                 "UpdateLocationNfs",
                 "UpdateLocationObjectStorage",
                 "UpdateLocationSmb",
                 "UpdateStorageSystem",
                 "UpdateTask",
                 "UpdateTaskExecution"
@@ -7786,19 +7789,20 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
                 "rbin:Attribute/ResourceType",
                 "rbin:Request/ResourceType"
             ]
         },
-        "AWS Resilience Hub Service": {
+        "AWS Resilience Hub": {
             "ARNFormat": "arn:aws:resiliencehub:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:resiliencehub:.+",
             "Actions": [
                 "AddDraftAppVersionResourceMappings",
+                "BatchUpdateRecommendationStatus",
                 "CreateApp",
                 "CreateAppVersionAppComponent",
                 "CreateAppVersionResource",
                 "CreateRecommendationTemplate",
                 "CreateResiliencyPolicy",
                 "DeleteApp",
                 "DeleteAppAssessment",
@@ -7814,14 +7818,15 @@
                 "DescribeAppVersionResource",
                 "DescribeAppVersionResourcesResolutionStatus",
                 "DescribeAppVersionTemplate",
                 "DescribeDraftAppVersionResourcesImportStatus",
                 "DescribeResiliencyPolicy",
                 "ImportResourcesToDraftAppVersion",
                 "ListAlarmRecommendations",
+                "ListAppAssessmentComplianceDrifts",
                 "ListAppAssessments",
                 "ListAppComponentCompliances",
                 "ListAppComponentRecommendations",
                 "ListAppInputSources",
                 "ListAppVersionAppComponents",
                 "ListAppVersionResourceMappings",
                 "ListAppVersionResources",
@@ -17451,14 +17456,15 @@
                 "CreateEventSubscription",
                 "CreateGlobalCluster",
                 "CreateOptionGroup",
                 "CrossRegionCommunication",
                 "DeleteBlueGreenDeployment",
                 "DeleteCustomDBEngineVersion",
                 "DeleteDBCluster",
+                "DeleteDBClusterAutomatedBackup",
                 "DeleteDBClusterEndpoint",
                 "DeleteDBClusterParameterGroup",
                 "DeleteDBClusterSnapshot",
                 "DeleteDBInstance",
                 "DeleteDBInstanceAutomatedBackup",
                 "DeleteDBParameterGroup",
                 "DeleteDBProxy",
@@ -17469,14 +17475,15 @@
                 "DeleteEventSubscription",
                 "DeleteGlobalCluster",
                 "DeleteOptionGroup",
                 "DeregisterDBProxyTargets",
                 "DescribeAccountAttributes",
                 "DescribeBlueGreenDeployments",
                 "DescribeCertificates",
+                "DescribeDBClusterAutomatedBackups",
                 "DescribeDBClusterBacktracks",
                 "DescribeDBClusterEndpoints",
                 "DescribeDBClusterParameterGroups",
                 "DescribeDBClusterParameters",
                 "DescribeDBClusterSnapshotAttributes",
                 "DescribeDBClusterSnapshots",
                 "DescribeDBClusters",
```

### Comparing `iam_actions-1.2.20230803/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230804/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9996423705722071%*

 * *Differences: {"'lookoutequipment'": "{'model-version': OrderedDict([('arn_pattern', "*

 * *                       "'arn:*:lookoutequipment:*:*:model/*/*/model-version/*'), "*

 * *                       "('condition_keys', 'aws:ResourceTag/${TagKey}')])}",*

 * * "'mq'": "{'brokers': {'arn_pattern': 'arn:*:mq:*:*:broker:*:*'}}"}*

```diff
@@ -3988,14 +3988,18 @@
         "label-group": {
             "arn_pattern": "arn:*:lookoutequipment:*:*:label-group/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "model": {
             "arn_pattern": "arn:*:lookoutequipment:*:*:model/*/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
+        },
+        "model-version": {
+            "arn_pattern": "arn:*:lookoutequipment:*:*:model/*/*/model-version/*",
+            "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "lookoutmetrics": {
         "Alert": {
             "arn_pattern": "arn:*:lookoutmetrics:*:*:Alert:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
@@ -4468,15 +4472,15 @@
         "project": {
             "arn_pattern": "arn:*:monitron:*:*:project/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "mq": {
         "brokers": {
-            "arn_pattern": "arn:*:mq:*:*:broker:*",
+            "arn_pattern": "arn:*:mq:*:*:broker:*:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "configurations": {
             "arn_pattern": "arn:*:mq:*:*:configuration:*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
```

### Comparing `iam_actions-1.2.20230803/iam_actions/services.json` & `iam_actions-1.2.20230804/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998750510274124%*

 * *Differences: {"'datasync'": "{'Actions': {insert: [(3, 'CreateLocationAzureBlob'), (20, "*

 * *               "'DescribeLocationAzureBlob'), (52, 'UpdateLocationAzureBlob')]}}",*

 * * "'rds'": "{'Actions': {insert: [(34, 'DeleteDBClusterAutomatedBackup'), (53, "*

 * *          "'DescribeDBClusterAutomatedBackups')]}}",*

 * * "'resiliencehub'": "{'Actions': {insert: [(1, 'BatchUpdateRecommendationStatus'), (25, "*

 * *                    "'ListAppAssessmentComplianceDrifts')]}, 'ServiceNames': ['AWS Resilience "*

 * *                    "Hub']}"}*

```diff
@@ -5223,14 +5223,15 @@
         "ARNRegexes": [
             "^arn:aws:datasync:.+"
         ],
         "Actions": [
             "AddStorageSystem",
             "CancelTaskExecution",
             "CreateAgent",
+            "CreateLocationAzureBlob",
             "CreateLocationEfs",
             "CreateLocationFsxLustre",
             "CreateLocationFsxOntap",
             "CreateLocationFsxOpenZfs",
             "CreateLocationFsxWindows",
             "CreateLocationHdfs",
             "CreateLocationNfs",
@@ -5239,14 +5240,15 @@
             "CreateLocationSmb",
             "CreateTask",
             "DeleteAgent",
             "DeleteLocation",
             "DeleteTask",
             "DescribeAgent",
             "DescribeDiscoveryJob",
+            "DescribeLocationAzureBlob",
             "DescribeLocationEfs",
             "DescribeLocationFsxLustre",
             "DescribeLocationFsxOntap",
             "DescribeLocationFsxOpenZfs",
             "DescribeLocationFsxWindows",
             "DescribeLocationHdfs",
             "DescribeLocationNfs",
@@ -5270,14 +5272,15 @@
             "StartDiscoveryJob",
             "StartTaskExecution",
             "StopDiscoveryJob",
             "TagResource",
             "UntagResource",
             "UpdateAgent",
             "UpdateDiscoveryJob",
+            "UpdateLocationAzureBlob",
             "UpdateLocationHdfs",
             "UpdateLocationNfs",
             "UpdateLocationObjectStorage",
             "UpdateLocationSmb",
             "UpdateStorageSystem",
             "UpdateTask",
             "UpdateTaskExecution"
@@ -16178,14 +16181,15 @@
             "CreateEventSubscription",
             "CreateGlobalCluster",
             "CreateOptionGroup",
             "CrossRegionCommunication",
             "DeleteBlueGreenDeployment",
             "DeleteCustomDBEngineVersion",
             "DeleteDBCluster",
+            "DeleteDBClusterAutomatedBackup",
             "DeleteDBClusterEndpoint",
             "DeleteDBClusterParameterGroup",
             "DeleteDBClusterSnapshot",
             "DeleteDBInstance",
             "DeleteDBInstanceAutomatedBackup",
             "DeleteDBParameterGroup",
             "DeleteDBProxy",
@@ -16196,14 +16200,15 @@
             "DeleteEventSubscription",
             "DeleteGlobalCluster",
             "DeleteOptionGroup",
             "DeregisterDBProxyTargets",
             "DescribeAccountAttributes",
             "DescribeBlueGreenDeployments",
             "DescribeCertificates",
+            "DescribeDBClusterAutomatedBackups",
             "DescribeDBClusterBacktracks",
             "DescribeDBClusterEndpoints",
             "DescribeDBClusterParameterGroups",
             "DescribeDBClusterParameters",
             "DescribeDBClusterSnapshotAttributes",
             "DescribeDBClusterSnapshots",
             "DescribeDBClusters",
@@ -16772,14 +16777,15 @@
             "arn:aws:resiliencehub:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:resiliencehub:.+"
         ],
         "Actions": [
             "AddDraftAppVersionResourceMappings",
+            "BatchUpdateRecommendationStatus",
             "CreateApp",
             "CreateAppVersionAppComponent",
             "CreateAppVersionResource",
             "CreateRecommendationTemplate",
             "CreateResiliencyPolicy",
             "DeleteApp",
             "DeleteAppAssessment",
@@ -16795,14 +16801,15 @@
             "DescribeAppVersionResource",
             "DescribeAppVersionResourcesResolutionStatus",
             "DescribeAppVersionTemplate",
             "DescribeDraftAppVersionResourcesImportStatus",
             "DescribeResiliencyPolicy",
             "ImportResourcesToDraftAppVersion",
             "ListAlarmRecommendations",
+            "ListAppAssessmentComplianceDrifts",
             "ListAppAssessments",
             "ListAppComponentCompliances",
             "ListAppComponentRecommendations",
             "ListAppInputSources",
             "ListAppVersionAppComponents",
             "ListAppVersionResourceMappings",
             "ListAppVersionResources",
@@ -16831,15 +16838,15 @@
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys"
         ],
         "HasResource": true,
         "ServiceNames": [
-            "AWS Resilience Hub Service"
+            "AWS Resilience Hub"
         ]
     },
     "resource-explorer": {
         "ARNFormats": [
             "arn:${Partition}:resource-explorer:${Region}:${Account}:${ResourceType}/${ResourceName}"
         ],
         "ARNRegexes": [
```

### Comparing `iam_actions-1.2.20230803/pyproject.toml` & `iam_actions-1.2.20230804/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230803"
+version = "1.2.20230804"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230803/setup.py` & `iam_actions-1.2.20230804/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230803',
+    'version': '1.2.20230804',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230803/PKG-INFO` & `iam_actions-1.2.20230804/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230803
+Version: 1.2.20230804
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

