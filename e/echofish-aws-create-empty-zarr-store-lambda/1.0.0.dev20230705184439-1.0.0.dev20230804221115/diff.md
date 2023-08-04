# Comparing `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439.tar.gz` & `tmp/echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439.tar", last modified: Wed Jul  5 18:45:35 2023, max compression
+gzip compressed data, was "echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115.tar", last modified: Fri Aug  4 22:12:01 2023, max compression
```

## Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439.tar` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2534 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2161 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      733 2023-07-05 18:45:32.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.720362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.720362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12014 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)      432 2023-07-05 18:44:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-05 18:45:35.724362 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2534 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      573 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       44 2023-07-05 18:45:35.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2868 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-04 22:11:59.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.948032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)    15401 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)     1230 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py
+-rw-r--r--   0 root         (0) root         (0)      297 2023-08-04 22:11:10.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda/sns_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 22:12:01.952032 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3241 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      773 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       91 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-08-04 22:12:01.000000 echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/LICENSE` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230705184439
+Version: 1.0.0.dev20230804221115
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,7 +60,22 @@
 ## Maven
 This project can use Apache Maven to easily build this project.  However, this is not required, but recommended.
 Maven can be easily installed by downloading it from the Maven site or using sdkman.
 
 ## Build with Maven
 After setting up your pyenv run:
 ```mvn clean install```
+
+## DOTENV
+export AWS_DEFAULT_PROFILE=echofish
+
+## Functional Testing
+To run a functional test, developer will need to save the associated environment variables in .env for the lambda to
+use. The ACCESS_KEY and SECRET_ACCESS_KEY can be generated in IAM, users, rudy-dev, security credentials,
+access keys, create access key. Copy other values as needed from deployed CloudFormation Template.
+```shell
+export OUTPUT_BUCKET=rudy-dev-echofish-118234403147-echofish-dev-output
+export TABLE_NAME=rudy-dev-echofish-EchoFish-File-Info
+export OUTPUT_BUCKET_ACCESS_KEY="XXX"
+export OUTPUT_BUCKET_SECRET_ACCESS_KEY="YYY"
+export TOPIC_ARN="arn:aws:sns:us-west-2:118234403147:rudy-dev-echofish-processing-finished"
+```
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/README.md` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -50,7 +50,22 @@
 ## Maven
 This project can use Apache Maven to easily build this project.  However, this is not required, but recommended.
 Maven can be easily installed by downloading it from the Maven site or using sdkman.
 
 ## Build with Maven
 After setting up your pyenv run:
 ```mvn clean install```
+
+## DOTENV
+export AWS_DEFAULT_PROFILE=echofish
+
+## Functional Testing
+To run a functional test, developer will need to save the associated environment variables in .env for the lambda to
+use. The ACCESS_KEY and SECRET_ACCESS_KEY can be generated in IAM, users, rudy-dev, security credentials,
+access keys, create access key. Copy other values as needed from deployed CloudFormation Template.
+```shell
+export OUTPUT_BUCKET=rudy-dev-echofish-118234403147-echofish-dev-output
+export TABLE_NAME=rudy-dev-echofish-EchoFish-File-Info
+export OUTPUT_BUCKET_ACCESS_KEY="XXX"
+export OUTPUT_BUCKET_SECRET_ACCESS_KEY="YYY"
+export TOPIC_ARN="arn:aws:sns:us-west-2:118234403147:rudy-dev-echofish-processing-finished"
+```
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/setup.py` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-create-empty-zarr-store-lambda",
-  version="1.0.0.dev20230705184439",
+  version="1.0.0.dev20230804221115",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
     "Programming Language :: Python :: 3.9",
     "License :: OSI Approved :: MIT License",
   ],
   python_requires='>=3.9',
   install_requires=[req for req in requirements if req[:2] != "# "]
-)
+)
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-create-empty-zarr-store-lambda
-Version: 1.0.0.dev20230705184439
+Version: 1.0.0.dev20230804221115
 Home-page: https://github.com/ci-cmg/echofish-aws-create-empty-zarr-store-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -60,7 +60,22 @@
 ## Maven
 This project can use Apache Maven to easily build this project.  However, this is not required, but recommended.
 Maven can be easily installed by downloading it from the Maven site or using sdkman.
 
 ## Build with Maven
 After setting up your pyenv run:
 ```mvn clean install```
+
+## DOTENV
+export AWS_DEFAULT_PROFILE=echofish
+
+## Functional Testing
+To run a functional test, developer will need to save the associated environment variables in .env for the lambda to
+use. The ACCESS_KEY and SECRET_ACCESS_KEY can be generated in IAM, users, rudy-dev, security credentials,
+access keys, create access key. Copy other values as needed from deployed CloudFormation Template.
+```shell
+export OUTPUT_BUCKET=rudy-dev-echofish-118234403147-echofish-dev-output
+export TABLE_NAME=rudy-dev-echofish-EchoFish-File-Info
+export OUTPUT_BUCKET_ACCESS_KEY="XXX"
+export OUTPUT_BUCKET_SECRET_ACCESS_KEY="YYY"
+export TOPIC_ARN="arn:aws:sns:us-west-2:118234403147:rudy-dev-echofish-processing-finished"
+```
```

### Comparing `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230705184439/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt` & `echofish-aws-create-empty-zarr-store-lambda-1.0.0.dev20230804221115/src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 LICENSE
 README.md
 setup.py
 src/echofish_aws_create_empty_zarr_store_lambda/__init__.py
+src/echofish_aws_create_empty_zarr_store_lambda/dynamo_operations.py
 src/echofish_aws_create_empty_zarr_store_lambda/lambda_executor.py
 src/echofish_aws_create_empty_zarr_store_lambda/lambda_handler.py
+src/echofish_aws_create_empty_zarr_store_lambda/s3_operations.py
+src/echofish_aws_create_empty_zarr_store_lambda/sns_operations.py
 src/echofish_aws_create_empty_zarr_store_lambda.egg-info/PKG-INFO
 src/echofish_aws_create_empty_zarr_store_lambda.egg-info/SOURCES.txt
 src/echofish_aws_create_empty_zarr_store_lambda.egg-info/dependency_links.txt
 src/echofish_aws_create_empty_zarr_store_lambda.egg-info/requires.txt
 src/echofish_aws_create_empty_zarr_store_lambda.egg-info/top_level.txt
```

