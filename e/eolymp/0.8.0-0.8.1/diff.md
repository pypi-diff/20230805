# Comparing `tmp/eolymp-0.8.0.tar.gz` & `tmp/eolymp-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eolymp-0.8.0.tar", last modified: Wed Jul 26 14:24:56 2023, max compression
+gzip compressed data, was "eolymp-0.8.1.tar", last modified: Sat Aug  5 15:23:54 2023, max compression
```

## Comparing `eolymp-0.8.0.tar` & `eolymp-0.8.1.tar`

### file list

```diff
@@ -1,387 +1,396 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.603084 eolymp-0.8.0/
--rw-r--r--   0 root         (0) root         (0)      911 2023-07-26 14:24:56.603084 eolymp-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      512 2023-07-26 14:24:55.000000 eolymp-0.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.515082 eolymp-0.8.0/eolymp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.515082 eolymp-0.8.0/eolymp/acl/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/acl/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/acl/acl_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6121 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/acl/acl_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4305 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/acl/acl_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.519082 eolymp-0.8.0/eolymp/annotations/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/annotations/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/endpoint_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1042 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/endpoint_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2308 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/http_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/http_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1536 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/ratelimit_pb2.py
--rw-r--r--   0 root         (0) root         (0)      623 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/ratelimit_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1462 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/scope_pb2.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/annotations/scope_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.519082 eolymp-0.8.0/eolymp/apollo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/apollo/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1364 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/apollo/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/apollo/events_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.519082 eolymp-0.8.0/eolymp/asset/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/asset/__init__.py
--rw-r--r--   0 root         (0) root         (0)      809 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/asset/asset_http.py
--rw-r--r--   0 root         (0) root         (0)     2995 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/asset/asset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2354 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/asset/asset_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.539083 eolymp-0.8.0/eolymp/atlas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/atlas/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2072 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/asset_service_http.py
--rw-r--r--   0 root         (0) root         (0)     5722 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/asset_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3872 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/asset_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    25164 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/atlas_http.py
--rw-r--r--   0 root         (0) root         (0)    30169 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/atlas_pb2.py
--rw-r--r--   0 root         (0) root         (0)      957 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/atlas_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1239 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/attachment_pb2.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/attachment_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2564 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/attachment_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7093 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/attachment_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4619 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/attachment_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1132 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/bookmark_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2831 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/bookmark_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1124 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/bookmark_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1218 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_file_pb2.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_file_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1640 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1625 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2896 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7639 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/code_template_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1413 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/editorial_pb2.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/editorial_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3205 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/editorial_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8288 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/editorial_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4418 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/editorial_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1859 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2046 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/library_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8197 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/library_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7646 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/library_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2772 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2416 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/problem_service_http.py
--rw-r--r--   0 root         (0) root         (0)     5937 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/problem_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/problem_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1445 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/scoring_score_pb2.py
--rw-r--r--   0 root         (0) root         (0)      953 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/scoring_score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1595 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/scoring_service_http.py
--rw-r--r--   0 root         (0) root         (0)     4331 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/scoring_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2529 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/scoring_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1955 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/solution_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1871 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/solution_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1764 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/statement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/statement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3195 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/statement_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8504 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/statement_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5202 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/statement_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4906 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7543 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2105 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/submission_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6050 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/submission_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5292 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/submission_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1155 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_config_pb2.py
--rw-r--r--   0 root         (0) root         (0)      407 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_config_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1244 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_feedback_pb2.py
--rw-r--r--   0 root         (0) root         (0)      381 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_feedback_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1270 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_scoring_pb2.py
--rw-r--r--   0 root         (0) root         (0)      396 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_scoring_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     7275 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_service_http.py
--rw-r--r--   0 root         (0) root         (0)    18070 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11063 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1372 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_test_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1029 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_test_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_testset_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1867 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/testing_testset_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1443 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/version_pb2.py
--rw-r--r--   0 root         (0) root         (0)      995 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/atlas/version_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.539083 eolymp-0.8.0/eolymp/auth/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/auth/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1650 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/claims_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1830 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/claims_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      493 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/oauth2_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6035 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/oauth2_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5486 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/oauth2_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)      490 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/sso_service_http.py
--rw-r--r--   0 root         (0) root         (0)     2894 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/sso_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1917 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/auth/sso_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.543083 eolymp-0.8.0/eolymp/cognito/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/cognito/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1483 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/access_key_pb2.py
--rw-r--r--   0 root         (0) root         (0)      997 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/access_key_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8446 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/cognito_http.py
--rw-r--r--   0 root         (0) root         (0)    26443 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/cognito_pb2.py
--rw-r--r--   0 root         (0) root         (0)    21628 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/cognito_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1321 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/entitlement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      451 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/entitlement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1170 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/quota_pb2.py
--rw-r--r--   0 root         (0) root         (0)      482 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/quota_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2297 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2923 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/cognito/user_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.551083 eolymp-0.8.0/eolymp/community/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/community/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3544 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/account_service_http.py
--rw-r--r--   0 root         (0) root         (0)    10020 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/account_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6384 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/account_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2632 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/attribute_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/attribute_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2568 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/attribute_service_http.py
--rw-r--r--   0 root         (0) root         (0)     7395 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/attribute_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4643 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/attribute_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1627 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/configuration_idp_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1447 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/configuration_idp_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1188 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/configuration_service_http.py
--rw-r--r--   0 root         (0) root         (0)     4128 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/configuration_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/configuration_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1696 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1025 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1158 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_ghost_pb2.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_ghost_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2173 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4017 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_service_http.py
--rw-r--r--   0 root         (0) root         (0)    11637 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8991 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1327 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_team_pb2.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_team_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2211 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_user_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2474 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/member_user_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1187 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/membership_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3943 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/membership_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1616 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/community/membership_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.551083 eolymp-0.8.0/eolymp/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1489 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/core/http_client.py
--rw-r--r--   0 root         (0) root         (0)     2288 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/core/oauth_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.559083 eolymp-0.8.0/eolymp/discussion/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/discussion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2180 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/discussion_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2032 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/discussion_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3064 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/discussion_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8074 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/discussion_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4433 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/discussion_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1438 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1784 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/forum_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1387 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/forum_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2478 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/forum_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6622 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/forum_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3860 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/forum_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1825 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/message_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1646 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/message_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2979 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/message_service_http.py
--rw-r--r--   0 root         (0) root         (0)     8680 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/message_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6502 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/message_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1442 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/subscription_pb2.py
--rw-r--r--   0 root         (0) root         (0)      734 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/subscription_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1185 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/subscription_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3644 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/subscription_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1289 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/discussion/subscription_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.559083 eolymp-0.8.0/eolymp/ecm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/ecm/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ecm/content_pb2.py
--rw-r--r--   0 root         (0) root         (0)      784 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ecm/content_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1487 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ecm/node_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ecm/node_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.567083 eolymp-0.8.0/eolymp/executor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/executor/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1617 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      834 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2558 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/executor_http.py
--rw-r--r--   0 root         (0) root         (0)     8384 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/executor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     5724 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/executor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1705 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/interactor_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1572 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/interactor_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6109 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11298 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1225 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/language_pb2.py
--rw-r--r--   0 root         (0) root         (0)      565 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/language_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     5233 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/report_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7802 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/report_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1290 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/runtime_pb2.py
--rw-r--r--   0 root         (0) root         (0)      752 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/runtime_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2965 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/status_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4284 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/status_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3640 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/task_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6288 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/task_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1565 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/usage_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1635 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/usage_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1950 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/verifier_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2026 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/executor/verifier_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.567083 eolymp-0.8.0/eolymp/geography/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/geography/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1223 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/country_pb2.py
--rw-r--r--   0 root         (0) root         (0)      549 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/country_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2233 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/geography_http.py
--rw-r--r--   0 root         (0) root         (0)     4943 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/geography_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2558 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/geography_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/region_pb2.py
--rw-r--r--   0 root         (0) root         (0)      660 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/geography/region_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.571083 eolymp-0.8.0/eolymp/harmony/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/harmony/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1265 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/agreement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/agreement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1727 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/consent_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1332 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/consent_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2234 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/harmony_http.py
--rw-r--r--   0 root         (0) root         (0)     4871 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/harmony_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2717 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/harmony/harmony_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.571083 eolymp-0.8.0/eolymp/helpdesk/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/helpdesk/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1422 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/auto_reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1035 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/auto_reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1458 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/document_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1126 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/document_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2439 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2041 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3573 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/helpdesk_http.py
--rw-r--r--   0 root         (0) root         (0)    10284 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/helpdesk_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7297 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/helpdesk_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8600 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/support_http.py
--rw-r--r--   0 root         (0) root         (0)    19983 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/support_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13222 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/support_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3595 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4215 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/helpdesk/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.583084 eolymp-0.8.0/eolymp/judge/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/judge/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2179 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/acl_http.py
--rw-r--r--   0 root         (0) root         (0)     5512 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/acl_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3991 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/acl_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2389 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2641 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1498 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/announcement_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1044 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/announcement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3524 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/contest_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4623 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/contest_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1777 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/entitlement_pb2.py
--rw-r--r--   0 root         (0) root         (0)      816 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/entitlement_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3285 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3207 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)    38096 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/judge_http.py
--rw-r--r--   0 root         (0) root         (0)    79306 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/judge_pb2.py
--rw-r--r--   0 root         (0) root         (0)    55068 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/judge_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2522 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/participant_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3192 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/participant_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3088 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/problem_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4266 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/problem_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1519 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/reply_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1141 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/reply_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1491 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/result_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1178 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/result_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2586 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/score_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3589 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/score_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4771 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/submission_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7066 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/submission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1557 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/template_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1421 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/template_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1768 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/ticket_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1841 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/judge/ticket_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.583084 eolymp-0.8.0/eolymp/keeper/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/keeper/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1257 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/keeper/blob_pb2.py
--rw-r--r--   0 root         (0) root         (0)      726 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/keeper/blob_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2965 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/keeper/keeper_http.py
--rw-r--r--   0 root         (0) root         (0)     7328 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/keeper/keeper_pb2.py
--rw-r--r--   0 root         (0) root         (0)     4406 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/keeper/keeper_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.587084 eolymp-0.8.0/eolymp/l10n/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/l10n/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9434 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/localization_service_http.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/localization_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15558 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/localization_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1252 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/project_pb2.py
--rw-r--r--   0 root         (0) root         (0)      753 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/project_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1267 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/project_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3835 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/project_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2221 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/project_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1460 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/term_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1055 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/term_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1851 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/translation_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1657 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/l10n/translation_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.587084 eolymp-0.8.0/eolymp/oauth2/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/oauth2/__init__.py
--rw-r--r--   0 root         (0) root         (0)      486 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/oauth2/oauth2_http.py
--rw-r--r--   0 root         (0) root         (0)     7848 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/oauth2/oauth2_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8829 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/oauth2/oauth2_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.587084 eolymp-0.8.0/eolymp/playground/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/playground/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1689 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/playground/playground_http.py
--rw-r--r--   0 root         (0) root         (0)     4248 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/playground/playground_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1982 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/playground/playground_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2162 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/playground/run_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2275 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/playground/run_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.591084 eolymp-0.8.0/eolymp/ranker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/ranker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2245 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/activity_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2299 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/activity_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1258 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1165 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/format_pb2.py
--rw-r--r--   0 root         (0) root         (0)      335 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/format_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     8724 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/ranker_http.py
--rw-r--r--   0 root         (0) root         (0)    21385 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/ranker_pb2.py
--rw-r--r--   0 root         (0) root         (0)    15143 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/ranker_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4876 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/scoreboard_pb2.py
--rw-r--r--   0 root         (0) root         (0)     8126 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/ranker/scoreboard_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.591084 eolymp-0.8.0/eolymp/resolver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/resolver/__init__.py
--rw-r--r--   0 root         (0) root         (0)      923 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/resolver/resolver_http.py
--rw-r--r--   0 root         (0) root         (0)     3800 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/resolver/resolver_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3246 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/resolver/resolver_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.595084 eolymp-0.8.0/eolymp/taxonomy/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/taxonomy/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1145 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/link_service_http.py
--rw-r--r--   0 root         (0) root         (0)     3120 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/link_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1167 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/link_service_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1496 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/topic_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1377 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/topic_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4010 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/topic_service_http.py
--rw-r--r--   0 root         (0) root         (0)    10053 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/topic_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6654 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/taxonomy/topic_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.599084 eolymp-0.8.0/eolymp/typewriter/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/typewriter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7630 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/block_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11265 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/block_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1443 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      704 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     1456 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/fragment_pb2.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/fragment_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2640 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/inline_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2997 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/inline_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     3884 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/typewriter_http.py
--rw-r--r--   0 root         (0) root         (0)    11054 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/typewriter_pb2.py
--rw-r--r--   0 root         (0) root         (0)     7632 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/typewriter/typewriter_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.599084 eolymp-0.8.0/eolymp/universe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/universe/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1501 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/permission_pb2.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/permission_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2788 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/space_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3731 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/space_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     6381 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/universe_http.py
--rw-r--r--   0 root         (0) root         (0)    14223 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/universe_pb2.py
--rw-r--r--   0 root         (0) root         (0)     9486 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/universe/universe_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.603084 eolymp-0.8.0/eolymp/wellknown/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/wellknown/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1190 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/wellknown/direction_pb2.py
--rw-r--r--   0 root         (0) root         (0)      331 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/wellknown/direction_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2426 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/wellknown/errors_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2458 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/wellknown/errors_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     4481 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/wellknown/expression_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3915 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/wellknown/expression_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.603084 eolymp-0.8.0/eolymp/worker/
--rw-r--r--   0 root         (0) root         (0)        0 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp/worker/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1274 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/events_pb2.py
--rw-r--r--   0 root         (0) root         (0)      505 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/events_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2649 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/job_pb2.py
--rw-r--r--   0 root         (0) root         (0)     2880 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/job_pb2.pyi
--rw-r--r--   0 root         (0) root         (0)     2751 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/worker_service_http.py
--rw-r--r--   0 root         (0) root         (0)     6564 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/worker_service_pb2.py
--rw-r--r--   0 root         (0) root         (0)     3389 2023-07-26 14:24:55.000000 eolymp-0.8.0/eolymp/worker/worker_service_pb2.pyi
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-26 14:24:56.515082 eolymp-0.8.0/eolymp.egg-info/
--rw-r--r--   0 root         (0) root         (0)      911 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11566 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-07-26 14:24:56.000000 eolymp-0.8.0/eolymp.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-26 14:24:56.603084 eolymp-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      974 2023-07-26 14:24:55.000000 eolymp-0.8.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.603536 eolymp-0.8.1/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-08-05 15:23:54.603536 eolymp-0.8.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      512 2023-08-05 15:23:53.000000 eolymp-0.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.531530 eolymp-0.8.1/eolymp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.535531 eolymp-0.8.1/eolymp/acl/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/acl/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/acl_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6121 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/acl_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4305 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/acl_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      842 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/entitlement_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2215 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/entitlement_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      798 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/acl/entitlement_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.535531 eolymp-0.8.1/eolymp/annotations/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/annotations/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/endpoint_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/endpoint_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2308 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/http_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/http_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      623 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/scope_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/annotations/scope_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.535531 eolymp-0.8.1/eolymp/apollo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/apollo/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1364 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/apollo/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/apollo/events_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.539531 eolymp-0.8.1/eolymp/asset/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/asset/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      809 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_http.py
+-rw-r--r--   0 root         (0) root         (0)     2995 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2354 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      816 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      355 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/asset/asset_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.551532 eolymp-0.8.1/eolymp/atlas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/atlas/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2072 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/asset_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     5722 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/asset_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3872 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/asset_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    25164 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/atlas_http.py
+-rw-r--r--   0 root         (0) root         (0)    30169 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/atlas_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      957 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/atlas_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2564 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7093 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4619 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1132 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/bookmark_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1218 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1640 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1625 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2896 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7639 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1413 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3205 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8288 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4418 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2046 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/library_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8197 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/library_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7646 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/library_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2772 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1592 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     5937 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/problem_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1445 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      953 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1595 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     4331 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2529 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/solution_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1871 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/solution_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1764 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3195 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8504 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5202 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/statement_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4906 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7543 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2105 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6050 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5292 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/submission_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_config_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      407 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_config_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1244 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_feedback_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      381 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_feedback_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_scoring_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      396 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_scoring_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     7275 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    18070 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11063 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1372 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_test_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_test_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1867 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/version_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      995 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/atlas/version_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.551532 eolymp-0.8.1/eolymp/auth/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/auth/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1650 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/claims_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/claims_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      493 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/oauth2_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6035 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5486 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)      490 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/sso_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     2894 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/sso_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1917 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/auth/sso_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.555532 eolymp-0.8.1/eolymp/cognito/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/cognito/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/access_key_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      997 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/access_key_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8102 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/cognito_http.py
+-rw-r--r--   0 root         (0) root         (0)    25518 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/cognito_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    21124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/cognito_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1170 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/quota_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      482 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/quota_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2297 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2923 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/cognito/user_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.559533 eolymp-0.8.1/eolymp/community/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/community/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3544 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/account_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     9900 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/account_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/account_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2632 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2568 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     7127 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4511 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/attribute_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1627 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_idp_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1447 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_idp_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1188 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3759 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/configuration_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1696 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_ghost_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_ghost_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2173 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4017 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    11354 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8833 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1195 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_team_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      469 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_team_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2124 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_user_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2513 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/member_user_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1187 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/membership_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/membership_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/community/membership_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.563533 eolymp-0.8.1/eolymp/content/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/content/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3542 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/content_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    10435 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/content_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7524 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/content_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/fragment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/content/fragment_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.563533 eolymp-0.8.1/eolymp/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/core/http_client.py
+-rw-r--r--   0 root         (0) root         (0)     2288 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/core/oauth_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.567533 eolymp-0.8.1/eolymp/discussion/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/discussion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2180 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2032 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3064 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8074 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4433 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1387 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2478 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6622 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3860 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/forum_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1825 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1646 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     8680 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6502 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/message_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1442 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      734 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1185 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3644 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.567533 eolymp-0.8.1/eolymp/ecm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ecm/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/content_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      784 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/content_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1487 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/node_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/ecm/node_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.571534 eolymp-0.8.1/eolymp/executor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/executor/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      834 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/executor_http.py
+-rw-r--r--   0 root         (0) root         (0)     8384 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/executor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     5724 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/executor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1705 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/interactor_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/interactor_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6109 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11298 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1225 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/language_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      565 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/language_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     5233 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/report_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7802 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/report_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1290 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/runtime_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      752 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/runtime_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/status_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4284 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/status_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/task_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6288 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/task_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/usage_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1635 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/usage_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1950 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/verifier_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2026 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/executor/verifier_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.575534 eolymp-0.8.1/eolymp/geography/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/geography/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1223 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/country_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      549 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/country_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2233 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/geography_http.py
+-rw-r--r--   0 root         (0) root         (0)     4943 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/geography_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2558 2023-08-05 15:23:53.000000 eolymp-0.8.1/eolymp/geography/geography_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/geography/region_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      660 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/geography/region_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.575534 eolymp-0.8.1/eolymp/harmony/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1265 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/agreement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      686 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/agreement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1727 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/consent_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/consent_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2234 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/harmony_http.py
+-rw-r--r--   0 root         (0) root         (0)     4871 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/harmony_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2717 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/harmony/harmony_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.579534 eolymp-0.8.1/eolymp/helpdesk/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1422 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1458 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/document_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1126 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/document_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2439 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3573 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/helpdesk_http.py
+-rw-r--r--   0 root         (0) root         (0)    10284 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7297 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/support_http.py
+-rw-r--r--   0 root         (0) root         (0)    19983 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/support_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    13222 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/support_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3595 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4215 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.587535 eolymp-0.8.1/eolymp/judge/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2179 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/acl_http.py
+-rw-r--r--   0 root         (0) root         (0)     5512 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/acl_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/acl_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2389 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2641 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/announcement_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/announcement_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3524 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/contest_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/contest_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3285 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3207 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)    37756 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/judge_http.py
+-rw-r--r--   0 root         (0) root         (0)    78184 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/judge_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    54096 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/judge_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2522 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/participant_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/participant_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3088 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/problem_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4266 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/problem_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1519 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/reply_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1141 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/reply_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1491 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/result_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1178 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/result_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2586 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/score_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/score_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4771 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/submission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7066 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/submission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1557 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/template_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/template_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1768 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/ticket_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/judge/ticket_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.587535 eolymp-0.8.1/eolymp/keeper/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1257 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/blob_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      726 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/blob_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2965 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/keeper_http.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/keeper_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     4406 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/keeper/keeper_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.587535 eolymp-0.8.1/eolymp/l10n/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9434 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/localization_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/localization_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15558 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/localization_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1252 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      753 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3835 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2221 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/project_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1460 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/term_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/term_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1851 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/translation_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/l10n/translation_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.591535 eolymp-0.8.1/eolymp/oauth2/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      486 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/oauth2_http.py
+-rw-r--r--   0 root         (0) root         (0)     8147 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9528 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.591535 eolymp-0.8.1/eolymp/playground/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1689 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/playground_http.py
+-rw-r--r--   0 root         (0) root         (0)     4248 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/playground_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1982 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/playground_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2162 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/run_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2275 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/playground/run_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.591535 eolymp-0.8.1/eolymp/ranker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2245 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/activity_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/activity_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1165 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/format_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      335 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/format_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     8724 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/ranker_http.py
+-rw-r--r--   0 root         (0) root         (0)    21385 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/ranker_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    15143 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/ranker_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4876 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     8126 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.595536 eolymp-0.8.1/eolymp/resolver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      923 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/resolver_http.py
+-rw-r--r--   0 root         (0) root         (0)     3800 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/resolver_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3246 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/resolver/resolver_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.595536 eolymp-0.8.1/eolymp/taxonomy/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1145 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/link_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     3120 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1167 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1496 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1377 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4010 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_service_http.py
+-rw-r--r--   0 root         (0) root         (0)    10053 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     6654 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.599536 eolymp-0.8.1/eolymp/typewriter/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7630 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/block_pb2.py
+-rw-r--r--   0 root         (0) root         (0)    11265 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/block_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1443 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      704 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     1456 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/fragment_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/fragment_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/inline_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/inline_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     3884 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/typewriter_http.py
+-rw-r--r--   0 root         (0) root         (0)    11054 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.599536 eolymp-0.8.1/eolymp/universe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1501 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/permission_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      921 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/permission_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/space_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3986 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/space_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/universe_http.py
+-rw-r--r--   0 root         (0) root         (0)    14148 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/universe_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     9254 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/universe/universe_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.599536 eolymp-0.8.1/eolymp/wellknown/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1190 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/direction_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      331 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/direction_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2426 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/errors_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2458 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/errors_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     4481 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/expression_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3915 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/wellknown/expression_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.603536 eolymp-0.8.1/eolymp/worker/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1274 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/events_pb2.py
+-rw-r--r--   0 root         (0) root         (0)      505 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/events_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2649 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/job_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     2880 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/job_pb2.pyi
+-rw-r--r--   0 root         (0) root         (0)     2751 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/worker_service_http.py
+-rw-r--r--   0 root         (0) root         (0)     6564 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/worker_service_pb2.py
+-rw-r--r--   0 root         (0) root         (0)     3389 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp/worker/worker_service_pb2.pyi
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 15:23:54.531530 eolymp-0.8.1/eolymp.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      911 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11858 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-05 15:23:54.000000 eolymp-0.8.1/eolymp.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 15:23:54.603536 eolymp-0.8.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      974 2023-08-05 15:23:54.000000 eolymp-0.8.1/setup.py
```

### Comparing `eolymp-0.8.0/PKG-INFO` & `eolymp-0.8.1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.8.0
+Version: 0.8.1
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.8.0/README.md` & `eolymp-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/acl/acl_service_http.py` & `eolymp-0.8.1/eolymp/acl/acl_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/acl/acl_service_pb2.py` & `eolymp-0.8.1/eolymp/acl/acl_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/acl/acl_service_pb2.pyi` & `eolymp-0.8.1/eolymp/acl/acl_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/endpoint_pb2.py` & `eolymp-0.8.1/eolymp/annotations/endpoint_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/endpoint_pb2.pyi` & `eolymp-0.8.1/eolymp/annotations/endpoint_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/http_pb2.py` & `eolymp-0.8.1/eolymp/annotations/http_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/http_pb2.pyi` & `eolymp-0.8.1/eolymp/annotations/http_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/ratelimit_pb2.py` & `eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/ratelimit_pb2.pyi` & `eolymp-0.8.1/eolymp/annotations/ratelimit_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/scope_pb2.py` & `eolymp-0.8.1/eolymp/annotations/scope_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/annotations/scope_pb2.pyi` & `eolymp-0.8.1/eolymp/annotations/scope_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/apollo/events_pb2.py` & `eolymp-0.8.1/eolymp/apollo/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/apollo/events_pb2.pyi` & `eolymp-0.8.1/eolymp/apollo/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/asset/asset_http.py` & `eolymp-0.8.1/eolymp/asset/asset_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/asset/asset_pb2.py` & `eolymp-0.8.1/eolymp/asset/asset_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/asset/asset_pb2.pyi` & `eolymp-0.8.1/eolymp/asset/asset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/asset_service_http.py` & `eolymp-0.8.1/eolymp/atlas/asset_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/asset_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/asset_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/asset_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/asset_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/atlas_http.py` & `eolymp-0.8.1/eolymp/atlas/atlas_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/atlas_pb2.py` & `eolymp-0.8.1/eolymp/atlas/atlas_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/atlas_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/atlas_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/attachment_pb2.py` & `eolymp-0.8.1/eolymp/atlas/attachment_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/attachment_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/attachment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/attachment_service_http.py` & `eolymp-0.8.1/eolymp/atlas/attachment_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/attachment_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/attachment_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/attachment_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/bookmark_service_http.py` & `eolymp-0.8.1/eolymp/atlas/bookmark_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/bookmark_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/bookmark_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/bookmark_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_file_pb2.py` & `eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_file_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/code_template_file_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_pb2.py` & `eolymp-0.8.1/eolymp/atlas/code_template_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/code_template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_service_http.py` & `eolymp-0.8.1/eolymp/atlas/code_template_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/code_template_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/code_template_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/editorial_pb2.py` & `eolymp-0.8.1/eolymp/atlas/editorial_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/editorial_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/editorial_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/editorial_service_http.py` & `eolymp-0.8.1/eolymp/atlas/editorial_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/editorial_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/editorial_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/editorial_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/events_pb2.py` & `eolymp-0.8.1/eolymp/atlas/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/events_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/library_service_http.py` & `eolymp-0.8.1/eolymp/atlas/library_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/library_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/library_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/library_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/library_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/problem_pb2.py` & `eolymp-0.8.1/eolymp/atlas/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/problem_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/problem_service_http.py` & `eolymp-0.8.1/eolymp/atlas/problem_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/problem_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/problem_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/problem_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/problem_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/scoring_score_pb2.py` & `eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/scoring_score_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/scoring_score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/scoring_service_http.py` & `eolymp-0.8.1/eolymp/atlas/scoring_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/scoring_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/scoring_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/scoring_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/solution_pb2.py` & `eolymp-0.8.1/eolymp/atlas/solution_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/solution_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/solution_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/statement_pb2.py` & `eolymp-0.8.1/eolymp/atlas/statement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/statement_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/statement_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/statement_service_http.py` & `eolymp-0.8.1/eolymp/atlas/statement_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/statement_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/statement_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/statement_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/statement_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/submission_pb2.py` & `eolymp-0.8.1/eolymp/atlas/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/submission_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/submission_service_http.py` & `eolymp-0.8.1/eolymp/atlas/submission_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/submission_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/submission_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/submission_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/submission_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_config_pb2.py` & `eolymp-0.8.1/eolymp/atlas/testing_config_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_feedback_pb2.py` & `eolymp-0.8.1/eolymp/atlas/testing_feedback_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_scoring_pb2.py` & `eolymp-0.8.1/eolymp/atlas/testing_scoring_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_service_http.py` & `eolymp-0.8.1/eolymp/atlas/testing_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_service_pb2.py` & `eolymp-0.8.1/eolymp/atlas/testing_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_service_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/testing_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_test_pb2.py` & `eolymp-0.8.1/eolymp/atlas/testing_test_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_test_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/testing_test_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_testset_pb2.py` & `eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/testing_testset_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/testing_testset_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/version_pb2.py` & `eolymp-0.8.1/eolymp/atlas/version_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/atlas/version_pb2.pyi` & `eolymp-0.8.1/eolymp/atlas/version_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/auth/claims_pb2.py` & `eolymp-0.8.1/eolymp/auth/claims_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/auth/claims_pb2.pyi` & `eolymp-0.8.1/eolymp/auth/claims_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/auth/oauth2_service_pb2.py` & `eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/auth/oauth2_service_pb2.pyi` & `eolymp-0.8.1/eolymp/auth/oauth2_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/auth/sso_service_pb2.py` & `eolymp-0.8.1/eolymp/auth/sso_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/auth/sso_service_pb2.pyi` & `eolymp-0.8.1/eolymp/auth/sso_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/cognito/access_key_pb2.py` & `eolymp-0.8.1/eolymp/cognito/access_key_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/cognito/access_key_pb2.pyi` & `eolymp-0.8.1/eolymp/cognito/access_key_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/cognito/cognito_http.py` & `eolymp-0.8.1/eolymp/cognito/cognito_http.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,25 +248,14 @@
             method="POST",
             url=self.url+path,
             request_data=request,
             response_symbol=_sym_db.GetSymbol("eolymp.cognito.CompleteRecoverOutput"),
             **kwargs,
         )
 
-    def ListEntitlements(self, request, **kwargs):
-        path = "/__cognito/entitlements"
-
-        return self.transport.request(
-            method="GET",
-            url=self.url+path,
-            request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.cognito.ListEntitlementsOutput"),
-            **kwargs,
-        )
-
     def SelfDestruct(self, request, **kwargs):
         path = "/self"
 
         return self.transport.request(
             method="DELETE",
             url=self.url+path,
             request_data=request,
```

### Comparing `eolymp-0.8.0/eolymp/cognito/cognito_pb2.py` & `eolymp-0.8.1/eolymp/cognito/cognito_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,22 +11,21 @@
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.cognito import access_key_pb2 as eolymp_dot_cognito_dot_access__key__pb2
-from eolymp.cognito import entitlement_pb2 as eolymp_dot_cognito_dot_entitlement__pb2
 from eolymp.cognito import quota_pb2 as eolymp_dot_cognito_dot_quota__pb2
 from eolymp.cognito import user_pb2 as eolymp_dot_cognito_dot_user__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x65olymp/cognito/cognito.proto\x12\x0e\x65olymp.cognito\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1f\x65olymp/cognito/access_key.proto\x1a eolymp/cognito/entitlement.proto\x1a\x1a\x65olymp/cognito/quota.proto\x1a\x19\x65olymp/cognito/user.proto\x1a!eolymp/wellknown/expression.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xcc\x02\n\x10\x43reateTokenInput\x12>\n\ngrant_type\x18\x01 \x01(\x0e\x32*.eolymp.cognito.CreateTokenInput.GrantType\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x11\n\tclient_id\x18\x04 \x01(\t\x12\x15\n\rclient_secret\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x15\n\rcode_verifier\x18\x07 \x01(\t\x12\r\n\x05scope\x18\x08 \x01(\t\x12\x15\n\rrefresh_token\x18\t \x01(\t\"_\n\tGrantType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08PASSWORD\x10\x01\x12\x16\n\x12\x41UTHORIZATION_CODE\x10\x02\x12\x11\n\rREFRESH_TOKEN\x10\x03\x12\x0f\n\x0bGOOGLE_CODE\x10\x04\"\xaa\x01\n\x11\x43reateTokenOutput\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12.\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x15\n\rrefresh_token\x18\n \x01(\t\x12\x0f\n\x07user_id\x18\x64 \x01(\t\x12\x10\n\x08username\x18\x65 \x01(\t\"%\n\x14IntrospectTokenInput\x12\r\n\x05token\x18\x01 \x01(\t\"\xfd\x01\n\x15IntrospectTokenOutput\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\r\n\x05scope\x18\x02 \x01(\t\x12*\n\x06\x65xpire\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07subject\x18\x04 \x01(\t\x12\x10\n\x08\x61udience\x18\x05 \x01(\t\x12\x0e\n\x06issuer\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x64 \x01(\t\x12\x10\n\x08nickname\x18\x65 \x01(\t\x12\x0f\n\x07picture\x18\x66 \x01(\t\x12\r\n\x05\x65mail\x18g \x01(\t\x12\x16\n\x0e\x65mail_verified\x18h \x01(\x08\x12\x0e\n\x06locale\x18i \x01(\t\"\xaf\x01\n\x18\x43reateAuthorizationInput\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63ode_challenge\x18\x02 \x01(\t\x12\x1d\n\x15\x63ode_challenge_method\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x15\n\rresponse_type\x18\x05 \x01(\t\x12\r\n\x05scope\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\"M\n\x19\x43reateAuthorizationOutput\x12\x1a\n\x12\x61uthorization_code\x18\x01 \x01(\t\x12\x14\n\x0credirect_uri\x18\x02 \x01(\t\"\x16\n\x14IntrospectQuotaInput\"\xe9\x01\n\x15IntrospectQuotaOutput\x12\x30\n\x11\x63ontests_per_user\x18\n \x01(\x0b\x32\x15.eolymp.cognito.Quota\x12\x33\n\x14problems_per_contest\x18\x0b \x01(\x0b\x32\x15.eolymp.cognito.Quota\x12\x37\n\x18participants_per_contest\x18\x0c \x01(\x0b\x32\x15.eolymp.cognito.Quota\x12\x30\n\x11problems_per_user\x18\x14 \x01(\x0b\x32\x15.eolymp.cognito.Quota\"\x15\n\x13IntrospectUserInput\":\n\x14IntrospectUserOutput\x12\"\n\x04user\x18\x01 \x01(\x0b\x32\x14.eolymp.cognito.User\"$\n\x11\x44\x65scribeUserInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"8\n\x12\x44\x65scribeUserOutput\x12\"\n\x04user\x18\x01 \x01(\x0b\x32\x14.eolymp.cognito.User\"\xd2\x01\n\x0eListUsersInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x36\n\x07\x66ilters\x18( \x01(\x0b\x32%.eolymp.cognito.ListUsersInput.Filter\x1aj\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x34\n\x08username\x18\x02 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"E\n\x0fListUsersOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12#\n\x05items\x18\x02 \x03(\x0b\x32\x14.eolymp.cognito.User\"\x9b\x01\n\x0f\x43reateUserInput\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x11\n\tfull_name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x10\n\x08\x62irthday\x18\x06 \x01(\t\x12\x0f\n\x07\x63\x61ptcha\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x14 \x01(\t\"D\n\x10\x43reateUserOutput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x02 \x01(\t\"\xac\x01\n\x0fNotifyUserInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12\x43\n\nparameters\x18\x03 \x03(\x0b\x32/.eolymp.cognito.NotifyUserInput.ParametersEntry\x1a\x31\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"+\n\x10NotifyUserOutput\x12\x17\n\x0fnotification_id\x18\x01 \x01(\t\"3\n\x10VerifyEmailInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"\x13\n\x11VerifyEmailOutput\"!\n\x10UpdateEmailInput\x12\r\n\x05\x65mail\x18\x01 \x01(\t\"4\n\x11UpdateEmailOutput\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x02 \x01(\t\"\xdc\x02\n\x12UpdateProfileInput\x12\x37\n\x05patch\x18\x01 \x03(\x0e\x32(.eolymp.cognito.UpdateProfileInput.Patch\x12\x10\n\x08username\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\n \x01(\t\x12\x0f\n\x07\x63ompany\x18\x0c \x01(\t\x12\x12\n\noccupation\x18\r \x01(\t\x12\x0f\n\x07\x63ountry\x18\x15 \x01(\t\x12\x0c\n\x04\x63ity\x18\x16 \x01(\t\x12\x10\n\x08\x62irthday\x18! \x01(\t\x12\x0e\n\x06locale\x18\" \x01(\t\"x\n\x05Patch\x12\x0c\n\x08USERNAME\x10\x00\x12\t\n\x05\x45MAIL\x10\x01\x12\x08\n\x04NAME\x10\x02\x12\x0b\n\x07\x43OMPANY\x10\x03\x12\x0e\n\nOCCUPATION\x10\x04\x12\x0b\n\x07\x43OUNTRY\x10\x05\x12\x08\n\x04\x43ITY\x10\x06\x12\x0c\n\x08\x42IRTHDAY\x10\x07\x12\n\n\x06LOCALE\x10\x08\"6\n\x13UpdateProfileOutput\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x01 \x01(\t\"f\n\x12UpdatePictureInput\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x10\n\x08offset_x\x18\n \x01(\r\x12\x10\n\x08offset_y\x18\x0b \x01(\r\x12\x0c\n\x04size\x18\x0c \x01(\r\"\x15\n\x13UpdatePictureOutput\"E\n\x13UpdatePasswordInput\x12\x18\n\x10\x63urrent_password\x18\x01 \x01(\t\x12\x14\n\x0cnew_password\x18\x02 \x01(\t\"\x16\n\x14UpdatePasswordOutput\"\x1e\n\x1cResendEmailVerificationInput\"@\n\x1dResendEmailVerificationOutput\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x01 \x01(\t\"D\n\x12StartRecoveryInput\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61ptcha\x18\x02 \x01(\t\x12\x0e\n\x06locale\x18\x14 \x01(\t\"2\n\x13StartRecoveryOutput\x12\x1b\n\x13\x65mail_recovery_hint\x18\x01 \x01(\t\"I\n\x14\x43ompleteRecoverInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"\x17\n\x15\x43ompleteRecoverOutput\"\x16\n\x14IntrospectRolesInput\"&\n\x15IntrospectRolesOutput\x12\r\n\x05roles\x18\x01 \x03(\t\"!\n\x0eListRolesInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\" \n\x0fListRolesOutput\x12\r\n\x05roles\x18\x01 \x03(\t\"2\n\x10UpdateRolesInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\r\n\x05roles\x18\x02 \x03(\t\"\x13\n\x11UpdateRolesOutput\"\x17\n\x15ListEntitlementsInput\"K\n\x16ListEntitlementsOutput\x12\x31\n\x0c\x65ntitlements\x18\x01 \x03(\x0e\x32\x1b.eolymp.cognito.Entitlement\"\x13\n\x11SelfDestructInput\"C\n\x12SelfDestructOutput\x12-\n\tdelete_on\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"!\n\x10RevokeTokenInput\x12\r\n\x05token\x18\x01 \x01(\t\"\x13\n\x11RevokeTokenOutput\"1\n\x0bSigninInput\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x0cSigninOutput\x12\"\n\x04user\x18\x01 \x01(\x0b\x32\x14.eolymp.cognito.User\"\"\n\x0cSignoutInput\x12\x12\n\neverywhere\x18\x01 \x01(\x08\"\x0f\n\rSignoutOutput\"G\n\x14\x43reateAccessKeyInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05scope\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\r\"7\n\x15\x43reateAccessKeyOutput\x12\x0e\n\x06key_id\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"&\n\x14\x44\x65leteAccessKeyInput\x12\x0e\n\x06key_id\x18\x01 \x01(\t\"\x17\n\x15\x44\x65leteAccessKeyOutput\"3\n\x13ListAccessKeysInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"O\n\x14ListAccessKeysOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12(\n\x05items\x18\x02 \x03(\x0b\x32\x19.eolymp.cognito.AccessKey2\xd3\x1a\n\x07\x43ognito\x12\x64\n\x0b\x43reateToken\x12 .eolymp.cognito.CreateTokenInput\x1a!.eolymp.cognito.CreateTokenOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12o\n\x0fIntrospectToken\x12$.eolymp.cognito.IntrospectTokenInput\x1a%.eolymp.cognito.IntrospectTokenOutput\"\x0f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x12\x63\n\x0bRevokeToken\x12 .eolymp.cognito.RevokeTokenInput\x1a!.eolymp.cognito.RevokeTokenOutput\"\x0f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x12l\n\x07Signout\x12\x1c.eolymp.cognito.SignoutInput\x1a\x1d.eolymp.cognito.SignoutOutput\"$\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x0f\"\r/self/signout\x12\xa3\x01\n\x0f\x43reateAccessKey\x12$.eolymp.cognito.CreateAccessKeyInput\x1a%.eolymp.cognito.CreateAccessKeyOutput\"C\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ognito:access-key:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x0e\"\x0c/access-keys\x12\xac\x01\n\x0f\x44\x65leteAccessKey\x12$.eolymp.cognito.DeleteAccessKeyInput\x1a%.eolymp.cognito.DeleteAccessKeyOutput\"L\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ognito:access-key:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x17*\x15/access-keys/{key_id}\x12\x9f\x01\n\x0eListAccessKeys\x12#.eolymp.cognito.ListAccessKeysInput\x1a$.eolymp.cognito.ListAccessKeysOutput\"B\x82\xe3\n\x1b\x8a\xe3\n\x17\x63ognito:access-key:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0e\x12\x0c/access-keys\x12n\n\nCreateUser\x12\x1f.eolymp.cognito.CreateUserInput\x1a .eolymp.cognito.CreateUserOutput\"\x1d\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x08\"\x06/users\x12\x82\x01\n\x0bVerifyEmail\x12 .eolymp.cognito.VerifyEmailInput\x1a!.eolymp.cognito.VerifyEmailOutput\".\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x01\x82\xd3\xe4\x93\x02\x19\"\x17/users/{user_id}/verify\x12\xae\x01\n\x17ResendEmailVerification\x12,.eolymp.cognito.ResendEmailVerificationInput\x1a-.eolymp.cognito.ResendEmailVerificationOutput\"6\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02!\"\x1f/self/email/resend-verification\x12v\n\x0bUpdateEmail\x12 .eolymp.cognito.UpdateEmailInput\x1a!.eolymp.cognito.UpdateEmailOutput\"\"\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x01\x82\xd3\xe4\x93\x02\r\"\x0b/self/email\x12v\n\rUpdateProfile\x12\".eolymp.cognito.UpdateProfileInput\x1a#.eolymp.cognito.UpdateProfileOutput\"\x1c\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x07\"\x05/self\x12~\n\rUpdatePicture\x12\".eolymp.cognito.UpdatePictureInput\x1a#.eolymp.cognito.UpdatePictureOutput\"$\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0f\"\r/self/picture\x12\x98\x01\n\x0eUpdatePassword\x12#.eolymp.cognito.UpdatePasswordInput\x1a$.eolymp.cognito.UpdatePasswordOutput\";\x82\xe3\n\x12\x8a\xe3\n\x0epassword_grant\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x10\"\x0e/self/password\x12y\n\x0eIntrospectUser\x12#.eolymp.cognito.IntrospectUserInput\x1a$.eolymp.cognito.IntrospectUserOutput\"\x1c\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x07\x12\x05/self\x12\x98\x01\n\x0c\x44\x65scribeUser\x12!.eolymp.cognito.DescribeUserInput\x1a\".eolymp.cognito.DescribeUserOutput\"A\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:user:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HC\xf8\xe2\n\xf4\x03\x82\xd3\xe4\x93\x02\x12\x12\x10/users/{user_id}\x12\x84\x01\n\tListUsers\x12\x1e.eolymp.cognito.ListUsersInput\x1a\x1f.eolymp.cognito.ListUsersOutput\"6\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:user:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00pA\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x08\x12\x06/users\x12\x82\x01\n\x0fIntrospectQuota\x12$.eolymp.cognito.IntrospectQuotaInput\x1a%.eolymp.cognito.IntrospectQuotaOutput\"\"\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\r\x12\x0b/self/quota\x12\x82\x01\n\x0fIntrospectRoles\x12$.eolymp.cognito.IntrospectRolesInput\x1a%.eolymp.cognito.IntrospectRolesOutput\"\"\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\r\x12\x0b/self/roles\x12\x94\x01\n\tListRoles\x12\x1e.eolymp.cognito.ListRolesInput\x1a\x1f.eolymp.cognito.ListRolesOutput\"F\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:role:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x18\x12\x16/users/{user_id}/roles\x12\x9a\x01\n\x0bUpdateRoles\x12 .eolymp.cognito.UpdateRolesInput\x1a!.eolymp.cognito.UpdateRolesOutput\"F\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:role:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x18\x1a\x16/users/{user_id}/roles\x12\x7f\n\rStartRecovery\x12\".eolymp.cognito.StartRecoveryInput\x1a#.eolymp.cognito.StartRecoveryOutput\"%\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x10\"\x0e/self/recovery\x12\x90\x01\n\x10\x43ompleteRecovery\x12$.eolymp.cognito.CompleteRecoverInput\x1a%.eolymp.cognito.CompleteRecoverOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x1a\"\x18/users/{user_id}/recover\x12\x91\x01\n\x10ListEntitlements\x12%.eolymp.cognito.ListEntitlementsInput\x1a&.eolymp.cognito.ListEntitlementsOutput\".\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x19\x12\x17/__cognito/entitlements\x12s\n\x0cSelfDestruct\x12!.eolymp.cognito.SelfDestructInput\x1a\".eolymp.cognito.SelfDestructOutput\"\x1c\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x07*\x05/selfB1Z/github.com/eolymp/go-sdk/eolymp/cognito;cognitob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x65olymp/cognito/cognito.proto\x12\x0e\x65olymp.cognito\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1f\x65olymp/cognito/access_key.proto\x1a\x1a\x65olymp/cognito/quota.proto\x1a\x19\x65olymp/cognito/user.proto\x1a!eolymp/wellknown/expression.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xcc\x02\n\x10\x43reateTokenInput\x12>\n\ngrant_type\x18\x01 \x01(\x0e\x32*.eolymp.cognito.CreateTokenInput.GrantType\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x11\n\tclient_id\x18\x04 \x01(\t\x12\x15\n\rclient_secret\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x15\n\rcode_verifier\x18\x07 \x01(\t\x12\r\n\x05scope\x18\x08 \x01(\t\x12\x15\n\rrefresh_token\x18\t \x01(\t\"_\n\tGrantType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08PASSWORD\x10\x01\x12\x16\n\x12\x41UTHORIZATION_CODE\x10\x02\x12\x11\n\rREFRESH_TOKEN\x10\x03\x12\x0f\n\x0bGOOGLE_CODE\x10\x04\"\xaa\x01\n\x11\x43reateTokenOutput\x12\r\n\x05token\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12.\n\nexpires_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06scopes\x18\x04 \x03(\t\x12\x15\n\rrefresh_token\x18\n \x01(\t\x12\x0f\n\x07user_id\x18\x64 \x01(\t\x12\x10\n\x08username\x18\x65 \x01(\t\"%\n\x14IntrospectTokenInput\x12\r\n\x05token\x18\x01 \x01(\t\"\xfd\x01\n\x15IntrospectTokenOutput\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\r\n\x05scope\x18\x02 \x01(\t\x12*\n\x06\x65xpire\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07subject\x18\x04 \x01(\t\x12\x10\n\x08\x61udience\x18\x05 \x01(\t\x12\x0e\n\x06issuer\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x64 \x01(\t\x12\x10\n\x08nickname\x18\x65 \x01(\t\x12\x0f\n\x07picture\x18\x66 \x01(\t\x12\r\n\x05\x65mail\x18g \x01(\t\x12\x16\n\x0e\x65mail_verified\x18h \x01(\x08\x12\x0e\n\x06locale\x18i \x01(\t\"\xaf\x01\n\x18\x43reateAuthorizationInput\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63ode_challenge\x18\x02 \x01(\t\x12\x1d\n\x15\x63ode_challenge_method\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x15\n\rresponse_type\x18\x05 \x01(\t\x12\r\n\x05scope\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\"M\n\x19\x43reateAuthorizationOutput\x12\x1a\n\x12\x61uthorization_code\x18\x01 \x01(\t\x12\x14\n\x0credirect_uri\x18\x02 \x01(\t\"\x16\n\x14IntrospectQuotaInput\"\xe9\x01\n\x15IntrospectQuotaOutput\x12\x30\n\x11\x63ontests_per_user\x18\n \x01(\x0b\x32\x15.eolymp.cognito.Quota\x12\x33\n\x14problems_per_contest\x18\x0b \x01(\x0b\x32\x15.eolymp.cognito.Quota\x12\x37\n\x18participants_per_contest\x18\x0c \x01(\x0b\x32\x15.eolymp.cognito.Quota\x12\x30\n\x11problems_per_user\x18\x14 \x01(\x0b\x32\x15.eolymp.cognito.Quota\"\x15\n\x13IntrospectUserInput\":\n\x14IntrospectUserOutput\x12\"\n\x04user\x18\x01 \x01(\x0b\x32\x14.eolymp.cognito.User\"$\n\x11\x44\x65scribeUserInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\"8\n\x12\x44\x65scribeUserOutput\x12\"\n\x04user\x18\x01 \x01(\x0b\x32\x14.eolymp.cognito.User\"\xd2\x01\n\x0eListUsersInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x36\n\x07\x66ilters\x18( \x01(\x0b\x32%.eolymp.cognito.ListUsersInput.Filter\x1aj\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x34\n\x08username\x18\x02 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"E\n\x0fListUsersOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12#\n\x05items\x18\x02 \x03(\x0b\x32\x14.eolymp.cognito.User\"\x9b\x01\n\x0f\x43reateUserInput\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x11\n\tfull_name\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x10\n\x08password\x18\x04 \x01(\t\x12\x0f\n\x07\x63ountry\x18\x05 \x01(\t\x12\x10\n\x08\x62irthday\x18\x06 \x01(\t\x12\x0f\n\x07\x63\x61ptcha\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x14 \x01(\t\"D\n\x10\x43reateUserOutput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x02 \x01(\t\"\xac\x01\n\x0fNotifyUserInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x10\n\x08template\x18\x02 \x01(\t\x12\x43\n\nparameters\x18\x03 \x03(\x0b\x32/.eolymp.cognito.NotifyUserInput.ParametersEntry\x1a\x31\n\x0fParametersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"+\n\x10NotifyUserOutput\x12\x17\n\x0fnotification_id\x18\x01 \x01(\t\"3\n\x10VerifyEmailInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"\x13\n\x11VerifyEmailOutput\"!\n\x10UpdateEmailInput\x12\r\n\x05\x65mail\x18\x01 \x01(\t\"4\n\x11UpdateEmailOutput\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x02 \x01(\t\"\xdc\x02\n\x12UpdateProfileInput\x12\x37\n\x05patch\x18\x01 \x03(\x0e\x32(.eolymp.cognito.UpdateProfileInput.Patch\x12\x10\n\x08username\x18\x02 \x01(\t\x12\r\n\x05\x65mail\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\n \x01(\t\x12\x0f\n\x07\x63ompany\x18\x0c \x01(\t\x12\x12\n\noccupation\x18\r \x01(\t\x12\x0f\n\x07\x63ountry\x18\x15 \x01(\t\x12\x0c\n\x04\x63ity\x18\x16 \x01(\t\x12\x10\n\x08\x62irthday\x18! \x01(\t\x12\x0e\n\x06locale\x18\" \x01(\t\"x\n\x05Patch\x12\x0c\n\x08USERNAME\x10\x00\x12\t\n\x05\x45MAIL\x10\x01\x12\x08\n\x04NAME\x10\x02\x12\x0b\n\x07\x43OMPANY\x10\x03\x12\x0e\n\nOCCUPATION\x10\x04\x12\x0b\n\x07\x43OUNTRY\x10\x05\x12\x08\n\x04\x43ITY\x10\x06\x12\x0c\n\x08\x42IRTHDAY\x10\x07\x12\n\n\x06LOCALE\x10\x08\"6\n\x13UpdateProfileOutput\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x01 \x01(\t\"f\n\x12UpdatePictureInput\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x10\n\x08offset_x\x18\n \x01(\r\x12\x10\n\x08offset_y\x18\x0b \x01(\r\x12\x0c\n\x04size\x18\x0c \x01(\r\"\x15\n\x13UpdatePictureOutput\"E\n\x13UpdatePasswordInput\x12\x18\n\x10\x63urrent_password\x18\x01 \x01(\t\x12\x14\n\x0cnew_password\x18\x02 \x01(\t\"\x16\n\x14UpdatePasswordOutput\"\x1e\n\x1cResendEmailVerificationInput\"@\n\x1dResendEmailVerificationOutput\x12\x1f\n\x17\x65mail_confirmation_hint\x18\x01 \x01(\t\"D\n\x12StartRecoveryInput\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x0f\n\x07\x63\x61ptcha\x18\x02 \x01(\t\x12\x0e\n\x06locale\x18\x14 \x01(\t\"2\n\x13StartRecoveryOutput\x12\x1b\n\x13\x65mail_recovery_hint\x18\x01 \x01(\t\"I\n\x14\x43ompleteRecoverInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\"\x17\n\x15\x43ompleteRecoverOutput\"\x16\n\x14IntrospectRolesInput\"&\n\x15IntrospectRolesOutput\x12\r\n\x05roles\x18\x01 \x03(\t\"!\n\x0eListRolesInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\" \n\x0fListRolesOutput\x12\r\n\x05roles\x18\x01 \x03(\t\"2\n\x10UpdateRolesInput\x12\x0f\n\x07user_id\x18\x01 \x01(\t\x12\r\n\x05roles\x18\x02 \x03(\t\"\x13\n\x11UpdateRolesOutput\"\x13\n\x11SelfDestructInput\"C\n\x12SelfDestructOutput\x12-\n\tdelete_on\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"!\n\x10RevokeTokenInput\x12\r\n\x05token\x18\x01 \x01(\t\"\x13\n\x11RevokeTokenOutput\"1\n\x0bSigninInput\x12\x10\n\x08username\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"2\n\x0cSigninOutput\x12\"\n\x04user\x18\x01 \x01(\x0b\x32\x14.eolymp.cognito.User\"\"\n\x0cSignoutInput\x12\x12\n\neverywhere\x18\x01 \x01(\x08\"\x0f\n\rSignoutOutput\"G\n\x14\x43reateAccessKeyInput\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05scope\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\r\"7\n\x15\x43reateAccessKeyOutput\x12\x0e\n\x06key_id\x18\x01 \x01(\t\x12\x0e\n\x06secret\x18\x02 \x01(\t\"&\n\x14\x44\x65leteAccessKeyInput\x12\x0e\n\x06key_id\x18\x01 \x01(\t\"\x17\n\x15\x44\x65leteAccessKeyOutput\"3\n\x13ListAccessKeysInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"O\n\x14ListAccessKeysOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12(\n\x05items\x18\x02 \x03(\x0b\x32\x19.eolymp.cognito.AccessKey2\xbf\x19\n\x07\x43ognito\x12\x64\n\x0b\x43reateToken\x12 .eolymp.cognito.CreateTokenInput\x1a!.eolymp.cognito.CreateTokenOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12o\n\x0fIntrospectToken\x12$.eolymp.cognito.IntrospectTokenInput\x1a%.eolymp.cognito.IntrospectTokenOutput\"\x0f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x12\x63\n\x0bRevokeToken\x12 .eolymp.cognito.RevokeTokenInput\x1a!.eolymp.cognito.RevokeTokenOutput\"\x0f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x12l\n\x07Signout\x12\x1c.eolymp.cognito.SignoutInput\x1a\x1d.eolymp.cognito.SignoutOutput\"$\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x0f\"\r/self/signout\x12\xa3\x01\n\x0f\x43reateAccessKey\x12$.eolymp.cognito.CreateAccessKeyInput\x1a%.eolymp.cognito.CreateAccessKeyOutput\"C\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ognito:access-key:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x0e\"\x0c/access-keys\x12\xac\x01\n\x0f\x44\x65leteAccessKey\x12$.eolymp.cognito.DeleteAccessKeyInput\x1a%.eolymp.cognito.DeleteAccessKeyOutput\"L\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ognito:access-key:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x17*\x15/access-keys/{key_id}\x12\x9f\x01\n\x0eListAccessKeys\x12#.eolymp.cognito.ListAccessKeysInput\x1a$.eolymp.cognito.ListAccessKeysOutput\"B\x82\xe3\n\x1b\x8a\xe3\n\x17\x63ognito:access-key:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x0e\x12\x0c/access-keys\x12n\n\nCreateUser\x12\x1f.eolymp.cognito.CreateUserInput\x1a .eolymp.cognito.CreateUserOutput\"\x1d\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x08\"\x06/users\x12\x82\x01\n\x0bVerifyEmail\x12 .eolymp.cognito.VerifyEmailInput\x1a!.eolymp.cognito.VerifyEmailOutput\".\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x01\x82\xd3\xe4\x93\x02\x19\"\x17/users/{user_id}/verify\x12\xae\x01\n\x17ResendEmailVerification\x12,.eolymp.cognito.ResendEmailVerificationInput\x1a-.eolymp.cognito.ResendEmailVerificationOutput\"6\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02!\"\x1f/self/email/resend-verification\x12v\n\x0bUpdateEmail\x12 .eolymp.cognito.UpdateEmailInput\x1a!.eolymp.cognito.UpdateEmailOutput\"\"\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x01\x82\xd3\xe4\x93\x02\r\"\x0b/self/email\x12v\n\rUpdateProfile\x12\".eolymp.cognito.UpdateProfileInput\x1a#.eolymp.cognito.UpdateProfileOutput\"\x1c\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x07\"\x05/self\x12~\n\rUpdatePicture\x12\".eolymp.cognito.UpdatePictureInput\x1a#.eolymp.cognito.UpdatePictureOutput\"$\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0f\"\r/self/picture\x12\x98\x01\n\x0eUpdatePassword\x12#.eolymp.cognito.UpdatePasswordInput\x1a$.eolymp.cognito.UpdatePasswordOutput\";\x82\xe3\n\x12\x8a\xe3\n\x0epassword_grant\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x10\"\x0e/self/password\x12y\n\x0eIntrospectUser\x12#.eolymp.cognito.IntrospectUserInput\x1a$.eolymp.cognito.IntrospectUserOutput\"\x1c\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x07\x12\x05/self\x12\x98\x01\n\x0c\x44\x65scribeUser\x12!.eolymp.cognito.DescribeUserInput\x1a\".eolymp.cognito.DescribeUserOutput\"A\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:user:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HC\xf8\xe2\n\xf4\x03\x82\xd3\xe4\x93\x02\x12\x12\x10/users/{user_id}\x12\x84\x01\n\tListUsers\x12\x1e.eolymp.cognito.ListUsersInput\x1a\x1f.eolymp.cognito.ListUsersOutput\"6\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:user:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00pA\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x08\x12\x06/users\x12\x82\x01\n\x0fIntrospectQuota\x12$.eolymp.cognito.IntrospectQuotaInput\x1a%.eolymp.cognito.IntrospectQuotaOutput\"\"\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\r\x12\x0b/self/quota\x12\x82\x01\n\x0fIntrospectRoles\x12$.eolymp.cognito.IntrospectRolesInput\x1a%.eolymp.cognito.IntrospectRolesOutput\"\"\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\r\x12\x0b/self/roles\x12\x94\x01\n\tListRoles\x12\x1e.eolymp.cognito.ListRolesInput\x1a\x1f.eolymp.cognito.ListRolesOutput\"F\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:role:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x18\x12\x16/users/{user_id}/roles\x12\x9a\x01\n\x0bUpdateRoles\x12 .eolymp.cognito.UpdateRolesInput\x1a!.eolymp.cognito.UpdateRolesOutput\"F\x82\xe3\n\x15\x8a\xe3\n\x11\x63ognito:role:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x18\x1a\x16/users/{user_id}/roles\x12\x7f\n\rStartRecovery\x12\".eolymp.cognito.StartRecoveryInput\x1a#.eolymp.cognito.StartRecoveryOutput\"%\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x10\"\x0e/self/recovery\x12\x90\x01\n\x10\x43ompleteRecovery\x12$.eolymp.cognito.CompleteRecoverInput\x1a%.eolymp.cognito.CompleteRecoverOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x1a\"\x18/users/{user_id}/recover\x12s\n\x0cSelfDestruct\x12!.eolymp.cognito.SelfDestructInput\x1a\".eolymp.cognito.SelfDestructOutput\"\x1c\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x07*\x05/selfB1Z/github.com/eolymp/go-sdk/eolymp/cognito;cognitob\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.cognito.cognito_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z/github.com/eolymp/go-sdk/eolymp/cognito;cognito'
@@ -74,134 +73,128 @@
   _COGNITO.methods_by_name['ListRoles']._serialized_options = b'\202\343\n\025\212\343\n\021cognito:role:read\352\342\n\013\365\342\n\000\000\200?\370\342\n\n\202\323\344\223\002\030\022\026/users/{user_id}/roles'
   _COGNITO.methods_by_name['UpdateRoles']._options = None
   _COGNITO.methods_by_name['UpdateRoles']._serialized_options = b'\202\343\n\025\212\343\n\021cognito:role:read\352\342\n\013\365\342\n\000\000\200?\370\342\n\n\202\323\344\223\002\030\032\026/users/{user_id}/roles'
   _COGNITO.methods_by_name['StartRecovery']._options = None
   _COGNITO.methods_by_name['StartRecovery']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\n2\202\323\344\223\002\020\"\016/self/recovery'
   _COGNITO.methods_by_name['CompleteRecovery']._options = None
   _COGNITO.methods_by_name['CompleteRecovery']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\n2\202\323\344\223\002\032\"\030/users/{user_id}/recover'
-  _COGNITO.methods_by_name['ListEntitlements']._options = None
-  _COGNITO.methods_by_name['ListEntitlements']._serialized_options = b'\352\342\n\013\365\342\n\000\000\200?\370\342\n\n\202\323\344\223\002\031\022\027/__cognito/entitlements'
   _COGNITO.methods_by_name['SelfDestruct']._options = None
   _COGNITO.methods_by_name['SelfDestruct']._serialized_options = b'\352\342\n\013\365\342\n\000\000\200?\370\342\n\n\202\323\344\223\002\007*\005/self'
-  _CREATETOKENINPUT._serialized_start=338
-  _CREATETOKENINPUT._serialized_end=670
-  _CREATETOKENINPUT_GRANTTYPE._serialized_start=575
-  _CREATETOKENINPUT_GRANTTYPE._serialized_end=670
-  _CREATETOKENOUTPUT._serialized_start=673
-  _CREATETOKENOUTPUT._serialized_end=843
-  _INTROSPECTTOKENINPUT._serialized_start=845
-  _INTROSPECTTOKENINPUT._serialized_end=882
-  _INTROSPECTTOKENOUTPUT._serialized_start=885
-  _INTROSPECTTOKENOUTPUT._serialized_end=1138
-  _CREATEAUTHORIZATIONINPUT._serialized_start=1141
-  _CREATEAUTHORIZATIONINPUT._serialized_end=1316
-  _CREATEAUTHORIZATIONOUTPUT._serialized_start=1318
-  _CREATEAUTHORIZATIONOUTPUT._serialized_end=1395
-  _INTROSPECTQUOTAINPUT._serialized_start=1397
-  _INTROSPECTQUOTAINPUT._serialized_end=1419
-  _INTROSPECTQUOTAOUTPUT._serialized_start=1422
-  _INTROSPECTQUOTAOUTPUT._serialized_end=1655
-  _INTROSPECTUSERINPUT._serialized_start=1657
-  _INTROSPECTUSERINPUT._serialized_end=1678
-  _INTROSPECTUSEROUTPUT._serialized_start=1680
-  _INTROSPECTUSEROUTPUT._serialized_end=1738
-  _DESCRIBEUSERINPUT._serialized_start=1740
-  _DESCRIBEUSERINPUT._serialized_end=1776
-  _DESCRIBEUSEROUTPUT._serialized_start=1778
-  _DESCRIBEUSEROUTPUT._serialized_end=1834
-  _LISTUSERSINPUT._serialized_start=1837
-  _LISTUSERSINPUT._serialized_end=2047
-  _LISTUSERSINPUT_FILTER._serialized_start=1941
-  _LISTUSERSINPUT_FILTER._serialized_end=2047
-  _LISTUSERSOUTPUT._serialized_start=2049
-  _LISTUSERSOUTPUT._serialized_end=2118
-  _CREATEUSERINPUT._serialized_start=2121
-  _CREATEUSERINPUT._serialized_end=2276
-  _CREATEUSEROUTPUT._serialized_start=2278
-  _CREATEUSEROUTPUT._serialized_end=2346
-  _NOTIFYUSERINPUT._serialized_start=2349
-  _NOTIFYUSERINPUT._serialized_end=2521
-  _NOTIFYUSERINPUT_PARAMETERSENTRY._serialized_start=2472
-  _NOTIFYUSERINPUT_PARAMETERSENTRY._serialized_end=2521
-  _NOTIFYUSEROUTPUT._serialized_start=2523
-  _NOTIFYUSEROUTPUT._serialized_end=2566
-  _VERIFYEMAILINPUT._serialized_start=2568
-  _VERIFYEMAILINPUT._serialized_end=2619
-  _VERIFYEMAILOUTPUT._serialized_start=2621
-  _VERIFYEMAILOUTPUT._serialized_end=2640
-  _UPDATEEMAILINPUT._serialized_start=2642
-  _UPDATEEMAILINPUT._serialized_end=2675
-  _UPDATEEMAILOUTPUT._serialized_start=2677
-  _UPDATEEMAILOUTPUT._serialized_end=2729
-  _UPDATEPROFILEINPUT._serialized_start=2732
-  _UPDATEPROFILEINPUT._serialized_end=3080
-  _UPDATEPROFILEINPUT_PATCH._serialized_start=2960
-  _UPDATEPROFILEINPUT_PATCH._serialized_end=3080
-  _UPDATEPROFILEOUTPUT._serialized_start=3082
-  _UPDATEPROFILEOUTPUT._serialized_end=3136
-  _UPDATEPICTUREINPUT._serialized_start=3138
-  _UPDATEPICTUREINPUT._serialized_end=3240
-  _UPDATEPICTUREOUTPUT._serialized_start=3242
-  _UPDATEPICTUREOUTPUT._serialized_end=3263
-  _UPDATEPASSWORDINPUT._serialized_start=3265
-  _UPDATEPASSWORDINPUT._serialized_end=3334
-  _UPDATEPASSWORDOUTPUT._serialized_start=3336
-  _UPDATEPASSWORDOUTPUT._serialized_end=3358
-  _RESENDEMAILVERIFICATIONINPUT._serialized_start=3360
-  _RESENDEMAILVERIFICATIONINPUT._serialized_end=3390
-  _RESENDEMAILVERIFICATIONOUTPUT._serialized_start=3392
-  _RESENDEMAILVERIFICATIONOUTPUT._serialized_end=3456
-  _STARTRECOVERYINPUT._serialized_start=3458
-  _STARTRECOVERYINPUT._serialized_end=3526
-  _STARTRECOVERYOUTPUT._serialized_start=3528
-  _STARTRECOVERYOUTPUT._serialized_end=3578
-  _COMPLETERECOVERINPUT._serialized_start=3580
-  _COMPLETERECOVERINPUT._serialized_end=3653
-  _COMPLETERECOVEROUTPUT._serialized_start=3655
-  _COMPLETERECOVEROUTPUT._serialized_end=3678
-  _INTROSPECTROLESINPUT._serialized_start=3680
-  _INTROSPECTROLESINPUT._serialized_end=3702
-  _INTROSPECTROLESOUTPUT._serialized_start=3704
-  _INTROSPECTROLESOUTPUT._serialized_end=3742
-  _LISTROLESINPUT._serialized_start=3744
-  _LISTROLESINPUT._serialized_end=3777
-  _LISTROLESOUTPUT._serialized_start=3779
-  _LISTROLESOUTPUT._serialized_end=3811
-  _UPDATEROLESINPUT._serialized_start=3813
-  _UPDATEROLESINPUT._serialized_end=3863
-  _UPDATEROLESOUTPUT._serialized_start=3865
-  _UPDATEROLESOUTPUT._serialized_end=3884
-  _LISTENTITLEMENTSINPUT._serialized_start=3886
-  _LISTENTITLEMENTSINPUT._serialized_end=3909
-  _LISTENTITLEMENTSOUTPUT._serialized_start=3911
-  _LISTENTITLEMENTSOUTPUT._serialized_end=3986
-  _SELFDESTRUCTINPUT._serialized_start=3988
-  _SELFDESTRUCTINPUT._serialized_end=4007
-  _SELFDESTRUCTOUTPUT._serialized_start=4009
-  _SELFDESTRUCTOUTPUT._serialized_end=4076
-  _REVOKETOKENINPUT._serialized_start=4078
-  _REVOKETOKENINPUT._serialized_end=4111
-  _REVOKETOKENOUTPUT._serialized_start=4113
-  _REVOKETOKENOUTPUT._serialized_end=4132
-  _SIGNININPUT._serialized_start=4134
-  _SIGNININPUT._serialized_end=4183
-  _SIGNINOUTPUT._serialized_start=4185
-  _SIGNINOUTPUT._serialized_end=4235
-  _SIGNOUTINPUT._serialized_start=4237
-  _SIGNOUTINPUT._serialized_end=4271
-  _SIGNOUTOUTPUT._serialized_start=4273
-  _SIGNOUTOUTPUT._serialized_end=4288
-  _CREATEACCESSKEYINPUT._serialized_start=4290
-  _CREATEACCESSKEYINPUT._serialized_end=4361
-  _CREATEACCESSKEYOUTPUT._serialized_start=4363
-  _CREATEACCESSKEYOUTPUT._serialized_end=4418
-  _DELETEACCESSKEYINPUT._serialized_start=4420
-  _DELETEACCESSKEYINPUT._serialized_end=4458
-  _DELETEACCESSKEYOUTPUT._serialized_start=4460
-  _DELETEACCESSKEYOUTPUT._serialized_end=4483
-  _LISTACCESSKEYSINPUT._serialized_start=4485
-  _LISTACCESSKEYSINPUT._serialized_end=4536
-  _LISTACCESSKEYSOUTPUT._serialized_start=4538
-  _LISTACCESSKEYSOUTPUT._serialized_end=4617
-  _COGNITO._serialized_start=4620
-  _COGNITO._serialized_end=8031
+  _CREATETOKENINPUT._serialized_start=304
+  _CREATETOKENINPUT._serialized_end=636
+  _CREATETOKENINPUT_GRANTTYPE._serialized_start=541
+  _CREATETOKENINPUT_GRANTTYPE._serialized_end=636
+  _CREATETOKENOUTPUT._serialized_start=639
+  _CREATETOKENOUTPUT._serialized_end=809
+  _INTROSPECTTOKENINPUT._serialized_start=811
+  _INTROSPECTTOKENINPUT._serialized_end=848
+  _INTROSPECTTOKENOUTPUT._serialized_start=851
+  _INTROSPECTTOKENOUTPUT._serialized_end=1104
+  _CREATEAUTHORIZATIONINPUT._serialized_start=1107
+  _CREATEAUTHORIZATIONINPUT._serialized_end=1282
+  _CREATEAUTHORIZATIONOUTPUT._serialized_start=1284
+  _CREATEAUTHORIZATIONOUTPUT._serialized_end=1361
+  _INTROSPECTQUOTAINPUT._serialized_start=1363
+  _INTROSPECTQUOTAINPUT._serialized_end=1385
+  _INTROSPECTQUOTAOUTPUT._serialized_start=1388
+  _INTROSPECTQUOTAOUTPUT._serialized_end=1621
+  _INTROSPECTUSERINPUT._serialized_start=1623
+  _INTROSPECTUSERINPUT._serialized_end=1644
+  _INTROSPECTUSEROUTPUT._serialized_start=1646
+  _INTROSPECTUSEROUTPUT._serialized_end=1704
+  _DESCRIBEUSERINPUT._serialized_start=1706
+  _DESCRIBEUSERINPUT._serialized_end=1742
+  _DESCRIBEUSEROUTPUT._serialized_start=1744
+  _DESCRIBEUSEROUTPUT._serialized_end=1800
+  _LISTUSERSINPUT._serialized_start=1803
+  _LISTUSERSINPUT._serialized_end=2013
+  _LISTUSERSINPUT_FILTER._serialized_start=1907
+  _LISTUSERSINPUT_FILTER._serialized_end=2013
+  _LISTUSERSOUTPUT._serialized_start=2015
+  _LISTUSERSOUTPUT._serialized_end=2084
+  _CREATEUSERINPUT._serialized_start=2087
+  _CREATEUSERINPUT._serialized_end=2242
+  _CREATEUSEROUTPUT._serialized_start=2244
+  _CREATEUSEROUTPUT._serialized_end=2312
+  _NOTIFYUSERINPUT._serialized_start=2315
+  _NOTIFYUSERINPUT._serialized_end=2487
+  _NOTIFYUSERINPUT_PARAMETERSENTRY._serialized_start=2438
+  _NOTIFYUSERINPUT_PARAMETERSENTRY._serialized_end=2487
+  _NOTIFYUSEROUTPUT._serialized_start=2489
+  _NOTIFYUSEROUTPUT._serialized_end=2532
+  _VERIFYEMAILINPUT._serialized_start=2534
+  _VERIFYEMAILINPUT._serialized_end=2585
+  _VERIFYEMAILOUTPUT._serialized_start=2587
+  _VERIFYEMAILOUTPUT._serialized_end=2606
+  _UPDATEEMAILINPUT._serialized_start=2608
+  _UPDATEEMAILINPUT._serialized_end=2641
+  _UPDATEEMAILOUTPUT._serialized_start=2643
+  _UPDATEEMAILOUTPUT._serialized_end=2695
+  _UPDATEPROFILEINPUT._serialized_start=2698
+  _UPDATEPROFILEINPUT._serialized_end=3046
+  _UPDATEPROFILEINPUT_PATCH._serialized_start=2926
+  _UPDATEPROFILEINPUT_PATCH._serialized_end=3046
+  _UPDATEPROFILEOUTPUT._serialized_start=3048
+  _UPDATEPROFILEOUTPUT._serialized_end=3102
+  _UPDATEPICTUREINPUT._serialized_start=3104
+  _UPDATEPICTUREINPUT._serialized_end=3206
+  _UPDATEPICTUREOUTPUT._serialized_start=3208
+  _UPDATEPICTUREOUTPUT._serialized_end=3229
+  _UPDATEPASSWORDINPUT._serialized_start=3231
+  _UPDATEPASSWORDINPUT._serialized_end=3300
+  _UPDATEPASSWORDOUTPUT._serialized_start=3302
+  _UPDATEPASSWORDOUTPUT._serialized_end=3324
+  _RESENDEMAILVERIFICATIONINPUT._serialized_start=3326
+  _RESENDEMAILVERIFICATIONINPUT._serialized_end=3356
+  _RESENDEMAILVERIFICATIONOUTPUT._serialized_start=3358
+  _RESENDEMAILVERIFICATIONOUTPUT._serialized_end=3422
+  _STARTRECOVERYINPUT._serialized_start=3424
+  _STARTRECOVERYINPUT._serialized_end=3492
+  _STARTRECOVERYOUTPUT._serialized_start=3494
+  _STARTRECOVERYOUTPUT._serialized_end=3544
+  _COMPLETERECOVERINPUT._serialized_start=3546
+  _COMPLETERECOVERINPUT._serialized_end=3619
+  _COMPLETERECOVEROUTPUT._serialized_start=3621
+  _COMPLETERECOVEROUTPUT._serialized_end=3644
+  _INTROSPECTROLESINPUT._serialized_start=3646
+  _INTROSPECTROLESINPUT._serialized_end=3668
+  _INTROSPECTROLESOUTPUT._serialized_start=3670
+  _INTROSPECTROLESOUTPUT._serialized_end=3708
+  _LISTROLESINPUT._serialized_start=3710
+  _LISTROLESINPUT._serialized_end=3743
+  _LISTROLESOUTPUT._serialized_start=3745
+  _LISTROLESOUTPUT._serialized_end=3777
+  _UPDATEROLESINPUT._serialized_start=3779
+  _UPDATEROLESINPUT._serialized_end=3829
+  _UPDATEROLESOUTPUT._serialized_start=3831
+  _UPDATEROLESOUTPUT._serialized_end=3850
+  _SELFDESTRUCTINPUT._serialized_start=3852
+  _SELFDESTRUCTINPUT._serialized_end=3871
+  _SELFDESTRUCTOUTPUT._serialized_start=3873
+  _SELFDESTRUCTOUTPUT._serialized_end=3940
+  _REVOKETOKENINPUT._serialized_start=3942
+  _REVOKETOKENINPUT._serialized_end=3975
+  _REVOKETOKENOUTPUT._serialized_start=3977
+  _REVOKETOKENOUTPUT._serialized_end=3996
+  _SIGNININPUT._serialized_start=3998
+  _SIGNININPUT._serialized_end=4047
+  _SIGNINOUTPUT._serialized_start=4049
+  _SIGNINOUTPUT._serialized_end=4099
+  _SIGNOUTINPUT._serialized_start=4101
+  _SIGNOUTINPUT._serialized_end=4135
+  _SIGNOUTOUTPUT._serialized_start=4137
+  _SIGNOUTOUTPUT._serialized_end=4152
+  _CREATEACCESSKEYINPUT._serialized_start=4154
+  _CREATEACCESSKEYINPUT._serialized_end=4225
+  _CREATEACCESSKEYOUTPUT._serialized_start=4227
+  _CREATEACCESSKEYOUTPUT._serialized_end=4282
+  _DELETEACCESSKEYINPUT._serialized_start=4284
+  _DELETEACCESSKEYINPUT._serialized_end=4322
+  _DELETEACCESSKEYOUTPUT._serialized_start=4324
+  _DELETEACCESSKEYOUTPUT._serialized_end=4347
+  _LISTACCESSKEYSINPUT._serialized_start=4349
+  _LISTACCESSKEYSINPUT._serialized_end=4400
+  _LISTACCESSKEYSOUTPUT._serialized_start=4402
+  _LISTACCESSKEYSOUTPUT._serialized_end=4481
+  _COGNITO._serialized_start=4484
+  _COGNITO._serialized_end=7747
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/cognito/cognito_pb2.pyi` & `eolymp-0.8.1/eolymp/cognito/cognito_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.cognito import access_key_pb2 as _access_key_pb2
-from eolymp.cognito import entitlement_pb2 as _entitlement_pb2
 from eolymp.cognito import quota_pb2 as _quota_pb2
 from eolymp.cognito import user_pb2 as _user_pb2
 from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
@@ -252,24 +251,14 @@
     __slots__ = ["items", "total"]
     ITEMS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     items: _containers.RepeatedCompositeFieldContainer[_access_key_pb2.AccessKey]
     total: int
     def __init__(self, total: _Optional[int] = ..., items: _Optional[_Iterable[_Union[_access_key_pb2.AccessKey, _Mapping]]] = ...) -> None: ...
 
-class ListEntitlementsInput(_message.Message):
-    __slots__ = []
-    def __init__(self) -> None: ...
-
-class ListEntitlementsOutput(_message.Message):
-    __slots__ = ["entitlements"]
-    ENTITLEMENTS_FIELD_NUMBER: _ClassVar[int]
-    entitlements: _containers.RepeatedScalarFieldContainer[_entitlement_pb2.Entitlement]
-    def __init__(self, entitlements: _Optional[_Iterable[_Union[_entitlement_pb2.Entitlement, str]]] = ...) -> None: ...
-
 class ListRolesInput(_message.Message):
     __slots__ = ["user_id"]
     USER_ID_FIELD_NUMBER: _ClassVar[int]
     user_id: str
     def __init__(self, user_id: _Optional[str] = ...) -> None: ...
 
 class ListRolesOutput(_message.Message):
```

### Comparing `eolymp-0.8.0/eolymp/cognito/entitlement_pb2.py` & `eolymp-0.8.1/eolymp/ranker/format_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/cognito/entitlement.proto
+# source: eolymp/ranker/format.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/cognito/entitlement.proto\x12\x0e\x65olymp.cognito*z\n\x0b\x45ntitlement\x12\x17\n\x13VIEW_PUBLIC_PROFILE\x10\x00\x12\x18\n\x14VIEW_BLOCKED_PROFILE\x10\x01\x12\x15\n\x11VIEW_PRIVATE_DATA\x10\x02\x12\x10\n\x0cMANAGE_ROLES\x10\x03\x12\x0f\n\x0b\x42LOCK_USERS\x10\x04\x42\x31Z/github.com/eolymp/go-sdk/eolymp/cognito;cognitob\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/ranker/format.proto\x12\reolymp.ranker*%\n\x06\x46ormat\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03IOI\x10\x01\x12\x08\n\x04ICPC\x10\x02\x42/Z-github.com/eolymp/go-sdk/eolymp/ranker;rankerb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.cognito.entitlement_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.ranker.format_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z/github.com/eolymp/go-sdk/eolymp/cognito;cognito'
-  _ENTITLEMENT._serialized_start=52
-  _ENTITLEMENT._serialized_end=174
+  DESCRIPTOR._serialized_options = b'Z-github.com/eolymp/go-sdk/eolymp/ranker;ranker'
+  _FORMAT._serialized_start=45
+  _FORMAT._serialized_end=82
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/cognito/quota_pb2.py` & `eolymp-0.8.1/eolymp/cognito/quota_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/cognito/user_pb2.py` & `eolymp-0.8.1/eolymp/cognito/user_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/cognito/user_pb2.pyi` & `eolymp-0.8.1/eolymp/cognito/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/account_service_http.py` & `eolymp-0.8.1/eolymp/community/account_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/account_service_pb2.py` & `eolymp-0.8.1/eolymp/community/account_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,18 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
-from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
 from eolymp.community import member_user_pb2 as eolymp_dot_community_dot_member__user__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&eolymp/community/account_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a eolymp/community/attribute.proto\x1a\x1d\x65olymp/community/member.proto\x1a\"eolymp/community/member_user.proto\"\x85\x01\n\x12\x43reateAccountInput\x12\'\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x16.eolymp.community.User\x12\x35\n\nattributes\x18\x02 \x03(\x0b\x32!.eolymp.community.Attribute.Value\x12\x0f\n\x07\x63\x61ptcha\x18\x64 \x01(\t\"#\n\x13\x43reateAccountOutput\x12\x0c\n\x04hint\x18\x64 \x01(\t\"\x16\n\x14\x44\x65scribeAccountInput\"w\n\x15\x44\x65scribeAccountOutput\x12\'\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x16.eolymp.community.User\x12\x35\n\nattributes\x18\x02 \x03(\x0b\x32!.eolymp.community.Attribute.Value\"\xeb\x03\n\x12UpdateAccountInput\x12\x39\n\x05patch\x18\x01 \x03(\x0e\x32*.eolymp.community.UpdateAccountInput.Patch\x12\x18\n\x10\x63urrent_password\x18\x02 \x01(\t\x12\'\n\x07\x61\x63\x63ount\x18\n \x01(\x0b\x32\x16.eolymp.community.User\x12\x35\n\nattributes\x18\x14 \x03(\x0b\x32!.eolymp.community.Attribute.Value\"\x9f\x02\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\x11\n\rUSER_NICKNAME\x10\x65\x12\x0e\n\nUSER_EMAIL\x10\x66\x12\x11\n\rUSER_PASSWORD\x10g\x12\r\n\tUSER_NAME\x10h\x12\x10\n\x0cUSER_PICTURE\x10i\x12\x11\n\rUSER_BIRTHDAY\x10j\x12\x10\n\x0cUSER_COUNTRY\x10k\x12\r\n\tUSER_CITY\x10l\x12\x14\n\x10USER_PREFERENCES\x10m\x12\x1c\n\x17USER_PREFERENCES_LOCALE\x10\xbe\x01\x12\x1e\n\x19USER_PREFERENCES_TIMEZONE\x10\xbf\x01\x12\x1d\n\x18USER_PREFERENCES_RUNTIME\x10\xc0\x01\x12\x0f\n\nATTRIBUTES\x10\x84\x07\"#\n\x13UpdateAccountOutput\x12\x0c\n\x04hint\x18\x01 \x01(\t\"f\n\x12UploadPictureInput\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x10\n\x08offset_x\x18\n \x01(\r\x12\x10\n\x08offset_y\x18\x0b \x01(\r\x12\x0c\n\x04size\x18\x0c \x01(\r\"\x15\n\x13UploadPictureOutput\"\x14\n\x12\x44\x65leteAccountInput\"\x15\n\x13\x44\x65leteAccountOutput\"\x19\n\x17ResendVerificationInput\"\x1a\n\x18ResendVerificationOutput\":\n\x19\x43ompleteVerificationInput\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\"\x1c\n\x1a\x43ompleteVerificationOutput\"D\n\x12StartRecoveryInput\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0f\n\x07\x63\x61ptcha\x18\x64 \x01(\t\"#\n\x13StartRecoveryOutput\x12\x0c\n\x04hint\x18\x01 \x01(\t\"G\n\x14\x43ompleteRecoverInput\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0f\n\x07subject\x18\x03 \x01(\t\"\x17\n\x15\x43ompleteRecoverOutput2\x91\n\n\x0e\x41\x63\x63ountService\x12}\n\rCreateAccount\x12$.eolymp.community.CreateAccountInput\x1a%.eolymp.community.CreateAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\n\"\x08/account\x12\x83\x01\n\x0f\x44\x65scribeAccount\x12&.eolymp.community.DescribeAccountInput\x1a\'.eolymp.community.DescribeAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\n\x12\x08/account\x12}\n\rUpdateAccount\x12$.eolymp.community.UpdateAccountInput\x1a%.eolymp.community.UpdateAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\n\x1a\x08/account\x12\x85\x01\n\rUploadPicture\x12$.eolymp.community.UploadPictureInput\x1a%.eolymp.community.UploadPictureOutput\"\'\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x12\"\x10/account/picture\x12}\n\rDeleteAccount\x12$.eolymp.community.DeleteAccountInput\x1a%.eolymp.community.DeleteAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\n*\x08/account\x12\xa0\x01\n\x12ResendVerification\x12).eolymp.community.ResendVerificationInput\x1a*.eolymp.community.ResendVerificationOutput\"3\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1e\"\x1c/account/verification/resend\x12\xa8\x01\n\x14\x43ompleteVerification\x12+.eolymp.community.CompleteVerificationInput\x1a,.eolymp.community.CompleteVerificationOutput\"5\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x01\x82\xd3\xe4\x93\x02 \"\x1e/account/verification/complete\x12\x8c\x01\n\rStartRecovery\x12$.eolymp.community.StartRecoveryInput\x1a%.eolymp.community.StartRecoveryOutput\".\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x19\"\x17/account/recovery/start\x12\x96\x01\n\x10\x43ompleteRecovery\x12&.eolymp.community.CompleteRecoverInput\x1a\'.eolymp.community.CompleteRecoverOutput\"1\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x1c\"\x1a/account/recovery/completeB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n&eolymp/community/account_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a eolymp/community/attribute.proto\x1a\"eolymp/community/member_user.proto\"\x85\x01\n\x12\x43reateAccountInput\x12\'\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x16.eolymp.community.User\x12\x35\n\nattributes\x18\x02 \x03(\x0b\x32!.eolymp.community.Attribute.Value\x12\x0f\n\x07\x63\x61ptcha\x18\x64 \x01(\t\"#\n\x13\x43reateAccountOutput\x12\x0c\n\x04hint\x18\x64 \x01(\t\"\x16\n\x14\x44\x65scribeAccountInput\"w\n\x15\x44\x65scribeAccountOutput\x12\'\n\x07\x61\x63\x63ount\x18\x01 \x01(\x0b\x32\x16.eolymp.community.User\x12\x35\n\nattributes\x18\x02 \x03(\x0b\x32!.eolymp.community.Attribute.Value\"\xeb\x03\n\x12UpdateAccountInput\x12\x39\n\x05patch\x18\x01 \x03(\x0e\x32*.eolymp.community.UpdateAccountInput.Patch\x12\x18\n\x10\x63urrent_password\x18\x02 \x01(\t\x12\'\n\x07\x61\x63\x63ount\x18\n \x01(\x0b\x32\x16.eolymp.community.User\x12\x35\n\nattributes\x18\x14 \x03(\x0b\x32!.eolymp.community.Attribute.Value\"\x9f\x02\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\x11\n\rUSER_NICKNAME\x10\x65\x12\x0e\n\nUSER_EMAIL\x10\x66\x12\x11\n\rUSER_PASSWORD\x10g\x12\r\n\tUSER_NAME\x10h\x12\x10\n\x0cUSER_PICTURE\x10i\x12\x11\n\rUSER_BIRTHDAY\x10j\x12\x10\n\x0cUSER_COUNTRY\x10k\x12\r\n\tUSER_CITY\x10l\x12\x14\n\x10USER_PREFERENCES\x10m\x12\x1c\n\x17USER_PREFERENCES_LOCALE\x10\xbe\x01\x12\x1e\n\x19USER_PREFERENCES_TIMEZONE\x10\xbf\x01\x12\x1d\n\x18USER_PREFERENCES_RUNTIME\x10\xc0\x01\x12\x0f\n\nATTRIBUTES\x10\x84\x07\"#\n\x13UpdateAccountOutput\x12\x0c\n\x04hint\x18\x01 \x01(\t\"f\n\x12UploadPictureInput\x12\x10\n\x08\x66ilename\x18\x01 \x01(\t\x12\x0c\n\x04\x64\x61ta\x18\x02 \x01(\x0c\x12\x10\n\x08offset_x\x18\n \x01(\r\x12\x10\n\x08offset_y\x18\x0b \x01(\r\x12\x0c\n\x04size\x18\x0c \x01(\r\"\x15\n\x13UploadPictureOutput\"\x14\n\x12\x44\x65leteAccountInput\"\x15\n\x13\x44\x65leteAccountOutput\"\x19\n\x17ResendVerificationInput\"\x1a\n\x18ResendVerificationOutput\":\n\x19\x43ompleteVerificationInput\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\"\x1c\n\x1a\x43ompleteVerificationOutput\"D\n\x12StartRecoveryInput\x12\r\n\x05\x65mail\x18\x01 \x01(\t\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0f\n\x07\x63\x61ptcha\x18\x64 \x01(\t\"#\n\x13StartRecoveryOutput\x12\x0c\n\x04hint\x18\x01 \x01(\t\"G\n\x14\x43ompleteRecoverInput\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\x12\x0f\n\x07subject\x18\x03 \x01(\t\"\x17\n\x15\x43ompleteRecoverOutput2\x91\n\n\x0e\x41\x63\x63ountService\x12}\n\rCreateAccount\x12$.eolymp.community.CreateAccountInput\x1a%.eolymp.community.CreateAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\n\"\x08/account\x12\x83\x01\n\x0f\x44\x65scribeAccount\x12&.eolymp.community.DescribeAccountInput\x1a\'.eolymp.community.DescribeAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\n\x12\x08/account\x12}\n\rUpdateAccount\x12$.eolymp.community.UpdateAccountInput\x1a%.eolymp.community.UpdateAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\n\x1a\x08/account\x12\x85\x01\n\rUploadPicture\x12$.eolymp.community.UploadPictureInput\x1a%.eolymp.community.UploadPictureOutput\"\'\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x12\"\x10/account/picture\x12}\n\rDeleteAccount\x12$.eolymp.community.DeleteAccountInput\x1a%.eolymp.community.DeleteAccountOutput\"\x1f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\n*\x08/account\x12\xa0\x01\n\x12ResendVerification\x12).eolymp.community.ResendVerificationInput\x1a*.eolymp.community.ResendVerificationOutput\"3\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1e\"\x1c/account/verification/resend\x12\xa8\x01\n\x14\x43ompleteVerification\x12+.eolymp.community.CompleteVerificationInput\x1a,.eolymp.community.CompleteVerificationOutput\"5\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x01\x82\xd3\xe4\x93\x02 \"\x1e/account/verification/complete\x12\x8c\x01\n\rStartRecovery\x12$.eolymp.community.StartRecoveryInput\x1a%.eolymp.community.StartRecoveryOutput\".\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x19\"\x17/account/recovery/start\x12\x96\x01\n\x10\x43ompleteRecovery\x12&.eolymp.community.CompleteRecoverInput\x1a\'.eolymp.community.CompleteRecoverOutput\"1\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x1c\"\x1a/account/recovery/completeB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.account_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
@@ -40,48 +39,48 @@
   _ACCOUNTSERVICE.methods_by_name['ResendVerification']._serialized_options = b'\352\342\n\013\365\342\n\000\000\200?\370\342\n\005\202\323\344\223\002\036\"\034/account/verification/resend'
   _ACCOUNTSERVICE.methods_by_name['CompleteVerification']._options = None
   _ACCOUNTSERVICE.methods_by_name['CompleteVerification']._serialized_options = b'\352\342\n\013\365\342\n\000\000\200?\370\342\n\001\202\323\344\223\002 \"\036/account/verification/complete'
   _ACCOUNTSERVICE.methods_by_name['StartRecovery']._options = None
   _ACCOUNTSERVICE.methods_by_name['StartRecovery']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\n2\202\323\344\223\002\031\"\027/account/recovery/start'
   _ACCOUNTSERVICE.methods_by_name['CompleteRecovery']._options = None
   _ACCOUNTSERVICE.methods_by_name['CompleteRecovery']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\n2\202\323\344\223\002\034\"\032/account/recovery/complete'
-  _CREATEACCOUNTINPUT._serialized_start=229
-  _CREATEACCOUNTINPUT._serialized_end=362
-  _CREATEACCOUNTOUTPUT._serialized_start=364
-  _CREATEACCOUNTOUTPUT._serialized_end=399
-  _DESCRIBEACCOUNTINPUT._serialized_start=401
-  _DESCRIBEACCOUNTINPUT._serialized_end=423
-  _DESCRIBEACCOUNTOUTPUT._serialized_start=425
-  _DESCRIBEACCOUNTOUTPUT._serialized_end=544
-  _UPDATEACCOUNTINPUT._serialized_start=547
-  _UPDATEACCOUNTINPUT._serialized_end=1038
-  _UPDATEACCOUNTINPUT_PATCH._serialized_start=751
-  _UPDATEACCOUNTINPUT_PATCH._serialized_end=1038
-  _UPDATEACCOUNTOUTPUT._serialized_start=1040
-  _UPDATEACCOUNTOUTPUT._serialized_end=1075
-  _UPLOADPICTUREINPUT._serialized_start=1077
-  _UPLOADPICTUREINPUT._serialized_end=1179
-  _UPLOADPICTUREOUTPUT._serialized_start=1181
-  _UPLOADPICTUREOUTPUT._serialized_end=1202
-  _DELETEACCOUNTINPUT._serialized_start=1204
-  _DELETEACCOUNTINPUT._serialized_end=1224
-  _DELETEACCOUNTOUTPUT._serialized_start=1226
-  _DELETEACCOUNTOUTPUT._serialized_end=1247
-  _RESENDVERIFICATIONINPUT._serialized_start=1249
-  _RESENDVERIFICATIONINPUT._serialized_end=1274
-  _RESENDVERIFICATIONOUTPUT._serialized_start=1276
-  _RESENDVERIFICATIONOUTPUT._serialized_end=1302
-  _COMPLETEVERIFICATIONINPUT._serialized_start=1304
-  _COMPLETEVERIFICATIONINPUT._serialized_end=1362
-  _COMPLETEVERIFICATIONOUTPUT._serialized_start=1364
-  _COMPLETEVERIFICATIONOUTPUT._serialized_end=1392
-  _STARTRECOVERYINPUT._serialized_start=1394
-  _STARTRECOVERYINPUT._serialized_end=1462
-  _STARTRECOVERYOUTPUT._serialized_start=1464
-  _STARTRECOVERYOUTPUT._serialized_end=1499
-  _COMPLETERECOVERINPUT._serialized_start=1501
-  _COMPLETERECOVERINPUT._serialized_end=1572
-  _COMPLETERECOVEROUTPUT._serialized_start=1574
-  _COMPLETERECOVEROUTPUT._serialized_end=1597
-  _ACCOUNTSERVICE._serialized_start=1600
-  _ACCOUNTSERVICE._serialized_end=2897
+  _CREATEACCOUNTINPUT._serialized_start=198
+  _CREATEACCOUNTINPUT._serialized_end=331
+  _CREATEACCOUNTOUTPUT._serialized_start=333
+  _CREATEACCOUNTOUTPUT._serialized_end=368
+  _DESCRIBEACCOUNTINPUT._serialized_start=370
+  _DESCRIBEACCOUNTINPUT._serialized_end=392
+  _DESCRIBEACCOUNTOUTPUT._serialized_start=394
+  _DESCRIBEACCOUNTOUTPUT._serialized_end=513
+  _UPDATEACCOUNTINPUT._serialized_start=516
+  _UPDATEACCOUNTINPUT._serialized_end=1007
+  _UPDATEACCOUNTINPUT_PATCH._serialized_start=720
+  _UPDATEACCOUNTINPUT_PATCH._serialized_end=1007
+  _UPDATEACCOUNTOUTPUT._serialized_start=1009
+  _UPDATEACCOUNTOUTPUT._serialized_end=1044
+  _UPLOADPICTUREINPUT._serialized_start=1046
+  _UPLOADPICTUREINPUT._serialized_end=1148
+  _UPLOADPICTUREOUTPUT._serialized_start=1150
+  _UPLOADPICTUREOUTPUT._serialized_end=1171
+  _DELETEACCOUNTINPUT._serialized_start=1173
+  _DELETEACCOUNTINPUT._serialized_end=1193
+  _DELETEACCOUNTOUTPUT._serialized_start=1195
+  _DELETEACCOUNTOUTPUT._serialized_end=1216
+  _RESENDVERIFICATIONINPUT._serialized_start=1218
+  _RESENDVERIFICATIONINPUT._serialized_end=1243
+  _RESENDVERIFICATIONOUTPUT._serialized_start=1245
+  _RESENDVERIFICATIONOUTPUT._serialized_end=1271
+  _COMPLETEVERIFICATIONINPUT._serialized_start=1273
+  _COMPLETEVERIFICATIONINPUT._serialized_end=1331
+  _COMPLETEVERIFICATIONOUTPUT._serialized_start=1333
+  _COMPLETEVERIFICATIONOUTPUT._serialized_end=1361
+  _STARTRECOVERYINPUT._serialized_start=1363
+  _STARTRECOVERYINPUT._serialized_end=1431
+  _STARTRECOVERYOUTPUT._serialized_start=1433
+  _STARTRECOVERYOUTPUT._serialized_end=1468
+  _COMPLETERECOVERINPUT._serialized_start=1470
+  _COMPLETERECOVERINPUT._serialized_end=1541
+  _COMPLETERECOVEROUTPUT._serialized_start=1543
+  _COMPLETERECOVEROUTPUT._serialized_end=1566
+  _ACCOUNTSERVICE._serialized_start=1569
+  _ACCOUNTSERVICE._serialized_end=2866
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/account_service_pb2.pyi` & `eolymp-0.8.1/eolymp/community/account_service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.community import attribute_pb2 as _attribute_pb2
-from eolymp.community import member_pb2 as _member_pb2
 from eolymp.community import member_user_pb2 as _member_user_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
```

### Comparing `eolymp-0.8.0/eolymp/community/attribute_pb2.py` & `eolymp-0.8.1/eolymp/community/attribute_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/attribute_pb2.pyi` & `eolymp-0.8.1/eolymp/community/attribute_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/attribute_service_http.py` & `eolymp-0.8.1/eolymp/community/attribute_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/attribute_service_pb2.py` & `eolymp-0.8.1/eolymp/community/attribute_service_pb2.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
-from eolymp.community import configuration_idp_pb2 as eolymp_dot_community_dot_configuration__idp__pb2
-from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(eolymp/community/attribute_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a(eolymp/community/configuration_idp.proto\x1a\x1d\x65olymp/community/member.proto\x1a!eolymp/wellknown/expression.proto\"]\n\x14\x43reateAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\x17\n\x15\x43reateAttributeOutput\"]\n\x14UpdateAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\x17\n\x15UpdateAttributeOutput\"-\n\x14RemoveAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"\x17\n\x15RemoveAttributeOutput\"/\n\x16\x44\x65scribeAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"I\n\x17\x44\x65scribeAttributeOutput\x12.\n\tattribute\x18\x01 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\xee\x02\n\x13ListAttributesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.community.ListAttributesInput.Filter\x1a\xf9\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12-\n\x03key\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x06hidden\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x32\n\x08required\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12.\n\x04type\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"Q\n\x14ListAttributesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.community.Attribute2\x95\x07\n\x10\x41ttributeService\x12\xa7\x01\n\x0f\x43reateAttribute\x12&.eolymp.community.CreateAttributeInput\x1a\'.eolymp.community.CreateAttributeOutput\"C\x82\xe3\n\x1d\x8a\xe3\n\x19\x63ommunity:attribute:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\"\x0b/attributes\x12\xb7\x01\n\x0fUpdateAttribute\x12&.eolymp.community.UpdateAttributeInput\x1a\'.eolymp.community.UpdateAttributeOutput\"S\x82\xe3\n\x1d\x8a\xe3\n\x19\x63ommunity:attribute:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\"\x1b/attributes/{attribute_key}\x12\xb7\x01\n\x0fRemoveAttribute\x12&.eolymp.community.RemoveAttributeInput\x1a\'.eolymp.community.RemoveAttributeOutput\"S\x82\xe3\n\x1d\x8a\xe3\n\x19\x63ommunity:attribute:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d*\x1b/attributes/{attribute_key}\x12\xbc\x01\n\x11\x44\x65scribeAttribute\x12(.eolymp.community.DescribeAttributeInput\x1a).eolymp.community.DescribeAttributeOutput\"R\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ommunity:attribute:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\x12\x1b/attributes/{attribute_key}\x12\xa3\x01\n\x0eListAttributes\x12%.eolymp.community.ListAttributesInput\x1a&.eolymp.community.ListAttributesOutput\"B\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ommunity:attribute:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\x12\x0b/attributesB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n(eolymp/community/attribute_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a!eolymp/wellknown/expression.proto\"]\n\x14\x43reateAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\x17\n\x15\x43reateAttributeOutput\"]\n\x14UpdateAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\x12.\n\tattribute\x18\x02 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\x17\n\x15UpdateAttributeOutput\"-\n\x14RemoveAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"\x17\n\x15RemoveAttributeOutput\"/\n\x16\x44\x65scribeAttributeInput\x12\x15\n\rattribute_key\x18\x01 \x01(\t\"I\n\x17\x44\x65scribeAttributeOutput\x12.\n\tattribute\x18\x01 \x01(\x0b\x32\x1b.eolymp.community.Attribute\"\xee\x02\n\x13ListAttributesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.community.ListAttributesInput.Filter\x1a\xf9\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12-\n\x03key\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x06hidden\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x32\n\x08required\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12.\n\x04type\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"Q\n\x14ListAttributesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.community.Attribute2\x95\x07\n\x10\x41ttributeService\x12\xa7\x01\n\x0f\x43reateAttribute\x12&.eolymp.community.CreateAttributeInput\x1a\'.eolymp.community.CreateAttributeOutput\"C\x82\xe3\n\x1d\x8a\xe3\n\x19\x63ommunity:attribute:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\"\x0b/attributes\x12\xb7\x01\n\x0fUpdateAttribute\x12&.eolymp.community.UpdateAttributeInput\x1a\'.eolymp.community.UpdateAttributeOutput\"S\x82\xe3\n\x1d\x8a\xe3\n\x19\x63ommunity:attribute:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\"\x1b/attributes/{attribute_key}\x12\xb7\x01\n\x0fRemoveAttribute\x12&.eolymp.community.RemoveAttributeInput\x1a\'.eolymp.community.RemoveAttributeOutput\"S\x82\xe3\n\x1d\x8a\xe3\n\x19\x63ommunity:attribute:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d*\x1b/attributes/{attribute_key}\x12\xbc\x01\n\x11\x44\x65scribeAttribute\x12(.eolymp.community.DescribeAttributeInput\x1a).eolymp.community.DescribeAttributeOutput\"R\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ommunity:attribute:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1d\x12\x1b/attributes/{attribute_key}\x12\xa3\x01\n\x0eListAttributes\x12%.eolymp.community.ListAttributesInput\x1a&.eolymp.community.ListAttributesOutput\"B\x82\xe3\n\x1c\x8a\xe3\n\x18\x63ommunity:attribute:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\r\x12\x0b/attributesB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.attribute_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
@@ -34,32 +32,32 @@
   _ATTRIBUTESERVICE.methods_by_name['UpdateAttribute']._serialized_options = b'\202\343\n\035\212\343\n\031community:attribute:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\035\"\033/attributes/{attribute_key}'
   _ATTRIBUTESERVICE.methods_by_name['RemoveAttribute']._options = None
   _ATTRIBUTESERVICE.methods_by_name['RemoveAttribute']._serialized_options = b'\202\343\n\035\212\343\n\031community:attribute:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\035*\033/attributes/{attribute_key}'
   _ATTRIBUTESERVICE.methods_by_name['DescribeAttribute']._options = None
   _ATTRIBUTESERVICE.methods_by_name['DescribeAttribute']._serialized_options = b'\202\343\n\034\212\343\n\030community:attribute:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\035\022\033/attributes/{attribute_key}'
   _ATTRIBUTESERVICE.methods_by_name['ListAttributes']._options = None
   _ATTRIBUTESERVICE.methods_by_name['ListAttributes']._serialized_options = b'\202\343\n\034\212\343\n\030community:attribute:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\r\022\013/attributes'
-  _CREATEATTRIBUTEINPUT._serialized_start=303
-  _CREATEATTRIBUTEINPUT._serialized_end=396
-  _CREATEATTRIBUTEOUTPUT._serialized_start=398
-  _CREATEATTRIBUTEOUTPUT._serialized_end=421
-  _UPDATEATTRIBUTEINPUT._serialized_start=423
-  _UPDATEATTRIBUTEINPUT._serialized_end=516
-  _UPDATEATTRIBUTEOUTPUT._serialized_start=518
-  _UPDATEATTRIBUTEOUTPUT._serialized_end=541
-  _REMOVEATTRIBUTEINPUT._serialized_start=543
-  _REMOVEATTRIBUTEINPUT._serialized_end=588
-  _REMOVEATTRIBUTEOUTPUT._serialized_start=590
-  _REMOVEATTRIBUTEOUTPUT._serialized_end=613
-  _DESCRIBEATTRIBUTEINPUT._serialized_start=615
-  _DESCRIBEATTRIBUTEINPUT._serialized_end=662
-  _DESCRIBEATTRIBUTEOUTPUT._serialized_start=664
-  _DESCRIBEATTRIBUTEOUTPUT._serialized_end=737
-  _LISTATTRIBUTESINPUT._serialized_start=740
-  _LISTATTRIBUTESINPUT._serialized_end=1106
-  _LISTATTRIBUTESINPUT_FILTER._serialized_start=857
-  _LISTATTRIBUTESINPUT_FILTER._serialized_end=1106
-  _LISTATTRIBUTESOUTPUT._serialized_start=1108
-  _LISTATTRIBUTESOUTPUT._serialized_end=1189
-  _ATTRIBUTESERVICE._serialized_start=1192
-  _ATTRIBUTESERVICE._serialized_end=2109
+  _CREATEATTRIBUTEINPUT._serialized_start=230
+  _CREATEATTRIBUTEINPUT._serialized_end=323
+  _CREATEATTRIBUTEOUTPUT._serialized_start=325
+  _CREATEATTRIBUTEOUTPUT._serialized_end=348
+  _UPDATEATTRIBUTEINPUT._serialized_start=350
+  _UPDATEATTRIBUTEINPUT._serialized_end=443
+  _UPDATEATTRIBUTEOUTPUT._serialized_start=445
+  _UPDATEATTRIBUTEOUTPUT._serialized_end=468
+  _REMOVEATTRIBUTEINPUT._serialized_start=470
+  _REMOVEATTRIBUTEINPUT._serialized_end=515
+  _REMOVEATTRIBUTEOUTPUT._serialized_start=517
+  _REMOVEATTRIBUTEOUTPUT._serialized_end=540
+  _DESCRIBEATTRIBUTEINPUT._serialized_start=542
+  _DESCRIBEATTRIBUTEINPUT._serialized_end=589
+  _DESCRIBEATTRIBUTEOUTPUT._serialized_start=591
+  _DESCRIBEATTRIBUTEOUTPUT._serialized_end=664
+  _LISTATTRIBUTESINPUT._serialized_start=667
+  _LISTATTRIBUTESINPUT._serialized_end=1033
+  _LISTATTRIBUTESINPUT_FILTER._serialized_start=784
+  _LISTATTRIBUTESINPUT_FILTER._serialized_end=1033
+  _LISTATTRIBUTESOUTPUT._serialized_start=1035
+  _LISTATTRIBUTESOUTPUT._serialized_end=1116
+  _ATTRIBUTESERVICE._serialized_start=1119
+  _ATTRIBUTESERVICE._serialized_end=2036
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/attribute_service_pb2.pyi` & `eolymp-0.8.1/eolymp/community/attribute_service_pb2.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.community import attribute_pb2 as _attribute_pb2
-from eolymp.community import configuration_idp_pb2 as _configuration_idp_pb2
-from eolymp.community import member_pb2 as _member_pb2
 from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `eolymp-0.8.0/eolymp/community/configuration_idp_pb2.py` & `eolymp-0.8.1/eolymp/community/configuration_idp_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/configuration_idp_pb2.pyi` & `eolymp-0.8.1/eolymp/community/configuration_idp_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/configuration_service_http.py` & `eolymp-0.8.1/eolymp/community/configuration_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/configuration_service_pb2.py` & `eolymp-0.8.1/eolymp/community/configuration_service_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,36 +10,33 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
-from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
 from eolymp.community import configuration_idp_pb2 as eolymp_dot_community_dot_configuration__idp__pb2
-from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
-from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,eolymp/community/configuration_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a(eolymp/community/configuration_idp.proto\x1a\x1d\x65olymp/community/member.proto\x1a!eolymp/wellknown/expression.proto\"\x1f\n\x1d\x44\x65scribeIdentityProviderInput\"v\n\x1e\x44\x65scribeIdentityProviderOutput\x12\x0f\n\x05local\x18\x01 \x01(\x08H\x00\x12\x37\n\x04oidc\x18\x03 \x01(\x0b\x32\'.eolymp.community.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"v\n\x1e\x43onfigureIdentityProviderInput\x12\x0f\n\x05local\x18\x01 \x01(\x08H\x00\x12\x37\n\x04oidc\x18\x03 \x01(\x0b\x32\'.eolymp.community.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"!\n\x1f\x43onfigureIdentityProviderOutput2\xf1\x02\n\x14\x43onfigurationService\x12\x9a\x01\n\x18\x44\x65scribeIdentityProvider\x12/.eolymp.community.DescribeIdentityProviderInput\x1a\x30.eolymp.community.DescribeIdentityProviderOutput\"\x1b\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x06\x12\x04/idp\x12\xbb\x01\n\x19\x43onfigureIdentityProvider\x12\x30.eolymp.community.ConfigureIdentityProviderInput\x1a\x31.eolymp.community.ConfigureIdentityProviderOutput\"9\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x06\x1a\x04/idpB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n,eolymp/community/configuration_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a(eolymp/community/configuration_idp.proto\"\x1f\n\x1d\x44\x65scribeIdentityProviderInput\"v\n\x1e\x44\x65scribeIdentityProviderOutput\x12\x0f\n\x05local\x18\x01 \x01(\x08H\x00\x12\x37\n\x04oidc\x18\x03 \x01(\x0b\x32\'.eolymp.community.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"v\n\x1e\x43onfigureIdentityProviderInput\x12\x0f\n\x05local\x18\x01 \x01(\x08H\x00\x12\x37\n\x04oidc\x18\x03 \x01(\x0b\x32\'.eolymp.community.IdentityProvider.OIDCH\x00\x42\n\n\x08provider\"!\n\x1f\x43onfigureIdentityProviderOutput2\xf1\x02\n\x14\x43onfigurationService\x12\x9a\x01\n\x18\x44\x65scribeIdentityProvider\x12/.eolymp.community.DescribeIdentityProviderInput\x1a\x30.eolymp.community.DescribeIdentityProviderOutput\"\x1b\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x06\x12\x04/idp\x12\xbb\x01\n\x19\x43onfigureIdentityProvider\x12\x30.eolymp.community.ConfigureIdentityProviderInput\x1a\x31.eolymp.community.ConfigureIdentityProviderOutput\"9\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x06\x1a\x04/idpB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.configuration_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
   _CONFIGURATIONSERVICE.methods_by_name['DescribeIdentityProvider']._options = None
   _CONFIGURATIONSERVICE.methods_by_name['DescribeIdentityProvider']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\nd\202\323\344\223\002\006\022\004/idp'
   _CONFIGURATIONSERVICE.methods_by_name['ConfigureIdentityProvider']._options = None
   _CONFIGURATIONSERVICE.methods_by_name['ConfigureIdentityProvider']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\200?\370\342\n\005\202\323\344\223\002\006\032\004/idp'
-  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_start=307
-  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_end=338
-  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_start=340
-  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_end=458
-  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_start=460
-  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_end=578
-  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_start=580
-  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_end=613
-  _CONFIGURATIONSERVICE._serialized_start=616
-  _CONFIGURATIONSERVICE._serialized_end=985
+  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_start=207
+  _DESCRIBEIDENTITYPROVIDERINPUT._serialized_end=238
+  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_start=240
+  _DESCRIBEIDENTITYPROVIDEROUTPUT._serialized_end=358
+  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_start=360
+  _CONFIGUREIDENTITYPROVIDERINPUT._serialized_end=478
+  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_start=480
+  _CONFIGUREIDENTITYPROVIDEROUTPUT._serialized_end=513
+  _CONFIGURATIONSERVICE._serialized_start=516
+  _CONFIGURATIONSERVICE._serialized_end=885
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/configuration_service_pb2.pyi` & `eolymp-0.8.1/eolymp/community/configuration_service_pb2.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
-from eolymp.community import attribute_pb2 as _attribute_pb2
 from eolymp.community import configuration_idp_pb2 as _configuration_idp_pb2
-from eolymp.community import member_pb2 as _member_pb2
-from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class ConfigureIdentityProviderInput(_message.Message):
```

### Comparing `eolymp-0.8.0/eolymp/community/events_pb2.py` & `eolymp-0.8.1/eolymp/community/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/events_pb2.pyi` & `eolymp-0.8.1/eolymp/community/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/member_ghost_pb2.py` & `eolymp-0.8.1/eolymp/community/member_ghost_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/member_pb2.py` & `eolymp-0.8.1/eolymp/community/member_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/member_pb2.pyi` & `eolymp-0.8.1/eolymp/community/member_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/member_service_http.py` & `eolymp-0.8.1/eolymp/community/member_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/member_service_pb2.py` & `eolymp-0.8.1/eolymp/community/member_service_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,22 +10,20 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
-from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
-from eolymp.community import configuration_idp_pb2 as eolymp_dot_community_dot_configuration__idp__pb2
 from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
 from eolymp.wellknown import direction_pb2 as eolymp_dot_wellknown_dot_direction__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%eolymp/community/member_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a(eolymp/community/configuration_idp.proto\x1a\x1d\x65olymp/community/member.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"=\n\x11\x43reateMemberInput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\'\n\x12\x43reateMemberOutput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"\xf6\x03\n\x11UpdateMemberInput\x12\x38\n\x05patch\x18\x01 \x03(\x0e\x32).eolymp.community.UpdateMemberInput.Patch\x12\x11\n\tmember_id\x18\x02 \x01(\t\x12(\n\x06member\x18\x03 \x01(\x0b\x32\x18.eolymp.community.Member\"\xe9\x02\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0e\n\nUNOFFICIAL\x10\x02\x12\x0b\n\x07\x41\x43\x43OUNT\x10\x64\x12\x11\n\rUSER_NICKNAME\x10\x65\x12\x0e\n\nUSER_EMAIL\x10\x66\x12\x11\n\rUSER_PASSWORD\x10g\x12\r\n\tUSER_NAME\x10h\x12\x10\n\x0cUSER_PICTURE\x10i\x12\x11\n\rUSER_BIRTHDAY\x10j\x12\x10\n\x0cUSER_COUNTRY\x10k\x12\r\n\tUSER_CITY\x10l\x12\x14\n\x10USER_PREFERENCES\x10m\x12\x1c\n\x17USER_PREFERENCES_LOCALE\x10\xbe\x01\x12\x1e\n\x19USER_PREFERENCES_TIMEZONE\x10\xbf\x01\x12\x1d\n\x18USER_PREFERENCES_RUNTIME\x10\xc0\x01\x12\x0e\n\tTEAM_NAME\x10\xc8\x01\x12\x0f\n\nGHOST_NAME\x10\xac\x02\x12\x0f\n\nATTRIBUTES\x10\x84\x07\"\x14\n\x12UpdateMemberOutput\"<\n\x11\x44\x65leteMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\x12\x14\n\x0c\x66orce_delete\x18\x02 \x01(\x08\"\x14\n\x12\x44\x65leteMemberOutput\"\'\n\x12RestoreMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"\x15\n\x13RestoreMemberOutput\"(\n\x13\x44\x65scribeMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"@\n\x14\x44\x65scribeMemberOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\xe2\x06\n\x10ListMembersInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12:\n\x07\x66ilters\x18( \x01(\x0b\x32).eolymp.community.ListMembersInput.Filter\x12\x39\n\x04sort\x18\x32 \x01(\x0e\x32+.eolymp.community.ListMembersInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\xcb\x04\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12.\n\x04type\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x34\n\x08nickname\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x30\n\x06\x61\x63tive\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nregistered\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nunofficial\x18\x06 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12/\n\x07team_id\x18\x07 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x37\n\x0buser_issuer\x18\x65 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x38\n\x0cuser_subject\x18\x66 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x36\n\nuser_email\x18g \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x35\n\tuser_name\x18h \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\"?\n\x08Sortable\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x0c\n\x08NICKNAME\x10\x01\x12\x0e\n\nCREATED_AT\x10\x02\x12\x08\n\x04TYPE\x10\x03\"K\n\x11ListMembersOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\'\n\x05items\x18\x02 \x03(\x0b\x32\x18.eolymp.community.Member\"7\n\x11\x41ssignMemberInput\x12\x0f\n\x07team_id\x18\x01 \x01(\t\x12\x11\n\tmember_id\x18\x02 \x01(\t\"\x14\n\x12\x41ssignMemberOutput\"9\n\x13UnassignMemberInput\x12\x0f\n\x07team_id\x18\x01 \x01(\t\x12\x11\n\tmember_id\x18\x02 \x01(\t\"\x16\n\x14UnassignMemberOutput2\xe1\n\n\rMemberService\x12\x98\x01\n\x0c\x43reateMember\x12#.eolymp.community.CreateMemberInput\x1a$.eolymp.community.CreateMemberOutput\"=\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\"\x08/members\x12\xa4\x01\n\x0cUpdateMember\x12#.eolymp.community.UpdateMemberInput\x1a$.eolymp.community.UpdateMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\"\x14/members/{member_id}\x12\xa4\x01\n\x0c\x44\x65leteMember\x12#.eolymp.community.DeleteMemberInput\x1a$.eolymp.community.DeleteMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16*\x14/members/{member_id}\x12\xaf\x01\n\rRestoreMember\x12$.eolymp.community.RestoreMemberInput\x1a%.eolymp.community.RestoreMemberOutput\"Q\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1e\"\x1c/members/{member_id}/restore\x12\xa9\x01\n\x0e\x44\x65scribeMember\x12%.eolymp.community.DescribeMemberInput\x1a&.eolymp.community.DescribeMemberOutput\"H\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\x12\x14/members/{member_id}\x12\x94\x01\n\x0bListMembers\x12\".eolymp.community.ListMembersInput\x1a#.eolymp.community.ListMembersOutput\"<\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\x12\x08/members\x12\xb4\x01\n\x0c\x41ssignMember\x12#.eolymp.community.AssignMemberInput\x1a$.eolymp.community.AssignMemberOutput\"Y\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02&\x1a$/members/{team_id}/users/{member_id}\x12\xba\x01\n\x0eUnassignMember\x12%.eolymp.community.UnassignMemberInput\x1a&.eolymp.community.UnassignMemberOutput\"Y\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02&*$/members/{team_id}/users/{member_id}B5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n%eolymp/community/member_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1d\x65olymp/community/member.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"=\n\x11\x43reateMemberInput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\'\n\x12\x43reateMemberOutput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"\xf6\x03\n\x11UpdateMemberInput\x12\x38\n\x05patch\x18\x01 \x03(\x0e\x32).eolymp.community.UpdateMemberInput.Patch\x12\x11\n\tmember_id\x18\x02 \x01(\t\x12(\n\x06member\x18\x03 \x01(\x0b\x32\x18.eolymp.community.Member\"\xe9\x02\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0e\n\nUNOFFICIAL\x10\x02\x12\x0b\n\x07\x41\x43\x43OUNT\x10\x64\x12\x11\n\rUSER_NICKNAME\x10\x65\x12\x0e\n\nUSER_EMAIL\x10\x66\x12\x11\n\rUSER_PASSWORD\x10g\x12\r\n\tUSER_NAME\x10h\x12\x10\n\x0cUSER_PICTURE\x10i\x12\x11\n\rUSER_BIRTHDAY\x10j\x12\x10\n\x0cUSER_COUNTRY\x10k\x12\r\n\tUSER_CITY\x10l\x12\x14\n\x10USER_PREFERENCES\x10m\x12\x1c\n\x17USER_PREFERENCES_LOCALE\x10\xbe\x01\x12\x1e\n\x19USER_PREFERENCES_TIMEZONE\x10\xbf\x01\x12\x1d\n\x18USER_PREFERENCES_RUNTIME\x10\xc0\x01\x12\x0e\n\tTEAM_NAME\x10\xc8\x01\x12\x0f\n\nGHOST_NAME\x10\xac\x02\x12\x0f\n\nATTRIBUTES\x10\x84\x07\"\x14\n\x12UpdateMemberOutput\"<\n\x11\x44\x65leteMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\x12\x14\n\x0c\x66orce_delete\x18\x02 \x01(\x08\"\x14\n\x12\x44\x65leteMemberOutput\"\'\n\x12RestoreMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"\x15\n\x13RestoreMemberOutput\"(\n\x13\x44\x65scribeMemberInput\x12\x11\n\tmember_id\x18\x01 \x01(\t\"@\n\x14\x44\x65scribeMemberOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"\xda\x06\n\x10ListMembersInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12:\n\x07\x66ilters\x18( \x01(\x0b\x32).eolymp.community.ListMembersInput.Filter\x12\x39\n\x04sort\x18\x32 \x01(\x0e\x32+.eolymp.community.ListMembersInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\xc7\x04\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12.\n\x04type\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x30\n\x06\x61\x63tive\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nincomplete\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nunofficial\x18\x06 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12/\n\x07team_id\x18\x07 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x37\n\x0buser_issuer\x18\x65 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x38\n\x0cuser_subject\x18\x66 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x36\n\nuser_email\x18g \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x35\n\tuser_name\x18h \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\";\n\x08Sortable\x12\x0b\n\x07\x44\x45\x46\x41ULT\x10\x00\x12\x08\n\x04NAME\x10\x01\x12\x0e\n\nCREATED_AT\x10\x02\x12\x08\n\x04TYPE\x10\x03\"K\n\x11ListMembersOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\'\n\x05items\x18\x02 \x03(\x0b\x32\x18.eolymp.community.Member\"7\n\x11\x41ssignMemberInput\x12\x0f\n\x07team_id\x18\x01 \x01(\t\x12\x11\n\tmember_id\x18\x02 \x01(\t\"\x14\n\x12\x41ssignMemberOutput\"9\n\x13UnassignMemberInput\x12\x0f\n\x07team_id\x18\x01 \x01(\t\x12\x11\n\tmember_id\x18\x02 \x01(\t\"\x16\n\x14UnassignMemberOutput2\xe1\n\n\rMemberService\x12\x98\x01\n\x0c\x43reateMember\x12#.eolymp.community.CreateMemberInput\x1a$.eolymp.community.CreateMemberOutput\"=\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\"\x08/members\x12\xa4\x01\n\x0cUpdateMember\x12#.eolymp.community.UpdateMemberInput\x1a$.eolymp.community.UpdateMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\"\x14/members/{member_id}\x12\xa4\x01\n\x0c\x44\x65leteMember\x12#.eolymp.community.DeleteMemberInput\x1a$.eolymp.community.DeleteMemberOutput\"I\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16*\x14/members/{member_id}\x12\xaf\x01\n\rRestoreMember\x12$.eolymp.community.RestoreMemberInput\x1a%.eolymp.community.RestoreMemberOutput\"Q\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1e\"\x1c/members/{member_id}/restore\x12\xa9\x01\n\x0e\x44\x65scribeMember\x12%.eolymp.community.DescribeMemberInput\x1a&.eolymp.community.DescribeMemberOutput\"H\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x16\x12\x14/members/{member_id}\x12\x94\x01\n\x0bListMembers\x12\".eolymp.community.ListMembersInput\x1a#.eolymp.community.ListMembersOutput\"<\x82\xe3\n\x19\x8a\xe3\n\x15\x63ommunity:member:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\x12\x08/members\x12\xb4\x01\n\x0c\x41ssignMember\x12#.eolymp.community.AssignMemberInput\x1a$.eolymp.community.AssignMemberOutput\"Y\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02&\x1a$/members/{team_id}/users/{member_id}\x12\xba\x01\n\x0eUnassignMember\x12%.eolymp.community.UnassignMemberInput\x1a&.eolymp.community.UnassignMemberOutput\"Y\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02&*$/members/{team_id}/users/{member_id}B5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.member_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
@@ -41,48 +39,48 @@
   _MEMBERSERVICE.methods_by_name['DescribeMember']._serialized_options = b'\202\343\n\031\212\343\n\025community:member:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\026\022\024/members/{member_id}'
   _MEMBERSERVICE.methods_by_name['ListMembers']._options = None
   _MEMBERSERVICE.methods_by_name['ListMembers']._serialized_options = b'\202\343\n\031\212\343\n\025community:member:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\n\022\010/members'
   _MEMBERSERVICE.methods_by_name['AssignMember']._options = None
   _MEMBERSERVICE.methods_by_name['AssignMember']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002&\032$/members/{team_id}/users/{member_id}'
   _MEMBERSERVICE.methods_by_name['UnassignMember']._options = None
   _MEMBERSERVICE.methods_by_name['UnassignMember']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002&*$/members/{team_id}/users/{member_id}'
-  _CREATEMEMBERINPUT._serialized_start=334
-  _CREATEMEMBERINPUT._serialized_end=395
-  _CREATEMEMBEROUTPUT._serialized_start=397
-  _CREATEMEMBEROUTPUT._serialized_end=436
-  _UPDATEMEMBERINPUT._serialized_start=439
-  _UPDATEMEMBERINPUT._serialized_end=941
-  _UPDATEMEMBERINPUT_PATCH._serialized_start=580
-  _UPDATEMEMBERINPUT_PATCH._serialized_end=941
-  _UPDATEMEMBEROUTPUT._serialized_start=943
-  _UPDATEMEMBEROUTPUT._serialized_end=963
-  _DELETEMEMBERINPUT._serialized_start=965
-  _DELETEMEMBERINPUT._serialized_end=1025
-  _DELETEMEMBEROUTPUT._serialized_start=1027
-  _DELETEMEMBEROUTPUT._serialized_end=1047
-  _RESTOREMEMBERINPUT._serialized_start=1049
-  _RESTOREMEMBERINPUT._serialized_end=1088
-  _RESTOREMEMBEROUTPUT._serialized_start=1090
-  _RESTOREMEMBEROUTPUT._serialized_end=1111
-  _DESCRIBEMEMBERINPUT._serialized_start=1113
-  _DESCRIBEMEMBERINPUT._serialized_end=1153
-  _DESCRIBEMEMBEROUTPUT._serialized_start=1155
-  _DESCRIBEMEMBEROUTPUT._serialized_end=1219
-  _LISTMEMBERSINPUT._serialized_start=1222
-  _LISTMEMBERSINPUT._serialized_end=2088
-  _LISTMEMBERSINPUT_FILTER._serialized_start=1436
-  _LISTMEMBERSINPUT_FILTER._serialized_end=2023
-  _LISTMEMBERSINPUT_SORTABLE._serialized_start=2025
-  _LISTMEMBERSINPUT_SORTABLE._serialized_end=2088
-  _LISTMEMBERSOUTPUT._serialized_start=2090
-  _LISTMEMBERSOUTPUT._serialized_end=2165
-  _ASSIGNMEMBERINPUT._serialized_start=2167
-  _ASSIGNMEMBERINPUT._serialized_end=2222
-  _ASSIGNMEMBEROUTPUT._serialized_start=2224
-  _ASSIGNMEMBEROUTPUT._serialized_end=2244
-  _UNASSIGNMEMBERINPUT._serialized_start=2246
-  _UNASSIGNMEMBERINPUT._serialized_end=2303
-  _UNASSIGNMEMBEROUTPUT._serialized_start=2305
-  _UNASSIGNMEMBEROUTPUT._serialized_end=2327
-  _MEMBERSERVICE._serialized_start=2330
-  _MEMBERSERVICE._serialized_end=3707
+  _CREATEMEMBERINPUT._serialized_start=258
+  _CREATEMEMBERINPUT._serialized_end=319
+  _CREATEMEMBEROUTPUT._serialized_start=321
+  _CREATEMEMBEROUTPUT._serialized_end=360
+  _UPDATEMEMBERINPUT._serialized_start=363
+  _UPDATEMEMBERINPUT._serialized_end=865
+  _UPDATEMEMBERINPUT_PATCH._serialized_start=504
+  _UPDATEMEMBERINPUT_PATCH._serialized_end=865
+  _UPDATEMEMBEROUTPUT._serialized_start=867
+  _UPDATEMEMBEROUTPUT._serialized_end=887
+  _DELETEMEMBERINPUT._serialized_start=889
+  _DELETEMEMBERINPUT._serialized_end=949
+  _DELETEMEMBEROUTPUT._serialized_start=951
+  _DELETEMEMBEROUTPUT._serialized_end=971
+  _RESTOREMEMBERINPUT._serialized_start=973
+  _RESTOREMEMBERINPUT._serialized_end=1012
+  _RESTOREMEMBEROUTPUT._serialized_start=1014
+  _RESTOREMEMBEROUTPUT._serialized_end=1035
+  _DESCRIBEMEMBERINPUT._serialized_start=1037
+  _DESCRIBEMEMBERINPUT._serialized_end=1077
+  _DESCRIBEMEMBEROUTPUT._serialized_start=1079
+  _DESCRIBEMEMBEROUTPUT._serialized_end=1143
+  _LISTMEMBERSINPUT._serialized_start=1146
+  _LISTMEMBERSINPUT._serialized_end=2004
+  _LISTMEMBERSINPUT_FILTER._serialized_start=1360
+  _LISTMEMBERSINPUT_FILTER._serialized_end=1943
+  _LISTMEMBERSINPUT_SORTABLE._serialized_start=1945
+  _LISTMEMBERSINPUT_SORTABLE._serialized_end=2004
+  _LISTMEMBERSOUTPUT._serialized_start=2006
+  _LISTMEMBERSOUTPUT._serialized_end=2081
+  _ASSIGNMEMBERINPUT._serialized_start=2083
+  _ASSIGNMEMBERINPUT._serialized_end=2138
+  _ASSIGNMEMBEROUTPUT._serialized_start=2140
+  _ASSIGNMEMBEROUTPUT._serialized_end=2160
+  _UNASSIGNMEMBERINPUT._serialized_start=2162
+  _UNASSIGNMEMBERINPUT._serialized_end=2219
+  _UNASSIGNMEMBEROUTPUT._serialized_start=2221
+  _UNASSIGNMEMBEROUTPUT._serialized_end=2243
+  _MEMBERSERVICE._serialized_start=2246
+  _MEMBERSERVICE._serialized_end=3623
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/member_service_pb2.pyi` & `eolymp-0.8.1/eolymp/community/member_service_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
-from eolymp.community import attribute_pb2 as _attribute_pb2
-from eolymp.community import configuration_idp_pb2 as _configuration_idp_pb2
 from eolymp.community import member_pb2 as _member_pb2
 from eolymp.wellknown import direction_pb2 as _direction_pb2
 from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
@@ -63,42 +61,42 @@
     def __init__(self, member: _Optional[_Union[_member_pb2.Member, _Mapping]] = ...) -> None: ...
 
 class ListMembersInput(_message.Message):
     __slots__ = ["filters", "offset", "order", "size", "sort"]
     class Sortable(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Filter(_message.Message):
-        __slots__ = ["active", "id", "nickname", "registered", "team_id", "type", "unofficial", "user_email", "user_issuer", "user_name", "user_subject"]
+        __slots__ = ["active", "id", "incomplete", "name", "team_id", "type", "unofficial", "user_email", "user_issuer", "user_name", "user_subject"]
         ACTIVE_FIELD_NUMBER: _ClassVar[int]
         ID_FIELD_NUMBER: _ClassVar[int]
-        NICKNAME_FIELD_NUMBER: _ClassVar[int]
-        REGISTERED_FIELD_NUMBER: _ClassVar[int]
+        INCOMPLETE_FIELD_NUMBER: _ClassVar[int]
+        NAME_FIELD_NUMBER: _ClassVar[int]
         TEAM_ID_FIELD_NUMBER: _ClassVar[int]
         TYPE_FIELD_NUMBER: _ClassVar[int]
         UNOFFICIAL_FIELD_NUMBER: _ClassVar[int]
         USER_EMAIL_FIELD_NUMBER: _ClassVar[int]
         USER_ISSUER_FIELD_NUMBER: _ClassVar[int]
         USER_NAME_FIELD_NUMBER: _ClassVar[int]
         USER_SUBJECT_FIELD_NUMBER: _ClassVar[int]
         active: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionBool]
         id: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionID]
-        nickname: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
-        registered: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionBool]
+        incomplete: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionBool]
+        name: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
         team_id: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionID]
         type: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionEnum]
         unofficial: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionBool]
         user_email: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
         user_issuer: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
         user_name: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
         user_subject: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
-        def __init__(self, id: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., type: _Optional[_Iterable[_Union[_expression_pb2.ExpressionEnum, _Mapping]]] = ..., nickname: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., active: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., registered: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., unofficial: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., team_id: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., user_issuer: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., user_subject: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., user_email: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., user_name: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ...) -> None: ...
+        def __init__(self, id: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., type: _Optional[_Iterable[_Union[_expression_pb2.ExpressionEnum, _Mapping]]] = ..., name: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., active: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., incomplete: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., unofficial: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., team_id: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., user_issuer: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., user_subject: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., user_email: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., user_name: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ...) -> None: ...
     CREATED_AT: ListMembersInput.Sortable
     DEFAULT: ListMembersInput.Sortable
     FILTERS_FIELD_NUMBER: _ClassVar[int]
-    NICKNAME: ListMembersInput.Sortable
+    NAME: ListMembersInput.Sortable
     OFFSET_FIELD_NUMBER: _ClassVar[int]
     ORDER_FIELD_NUMBER: _ClassVar[int]
     SIZE_FIELD_NUMBER: _ClassVar[int]
     SORT_FIELD_NUMBER: _ClassVar[int]
     TYPE: ListMembersInput.Sortable
     filters: ListMembersInput.Filter
     offset: int
```

### Comparing `eolymp-0.8.0/eolymp/community/member_team_pb2.py` & `eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/community/member_team.proto
+# source: eolymp/helpdesk/auto_reply.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.community import member_user_pb2 as eolymp_dot_community_dot_member__user__pb2
+from eolymp.ecm import content_pb2 as eolymp_dot_ecm_dot_content__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/community/member_team.proto\x12\x10\x65olymp.community\x1a\"eolymp/community/member_user.proto\"%\n\x04Team\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0f\n\x07staffed\x18\x02 \x01(\x08\x42\x35Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/helpdesk/auto_reply.proto\x12\x0f\x65olymp.helpdesk\x1a\x18\x65olymp/ecm/content.proto\"k\n\tAutoReply\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x14 \x01(\t\x12$\n\x07message\x18\x15 \x01(\x0b\x32\x13.eolymp.ecm.Content\x12\x0e\n\x06labels\x18\x16 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdeskb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.member_team_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.helpdesk.auto_reply_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
-  _TEAM._serialized_start=92
-  _TEAM._serialized_end=129
+  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdesk'
+  _AUTOREPLY._serialized_start=79
+  _AUTOREPLY._serialized_end=186
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/member_team_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/language_pb2.pyi`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,15 @@
-from eolymp.community import member_user_pb2 as _member_user_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Team(_message.Message):
-    __slots__ = ["name", "staffed"]
+class Language(_message.Message):
+    __slots__ = ["deprecated", "id", "name"]
+    DEPRECATED_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
-    STAFFED_FIELD_NUMBER: _ClassVar[int]
+    deprecated: bool
+    id: str
     name: str
-    staffed: bool
-    def __init__(self, name: _Optional[str] = ..., staffed: bool = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., deprecated: bool = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/community/member_user_pb2.py` & `eolymp-0.8.1/eolymp/community/member_user_pb2.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,23 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/community/member_user.proto\x12\x10\x65olymp.community\x1a eolymp/community/attribute.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\x91\x03\n\x04User\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x10\n\x08nickname\x18\n \x01(\t\x12\x1f\n\x17nickname_change_timeout\x18\x0b \x01(\r\x12\r\n\x05\x65mail\x18\x14 \x01(\t\x12\x16\n\x0e\x65mail_verified\x18\x15 \x01(\x08\x12\x10\n\x08password\x18\x1e \x01(\t\x12\x14\n\x0cpassword_age\x18\x1f \x01(\r\x12\x0c\n\x04name\x18( \x01(\t\x12\x0f\n\x07picture\x18\x32 \x01(\t\x12,\n\x08\x62irthday\x18< \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x63ountry\x18\x46 \x01(\t\x12\x0c\n\x04\x63ity\x18I \x01(\t\x12\x38\n\x0bpreferences\x18\xa0\x06 \x01(\x0b\x32\".eolymp.community.User.Preferences\x1a@\n\x0bPreferences\x12\x0e\n\x06locale\x18\x01 \x01(\t\x12\x10\n\x08timezone\x18\x02 \x01(\t\x12\x0f\n\x07runtime\x18\n \x01(\tB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\"eolymp/community/member_user.proto\x12\x10\x65olymp.community\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa2\x03\n\x04User\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x10\n\x08nickname\x18\n \x01(\t\x12\x1f\n\x17nickname_change_timeout\x18\x0b \x01(\r\x12\r\n\x05\x65mail\x18\x14 \x01(\t\x12\x16\n\x0e\x65mail_verified\x18\x15 \x01(\x08\x12\x10\n\x08password\x18\x1e \x01(\t\x12\x14\n\x0cpassword_age\x18\x1f \x01(\r\x12\x0c\n\x04name\x18( \x01(\t\x12\x0f\n\x07picture\x18\x32 \x01(\t\x12,\n\x08\x62irthday\x18< \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07\x63ountry\x18\x46 \x01(\t\x12\x0c\n\x04\x63ity\x18I \x01(\t\x12\x0f\n\x07team_id\x18\x64 \x01(\t\x12\x38\n\x0bpreferences\x18\xa0\x06 \x01(\x0b\x32\".eolymp.community.User.Preferences\x1a@\n\x0bPreferences\x12\x0e\n\x06locale\x18\x01 \x01(\t\x12\x10\n\x08timezone\x18\x02 \x01(\t\x12\x0f\n\x07runtime\x18\n \x01(\tB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.member_user_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
-  _USER._serialized_start=124
-  _USER._serialized_end=525
-  _USER_PREFERENCES._serialized_start=461
-  _USER_PREFERENCES._serialized_end=525
+  _USER._serialized_start=90
+  _USER._serialized_end=508
+  _USER_PREFERENCES._serialized_start=444
+  _USER_PREFERENCES._serialized_end=508
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/member_user_pb2.pyi` & `eolymp-0.8.1/eolymp/community/member_user_pb2.pyi`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-from eolymp.community import attribute_pb2 as _attribute_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class User(_message.Message):
-    __slots__ = ["birthday", "city", "country", "email", "email_verified", "issuer", "name", "nickname", "nickname_change_timeout", "password", "password_age", "picture", "preferences", "subject"]
+    __slots__ = ["birthday", "city", "country", "email", "email_verified", "issuer", "name", "nickname", "nickname_change_timeout", "password", "password_age", "picture", "preferences", "subject", "team_id"]
     class Preferences(_message.Message):
         __slots__ = ["locale", "runtime", "timezone"]
         LOCALE_FIELD_NUMBER: _ClassVar[int]
         RUNTIME_FIELD_NUMBER: _ClassVar[int]
         TIMEZONE_FIELD_NUMBER: _ClassVar[int]
         locale: str
         runtime: str
@@ -27,22 +26,24 @@
     NICKNAME_CHANGE_TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     NICKNAME_FIELD_NUMBER: _ClassVar[int]
     PASSWORD_AGE_FIELD_NUMBER: _ClassVar[int]
     PASSWORD_FIELD_NUMBER: _ClassVar[int]
     PICTURE_FIELD_NUMBER: _ClassVar[int]
     PREFERENCES_FIELD_NUMBER: _ClassVar[int]
     SUBJECT_FIELD_NUMBER: _ClassVar[int]
+    TEAM_ID_FIELD_NUMBER: _ClassVar[int]
     birthday: _timestamp_pb2.Timestamp
     city: str
     country: str
     email: str
     email_verified: bool
     issuer: str
     name: str
     nickname: str
     nickname_change_timeout: int
     password: str
     password_age: int
     picture: str
     preferences: User.Preferences
     subject: str
-    def __init__(self, issuer: _Optional[str] = ..., subject: _Optional[str] = ..., nickname: _Optional[str] = ..., nickname_change_timeout: _Optional[int] = ..., email: _Optional[str] = ..., email_verified: bool = ..., password: _Optional[str] = ..., password_age: _Optional[int] = ..., name: _Optional[str] = ..., picture: _Optional[str] = ..., birthday: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., country: _Optional[str] = ..., city: _Optional[str] = ..., preferences: _Optional[_Union[User.Preferences, _Mapping]] = ...) -> None: ...
+    team_id: str
+    def __init__(self, issuer: _Optional[str] = ..., subject: _Optional[str] = ..., nickname: _Optional[str] = ..., nickname_change_timeout: _Optional[int] = ..., email: _Optional[str] = ..., email_verified: bool = ..., password: _Optional[str] = ..., password_age: _Optional[int] = ..., name: _Optional[str] = ..., picture: _Optional[str] = ..., birthday: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., country: _Optional[str] = ..., city: _Optional[str] = ..., team_id: _Optional[str] = ..., preferences: _Optional[_Union[User.Preferences, _Mapping]] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/community/membership_service_http.py` & `eolymp-0.8.1/eolymp/community/membership_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/community/membership_service_pb2.py` & `eolymp-0.8.1/eolymp/community/membership_service_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,36 +11,33 @@
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.community import attribute_pb2 as eolymp_dot_community_dot_attribute__pb2
-from eolymp.community import configuration_idp_pb2 as eolymp_dot_community_dot_configuration__idp__pb2
 from eolymp.community import member_pb2 as eolymp_dot_community_dot_member__pb2
-from eolymp.wellknown import direction_pb2 as eolymp_dot_wellknown_dot_direction__pb2
-from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)eolymp/community/membership_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a(eolymp/community/configuration_idp.proto\x1a\x1d\x65olymp/community/member.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"\x19\n\x17\x44\x65scribeMembershipInput\"D\n\x18\x44\x65scribeMembershipOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"N\n\x15UpdateMembershipInput\x12\x35\n\nattributes\x18\x01 \x03(\x0b\x32!.eolymp.community.Attribute.Value\"\x18\n\x16UpdateMembershipOutput2\xe0\x02\n\x11MembershipService\x12\x92\x01\n\x12\x44\x65scribeMembership\x12).eolymp.community.DescribeMembershipInput\x1a*.eolymp.community.DescribeMembershipOutput\"%\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x10\x12\x0e/members/_self\x12\xb5\x01\n\x10UpdateMembership\x12\'.eolymp.community.UpdateMembershipInput\x1a(.eolymp.community.UpdateMembershipOutput\"N\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1b\"\x19/members/_self/attributesB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)eolymp/community/membership_service.proto\x12\x10\x65olymp.community\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/community/attribute.proto\x1a\x1d\x65olymp/community/member.proto\"\x19\n\x17\x44\x65scribeMembershipInput\"D\n\x18\x44\x65scribeMembershipOutput\x12(\n\x06member\x18\x01 \x01(\x0b\x32\x18.eolymp.community.Member\"N\n\x15UpdateMembershipInput\x12\x35\n\nattributes\x18\x01 \x03(\x0b\x32!.eolymp.community.Attribute.Value\"\x18\n\x16UpdateMembershipOutput2\xe0\x02\n\x11MembershipService\x12\x92\x01\n\x12\x44\x65scribeMembership\x12).eolymp.community.DescribeMembershipInput\x1a*.eolymp.community.DescribeMembershipOutput\"%\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x10\x12\x0e/members/_self\x12\xb5\x01\n\x10UpdateMembership\x12\'.eolymp.community.UpdateMembershipInput\x1a(.eolymp.community.UpdateMembershipOutput\"N\x82\xe3\n\x1a\x8a\xe3\n\x16\x63ommunity:member:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1b\"\x19/members/_self/attributesB5Z3github.com/eolymp/go-sdk/eolymp/community;communityb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.community.membership_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/community;community'
   _MEMBERSHIPSERVICE.methods_by_name['DescribeMembership']._options = None
   _MEMBERSHIPSERVICE.methods_by_name['DescribeMembership']._serialized_options = b'\352\342\n\013\365\342\n\000\000 A\370\342\n2\202\323\344\223\002\020\022\016/members/_self'
   _MEMBERSHIPSERVICE.methods_by_name['UpdateMembership']._options = None
   _MEMBERSHIPSERVICE.methods_by_name['UpdateMembership']._serialized_options = b'\202\343\n\032\212\343\n\026community:member:write\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\033\"\031/members/_self/attributes'
-  _DESCRIBEMEMBERSHIPINPUT._serialized_start=338
-  _DESCRIBEMEMBERSHIPINPUT._serialized_end=363
-  _DESCRIBEMEMBERSHIPOUTPUT._serialized_start=365
-  _DESCRIBEMEMBERSHIPOUTPUT._serialized_end=433
-  _UPDATEMEMBERSHIPINPUT._serialized_start=435
-  _UPDATEMEMBERSHIPINPUT._serialized_end=513
-  _UPDATEMEMBERSHIPOUTPUT._serialized_start=515
-  _UPDATEMEMBERSHIPOUTPUT._serialized_end=539
-  _MEMBERSHIPSERVICE._serialized_start=542
-  _MEMBERSHIPSERVICE._serialized_end=894
+  _DESCRIBEMEMBERSHIPINPUT._serialized_start=227
+  _DESCRIBEMEMBERSHIPINPUT._serialized_end=252
+  _DESCRIBEMEMBERSHIPOUTPUT._serialized_start=254
+  _DESCRIBEMEMBERSHIPOUTPUT._serialized_end=322
+  _UPDATEMEMBERSHIPINPUT._serialized_start=324
+  _UPDATEMEMBERSHIPINPUT._serialized_end=402
+  _UPDATEMEMBERSHIPOUTPUT._serialized_start=404
+  _UPDATEMEMBERSHIPOUTPUT._serialized_end=428
+  _MEMBERSHIPSERVICE._serialized_start=431
+  _MEMBERSHIPSERVICE._serialized_end=783
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/community/membership_service_pb2.pyi` & `eolymp-0.8.1/eolymp/community/membership_service_pb2.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.community import attribute_pb2 as _attribute_pb2
-from eolymp.community import configuration_idp_pb2 as _configuration_idp_pb2
 from eolymp.community import member_pb2 as _member_pb2
-from eolymp.wellknown import direction_pb2 as _direction_pb2
-from eolymp.wellknown import expression_pb2 as _expression_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Iterable as _Iterable, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
```

### Comparing `eolymp-0.8.0/eolymp/core/http_client.py` & `eolymp-0.8.1/eolymp/core/http_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/core/oauth_client.py` & `eolymp-0.8.1/eolymp/core/oauth_client.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/discussion_pb2.py` & `eolymp-0.8.1/eolymp/discussion/discussion_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/discussion_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/discussion_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/discussion_service_http.py` & `eolymp-0.8.1/eolymp/discussion/discussion_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/discussion_service_pb2.py` & `eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/discussion_service_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/discussion_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/events_pb2.py` & `eolymp-0.8.1/eolymp/discussion/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/events_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/forum_pb2.py` & `eolymp-0.8.1/eolymp/discussion/forum_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/forum_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/forum_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/forum_service_http.py` & `eolymp-0.8.1/eolymp/discussion/forum_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/forum_service_pb2.py` & `eolymp-0.8.1/eolymp/discussion/forum_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/forum_service_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/forum_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/message_pb2.py` & `eolymp-0.8.1/eolymp/discussion/message_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/message_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/message_service_http.py` & `eolymp-0.8.1/eolymp/discussion/message_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/message_service_pb2.py` & `eolymp-0.8.1/eolymp/discussion/message_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/message_service_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/message_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/subscription_pb2.py` & `eolymp-0.8.1/eolymp/discussion/subscription_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/subscription_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/subscription_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/subscription_service_http.py` & `eolymp-0.8.1/eolymp/discussion/subscription_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/subscription_service_pb2.py` & `eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/discussion/subscription_service_pb2.pyi` & `eolymp-0.8.1/eolymp/discussion/subscription_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ecm/content_pb2.py` & `eolymp-0.8.1/eolymp/ecm/content_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ecm/content_pb2.pyi` & `eolymp-0.8.1/eolymp/ecm/content_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ecm/node_pb2.py` & `eolymp-0.8.1/eolymp/ecm/node_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ecm/node_pb2.pyi` & `eolymp-0.8.1/eolymp/ecm/node_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/events_pb2.py` & `eolymp-0.8.1/eolymp/executor/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/events_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/executor_http.py` & `eolymp-0.8.1/eolymp/executor/executor_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/executor_pb2.py` & `eolymp-0.8.1/eolymp/executor/executor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/executor_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/executor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/interactor_pb2.py` & `eolymp-0.8.1/eolymp/executor/interactor_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/interactor_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/interactor_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/job_pb2.py` & `eolymp-0.8.1/eolymp/executor/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/job_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/job_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/language_pb2.py` & `eolymp-0.8.1/eolymp/executor/language_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/language_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/runtime_pb2.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Language(_message.Message):
-    __slots__ = ["deprecated", "id", "name"]
+class Runtime(_message.Message):
+    __slots__ = ["deprecated", "id", "lang", "name", "version"]
     DEPRECATED_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
+    LANG_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
+    VERSION_FIELD_NUMBER: _ClassVar[int]
     deprecated: bool
     id: str
+    lang: str
     name: str
-    def __init__(self, id: _Optional[str] = ..., name: _Optional[str] = ..., deprecated: bool = ...) -> None: ...
+    version: str
+    def __init__(self, id: _Optional[str] = ..., lang: _Optional[str] = ..., version: _Optional[str] = ..., name: _Optional[str] = ..., deprecated: bool = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/executor/report_pb2.py` & `eolymp-0.8.1/eolymp/executor/report_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/report_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/report_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/runtime_pb2.py` & `eolymp-0.8.1/eolymp/executor/runtime_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/runtime_pb2.pyi` & `eolymp-0.8.1/eolymp/harmony/agreement_pb2.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Optional as _Optional
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Runtime(_message.Message):
-    __slots__ = ["deprecated", "id", "lang", "name", "version"]
-    DEPRECATED_FIELD_NUMBER: _ClassVar[int]
+class Agreement(_message.Message):
+    __slots__ = ["description", "id", "required", "summary"]
+    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
-    LANG_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    VERSION_FIELD_NUMBER: _ClassVar[int]
-    deprecated: bool
+    REQUIRED_FIELD_NUMBER: _ClassVar[int]
+    SUMMARY_FIELD_NUMBER: _ClassVar[int]
+    description: str
     id: str
-    lang: str
-    name: str
-    version: str
-    def __init__(self, id: _Optional[str] = ..., lang: _Optional[str] = ..., version: _Optional[str] = ..., name: _Optional[str] = ..., deprecated: bool = ...) -> None: ...
+    required: bool
+    summary: str
+    def __init__(self, id: _Optional[str] = ..., required: bool = ..., summary: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/executor/status_pb2.py` & `eolymp-0.8.1/eolymp/executor/status_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/status_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/task_pb2.py` & `eolymp-0.8.1/eolymp/executor/task_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/task_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/task_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/usage_pb2.py` & `eolymp-0.8.1/eolymp/executor/usage_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/usage_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/usage_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/verifier_pb2.py` & `eolymp-0.8.1/eolymp/executor/verifier_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/executor/verifier_pb2.pyi` & `eolymp-0.8.1/eolymp/executor/verifier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/country_pb2.py` & `eolymp-0.8.1/eolymp/geography/country_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/country_pb2.pyi` & `eolymp-0.8.1/eolymp/geography/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/geography_http.py` & `eolymp-0.8.1/eolymp/geography/geography_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/geography_pb2.py` & `eolymp-0.8.1/eolymp/geography/geography_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/geography_pb2.pyi` & `eolymp-0.8.1/eolymp/geography/geography_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/region_pb2.py` & `eolymp-0.8.1/eolymp/geography/region_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/geography/region_pb2.pyi` & `eolymp-0.8.1/eolymp/geography/region_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/harmony/agreement_pb2.py` & `eolymp-0.8.1/eolymp/harmony/agreement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/harmony/agreement_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/announcement_pb2.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,22 @@
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional
+from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Agreement(_message.Message):
-    __slots__ = ["description", "id", "required", "summary"]
-    DESCRIPTION_FIELD_NUMBER: _ClassVar[int]
+class Announcement(_message.Message):
+    __slots__ = ["contest_id", "created_at", "ern", "id", "message", "subject"]
+    CONTEST_ID_FIELD_NUMBER: _ClassVar[int]
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    ERN_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
-    REQUIRED_FIELD_NUMBER: _ClassVar[int]
-    SUMMARY_FIELD_NUMBER: _ClassVar[int]
-    description: str
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    SUBJECT_FIELD_NUMBER: _ClassVar[int]
+    contest_id: str
+    created_at: _timestamp_pb2.Timestamp
+    ern: str
     id: str
-    required: bool
-    summary: str
-    def __init__(self, id: _Optional[str] = ..., required: bool = ..., summary: _Optional[str] = ..., description: _Optional[str] = ...) -> None: ...
+    message: str
+    subject: str
+    def __init__(self, id: _Optional[str] = ..., ern: _Optional[str] = ..., contest_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., subject: _Optional[str] = ..., message: _Optional[str] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/harmony/consent_pb2.py` & `eolymp-0.8.1/eolymp/harmony/consent_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/harmony/consent_pb2.pyi` & `eolymp-0.8.1/eolymp/harmony/consent_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/harmony/harmony_http.py` & `eolymp-0.8.1/eolymp/harmony/harmony_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/harmony/harmony_pb2.py` & `eolymp-0.8.1/eolymp/harmony/harmony_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/harmony/harmony_pb2.pyi` & `eolymp-0.8.1/eolymp/harmony/harmony_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/auto_reply_pb2.py` & `eolymp-0.8.1/eolymp/helpdesk/document_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/helpdesk/auto_reply.proto
+# source: eolymp/helpdesk/document.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.ecm import content_pb2 as eolymp_dot_ecm_dot_content__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/helpdesk/auto_reply.proto\x12\x0f\x65olymp.helpdesk\x1a\x18\x65olymp/ecm/content.proto\"k\n\tAutoReply\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0e\n\x06locale\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x14 \x01(\t\x12$\n\x07message\x18\x15 \x01(\x0b\x32\x13.eolymp.ecm.Content\x12\x0e\n\x06labels\x18\x16 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdeskb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/helpdesk/document.proto\x12\x0f\x65olymp.helpdesk\x1a\x18\x65olymp/ecm/content.proto\"y\n\x08\x44ocument\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\r\n\x05title\x18\x0c \x01(\t\x12$\n\x07\x63ontent\x18\x33 \x01(\x0b\x32\x13.eolymp.ecm.Content\x12\x0e\n\x06labels\x18\x64 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdeskb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.helpdesk.auto_reply_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.helpdesk.document_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdesk'
-  _AUTOREPLY._serialized_start=79
-  _AUTOREPLY._serialized_end=186
+  _DOCUMENT._serialized_start=77
+  _DOCUMENT._serialized_end=198
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/helpdesk/auto_reply_pb2.pyi` & `eolymp-0.8.1/eolymp/helpdesk/auto_reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/document_pb2.py` & `eolymp-0.8.1/eolymp/judge/template_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/helpdesk/document.proto
+# source: eolymp/judge/template.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.ecm import content_pb2 as eolymp_dot_ecm_dot_content__pb2
+from eolymp.atlas import code_template_file_pb2 as eolymp_dot_atlas_dot_code__template__file__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/helpdesk/document.proto\x12\x0f\x65olymp.helpdesk\x1a\x18\x65olymp/ecm/content.proto\"y\n\x08\x44ocument\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\r\n\x05title\x18\x0c \x01(\t\x12$\n\x07\x63ontent\x18\x33 \x01(\x0b\x32\x13.eolymp.ecm.Content\x12\x0e\n\x06labels\x18\x64 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdeskb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65olymp/judge/template.proto\x12\x0c\x65olymp.judge\x1a%eolymp/atlas/code_template_file.proto\"\xa8\x01\n\x08Template\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x0f\n\x07runtime\x18\x03 \x01(\t\x12\x12\n\nsource_ern\x18\n \x01(\t\x12\x12\n\nheader_ern\x18\x0b \x01(\t\x12\x12\n\nfooter_ern\x18\x0c \x01(\t\x12!\n\x05\x66iles\x18\x1e \x03(\x0b\x32\x12.eolymp.atlas.FileB-Z+github.com/eolymp/go-sdk/eolymp/judge;judgeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.helpdesk.document_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.judge.template_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/helpdesk;helpdesk'
-  _DOCUMENT._serialized_start=77
-  _DOCUMENT._serialized_end=198
+  DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/judge;judge'
+  _TEMPLATE._serialized_start=85
+  _TEMPLATE._serialized_end=253
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/helpdesk/document_pb2.pyi` & `eolymp-0.8.1/eolymp/helpdesk/document_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/events_pb2.py` & `eolymp-0.8.1/eolymp/helpdesk/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/events_pb2.pyi` & `eolymp-0.8.1/eolymp/helpdesk/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/helpdesk_http.py` & `eolymp-0.8.1/eolymp/helpdesk/helpdesk_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/helpdesk_pb2.py` & `eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/helpdesk_pb2.pyi` & `eolymp-0.8.1/eolymp/helpdesk/helpdesk_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/support_http.py` & `eolymp-0.8.1/eolymp/helpdesk/support_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/support_pb2.py` & `eolymp-0.8.1/eolymp/helpdesk/support_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/support_pb2.pyi` & `eolymp-0.8.1/eolymp/helpdesk/support_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/ticket_pb2.py` & `eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/helpdesk/ticket_pb2.pyi` & `eolymp-0.8.1/eolymp/helpdesk/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/acl_http.py` & `eolymp-0.8.1/eolymp/judge/acl_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/acl_pb2.py` & `eolymp-0.8.1/eolymp/judge/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/acl_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/acl_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/activity_pb2.py` & `eolymp-0.8.1/eolymp/judge/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/activity_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/activity_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/announcement_pb2.py` & `eolymp-0.8.1/eolymp/judge/announcement_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/announcement_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/result_pb2.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from eolymp.judge import score_pb2 as _score_pb2
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Announcement(_message.Message):
-    __slots__ = ["contest_id", "created_at", "ern", "id", "message", "subject"]
+class Result(_message.Message):
+    __slots__ = ["contest_id", "name", "out_of_competition", "participant_id", "rank", "rank_lower", "score"]
     CONTEST_ID_FIELD_NUMBER: _ClassVar[int]
-    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    ERN_FIELD_NUMBER: _ClassVar[int]
-    ID_FIELD_NUMBER: _ClassVar[int]
-    MESSAGE_FIELD_NUMBER: _ClassVar[int]
-    SUBJECT_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    OUT_OF_COMPETITION_FIELD_NUMBER: _ClassVar[int]
+    PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
+    RANK_FIELD_NUMBER: _ClassVar[int]
+    RANK_LOWER_FIELD_NUMBER: _ClassVar[int]
+    SCORE_FIELD_NUMBER: _ClassVar[int]
     contest_id: str
-    created_at: _timestamp_pb2.Timestamp
-    ern: str
-    id: str
-    message: str
-    subject: str
-    def __init__(self, id: _Optional[str] = ..., ern: _Optional[str] = ..., contest_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., subject: _Optional[str] = ..., message: _Optional[str] = ...) -> None: ...
+    name: str
+    out_of_competition: bool
+    participant_id: str
+    rank: int
+    rank_lower: int
+    score: _score_pb2.Score
+    def __init__(self, participant_id: _Optional[str] = ..., contest_id: _Optional[str] = ..., name: _Optional[str] = ..., out_of_competition: bool = ..., rank: _Optional[int] = ..., rank_lower: _Optional[int] = ..., score: _Optional[_Union[_score_pb2.Score, _Mapping]] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/judge/contest_pb2.py` & `eolymp-0.8.1/eolymp/judge/contest_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/contest_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/contest_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/entitlement_pb2.py` & `eolymp-0.8.1/eolymp/l10n/term_pb2.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/judge/entitlement.proto
+# source: eolymp/l10n/term.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/judge/entitlement.proto\x12\x0c\x65olymp.judge*\xff\x02\n\x0b\x45ntitlement\x12\x08\n\x04NONE\x10\x00\x12\x12\n\x0e\x43REATE_CONTEST\x10\x01\x12\x12\n\x0eLOOKUP_CONTEST\x10\x02\x12\x12\n\x0eMANAGE_CONTEST\x10\x03\x12\x10\n\x0cVIEW_RUNTIME\x10\x04\x12\x1a\n\x16VIEW_REGISTRATION_FORM\x10\x05\x12\x14\n\x10VIEW_PARTICIPANT\x10\x06\x12\x16\n\x12MANAGE_PARTICIPANT\x10\x07\x12\x10\n\x0cVIEW_PROBLEM\x10\x08\x12\x12\n\x0eMANAGE_PROBLEM\x10\t\x12\x15\n\x11\x43REATE_SUBMISSION\x10\n\x12\x13\n\x0fVIEW_SUBMISSION\x10\x0b\x12\x15\n\x11MANAGE_SUBMISSION\x10\x0c\x12\x15\n\x11VIEW_ANNOUNCEMENT\x10\r\x12\x17\n\x13MANAGE_ANNOUNCEMENT\x10\x0e\x12\x11\n\rCREATE_TICKET\x10\x0f\x12\x0f\n\x0bVIEW_TICKET\x10\x10\x12\x11\n\rMANAGE_TICKET\x10\x11\x42-Z+github.com/eolymp/go-sdk/eolymp/judge;judgeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x65olymp/l10n/term.proto\x12\x0b\x65olymp.l10n\"\x9f\x01\n\x04Term\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12(\n\x06status\x18\x04 \x01(\x0e\x32\x18.eolymp.l10n.Term.Status\".\n\x06Status\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0e\n\nDEPRECATED\x10\x02\x42+Z)github.com/eolymp/go-sdk/eolymp/l10n;l10nb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.judge.entitlement_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.l10n.term_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/judge;judge'
-  _ENTITLEMENT._serialized_start=49
-  _ENTITLEMENT._serialized_end=432
+  DESCRIPTOR._serialized_options = b'Z)github.com/eolymp/go-sdk/eolymp/l10n;l10n'
+  _TERM._serialized_start=40
+  _TERM._serialized_end=199
+  _TERM_STATUS._serialized_start=153
+  _TERM_STATUS._serialized_end=199
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/judge/events_pb2.py` & `eolymp-0.8.1/eolymp/judge/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/events_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/judge_http.py` & `eolymp-0.8.1/eolymp/judge/judge_http.py`

 * *Files 0% similar despite different names*

```diff
@@ -1068,25 +1068,14 @@
             method="POST",
             url=self.url+path,
             request_data=request,
             response_symbol=_sym_db.GetSymbol("eolymp.judge.RebuildScoreOutput"),
             **kwargs,
         )
 
-    def ListEntitlements(self, request, **kwargs):
-        path = "/__judge/entitlements"
-
-        return self.transport.request(
-            method="GET",
-            url=self.url+path,
-            request_data=request,
-            response_symbol=_sym_db.GetSymbol("eolymp.judge.ListEntitlementsOutput"),
-            **kwargs,
-        )
-
     def ListActivities(self, request, **kwargs):
         path = "/contests/"+urllib.parse.quote(request.contest_id)+"/activities"
 
         # Cleanup URL parameters to avoid any ambiguity
         request.contest_id = ""
 
         return self.transport.request(
```

### Comparing `eolymp-0.8.0/eolymp/judge/judge_pb2.py` & `eolymp-0.8.1/eolymp/judge/judge_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,27 @@
 
 from eolymp.annotations import http_pb2 as eolymp_dot_annotations_dot_http__pb2
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.judge import activity_pb2 as eolymp_dot_judge_dot_activity__pb2
 from eolymp.judge import announcement_pb2 as eolymp_dot_judge_dot_announcement__pb2
 from eolymp.judge import contest_pb2 as eolymp_dot_judge_dot_contest__pb2
-from eolymp.judge import entitlement_pb2 as eolymp_dot_judge_dot_entitlement__pb2
 from eolymp.judge import participant_pb2 as eolymp_dot_judge_dot_participant__pb2
 from eolymp.judge import problem_pb2 as eolymp_dot_judge_dot_problem__pb2
 from eolymp.judge import reply_pb2 as eolymp_dot_judge_dot_reply__pb2
 from eolymp.judge import result_pb2 as eolymp_dot_judge_dot_result__pb2
 from eolymp.judge import score_pb2 as eolymp_dot_judge_dot_score__pb2
 from eolymp.judge import submission_pb2 as eolymp_dot_judge_dot_submission__pb2
 from eolymp.judge import template_pb2 as eolymp_dot_judge_dot_template__pb2
 from eolymp.judge import ticket_pb2 as eolymp_dot_judge_dot_ticket__pb2
 from eolymp.wellknown import direction_pb2 as eolymp_dot_wellknown_dot_direction__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x65olymp/judge/judge.proto\x12\x0c\x65olymp.judge\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1b\x65olymp/judge/activity.proto\x1a\x1f\x65olymp/judge/announcement.proto\x1a\x1a\x65olymp/judge/contest.proto\x1a\x1e\x65olymp/judge/entitlement.proto\x1a\x1e\x65olymp/judge/participant.proto\x1a\x1a\x65olymp/judge/problem.proto\x1a\x18\x65olymp/judge/reply.proto\x1a\x19\x65olymp/judge/result.proto\x1a\x18\x65olymp/judge/score.proto\x1a\x1d\x65olymp/judge/submission.proto\x1a\x1b\x65olymp/judge/template.proto\x1a\x19\x65olymp/judge/ticket.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"<\n\x12\x43reateContestInput\x12&\n\x07\x63ontest\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Contest\")\n\x13\x43reateContestOutput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"(\n\x12\x44\x65leteContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x15\n\x13\x44\x65leteContestOutput\"P\n\x12UpdateContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12&\n\x07\x63ontest\x18\x02 \x01(\x0b\x32\x15.eolymp.judge.Contest\"\x15\n\x13UpdateContestOutput\"*\n\x14\x44\x65scribeContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"?\n\x15\x44\x65scribeContestOutput\x12&\n\x07\x63ontest\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Contest\"!\n\x12LookupContestInput\x12\x0b\n\x03key\x18\x01 \x01(\t\"s\n\x13LookupContestOutput\x12&\n\x07\x63ontest\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Contest\x12\x34\n\nappearance\x18\x02 \x01(\x0b\x32 .eolymp.judge.Contest.Appearance\"\x8e\x04\n\x11ListContestsInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x37\n\x07\x66ilters\x18( \x01(\x0b\x32&.eolymp.judge.ListContestsInput.Filter\x1a\xa1\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12-\n\x03own\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x38\n\tstarts_at\x18\x04 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x36\n\x07\x65nds_at\x18\x05 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x30\n\x06public\x18\x06 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nvisibility\x18\x07 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x06\x66ormat\x18\x08 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"I\n\x12ListContestsOutput\x12$\n\x05items\x18\x01 \x03(\x0b\x32\x15.eolymp.judge.Contest\x12\r\n\x05total\x18\x02 \x01(\x05\"&\n\x10OpenContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x13\n\x11OpenContestOutput\"\'\n\x11\x43loseContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x14\n\x12\x43loseContestOutput\")\n\x13SuspendContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x16\n\x14SuspendContestOutput\"(\n\x12\x46reezeContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x15\n\x13\x46reezeContestOutput\"(\n\x12ResumeContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x15\n\x13ResumeContestOutput\"&\n\x10JoinContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x13\n\x11JoinContestOutput\"\'\n\x11StartContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x14\n\x12StartContestOutput\"\x7f\n\x12ImportProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\timport_id\x18\x02 \x01(\t\x12\r\n\x05index\x18\n \x01(\r\x12\x14\n\x0csubmit_limit\x18\x0b \x01(\r\x12\x1d\n\x15score_by_best_testset\x18\x0c \x01(\x08\")\n\x13ImportProblemOutput\x12\x12\n\nproblem_id\x18\x02 \x01(\t\":\n\x10SyncProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"\x13\n\x11SyncProblemOutput\"\x80\x01\n\x12UpdateProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\r\n\x05index\x18\n \x01(\r\x12\x14\n\x0csubmit_limit\x18\x0b \x01(\r\x12\x1d\n\x15score_by_best_testset\x18\x0c \x01(\x08\"\x15\n\x13UpdateProblemOutput\"<\n\x12\x44\x65leteProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"\x15\n\x13\x44\x65leteProblemOutput\"<\n\x12RetestProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"\x15\n\x13RetestProblemOutput\"E\n\x11ListProblemsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"I\n\x12ListProblemsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12$\n\x05items\x18\x02 \x03(\x0b\x32\x15.eolymp.judge.Problem\"T\n\x14\x44\x65scribeProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x14\n\x0bproblem_ern\x18\x8fN \x01(\t\"?\n\x15\x44\x65scribeProblemOutput\x12&\n\x07problem\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Problem\"=\n\x13ListStatementsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"U\n\x14ListStatementsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12.\n\x05items\x18\x02 \x03(\x0b\x32\x1f.eolymp.judge.Problem.Statement\">\n\x14ListAttachmentsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"W\n\x15ListAttachmentsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12/\n\x05items\x18\x02 \x03(\x0b\x32 .eolymp.judge.Problem.Attachment\";\n\x11ListExamplesInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"N\n\x12ListExamplesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12)\n\x05items\x18\x02 \x03(\x0b\x32\x1a.eolymp.judge.Problem.Test\"f\n\x13\x41\x64\x64ParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tmember_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12out_of_competition\x18\x04 \x01(\x08\".\n\x14\x41\x64\x64ParticipantOutput\x12\x16\n\x0eparticipant_id\x18\x01 \x01(\t\"D\n\x16\x45nableParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x19\n\x17\x45nableParticipantOutput\"E\n\x17\x44isableParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x1a\n\x18\x44isableParticipantOutput\"\x81\x02\n\x16UpdateParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12\x39\n\x05patch\x18\x03 \x01(\x0e\x32*.eolymp.judge.UpdateParticipantInput.Patch\x12\x0c\n\x04name\x18\n \x01(\t\x12\x12\n\nbonus_time\x18\x0c \x01(\r\x12\x1a\n\x12out_of_competition\x18\x0b \x01(\x08\"B\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\x08\n\x04NAME\x10\x01\x12\x0e\n\nBONUS_TIME\x10\x03\x12\x16\n\x12OUT_OF_COMPETITION\x10\x04\"\x19\n\x17UpdateParticipantOutput\"D\n\x16RemoveParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x19\n\x17RemoveParticipantOutput\")\n\x13VerifyPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"7\n\x14VerifyPasscodeOutput\x12\x10\n\x08required\x18\x01 \x01(\x08\x12\r\n\x05valid\x18\x02 \x01(\x08\":\n\x12\x45nterPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x10\n\x08passcode\x18\x02 \x01(\t\"\x15\n\x13\x45nterPasscodeOutput\"@\n\x12ResetPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\'\n\x13ResetPasscodeOutput\x12\x10\n\x08passcode\x18\x01 \x01(\t\"P\n\x10SetPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12\x10\n\x08passcode\x18\x03 \x01(\t\"\x13\n\x11SetPasscodeOutput\"A\n\x13RemovePasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x16\n\x14RemovePasscodeOutput\"\xe8\x05\n\x15ListParticipantsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12;\n\x07\x66ilters\x18( \x01(\x0b\x32*.eolymp.judge.ListParticipantsInput.Filter\x12:\n\x04sort\x18\x32 \x01(\x0e\x32,.eolymp.judge.ListParticipantsInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\xa8\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x31\n\tmember_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x04name\x18\x08 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x30\n\x06status\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x05score\x18\x04 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x32\n\x07penalty\x18\x05 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x39\n\nstarted_at\x18\x06 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12:\n\x0b\x63omplete_at\x18\x07 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\"M\n\x08Sortable\x12\x08\n\x04RANK\x10\x00\x12\t\n\x05SCORE\x10\x01\x12\x0b\n\x07PENALTY\x10\x02\x12\x0e\n\nSTARTED_AT\x10\x03\x12\x0f\n\x0b\x43OMPLETE_AT\x10\x04\"Q\n\x16ListParticipantsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12(\n\x05items\x18\x02 \x03(\x0b\x32\x19.eolymp.judge.Participant\"0\n\x1aIntrospectParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"M\n\x1bIntrospectParticipantOutput\x12.\n\x0bparticipant\x18\x01 \x01(\x0b\x32\x19.eolymp.judge.Participant\"F\n\x18\x44\x65scribeParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"K\n\x19\x44\x65scribeParticipantOutput\x12.\n\x0bparticipant\x18\x01 \x01(\x0b\x32\x19.eolymp.judge.Participant\"]\n\x15\x43reateSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x0c\n\x04lang\x18\x03 \x01(\t\x12\x0e\n\x06source\x18\x04 \x01(\t\"/\n\x16\x43reateSubmissionOutput\x12\x15\n\rsubmission_id\x18\x01 \x01(\t\"\xe4\x04\n\x14ListSubmissionsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12:\n\x07\x66ilters\x18( \x01(\x0b\x32).eolymp.judge.ListSubmissionsInput.Filter\x1a\xdd\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x36\n\x0eparticipant_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x32\n\nproblem_id\x18\x03 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x06status\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12.\n\x04lang\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x05score\x18\x06 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x35\n\npercentage\x18\x07 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12;\n\x0csubmitted_at\x18\x08 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x33\n\tsignature\x18\t \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"O\n\x15ListSubmissionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\'\n\x05items\x18\x02 \x03(\x0b\x32\x18.eolymp.judge.Submission\"D\n\x17\x44\x65scribeSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"H\n\x18\x44\x65scribeSubmissionOutput\x12,\n\nsubmission\x18\x01 \x01(\x0b\x32\x18.eolymp.judge.Submission\"B\n\x15RetestSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"\x18\n\x16RetestSubmissionOutput\"B\n\x15\x44\x65leteSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"\x18\n\x16\x44\x65leteSubmissionOutput\"C\n\x16RestoreSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"\x19\n\x17RestoreSubmissionOutput\"I\n\x11\x43reateTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"\'\n\x12\x43reateTicketOutput\x12\x11\n\tticket_id\x18\x01 \x01(\t\"9\n\x10\x43loseTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x13\n\x11\x43loseTicketOutput\"8\n\x0fOpenTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x12\n\x10OpenTicketOutput\"8\n\x0fReadTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x12\n\x10ReadTicketOutput\":\n\x11\x44\x65leteTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x14\n\x12\x44\x65leteTicketOutput\"<\n\x13\x44\x65scribeTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"<\n\x14\x44\x65scribeTicketOutput\x12$\n\x06ticket\x18\x01 \x01(\x0b\x32\x14.eolymp.judge.Ticket\"\x96\x05\n\x10ListTicketsInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x36\n\x07\x66ilters\x18( \x01(\x0b\x32%.eolymp.judge.ListTicketsInput.Filter\x12\x35\n\x04sort\x18\x32 \x01(\x0e\x32\'.eolymp.judge.ListTicketsInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\x80\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x32\n\ncontest_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x36\n\x0eparticipant_id\x18\x03 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12@\n\x16is_read_by_participant\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12:\n\x10is_read_by_owner\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x31\n\x07is_open\x18\x06 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12-\n\x03own\x18\x07 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"F\n\x08Sortable\x12\x0e\n\nCREATED_AT\x10\x00\x12\x11\n\rREAD_BY_OWNER\x10\x01\x12\x17\n\x13READ_BY_PARTICIPANT\x10\x02\"G\n\x11ListTicketsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12#\n\x05items\x18\x02 \x03(\x0b\x32\x14.eolymp.judge.Ticket\"E\n\x10ReplyTicketInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\n \x01(\t\x12\r\n\x05\x63lose\x18\x15 \x01(\x08\"%\n\x11ReplyTicketOutput\x12\x10\n\x08reply_id\x18\x01 \x01(\t\"C\n\x10ListRepliesInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"F\n\x11ListRepliesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\"\n\x05items\x18\x02 \x03(\x0b\x32\x13.eolymp.judge.Reply\"7\n\x10\x44\x65leteReplyInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x10\n\x08reply_id\x18\x02 \x01(\t\"\x13\n\x11\x44\x65leteReplyOutput\"H\n\x10UpdateReplyInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x10\n\x08reply_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"\x13\n\x11UpdateReplyOutput\"<\n\x15\x43onfigureRuntimeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0f\n\x07runtime\x18\x02 \x03(\t\"\x18\n\x16\x43onfigureRuntimeOutput\"*\n\x14\x44\x65scribeRuntimeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"(\n\x15\x44\x65scribeRuntimeOutput\x12\x0f\n\x07runtime\x18\x01 \x03(\t\"[\n\x15\x43onfigureScoringInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12.\n\x07scoring\x18\x02 \x01(\x0b\x32\x1d.eolymp.judge.Contest.Scoring\"\x18\n\x16\x43onfigureScoringOutput\"*\n\x14\x44\x65scribeScoringInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"G\n\x15\x44\x65scribeScoringOutput\x12.\n\x07scoring\x18\x01 \x01(\x0b\x32\x1d.eolymp.judge.Contest.Scoring\"_\n\x17\x43reateAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x30\n\x0c\x61nnouncement\x18\x02 \x01(\x0b\x32\x1a.eolymp.judge.Announcement\"&\n\x18\x43reateAnnouncementOutput\x12\n\n\x02id\x18\x01 \x01(\t\"x\n\x17UpdateAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\x12\x30\n\x0c\x61nnouncement\x18\x03 \x01(\x0b\x32\x1a.eolymp.judge.Announcement\"\x1a\n\x18UpdateAnnouncementOutput\"F\n\x17\x44\x65leteAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"\x1a\n\x18\x44\x65leteAnnouncementOutput\"D\n\x15ReadAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"\x18\n\x16ReadAnnouncementOutput\"H\n\x19\x44\x65scribeAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"N\n\x1a\x44\x65scribeAnnouncementOutput\x12\x30\n\x0c\x61nnouncement\x18\x01 \x01(\x0b\x32\x1a.eolymp.judge.Announcement\"N\n\x1f\x44\x65scribeAnnouncementStatusInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"3\n DescribeAnnouncementStatusOutput\x12\x0f\n\x07is_read\x18\x01 \x01(\x08\"\xf1\x01\n\x16ListAnnouncementsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12<\n\x07\x66ilters\x18( \x01(\x0b\x32+.eolymp.judge.ListAnnouncementsInput.Filter\x1ag\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x31\n\x07is_read\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"S\n\x17ListAnnouncementsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12)\n\x05items\x18\x02 \x03(\x0b\x32\x1a.eolymp.judge.Announcement\"n\n\x19\x44\x65scribeCodeTemplateInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x13\n\x0btemplate_id\x18\x03 \x01(\t\x12\x14\n\x0ctemplate_ern\x18\x04 \x01(\t\"F\n\x1a\x44\x65scribeCodeTemplateOutput\x12(\n\x08template\x18\x01 \x01(\x0b\x32\x16.eolymp.judge.Template\"h\n\x17LookupCodeTemplateInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x14\n\x0bproblem_ern\x18\xe7\x07 \x01(\t\x12\x0f\n\x07runtime\x18\n \x01(\t\"D\n\x18LookupCodeTemplateOutput\x12(\n\x08template\x18\x01 \x01(\x0b\x32\x16.eolymp.judge.Template\"\'\n\x11RebuildScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\")\n\x12RebuildScoreOutput\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\t\"*\n\x14IntrospectScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\";\n\x15IntrospectScoreOutput\x12\"\n\x05score\x18\x01 \x01(\x0b\x32\x13.eolymp.judge.Score\"\x85\x01\n\x12\x44\x65scribeScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12.\n\x04mode\x18\x03 \x01(\x0e\x32 .eolymp.judge.Score.FetchingMode\x12\x13\n\x0btime_offset\x18\x04 \x01(\x05\"9\n\x13\x44\x65scribeScoreOutput\x12\"\n\x05score\x18\x01 \x01(\x0b\x32\x13.eolymp.judge.Score\"c\n\x10ImportScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12#\n\x06scores\x18\n \x03(\x0b\x32\x13.eolymp.judge.Score\"\x13\n\x11ImportScoreOutput\">\n\x10\x45xportScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"8\n\x11\x45xportScoreOutput\x12#\n\x06scores\x18\n \x03(\x0b\x32\x13.eolymp.judge.Score\"\x88\x01\n\x0fListResultInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12.\n\x04mode\x18\x02 \x01(\x0e\x32 .eolymp.judge.Score.FetchingMode\x12\x13\n\x0btime_offset\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"F\n\x10ListResultOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12#\n\x05items\x18\x02 \x03(\x0b\x32\x14.eolymp.judge.Result\"\x80\x01\n\x15ListEntitlementsInput\x12\x14\n\ncontest_id\x18\x01 \x01(\tH\x00\x12\x17\n\rsubmission_id\x18\x02 \x01(\tH\x00\x12\x13\n\tticket_id\x18\x03 \x01(\tH\x00\x12\x18\n\x0eparticipant_id\x18\x04 \x01(\tH\x00\x42\t\n\x07\x63ontext\"I\n\x16ListEntitlementsOutput\x12/\n\x0c\x65ntitlements\x18\x01 \x03(\x0e\x32\x19.eolymp.judge.Entitlement\"G\n\x13ListActivitiesInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"L\n\x14ListActivitiesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12%\n\x05items\x18\x02 \x03(\x0b\x32\x16.eolymp.judge.Activity\"d\n\x18\x43onfigureAppearanceInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x34\n\nappearance\x18\x02 \x01(\x0b\x32 .eolymp.judge.Contest.Appearance\"\x1b\n\x19\x43onfigureAppearanceOutput\"-\n\x17\x44\x65scribeAppearanceInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"P\n\x18\x44\x65scribeAppearanceOutput\x12\x34\n\nappearance\x18\x01 \x01(\x0b\x32 .eolymp.judge.Contest.Appearance2\xfcj\n\x05Judge\x12\x80\x01\n\rLookupContest\x12 .eolymp.judge.LookupContestInput\x1a!.eolymp.judge.LookupContestOutput\"*\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02\x14\x12\x12/contests/__lookup\x12\x91\x01\n\rCreateContest\x12 .eolymp.judge.CreateContestInput\x1a!.eolymp.judge.CreateContestOutput\";\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7\xa3=\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0b\"\t/contests\x12\x9e\x01\n\rDeleteContest\x12 .eolymp.judge.DeleteContestInput\x1a!.eolymp.judge.DeleteContestOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18*\x16/contests/{contest_id}\x12\x9e\x01\n\rUpdateContest\x12 .eolymp.judge.UpdateContestInput\x1a!.eolymp.judge.UpdateContestOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18\x1a\x16/contests/{contest_id}\x12\x89\x01\n\x0f\x44\x65scribeContest\x12\".eolymp.judge.DescribeContestInput\x1a#.eolymp.judge.DescribeContestOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x18\x12\x16/contests/{contest_id}\x12s\n\x0cListContests\x12\x1f.eolymp.judge.ListContestsInput\x1a .eolymp.judge.ListContestsOutput\" \xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x0b\x12\t/contests\x12\x9d\x01\n\x0bOpenContest\x12\x1e.eolymp.judge.OpenContestInput\x1a\x1f.eolymp.judge.OpenContestOutput\"M\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1d\"\x1b/contests/{contest_id}/open\x12\xa1\x01\n\x0c\x43loseContest\x12\x1f.eolymp.judge.CloseContestInput\x1a .eolymp.judge.CloseContestOutput\"N\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1e\"\x1c/contests/{contest_id}/close\x12\xa9\x01\n\x0eSuspendContest\x12!.eolymp.judge.SuspendContestInput\x1a\".eolymp.judge.SuspendContestOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/suspend\x12\xa5\x01\n\rFreezeContest\x12 .eolymp.judge.FreezeContestInput\x1a!.eolymp.judge.FreezeContestOutput\"O\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1f\"\x1d/contests/{contest_id}/freeze\x12\xa5\x01\n\rResumeContest\x12 .eolymp.judge.ResumeContestInput\x1a!.eolymp.judge.ResumeContestOutput\"O\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1f\"\x1d/contests/{contest_id}/resume\x12\xaf\x01\n\x10\x43onfigureRuntime\x12#.eolymp.judge.ConfigureRuntimeInput\x1a$.eolymp.judge.ConfigureRuntimeOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/runtime\x12\xab\x01\n\x0f\x44\x65scribeRuntime\x12\".eolymp.judge.DescribeRuntimeInput\x1a#.eolymp.judge.DescribeRuntimeOutput\"O\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02 \x12\x1e/contests/{contest_id}/runtime\x12\xbb\x01\n\x13\x43onfigureAppearance\x12&.eolymp.judge.ConfigureAppearanceInput\x1a\'.eolymp.judge.ConfigureAppearanceOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02#\"!/contests/{contest_id}/appearance\x12\xb7\x01\n\x12\x44\x65scribeAppearance\x12%.eolymp.judge.DescribeAppearanceInput\x1a&.eolymp.judge.DescribeAppearanceOutput\"R\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02#\x12!/contests/{contest_id}/appearance\x12\xaf\x01\n\x10\x43onfigureScoring\x12#.eolymp.judge.ConfigureScoringInput\x1a$.eolymp.judge.ConfigureScoringOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/scoring\x12\xab\x01\n\x0f\x44\x65scribeScoring\x12\".eolymp.judge.DescribeScoringInput\x1a#.eolymp.judge.DescribeScoringOutput\"O\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02 \x12\x1e/contests/{contest_id}/scoring\x12\xa7\x01\n\rImportProblem\x12 .eolymp.judge.ImportProblemInput\x1a!.eolymp.judge.ImportProblemOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02!\"\x1f/contests/{contest_id}/problems\x12\xb3\x01\n\x0bSyncProblem\x12\x1e.eolymp.judge.SyncProblemInput\x1a\x1f.eolymp.judge.SyncProblemOutput\"c\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x33\"1/contests/{contest_id}/problems/{problem_id}/sync\x12\xb4\x01\n\rUpdateProblem\x12 .eolymp.judge.UpdateProblemInput\x1a!.eolymp.judge.UpdateProblemOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02.\",/contests/{contest_id}/problems/{problem_id}\x12\xa3\x01\n\x0cListProblems\x12\x1f.eolymp.judge.ListProblemsInput\x1a .eolymp.judge.ListProblemsOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00@@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02!\x12\x1f/contests/{contest_id}/problems\x12\xba\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.judge.DescribeProblemInput\x1a#.eolymp.judge.DescribeProblemOutput\"^\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02.\x12,/contests/{contest_id}/problems/{problem_id}\x12\xe0\x01\n\x14\x44\x65scribeCodeTemplate\x12\'.eolymp.judge.DescribeCodeTemplateInput\x1a(.eolymp.judge.DescribeCodeTemplateOutput\"u\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x46\x12\x44/contests/{contest_id}/problems/{problem_id}/templates/{template_id}\x12\xd2\x01\n\x12LookupCodeTemplate\x12%.eolymp.judge.LookupCodeTemplateInput\x1a&.eolymp.judge.LookupCodeTemplateOutput\"m\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02>\x12</contests/{contest_id}/problems/{problem_id}/lookup-template\x12\xc1\x01\n\x0eListStatements\x12!.eolymp.judge.ListStatementsInput\x1a\".eolymp.judge.ListStatementsOutput\"h\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x39\x12\x37/contests/{contest_id}/problems/{problem_id}/statements\x12\xc5\x01\n\x0fListAttachments\x12\".eolymp.judge.ListAttachmentsInput\x1a#.eolymp.judge.ListAttachmentsOutput\"i\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02:\x12\x38/contests/{contest_id}/problems/{problem_id}/attachments\x12\xb9\x01\n\x0cListExamples\x12\x1f.eolymp.judge.ListExamplesInput\x1a .eolymp.judge.ListExamplesOutput\"f\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x37\x12\x35/contests/{contest_id}/problems/{problem_id}/examples\x12\xb4\x01\n\rDeleteProblem\x12 .eolymp.judge.DeleteProblemInput\x1a!.eolymp.judge.DeleteProblemOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02.*,/contests/{contest_id}/problems/{problem_id}\x12\xbb\x01\n\rRetestProblem\x12 .eolymp.judge.RetestProblemInput\x1a!.eolymp.judge.RetestProblemOutput\"e\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x35\x12\x33/contests/{contest_id}/problems/{problem_id}/retest\x12\xae\x01\n\x0e\x41\x64\x64Participant\x12!.eolymp.judge.AddParticipantInput\x1a\".eolymp.judge.AddParticipantOutput\"U\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02%\"#/contests/{contest_id}/participants\x12\xcf\x01\n\x11\x45nableParticipant\x12$.eolymp.judge.EnableParticipantInput\x1a%.eolymp.judge.EnableParticipantOutput\"m\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02=\";/contests/{contest_id}/participants/{participant_id}/enable\x12\xd3\x01\n\x12\x44isableParticipant\x12%.eolymp.judge.DisableParticipantInput\x1a&.eolymp.judge.DisableParticipantOutput\"n\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02>\"</contests/{contest_id}/participants/{participant_id}/disable\x12\xc8\x01\n\x11UpdateParticipant\x12$.eolymp.judge.UpdateParticipantInput\x1a%.eolymp.judge.UpdateParticipantOutput\"f\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x36\x1a\x34/contests/{contest_id}/participants/{participant_id}\x12\xc8\x01\n\x11RemoveParticipant\x12$.eolymp.judge.RemoveParticipantInput\x1a%.eolymp.judge.RemoveParticipantOutput\"f\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x36*4/contests/{contest_id}/participants/{participant_id}\x12\xb3\x01\n\x10ListParticipants\x12#.eolymp.judge.ListParticipantsInput\x1a$.eolymp.judge.ListParticipantsOutput\"T\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02%\x12#/contests/{contest_id}/participants\x12\xce\x01\n\x13\x44\x65scribeParticipant\x12&.eolymp.judge.DescribeParticipantInput\x1a\'.eolymp.judge.DescribeParticipantOutput\"f\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02\x36\x12\x34/contests/{contest_id}/participants/{participant_id}\x12\xa6\x01\n\x15IntrospectParticipant\x12(.eolymp.judge.IntrospectParticipantInput\x1a).eolymp.judge.IntrospectParticipantOutput\"8\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02#\x12!/contests/{contest_id}/introspect\x12\x82\x01\n\x0bJoinContest\x12\x1e.eolymp.judge.JoinContestInput\x1a\x1f.eolymp.judge.JoinContestOutput\"2\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x03\x82\xd3\xe4\x93\x02\x1d\"\x1b/contests/{contest_id}/join\x12\xa7\x01\n\x0cStartContest\x12\x1f.eolymp.judge.StartContestInput\x1a .eolymp.judge.StartContestOutput\"T\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x03\x82\xd3\xe4\x93\x02\x1e\"\x1c/contests/{contest_id}/start\x12\xb0\x01\n\x0eVerifyPasscode\x12!.eolymp.judge.VerifyPasscodeInput\x1a\".eolymp.judge.VerifyPasscodeOutput\"W\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02(\"&/contests/{contest_id}/verify-passcode\x12\xb3\x01\n\rEnterPasscode\x12 .eolymp.judge.EnterPasscodeInput\x1a!.eolymp.judge.EnterPasscodeOutput\"]\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\'\"%/contests/{contest_id}/enter-passcode\x12\xc5\x01\n\rResetPasscode\x12 .eolymp.judge.ResetPasscodeInput\x1a!.eolymp.judge.ResetPasscodeOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02?\"=/contests/{contest_id}/participants/{participant_id}/passcode\x12\xbf\x01\n\x0bSetPasscode\x12\x1e.eolymp.judge.SetPasscodeInput\x1a\x1f.eolymp.judge.SetPasscodeOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02?\x1a=/contests/{contest_id}/participants/{participant_id}/passcode\x12\xc8\x01\n\x0eRemovePasscode\x12!.eolymp.judge.RemovePasscodeInput\x1a\".eolymp.judge.RemovePasscodeOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02?*=/contests/{contest_id}/participants/{participant_id}/passcode\x12\xcf\x01\n\x10\x43reateSubmission\x12#.eolymp.judge.CreateSubmissionInput\x1a$.eolymp.judge.CreateSubmissionOutput\"p\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\n\x82\xd3\xe4\x93\x02:\"8/contests/{contest_id}/problems/{problem_id}/submissions\x12\xaf\x01\n\x0fListSubmissions\x12\".eolymp.judge.ListSubmissionsInput\x1a#.eolymp.judge.ListSubmissionsOutput\"S\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02$\x12\"/contests/{contest_id}/submissions\x12\xc8\x01\n\x12\x44\x65scribeSubmission\x12%.eolymp.judge.DescribeSubmissionInput\x1a&.eolymp.judge.DescribeSubmissionOutput\"c\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x34\x12\x32/contests/{contest_id}/submissions/{submission_id}\x12\xca\x01\n\x10RetestSubmission\x12#.eolymp.judge.RetestSubmissionInput\x1a$.eolymp.judge.RetestSubmissionOutput\"k\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02;\"9/contests/{contest_id}/submissions/{submission_id}/retest\x12\xc3\x01\n\x10\x44\x65leteSubmission\x12#.eolymp.judge.DeleteSubmissionInput\x1a$.eolymp.judge.DeleteSubmissionOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x34*2/contests/{contest_id}/submissions/{submission_id}\x12\xce\x01\n\x11RestoreSubmission\x12$.eolymp.judge.RestoreSubmissionInput\x1a%.eolymp.judge.RestoreSubmissionOutput\"l\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02<\":/contests/{contest_id}/submissions/{submission_id}/restore\x12\xa9\x01\n\x0c\x43reateTicket\x12\x1f.eolymp.judge.CreateTicketInput\x1a .eolymp.judge.CreateTicketOutput\"V\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/tickets\x12\x9c\x01\n\x0b\x43loseTicket\x12\x1e.eolymp.judge.CloseTicketInput\x1a\x1f.eolymp.judge.CloseTicketOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c\"\x1a/tickets/{ticket_id}/close\x12\x98\x01\n\nOpenTicket\x12\x1d.eolymp.judge.OpenTicketInput\x1a\x1e.eolymp.judge.OpenTicketOutput\"K\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1b\"\x19/tickets/{ticket_id}/open\x12\x97\x01\n\nReadTicket\x12\x1d.eolymp.judge.ReadTicketInput\x1a\x1e.eolymp.judge.ReadTicketOutput\"J\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x1b\"\x19/tickets/{ticket_id}/read\x12\x99\x01\n\x0c\x44\x65leteTicket\x12\x1f.eolymp.judge.DeleteTicketInput\x1a .eolymp.judge.DeleteTicketOutput\"F\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x16*\x14/tickets/{ticket_id}\x12\x9e\x01\n\x0e\x44\x65scribeTicket\x12!.eolymp.judge.DescribeTicketInput\x1a\".eolymp.judge.DescribeTicketOutput\"E\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x16\x12\x14/tickets/{ticket_id}\x12\x89\x01\n\x0bListTickets\x12\x1e.eolymp.judge.ListTicketsInput\x1a\x1f.eolymp.judge.ListTicketsOutput\"9\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\x12\x08/tickets\x12\xa4\x01\n\x0bReplyTicket\x12\x1e.eolymp.judge.ReplyTicketInput\x1a\x1f.eolymp.judge.ReplyTicketOutput\"T\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1e\"\x1c/tickets/{ticket_id}/replies\x12\x9d\x01\n\x0bListReplies\x12\x1e.eolymp.judge.ListRepliesInput\x1a\x1f.eolymp.judge.ListRepliesOutput\"M\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1e\x12\x1c/tickets/{ticket_id}/replies\x12\xa9\x01\n\x0b\x44\x65leteReply\x12\x1e.eolymp.judge.DeleteReplyInput\x1a\x1f.eolymp.judge.DeleteReplyOutput\"Y\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02)*\'/tickets/{ticket_id}/replies/{reply_id}\x12\xa9\x01\n\x0bUpdateReply\x12\x1e.eolymp.judge.UpdateReplyInput\x1a\x1f.eolymp.judge.UpdateReplyOutput\"Y\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02)\"\'/tickets/{ticket_id}/replies/{reply_id}\x12\xbb\x01\n\x12\x43reateAnnouncement\x12%.eolymp.judge.CreateAnnouncementInput\x1a&.eolymp.judge.CreateAnnouncementOutput\"V\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02&\"$/contests/{contest_id}/announcements\x12\xcd\x01\n\x12UpdateAnnouncement\x12%.eolymp.judge.UpdateAnnouncementInput\x1a&.eolymp.judge.UpdateAnnouncementOutput\"h\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x38\"6/contests/{contest_id}/announcements/{announcement_id}\x12\xcd\x01\n\x12\x44\x65leteAnnouncement\x12%.eolymp.judge.DeleteAnnouncementInput\x1a&.eolymp.judge.DeleteAnnouncementOutput\"h\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x38*6/contests/{contest_id}/announcements/{announcement_id}\x12\xcb\x01\n\x10ReadAnnouncement\x12#.eolymp.judge.ReadAnnouncementInput\x1a$.eolymp.judge.ReadAnnouncementOutput\"l\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02=\";/contests/{contest_id}/announcements/{announcement_id}/read\x12\xd2\x01\n\x14\x44\x65scribeAnnouncement\x12\'.eolymp.judge.DescribeAnnouncementInput\x1a(.eolymp.judge.DescribeAnnouncementOutput\"g\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x38\x12\x36/contests/{contest_id}/announcements/{announcement_id}\x12\xeb\x01\n\x1a\x44\x65scribeAnnouncementStatus\x12-.eolymp.judge.DescribeAnnouncementStatusInput\x1a..eolymp.judge.DescribeAnnouncementStatusOutput\"n\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02?\x12=/contests/{contest_id}/announcements/{announcement_id}/status\x12\xb7\x01\n\x11ListAnnouncements\x12$.eolymp.judge.ListAnnouncementsInput\x1a%.eolymp.judge.ListAnnouncementsOutput\"U\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02&\x12$/contests/{contest_id}/announcements\x12\x9a\x01\n\x0fIntrospectScore\x12\".eolymp.judge.IntrospectScoreInput\x1a#.eolymp.judge.IntrospectScoreOutput\">\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02)\x12\'/contests/{contest_id}/introspect/score\x12\xc2\x01\n\rDescribeScore\x12 .eolymp.judge.DescribeScoreInput\x1a!.eolymp.judge.DescribeScoreOutput\"l\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02<\x12:/contests/{contest_id}/participants/{participant_id}/score\x12\xbd\x01\n\x0bImportScore\x12\x1e.eolymp.judge.ImportScoreInput\x1a\x1f.eolymp.judge.ImportScoreOutput\"m\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02=\";/contests/{contest_id}/participants/{participant_id}/scores\x12\xbd\x01\n\x0b\x45xportScore\x12\x1e.eolymp.judge.ExportScoreInput\x1a\x1f.eolymp.judge.ExportScoreOutput\"m\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02=\x12;/contests/{contest_id}/participants/{participant_id}/scores\x12\x9d\x01\n\nListResult\x12\x1d.eolymp.judge.ListResultInput\x1a\x1e.eolymp.judge.ListResultOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02 \x12\x1e/contests/{contest_id}/results\x12\xa3\x01\n\x0cRebuildScore\x12\x1f.eolymp.judge.RebuildScoreInput\x1a .eolymp.judge.RebuildScoreOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/rebuild\x12\x8b\x01\n\x10ListEntitlements\x12#.eolymp.judge.ListEntitlementsInput\x1a$.eolymp.judge.ListEntitlementsOutput\",\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x17\x12\x15/__judge/entitlements\x12\xab\x01\n\x0eListActivities\x12!.eolymp.judge.ListActivitiesInput\x1a\".eolymp.judge.ListActivitiesOutput\"R\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02#\x12!/contests/{contest_id}/activitiesB-Z+github.com/eolymp/go-sdk/eolymp/judge;judgeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x18\x65olymp/judge/judge.proto\x12\x0c\x65olymp.judge\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a\x1b\x65olymp/judge/activity.proto\x1a\x1f\x65olymp/judge/announcement.proto\x1a\x1a\x65olymp/judge/contest.proto\x1a\x1e\x65olymp/judge/participant.proto\x1a\x1a\x65olymp/judge/problem.proto\x1a\x18\x65olymp/judge/reply.proto\x1a\x19\x65olymp/judge/result.proto\x1a\x18\x65olymp/judge/score.proto\x1a\x1d\x65olymp/judge/submission.proto\x1a\x1b\x65olymp/judge/template.proto\x1a\x19\x65olymp/judge/ticket.proto\x1a eolymp/wellknown/direction.proto\x1a!eolymp/wellknown/expression.proto\"<\n\x12\x43reateContestInput\x12&\n\x07\x63ontest\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Contest\")\n\x13\x43reateContestOutput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"(\n\x12\x44\x65leteContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x15\n\x13\x44\x65leteContestOutput\"P\n\x12UpdateContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12&\n\x07\x63ontest\x18\x02 \x01(\x0b\x32\x15.eolymp.judge.Contest\"\x15\n\x13UpdateContestOutput\"*\n\x14\x44\x65scribeContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"?\n\x15\x44\x65scribeContestOutput\x12&\n\x07\x63ontest\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Contest\"!\n\x12LookupContestInput\x12\x0b\n\x03key\x18\x01 \x01(\t\"s\n\x13LookupContestOutput\x12&\n\x07\x63ontest\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Contest\x12\x34\n\nappearance\x18\x02 \x01(\x0b\x32 .eolymp.judge.Contest.Appearance\"\x8e\x04\n\x11ListContestsInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x37\n\x07\x66ilters\x18( \x01(\x0b\x32&.eolymp.judge.ListContestsInput.Filter\x1a\xa1\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12-\n\x03own\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x38\n\tstarts_at\x18\x04 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x36\n\x07\x65nds_at\x18\x05 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x30\n\x06public\x18\x06 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x34\n\nvisibility\x18\x07 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x06\x66ormat\x18\x08 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"I\n\x12ListContestsOutput\x12$\n\x05items\x18\x01 \x03(\x0b\x32\x15.eolymp.judge.Contest\x12\r\n\x05total\x18\x02 \x01(\x05\"&\n\x10OpenContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x13\n\x11OpenContestOutput\"\'\n\x11\x43loseContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x14\n\x12\x43loseContestOutput\")\n\x13SuspendContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x16\n\x14SuspendContestOutput\"(\n\x12\x46reezeContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x15\n\x13\x46reezeContestOutput\"(\n\x12ResumeContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x15\n\x13ResumeContestOutput\"&\n\x10JoinContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x13\n\x11JoinContestOutput\"\'\n\x11StartContestInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"\x14\n\x12StartContestOutput\"\x7f\n\x12ImportProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\timport_id\x18\x02 \x01(\t\x12\r\n\x05index\x18\n \x01(\r\x12\x14\n\x0csubmit_limit\x18\x0b \x01(\r\x12\x1d\n\x15score_by_best_testset\x18\x0c \x01(\x08\")\n\x13ImportProblemOutput\x12\x12\n\nproblem_id\x18\x02 \x01(\t\":\n\x10SyncProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"\x13\n\x11SyncProblemOutput\"\x80\x01\n\x12UpdateProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\r\n\x05index\x18\n \x01(\r\x12\x14\n\x0csubmit_limit\x18\x0b \x01(\r\x12\x1d\n\x15score_by_best_testset\x18\x0c \x01(\x08\"\x15\n\x13UpdateProblemOutput\"<\n\x12\x44\x65leteProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"\x15\n\x13\x44\x65leteProblemOutput\"<\n\x12RetestProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"\x15\n\x13RetestProblemOutput\"E\n\x11ListProblemsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"I\n\x12ListProblemsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12$\n\x05items\x18\x02 \x03(\x0b\x32\x15.eolymp.judge.Problem\"T\n\x14\x44\x65scribeProblemInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x14\n\x0bproblem_ern\x18\x8fN \x01(\t\"?\n\x15\x44\x65scribeProblemOutput\x12&\n\x07problem\x18\x01 \x01(\x0b\x32\x15.eolymp.judge.Problem\"=\n\x13ListStatementsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"U\n\x14ListStatementsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12.\n\x05items\x18\x02 \x03(\x0b\x32\x1f.eolymp.judge.Problem.Statement\">\n\x14ListAttachmentsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"W\n\x15ListAttachmentsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12/\n\x05items\x18\x02 \x03(\x0b\x32 .eolymp.judge.Problem.Attachment\";\n\x11ListExamplesInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\"N\n\x12ListExamplesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12)\n\x05items\x18\x02 \x03(\x0b\x32\x1a.eolymp.judge.Problem.Test\"f\n\x13\x41\x64\x64ParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tmember_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x1a\n\x12out_of_competition\x18\x04 \x01(\x08\".\n\x14\x41\x64\x64ParticipantOutput\x12\x16\n\x0eparticipant_id\x18\x01 \x01(\t\"D\n\x16\x45nableParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x19\n\x17\x45nableParticipantOutput\"E\n\x17\x44isableParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x1a\n\x18\x44isableParticipantOutput\"\x81\x02\n\x16UpdateParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12\x39\n\x05patch\x18\x03 \x01(\x0e\x32*.eolymp.judge.UpdateParticipantInput.Patch\x12\x0c\n\x04name\x18\n \x01(\t\x12\x12\n\nbonus_time\x18\x0c \x01(\r\x12\x1a\n\x12out_of_competition\x18\x0b \x01(\x08\"B\n\x05Patch\x12\x07\n\x03\x41LL\x10\x00\x12\x08\n\x04NAME\x10\x01\x12\x0e\n\nBONUS_TIME\x10\x03\x12\x16\n\x12OUT_OF_COMPETITION\x10\x04\"\x19\n\x17UpdateParticipantOutput\"D\n\x16RemoveParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x19\n\x17RemoveParticipantOutput\")\n\x13VerifyPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"7\n\x14VerifyPasscodeOutput\x12\x10\n\x08required\x18\x01 \x01(\x08\x12\r\n\x05valid\x18\x02 \x01(\x08\":\n\x12\x45nterPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x10\n\x08passcode\x18\x02 \x01(\t\"\x15\n\x13\x45nterPasscodeOutput\"@\n\x12ResetPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\'\n\x13ResetPasscodeOutput\x12\x10\n\x08passcode\x18\x01 \x01(\t\"P\n\x10SetPasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12\x10\n\x08passcode\x18\x03 \x01(\t\"\x13\n\x11SetPasscodeOutput\"A\n\x13RemovePasscodeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"\x16\n\x14RemovePasscodeOutput\"\xe8\x05\n\x15ListParticipantsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12;\n\x07\x66ilters\x18( \x01(\x0b\x32*.eolymp.judge.ListParticipantsInput.Filter\x12:\n\x04sort\x18\x32 \x01(\x0e\x32,.eolymp.judge.ListParticipantsInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\xa8\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x31\n\tmember_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x04name\x18\x08 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12\x30\n\x06status\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x05score\x18\x04 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x32\n\x07penalty\x18\x05 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x39\n\nstarted_at\x18\x06 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12:\n\x0b\x63omplete_at\x18\x07 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\"M\n\x08Sortable\x12\x08\n\x04RANK\x10\x00\x12\t\n\x05SCORE\x10\x01\x12\x0b\n\x07PENALTY\x10\x02\x12\x0e\n\nSTARTED_AT\x10\x03\x12\x0f\n\x0b\x43OMPLETE_AT\x10\x04\"Q\n\x16ListParticipantsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12(\n\x05items\x18\x02 \x03(\x0b\x32\x19.eolymp.judge.Participant\"0\n\x1aIntrospectParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"M\n\x1bIntrospectParticipantOutput\x12.\n\x0bparticipant\x18\x01 \x01(\x0b\x32\x19.eolymp.judge.Participant\"F\n\x18\x44\x65scribeParticipantInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"K\n\x19\x44\x65scribeParticipantOutput\x12.\n\x0bparticipant\x18\x01 \x01(\x0b\x32\x19.eolymp.judge.Participant\"]\n\x15\x43reateSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x0c\n\x04lang\x18\x03 \x01(\t\x12\x0e\n\x06source\x18\x04 \x01(\t\"/\n\x16\x43reateSubmissionOutput\x12\x15\n\rsubmission_id\x18\x01 \x01(\t\"\xe4\x04\n\x14ListSubmissionsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12:\n\x07\x66ilters\x18( \x01(\x0b\x32).eolymp.judge.ListSubmissionsInput.Filter\x1a\xdd\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x36\n\x0eparticipant_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x32\n\nproblem_id\x18\x03 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x06status\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12.\n\x04lang\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\x12\x30\n\x05score\x18\x06 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12\x35\n\npercentage\x18\x07 \x03(\x0b\x32!.eolymp.wellknown.ExpressionFloat\x12;\n\x0csubmitted_at\x18\x08 \x03(\x0b\x32%.eolymp.wellknown.ExpressionTimestamp\x12\x33\n\tsignature\x18\t \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"O\n\x15ListSubmissionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\'\n\x05items\x18\x02 \x03(\x0b\x32\x18.eolymp.judge.Submission\"D\n\x17\x44\x65scribeSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"H\n\x18\x44\x65scribeSubmissionOutput\x12,\n\nsubmission\x18\x01 \x01(\x0b\x32\x18.eolymp.judge.Submission\"B\n\x15RetestSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"\x18\n\x16RetestSubmissionOutput\"B\n\x15\x44\x65leteSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"\x18\n\x16\x44\x65leteSubmissionOutput\"C\n\x16RestoreSubmissionInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x15\n\rsubmission_id\x18\x02 \x01(\t\"\x19\n\x17RestoreSubmissionOutput\"I\n\x11\x43reateTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"\'\n\x12\x43reateTicketOutput\x12\x11\n\tticket_id\x18\x01 \x01(\t\"9\n\x10\x43loseTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x13\n\x11\x43loseTicketOutput\"8\n\x0fOpenTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x12\n\x10OpenTicketOutput\"8\n\x0fReadTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x12\n\x10ReadTicketOutput\":\n\x11\x44\x65leteTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"\x14\n\x12\x44\x65leteTicketOutput\"<\n\x13\x44\x65scribeTicketInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x11\n\tticket_id\x18\x02 \x01(\t\"<\n\x14\x44\x65scribeTicketOutput\x12$\n\x06ticket\x18\x01 \x01(\x0b\x32\x14.eolymp.judge.Ticket\"\x96\x05\n\x10ListTicketsInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x36\n\x07\x66ilters\x18( \x01(\x0b\x32%.eolymp.judge.ListTicketsInput.Filter\x12\x35\n\x04sort\x18\x32 \x01(\x0e\x32\'.eolymp.judge.ListTicketsInput.Sortable\x12*\n\x05order\x18\x33 \x01(\x0e\x32\x1b.eolymp.wellknown.Direction\x1a\x80\x03\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x32\n\ncontest_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x36\n\x0eparticipant_id\x18\x03 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12@\n\x16is_read_by_participant\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12:\n\x10is_read_by_owner\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x31\n\x07is_open\x18\x06 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12-\n\x03own\x18\x07 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"F\n\x08Sortable\x12\x0e\n\nCREATED_AT\x10\x00\x12\x11\n\rREAD_BY_OWNER\x10\x01\x12\x17\n\x13READ_BY_PARTICIPANT\x10\x02\"G\n\x11ListTicketsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12#\n\x05items\x18\x02 \x03(\x0b\x32\x14.eolymp.judge.Ticket\"E\n\x10ReplyTicketInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x0f\n\x07message\x18\n \x01(\t\x12\r\n\x05\x63lose\x18\x15 \x01(\x08\"%\n\x11ReplyTicketOutput\x12\x10\n\x08reply_id\x18\x01 \x01(\t\"C\n\x10ListRepliesInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"F\n\x11ListRepliesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12\"\n\x05items\x18\x02 \x03(\x0b\x32\x13.eolymp.judge.Reply\"7\n\x10\x44\x65leteReplyInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x10\n\x08reply_id\x18\x02 \x01(\t\"\x13\n\x11\x44\x65leteReplyOutput\"H\n\x10UpdateReplyInput\x12\x11\n\tticket_id\x18\x01 \x01(\t\x12\x10\n\x08reply_id\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t\"\x13\n\x11UpdateReplyOutput\"<\n\x15\x43onfigureRuntimeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0f\n\x07runtime\x18\x02 \x03(\t\"\x18\n\x16\x43onfigureRuntimeOutput\"*\n\x14\x44\x65scribeRuntimeInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"(\n\x15\x44\x65scribeRuntimeOutput\x12\x0f\n\x07runtime\x18\x01 \x03(\t\"[\n\x15\x43onfigureScoringInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12.\n\x07scoring\x18\x02 \x01(\x0b\x32\x1d.eolymp.judge.Contest.Scoring\"\x18\n\x16\x43onfigureScoringOutput\"*\n\x14\x44\x65scribeScoringInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"G\n\x15\x44\x65scribeScoringOutput\x12.\n\x07scoring\x18\x01 \x01(\x0b\x32\x1d.eolymp.judge.Contest.Scoring\"_\n\x17\x43reateAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x30\n\x0c\x61nnouncement\x18\x02 \x01(\x0b\x32\x1a.eolymp.judge.Announcement\"&\n\x18\x43reateAnnouncementOutput\x12\n\n\x02id\x18\x01 \x01(\t\"x\n\x17UpdateAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\x12\x30\n\x0c\x61nnouncement\x18\x03 \x01(\x0b\x32\x1a.eolymp.judge.Announcement\"\x1a\n\x18UpdateAnnouncementOutput\"F\n\x17\x44\x65leteAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"\x1a\n\x18\x44\x65leteAnnouncementOutput\"D\n\x15ReadAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"\x18\n\x16ReadAnnouncementOutput\"H\n\x19\x44\x65scribeAnnouncementInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"N\n\x1a\x44\x65scribeAnnouncementOutput\x12\x30\n\x0c\x61nnouncement\x18\x01 \x01(\x0b\x32\x1a.eolymp.judge.Announcement\"N\n\x1f\x44\x65scribeAnnouncementStatusInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x17\n\x0f\x61nnouncement_id\x18\x02 \x01(\t\"3\n DescribeAnnouncementStatusOutput\x12\x0f\n\x07is_read\x18\x01 \x01(\x08\"\xf1\x01\n\x16ListAnnouncementsInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12<\n\x07\x66ilters\x18( \x01(\x0b\x32+.eolymp.judge.ListAnnouncementsInput.Filter\x1ag\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x31\n\x07is_read\x18\x02 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"S\n\x17ListAnnouncementsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12)\n\x05items\x18\x02 \x03(\x0b\x32\x1a.eolymp.judge.Announcement\"n\n\x19\x44\x65scribeCodeTemplateInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x13\n\x0btemplate_id\x18\x03 \x01(\t\x12\x14\n\x0ctemplate_ern\x18\x04 \x01(\t\"F\n\x1a\x44\x65scribeCodeTemplateOutput\x12(\n\x08template\x18\x01 \x01(\x0b\x32\x16.eolymp.judge.Template\"h\n\x17LookupCodeTemplateInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x14\n\x0bproblem_ern\x18\xe7\x07 \x01(\t\x12\x0f\n\x07runtime\x18\n \x01(\t\"D\n\x18LookupCodeTemplateOutput\x12(\n\x08template\x18\x01 \x01(\x0b\x32\x16.eolymp.judge.Template\"\'\n\x11RebuildScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\")\n\x12RebuildScoreOutput\x12\x13\n\x0b\x61\x63tivity_id\x18\x01 \x01(\t\"*\n\x14IntrospectScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\";\n\x15IntrospectScoreOutput\x12\"\n\x05score\x18\x01 \x01(\x0b\x32\x13.eolymp.judge.Score\"\x85\x01\n\x12\x44\x65scribeScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12.\n\x04mode\x18\x03 \x01(\x0e\x32 .eolymp.judge.Score.FetchingMode\x12\x13\n\x0btime_offset\x18\x04 \x01(\x05\"9\n\x13\x44\x65scribeScoreOutput\x12\"\n\x05score\x18\x01 \x01(\x0b\x32\x13.eolymp.judge.Score\"c\n\x10ImportScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\x12#\n\x06scores\x18\n \x03(\x0b\x32\x13.eolymp.judge.Score\"\x13\n\x11ImportScoreOutput\">\n\x10\x45xportScoreInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x16\n\x0eparticipant_id\x18\x02 \x01(\t\"8\n\x11\x45xportScoreOutput\x12#\n\x06scores\x18\n \x03(\x0b\x32\x13.eolymp.judge.Score\"\x88\x01\n\x0fListResultInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12.\n\x04mode\x18\x02 \x01(\x0e\x32 .eolymp.judge.Score.FetchingMode\x12\x13\n\x0btime_offset\x18\x03 \x01(\x05\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"F\n\x10ListResultOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12#\n\x05items\x18\x02 \x03(\x0b\x32\x14.eolymp.judge.Result\"G\n\x13ListActivitiesInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\"L\n\x14ListActivitiesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12%\n\x05items\x18\x02 \x03(\x0b\x32\x16.eolymp.judge.Activity\"d\n\x18\x43onfigureAppearanceInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\x12\x34\n\nappearance\x18\x02 \x01(\x0b\x32 .eolymp.judge.Contest.Appearance\"\x1b\n\x19\x43onfigureAppearanceOutput\"-\n\x17\x44\x65scribeAppearanceInput\x12\x12\n\ncontest_id\x18\x01 \x01(\t\"P\n\x18\x44\x65scribeAppearanceOutput\x12\x34\n\nappearance\x18\x01 \x01(\x0b\x32 .eolymp.judge.Contest.Appearance2\xeei\n\x05Judge\x12\x80\x01\n\rLookupContest\x12 .eolymp.judge.LookupContestInput\x1a!.eolymp.judge.LookupContestOutput\"*\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02\x14\x12\x12/contests/__lookup\x12\x91\x01\n\rCreateContest\x12 .eolymp.judge.CreateContestInput\x1a!.eolymp.judge.CreateContestOutput\";\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7\xa3=\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x0b\"\t/contests\x12\x9e\x01\n\rDeleteContest\x12 .eolymp.judge.DeleteContestInput\x1a!.eolymp.judge.DeleteContestOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18*\x16/contests/{contest_id}\x12\x9e\x01\n\rUpdateContest\x12 .eolymp.judge.UpdateContestInput\x1a!.eolymp.judge.UpdateContestOutput\"H\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x18\x1a\x16/contests/{contest_id}\x12\x89\x01\n\x0f\x44\x65scribeContest\x12\".eolymp.judge.DescribeContestInput\x1a#.eolymp.judge.DescribeContestOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x18\x12\x16/contests/{contest_id}\x12s\n\x0cListContests\x12\x1f.eolymp.judge.ListContestsInput\x1a .eolymp.judge.ListContestsOutput\" \xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x0b\x12\t/contests\x12\x9d\x01\n\x0bOpenContest\x12\x1e.eolymp.judge.OpenContestInput\x1a\x1f.eolymp.judge.OpenContestOutput\"M\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1d\"\x1b/contests/{contest_id}/open\x12\xa1\x01\n\x0c\x43loseContest\x12\x1f.eolymp.judge.CloseContestInput\x1a .eolymp.judge.CloseContestOutput\"N\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1e\"\x1c/contests/{contest_id}/close\x12\xa9\x01\n\x0eSuspendContest\x12!.eolymp.judge.SuspendContestInput\x1a\".eolymp.judge.SuspendContestOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/suspend\x12\xa5\x01\n\rFreezeContest\x12 .eolymp.judge.FreezeContestInput\x1a!.eolymp.judge.FreezeContestOutput\"O\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1f\"\x1d/contests/{contest_id}/freeze\x12\xa5\x01\n\rResumeContest\x12 .eolymp.judge.ResumeContestInput\x1a!.eolymp.judge.ResumeContestOutput\"O\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1f\"\x1d/contests/{contest_id}/resume\x12\xaf\x01\n\x10\x43onfigureRuntime\x12#.eolymp.judge.ConfigureRuntimeInput\x1a$.eolymp.judge.ConfigureRuntimeOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/runtime\x12\xab\x01\n\x0f\x44\x65scribeRuntime\x12\".eolymp.judge.DescribeRuntimeInput\x1a#.eolymp.judge.DescribeRuntimeOutput\"O\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02 \x12\x1e/contests/{contest_id}/runtime\x12\xbb\x01\n\x13\x43onfigureAppearance\x12&.eolymp.judge.ConfigureAppearanceInput\x1a\'.eolymp.judge.ConfigureAppearanceOutput\"S\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02#\"!/contests/{contest_id}/appearance\x12\xb7\x01\n\x12\x44\x65scribeAppearance\x12%.eolymp.judge.DescribeAppearanceInput\x1a&.eolymp.judge.DescribeAppearanceOutput\"R\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02#\x12!/contests/{contest_id}/appearance\x12\xaf\x01\n\x10\x43onfigureScoring\x12#.eolymp.judge.ConfigureScoringInput\x1a$.eolymp.judge.ConfigureScoringOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/scoring\x12\xab\x01\n\x0f\x44\x65scribeScoring\x12\".eolymp.judge.DescribeScoringInput\x1a#.eolymp.judge.DescribeScoringOutput\"O\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02 \x12\x1e/contests/{contest_id}/scoring\x12\xa7\x01\n\rImportProblem\x12 .eolymp.judge.ImportProblemInput\x1a!.eolymp.judge.ImportProblemOutput\"Q\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02!\"\x1f/contests/{contest_id}/problems\x12\xb3\x01\n\x0bSyncProblem\x12\x1e.eolymp.judge.SyncProblemInput\x1a\x1f.eolymp.judge.SyncProblemOutput\"c\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x33\"1/contests/{contest_id}/problems/{problem_id}/sync\x12\xb4\x01\n\rUpdateProblem\x12 .eolymp.judge.UpdateProblemInput\x1a!.eolymp.judge.UpdateProblemOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02.\",/contests/{contest_id}/problems/{problem_id}\x12\xa3\x01\n\x0cListProblems\x12\x1f.eolymp.judge.ListProblemsInput\x1a .eolymp.judge.ListProblemsOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00@@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02!\x12\x1f/contests/{contest_id}/problems\x12\xba\x01\n\x0f\x44\x65scribeProblem\x12\".eolymp.judge.DescribeProblemInput\x1a#.eolymp.judge.DescribeProblemOutput\"^\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02.\x12,/contests/{contest_id}/problems/{problem_id}\x12\xe0\x01\n\x14\x44\x65scribeCodeTemplate\x12\'.eolymp.judge.DescribeCodeTemplateInput\x1a(.eolymp.judge.DescribeCodeTemplateOutput\"u\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x46\x12\x44/contests/{contest_id}/problems/{problem_id}/templates/{template_id}\x12\xd2\x01\n\x12LookupCodeTemplate\x12%.eolymp.judge.LookupCodeTemplateInput\x1a&.eolymp.judge.LookupCodeTemplateOutput\"m\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02>\x12</contests/{contest_id}/problems/{problem_id}/lookup-template\x12\xc1\x01\n\x0eListStatements\x12!.eolymp.judge.ListStatementsInput\x1a\".eolymp.judge.ListStatementsOutput\"h\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x39\x12\x37/contests/{contest_id}/problems/{problem_id}/statements\x12\xc5\x01\n\x0fListAttachments\x12\".eolymp.judge.ListAttachmentsInput\x1a#.eolymp.judge.ListAttachmentsOutput\"i\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02:\x12\x38/contests/{contest_id}/problems/{problem_id}/attachments\x12\xb9\x01\n\x0cListExamples\x12\x1f.eolymp.judge.ListExamplesInput\x1a .eolymp.judge.ListExamplesOutput\"f\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0\x41\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x37\x12\x35/contests/{contest_id}/problems/{problem_id}/examples\x12\xb4\x01\n\rDeleteProblem\x12 .eolymp.judge.DeleteProblemInput\x1a!.eolymp.judge.DeleteProblemOutput\"^\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02.*,/contests/{contest_id}/problems/{problem_id}\x12\xbb\x01\n\rRetestProblem\x12 .eolymp.judge.RetestProblemInput\x1a!.eolymp.judge.RetestProblemOutput\"e\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x35\x12\x33/contests/{contest_id}/problems/{problem_id}/retest\x12\xae\x01\n\x0e\x41\x64\x64Participant\x12!.eolymp.judge.AddParticipantInput\x1a\".eolymp.judge.AddParticipantOutput\"U\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02%\"#/contests/{contest_id}/participants\x12\xcf\x01\n\x11\x45nableParticipant\x12$.eolymp.judge.EnableParticipantInput\x1a%.eolymp.judge.EnableParticipantOutput\"m\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02=\";/contests/{contest_id}/participants/{participant_id}/enable\x12\xd3\x01\n\x12\x44isableParticipant\x12%.eolymp.judge.DisableParticipantInput\x1a&.eolymp.judge.DisableParticipantOutput\"n\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02>\"</contests/{contest_id}/participants/{participant_id}/disable\x12\xc8\x01\n\x11UpdateParticipant\x12$.eolymp.judge.UpdateParticipantInput\x1a%.eolymp.judge.UpdateParticipantOutput\"f\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x36\x1a\x34/contests/{contest_id}/participants/{participant_id}\x12\xc8\x01\n\x11RemoveParticipant\x12$.eolymp.judge.RemoveParticipantInput\x1a%.eolymp.judge.RemoveParticipantOutput\"f\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x36*4/contests/{contest_id}/participants/{participant_id}\x12\xb3\x01\n\x10ListParticipants\x12#.eolymp.judge.ListParticipantsInput\x1a$.eolymp.judge.ListParticipantsOutput\"T\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02%\x12#/contests/{contest_id}/participants\x12\xce\x01\n\x13\x44\x65scribeParticipant\x12&.eolymp.judge.DescribeParticipantInput\x1a\'.eolymp.judge.DescribeParticipantOutput\"f\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02\x36\x12\x34/contests/{contest_id}/participants/{participant_id}\x12\xa6\x01\n\x15IntrospectParticipant\x12(.eolymp.judge.IntrospectParticipantInput\x1a).eolymp.judge.IntrospectParticipantOutput\"8\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02#\x12!/contests/{contest_id}/introspect\x12\x82\x01\n\x0bJoinContest\x12\x1e.eolymp.judge.JoinContestInput\x1a\x1f.eolymp.judge.JoinContestOutput\"2\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x03\x82\xd3\xe4\x93\x02\x1d\"\x1b/contests/{contest_id}/join\x12\xa7\x01\n\x0cStartContest\x12\x1f.eolymp.judge.StartContestInput\x1a .eolymp.judge.StartContestOutput\"T\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x03\x82\xd3\xe4\x93\x02\x1e\"\x1c/contests/{contest_id}/start\x12\xb0\x01\n\x0eVerifyPasscode\x12!.eolymp.judge.VerifyPasscodeInput\x1a\".eolymp.judge.VerifyPasscodeOutput\"W\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02(\"&/contests/{contest_id}/verify-passcode\x12\xb3\x01\n\rEnterPasscode\x12 .eolymp.judge.EnterPasscodeInput\x1a!.eolymp.judge.EnterPasscodeOutput\"]\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\'\"%/contests/{contest_id}/enter-passcode\x12\xc5\x01\n\rResetPasscode\x12 .eolymp.judge.ResetPasscodeInput\x1a!.eolymp.judge.ResetPasscodeOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02?\"=/contests/{contest_id}/participants/{participant_id}/passcode\x12\xbf\x01\n\x0bSetPasscode\x12\x1e.eolymp.judge.SetPasscodeInput\x1a\x1f.eolymp.judge.SetPasscodeOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02?\x1a=/contests/{contest_id}/participants/{participant_id}/passcode\x12\xc8\x01\n\x0eRemovePasscode\x12!.eolymp.judge.RemovePasscodeInput\x1a\".eolymp.judge.RemovePasscodeOutput\"o\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02?*=/contests/{contest_id}/participants/{participant_id}/passcode\x12\xcf\x01\n\x10\x43reateSubmission\x12#.eolymp.judge.CreateSubmissionInput\x1a$.eolymp.judge.CreateSubmissionOutput\"p\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\n\x82\xd3\xe4\x93\x02:\"8/contests/{contest_id}/problems/{problem_id}/submissions\x12\xaf\x01\n\x0fListSubmissions\x12\".eolymp.judge.ListSubmissionsInput\x1a#.eolymp.judge.ListSubmissionsOutput\"S\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02$\x12\"/contests/{contest_id}/submissions\x12\xc8\x01\n\x12\x44\x65scribeSubmission\x12%.eolymp.judge.DescribeSubmissionInput\x1a&.eolymp.judge.DescribeSubmissionOutput\"c\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x34\x12\x32/contests/{contest_id}/submissions/{submission_id}\x12\xca\x01\n\x10RetestSubmission\x12#.eolymp.judge.RetestSubmissionInput\x1a$.eolymp.judge.RetestSubmissionOutput\"k\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02;\"9/contests/{contest_id}/submissions/{submission_id}/retest\x12\xc3\x01\n\x10\x44\x65leteSubmission\x12#.eolymp.judge.DeleteSubmissionInput\x1a$.eolymp.judge.DeleteSubmissionOutput\"d\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02\x34*2/contests/{contest_id}/submissions/{submission_id}\x12\xce\x01\n\x11RestoreSubmission\x12$.eolymp.judge.RestoreSubmissionInput\x1a%.eolymp.judge.RestoreSubmissionOutput\"l\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02<\":/contests/{contest_id}/submissions/{submission_id}/restore\x12\xa9\x01\n\x0c\x43reateTicket\x12\x1f.eolymp.judge.CreateTicketInput\x1a .eolymp.judge.CreateTicketOutput\"V\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/tickets\x12\x9c\x01\n\x0b\x43loseTicket\x12\x1e.eolymp.judge.CloseTicketInput\x1a\x1f.eolymp.judge.CloseTicketOutput\"L\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1c\"\x1a/tickets/{ticket_id}/close\x12\x98\x01\n\nOpenTicket\x12\x1d.eolymp.judge.OpenTicketInput\x1a\x1e.eolymp.judge.OpenTicketOutput\"K\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1b\"\x19/tickets/{ticket_id}/open\x12\x97\x01\n\nReadTicket\x12\x1d.eolymp.judge.ReadTicketInput\x1a\x1e.eolymp.judge.ReadTicketOutput\"J\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x1b\"\x19/tickets/{ticket_id}/read\x12\x99\x01\n\x0c\x44\x65leteTicket\x12\x1f.eolymp.judge.DeleteTicketInput\x1a .eolymp.judge.DeleteTicketOutput\"F\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x16*\x14/tickets/{ticket_id}\x12\x9e\x01\n\x0e\x44\x65scribeTicket\x12!.eolymp.judge.DescribeTicketInput\x1a\".eolymp.judge.DescribeTicketOutput\"E\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x16\x12\x14/tickets/{ticket_id}\x12\x89\x01\n\x0bListTickets\x12\x1e.eolymp.judge.ListTicketsInput\x1a\x1f.eolymp.judge.ListTicketsOutput\"9\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\n\x12\x08/tickets\x12\xa4\x01\n\x0bReplyTicket\x12\x1e.eolymp.judge.ReplyTicketInput\x1a\x1f.eolymp.judge.ReplyTicketOutput\"T\x82\xe3\n\x1d\x8a\xe3\n\x19judge:contest:participate\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x1e\"\x1c/tickets/{ticket_id}/replies\x12\x9d\x01\n\x0bListReplies\x12\x1e.eolymp.judge.ListRepliesInput\x1a\x1f.eolymp.judge.ListRepliesOutput\"M\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\x1e\x12\x1c/tickets/{ticket_id}/replies\x12\xa9\x01\n\x0b\x44\x65leteReply\x12\x1e.eolymp.judge.DeleteReplyInput\x1a\x1f.eolymp.judge.DeleteReplyOutput\"Y\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02)*\'/tickets/{ticket_id}/replies/{reply_id}\x12\xa9\x01\n\x0bUpdateReply\x12\x1e.eolymp.judge.UpdateReplyInput\x1a\x1f.eolymp.judge.UpdateReplyOutput\"Y\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\n\xd7#>\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02)\"\'/tickets/{ticket_id}/replies/{reply_id}\x12\xbb\x01\n\x12\x43reateAnnouncement\x12%.eolymp.judge.CreateAnnouncementInput\x1a&.eolymp.judge.CreateAnnouncementOutput\"V\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02&\"$/contests/{contest_id}/announcements\x12\xcd\x01\n\x12UpdateAnnouncement\x12%.eolymp.judge.UpdateAnnouncementInput\x1a&.eolymp.judge.UpdateAnnouncementOutput\"h\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x38\"6/contests/{contest_id}/announcements/{announcement_id}\x12\xcd\x01\n\x12\x44\x65leteAnnouncement\x12%.eolymp.judge.DeleteAnnouncementInput\x1a&.eolymp.judge.DeleteAnnouncementOutput\"h\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x38*6/contests/{contest_id}/announcements/{announcement_id}\x12\xcb\x01\n\x10ReadAnnouncement\x12#.eolymp.judge.ReadAnnouncementInput\x1a$.eolymp.judge.ReadAnnouncementOutput\"l\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02=\";/contests/{contest_id}/announcements/{announcement_id}/read\x12\xd2\x01\n\x14\x44\x65scribeAnnouncement\x12\'.eolymp.judge.DescribeAnnouncementInput\x1a(.eolymp.judge.DescribeAnnouncementOutput\"g\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x38\x12\x36/contests/{contest_id}/announcements/{announcement_id}\x12\xeb\x01\n\x1a\x44\x65scribeAnnouncementStatus\x12-.eolymp.judge.DescribeAnnouncementStatusInput\x1a..eolymp.judge.DescribeAnnouncementStatusOutput\"n\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02?\x12=/contests/{contest_id}/announcements/{announcement_id}/status\x12\xb7\x01\n\x11ListAnnouncements\x12$.eolymp.judge.ListAnnouncementsInput\x1a%.eolymp.judge.ListAnnouncementsOutput\"U\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02&\x12$/contests/{contest_id}/announcements\x12\x9a\x01\n\x0fIntrospectScore\x12\".eolymp.judge.IntrospectScoreInput\x1a#.eolymp.judge.IntrospectScoreOutput\">\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02)\x12\'/contests/{contest_id}/introspect/score\x12\xc2\x01\n\rDescribeScore\x12 .eolymp.judge.DescribeScoreInput\x1a!.eolymp.judge.DescribeScoreOutput\"l\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02<\x12:/contests/{contest_id}/participants/{participant_id}/score\x12\xbd\x01\n\x0bImportScore\x12\x1e.eolymp.judge.ImportScoreInput\x1a\x1f.eolymp.judge.ImportScoreOutput\"m\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02=\";/contests/{contest_id}/participants/{participant_id}/scores\x12\xbd\x01\n\x0b\x45xportScore\x12\x1e.eolymp.judge.ExportScoreInput\x1a\x1f.eolymp.judge.ExportScoreOutput\"m\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02=\x12;/contests/{contest_id}/participants/{participant_id}/scores\x12\x9d\x01\n\nListResult\x12\x1d.eolymp.judge.ListResultInput\x1a\x1e.eolymp.judge.ListResultOutput\"P\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0c\xf5\xe2\n\x00\x00HB\xf8\xe2\n\xc8\x01\x82\xd3\xe4\x93\x02 \x12\x1e/contests/{contest_id}/results\x12\xa3\x01\n\x0cRebuildScore\x12\x1f.eolymp.judge.RebuildScoreInput\x1a .eolymp.judge.RebuildScoreOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13judge:contest:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02 \"\x1e/contests/{contest_id}/rebuild\x12\xab\x01\n\x0eListActivities\x12!.eolymp.judge.ListActivitiesInput\x1a\".eolymp.judge.ListActivitiesOutput\"R\x82\xe3\n\x16\x8a\xe3\n\x12judge:contest:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02#\x12!/contests/{contest_id}/activitiesB-Z+github.com/eolymp/go-sdk/eolymp/judge;judgeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.judge.judge_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/judge;judge'
@@ -182,334 +181,328 @@
   _JUDGE.methods_by_name['ImportScore']._serialized_options = b'\202\343\n\026\212\343\n\022judge:contest:read\352\342\n\014\365\342\n\000\000HB\370\342\n\310\001\202\323\344\223\002=\";/contests/{contest_id}/participants/{participant_id}/scores'
   _JUDGE.methods_by_name['ExportScore']._options = None
   _JUDGE.methods_by_name['ExportScore']._serialized_options = b'\202\343\n\026\212\343\n\022judge:contest:read\352\342\n\014\365\342\n\000\000HB\370\342\n\310\001\202\323\344\223\002=\022;/contests/{contest_id}/participants/{participant_id}/scores'
   _JUDGE.methods_by_name['ListResult']._options = None
   _JUDGE.methods_by_name['ListResult']._serialized_options = b'\202\343\n\026\212\343\n\022judge:contest:read\352\342\n\014\365\342\n\000\000HB\370\342\n\310\001\202\323\344\223\002 \022\036/contests/{contest_id}/results'
   _JUDGE.methods_by_name['RebuildScore']._options = None
   _JUDGE.methods_by_name['RebuildScore']._serialized_options = b'\202\343\n\027\212\343\n\023judge:contest:write\352\342\n\013\365\342\n\000\000\000@\370\342\n\n\202\323\344\223\002 \"\036/contests/{contest_id}/rebuild'
-  _JUDGE.methods_by_name['ListEntitlements']._options = None
-  _JUDGE.methods_by_name['ListEntitlements']._serialized_options = b'\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002\027\022\025/__judge/entitlements'
   _JUDGE.methods_by_name['ListActivities']._options = None
   _JUDGE.methods_by_name['ListActivities']._serialized_options = b'\202\343\n\026\212\343\n\022judge:contest:read\352\342\n\013\365\342\n\000\000\240@\370\342\n\024\202\323\344\223\002#\022!/contests/{contest_id}/activities'
-  _CREATECONTESTINPUT._serialized_start=558
-  _CREATECONTESTINPUT._serialized_end=618
-  _CREATECONTESTOUTPUT._serialized_start=620
-  _CREATECONTESTOUTPUT._serialized_end=661
-  _DELETECONTESTINPUT._serialized_start=663
-  _DELETECONTESTINPUT._serialized_end=703
-  _DELETECONTESTOUTPUT._serialized_start=705
-  _DELETECONTESTOUTPUT._serialized_end=726
-  _UPDATECONTESTINPUT._serialized_start=728
-  _UPDATECONTESTINPUT._serialized_end=808
-  _UPDATECONTESTOUTPUT._serialized_start=810
-  _UPDATECONTESTOUTPUT._serialized_end=831
-  _DESCRIBECONTESTINPUT._serialized_start=833
-  _DESCRIBECONTESTINPUT._serialized_end=875
-  _DESCRIBECONTESTOUTPUT._serialized_start=877
-  _DESCRIBECONTESTOUTPUT._serialized_end=940
-  _LOOKUPCONTESTINPUT._serialized_start=942
-  _LOOKUPCONTESTINPUT._serialized_end=975
-  _LOOKUPCONTESTOUTPUT._serialized_start=977
-  _LOOKUPCONTESTOUTPUT._serialized_end=1092
-  _LISTCONTESTSINPUT._serialized_start=1095
-  _LISTCONTESTSINPUT._serialized_end=1621
-  _LISTCONTESTSINPUT_FILTER._serialized_start=1204
-  _LISTCONTESTSINPUT_FILTER._serialized_end=1621
-  _LISTCONTESTSOUTPUT._serialized_start=1623
-  _LISTCONTESTSOUTPUT._serialized_end=1696
-  _OPENCONTESTINPUT._serialized_start=1698
-  _OPENCONTESTINPUT._serialized_end=1736
-  _OPENCONTESTOUTPUT._serialized_start=1738
-  _OPENCONTESTOUTPUT._serialized_end=1757
-  _CLOSECONTESTINPUT._serialized_start=1759
-  _CLOSECONTESTINPUT._serialized_end=1798
-  _CLOSECONTESTOUTPUT._serialized_start=1800
-  _CLOSECONTESTOUTPUT._serialized_end=1820
-  _SUSPENDCONTESTINPUT._serialized_start=1822
-  _SUSPENDCONTESTINPUT._serialized_end=1863
-  _SUSPENDCONTESTOUTPUT._serialized_start=1865
-  _SUSPENDCONTESTOUTPUT._serialized_end=1887
-  _FREEZECONTESTINPUT._serialized_start=1889
-  _FREEZECONTESTINPUT._serialized_end=1929
-  _FREEZECONTESTOUTPUT._serialized_start=1931
-  _FREEZECONTESTOUTPUT._serialized_end=1952
-  _RESUMECONTESTINPUT._serialized_start=1954
-  _RESUMECONTESTINPUT._serialized_end=1994
-  _RESUMECONTESTOUTPUT._serialized_start=1996
-  _RESUMECONTESTOUTPUT._serialized_end=2017
-  _JOINCONTESTINPUT._serialized_start=2019
-  _JOINCONTESTINPUT._serialized_end=2057
-  _JOINCONTESTOUTPUT._serialized_start=2059
-  _JOINCONTESTOUTPUT._serialized_end=2078
-  _STARTCONTESTINPUT._serialized_start=2080
-  _STARTCONTESTINPUT._serialized_end=2119
-  _STARTCONTESTOUTPUT._serialized_start=2121
-  _STARTCONTESTOUTPUT._serialized_end=2141
-  _IMPORTPROBLEMINPUT._serialized_start=2143
-  _IMPORTPROBLEMINPUT._serialized_end=2270
-  _IMPORTPROBLEMOUTPUT._serialized_start=2272
-  _IMPORTPROBLEMOUTPUT._serialized_end=2313
-  _SYNCPROBLEMINPUT._serialized_start=2315
-  _SYNCPROBLEMINPUT._serialized_end=2373
-  _SYNCPROBLEMOUTPUT._serialized_start=2375
-  _SYNCPROBLEMOUTPUT._serialized_end=2394
-  _UPDATEPROBLEMINPUT._serialized_start=2397
-  _UPDATEPROBLEMINPUT._serialized_end=2525
-  _UPDATEPROBLEMOUTPUT._serialized_start=2527
-  _UPDATEPROBLEMOUTPUT._serialized_end=2548
-  _DELETEPROBLEMINPUT._serialized_start=2550
-  _DELETEPROBLEMINPUT._serialized_end=2610
-  _DELETEPROBLEMOUTPUT._serialized_start=2612
-  _DELETEPROBLEMOUTPUT._serialized_end=2633
-  _RETESTPROBLEMINPUT._serialized_start=2635
-  _RETESTPROBLEMINPUT._serialized_end=2695
-  _RETESTPROBLEMOUTPUT._serialized_start=2697
-  _RETESTPROBLEMOUTPUT._serialized_end=2718
-  _LISTPROBLEMSINPUT._serialized_start=2720
-  _LISTPROBLEMSINPUT._serialized_end=2789
-  _LISTPROBLEMSOUTPUT._serialized_start=2791
-  _LISTPROBLEMSOUTPUT._serialized_end=2864
-  _DESCRIBEPROBLEMINPUT._serialized_start=2866
-  _DESCRIBEPROBLEMINPUT._serialized_end=2950
-  _DESCRIBEPROBLEMOUTPUT._serialized_start=2952
-  _DESCRIBEPROBLEMOUTPUT._serialized_end=3015
-  _LISTSTATEMENTSINPUT._serialized_start=3017
-  _LISTSTATEMENTSINPUT._serialized_end=3078
-  _LISTSTATEMENTSOUTPUT._serialized_start=3080
-  _LISTSTATEMENTSOUTPUT._serialized_end=3165
-  _LISTATTACHMENTSINPUT._serialized_start=3167
-  _LISTATTACHMENTSINPUT._serialized_end=3229
-  _LISTATTACHMENTSOUTPUT._serialized_start=3231
-  _LISTATTACHMENTSOUTPUT._serialized_end=3318
-  _LISTEXAMPLESINPUT._serialized_start=3320
-  _LISTEXAMPLESINPUT._serialized_end=3379
-  _LISTEXAMPLESOUTPUT._serialized_start=3381
-  _LISTEXAMPLESOUTPUT._serialized_end=3459
-  _ADDPARTICIPANTINPUT._serialized_start=3461
-  _ADDPARTICIPANTINPUT._serialized_end=3563
-  _ADDPARTICIPANTOUTPUT._serialized_start=3565
-  _ADDPARTICIPANTOUTPUT._serialized_end=3611
-  _ENABLEPARTICIPANTINPUT._serialized_start=3613
-  _ENABLEPARTICIPANTINPUT._serialized_end=3681
-  _ENABLEPARTICIPANTOUTPUT._serialized_start=3683
-  _ENABLEPARTICIPANTOUTPUT._serialized_end=3708
-  _DISABLEPARTICIPANTINPUT._serialized_start=3710
-  _DISABLEPARTICIPANTINPUT._serialized_end=3779
-  _DISABLEPARTICIPANTOUTPUT._serialized_start=3781
-  _DISABLEPARTICIPANTOUTPUT._serialized_end=3807
-  _UPDATEPARTICIPANTINPUT._serialized_start=3810
-  _UPDATEPARTICIPANTINPUT._serialized_end=4067
-  _UPDATEPARTICIPANTINPUT_PATCH._serialized_start=4001
-  _UPDATEPARTICIPANTINPUT_PATCH._serialized_end=4067
-  _UPDATEPARTICIPANTOUTPUT._serialized_start=4069
-  _UPDATEPARTICIPANTOUTPUT._serialized_end=4094
-  _REMOVEPARTICIPANTINPUT._serialized_start=4096
-  _REMOVEPARTICIPANTINPUT._serialized_end=4164
-  _REMOVEPARTICIPANTOUTPUT._serialized_start=4166
-  _REMOVEPARTICIPANTOUTPUT._serialized_end=4191
-  _VERIFYPASSCODEINPUT._serialized_start=4193
-  _VERIFYPASSCODEINPUT._serialized_end=4234
-  _VERIFYPASSCODEOUTPUT._serialized_start=4236
-  _VERIFYPASSCODEOUTPUT._serialized_end=4291
-  _ENTERPASSCODEINPUT._serialized_start=4293
-  _ENTERPASSCODEINPUT._serialized_end=4351
-  _ENTERPASSCODEOUTPUT._serialized_start=4353
-  _ENTERPASSCODEOUTPUT._serialized_end=4374
-  _RESETPASSCODEINPUT._serialized_start=4376
-  _RESETPASSCODEINPUT._serialized_end=4440
-  _RESETPASSCODEOUTPUT._serialized_start=4442
-  _RESETPASSCODEOUTPUT._serialized_end=4481
-  _SETPASSCODEINPUT._serialized_start=4483
-  _SETPASSCODEINPUT._serialized_end=4563
-  _SETPASSCODEOUTPUT._serialized_start=4565
-  _SETPASSCODEOUTPUT._serialized_end=4584
-  _REMOVEPASSCODEINPUT._serialized_start=4586
-  _REMOVEPASSCODEINPUT._serialized_end=4651
-  _REMOVEPASSCODEOUTPUT._serialized_start=4653
-  _REMOVEPASSCODEOUTPUT._serialized_end=4675
-  _LISTPARTICIPANTSINPUT._serialized_start=4678
-  _LISTPARTICIPANTSINPUT._serialized_end=5422
-  _LISTPARTICIPANTSINPUT_FILTER._serialized_start=4919
-  _LISTPARTICIPANTSINPUT_FILTER._serialized_end=5343
-  _LISTPARTICIPANTSINPUT_SORTABLE._serialized_start=5345
-  _LISTPARTICIPANTSINPUT_SORTABLE._serialized_end=5422
-  _LISTPARTICIPANTSOUTPUT._serialized_start=5424
-  _LISTPARTICIPANTSOUTPUT._serialized_end=5505
-  _INTROSPECTPARTICIPANTINPUT._serialized_start=5507
-  _INTROSPECTPARTICIPANTINPUT._serialized_end=5555
-  _INTROSPECTPARTICIPANTOUTPUT._serialized_start=5557
-  _INTROSPECTPARTICIPANTOUTPUT._serialized_end=5634
-  _DESCRIBEPARTICIPANTINPUT._serialized_start=5636
-  _DESCRIBEPARTICIPANTINPUT._serialized_end=5706
-  _DESCRIBEPARTICIPANTOUTPUT._serialized_start=5708
-  _DESCRIBEPARTICIPANTOUTPUT._serialized_end=5783
-  _CREATESUBMISSIONINPUT._serialized_start=5785
-  _CREATESUBMISSIONINPUT._serialized_end=5878
-  _CREATESUBMISSIONOUTPUT._serialized_start=5880
-  _CREATESUBMISSIONOUTPUT._serialized_end=5927
-  _LISTSUBMISSIONSINPUT._serialized_start=5930
-  _LISTSUBMISSIONSINPUT._serialized_end=6542
-  _LISTSUBMISSIONSINPUT_FILTER._serialized_start=6065
-  _LISTSUBMISSIONSINPUT_FILTER._serialized_end=6542
-  _LISTSUBMISSIONSOUTPUT._serialized_start=6544
-  _LISTSUBMISSIONSOUTPUT._serialized_end=6623
-  _DESCRIBESUBMISSIONINPUT._serialized_start=6625
-  _DESCRIBESUBMISSIONINPUT._serialized_end=6693
-  _DESCRIBESUBMISSIONOUTPUT._serialized_start=6695
-  _DESCRIBESUBMISSIONOUTPUT._serialized_end=6767
-  _RETESTSUBMISSIONINPUT._serialized_start=6769
-  _RETESTSUBMISSIONINPUT._serialized_end=6835
-  _RETESTSUBMISSIONOUTPUT._serialized_start=6837
-  _RETESTSUBMISSIONOUTPUT._serialized_end=6861
-  _DELETESUBMISSIONINPUT._serialized_start=6863
-  _DELETESUBMISSIONINPUT._serialized_end=6929
-  _DELETESUBMISSIONOUTPUT._serialized_start=6931
-  _DELETESUBMISSIONOUTPUT._serialized_end=6955
-  _RESTORESUBMISSIONINPUT._serialized_start=6957
-  _RESTORESUBMISSIONINPUT._serialized_end=7024
-  _RESTORESUBMISSIONOUTPUT._serialized_start=7026
-  _RESTORESUBMISSIONOUTPUT._serialized_end=7051
-  _CREATETICKETINPUT._serialized_start=7053
-  _CREATETICKETINPUT._serialized_end=7126
-  _CREATETICKETOUTPUT._serialized_start=7128
-  _CREATETICKETOUTPUT._serialized_end=7167
-  _CLOSETICKETINPUT._serialized_start=7169
-  _CLOSETICKETINPUT._serialized_end=7226
-  _CLOSETICKETOUTPUT._serialized_start=7228
-  _CLOSETICKETOUTPUT._serialized_end=7247
-  _OPENTICKETINPUT._serialized_start=7249
-  _OPENTICKETINPUT._serialized_end=7305
-  _OPENTICKETOUTPUT._serialized_start=7307
-  _OPENTICKETOUTPUT._serialized_end=7325
-  _READTICKETINPUT._serialized_start=7327
-  _READTICKETINPUT._serialized_end=7383
-  _READTICKETOUTPUT._serialized_start=7385
-  _READTICKETOUTPUT._serialized_end=7403
-  _DELETETICKETINPUT._serialized_start=7405
-  _DELETETICKETINPUT._serialized_end=7463
-  _DELETETICKETOUTPUT._serialized_start=7465
-  _DELETETICKETOUTPUT._serialized_end=7485
-  _DESCRIBETICKETINPUT._serialized_start=7487
-  _DESCRIBETICKETINPUT._serialized_end=7547
-  _DESCRIBETICKETOUTPUT._serialized_start=7549
-  _DESCRIBETICKETOUTPUT._serialized_end=7609
-  _LISTTICKETSINPUT._serialized_start=7612
-  _LISTTICKETSINPUT._serialized_end=8274
-  _LISTTICKETSINPUT_FILTER._serialized_start=7818
-  _LISTTICKETSINPUT_FILTER._serialized_end=8202
-  _LISTTICKETSINPUT_SORTABLE._serialized_start=8204
-  _LISTTICKETSINPUT_SORTABLE._serialized_end=8274
-  _LISTTICKETSOUTPUT._serialized_start=8276
-  _LISTTICKETSOUTPUT._serialized_end=8347
-  _REPLYTICKETINPUT._serialized_start=8349
-  _REPLYTICKETINPUT._serialized_end=8418
-  _REPLYTICKETOUTPUT._serialized_start=8420
-  _REPLYTICKETOUTPUT._serialized_end=8457
-  _LISTREPLIESINPUT._serialized_start=8459
-  _LISTREPLIESINPUT._serialized_end=8526
-  _LISTREPLIESOUTPUT._serialized_start=8528
-  _LISTREPLIESOUTPUT._serialized_end=8598
-  _DELETEREPLYINPUT._serialized_start=8600
-  _DELETEREPLYINPUT._serialized_end=8655
-  _DELETEREPLYOUTPUT._serialized_start=8657
-  _DELETEREPLYOUTPUT._serialized_end=8676
-  _UPDATEREPLYINPUT._serialized_start=8678
-  _UPDATEREPLYINPUT._serialized_end=8750
-  _UPDATEREPLYOUTPUT._serialized_start=8752
-  _UPDATEREPLYOUTPUT._serialized_end=8771
-  _CONFIGURERUNTIMEINPUT._serialized_start=8773
-  _CONFIGURERUNTIMEINPUT._serialized_end=8833
-  _CONFIGURERUNTIMEOUTPUT._serialized_start=8835
-  _CONFIGURERUNTIMEOUTPUT._serialized_end=8859
-  _DESCRIBERUNTIMEINPUT._serialized_start=8861
-  _DESCRIBERUNTIMEINPUT._serialized_end=8903
-  _DESCRIBERUNTIMEOUTPUT._serialized_start=8905
-  _DESCRIBERUNTIMEOUTPUT._serialized_end=8945
-  _CONFIGURESCORINGINPUT._serialized_start=8947
-  _CONFIGURESCORINGINPUT._serialized_end=9038
-  _CONFIGURESCORINGOUTPUT._serialized_start=9040
-  _CONFIGURESCORINGOUTPUT._serialized_end=9064
-  _DESCRIBESCORINGINPUT._serialized_start=9066
-  _DESCRIBESCORINGINPUT._serialized_end=9108
-  _DESCRIBESCORINGOUTPUT._serialized_start=9110
-  _DESCRIBESCORINGOUTPUT._serialized_end=9181
-  _CREATEANNOUNCEMENTINPUT._serialized_start=9183
-  _CREATEANNOUNCEMENTINPUT._serialized_end=9278
-  _CREATEANNOUNCEMENTOUTPUT._serialized_start=9280
-  _CREATEANNOUNCEMENTOUTPUT._serialized_end=9318
-  _UPDATEANNOUNCEMENTINPUT._serialized_start=9320
-  _UPDATEANNOUNCEMENTINPUT._serialized_end=9440
-  _UPDATEANNOUNCEMENTOUTPUT._serialized_start=9442
-  _UPDATEANNOUNCEMENTOUTPUT._serialized_end=9468
-  _DELETEANNOUNCEMENTINPUT._serialized_start=9470
-  _DELETEANNOUNCEMENTINPUT._serialized_end=9540
-  _DELETEANNOUNCEMENTOUTPUT._serialized_start=9542
-  _DELETEANNOUNCEMENTOUTPUT._serialized_end=9568
-  _READANNOUNCEMENTINPUT._serialized_start=9570
-  _READANNOUNCEMENTINPUT._serialized_end=9638
-  _READANNOUNCEMENTOUTPUT._serialized_start=9640
-  _READANNOUNCEMENTOUTPUT._serialized_end=9664
-  _DESCRIBEANNOUNCEMENTINPUT._serialized_start=9666
-  _DESCRIBEANNOUNCEMENTINPUT._serialized_end=9738
-  _DESCRIBEANNOUNCEMENTOUTPUT._serialized_start=9740
-  _DESCRIBEANNOUNCEMENTOUTPUT._serialized_end=9818
-  _DESCRIBEANNOUNCEMENTSTATUSINPUT._serialized_start=9820
-  _DESCRIBEANNOUNCEMENTSTATUSINPUT._serialized_end=9898
-  _DESCRIBEANNOUNCEMENTSTATUSOUTPUT._serialized_start=9900
-  _DESCRIBEANNOUNCEMENTSTATUSOUTPUT._serialized_end=9951
-  _LISTANNOUNCEMENTSINPUT._serialized_start=9954
-  _LISTANNOUNCEMENTSINPUT._serialized_end=10195
-  _LISTANNOUNCEMENTSINPUT_FILTER._serialized_start=10092
-  _LISTANNOUNCEMENTSINPUT_FILTER._serialized_end=10195
-  _LISTANNOUNCEMENTSOUTPUT._serialized_start=10197
-  _LISTANNOUNCEMENTSOUTPUT._serialized_end=10280
-  _DESCRIBECODETEMPLATEINPUT._serialized_start=10282
-  _DESCRIBECODETEMPLATEINPUT._serialized_end=10392
-  _DESCRIBECODETEMPLATEOUTPUT._serialized_start=10394
-  _DESCRIBECODETEMPLATEOUTPUT._serialized_end=10464
-  _LOOKUPCODETEMPLATEINPUT._serialized_start=10466
-  _LOOKUPCODETEMPLATEINPUT._serialized_end=10570
-  _LOOKUPCODETEMPLATEOUTPUT._serialized_start=10572
-  _LOOKUPCODETEMPLATEOUTPUT._serialized_end=10640
-  _REBUILDSCOREINPUT._serialized_start=10642
-  _REBUILDSCOREINPUT._serialized_end=10681
-  _REBUILDSCOREOUTPUT._serialized_start=10683
-  _REBUILDSCOREOUTPUT._serialized_end=10724
-  _INTROSPECTSCOREINPUT._serialized_start=10726
-  _INTROSPECTSCOREINPUT._serialized_end=10768
-  _INTROSPECTSCOREOUTPUT._serialized_start=10770
-  _INTROSPECTSCOREOUTPUT._serialized_end=10829
-  _DESCRIBESCOREINPUT._serialized_start=10832
-  _DESCRIBESCOREINPUT._serialized_end=10965
-  _DESCRIBESCOREOUTPUT._serialized_start=10967
-  _DESCRIBESCOREOUTPUT._serialized_end=11024
-  _IMPORTSCOREINPUT._serialized_start=11026
-  _IMPORTSCOREINPUT._serialized_end=11125
-  _IMPORTSCOREOUTPUT._serialized_start=11127
-  _IMPORTSCOREOUTPUT._serialized_end=11146
-  _EXPORTSCOREINPUT._serialized_start=11148
-  _EXPORTSCOREINPUT._serialized_end=11210
-  _EXPORTSCOREOUTPUT._serialized_start=11212
-  _EXPORTSCOREOUTPUT._serialized_end=11268
-  _LISTRESULTINPUT._serialized_start=11271
-  _LISTRESULTINPUT._serialized_end=11407
-  _LISTRESULTOUTPUT._serialized_start=11409
-  _LISTRESULTOUTPUT._serialized_end=11479
-  _LISTENTITLEMENTSINPUT._serialized_start=11482
-  _LISTENTITLEMENTSINPUT._serialized_end=11610
-  _LISTENTITLEMENTSOUTPUT._serialized_start=11612
-  _LISTENTITLEMENTSOUTPUT._serialized_end=11685
-  _LISTACTIVITIESINPUT._serialized_start=11687
-  _LISTACTIVITIESINPUT._serialized_end=11758
-  _LISTACTIVITIESOUTPUT._serialized_start=11760
-  _LISTACTIVITIESOUTPUT._serialized_end=11836
-  _CONFIGUREAPPEARANCEINPUT._serialized_start=11838
-  _CONFIGUREAPPEARANCEINPUT._serialized_end=11938
-  _CONFIGUREAPPEARANCEOUTPUT._serialized_start=11940
-  _CONFIGUREAPPEARANCEOUTPUT._serialized_end=11967
-  _DESCRIBEAPPEARANCEINPUT._serialized_start=11969
-  _DESCRIBEAPPEARANCEINPUT._serialized_end=12014
-  _DESCRIBEAPPEARANCEOUTPUT._serialized_start=12016
-  _DESCRIBEAPPEARANCEOUTPUT._serialized_end=12096
-  _JUDGE._serialized_start=12099
-  _JUDGE._serialized_end=25791
+  _CREATECONTESTINPUT._serialized_start=526
+  _CREATECONTESTINPUT._serialized_end=586
+  _CREATECONTESTOUTPUT._serialized_start=588
+  _CREATECONTESTOUTPUT._serialized_end=629
+  _DELETECONTESTINPUT._serialized_start=631
+  _DELETECONTESTINPUT._serialized_end=671
+  _DELETECONTESTOUTPUT._serialized_start=673
+  _DELETECONTESTOUTPUT._serialized_end=694
+  _UPDATECONTESTINPUT._serialized_start=696
+  _UPDATECONTESTINPUT._serialized_end=776
+  _UPDATECONTESTOUTPUT._serialized_start=778
+  _UPDATECONTESTOUTPUT._serialized_end=799
+  _DESCRIBECONTESTINPUT._serialized_start=801
+  _DESCRIBECONTESTINPUT._serialized_end=843
+  _DESCRIBECONTESTOUTPUT._serialized_start=845
+  _DESCRIBECONTESTOUTPUT._serialized_end=908
+  _LOOKUPCONTESTINPUT._serialized_start=910
+  _LOOKUPCONTESTINPUT._serialized_end=943
+  _LOOKUPCONTESTOUTPUT._serialized_start=945
+  _LOOKUPCONTESTOUTPUT._serialized_end=1060
+  _LISTCONTESTSINPUT._serialized_start=1063
+  _LISTCONTESTSINPUT._serialized_end=1589
+  _LISTCONTESTSINPUT_FILTER._serialized_start=1172
+  _LISTCONTESTSINPUT_FILTER._serialized_end=1589
+  _LISTCONTESTSOUTPUT._serialized_start=1591
+  _LISTCONTESTSOUTPUT._serialized_end=1664
+  _OPENCONTESTINPUT._serialized_start=1666
+  _OPENCONTESTINPUT._serialized_end=1704
+  _OPENCONTESTOUTPUT._serialized_start=1706
+  _OPENCONTESTOUTPUT._serialized_end=1725
+  _CLOSECONTESTINPUT._serialized_start=1727
+  _CLOSECONTESTINPUT._serialized_end=1766
+  _CLOSECONTESTOUTPUT._serialized_start=1768
+  _CLOSECONTESTOUTPUT._serialized_end=1788
+  _SUSPENDCONTESTINPUT._serialized_start=1790
+  _SUSPENDCONTESTINPUT._serialized_end=1831
+  _SUSPENDCONTESTOUTPUT._serialized_start=1833
+  _SUSPENDCONTESTOUTPUT._serialized_end=1855
+  _FREEZECONTESTINPUT._serialized_start=1857
+  _FREEZECONTESTINPUT._serialized_end=1897
+  _FREEZECONTESTOUTPUT._serialized_start=1899
+  _FREEZECONTESTOUTPUT._serialized_end=1920
+  _RESUMECONTESTINPUT._serialized_start=1922
+  _RESUMECONTESTINPUT._serialized_end=1962
+  _RESUMECONTESTOUTPUT._serialized_start=1964
+  _RESUMECONTESTOUTPUT._serialized_end=1985
+  _JOINCONTESTINPUT._serialized_start=1987
+  _JOINCONTESTINPUT._serialized_end=2025
+  _JOINCONTESTOUTPUT._serialized_start=2027
+  _JOINCONTESTOUTPUT._serialized_end=2046
+  _STARTCONTESTINPUT._serialized_start=2048
+  _STARTCONTESTINPUT._serialized_end=2087
+  _STARTCONTESTOUTPUT._serialized_start=2089
+  _STARTCONTESTOUTPUT._serialized_end=2109
+  _IMPORTPROBLEMINPUT._serialized_start=2111
+  _IMPORTPROBLEMINPUT._serialized_end=2238
+  _IMPORTPROBLEMOUTPUT._serialized_start=2240
+  _IMPORTPROBLEMOUTPUT._serialized_end=2281
+  _SYNCPROBLEMINPUT._serialized_start=2283
+  _SYNCPROBLEMINPUT._serialized_end=2341
+  _SYNCPROBLEMOUTPUT._serialized_start=2343
+  _SYNCPROBLEMOUTPUT._serialized_end=2362
+  _UPDATEPROBLEMINPUT._serialized_start=2365
+  _UPDATEPROBLEMINPUT._serialized_end=2493
+  _UPDATEPROBLEMOUTPUT._serialized_start=2495
+  _UPDATEPROBLEMOUTPUT._serialized_end=2516
+  _DELETEPROBLEMINPUT._serialized_start=2518
+  _DELETEPROBLEMINPUT._serialized_end=2578
+  _DELETEPROBLEMOUTPUT._serialized_start=2580
+  _DELETEPROBLEMOUTPUT._serialized_end=2601
+  _RETESTPROBLEMINPUT._serialized_start=2603
+  _RETESTPROBLEMINPUT._serialized_end=2663
+  _RETESTPROBLEMOUTPUT._serialized_start=2665
+  _RETESTPROBLEMOUTPUT._serialized_end=2686
+  _LISTPROBLEMSINPUT._serialized_start=2688
+  _LISTPROBLEMSINPUT._serialized_end=2757
+  _LISTPROBLEMSOUTPUT._serialized_start=2759
+  _LISTPROBLEMSOUTPUT._serialized_end=2832
+  _DESCRIBEPROBLEMINPUT._serialized_start=2834
+  _DESCRIBEPROBLEMINPUT._serialized_end=2918
+  _DESCRIBEPROBLEMOUTPUT._serialized_start=2920
+  _DESCRIBEPROBLEMOUTPUT._serialized_end=2983
+  _LISTSTATEMENTSINPUT._serialized_start=2985
+  _LISTSTATEMENTSINPUT._serialized_end=3046
+  _LISTSTATEMENTSOUTPUT._serialized_start=3048
+  _LISTSTATEMENTSOUTPUT._serialized_end=3133
+  _LISTATTACHMENTSINPUT._serialized_start=3135
+  _LISTATTACHMENTSINPUT._serialized_end=3197
+  _LISTATTACHMENTSOUTPUT._serialized_start=3199
+  _LISTATTACHMENTSOUTPUT._serialized_end=3286
+  _LISTEXAMPLESINPUT._serialized_start=3288
+  _LISTEXAMPLESINPUT._serialized_end=3347
+  _LISTEXAMPLESOUTPUT._serialized_start=3349
+  _LISTEXAMPLESOUTPUT._serialized_end=3427
+  _ADDPARTICIPANTINPUT._serialized_start=3429
+  _ADDPARTICIPANTINPUT._serialized_end=3531
+  _ADDPARTICIPANTOUTPUT._serialized_start=3533
+  _ADDPARTICIPANTOUTPUT._serialized_end=3579
+  _ENABLEPARTICIPANTINPUT._serialized_start=3581
+  _ENABLEPARTICIPANTINPUT._serialized_end=3649
+  _ENABLEPARTICIPANTOUTPUT._serialized_start=3651
+  _ENABLEPARTICIPANTOUTPUT._serialized_end=3676
+  _DISABLEPARTICIPANTINPUT._serialized_start=3678
+  _DISABLEPARTICIPANTINPUT._serialized_end=3747
+  _DISABLEPARTICIPANTOUTPUT._serialized_start=3749
+  _DISABLEPARTICIPANTOUTPUT._serialized_end=3775
+  _UPDATEPARTICIPANTINPUT._serialized_start=3778
+  _UPDATEPARTICIPANTINPUT._serialized_end=4035
+  _UPDATEPARTICIPANTINPUT_PATCH._serialized_start=3969
+  _UPDATEPARTICIPANTINPUT_PATCH._serialized_end=4035
+  _UPDATEPARTICIPANTOUTPUT._serialized_start=4037
+  _UPDATEPARTICIPANTOUTPUT._serialized_end=4062
+  _REMOVEPARTICIPANTINPUT._serialized_start=4064
+  _REMOVEPARTICIPANTINPUT._serialized_end=4132
+  _REMOVEPARTICIPANTOUTPUT._serialized_start=4134
+  _REMOVEPARTICIPANTOUTPUT._serialized_end=4159
+  _VERIFYPASSCODEINPUT._serialized_start=4161
+  _VERIFYPASSCODEINPUT._serialized_end=4202
+  _VERIFYPASSCODEOUTPUT._serialized_start=4204
+  _VERIFYPASSCODEOUTPUT._serialized_end=4259
+  _ENTERPASSCODEINPUT._serialized_start=4261
+  _ENTERPASSCODEINPUT._serialized_end=4319
+  _ENTERPASSCODEOUTPUT._serialized_start=4321
+  _ENTERPASSCODEOUTPUT._serialized_end=4342
+  _RESETPASSCODEINPUT._serialized_start=4344
+  _RESETPASSCODEINPUT._serialized_end=4408
+  _RESETPASSCODEOUTPUT._serialized_start=4410
+  _RESETPASSCODEOUTPUT._serialized_end=4449
+  _SETPASSCODEINPUT._serialized_start=4451
+  _SETPASSCODEINPUT._serialized_end=4531
+  _SETPASSCODEOUTPUT._serialized_start=4533
+  _SETPASSCODEOUTPUT._serialized_end=4552
+  _REMOVEPASSCODEINPUT._serialized_start=4554
+  _REMOVEPASSCODEINPUT._serialized_end=4619
+  _REMOVEPASSCODEOUTPUT._serialized_start=4621
+  _REMOVEPASSCODEOUTPUT._serialized_end=4643
+  _LISTPARTICIPANTSINPUT._serialized_start=4646
+  _LISTPARTICIPANTSINPUT._serialized_end=5390
+  _LISTPARTICIPANTSINPUT_FILTER._serialized_start=4887
+  _LISTPARTICIPANTSINPUT_FILTER._serialized_end=5311
+  _LISTPARTICIPANTSINPUT_SORTABLE._serialized_start=5313
+  _LISTPARTICIPANTSINPUT_SORTABLE._serialized_end=5390
+  _LISTPARTICIPANTSOUTPUT._serialized_start=5392
+  _LISTPARTICIPANTSOUTPUT._serialized_end=5473
+  _INTROSPECTPARTICIPANTINPUT._serialized_start=5475
+  _INTROSPECTPARTICIPANTINPUT._serialized_end=5523
+  _INTROSPECTPARTICIPANTOUTPUT._serialized_start=5525
+  _INTROSPECTPARTICIPANTOUTPUT._serialized_end=5602
+  _DESCRIBEPARTICIPANTINPUT._serialized_start=5604
+  _DESCRIBEPARTICIPANTINPUT._serialized_end=5674
+  _DESCRIBEPARTICIPANTOUTPUT._serialized_start=5676
+  _DESCRIBEPARTICIPANTOUTPUT._serialized_end=5751
+  _CREATESUBMISSIONINPUT._serialized_start=5753
+  _CREATESUBMISSIONINPUT._serialized_end=5846
+  _CREATESUBMISSIONOUTPUT._serialized_start=5848
+  _CREATESUBMISSIONOUTPUT._serialized_end=5895
+  _LISTSUBMISSIONSINPUT._serialized_start=5898
+  _LISTSUBMISSIONSINPUT._serialized_end=6510
+  _LISTSUBMISSIONSINPUT_FILTER._serialized_start=6033
+  _LISTSUBMISSIONSINPUT_FILTER._serialized_end=6510
+  _LISTSUBMISSIONSOUTPUT._serialized_start=6512
+  _LISTSUBMISSIONSOUTPUT._serialized_end=6591
+  _DESCRIBESUBMISSIONINPUT._serialized_start=6593
+  _DESCRIBESUBMISSIONINPUT._serialized_end=6661
+  _DESCRIBESUBMISSIONOUTPUT._serialized_start=6663
+  _DESCRIBESUBMISSIONOUTPUT._serialized_end=6735
+  _RETESTSUBMISSIONINPUT._serialized_start=6737
+  _RETESTSUBMISSIONINPUT._serialized_end=6803
+  _RETESTSUBMISSIONOUTPUT._serialized_start=6805
+  _RETESTSUBMISSIONOUTPUT._serialized_end=6829
+  _DELETESUBMISSIONINPUT._serialized_start=6831
+  _DELETESUBMISSIONINPUT._serialized_end=6897
+  _DELETESUBMISSIONOUTPUT._serialized_start=6899
+  _DELETESUBMISSIONOUTPUT._serialized_end=6923
+  _RESTORESUBMISSIONINPUT._serialized_start=6925
+  _RESTORESUBMISSIONINPUT._serialized_end=6992
+  _RESTORESUBMISSIONOUTPUT._serialized_start=6994
+  _RESTORESUBMISSIONOUTPUT._serialized_end=7019
+  _CREATETICKETINPUT._serialized_start=7021
+  _CREATETICKETINPUT._serialized_end=7094
+  _CREATETICKETOUTPUT._serialized_start=7096
+  _CREATETICKETOUTPUT._serialized_end=7135
+  _CLOSETICKETINPUT._serialized_start=7137
+  _CLOSETICKETINPUT._serialized_end=7194
+  _CLOSETICKETOUTPUT._serialized_start=7196
+  _CLOSETICKETOUTPUT._serialized_end=7215
+  _OPENTICKETINPUT._serialized_start=7217
+  _OPENTICKETINPUT._serialized_end=7273
+  _OPENTICKETOUTPUT._serialized_start=7275
+  _OPENTICKETOUTPUT._serialized_end=7293
+  _READTICKETINPUT._serialized_start=7295
+  _READTICKETINPUT._serialized_end=7351
+  _READTICKETOUTPUT._serialized_start=7353
+  _READTICKETOUTPUT._serialized_end=7371
+  _DELETETICKETINPUT._serialized_start=7373
+  _DELETETICKETINPUT._serialized_end=7431
+  _DELETETICKETOUTPUT._serialized_start=7433
+  _DELETETICKETOUTPUT._serialized_end=7453
+  _DESCRIBETICKETINPUT._serialized_start=7455
+  _DESCRIBETICKETINPUT._serialized_end=7515
+  _DESCRIBETICKETOUTPUT._serialized_start=7517
+  _DESCRIBETICKETOUTPUT._serialized_end=7577
+  _LISTTICKETSINPUT._serialized_start=7580
+  _LISTTICKETSINPUT._serialized_end=8242
+  _LISTTICKETSINPUT_FILTER._serialized_start=7786
+  _LISTTICKETSINPUT_FILTER._serialized_end=8170
+  _LISTTICKETSINPUT_SORTABLE._serialized_start=8172
+  _LISTTICKETSINPUT_SORTABLE._serialized_end=8242
+  _LISTTICKETSOUTPUT._serialized_start=8244
+  _LISTTICKETSOUTPUT._serialized_end=8315
+  _REPLYTICKETINPUT._serialized_start=8317
+  _REPLYTICKETINPUT._serialized_end=8386
+  _REPLYTICKETOUTPUT._serialized_start=8388
+  _REPLYTICKETOUTPUT._serialized_end=8425
+  _LISTREPLIESINPUT._serialized_start=8427
+  _LISTREPLIESINPUT._serialized_end=8494
+  _LISTREPLIESOUTPUT._serialized_start=8496
+  _LISTREPLIESOUTPUT._serialized_end=8566
+  _DELETEREPLYINPUT._serialized_start=8568
+  _DELETEREPLYINPUT._serialized_end=8623
+  _DELETEREPLYOUTPUT._serialized_start=8625
+  _DELETEREPLYOUTPUT._serialized_end=8644
+  _UPDATEREPLYINPUT._serialized_start=8646
+  _UPDATEREPLYINPUT._serialized_end=8718
+  _UPDATEREPLYOUTPUT._serialized_start=8720
+  _UPDATEREPLYOUTPUT._serialized_end=8739
+  _CONFIGURERUNTIMEINPUT._serialized_start=8741
+  _CONFIGURERUNTIMEINPUT._serialized_end=8801
+  _CONFIGURERUNTIMEOUTPUT._serialized_start=8803
+  _CONFIGURERUNTIMEOUTPUT._serialized_end=8827
+  _DESCRIBERUNTIMEINPUT._serialized_start=8829
+  _DESCRIBERUNTIMEINPUT._serialized_end=8871
+  _DESCRIBERUNTIMEOUTPUT._serialized_start=8873
+  _DESCRIBERUNTIMEOUTPUT._serialized_end=8913
+  _CONFIGURESCORINGINPUT._serialized_start=8915
+  _CONFIGURESCORINGINPUT._serialized_end=9006
+  _CONFIGURESCORINGOUTPUT._serialized_start=9008
+  _CONFIGURESCORINGOUTPUT._serialized_end=9032
+  _DESCRIBESCORINGINPUT._serialized_start=9034
+  _DESCRIBESCORINGINPUT._serialized_end=9076
+  _DESCRIBESCORINGOUTPUT._serialized_start=9078
+  _DESCRIBESCORINGOUTPUT._serialized_end=9149
+  _CREATEANNOUNCEMENTINPUT._serialized_start=9151
+  _CREATEANNOUNCEMENTINPUT._serialized_end=9246
+  _CREATEANNOUNCEMENTOUTPUT._serialized_start=9248
+  _CREATEANNOUNCEMENTOUTPUT._serialized_end=9286
+  _UPDATEANNOUNCEMENTINPUT._serialized_start=9288
+  _UPDATEANNOUNCEMENTINPUT._serialized_end=9408
+  _UPDATEANNOUNCEMENTOUTPUT._serialized_start=9410
+  _UPDATEANNOUNCEMENTOUTPUT._serialized_end=9436
+  _DELETEANNOUNCEMENTINPUT._serialized_start=9438
+  _DELETEANNOUNCEMENTINPUT._serialized_end=9508
+  _DELETEANNOUNCEMENTOUTPUT._serialized_start=9510
+  _DELETEANNOUNCEMENTOUTPUT._serialized_end=9536
+  _READANNOUNCEMENTINPUT._serialized_start=9538
+  _READANNOUNCEMENTINPUT._serialized_end=9606
+  _READANNOUNCEMENTOUTPUT._serialized_start=9608
+  _READANNOUNCEMENTOUTPUT._serialized_end=9632
+  _DESCRIBEANNOUNCEMENTINPUT._serialized_start=9634
+  _DESCRIBEANNOUNCEMENTINPUT._serialized_end=9706
+  _DESCRIBEANNOUNCEMENTOUTPUT._serialized_start=9708
+  _DESCRIBEANNOUNCEMENTOUTPUT._serialized_end=9786
+  _DESCRIBEANNOUNCEMENTSTATUSINPUT._serialized_start=9788
+  _DESCRIBEANNOUNCEMENTSTATUSINPUT._serialized_end=9866
+  _DESCRIBEANNOUNCEMENTSTATUSOUTPUT._serialized_start=9868
+  _DESCRIBEANNOUNCEMENTSTATUSOUTPUT._serialized_end=9919
+  _LISTANNOUNCEMENTSINPUT._serialized_start=9922
+  _LISTANNOUNCEMENTSINPUT._serialized_end=10163
+  _LISTANNOUNCEMENTSINPUT_FILTER._serialized_start=10060
+  _LISTANNOUNCEMENTSINPUT_FILTER._serialized_end=10163
+  _LISTANNOUNCEMENTSOUTPUT._serialized_start=10165
+  _LISTANNOUNCEMENTSOUTPUT._serialized_end=10248
+  _DESCRIBECODETEMPLATEINPUT._serialized_start=10250
+  _DESCRIBECODETEMPLATEINPUT._serialized_end=10360
+  _DESCRIBECODETEMPLATEOUTPUT._serialized_start=10362
+  _DESCRIBECODETEMPLATEOUTPUT._serialized_end=10432
+  _LOOKUPCODETEMPLATEINPUT._serialized_start=10434
+  _LOOKUPCODETEMPLATEINPUT._serialized_end=10538
+  _LOOKUPCODETEMPLATEOUTPUT._serialized_start=10540
+  _LOOKUPCODETEMPLATEOUTPUT._serialized_end=10608
+  _REBUILDSCOREINPUT._serialized_start=10610
+  _REBUILDSCOREINPUT._serialized_end=10649
+  _REBUILDSCOREOUTPUT._serialized_start=10651
+  _REBUILDSCOREOUTPUT._serialized_end=10692
+  _INTROSPECTSCOREINPUT._serialized_start=10694
+  _INTROSPECTSCOREINPUT._serialized_end=10736
+  _INTROSPECTSCOREOUTPUT._serialized_start=10738
+  _INTROSPECTSCOREOUTPUT._serialized_end=10797
+  _DESCRIBESCOREINPUT._serialized_start=10800
+  _DESCRIBESCOREINPUT._serialized_end=10933
+  _DESCRIBESCOREOUTPUT._serialized_start=10935
+  _DESCRIBESCOREOUTPUT._serialized_end=10992
+  _IMPORTSCOREINPUT._serialized_start=10994
+  _IMPORTSCOREINPUT._serialized_end=11093
+  _IMPORTSCOREOUTPUT._serialized_start=11095
+  _IMPORTSCOREOUTPUT._serialized_end=11114
+  _EXPORTSCOREINPUT._serialized_start=11116
+  _EXPORTSCOREINPUT._serialized_end=11178
+  _EXPORTSCOREOUTPUT._serialized_start=11180
+  _EXPORTSCOREOUTPUT._serialized_end=11236
+  _LISTRESULTINPUT._serialized_start=11239
+  _LISTRESULTINPUT._serialized_end=11375
+  _LISTRESULTOUTPUT._serialized_start=11377
+  _LISTRESULTOUTPUT._serialized_end=11447
+  _LISTACTIVITIESINPUT._serialized_start=11449
+  _LISTACTIVITIESINPUT._serialized_end=11520
+  _LISTACTIVITIESOUTPUT._serialized_start=11522
+  _LISTACTIVITIESOUTPUT._serialized_end=11598
+  _CONFIGUREAPPEARANCEINPUT._serialized_start=11600
+  _CONFIGUREAPPEARANCEINPUT._serialized_end=11700
+  _CONFIGUREAPPEARANCEOUTPUT._serialized_start=11702
+  _CONFIGUREAPPEARANCEOUTPUT._serialized_end=11729
+  _DESCRIBEAPPEARANCEINPUT._serialized_start=11731
+  _DESCRIBEAPPEARANCEINPUT._serialized_end=11776
+  _DESCRIBEAPPEARANCEOUTPUT._serialized_start=11778
+  _DESCRIBEAPPEARANCEOUTPUT._serialized_end=11858
+  _JUDGE._serialized_start=11861
+  _JUDGE._serialized_end=25411
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/judge/judge_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/judge_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from eolymp.annotations import http_pb2 as _http_pb2
 from eolymp.annotations import ratelimit_pb2 as _ratelimit_pb2
 from eolymp.annotations import scope_pb2 as _scope_pb2
 from eolymp.judge import activity_pb2 as _activity_pb2
 from eolymp.judge import announcement_pb2 as _announcement_pb2
 from eolymp.judge import contest_pb2 as _contest_pb2
-from eolymp.judge import entitlement_pb2 as _entitlement_pb2
 from eolymp.judge import participant_pb2 as _participant_pb2
 from eolymp.judge import problem_pb2 as _problem_pb2
 from eolymp.judge import reply_pb2 as _reply_pb2
 from eolymp.judge import result_pb2 as _result_pb2
 from eolymp.judge import score_pb2 as _score_pb2
 from eolymp.judge import submission_pb2 as _submission_pb2
 from eolymp.judge import template_pb2 as _template_pb2
@@ -621,32 +620,14 @@
     __slots__ = ["items", "total"]
     ITEMS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     items: _containers.RepeatedCompositeFieldContainer[_contest_pb2.Contest]
     total: int
     def __init__(self, items: _Optional[_Iterable[_Union[_contest_pb2.Contest, _Mapping]]] = ..., total: _Optional[int] = ...) -> None: ...
 
-class ListEntitlementsInput(_message.Message):
-    __slots__ = ["contest_id", "participant_id", "submission_id", "ticket_id"]
-    CONTEST_ID_FIELD_NUMBER: _ClassVar[int]
-    PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
-    SUBMISSION_ID_FIELD_NUMBER: _ClassVar[int]
-    TICKET_ID_FIELD_NUMBER: _ClassVar[int]
-    contest_id: str
-    participant_id: str
-    submission_id: str
-    ticket_id: str
-    def __init__(self, contest_id: _Optional[str] = ..., submission_id: _Optional[str] = ..., ticket_id: _Optional[str] = ..., participant_id: _Optional[str] = ...) -> None: ...
-
-class ListEntitlementsOutput(_message.Message):
-    __slots__ = ["entitlements"]
-    ENTITLEMENTS_FIELD_NUMBER: _ClassVar[int]
-    entitlements: _containers.RepeatedScalarFieldContainer[_entitlement_pb2.Entitlement]
-    def __init__(self, entitlements: _Optional[_Iterable[_Union[_entitlement_pb2.Entitlement, str]]] = ...) -> None: ...
-
 class ListExamplesInput(_message.Message):
     __slots__ = ["contest_id", "problem_id"]
     CONTEST_ID_FIELD_NUMBER: _ClassVar[int]
     PROBLEM_ID_FIELD_NUMBER: _ClassVar[int]
     contest_id: str
     problem_id: str
     def __init__(self, contest_id: _Optional[str] = ..., problem_id: _Optional[str] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/judge/participant_pb2.py` & `eolymp-0.8.1/eolymp/judge/participant_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/participant_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/participant_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/problem_pb2.py` & `eolymp-0.8.1/eolymp/judge/problem_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/problem_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/problem_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/reply_pb2.py` & `eolymp-0.8.1/eolymp/judge/reply_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/reply_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/reply_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/result_pb2.py` & `eolymp-0.8.1/eolymp/judge/result_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/result_pb2.pyi` & `eolymp-0.8.1/eolymp/ranker/activity_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,44 @@
-from eolymp.judge import score_pb2 as _score_pb2
+from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Result(_message.Message):
-    __slots__ = ["contest_id", "name", "out_of_competition", "participant_id", "rank", "rank_lower", "score"]
-    CONTEST_ID_FIELD_NUMBER: _ClassVar[int]
-    NAME_FIELD_NUMBER: _ClassVar[int]
-    OUT_OF_COMPETITION_FIELD_NUMBER: _ClassVar[int]
-    PARTICIPANT_ID_FIELD_NUMBER: _ClassVar[int]
-    RANK_FIELD_NUMBER: _ClassVar[int]
-    RANK_LOWER_FIELD_NUMBER: _ClassVar[int]
-    SCORE_FIELD_NUMBER: _ClassVar[int]
-    contest_id: str
-    name: str
-    out_of_competition: bool
-    participant_id: str
-    rank: int
-    rank_lower: int
-    score: _score_pb2.Score
-    def __init__(self, participant_id: _Optional[str] = ..., contest_id: _Optional[str] = ..., name: _Optional[str] = ..., out_of_competition: bool = ..., rank: _Optional[int] = ..., rank_lower: _Optional[int] = ..., score: _Optional[_Union[_score_pb2.Score, _Mapping]] = ...) -> None: ...
+class Activity(_message.Message):
+    __slots__ = ["complete_at", "created_at", "error", "id", "progress", "progress_at", "scoreboard_id", "started_at", "status", "total", "type"]
+    class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
+        __slots__ = []
+    COMPLETE: Activity.Status
+    COMPLETE_AT_FIELD_NUMBER: _ClassVar[int]
+    CREATED: Activity.Status
+    CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    ERROR: Activity.Status
+    ERROR_FIELD_NUMBER: _ClassVar[int]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    NONE: Activity.Type
+    PROGRESS_AT_FIELD_NUMBER: _ClassVar[int]
+    PROGRESS_FIELD_NUMBER: _ClassVar[int]
+    SCOREBOARD_ID_FIELD_NUMBER: _ClassVar[int]
+    SCOREBOARD_REBUILD: Activity.Type
+    STARTED: Activity.Status
+    STARTED_AT_FIELD_NUMBER: _ClassVar[int]
+    STATUS_FIELD_NUMBER: _ClassVar[int]
+    TOTAL_FIELD_NUMBER: _ClassVar[int]
+    TYPE_FIELD_NUMBER: _ClassVar[int]
+    UNKNOWN: Activity.Status
+    complete_at: _timestamp_pb2.Timestamp
+    created_at: _timestamp_pb2.Timestamp
+    error: str
+    id: str
+    progress: int
+    progress_at: _timestamp_pb2.Timestamp
+    scoreboard_id: str
+    started_at: _timestamp_pb2.Timestamp
+    status: Activity.Status
+    total: int
+    type: Activity.Type
+    def __init__(self, id: _Optional[str] = ..., type: _Optional[_Union[Activity.Type, str]] = ..., status: _Optional[_Union[Activity.Status, str]] = ..., scoreboard_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., progress_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., complete_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., progress: _Optional[int] = ..., total: _Optional[int] = ..., error: _Optional[str] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/judge/score_pb2.py` & `eolymp-0.8.1/eolymp/judge/score_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/score_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/score_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/submission_pb2.py` & `eolymp-0.8.1/eolymp/judge/submission_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/submission_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/submission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/template_pb2.py` & `eolymp-0.8.1/eolymp/typewriter/fragment_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/judge/template.proto
+# source: eolymp/typewriter/fragment.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.atlas import code_template_file_pb2 as eolymp_dot_atlas_dot_code__template__file__pb2
+from eolymp.ecm import node_pb2 as eolymp_dot_ecm_dot_node__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65olymp/judge/template.proto\x12\x0c\x65olymp.judge\x1a%eolymp/atlas/code_template_file.proto\"\xa8\x01\n\x08Template\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x03\x65rn\x18\x8fN \x01(\t\x12\x12\n\nproblem_id\x18\x02 \x01(\t\x12\x0f\n\x07runtime\x18\x03 \x01(\t\x12\x12\n\nsource_ern\x18\n \x01(\t\x12\x12\n\nheader_ern\x18\x0b \x01(\t\x12\x12\n\nfooter_ern\x18\x0c \x01(\t\x12!\n\x05\x66iles\x18\x1e \x03(\x0b\x32\x12.eolymp.atlas.FileB-Z+github.com/eolymp/go-sdk/eolymp/judge;judgeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/typewriter/fragment.proto\x12\x11\x65olymp.typewriter\x1a\x15\x65olymp/ecm/node.proto\"v\n\x08\x46ragment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\r\n\x05title\x18\x0c \x01(\t\x12!\n\x07\x63ontent\x18\x33 \x01(\x0b\x32\x10.eolymp.ecm.Node\x12\x0e\n\x06labels\x18\x64 \x03(\tB7Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriterb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.judge.template_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.typewriter.fragment_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z+github.com/eolymp/go-sdk/eolymp/judge;judge'
-  _TEMPLATE._serialized_start=85
-  _TEMPLATE._serialized_end=253
+  DESCRIPTOR._serialized_options = b'Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriter'
+  _FRAGMENT._serialized_start=78
+  _FRAGMENT._serialized_end=196
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/judge/template_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/ticket_pb2.py` & `eolymp-0.8.1/eolymp/judge/ticket_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/judge/ticket_pb2.pyi` & `eolymp-0.8.1/eolymp/judge/ticket_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/keeper/blob_pb2.py` & `eolymp-0.8.1/eolymp/keeper/blob_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/keeper/blob_pb2.pyi` & `eolymp-0.8.1/eolymp/keeper/blob_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/keeper/keeper_http.py` & `eolymp-0.8.1/eolymp/keeper/keeper_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/keeper/keeper_pb2.py` & `eolymp-0.8.1/eolymp/keeper/keeper_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/keeper/keeper_pb2.pyi` & `eolymp-0.8.1/eolymp/keeper/keeper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/localization_service_http.py` & `eolymp-0.8.1/eolymp/l10n/localization_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/localization_service_pb2.py` & `eolymp-0.8.1/eolymp/l10n/localization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/localization_service_pb2.pyi` & `eolymp-0.8.1/eolymp/l10n/localization_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/project_pb2.py` & `eolymp-0.8.1/eolymp/l10n/project_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/project_pb2.pyi` & `eolymp-0.8.1/eolymp/l10n/project_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/project_service_http.py` & `eolymp-0.8.1/eolymp/l10n/project_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/project_service_pb2.py` & `eolymp-0.8.1/eolymp/l10n/project_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/project_service_pb2.pyi` & `eolymp-0.8.1/eolymp/l10n/project_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/term_pb2.py` & `eolymp-0.8.1/eolymp/taxonomy/topic_pb2.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/l10n/term.proto
+# source: eolymp/taxonomy/topic.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x16\x65olymp/l10n/term.proto\x12\x0b\x65olymp.l10n\"\x9f\x01\n\x04Term\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x05 \x01(\t\x12\x0f\n\x07message\x18\x02 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x03 \x01(\t\x12(\n\x06status\x18\x04 \x01(\x0e\x32\x18.eolymp.l10n.Term.Status\".\n\x06Status\x12\x08\n\x04NONE\x10\x00\x12\n\n\x06\x41\x43TIVE\x10\x01\x12\x0e\n\nDEPRECATED\x10\x02\x42+Z)github.com/eolymp/go-sdk/eolymp/l10n;l10nb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65olymp/taxonomy/topic.proto\x12\x0f\x65olymp.taxonomy\"\x94\x01\n\x05Topic\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x1aN\n\x0bTranslation\x12\x0e\n\x06locale\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/taxonomy;taxonomyb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.l10n.term_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.taxonomy.topic_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z)github.com/eolymp/go-sdk/eolymp/l10n;l10n'
-  _TERM._serialized_start=40
-  _TERM._serialized_end=199
-  _TERM_STATUS._serialized_start=153
-  _TERM_STATUS._serialized_end=199
+  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/taxonomy;taxonomy'
+  _TOPIC._serialized_start=49
+  _TOPIC._serialized_end=197
+  _TOPIC_TRANSLATION._serialized_start=119
+  _TOPIC_TRANSLATION._serialized_end=197
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/l10n/term_pb2.pyi` & `eolymp-0.8.1/eolymp/l10n/term_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/translation_pb2.py` & `eolymp-0.8.1/eolymp/l10n/translation_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/l10n/translation_pb2.pyi` & `eolymp-0.8.1/eolymp/l10n/translation_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/oauth2/oauth2_pb2.py` & `eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/oauth2/oauth2.proto\x12\reolymp.oauth2\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd5\x02\n\nTokenInput\x12\x37\n\ngrant_type\x18\x01 \x01(\x0e\x32#.eolymp.oauth2.TokenInput.GrantType\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x11\n\tclient_id\x18\x04 \x01(\t\x12\x15\n\rclient_secret\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x15\n\rcode_verifier\x18\x07 \x01(\t\x12\r\n\x05scope\x18\x08 \x01(\t\x12\x15\n\rrefresh_token\x18\t \x01(\t\x12\x14\n\x0credirect_uri\x18\n \x01(\t\"_\n\tGrantType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08PASSWORD\x10\x01\x12\x16\n\x12\x41UTHORIZATION_CODE\x10\x02\x12\x11\n\rREFRESH_TOKEN\x10\x03\x12\x0f\n\x0bGOOGLE_CODE\x10\x04\"\x83\x01\n\x0bTokenOutput\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x12\n\ntoken_type\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\r\x12\x15\n\rrefresh_token\x18\x04 \x01(\t\x12\r\n\x05scope\x18\x05 \x01(\t\x12\x10\n\x08id_token\x18\x64 \x01(\t\"\xa5\x01\n\x0e\x41uthorizeInput\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63ode_challenge\x18\x02 \x01(\t\x12\x1d\n\x15\x63ode_challenge_method\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x15\n\rresponse_type\x18\x05 \x01(\t\x12\r\n\x05scope\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\"\'\n\x0f\x41uthorizeOutput\x12\x14\n\x0credirect_uri\x18\x01 \x01(\t\",\n\rCallbackInput\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\"&\n\x0e\x43\x61llbackOutput\x12\x14\n\x0credirect_uri\x18\x01 \x01(\t\"\x0f\n\rUserInfoInput\"\xe8\x01\n\x0eUserInfoOutput\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\ngiven_name\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x61mily_name\x18\x05 \x01(\t\x12\x13\n\x0bmiddle_name\x18\x06 \x01(\t\x12\x10\n\x08nickname\x18\x07 \x01(\t\x12\x0f\n\x07picture\x18\x08 \x01(\t\x12\r\n\x05\x65mail\x18\t \x01(\t\x12\x16\n\x0e\x65mail_verified\x18\n \x01(\x08\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\x0f\n\x07profile\x18\x0c \x01(\t\" \n\x0fIntrospectInput\x12\r\n\x05token\x18\x01 \x01(\t\"\xf8\x01\n\x10IntrospectOutput\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\r\n\x05scope\x18\x02 \x01(\t\x12*\n\x06\x65xpire\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07subject\x18\x04 \x01(\t\x12\x10\n\x08\x61udience\x18\x05 \x01(\t\x12\x0e\n\x06issuer\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x64 \x01(\t\x12\x10\n\x08nickname\x18\x65 \x01(\t\x12\x0f\n\x07picture\x18\x66 \x01(\t\x12\r\n\x05\x65mail\x18g \x01(\t\x12\x16\n\x0e\x65mail_verified\x18h \x01(\x08\x12\x0e\n\x06locale\x18i \x01(\t\"\xa4\x01\n\rAuthCodeInput\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63ode_challenge\x18\x02 \x01(\t\x12\x1d\n\x15\x63ode_challenge_method\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x15\n\rresponse_type\x18\x05 \x01(\t\x12\r\n\x05scope\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\"B\n\x0e\x41uthCodeOutput\x12\x1a\n\x12\x61uthorization_code\x18\x01 \x01(\t\x12\x14\n\x0credirect_uri\x18\x02 \x01(\t\"\x1c\n\x0bRevokeInput\x12\r\n\x05token\x18\x01 \x01(\t\"\x0e\n\x0cRevokeOutput2\xfe\x04\n\x06OAuth2\x12P\n\x05Token\x12\x19.eolymp.oauth2.TokenInput\x1a\x1a.eolymp.oauth2.TokenOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12Y\n\x08UserInfo\x12\x1c.eolymp.oauth2.UserInfoInput\x1a\x1d.eolymp.oauth2.UserInfoOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12^\n\nIntrospect\x12\x1e.eolymp.oauth2.IntrospectInput\x1a\x1f.eolymp.oauth2.IntrospectOutput\"\x0f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x12S\n\x06Revoke\x12\x1a.eolymp.oauth2.RevokeInput\x1a\x1b.eolymp.oauth2.RevokeOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12Y\n\x08\x41uthCode\x12\x1c.eolymp.oauth2.AuthCodeInput\x1a\x1d.eolymp.oauth2.AuthCodeOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12\\\n\tAuthorize\x12\x1d.eolymp.oauth2.AuthorizeInput\x1a\x1e.eolymp.oauth2.AuthorizeOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12Y\n\x08\x43\x61llback\x12\x1c.eolymp.oauth2.CallbackInput\x1a\x1d.eolymp.oauth2.CallbackOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x42/Z-github.com/eolymp/go-sdk/eolymp/oauth2;oauth2b\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/oauth2/oauth2.proto\x12\reolymp.oauth2\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xd5\x02\n\nTokenInput\x12\x37\n\ngrant_type\x18\x01 \x01(\x0e\x32#.eolymp.oauth2.TokenInput.GrantType\x12\x10\n\x08username\x18\x02 \x01(\t\x12\x10\n\x08password\x18\x03 \x01(\t\x12\x11\n\tclient_id\x18\x04 \x01(\t\x12\x15\n\rclient_secret\x18\x05 \x01(\t\x12\x0c\n\x04\x63ode\x18\x06 \x01(\t\x12\x15\n\rcode_verifier\x18\x07 \x01(\t\x12\r\n\x05scope\x18\x08 \x01(\t\x12\x15\n\rrefresh_token\x18\t \x01(\t\x12\x14\n\x0credirect_uri\x18\n \x01(\t\"_\n\tGrantType\x12\x08\n\x04NONE\x10\x00\x12\x0c\n\x08PASSWORD\x10\x01\x12\x16\n\x12\x41UTHORIZATION_CODE\x10\x02\x12\x11\n\rREFRESH_TOKEN\x10\x03\x12\x0f\n\x0bGOOGLE_CODE\x10\x04\"\x83\x02\n\x0bTokenOutput\x12\x14\n\x0c\x61\x63\x63\x65ss_token\x18\x01 \x01(\t\x12\x12\n\ntoken_type\x18\x02 \x01(\t\x12\x12\n\nexpires_in\x18\x03 \x01(\r\x12\x15\n\rrefresh_token\x18\x04 \x01(\t\x12\r\n\x05scope\x18\x05 \x01(\t\x12\x10\n\x08id_token\x18\x64 \x01(\t\x12\x10\n\x07subject\x18\x84\x07 \x01(\t\x12\x0f\n\x06issuer\x18\x85\x07 \x01(\t\x12\r\n\x04name\x18\x86\x07 \x01(\t\x12\x11\n\x08nickname\x18\x87\x07 \x01(\t\x12\x10\n\x07picture\x18\x88\x07 \x01(\t\x12\x0e\n\x05\x65mail\x18\x89\x07 \x01(\t\x12\x17\n\x0e\x65mail_verified\x18\x8a\x07 \x01(\x08\"\xa5\x01\n\x0e\x41uthorizeInput\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63ode_challenge\x18\x02 \x01(\t\x12\x1d\n\x15\x63ode_challenge_method\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x15\n\rresponse_type\x18\x05 \x01(\t\x12\r\n\x05scope\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\"\'\n\x0f\x41uthorizeOutput\x12\x14\n\x0credirect_uri\x18\x01 \x01(\t\",\n\rCallbackInput\x12\x0c\n\x04\x63ode\x18\x01 \x01(\t\x12\r\n\x05state\x18\x02 \x01(\t\"&\n\x0e\x43\x61llbackOutput\x12\x14\n\x0credirect_uri\x18\x01 \x01(\t\"\x0f\n\rUserInfoInput\"\xe8\x01\n\x0eUserInfoOutput\x12\x0e\n\x06issuer\x18\x01 \x01(\t\x12\x0f\n\x07subject\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x12\n\ngiven_name\x18\x04 \x01(\t\x12\x13\n\x0b\x66\x61mily_name\x18\x05 \x01(\t\x12\x13\n\x0bmiddle_name\x18\x06 \x01(\t\x12\x10\n\x08nickname\x18\x07 \x01(\t\x12\x0f\n\x07picture\x18\x08 \x01(\t\x12\r\n\x05\x65mail\x18\t \x01(\t\x12\x16\n\x0e\x65mail_verified\x18\n \x01(\x08\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\x0f\n\x07profile\x18\x0c \x01(\t\" \n\x0fIntrospectInput\x12\r\n\x05token\x18\x01 \x01(\t\"\xf8\x01\n\x10IntrospectOutput\x12\x0e\n\x06\x61\x63tive\x18\x01 \x01(\x08\x12\r\n\x05scope\x18\x02 \x01(\t\x12*\n\x06\x65xpire\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07subject\x18\x04 \x01(\t\x12\x10\n\x08\x61udience\x18\x05 \x01(\t\x12\x0e\n\x06issuer\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x64 \x01(\t\x12\x10\n\x08nickname\x18\x65 \x01(\t\x12\x0f\n\x07picture\x18\x66 \x01(\t\x12\r\n\x05\x65mail\x18g \x01(\t\x12\x16\n\x0e\x65mail_verified\x18h \x01(\x08\x12\x0e\n\x06locale\x18i \x01(\t\"\xa4\x01\n\rAuthCodeInput\x12\x11\n\tclient_id\x18\x01 \x01(\t\x12\x16\n\x0e\x63ode_challenge\x18\x02 \x01(\t\x12\x1d\n\x15\x63ode_challenge_method\x18\x03 \x01(\t\x12\x14\n\x0credirect_uri\x18\x04 \x01(\t\x12\x15\n\rresponse_type\x18\x05 \x01(\t\x12\r\n\x05scope\x18\x06 \x01(\t\x12\r\n\x05state\x18\x07 \x01(\t\"B\n\x0e\x41uthCodeOutput\x12\x1a\n\x12\x61uthorization_code\x18\x01 \x01(\t\x12\x14\n\x0credirect_uri\x18\x02 \x01(\t\"\x1c\n\x0bRevokeInput\x12\r\n\x05token\x18\x01 \x01(\t\"\x0e\n\x0cRevokeOutput2\xfe\x04\n\x06OAuth2\x12P\n\x05Token\x12\x19.eolymp.oauth2.TokenInput\x1a\x1a.eolymp.oauth2.TokenOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12Y\n\x08UserInfo\x12\x1c.eolymp.oauth2.UserInfoInput\x1a\x1d.eolymp.oauth2.UserInfoOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12^\n\nIntrospect\x12\x1e.eolymp.oauth2.IntrospectInput\x1a\x1f.eolymp.oauth2.IntrospectOutput\"\x0f\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x12S\n\x06Revoke\x12\x1a.eolymp.oauth2.RevokeInput\x1a\x1b.eolymp.oauth2.RevokeOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12Y\n\x08\x41uthCode\x12\x1c.eolymp.oauth2.AuthCodeInput\x1a\x1d.eolymp.oauth2.AuthCodeOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12\\\n\tAuthorize\x12\x1d.eolymp.oauth2.AuthorizeInput\x1a\x1e.eolymp.oauth2.AuthorizeOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x12Y\n\x08\x43\x61llback\x12\x1c.eolymp.oauth2.CallbackInput\x1a\x1d.eolymp.oauth2.CallbackOutput\"\x10\xea\xe2\n\x0c\xf5\xe2\n\x00\x00\xf0\x41\xf8\xe2\n\xac\x02\x42/Z-github.com/eolymp/go-sdk/eolymp/oauth2;oauth2b\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.oauth2.oauth2_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z-github.com/eolymp/go-sdk/eolymp/oauth2;oauth2'
@@ -38,35 +38,35 @@
   _OAUTH2.methods_by_name['Callback']._options = None
   _OAUTH2.methods_by_name['Callback']._serialized_options = b'\352\342\n\014\365\342\n\000\000\360A\370\342\n\254\002'
   _TOKENINPUT._serialized_start=115
   _TOKENINPUT._serialized_end=456
   _TOKENINPUT_GRANTTYPE._serialized_start=361
   _TOKENINPUT_GRANTTYPE._serialized_end=456
   _TOKENOUTPUT._serialized_start=459
-  _TOKENOUTPUT._serialized_end=590
-  _AUTHORIZEINPUT._serialized_start=593
-  _AUTHORIZEINPUT._serialized_end=758
-  _AUTHORIZEOUTPUT._serialized_start=760
-  _AUTHORIZEOUTPUT._serialized_end=799
-  _CALLBACKINPUT._serialized_start=801
-  _CALLBACKINPUT._serialized_end=845
-  _CALLBACKOUTPUT._serialized_start=847
-  _CALLBACKOUTPUT._serialized_end=885
-  _USERINFOINPUT._serialized_start=887
-  _USERINFOINPUT._serialized_end=902
-  _USERINFOOUTPUT._serialized_start=905
-  _USERINFOOUTPUT._serialized_end=1137
-  _INTROSPECTINPUT._serialized_start=1139
-  _INTROSPECTINPUT._serialized_end=1171
-  _INTROSPECTOUTPUT._serialized_start=1174
-  _INTROSPECTOUTPUT._serialized_end=1422
-  _AUTHCODEINPUT._serialized_start=1425
-  _AUTHCODEINPUT._serialized_end=1589
-  _AUTHCODEOUTPUT._serialized_start=1591
-  _AUTHCODEOUTPUT._serialized_end=1657
-  _REVOKEINPUT._serialized_start=1659
-  _REVOKEINPUT._serialized_end=1687
-  _REVOKEOUTPUT._serialized_start=1689
-  _REVOKEOUTPUT._serialized_end=1703
-  _OAUTH2._serialized_start=1706
-  _OAUTH2._serialized_end=2344
+  _TOKENOUTPUT._serialized_end=718
+  _AUTHORIZEINPUT._serialized_start=721
+  _AUTHORIZEINPUT._serialized_end=886
+  _AUTHORIZEOUTPUT._serialized_start=888
+  _AUTHORIZEOUTPUT._serialized_end=927
+  _CALLBACKINPUT._serialized_start=929
+  _CALLBACKINPUT._serialized_end=973
+  _CALLBACKOUTPUT._serialized_start=975
+  _CALLBACKOUTPUT._serialized_end=1013
+  _USERINFOINPUT._serialized_start=1015
+  _USERINFOINPUT._serialized_end=1030
+  _USERINFOOUTPUT._serialized_start=1033
+  _USERINFOOUTPUT._serialized_end=1265
+  _INTROSPECTINPUT._serialized_start=1267
+  _INTROSPECTINPUT._serialized_end=1299
+  _INTROSPECTOUTPUT._serialized_start=1302
+  _INTROSPECTOUTPUT._serialized_end=1550
+  _AUTHCODEINPUT._serialized_start=1553
+  _AUTHCODEINPUT._serialized_end=1717
+  _AUTHCODEOUTPUT._serialized_start=1719
+  _AUTHCODEOUTPUT._serialized_end=1785
+  _REVOKEINPUT._serialized_start=1787
+  _REVOKEINPUT._serialized_end=1815
+  _REVOKEOUTPUT._serialized_start=1817
+  _REVOKEOUTPUT._serialized_end=1831
+  _OAUTH2._serialized_start=1834
+  _OAUTH2._serialized_end=2472
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/oauth2/oauth2_pb2.pyi` & `eolymp-0.8.1/eolymp/oauth2/oauth2_pb2.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -143,28 +143,42 @@
     redirect_uri: str
     refresh_token: str
     scope: str
     username: str
     def __init__(self, grant_type: _Optional[_Union[TokenInput.GrantType, str]] = ..., username: _Optional[str] = ..., password: _Optional[str] = ..., client_id: _Optional[str] = ..., client_secret: _Optional[str] = ..., code: _Optional[str] = ..., code_verifier: _Optional[str] = ..., scope: _Optional[str] = ..., refresh_token: _Optional[str] = ..., redirect_uri: _Optional[str] = ...) -> None: ...
 
 class TokenOutput(_message.Message):
-    __slots__ = ["access_token", "expires_in", "id_token", "refresh_token", "scope", "token_type"]
+    __slots__ = ["access_token", "email", "email_verified", "expires_in", "id_token", "issuer", "name", "nickname", "picture", "refresh_token", "scope", "subject", "token_type"]
     ACCESS_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_FIELD_NUMBER: _ClassVar[int]
+    EMAIL_VERIFIED_FIELD_NUMBER: _ClassVar[int]
     EXPIRES_IN_FIELD_NUMBER: _ClassVar[int]
     ID_TOKEN_FIELD_NUMBER: _ClassVar[int]
+    ISSUER_FIELD_NUMBER: _ClassVar[int]
+    NAME_FIELD_NUMBER: _ClassVar[int]
+    NICKNAME_FIELD_NUMBER: _ClassVar[int]
+    PICTURE_FIELD_NUMBER: _ClassVar[int]
     REFRESH_TOKEN_FIELD_NUMBER: _ClassVar[int]
     SCOPE_FIELD_NUMBER: _ClassVar[int]
+    SUBJECT_FIELD_NUMBER: _ClassVar[int]
     TOKEN_TYPE_FIELD_NUMBER: _ClassVar[int]
     access_token: str
+    email: str
+    email_verified: bool
     expires_in: int
     id_token: str
+    issuer: str
+    name: str
+    nickname: str
+    picture: str
     refresh_token: str
     scope: str
+    subject: str
     token_type: str
-    def __init__(self, access_token: _Optional[str] = ..., token_type: _Optional[str] = ..., expires_in: _Optional[int] = ..., refresh_token: _Optional[str] = ..., scope: _Optional[str] = ..., id_token: _Optional[str] = ...) -> None: ...
+    def __init__(self, access_token: _Optional[str] = ..., token_type: _Optional[str] = ..., expires_in: _Optional[int] = ..., refresh_token: _Optional[str] = ..., scope: _Optional[str] = ..., id_token: _Optional[str] = ..., subject: _Optional[str] = ..., issuer: _Optional[str] = ..., name: _Optional[str] = ..., nickname: _Optional[str] = ..., picture: _Optional[str] = ..., email: _Optional[str] = ..., email_verified: bool = ...) -> None: ...
 
 class UserInfoInput(_message.Message):
     __slots__ = []
     def __init__(self) -> None: ...
 
 class UserInfoOutput(_message.Message):
     __slots__ = ["email", "email_verified", "family_name", "given_name", "issuer", "locale", "middle_name", "name", "nickname", "picture", "profile", "subject"]
```

### Comparing `eolymp-0.8.0/eolymp/playground/playground_http.py` & `eolymp-0.8.1/eolymp/playground/playground_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/playground/playground_pb2.py` & `eolymp-0.8.1/eolymp/playground/playground_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/playground/playground_pb2.pyi` & `eolymp-0.8.1/eolymp/playground/playground_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/playground/run_pb2.py` & `eolymp-0.8.1/eolymp/playground/run_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/playground/run_pb2.pyi` & `eolymp-0.8.1/eolymp/playground/run_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/activity_pb2.py` & `eolymp-0.8.1/eolymp/ranker/activity_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/activity_pb2.pyi` & `eolymp-0.8.1/eolymp/worker/job_pb2.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,57 @@
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
+from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
 from typing import ClassVar as _ClassVar, Mapping as _Mapping, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
-class Activity(_message.Message):
-    __slots__ = ["complete_at", "created_at", "error", "id", "progress", "progress_at", "scoreboard_id", "started_at", "status", "total", "type"]
+class Job(_message.Message):
+    __slots__ = ["complete_at", "created_at", "id", "inputs", "logs", "outputs", "progress", "progress_at", "started_at", "status", "total", "type"]
     class Status(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
-    class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
-        __slots__ = []
-    COMPLETE: Activity.Status
+    class InputsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    class OutputsEntry(_message.Message):
+        __slots__ = ["key", "value"]
+        KEY_FIELD_NUMBER: _ClassVar[int]
+        VALUE_FIELD_NUMBER: _ClassVar[int]
+        key: str
+        value: str
+        def __init__(self, key: _Optional[str] = ..., value: _Optional[str] = ...) -> None: ...
+    COMPLETE: Job.Status
     COMPLETE_AT_FIELD_NUMBER: _ClassVar[int]
-    CREATED: Activity.Status
+    CREATED: Job.Status
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
-    ERROR: Activity.Status
-    ERROR_FIELD_NUMBER: _ClassVar[int]
+    ERROR: Job.Status
     ID_FIELD_NUMBER: _ClassVar[int]
-    NONE: Activity.Type
+    INPUTS_FIELD_NUMBER: _ClassVar[int]
+    LOGS_FIELD_NUMBER: _ClassVar[int]
+    OUTPUTS_FIELD_NUMBER: _ClassVar[int]
     PROGRESS_AT_FIELD_NUMBER: _ClassVar[int]
     PROGRESS_FIELD_NUMBER: _ClassVar[int]
-    SCOREBOARD_ID_FIELD_NUMBER: _ClassVar[int]
-    SCOREBOARD_REBUILD: Activity.Type
-    STARTED: Activity.Status
+    STARTED: Job.Status
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     TOTAL_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
-    UNKNOWN: Activity.Status
+    UNKNOWN: Job.Status
     complete_at: _timestamp_pb2.Timestamp
     created_at: _timestamp_pb2.Timestamp
-    error: str
     id: str
+    inputs: _containers.ScalarMap[str, str]
+    logs: str
+    outputs: _containers.ScalarMap[str, str]
     progress: int
     progress_at: _timestamp_pb2.Timestamp
-    scoreboard_id: str
     started_at: _timestamp_pb2.Timestamp
-    status: Activity.Status
+    status: Job.Status
     total: int
-    type: Activity.Type
-    def __init__(self, id: _Optional[str] = ..., type: _Optional[_Union[Activity.Type, str]] = ..., status: _Optional[_Union[Activity.Status, str]] = ..., scoreboard_id: _Optional[str] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., progress_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., complete_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., progress: _Optional[int] = ..., total: _Optional[int] = ..., error: _Optional[str] = ...) -> None: ...
+    type: str
+    def __init__(self, id: _Optional[str] = ..., type: _Optional[str] = ..., inputs: _Optional[_Mapping[str, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., progress_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., complete_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., progress: _Optional[int] = ..., total: _Optional[int] = ..., status: _Optional[_Union[Job.Status, str]] = ..., outputs: _Optional[_Mapping[str, str]] = ..., logs: _Optional[str] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/ranker/events_pb2.py` & `eolymp-0.8.1/eolymp/ranker/events_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/events_pb2.pyi` & `eolymp-0.8.1/eolymp/ranker/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/format_pb2.py` & `eolymp-0.8.1/eolymp/wellknown/direction_pb2.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/ranker/format.proto
+# source: eolymp/wellknown/direction.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/ranker/format.proto\x12\reolymp.ranker*%\n\x06\x46ormat\x12\x08\n\x04NONE\x10\x00\x12\x07\n\x03IOI\x10\x01\x12\x08\n\x04ICPC\x10\x02\x42/Z-github.com/eolymp/go-sdk/eolymp/ranker;rankerb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/wellknown/direction.proto\x12\x10\x65olymp.wellknown*\x1e\n\tDirection\x12\x07\n\x03\x41SC\x10\x00\x12\x08\n\x04\x44\x45SC\x10\x01\x42\x35Z3github.com/eolymp/go-sdk/eolymp/wellknown;wellknownb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.ranker.format_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.wellknown.direction_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z-github.com/eolymp/go-sdk/eolymp/ranker;ranker'
-  _FORMAT._serialized_start=45
-  _FORMAT._serialized_end=82
+  DESCRIPTOR._serialized_options = b'Z3github.com/eolymp/go-sdk/eolymp/wellknown;wellknown'
+  _DIRECTION._serialized_start=54
+  _DIRECTION._serialized_end=84
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/ranker/ranker_http.py` & `eolymp-0.8.1/eolymp/ranker/ranker_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/ranker_pb2.py` & `eolymp-0.8.1/eolymp/ranker/ranker_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/ranker_pb2.pyi` & `eolymp-0.8.1/eolymp/ranker/ranker_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/scoreboard_pb2.py` & `eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/ranker/scoreboard_pb2.pyi` & `eolymp-0.8.1/eolymp/ranker/scoreboard_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/resolver/resolver_http.py` & `eolymp-0.8.1/eolymp/resolver/resolver_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/resolver/resolver_pb2.py` & `eolymp-0.8.1/eolymp/resolver/resolver_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/resolver/resolver_pb2.pyi` & `eolymp-0.8.1/eolymp/resolver/resolver_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/link_service_http.py` & `eolymp-0.8.1/eolymp/taxonomy/link_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/link_service_pb2.py` & `eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/link_service_pb2.pyi` & `eolymp-0.8.1/eolymp/taxonomy/link_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/topic_pb2.py` & `eolymp-0.8.1/eolymp/typewriter/events_pb2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/taxonomy/topic.proto
+# source: eolymp/typewriter/events.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from eolymp.typewriter import fragment_pb2 as eolymp_dot_typewriter_dot_fragment__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65olymp/taxonomy/topic.proto\x12\x0f\x65olymp.taxonomy\"\x94\x01\n\x05Topic\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\t\x1aN\n\x0bTranslation\x12\x0e\n\x06locale\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07summary\x18\x03 \x01(\t\x12\x10\n\x08keywords\x18\x04 \x03(\tB3Z1github.com/eolymp/go-sdk/eolymp/taxonomy;taxonomyb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/typewriter/events.proto\x12\x11\x65olymp.typewriter\x1a eolymp/typewriter/fragment.proto\"o\n\x14\x46ragmentChangedEvent\x12+\n\x06\x62\x65\x66ore\x18\x01 \x01(\x0b\x32\x1b.eolymp.typewriter.Fragment\x12*\n\x05\x61\x66ter\x18\x02 \x01(\x0b\x32\x1b.eolymp.typewriter.FragmentB7Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriterb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.taxonomy.topic_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.typewriter.events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/taxonomy;taxonomy'
-  _TOPIC._serialized_start=49
-  _TOPIC._serialized_end=197
-  _TOPIC_TRANSLATION._serialized_start=119
-  _TOPIC_TRANSLATION._serialized_end=197
+  DESCRIPTOR._serialized_options = b'Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriter'
+  _FRAGMENTCHANGEDEVENT._serialized_start=87
+  _FRAGMENTCHANGEDEVENT._serialized_end=198
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/taxonomy/topic_pb2.pyi` & `eolymp-0.8.1/eolymp/taxonomy/topic_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/topic_service_http.py` & `eolymp-0.8.1/eolymp/taxonomy/topic_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/topic_service_pb2.py` & `eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/taxonomy/topic_service_pb2.pyi` & `eolymp-0.8.1/eolymp/taxonomy/topic_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/block_pb2.py` & `eolymp-0.8.1/eolymp/typewriter/block_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/block_pb2.pyi` & `eolymp-0.8.1/eolymp/typewriter/block_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/events_pb2.py` & `eolymp-0.8.1/eolymp/universe/permission_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/typewriter/events.proto
+# source: eolymp/universe/permission.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.typewriter import fragment_pb2 as eolymp_dot_typewriter_dot_fragment__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/typewriter/events.proto\x12\x11\x65olymp.typewriter\x1a eolymp/typewriter/fragment.proto\"o\n\x14\x46ragmentChangedEvent\x12+\n\x06\x62\x65\x66ore\x18\x01 \x01(\x0b\x32\x1b.eolymp.typewriter.Fragment\x12*\n\x05\x61\x66ter\x18\x02 \x01(\x0b\x32\x1b.eolymp.typewriter.FragmentB7Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriterb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/universe/permission.proto\x12\x0f\x65olymp.universe\"\x99\x01\n\nPermission\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x04role\x18\x02 \x01(\x0e\x32 .eolymp.universe.Permission.Role\x12\x0f\n\x07user_id\x18\x03 \x01(\t\">\n\x04Role\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05OWNER\x10\x01\x12\t\n\x05\x41\x44MIN\x10\x02\x12\n\n\x06VIEWER\x10\x03\x12\n\n\x06\x43USTOM\x10\x04\x42\x33Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.typewriter.events_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.universe.permission_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriter'
-  _FRAGMENTCHANGEDEVENT._serialized_start=87
-  _FRAGMENTCHANGEDEVENT._serialized_end=198
+  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/universe;universe'
+  _PERMISSION._serialized_start=54
+  _PERMISSION._serialized_end=207
+  _PERMISSION_ROLE._serialized_start=145
+  _PERMISSION_ROLE._serialized_end=207
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/typewriter/events_pb2.pyi` & `eolymp-0.8.1/eolymp/typewriter/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/fragment_pb2.py` & `eolymp-0.8.1/eolymp/worker/events_pb2.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/typewriter/fragment.proto
+# source: eolymp/worker/events.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-from eolymp.ecm import node_pb2 as eolymp_dot_ecm_dot_node__pb2
+from eolymp.worker import job_pb2 as eolymp_dot_worker_dot_job__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/typewriter/fragment.proto\x12\x11\x65olymp.typewriter\x1a\x15\x65olymp/ecm/node.proto\"v\n\x08\x46ragment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\r\n\x05title\x18\x0c \x01(\t\x12!\n\x07\x63ontent\x18\x33 \x01(\x0b\x32\x10.eolymp.ecm.Node\x12\x0e\n\x06labels\x18\x64 \x03(\tB7Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriterb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1a\x65olymp/worker/events.proto\x12\reolymp.worker\x1a\x17\x65olymp/worker/job.proto\"2\n\x0fJobTriggerEvent\x12\x1f\n\x03job\x18\x01 \x01(\x0b\x32\x12.eolymp.worker.JobB/Z-github.com/eolymp/go-sdk/eolymp/worker;workerb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.typewriter.fragment_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.worker.events_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z5github.com/eolymp/go-sdk/eolymp/typewriter;typewriter'
-  _FRAGMENT._serialized_start=78
-  _FRAGMENT._serialized_end=196
+  DESCRIPTOR._serialized_options = b'Z-github.com/eolymp/go-sdk/eolymp/worker;worker'
+  _JOBTRIGGEREVENT._serialized_start=70
+  _JOBTRIGGEREVENT._serialized_end=120
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/typewriter/fragment_pb2.pyi` & `eolymp-0.8.1/eolymp/typewriter/fragment_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/inline_pb2.py` & `eolymp-0.8.1/eolymp/typewriter/inline_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/inline_pb2.pyi` & `eolymp-0.8.1/eolymp/typewriter/inline_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/typewriter_http.py` & `eolymp-0.8.1/eolymp/typewriter/typewriter_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/typewriter_pb2.py` & `eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/typewriter/typewriter_pb2.pyi` & `eolymp-0.8.1/eolymp/typewriter/typewriter_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/universe/permission_pb2.py` & `eolymp-0.8.1/eolymp/content/fragment_pb2.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: eolymp/universe/permission.proto
+# source: eolymp/content/fragment.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from eolymp.ecm import content_pb2 as eolymp_dot_ecm_dot_content__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n eolymp/universe/permission.proto\x12\x0f\x65olymp.universe\"\x99\x01\n\nPermission\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\x04role\x18\x02 \x01(\x0e\x32 .eolymp.universe.Permission.Role\x12\x0f\n\x07user_id\x18\x03 \x01(\t\">\n\x04Role\x12\x08\n\x04NONE\x10\x00\x12\t\n\x05OWNER\x10\x01\x12\t\n\x05\x41\x44MIN\x10\x02\x12\n\n\x06VIEWER\x10\x03\x12\n\n\x06\x43USTOM\x10\x04\x42\x33Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1d\x65olymp/content/fragment.proto\x12\x0e\x65olymp.content\x1a\x18\x65olymp/ecm/content.proto\"y\n\x08\x46ragment\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04path\x18\n \x01(\t\x12\x0e\n\x06locale\x18\x0b \x01(\t\x12\r\n\x05title\x18\x0c \x01(\t\x12$\n\x07\x63ontent\x18\x33 \x01(\x0b\x32\x13.eolymp.ecm.Content\x12\x0e\n\x06labels\x18\x64 \x03(\tB1Z/github.com/eolymp/go-sdk/eolymp/content;contentb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.universe.permission_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.content.fragment_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/universe;universe'
-  _PERMISSION._serialized_start=54
-  _PERMISSION._serialized_end=207
-  _PERMISSION_ROLE._serialized_start=145
-  _PERMISSION_ROLE._serialized_end=207
+  DESCRIPTOR._serialized_options = b'Z/github.com/eolymp/go-sdk/eolymp/content;content'
+  _FRAGMENT._serialized_start=75
+  _FRAGMENT._serialized_end=196
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/universe/permission_pb2.pyi` & `eolymp-0.8.1/eolymp/universe/permission_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/universe/space_pb2.py` & `eolymp-0.8.1/eolymp/universe/space_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,26 +9,26 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65olymp/universe/space.proto\x12\x0f\x65olymp.universe\"\x8d\x06\n\x05Space\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\n \x01(\t\x12\r\n\x05image\x18\x0b \x01(\t\x12)\n\x04type\x18\x0c \x01(\x0e\x32\x1b.eolymp.universe.Space.Type\x12\x0c\n\x04plan\x18\r \x01(\t\x12\x35\n\nvisibility\x18\x0e \x01(\x0e\x32!.eolymp.universe.Space.Visibility\x12\x35\n\nmembership\x18\x14 \x01(\x0e\x32!.eolymp.universe.Space.Membership\x12\x15\n\rmin_team_size\x18\x15 \x01(\r\x12\x15\n\rmax_team_size\x18\x16 \x01(\r\x1a\x99\x02\n\x05Quota\x12\x1a\n\x12problems_per_space\x18\x01 \x01(\r\x12\x19\n\x11members_per_space\x18\x02 \x01(\r\x12\x1a\n\x12\x63ontests_per_space\x18\x03 \x01(\r\x12!\n\x19\x61\x63tive_contests_per_space\x18\x04 \x01(\r\x12\x1d\n\x15scoreboards_per_space\x18\x05 \x01(\r\x12\x1d\n\x15permissions_per_space\x18\x06 \x01(\r\x12\x1c\n\x14\x61ttributes_per_space\x18\x07 \x01(\r\x12\x1c\n\x14problems_per_contest\x18\n \x01(\r\x12 \n\x18participants_per_contest\x18\x0b \x01(\r\"Q\n\x04Type\x12\x10\n\x0cUNKNOWN_TYPE\x10\x00\x12\t\n\x05OTHER\x10\x01\x12\r\n\tCLASSROOM\x10\x02\x12\x0c\n\x08TEAMROOM\x10\x03\x12\x0f\n\x0b\x43OMPETITION\x10\x04\">\n\nMembership\x12\x16\n\x12UNKNOWN_MEMBERSHIP\x10\x00\x12\x0e\n\nINDIVIDUAL\x10\x01\x12\x08\n\x04TEAM\x10\x02\"=\n\nVisibility\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\n\n\x06PUBLIC\x10\x01\x12\x0b\n\x07PRIVATE\x10\x02\x42\x33Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1b\x65olymp/universe/space.proto\x12\x0f\x65olymp.universe\"\xa3\x06\n\x05Space\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0b\n\x03key\x18\x02 \x01(\t\x12\x0b\n\x03url\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\n \x01(\t\x12\r\n\x05image\x18\x0b \x01(\t\x12)\n\x04type\x18\x0c \x01(\x0e\x32\x1b.eolymp.universe.Space.Type\x12\x0c\n\x04plan\x18\r \x01(\t\x12\x35\n\nvisibility\x18\x0e \x01(\x0e\x32!.eolymp.universe.Space.Visibility\x12\x35\n\nmembership\x18\x14 \x01(\x0e\x32!.eolymp.universe.Space.Membership\x12\x15\n\rmin_team_size\x18\x15 \x01(\r\x12\x15\n\rmax_team_size\x18\x16 \x01(\r\x12\x14\n\x0bpermissions\x18\xf3N \x03(\t\x1a\x99\x02\n\x05Quota\x12\x1a\n\x12problems_per_space\x18\x01 \x01(\r\x12\x19\n\x11members_per_space\x18\x02 \x01(\r\x12\x1a\n\x12\x63ontests_per_space\x18\x03 \x01(\r\x12!\n\x19\x61\x63tive_contests_per_space\x18\x04 \x01(\r\x12\x1d\n\x15scoreboards_per_space\x18\x05 \x01(\r\x12\x1d\n\x15permissions_per_space\x18\x06 \x01(\r\x12\x1c\n\x14\x61ttributes_per_space\x18\x07 \x01(\r\x12\x1c\n\x14problems_per_contest\x18\n \x01(\r\x12 \n\x18participants_per_contest\x18\x0b \x01(\r\"Q\n\x04Type\x12\x10\n\x0cUNKNOWN_TYPE\x10\x00\x12\t\n\x05OTHER\x10\x01\x12\r\n\tCLASSROOM\x10\x02\x12\x0c\n\x08TEAMROOM\x10\x03\x12\x0f\n\x0b\x43OMPETITION\x10\x04\">\n\nMembership\x12\x16\n\x12UNKNOWN_MEMBERSHIP\x10\x00\x12\x0e\n\nINDIVIDUAL\x10\x01\x12\x08\n\x04TEAM\x10\x02\"=\n\nVisibility\x12\x16\n\x12UNKNOWN_VISIBILITY\x10\x00\x12\n\n\x06PUBLIC\x10\x01\x12\x0b\n\x07PRIVATE\x10\x02\x42\x33Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.universe.space_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/universe;universe'
   _SPACE._serialized_start=49
-  _SPACE._serialized_end=830
-  _SPACE_QUOTA._serialized_start=339
-  _SPACE_QUOTA._serialized_end=620
-  _SPACE_TYPE._serialized_start=622
-  _SPACE_TYPE._serialized_end=703
-  _SPACE_MEMBERSHIP._serialized_start=705
-  _SPACE_MEMBERSHIP._serialized_end=767
-  _SPACE_VISIBILITY._serialized_start=769
-  _SPACE_VISIBILITY._serialized_end=830
+  _SPACE._serialized_end=852
+  _SPACE_QUOTA._serialized_start=361
+  _SPACE_QUOTA._serialized_end=642
+  _SPACE_TYPE._serialized_start=644
+  _SPACE_TYPE._serialized_end=725
+  _SPACE_MEMBERSHIP._serialized_start=727
+  _SPACE_MEMBERSHIP._serialized_end=789
+  _SPACE_VISIBILITY._serialized_start=791
+  _SPACE_VISIBILITY._serialized_end=852
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/universe/space_pb2.pyi` & `eolymp-0.8.1/eolymp/universe/space_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
+from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
-from typing import ClassVar as _ClassVar, Optional as _Optional, Union as _Union
+from typing import ClassVar as _ClassVar, Iterable as _Iterable, Optional as _Optional, Union as _Union
 
 DESCRIPTOR: _descriptor.FileDescriptor
 
 class Space(_message.Message):
-    __slots__ = ["id", "image", "key", "max_team_size", "membership", "min_team_size", "name", "plan", "type", "url", "visibility"]
+    __slots__ = ["id", "image", "key", "max_team_size", "membership", "min_team_size", "name", "permissions", "plan", "type", "url", "visibility"]
     class Membership(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Type(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Visibility(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
     class Quota(_message.Message):
@@ -41,14 +42,15 @@
     INDIVIDUAL: Space.Membership
     KEY_FIELD_NUMBER: _ClassVar[int]
     MAX_TEAM_SIZE_FIELD_NUMBER: _ClassVar[int]
     MEMBERSHIP_FIELD_NUMBER: _ClassVar[int]
     MIN_TEAM_SIZE_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     OTHER: Space.Type
+    PERMISSIONS_FIELD_NUMBER: _ClassVar[int]
     PLAN_FIELD_NUMBER: _ClassVar[int]
     PRIVATE: Space.Visibility
     PUBLIC: Space.Visibility
     TEAM: Space.Membership
     TEAMROOM: Space.Type
     TYPE_FIELD_NUMBER: _ClassVar[int]
     UNKNOWN_MEMBERSHIP: Space.Membership
@@ -59,12 +61,13 @@
     id: str
     image: str
     key: str
     max_team_size: int
     membership: Space.Membership
     min_team_size: int
     name: str
+    permissions: _containers.RepeatedScalarFieldContainer[str]
     plan: str
     type: Space.Type
     url: str
     visibility: Space.Visibility
-    def __init__(self, id: _Optional[str] = ..., key: _Optional[str] = ..., url: _Optional[str] = ..., name: _Optional[str] = ..., image: _Optional[str] = ..., type: _Optional[_Union[Space.Type, str]] = ..., plan: _Optional[str] = ..., visibility: _Optional[_Union[Space.Visibility, str]] = ..., membership: _Optional[_Union[Space.Membership, str]] = ..., min_team_size: _Optional[int] = ..., max_team_size: _Optional[int] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., key: _Optional[str] = ..., url: _Optional[str] = ..., name: _Optional[str] = ..., image: _Optional[str] = ..., type: _Optional[_Union[Space.Type, str]] = ..., plan: _Optional[str] = ..., visibility: _Optional[_Union[Space.Visibility, str]] = ..., membership: _Optional[_Union[Space.Membership, str]] = ..., min_team_size: _Optional[int] = ..., max_team_size: _Optional[int] = ..., permissions: _Optional[_Iterable[str]] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/universe/universe_http.py` & `eolymp-0.8.1/eolymp/universe/universe_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/universe/universe_pb2.py` & `eolymp-0.8.1/eolymp/universe/universe_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from eolymp.annotations import ratelimit_pb2 as eolymp_dot_annotations_dot_ratelimit__pb2
 from eolymp.annotations import scope_pb2 as eolymp_dot_annotations_dot_scope__pb2
 from eolymp.universe import permission_pb2 as eolymp_dot_universe_dot_permission__pb2
 from eolymp.universe import space_pb2 as eolymp_dot_universe_dot_space__pb2
 from eolymp.wellknown import expression_pb2 as eolymp_dot_wellknown_dot_expression__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/universe/universe.proto\x12\x0f\x65olymp.universe\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/universe/permission.proto\x1a\x1b\x65olymp/universe/space.proto\x1a!eolymp/wellknown/expression.proto\"9\n\x10\x43reateSpaceInput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"%\n\x11\x43reateSpaceOutput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"K\n\x10UpdateSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12%\n\x05space\x18\x02 \x01(\x0b\x32\x16.eolymp.universe.Space\"\x13\n\x11UpdateSpaceOutput\"$\n\x10\x44\x65leteSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"\x13\n\x11\x44\x65leteSpaceOutput\"\x1f\n\x10LookupSpaceInput\x12\x0b\n\x03key\x18\x01 \x01(\t\":\n\x11LookupSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"<\n\x13\x44\x65scribeSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeQuotaInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"B\n\x13\x44\x65scribeQuotaOutput\x12+\n\x05quota\x18\x01 \x01(\x0b\x32\x1c.eolymp.universe.Space.Quota\"Q\n\x10UpdateQuotaInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12+\n\x05quota\x18\x02 \x01(\x0b\x32\x1c.eolymp.universe.Space.Quota\"\x13\n\x11UpdateQuotaOutput\"\xef\x02\n\x0fListSpacesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x38\n\x07\x66ilters\x18( \x01(\x0b\x32\'.eolymp.universe.ListSpacesInput.Filter\x1a\x83\x02\n\x06\x46ilter\x12\r\n\x05query\x18\x64 \x01(\t\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12+\n\x03key\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12-\n\x03own\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\x12\x30\n\x06member\x18\x05 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"H\n\x10ListSpacesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12%\n\x05items\x18\x02 \x03(\x0b\x32\x16.eolymp.universe.Space\"i\n\x14GrantPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12.\n\x04role\x18\x02 \x01(\x0e\x32 .eolymp.universe.Permission.Role\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x17\n\x15GrantPermissionOutput\":\n\x15RevokePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x18\n\x16RevokePermissionOutput\"<\n\x17\x44\x65scribePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\"K\n\x18\x44\x65scribePermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"-\n\x19IntrospectPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"M\n\x1aIntrospectPermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"\x9d\x02\n\x14ListPermissionsInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.universe.ListPermissionsInput.Filter\x1a\x95\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12/\n\x07user_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12.\n\x04role\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"R\n\x15ListPermissionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.universe.Permission2\xbf\x10\n\x08Universe\x12\x83\x01\n\x0bLookupSpace\x12!.eolymp.universe.LookupSpaceInput\x1a\".eolymp.universe.LookupSpaceOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/spaces/__lookup/{key}\x12\x90\x01\n\x0b\x43reateSpace\x12!.eolymp.universe.CreateSpaceInput\x1a\".eolymp.universe.CreateSpaceOutput\":\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\t\"\x07/spaces\x12\x9b\x01\n\x0bUpdateSpace\x12!.eolymp.universe.UpdateSpaceInput\x1a\".eolymp.universe.UpdateSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x14\x1a\x12/spaces/{space_id}\x12\x9b\x01\n\x0b\x44\x65leteSpace\x12!.eolymp.universe.DeleteSpaceInput\x1a\".eolymp.universe.DeleteSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x14*\x12/spaces/{space_id}\x12\x85\x01\n\rDescribeSpace\x12#.eolymp.universe.DescribeSpaceInput\x1a$.eolymp.universe.DescribeSpaceOutput\")\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x14\x12\x12/spaces/{space_id}\x12\x8b\x01\n\rDescribeQuota\x12#.eolymp.universe.DescribeQuotaInput\x1a$.eolymp.universe.DescribeQuotaOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1a\x12\x18/spaces/{space_id}/quota\x12\x85\x01\n\x0bUpdateQuota\x12!.eolymp.universe.UpdateQuotaInput\x1a\".eolymp.universe.UpdateQuotaOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1a\x1a\x18/spaces/{space_id}/quota\x12\x8c\x01\n\nListSpaces\x12 .eolymp.universe.ListSpacesInput\x1a!.eolymp.universe.ListSpacesOutput\"9\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\t\x12\x07/spaces\x12\xbd\x01\n\x0fGrantPermission\x12%.eolymp.universe.GrantPermissionInput\x1a&.eolymp.universe.GrantPermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x1a(/spaces/{space_id}/permissions/{user_id}\x12\xc0\x01\n\x10RevokePermission\x12&.eolymp.universe.RevokePermissionInput\x1a\'.eolymp.universe.RevokePermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02**(/spaces/{space_id}/permissions/{user_id}\x12\xc5\x01\n\x12\x44\x65scribePermission\x12(.eolymp.universe.DescribePermissionInput\x1a).eolymp.universe.DescribePermissionOutput\"Z\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/permissions/{user_id}\x12\xb0\x01\n\x14IntrospectPermission\x12*.eolymp.universe.IntrospectPermissionInput\x1a+.eolymp.universe.IntrospectPermissionOutput\"?\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/introspect-permission\x12\xb2\x01\n\x0fListPermissions\x12%.eolymp.universe.ListPermissionsInput\x1a&.eolymp.universe.ListPermissionsOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02 \x12\x1e/spaces/{space_id}/permissionsB3Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1e\x65olymp/universe/universe.proto\x12\x0f\x65olymp.universe\x1a\x1d\x65olymp/annotations/http.proto\x1a\"eolymp/annotations/ratelimit.proto\x1a\x1e\x65olymp/annotations/scope.proto\x1a eolymp/universe/permission.proto\x1a\x1b\x65olymp/universe/space.proto\x1a!eolymp/wellknown/expression.proto\"9\n\x10\x43reateSpaceInput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"%\n\x11\x43reateSpaceOutput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"K\n\x10UpdateSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12%\n\x05space\x18\x02 \x01(\x0b\x32\x16.eolymp.universe.Space\"\x13\n\x11UpdateSpaceOutput\"$\n\x10\x44\x65leteSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"\x13\n\x11\x44\x65leteSpaceOutput\"\x1f\n\x10LookupSpaceInput\x12\x0b\n\x03key\x18\x01 \x01(\t\":\n\x11LookupSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeSpaceInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"<\n\x13\x44\x65scribeSpaceOutput\x12%\n\x05space\x18\x01 \x01(\x0b\x32\x16.eolymp.universe.Space\"&\n\x12\x44\x65scribeQuotaInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"B\n\x13\x44\x65scribeQuotaOutput\x12+\n\x05quota\x18\x01 \x01(\x0b\x32\x1c.eolymp.universe.Space.Quota\"Q\n\x10UpdateQuotaInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12+\n\x05quota\x18\x02 \x01(\x0b\x32\x1c.eolymp.universe.Space.Quota\"\x13\n\x11UpdateQuotaOutput\"\xbd\x02\n\x0fListSpacesInput\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12\x38\n\x07\x66ilters\x18( \x01(\x0b\x32\'.eolymp.universe.ListSpacesInput.Filter\x1a\xd1\x01\n\x06\x46ilter\x12\r\n\x05query\x18\x64 \x01(\t\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12+\n\x03key\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12\x30\n\x04name\x18\x03 \x03(\x0b\x32\".eolymp.wellknown.ExpressionString\x12-\n\x03own\x18\x04 \x03(\x0b\x32 .eolymp.wellknown.ExpressionBool\"H\n\x10ListSpacesOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12%\n\x05items\x18\x02 \x03(\x0b\x32\x16.eolymp.universe.Space\"i\n\x14GrantPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12.\n\x04role\x18\x02 \x01(\x0e\x32 .eolymp.universe.Permission.Role\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x17\n\x15GrantPermissionOutput\":\n\x15RevokePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x03 \x01(\t\"\x18\n\x16RevokePermissionOutput\"<\n\x17\x44\x65scribePermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0f\n\x07user_id\x18\x02 \x01(\t\"K\n\x18\x44\x65scribePermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"-\n\x19IntrospectPermissionInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\"M\n\x1aIntrospectPermissionOutput\x12/\n\npermission\x18\x01 \x01(\x0b\x32\x1b.eolymp.universe.Permission\"\x9d\x02\n\x14ListPermissionsInput\x12\x10\n\x08space_id\x18\x01 \x01(\t\x12\x0e\n\x06offset\x18\n \x01(\x05\x12\x0c\n\x04size\x18\x0b \x01(\x05\x12=\n\x07\x66ilters\x18( \x01(\x0b\x32,.eolymp.universe.ListPermissionsInput.Filter\x1a\x95\x01\n\x06\x46ilter\x12*\n\x02id\x18\x01 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12/\n\x07user_id\x18\x02 \x03(\x0b\x32\x1e.eolymp.wellknown.ExpressionID\x12.\n\x04role\x18\x03 \x03(\x0b\x32 .eolymp.wellknown.ExpressionEnum\"R\n\x15ListPermissionsOutput\x12\r\n\x05total\x18\x01 \x01(\x05\x12*\n\x05items\x18\x02 \x03(\x0b\x32\x1b.eolymp.universe.Permission2\xbf\x10\n\x08Universe\x12\x83\x01\n\x0bLookupSpace\x12!.eolymp.universe.LookupSpaceInput\x1a\".eolymp.universe.LookupSpaceOutput\"-\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x18\x12\x16/spaces/__lookup/{key}\x12\x90\x01\n\x0b\x43reateSpace\x12!.eolymp.universe.CreateSpaceInput\x1a\".eolymp.universe.CreateSpaceOutput\":\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\t\"\x07/spaces\x12\x9b\x01\n\x0bUpdateSpace\x12!.eolymp.universe.UpdateSpaceInput\x1a\".eolymp.universe.UpdateSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x80?\xf8\xe2\n\x05\x82\xd3\xe4\x93\x02\x14\x1a\x12/spaces/{space_id}\x12\x9b\x01\n\x0b\x44\x65leteSpace\x12!.eolymp.universe.DeleteSpaceInput\x1a\".eolymp.universe.DeleteSpaceOutput\"E\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\x00@\xf8\xe2\n\n\x82\xd3\xe4\x93\x02\x14*\x12/spaces/{space_id}\x12\x85\x01\n\rDescribeSpace\x12#.eolymp.universe.DescribeSpaceInput\x1a$.eolymp.universe.DescribeSpaceOutput\")\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x14\x12\x12/spaces/{space_id}\x12\x8b\x01\n\rDescribeQuota\x12#.eolymp.universe.DescribeQuotaInput\x1a$.eolymp.universe.DescribeQuotaOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1a\x12\x18/spaces/{space_id}/quota\x12\x85\x01\n\x0bUpdateQuota\x12!.eolymp.universe.UpdateQuotaInput\x1a\".eolymp.universe.UpdateQuotaOutput\"/\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\nd\x82\xd3\xe4\x93\x02\x1a\x1a\x18/spaces/{space_id}/quota\x12\x8c\x01\n\nListSpaces\x12 .eolymp.universe.ListSpacesInput\x1a!.eolymp.universe.ListSpacesOutput\"9\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02\t\x12\x07/spaces\x12\xbd\x01\n\x0fGrantPermission\x12%.eolymp.universe.GrantPermissionInput\x1a&.eolymp.universe.GrantPermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x1a(/spaces/{space_id}/permissions/{user_id}\x12\xc0\x01\n\x10RevokePermission\x12&.eolymp.universe.RevokePermissionInput\x1a\'.eolymp.universe.RevokePermissionOutput\"[\x82\xe3\n\x18\x8a\xe3\n\x14universe:space:write\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02**(/spaces/{space_id}/permissions/{user_id}\x12\xc5\x01\n\x12\x44\x65scribePermission\x12(.eolymp.universe.DescribePermissionInput\x1a).eolymp.universe.DescribePermissionOutput\"Z\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/permissions/{user_id}\x12\xb0\x01\n\x14IntrospectPermission\x12*.eolymp.universe.IntrospectPermissionInput\x1a+.eolymp.universe.IntrospectPermissionOutput\"?\xea\xe2\n\x0b\xf5\xe2\n\x00\x00 A\xf8\xe2\n2\x82\xd3\xe4\x93\x02*\x12(/spaces/{space_id}/introspect-permission\x12\xb2\x01\n\x0fListPermissions\x12%.eolymp.universe.ListPermissionsInput\x1a&.eolymp.universe.ListPermissionsOutput\"P\x82\xe3\n\x17\x8a\xe3\n\x13universe:space:read\xea\xe2\n\x0b\xf5\xe2\n\x00\x00\xa0@\xf8\xe2\n\x14\x82\xd3\xe4\x93\x02 \x12\x1e/spaces/{space_id}/permissionsB3Z1github.com/eolymp/go-sdk/eolymp/universe;universeb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'eolymp.universe.universe_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'Z1github.com/eolymp/go-sdk/eolymp/universe;universe'
@@ -78,37 +78,37 @@
   _DESCRIBEQUOTAOUTPUT._serialized_start=738
   _DESCRIBEQUOTAOUTPUT._serialized_end=804
   _UPDATEQUOTAINPUT._serialized_start=806
   _UPDATEQUOTAINPUT._serialized_end=887
   _UPDATEQUOTAOUTPUT._serialized_start=889
   _UPDATEQUOTAOUTPUT._serialized_end=908
   _LISTSPACESINPUT._serialized_start=911
-  _LISTSPACESINPUT._serialized_end=1278
+  _LISTSPACESINPUT._serialized_end=1228
   _LISTSPACESINPUT_FILTER._serialized_start=1019
-  _LISTSPACESINPUT_FILTER._serialized_end=1278
-  _LISTSPACESOUTPUT._serialized_start=1280
-  _LISTSPACESOUTPUT._serialized_end=1352
-  _GRANTPERMISSIONINPUT._serialized_start=1354
-  _GRANTPERMISSIONINPUT._serialized_end=1459
-  _GRANTPERMISSIONOUTPUT._serialized_start=1461
-  _GRANTPERMISSIONOUTPUT._serialized_end=1484
-  _REVOKEPERMISSIONINPUT._serialized_start=1486
-  _REVOKEPERMISSIONINPUT._serialized_end=1544
-  _REVOKEPERMISSIONOUTPUT._serialized_start=1546
-  _REVOKEPERMISSIONOUTPUT._serialized_end=1570
-  _DESCRIBEPERMISSIONINPUT._serialized_start=1572
-  _DESCRIBEPERMISSIONINPUT._serialized_end=1632
-  _DESCRIBEPERMISSIONOUTPUT._serialized_start=1634
-  _DESCRIBEPERMISSIONOUTPUT._serialized_end=1709
-  _INTROSPECTPERMISSIONINPUT._serialized_start=1711
-  _INTROSPECTPERMISSIONINPUT._serialized_end=1756
-  _INTROSPECTPERMISSIONOUTPUT._serialized_start=1758
-  _INTROSPECTPERMISSIONOUTPUT._serialized_end=1835
-  _LISTPERMISSIONSINPUT._serialized_start=1838
-  _LISTPERMISSIONSINPUT._serialized_end=2123
-  _LISTPERMISSIONSINPUT_FILTER._serialized_start=1974
-  _LISTPERMISSIONSINPUT_FILTER._serialized_end=2123
-  _LISTPERMISSIONSOUTPUT._serialized_start=2125
-  _LISTPERMISSIONSOUTPUT._serialized_end=2207
-  _UNIVERSE._serialized_start=2210
-  _UNIVERSE._serialized_end=4321
+  _LISTSPACESINPUT_FILTER._serialized_end=1228
+  _LISTSPACESOUTPUT._serialized_start=1230
+  _LISTSPACESOUTPUT._serialized_end=1302
+  _GRANTPERMISSIONINPUT._serialized_start=1304
+  _GRANTPERMISSIONINPUT._serialized_end=1409
+  _GRANTPERMISSIONOUTPUT._serialized_start=1411
+  _GRANTPERMISSIONOUTPUT._serialized_end=1434
+  _REVOKEPERMISSIONINPUT._serialized_start=1436
+  _REVOKEPERMISSIONINPUT._serialized_end=1494
+  _REVOKEPERMISSIONOUTPUT._serialized_start=1496
+  _REVOKEPERMISSIONOUTPUT._serialized_end=1520
+  _DESCRIBEPERMISSIONINPUT._serialized_start=1522
+  _DESCRIBEPERMISSIONINPUT._serialized_end=1582
+  _DESCRIBEPERMISSIONOUTPUT._serialized_start=1584
+  _DESCRIBEPERMISSIONOUTPUT._serialized_end=1659
+  _INTROSPECTPERMISSIONINPUT._serialized_start=1661
+  _INTROSPECTPERMISSIONINPUT._serialized_end=1706
+  _INTROSPECTPERMISSIONOUTPUT._serialized_start=1708
+  _INTROSPECTPERMISSIONOUTPUT._serialized_end=1785
+  _LISTPERMISSIONSINPUT._serialized_start=1788
+  _LISTPERMISSIONSINPUT._serialized_end=2073
+  _LISTPERMISSIONSINPUT_FILTER._serialized_start=1924
+  _LISTPERMISSIONSINPUT_FILTER._serialized_end=2073
+  _LISTPERMISSIONSOUTPUT._serialized_start=2075
+  _LISTPERMISSIONSOUTPUT._serialized_end=2157
+  _UNIVERSE._serialized_start=2160
+  _UNIVERSE._serialized_end=4271
 # @@protoc_insertion_point(module_scope)
```

### Comparing `eolymp-0.8.0/eolymp/universe/universe_pb2.pyi` & `eolymp-0.8.1/eolymp/universe/universe_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -125,28 +125,26 @@
     items: _containers.RepeatedCompositeFieldContainer[_permission_pb2.Permission]
     total: int
     def __init__(self, total: _Optional[int] = ..., items: _Optional[_Iterable[_Union[_permission_pb2.Permission, _Mapping]]] = ...) -> None: ...
 
 class ListSpacesInput(_message.Message):
     __slots__ = ["filters", "offset", "size"]
     class Filter(_message.Message):
-        __slots__ = ["id", "key", "member", "name", "own", "query"]
+        __slots__ = ["id", "key", "name", "own", "query"]
         ID_FIELD_NUMBER: _ClassVar[int]
         KEY_FIELD_NUMBER: _ClassVar[int]
-        MEMBER_FIELD_NUMBER: _ClassVar[int]
         NAME_FIELD_NUMBER: _ClassVar[int]
         OWN_FIELD_NUMBER: _ClassVar[int]
         QUERY_FIELD_NUMBER: _ClassVar[int]
         id: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionID]
         key: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionID]
-        member: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionBool]
         name: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionString]
         own: _containers.RepeatedCompositeFieldContainer[_expression_pb2.ExpressionBool]
         query: str
-        def __init__(self, query: _Optional[str] = ..., id: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., key: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., name: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., own: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ..., member: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ...) -> None: ...
+        def __init__(self, query: _Optional[str] = ..., id: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., key: _Optional[_Iterable[_Union[_expression_pb2.ExpressionID, _Mapping]]] = ..., name: _Optional[_Iterable[_Union[_expression_pb2.ExpressionString, _Mapping]]] = ..., own: _Optional[_Iterable[_Union[_expression_pb2.ExpressionBool, _Mapping]]] = ...) -> None: ...
     FILTERS_FIELD_NUMBER: _ClassVar[int]
     OFFSET_FIELD_NUMBER: _ClassVar[int]
     SIZE_FIELD_NUMBER: _ClassVar[int]
     filters: ListSpacesInput.Filter
     offset: int
     size: int
     def __init__(self, offset: _Optional[int] = ..., size: _Optional[int] = ..., filters: _Optional[_Union[ListSpacesInput.Filter, _Mapping]] = ...) -> None: ...
```

### Comparing `eolymp-0.8.0/eolymp/wellknown/errors_pb2.py` & `eolymp-0.8.1/eolymp/wellknown/errors_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/wellknown/errors_pb2.pyi` & `eolymp-0.8.1/eolymp/wellknown/errors_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/wellknown/expression_pb2.py` & `eolymp-0.8.1/eolymp/wellknown/expression_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/wellknown/expression_pb2.pyi` & `eolymp-0.8.1/eolymp/wellknown/expression_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/worker/job_pb2.py` & `eolymp-0.8.1/eolymp/worker/job_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/worker/worker_service_http.py` & `eolymp-0.8.1/eolymp/worker/worker_service_http.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/worker/worker_service_pb2.py` & `eolymp-0.8.1/eolymp/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp/worker/worker_service_pb2.pyi` & `eolymp-0.8.1/eolymp/worker/worker_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `eolymp-0.8.0/eolymp.egg-info/PKG-INFO` & `eolymp-0.8.1/eolymp.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eolymp
-Version: 0.8.0
+Version: 0.8.1
 Summary: Eolymp SDK for Python
 Home-page: https://github.com/eolymp/contracts
 Author: Sergey Kolodyazhnyy
 Author-email: sergey@eolymp.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `eolymp-0.8.0/eolymp.egg-info/SOURCES.txt` & `eolymp-0.8.1/eolymp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -5,14 +5,17 @@
 eolymp.egg-info/SOURCES.txt
 eolymp.egg-info/dependency_links.txt
 eolymp.egg-info/top_level.txt
 eolymp/acl/__init__.py
 eolymp/acl/acl_service_http.py
 eolymp/acl/acl_service_pb2.py
 eolymp/acl/acl_service_pb2.pyi
+eolymp/acl/entitlement_service_http.py
+eolymp/acl/entitlement_service_pb2.py
+eolymp/acl/entitlement_service_pb2.pyi
 eolymp/annotations/__init__.py
 eolymp/annotations/endpoint_pb2.py
 eolymp/annotations/endpoint_pb2.pyi
 eolymp/annotations/http_pb2.py
 eolymp/annotations/http_pb2.pyi
 eolymp/annotations/ratelimit_pb2.py
 eolymp/annotations/ratelimit_pb2.pyi
@@ -21,14 +24,17 @@
 eolymp/apollo/__init__.py
 eolymp/apollo/events_pb2.py
 eolymp/apollo/events_pb2.pyi
 eolymp/asset/__init__.py
 eolymp/asset/asset_http.py
 eolymp/asset/asset_pb2.py
 eolymp/asset/asset_pb2.pyi
+eolymp/asset/asset_service_http.py
+eolymp/asset/asset_service_pb2.py
+eolymp/asset/asset_service_pb2.pyi
 eolymp/atlas/__init__.py
 eolymp/atlas/asset_service_http.py
 eolymp/atlas/asset_service_pb2.py
 eolymp/atlas/asset_service_pb2.pyi
 eolymp/atlas/atlas_http.py
 eolymp/atlas/atlas_pb2.py
 eolymp/atlas/atlas_pb2.pyi
@@ -105,16 +111,14 @@
 eolymp/auth/sso_service_pb2.pyi
 eolymp/cognito/__init__.py
 eolymp/cognito/access_key_pb2.py
 eolymp/cognito/access_key_pb2.pyi
 eolymp/cognito/cognito_http.py
 eolymp/cognito/cognito_pb2.py
 eolymp/cognito/cognito_pb2.pyi
-eolymp/cognito/entitlement_pb2.py
-eolymp/cognito/entitlement_pb2.pyi
 eolymp/cognito/quota_pb2.py
 eolymp/cognito/quota_pb2.pyi
 eolymp/cognito/user_pb2.py
 eolymp/cognito/user_pb2.pyi
 eolymp/community/__init__.py
 eolymp/community/account_service_http.py
 eolymp/community/account_service_pb2.py
@@ -141,14 +145,20 @@
 eolymp/community/member_team_pb2.py
 eolymp/community/member_team_pb2.pyi
 eolymp/community/member_user_pb2.py
 eolymp/community/member_user_pb2.pyi
 eolymp/community/membership_service_http.py
 eolymp/community/membership_service_pb2.py
 eolymp/community/membership_service_pb2.pyi
+eolymp/content/__init__.py
+eolymp/content/content_service_http.py
+eolymp/content/content_service_pb2.py
+eolymp/content/content_service_pb2.pyi
+eolymp/content/fragment_pb2.py
+eolymp/content/fragment_pb2.pyi
 eolymp/core/__init__.py
 eolymp/core/http_client.py
 eolymp/core/oauth_client.py
 eolymp/discussion/__init__.py
 eolymp/discussion/discussion_pb2.py
 eolymp/discussion/discussion_pb2.pyi
 eolymp/discussion/discussion_service_http.py
@@ -237,16 +247,14 @@
 eolymp/judge/acl_pb2.pyi
 eolymp/judge/activity_pb2.py
 eolymp/judge/activity_pb2.pyi
 eolymp/judge/announcement_pb2.py
 eolymp/judge/announcement_pb2.pyi
 eolymp/judge/contest_pb2.py
 eolymp/judge/contest_pb2.pyi
-eolymp/judge/entitlement_pb2.py
-eolymp/judge/entitlement_pb2.pyi
 eolymp/judge/events_pb2.py
 eolymp/judge/events_pb2.pyi
 eolymp/judge/judge_http.py
 eolymp/judge/judge_pb2.py
 eolymp/judge/judge_pb2.pyi
 eolymp/judge/participant_pb2.py
 eolymp/judge/participant_pb2.pyi
```

### Comparing `eolymp-0.8.0/setup.py` & `eolymp-0.8.1/setup.py`

 * *Files identical despite different names*

