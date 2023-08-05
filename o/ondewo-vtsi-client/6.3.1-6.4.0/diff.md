# Comparing `tmp/ondewo-vtsi-client-6.3.1.tar.gz` & `tmp/ondewo-vtsi-client-6.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ondewo-vtsi-client-6.3.1.tar", last modified: Fri Aug  4 06:02:43 2023, max compression
+gzip compressed data, was "ondewo-vtsi-client-6.4.0.tar", last modified: Sat Aug  5 17:45:00 2023, max compression
```

## Comparing `ondewo-vtsi-client-6.3.1.tar` & `ondewo-vtsi-client-6.4.0.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.458045 ondewo-vtsi-client-6.3.1/
--rw-rw-r--   0 root         (0) root         (0)    10257 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/LICENSE
--rw-rw-r--   0 root         (0) root         (0)       71 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     9088 2023-08-04 06:02:43.458045 ondewo-vtsi-client-6.3.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     8516 2023-01-28 16:53:50.000000 ondewo-vtsi-client-6.3.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.452045 ondewo-vtsi-client-6.3.1/ondewo/
--rw-rw-r--   0 root         (0) root         (0)       81 2022-12-09 10:08:28.000000 ondewo-vtsi-client-6.3.1/ondewo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.455045 ondewo-vtsi-client-6.3.1/ondewo/nlu/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    73267 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/agent_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    87204 2023-08-04 06:02:36.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/agent_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    28593 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/aiservices_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16826 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/aiservices_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     1592 2023-08-04 06:02:36.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/common_pb2.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/common_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    10331 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/context_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14789 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/context_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    29810 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/entity_type_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    36069 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/entity_type_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    71700 2023-08-04 06:02:36.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/intent_pb2.py
--rw-r--r--   0 root         (0) root         (0)    59591 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/intent_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)     3354 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/operation_metadata_pb2.py
--rw-r--r--   0 root         (0) root         (0)      158 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/operation_metadata_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7876 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/operations_pb2.py
--rw-r--r--   0 root         (0) root         (0)    11374 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/operations_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     9514 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/project_role_pb2.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/project_role_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     7450 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/project_statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16562 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/project_statistics_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     3001 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/server_statistics_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6634 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/server_statistics_pb2_grpc.py
--rw-rw-r--   0 root         (0) root         (0)    65793 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/session_pb2.py
--rw-r--r--   0 root         (0) root         (0)    59122 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/session_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    19597 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/user_pb2.py
--rw-r--r--   0 root         (0) root         (0)    27124 2023-08-04 06:02:36.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/user_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)    20143 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/utility_pb2.py
--rw-r--r--   0 root         (0) root         (0)    16902 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/utility_pb2_grpc.py
--rw-r--r--   0 root         (0) root         (0)     6345 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/webhook_pb2.py
--rw-r--r--   0 root         (0) root         (0)     6508 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/nlu/webhook_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.456045 ondewo-vtsi-client-6.3.1/ondewo/qa/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/qa/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11401 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/qa/qa_pb2.py
--rw-r--r--   0 root         (0) root         (0)    13389 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/qa/qa_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.456045 ondewo-vtsi-client-6.3.1/ondewo/s2t/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/s2t/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    38422 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/s2t/speech_to_text_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    30933 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/s2t/speech_to_text_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.456045 ondewo-vtsi-client-6.3.1/ondewo/sip/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/sip/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    10949 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/sip/sip_pb2.py
--rw-rw-r--   0 root         (0) root         (0)    21323 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/sip/sip_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.457045 ondewo-vtsi-client-6.3.1/ondewo/t2s/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/t2s/__init__.py
--rw-r--r--   0 root         (0) root         (0)    31234 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/t2s/text_to_speech_pb2.py
--rw-r--r--   0 root         (0) root         (0)    33144 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/t2s/text_to_speech_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.457045 ondewo-vtsi-client-6.3.1/ondewo/vtsi/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42646 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/calls_pb2.py
--rw-r--r--   0 root         (0) root         (0)    29068 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/calls_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.457045 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/
--rw-rw-r--   0 root         (0) root         (0)        0 2023-01-24 18:48:07.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/__init__.py
--rw-rw-r--   0 root         (0) root         (0)      735 2023-01-29 01:16:45.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/client.py
--rw-rw-r--   0 root         (0) root         (0)      263 2023-01-29 00:08:08.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/client_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.458045 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/services/
--rw-rw-r--   0 root         (0) root         (0)        0 2022-12-09 10:08:28.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/services/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     3734 2023-01-29 00:41:36.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/services/calls.py
--rw-rw-r--   0 root         (0) root         (0)     2357 2023-08-04 05:58:12.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/services/projects.py
--rw-rw-r--   0 root         (0) root         (0)      317 2023-01-29 01:19:24.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/services_container.py
--rw-r--r--   0 root         (0) root         (0)    17004 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/projects_pb2.py
--rw-r--r--   0 root         (0) root         (0)    14451 2023-08-04 06:02:35.000000 ondewo-vtsi-client-6.3.1/ondewo/vtsi/projects_pb2_grpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-04 06:02:43.458045 ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/
--rw-r--r--   0 root         (0) root         (0)     9088 2023-08-04 06:02:43.000000 ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1955 2023-08-04 06:02:43.000000 ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-04 06:02:43.000000 ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      211 2023-08-04 06:02:43.000000 ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-08-04 06:02:43.000000 ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/top_level.txt
--rw-rw-r--   0 root         (0) root         (0)       67 2023-08-04 06:02:43.458045 ondewo-vtsi-client-6.3.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)     1586 2023-08-04 06:02:39.000000 ondewo-vtsi-client-6.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/
+-rw-rw-r--   0 root         (0) root         (0)    10257 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)       71 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     8516 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.142465 ondewo-vtsi-client-6.4.0/ondewo/
+-rw-rw-r--   0 root         (0) root         (0)       81 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/nlu/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    73267 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    87204 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    28593 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16826 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     1592 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/common_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/common_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    10331 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14789 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    29810 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    36069 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    71700 2023-08-05 17:44:43.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59591 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3354 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operation_metadata_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)      158 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operation_metadata_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7876 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    11374 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     9514 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    10478 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     7450 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16562 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     3001 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6634 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    65793 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    59122 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    19597 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    27124 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)    20143 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    16902 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2_grpc.py
+-rw-rw-r--   0 root         (0) root         (0)     6345 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)     6508 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/qa/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/qa/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    11401 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    13389 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/s2t/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/s2t/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    38422 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    30933 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.145465 ondewo-vtsi-client-6.4.0/ondewo/sip/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/sip/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10949 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    21323 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/t2s/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/t2s/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    31234 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    33144 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/vtsi/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    47012 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    35863 2023-08-05 17:44:42.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)      735 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/client.py
+-rw-rw-r--   0 root         (0) root         (0)      263 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/client_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.146465 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    10991 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/calls.py
+-rw-rw-r--   0 root         (0) root         (0)     5017 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services/projects.py
+-rw-rw-r--   0 root         (0) root         (0)      317 2023-08-05 17:43:03.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/services_container.py
+-rw-rw-r--   0 root         (0) root         (0)    17177 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2.py
+-rw-rw-r--   0 root         (0) root         (0)    14451 2023-08-05 17:44:41.000000 ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2_grpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     9088 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1955 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      211 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-08-05 17:45:00.000000 ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0) root         (0)       67 2023-08-05 17:45:00.147465 ondewo-vtsi-client-6.4.0/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)     1586 2023-08-05 17:44:45.000000 ondewo-vtsi-client-6.4.0/setup.py
```

### Comparing `ondewo-vtsi-client-6.3.1/LICENSE` & `ondewo-vtsi-client-6.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/PKG-INFO` & `ondewo-vtsi-client-6.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.3.1
+Version: 6.4.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.3.1 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.4.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.3.1/README.md` & `ondewo-vtsi-client-6.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/agent_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/agent_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/agent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/aiservices_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/aiservices_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/aiservices_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/common_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/common_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/context_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/context_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/context_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/entity_type_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/entity_type_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/entity_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/intent_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/intent_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/intent_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/operation_metadata_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/operation_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/operations_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/operations_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/operations_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/project_role_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/project_role_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_role_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/project_statistics_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/project_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/project_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/server_statistics_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/server_statistics_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/server_statistics_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/session_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/session_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/session_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/user_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/user_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/utility_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/utility_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/utility_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/webhook_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/nlu/webhook_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/nlu/webhook_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/qa/qa_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/qa/qa_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/qa/qa_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/s2t/speech_to_text_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/s2t/speech_to_text_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/s2t/speech_to_text_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/sip/sip_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/sip/sip_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/sip/sip_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/t2s/text_to_speech_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/t2s/text_to_speech_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/t2s/text_to_speech_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/vtsi/calls_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,38 +3,40 @@
 # source: ondewo/vtsi/calls.proto
 """Generated protocol buffer code."""
 from ondewo.sip import sip_pb2 as ondewo_dot_sip_dot_sip__pb2
 from ondewo.t2s import text_to_speech_pb2 as ondewo_dot_t2s_dot_text__to__speech__pb2
 from ondewo.s2t import speech_to_text_pb2 as ondewo_dot_s2t_dot_speech__to__text__pb2
 from ondewo.nlu import context_pb2 as ondewo_dot_nlu_dot_context__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
+from google.protobuf import struct_pb2 as google_dot_protobuf_dot_struct__pb2
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 from google.api import annotations_pb2 as google_dot_api_dot_annotations__pb2
 from google.protobuf.internal import enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import message as _message
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17ondewo/vtsi/calls.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x18ondewo/nlu/context.proto\x1a\x1fondewo/s2t/speech-to-text.proto\x1a\x1fondewo/t2s/text-to-speech.proto\x1a\x14ondewo/sip/sip.proto\"B\n\x11\x42\x61seServiceConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x11\n\tgrpc_cert\x18\x03 \x01(\t\"5\n\x0b\x43redentials\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\xaa\x02\n\rNluVtsiConfig\x12\x37\n\x0fnlu_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12/\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x18.ondewo.vtsi.CredentialsH\x00\x12\x14\n\nauth_token\x18\x03 \x01(\tH\x00\x12\x12\n\nagent_name\x18\x04 \x01(\t\x12\x15\n\rlanguage_code\x18\x05 \x01(\t\x12\x16\n\x0einitial_intent\x18\x06 \x01(\t\x12%\n\x08\x63ontexts\x18\x07 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x1d\n\x15http_basic_auth_token\x18\x08 \x01(\tB\x10\n\x0e\x61uthentication\"\x7f\n\rT2sVtsiConfig\x12\x37\n\x0ft2s_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12\x35\n\x12t2s_request_config\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"\x94\x01\n\rS2tVtsiConfig\x12\x37\n\x0fs2t_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12J\n\x1ds2t_transcribe_request_config\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"N\n\x0e\x41steriskConfig\x12<\n\x14\x61sterisk_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\"\xea\x01\n\x14\x43ommonServicesConfig\x12\x33\n\x0fs2t_vtsi_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.S2tVtsiConfig\x12\x33\n\x0fnlu_vtsi_config\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.NluVtsiConfig\x12\x33\n\x0ft2s_vtsi_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.T2sVtsiConfig\x12\x33\n\x0f\x63si_vtsi_config\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.CsiVtsiConfig\"(\n\rSipBaseConfig\x12\x17\n\x0fsip_sim_version\x18\x01 \x01(\t\"\xcf\x01\n\x0fSipCallerConfig\x12\x33\n\x0fsip_base_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x11\n\tcallee_id\x18\x02 \x01(\t\x12\x41\n\x0bsip_headers\x18\x03 \x03(\x0b\x32,.ondewo.vtsi.SipCallerConfig.SipHeadersEntry\x1a\x31\n\x0fSipHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xee\x02\n\rCsiVtsiConfig\x12\x39\n\x12s2t_vtsi_callbacks\x18\x01 \x01(\x0b\x32\x1d.ondewo.vtsi.S2tVtsiCallbacks\x12\x39\n\x12nlu_vtsi_callbacks\x18\x02 \x01(\x0b\x32\x1d.ondewo.vtsi.NluVtsiCallbacks\x12\x39\n\x12t2s_vtsi_callbacks\x18\x03 \x01(\x0b\x32\x1d.ondewo.vtsi.T2sVtsiCallbacks\x12H\n\x19\x61udio_object_store_config\x18\x04 \x01(\x0b\x32%.ondewo.vtsi.AudioObjectStorageConfig\x12?\n\x15message_broker_config\x18\x05 \x01(\x0b\x32 .ondewo.vtsi.MessageBrokerConfig\x12!\n\x19\x61\x63tivate_control_messages\x18\x06 \x01(\x08\"\xfd\x01\n\x18\x41udioObjectStorageConfig\x12%\n\x1d\x61\x63tivate_audio_object_storage\x18\x01 \x01(\x08\x12p\n/audio_object_storage_services_activation_config\x18\x02 \x01(\x0b\x32\x37.ondewo.vtsi.AudioObjectStorageServicesActivationConfig\x12\x30\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfigH\x00\x42\x16\n\x14\x61udio_storage_config\"X\n*AudioObjectStorageServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x02 \x01(\x08\"\xef\x01\n\x13MessageBrokerConfig\x12\x1f\n\x17\x61\x63tivate_message_broker\x18\x01 \x01(\x08\x12\x65\n)message_broker_services_activation_config\x18\x02 \x01(\x0b\x32\x32.ondewo.vtsi.MessageBrokerServicesActivationConfig\x12\x37\n\x10rabbit_mq_config\x18\x03 \x01(\x0b\x32\x1b.ondewo.vtsi.RabbitMqConfigH\x00\x42\x17\n\x15message_broker_config\"\x7f\n%MessageBrokerServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_nlu\x18\x02 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x03 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_sip\x18\x04 \x01(\x08\"\\\n\x0eRabbitMqConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0e\n\x06port_2\x18\x03 \x01(\x05\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x10\n\x08password\x18\x05 \x01(\t\"x\n\x0bMinioConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x12\n\naccess_key\x18\x03 \x01(\t\x12\x12\n\nsecret_key\x18\x04 \x01(\t\x12\x0e\n\x06secure\x18\x05 \x01(\x08\x12\x15\n\rsession_token\x18\x06 \x01(\t\"I\n\x10S2tVtsiCallbacks\x12\x19\n\x11pre_s2t_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_s2t_callbacks\x18\x02 \x03(\t\"I\n\x10NluVtsiCallbacks\x12\x19\n\x11pre_nlu_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_nlu_callbacks\x18\x02 \x03(\t\"I\n\x10T2sVtsiCallbacks\x12\x19\n\x11pre_t2s_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_t2s_callbacks\x18\x02 \x03(\t\"\xa3\x01\n\x08Listener\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x33\n\x0fsip_base_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"\xa5\x01\n\x06\x43\x61ller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x37\n\x11sip_caller_config\x18\x03 \x01(\x0b\x32\x1c.ondewo.vtsi.SipCallerConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"\xa9\x01\n\x14StartListenerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x33\n\x0fsip_base_config\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x03 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"r\n\x15StartListenerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\'\n\x08listener\x18\x02 \x01(\x0b\x32\x15.ondewo.vtsi.Listener\x12\x15\n\rerror_message\x18\x03 \x01(\t\"p\n\x15StartListenersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12<\n\x11listener_requests\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.StartListenerRequest\"\x8a\x01\n\x16StartListenersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12>\n\x12listener_responses\x18\x02 \x03(\x0b\x32\".ondewo.vtsi.StartListenerResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\xab\x01\n\x12StartCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x37\n\x11sip_caller_config\x18\x02 \x01(\x0b\x32\x1c.ondewo.vtsi.SipCallerConfig\x12\x41\n\x16\x63ommon_services_config\x18\x03 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"l\n\x13StartCallerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12#\n\x06\x63\x61ller\x18\x02 \x01(\x0b\x32\x13.ondewo.vtsi.Caller\x12\x15\n\rerror_message\x18\x03 \x01(\t\"j\n\x13StartCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x38\n\x0f\x63\x61ller_requests\x18\x02 \x03(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\"\x84\x01\n\x14StartCallersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12:\n\x10\x63\x61ller_responses\x18\x02 \x03(\x0b\x32 .ondewo.vtsi.StartCallerResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\x9e\x01\n\x1bStartScheduledCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x30\n\x07request\x18\x02 \x01(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\x12\x32\n\x0escheduled_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x01\n\x1cStartScheduledCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12K\n\x19scheduled_caller_requests\x18\x02 \x03(\x0b\x32(.ondewo.vtsi.StartScheduledCallerRequest\"\x89\x01\n\x1dStartScheduledCallersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12M\n\x1ascheduled_caller_responses\x18\x02 \x03(\x0b\x32).ondewo.vtsi.StartScheduledCallerResponse\"\x88\x01\n\x1cStartScheduledCallerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x36\n\x10scheduled_caller\x18\x02 \x01(\x0b\x32\x1c.ondewo.vtsi.ScheduledCaller\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\xd9\x01\n\x0fScheduledCaller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12.\n\nsip_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\x12\x32\n\x0escheduled_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"?\n\x0fStopCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\"W\n\x10StopCallResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x15\n\rerror_message\x18\x03 \x01(\t\"A\n\x10StopCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x12\n\ncall_names\x18\x02 \x03(\t\"f\n\x11StopCallsResponse\x12:\n\x13stop_call_responses\x18\x01 \x03(\x0b\x32\x1d.ondewo.vtsi.StopCallResponse\x12\x15\n\rerror_message\x18\x02 \x01(\t\"0\n\x13StopAllCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\"X\n\x13TransferCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x13\n\x0btransfer_id\x18\x03 \x03(\t\"p\n\x14TransferCallResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x13\n\x0btransfer_id\x18\x03 \x01(\t\x12\x15\n\rerror_message\x18\x04 \x01(\t\"s\n\x14TransferCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12@\n\x16transfer_call_requests\x18\x02 \x03(\x0b\x32 .ondewo.vtsi.TransferCallRequest\"\x8d\x01\n\x15TransferCallsResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x42\n\x17transfer_call_responses\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.TransferCallResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"u\n\x12GetCallInfoRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x31\n\x0e\x63\x61ll_info_view\x18\x03 \x01(\x0e\x32\x19.ondewo.vtsi.CallInfoView\"j\n\x13GetCallInfoResponse\x12)\n\nactive_log\x18\x01 \x01(\x0b\x32\x15.ondewo.vtsi.CallInfo\x12(\n\tdone_logs\x18\x02 \x03(\x0b\x32\x15.ondewo.vtsi.CallInfo\"\x92\x03\n\x08\x43\x61llInfo\x12\x11\n\tcall_name\x18\x01 \x01(\t\x12\x13\n\x0bsip_account\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t\x12(\n\tcall_type\x18\x04 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\x12\x14\n\x0cphone_number\x18\x05 \x01(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12)\n\nsip_status\x18\x08 \x01(\x0b\x32\x15.ondewo.sip.SipStatus\x12@\n\x12sip_status_history\x18\t \x01(\x0b\x32$.ondewo.sip.SipStatusHistoryResponse\x12;\n\x11services_statuses\x18\n \x01(\x0b\x32 .ondewo.vtsi.AllServicesStatuses\"\x8d\x01\n\x13ListCallInfoRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x31\n\x0e\x63\x61ll_info_view\x18\x02 \x01(\x0e\x32\x19.ondewo.vtsi.CallInfoView\x12(\n\tcall_type\x18\x03 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\"A\n\x14ListCallInfoResponse\x12)\n\ncall_infos\x18\x01 \x03(\x0b\x32\x15.ondewo.vtsi.CallInfo\"\x8a\x02\n\x13\x41llServicesStatuses\x12.\n\nstatus_sip\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12\x33\n\x0fstatus_asterisk\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_nlu\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_stt\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_tts\x18\x05 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\"7\n\rServiceStatus\x12\x0f\n\x07healthy\x18\x01 \x01(\x08\x12\x15\n\rerror_message\x18\x02 \x01(\t\"o\n\x13GetAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x13\n\x0bobject_name\x18\x02 \x01(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"%\n\x14GetAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c\"\x80\x01\n#GetFullConversationAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x14\n\x0cobject_names\x18\x02 \x03(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"5\n$GetFullConversationAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c*%\n\x0c\x43\x61llInfoView\x12\x0b\n\x07SHALLOW\x10\x00\x12\x08\n\x04\x46ULL\x10\x01*.\n\x08\x43\x61llType\x12\x08\n\x04\x62oth\x10\x00\x12\x0c\n\x08listener\x10\x01\x12\n\n\x06\x63\x61ller\x10\x02\x32\xd6\n\n\x05\x43\x61lls\x12P\n\x0bStartCaller\x12\x1f.ondewo.vtsi.StartCallerRequest\x1a .ondewo.vtsi.StartCallerResponse\x12S\n\x0cStartCallers\x12 .ondewo.vtsi.StartCallersRequest\x1a!.ondewo.vtsi.StartCallersResponse\x12V\n\rStartListener\x12!.ondewo.vtsi.StartListenerRequest\x1a\".ondewo.vtsi.StartListenerResponse\x12Y\n\x0eStartListeners\x12\".ondewo.vtsi.StartListenersRequest\x1a#.ondewo.vtsi.StartListenersResponse\x12k\n\x14StartScheduledCaller\x12(.ondewo.vtsi.StartScheduledCallerRequest\x1a).ondewo.vtsi.StartScheduledCallerResponse\x12n\n\x15StartScheduledCallers\x12).ondewo.vtsi.StartScheduledCallersRequest\x1a*.ondewo.vtsi.StartScheduledCallersResponse\x12G\n\x08StopCall\x12\x1c.ondewo.vtsi.StopCallRequest\x1a\x1d.ondewo.vtsi.StopCallResponse\x12J\n\tStopCalls\x12\x1d.ondewo.vtsi.StopCallsRequest\x1a\x1e.ondewo.vtsi.StopCallsResponse\x12P\n\x0cStopAllCalls\x12 .ondewo.vtsi.StopAllCallsRequest\x1a\x1e.ondewo.vtsi.StopCallsResponse\x12S\n\x0cTransferCall\x12 .ondewo.vtsi.TransferCallRequest\x1a!.ondewo.vtsi.TransferCallResponse\x12V\n\rTransferCalls\x12!.ondewo.vtsi.TransferCallsRequest\x1a\".ondewo.vtsi.TransferCallsResponse\x12P\n\x0bGetCallInfo\x12\x1f.ondewo.vtsi.GetCallInfoRequest\x1a .ondewo.vtsi.GetCallInfoResponse\x12S\n\x0cListCallInfo\x12 .ondewo.vtsi.ListCallInfoRequest\x1a!.ondewo.vtsi.ListCallInfoResponse\x12S\n\x0cGetAudioFile\x12 .ondewo.vtsi.GetAudioFileRequest\x1a!.ondewo.vtsi.GetAudioFileResponse\x12\x85\x01\n\x1cGetFullConversationAudioFile\x12\x30.ondewo.vtsi.GetFullConversationAudioFileRequest\x1a\x31.ondewo.vtsi.GetFullConversationAudioFileResponse\"\x00\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17ondewo/vtsi/calls.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/api/annotations.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x18ondewo/nlu/context.proto\x1a\x1fondewo/s2t/speech-to-text.proto\x1a\x1fondewo/t2s/text-to-speech.proto\x1a\x14ondewo/sip/sip.proto\"B\n\x11\x42\x61seServiceConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x11\n\tgrpc_cert\x18\x03 \x01(\t\"5\n\x0b\x43redentials\x12\x14\n\x0c\x61\x63\x63ount_name\x18\x01 \x01(\t\x12\x10\n\x08password\x18\x02 \x01(\t\"\xaa\x02\n\rNluVtsiConfig\x12\x37\n\x0fnlu_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12/\n\x0b\x63redentials\x18\x02 \x01(\x0b\x32\x18.ondewo.vtsi.CredentialsH\x00\x12\x14\n\nauth_token\x18\x03 \x01(\tH\x00\x12\x12\n\nagent_name\x18\x04 \x01(\t\x12\x15\n\rlanguage_code\x18\x05 \x01(\t\x12\x16\n\x0einitial_intent\x18\x06 \x01(\t\x12%\n\x08\x63ontexts\x18\x07 \x03(\x0b\x32\x13.ondewo.nlu.Context\x12\x1d\n\x15http_basic_auth_token\x18\x08 \x01(\tB\x10\n\x0e\x61uthentication\"\x7f\n\rT2sVtsiConfig\x12\x37\n\x0ft2s_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12\x35\n\x12t2s_request_config\x18\x02 \x01(\x0b\x32\x19.ondewo.t2s.RequestConfig\"\x94\x01\n\rS2tVtsiConfig\x12\x37\n\x0fs2t_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\x12J\n\x1ds2t_transcribe_request_config\x18\x02 \x01(\x0b\x32#.ondewo.s2t.TranscribeRequestConfig\"N\n\x0e\x41steriskConfig\x12<\n\x14\x61sterisk_base_config\x18\x01 \x01(\x0b\x32\x1e.ondewo.vtsi.BaseServiceConfig\"\xea\x01\n\x14\x43ommonServicesConfig\x12\x33\n\x0fs2t_vtsi_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.S2tVtsiConfig\x12\x33\n\x0fnlu_vtsi_config\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.NluVtsiConfig\x12\x33\n\x0ft2s_vtsi_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.T2sVtsiConfig\x12\x33\n\x0f\x63si_vtsi_config\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.CsiVtsiConfig\"(\n\rSipBaseConfig\x12\x17\n\x0fsip_sim_version\x18\x01 \x01(\t\"\xcf\x01\n\x0fSipCallerConfig\x12\x33\n\x0fsip_base_config\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x11\n\tcallee_id\x18\x02 \x01(\t\x12\x41\n\x0bsip_headers\x18\x03 \x03(\x0b\x32,.ondewo.vtsi.SipCallerConfig.SipHeadersEntry\x1a\x31\n\x0fSipHeadersEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12\r\n\x05value\x18\x02 \x01(\t:\x02\x38\x01\"\xee\x02\n\rCsiVtsiConfig\x12\x39\n\x12s2t_vtsi_callbacks\x18\x01 \x01(\x0b\x32\x1d.ondewo.vtsi.S2tVtsiCallbacks\x12\x39\n\x12nlu_vtsi_callbacks\x18\x02 \x01(\x0b\x32\x1d.ondewo.vtsi.NluVtsiCallbacks\x12\x39\n\x12t2s_vtsi_callbacks\x18\x03 \x01(\x0b\x32\x1d.ondewo.vtsi.T2sVtsiCallbacks\x12H\n\x19\x61udio_object_store_config\x18\x04 \x01(\x0b\x32%.ondewo.vtsi.AudioObjectStorageConfig\x12?\n\x15message_broker_config\x18\x05 \x01(\x0b\x32 .ondewo.vtsi.MessageBrokerConfig\x12!\n\x19\x61\x63tivate_control_messages\x18\x06 \x01(\x08\"\xfd\x01\n\x18\x41udioObjectStorageConfig\x12%\n\x1d\x61\x63tivate_audio_object_storage\x18\x01 \x01(\x08\x12p\n/audio_object_storage_services_activation_config\x18\x02 \x01(\x0b\x32\x37.ondewo.vtsi.AudioObjectStorageServicesActivationConfig\x12\x30\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfigH\x00\x42\x16\n\x14\x61udio_storage_config\"X\n*AudioObjectStorageServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x02 \x01(\x08\"\xef\x01\n\x13MessageBrokerConfig\x12\x1f\n\x17\x61\x63tivate_message_broker\x18\x01 \x01(\x08\x12\x65\n)message_broker_services_activation_config\x18\x02 \x01(\x0b\x32\x32.ondewo.vtsi.MessageBrokerServicesActivationConfig\x12\x37\n\x10rabbit_mq_config\x18\x03 \x01(\x0b\x32\x1b.ondewo.vtsi.RabbitMqConfigH\x00\x42\x17\n\x15message_broker_config\"\x7f\n%MessageBrokerServicesActivationConfig\x12\x14\n\x0c\x61\x63tivate_s2t\x18\x01 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_nlu\x18\x02 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_t2s\x18\x03 \x01(\x08\x12\x14\n\x0c\x61\x63tivate_sip\x18\x04 \x01(\x08\"\\\n\x0eRabbitMqConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x0e\n\x06port_2\x18\x03 \x01(\x05\x12\x0c\n\x04user\x18\x04 \x01(\t\x12\x10\n\x08password\x18\x05 \x01(\t\"x\n\x0bMinioConfig\x12\x0c\n\x04host\x18\x01 \x01(\t\x12\x0c\n\x04port\x18\x02 \x01(\x05\x12\x12\n\naccess_key\x18\x03 \x01(\t\x12\x12\n\nsecret_key\x18\x04 \x01(\t\x12\x0e\n\x06secure\x18\x05 \x01(\x08\x12\x15\n\rsession_token\x18\x06 \x01(\t\"I\n\x10S2tVtsiCallbacks\x12\x19\n\x11pre_s2t_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_s2t_callbacks\x18\x02 \x03(\t\"I\n\x10NluVtsiCallbacks\x12\x19\n\x11pre_nlu_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_nlu_callbacks\x18\x02 \x03(\t\"I\n\x10T2sVtsiCallbacks\x12\x19\n\x11pre_t2s_callbacks\x18\x01 \x03(\t\x12\x1a\n\x12post_t2s_callbacks\x18\x02 \x03(\t\"\xa3\x01\n\x08Listener\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x33\n\x0fsip_base_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"\xa5\x01\n\x06\x43\x61ller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x37\n\x11sip_caller_config\x18\x03 \x01(\x0b\x32\x1c.ondewo.vtsi.SipCallerConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"\xa9\x01\n\x14StartListenerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x33\n\x0fsip_base_config\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x03 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"r\n\x15StartListenerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\'\n\x08listener\x18\x02 \x01(\x0b\x32\x15.ondewo.vtsi.Listener\x12\x15\n\rerror_message\x18\x03 \x01(\t\"p\n\x15StartListenersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12<\n\x11listener_requests\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.StartListenerRequest\"\x8a\x01\n\x16StartListenersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12>\n\x12listener_responses\x18\x02 \x03(\x0b\x32\".ondewo.vtsi.StartListenerResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\xab\x01\n\x12StartCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x37\n\x11sip_caller_config\x18\x02 \x01(\x0b\x32\x1c.ondewo.vtsi.SipCallerConfig\x12\x41\n\x16\x63ommon_services_config\x18\x03 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\"l\n\x13StartCallerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12#\n\x06\x63\x61ller\x18\x02 \x01(\x0b\x32\x13.ondewo.vtsi.Caller\x12\x15\n\rerror_message\x18\x03 \x01(\t\"j\n\x13StartCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x38\n\x0f\x63\x61ller_requests\x18\x02 \x03(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\"\x84\x01\n\x14StartCallersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12:\n\x10\x63\x61ller_responses\x18\x02 \x03(\x0b\x32 .ondewo.vtsi.StartCallerResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"W\n\x12ListCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x17\n\npage_token\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_page_token\";\n\x13ListCallersResponse\x12$\n\x07\x63\x61llers\x18\x01 \x03(\x0b\x32\x13.ondewo.vtsi.Caller\";\n\x10GetCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"Y\n\x14ListListenersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x17\n\npage_token\x18\x02 \x01(\tH\x00\x88\x01\x01\x42\r\n\x0b_page_token\"Z\n\x15ListListenersResponse\x12(\n\tlisteners\x18\x01 \x03(\x0b\x32\x15.ondewo.vtsi.Listener\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"=\n\x12GetListenerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\"\x9e\x01\n\x1bStartScheduledCallerRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x30\n\x07request\x18\x02 \x01(\x0b\x32\x1f.ondewo.vtsi.StartCallerRequest\x12\x32\n\x0escheduled_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\x86\x01\n\x1cStartScheduledCallersRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12K\n\x19scheduled_caller_requests\x18\x02 \x03(\x0b\x32(.ondewo.vtsi.StartScheduledCallerRequest\"\x89\x01\n\x1dStartScheduledCallersResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12M\n\x1ascheduled_caller_responses\x18\x02 \x03(\x0b\x32).ondewo.vtsi.StartScheduledCallerResponse\"\x88\x01\n\x1cStartScheduledCallerResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x36\n\x10scheduled_caller\x18\x02 \x01(\x0b\x32\x1c.ondewo.vtsi.ScheduledCaller\x12\x15\n\rerror_message\x18\x03 \x01(\t\"\xd9\x01\n\x0fScheduledCaller\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12.\n\nsip_config\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.SipBaseConfig\x12\x41\n\x16\x63ommon_services_config\x18\x04 \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfig\x12\x32\n\x0escheduled_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"?\n\x0fStopCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\"W\n\x10StopCallResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x15\n\rerror_message\x18\x03 \x01(\t\"A\n\x10StopCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x12\n\ncall_names\x18\x02 \x03(\t\"f\n\x11StopCallsResponse\x12:\n\x13stop_call_responses\x18\x01 \x03(\x0b\x32\x1d.ondewo.vtsi.StopCallResponse\x12\x15\n\rerror_message\x18\x02 \x01(\t\"0\n\x13StopAllCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\"X\n\x13TransferCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x13\n\x0btransfer_id\x18\x03 \x03(\t\"p\n\x14TransferCallResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12\x13\n\x0btransfer_id\x18\x03 \x01(\t\x12\x15\n\rerror_message\x18\x04 \x01(\t\"s\n\x14TransferCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12@\n\x16transfer_call_requests\x18\x02 \x03(\x0b\x32 .ondewo.vtsi.TransferCallRequest\"\x8d\x01\n\x15TransferCallsResponse\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x42\n\x17transfer_call_responses\x18\x02 \x03(\x0b\x32!.ondewo.vtsi.TransferCallResponse\x12\x15\n\rerror_message\x18\x03 \x01(\t\"{\n\x0eGetCallRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12\x11\n\tcall_name\x18\x02 \x01(\t\x12-\n\tcall_view\x18\x03 \x01(\x0e\x32\x15.ondewo.vtsi.CallViewH\x00\x88\x01\x01\x42\x0c\n\n_call_view\"\xe5\x05\n\x04\x43\x61ll\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bsip_account\x18\x02 \x01(\t\x12\x16\n\x0e\x63ontainer_name\x18\x03 \x01(\t\x12(\n\tcall_type\x18\x04 \x01(\x0e\x32\x15.ondewo.vtsi.CallType\x12\x14\n\x0cphone_number\x18\x05 \x01(\t\x12.\n\nstart_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x0fsip_status_type\x18\x08 \x01(\x0e\x32 .ondewo.sip.SipStatus.StatusType\x12.\n\nsip_status\x18\t \x01(\x0b\x32\x15.ondewo.sip.SipStatusH\x00\x88\x01\x01\x12\x45\n\x12sip_status_history\x18\n \x01(\x0b\x32$.ondewo.sip.SipStatusHistoryResponseH\x01\x88\x01\x01\x12@\n\x11services_statuses\x18\x0b \x01(\x0b\x32 .ondewo.vtsi.AllServicesStatusesH\x02\x88\x01\x01\x12\x0e\n\x06\x61\x63tive\x18\x0c \x01(\x08\x12\x19\n\x11vtsi_project_name\x18\r \x01(\t\x12\x46\n\x16\x63ommon_services_config\x18\x0e \x01(\x0b\x32!.ondewo.vtsi.CommonServicesConfigH\x03\x88\x01\x01\x12\x15\n\x08sip_port\x18\x0f \x01(\x05H\x04\x88\x01\x01\x12\x15\n\x08\x63si_port\x18\x10 \x01(\x05H\x05\x88\x01\x01\x42\r\n\x0b_sip_statusB\x15\n\x13_sip_status_historyB\x14\n\x12_services_statusesB\x19\n\x17_common_services_configB\x0b\n\t_sip_portB\x0b\n\t_csi_port\"\xc3\x02\n\x10ListCallsRequest\x12\x19\n\x11vtsi_project_name\x18\x01 \x01(\t\x12-\n\tcall_view\x18\x02 \x01(\x0e\x32\x15.ondewo.vtsi.CallViewH\x00\x88\x01\x01\x12-\n\tcall_type\x18\x03 \x01(\x0e\x32\x15.ondewo.vtsi.CallTypeH\x01\x88\x01\x01\x12\x17\n\npage_token\x18\x04 \x01(\tH\x02\x88\x01\x01\x12\x13\n\x06\x61\x63tive\x18\x05 \x01(\x08H\x03\x88\x01\x01\x12>\n\x0fsip_status_type\x18\x06 \x01(\x0e\x32 .ondewo.sip.SipStatus.StatusTypeH\x04\x88\x01\x01\x42\x0c\n\n_call_viewB\x0c\n\n_call_typeB\r\n\x0b_page_tokenB\t\n\x07_activeB\x12\n\x10_sip_status_type\"N\n\x11ListCallsResponse\x12 \n\x05\x63\x61lls\x18\x01 \x03(\x0b\x32\x11.ondewo.vtsi.Call\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x8a\x02\n\x13\x41llServicesStatuses\x12.\n\nstatus_sip\x18\x01 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12\x33\n\x0fstatus_asterisk\x18\x02 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_nlu\x18\x03 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_stt\x18\x04 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\x12.\n\nstatus_tts\x18\x05 \x01(\x0b\x32\x1a.ondewo.vtsi.ServiceStatus\"7\n\rServiceStatus\x12\x0f\n\x07healthy\x18\x01 \x01(\x08\x12\x15\n\rerror_message\x18\x02 \x01(\t\"o\n\x13GetAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x13\n\x0bobject_name\x18\x02 \x01(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"%\n\x14GetAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c\"\x80\x01\n#GetFullConversationAudioFileRequest\x12\x13\n\x0b\x62ucket_name\x18\x01 \x01(\t\x12\x14\n\x0cobject_names\x18\x02 \x03(\t\x12.\n\x0cminio_config\x18\x03 \x01(\x0b\x32\x18.ondewo.vtsi.MinioConfig\"5\n$GetFullConversationAudioFileResponse\x12\r\n\x05\x61udio\x18\x01 \x01(\x0c*.\n\x08\x43\x61llView\x12\x0b\n\x07MINIMUM\x10\x00\x12\x0b\n\x07SHALLOW\x10\x01\x12\x08\n\x04\x46ULL\x10\x02*.\n\x08\x43\x61llType\x12\x08\n\x04\x42OTH\x10\x00\x12\x0c\n\x08LISTENER\x10\x01\x12\n\n\x06\x43\x41LLER\x10\x02\x32\xe8\x0c\n\x05\x43\x61lls\x12P\n\x0bStartCaller\x12\x1f.ondewo.vtsi.StartCallerRequest\x1a .ondewo.vtsi.StartCallerResponse\x12S\n\x0cStartCallers\x12 .ondewo.vtsi.StartCallersRequest\x1a!.ondewo.vtsi.StartCallersResponse\x12P\n\x0bListCallers\x12\x1f.ondewo.vtsi.ListCallersRequest\x1a .ondewo.vtsi.ListCallersResponse\x12?\n\tGetCaller\x12\x1d.ondewo.vtsi.GetCallerRequest\x1a\x13.ondewo.vtsi.Caller\x12V\n\rStartListener\x12!.ondewo.vtsi.StartListenerRequest\x1a\".ondewo.vtsi.StartListenerResponse\x12Y\n\x0eStartListeners\x12\".ondewo.vtsi.StartListenersRequest\x1a#.ondewo.vtsi.StartListenersResponse\x12V\n\rListListeners\x12!.ondewo.vtsi.ListListenersRequest\x1a\".ondewo.vtsi.ListListenersResponse\x12\x45\n\x0bGetListener\x12\x1f.ondewo.vtsi.GetListenerRequest\x1a\x15.ondewo.vtsi.Listener\x12k\n\x14StartScheduledCaller\x12(.ondewo.vtsi.StartScheduledCallerRequest\x1a).ondewo.vtsi.StartScheduledCallerResponse\x12n\n\x15StartScheduledCallers\x12).ondewo.vtsi.StartScheduledCallersRequest\x1a*.ondewo.vtsi.StartScheduledCallersResponse\x12G\n\x08StopCall\x12\x1c.ondewo.vtsi.StopCallRequest\x1a\x1d.ondewo.vtsi.StopCallResponse\x12J\n\tStopCalls\x12\x1d.ondewo.vtsi.StopCallsRequest\x1a\x1e.ondewo.vtsi.StopCallsResponse\x12P\n\x0cStopAllCalls\x12 .ondewo.vtsi.StopAllCallsRequest\x1a\x1e.ondewo.vtsi.StopCallsResponse\x12S\n\x0cTransferCall\x12 .ondewo.vtsi.TransferCallRequest\x1a!.ondewo.vtsi.TransferCallResponse\x12V\n\rTransferCalls\x12!.ondewo.vtsi.TransferCallsRequest\x1a\".ondewo.vtsi.TransferCallsResponse\x12\x39\n\x07GetCall\x12\x1b.ondewo.vtsi.GetCallRequest\x1a\x11.ondewo.vtsi.Call\x12J\n\tListCalls\x12\x1d.ondewo.vtsi.ListCallsRequest\x1a\x1e.ondewo.vtsi.ListCallsResponse\x12S\n\x0cGetAudioFile\x12 .ondewo.vtsi.GetAudioFileRequest\x1a!.ondewo.vtsi.GetAudioFileResponse\x12\x85\x01\n\x1cGetFullConversationAudioFile\x12\x30.ondewo.vtsi.GetFullConversationAudioFileRequest\x1a\x31.ondewo.vtsi.GetFullConversationAudioFileResponse\"\x00\x62\x06proto3')
 
-_CALLINFOVIEW = DESCRIPTOR.enum_types_by_name['CallInfoView']
-CallInfoView = enum_type_wrapper.EnumTypeWrapper(_CALLINFOVIEW)
+_CALLVIEW = DESCRIPTOR.enum_types_by_name['CallView']
+CallView = enum_type_wrapper.EnumTypeWrapper(_CALLVIEW)
 _CALLTYPE = DESCRIPTOR.enum_types_by_name['CallType']
 CallType = enum_type_wrapper.EnumTypeWrapper(_CALLTYPE)
-SHALLOW = 0
-FULL = 1
-both = 0
-listener = 1
-caller = 2
+MINIMUM = 0
+SHALLOW = 1
+FULL = 2
+BOTH = 0
+LISTENER = 1
+CALLER = 2
 
 
 _BASESERVICECONFIG = DESCRIPTOR.message_types_by_name['BaseServiceConfig']
 _CREDENTIALS = DESCRIPTOR.message_types_by_name['Credentials']
 _NLUVTSICONFIG = DESCRIPTOR.message_types_by_name['NluVtsiConfig']
 _T2SVTSICONFIG = DESCRIPTOR.message_types_by_name['T2sVtsiConfig']
 _S2TVTSICONFIG = DESCRIPTOR.message_types_by_name['S2tVtsiConfig']
@@ -59,33 +61,38 @@
 _STARTLISTENERRESPONSE = DESCRIPTOR.message_types_by_name['StartListenerResponse']
 _STARTLISTENERSREQUEST = DESCRIPTOR.message_types_by_name['StartListenersRequest']
 _STARTLISTENERSRESPONSE = DESCRIPTOR.message_types_by_name['StartListenersResponse']
 _STARTCALLERREQUEST = DESCRIPTOR.message_types_by_name['StartCallerRequest']
 _STARTCALLERRESPONSE = DESCRIPTOR.message_types_by_name['StartCallerResponse']
 _STARTCALLERSREQUEST = DESCRIPTOR.message_types_by_name['StartCallersRequest']
 _STARTCALLERSRESPONSE = DESCRIPTOR.message_types_by_name['StartCallersResponse']
+_LISTCALLERSREQUEST = DESCRIPTOR.message_types_by_name['ListCallersRequest']
+_LISTCALLERSRESPONSE = DESCRIPTOR.message_types_by_name['ListCallersResponse']
+_GETCALLERREQUEST = DESCRIPTOR.message_types_by_name['GetCallerRequest']
+_LISTLISTENERSREQUEST = DESCRIPTOR.message_types_by_name['ListListenersRequest']
+_LISTLISTENERSRESPONSE = DESCRIPTOR.message_types_by_name['ListListenersResponse']
+_GETLISTENERREQUEST = DESCRIPTOR.message_types_by_name['GetListenerRequest']
 _STARTSCHEDULEDCALLERREQUEST = DESCRIPTOR.message_types_by_name['StartScheduledCallerRequest']
 _STARTSCHEDULEDCALLERSREQUEST = DESCRIPTOR.message_types_by_name['StartScheduledCallersRequest']
 _STARTSCHEDULEDCALLERSRESPONSE = DESCRIPTOR.message_types_by_name['StartScheduledCallersResponse']
 _STARTSCHEDULEDCALLERRESPONSE = DESCRIPTOR.message_types_by_name['StartScheduledCallerResponse']
 _SCHEDULEDCALLER = DESCRIPTOR.message_types_by_name['ScheduledCaller']
 _STOPCALLREQUEST = DESCRIPTOR.message_types_by_name['StopCallRequest']
 _STOPCALLRESPONSE = DESCRIPTOR.message_types_by_name['StopCallResponse']
 _STOPCALLSREQUEST = DESCRIPTOR.message_types_by_name['StopCallsRequest']
 _STOPCALLSRESPONSE = DESCRIPTOR.message_types_by_name['StopCallsResponse']
 _STOPALLCALLSREQUEST = DESCRIPTOR.message_types_by_name['StopAllCallsRequest']
 _TRANSFERCALLREQUEST = DESCRIPTOR.message_types_by_name['TransferCallRequest']
 _TRANSFERCALLRESPONSE = DESCRIPTOR.message_types_by_name['TransferCallResponse']
 _TRANSFERCALLSREQUEST = DESCRIPTOR.message_types_by_name['TransferCallsRequest']
 _TRANSFERCALLSRESPONSE = DESCRIPTOR.message_types_by_name['TransferCallsResponse']
-_GETCALLINFOREQUEST = DESCRIPTOR.message_types_by_name['GetCallInfoRequest']
-_GETCALLINFORESPONSE = DESCRIPTOR.message_types_by_name['GetCallInfoResponse']
-_CALLINFO = DESCRIPTOR.message_types_by_name['CallInfo']
-_LISTCALLINFOREQUEST = DESCRIPTOR.message_types_by_name['ListCallInfoRequest']
-_LISTCALLINFORESPONSE = DESCRIPTOR.message_types_by_name['ListCallInfoResponse']
+_GETCALLREQUEST = DESCRIPTOR.message_types_by_name['GetCallRequest']
+_CALL = DESCRIPTOR.message_types_by_name['Call']
+_LISTCALLSREQUEST = DESCRIPTOR.message_types_by_name['ListCallsRequest']
+_LISTCALLSRESPONSE = DESCRIPTOR.message_types_by_name['ListCallsResponse']
 _ALLSERVICESSTATUSES = DESCRIPTOR.message_types_by_name['AllServicesStatuses']
 _SERVICESTATUS = DESCRIPTOR.message_types_by_name['ServiceStatus']
 _GETAUDIOFILEREQUEST = DESCRIPTOR.message_types_by_name['GetAudioFileRequest']
 _GETAUDIOFILERESPONSE = DESCRIPTOR.message_types_by_name['GetAudioFileResponse']
 _GETFULLCONVERSATIONAUDIOFILEREQUEST = DESCRIPTOR.message_types_by_name['GetFullConversationAudioFileRequest']
 _GETFULLCONVERSATIONAUDIOFILERESPONSE = DESCRIPTOR.message_types_by_name['GetFullConversationAudioFileResponse']
 BaseServiceConfig = _reflection.GeneratedProtocolMessageType('BaseServiceConfig', (_message.Message,), {
@@ -294,14 +301,56 @@
 StartCallersResponse = _reflection.GeneratedProtocolMessageType('StartCallersResponse', (_message.Message,), {
     'DESCRIPTOR': _STARTCALLERSRESPONSE,
     '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartCallersResponse)
 })
 _sym_db.RegisterMessage(StartCallersResponse)
 
+ListCallersRequest = _reflection.GeneratedProtocolMessageType('ListCallersRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTCALLERSREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallersRequest)
+})
+_sym_db.RegisterMessage(ListCallersRequest)
+
+ListCallersResponse = _reflection.GeneratedProtocolMessageType('ListCallersResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTCALLERSRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallersResponse)
+})
+_sym_db.RegisterMessage(ListCallersResponse)
+
+GetCallerRequest = _reflection.GeneratedProtocolMessageType('GetCallerRequest', (_message.Message,), {
+    'DESCRIPTOR': _GETCALLERREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetCallerRequest)
+})
+_sym_db.RegisterMessage(GetCallerRequest)
+
+ListListenersRequest = _reflection.GeneratedProtocolMessageType('ListListenersRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTLISTENERSREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListListenersRequest)
+})
+_sym_db.RegisterMessage(ListListenersRequest)
+
+ListListenersResponse = _reflection.GeneratedProtocolMessageType('ListListenersResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTLISTENERSRESPONSE,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListListenersResponse)
+})
+_sym_db.RegisterMessage(ListListenersResponse)
+
+GetListenerRequest = _reflection.GeneratedProtocolMessageType('GetListenerRequest', (_message.Message,), {
+    'DESCRIPTOR': _GETLISTENERREQUEST,
+    '__module__': 'ondewo.vtsi.calls_pb2'
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetListenerRequest)
+})
+_sym_db.RegisterMessage(GetListenerRequest)
+
 StartScheduledCallerRequest = _reflection.GeneratedProtocolMessageType('StartScheduledCallerRequest', (_message.Message,), {
     'DESCRIPTOR': _STARTSCHEDULEDCALLERREQUEST,
     '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.StartScheduledCallerRequest)
 })
 _sym_db.RegisterMessage(StartScheduledCallerRequest)
 
@@ -392,48 +441,41 @@
 TransferCallsResponse = _reflection.GeneratedProtocolMessageType('TransferCallsResponse', (_message.Message,), {
     'DESCRIPTOR': _TRANSFERCALLSRESPONSE,
     '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.TransferCallsResponse)
 })
 _sym_db.RegisterMessage(TransferCallsResponse)
 
-GetCallInfoRequest = _reflection.GeneratedProtocolMessageType('GetCallInfoRequest', (_message.Message,), {
-    'DESCRIPTOR': _GETCALLINFOREQUEST,
-    '__module__': 'ondewo.vtsi.calls_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetCallInfoRequest)
-})
-_sym_db.RegisterMessage(GetCallInfoRequest)
-
-GetCallInfoResponse = _reflection.GeneratedProtocolMessageType('GetCallInfoResponse', (_message.Message,), {
-    'DESCRIPTOR': _GETCALLINFORESPONSE,
+GetCallRequest = _reflection.GeneratedProtocolMessageType('GetCallRequest', (_message.Message,), {
+    'DESCRIPTOR': _GETCALLREQUEST,
     '__module__': 'ondewo.vtsi.calls_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetCallInfoResponse)
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.GetCallRequest)
 })
-_sym_db.RegisterMessage(GetCallInfoResponse)
+_sym_db.RegisterMessage(GetCallRequest)
 
-CallInfo = _reflection.GeneratedProtocolMessageType('CallInfo', (_message.Message,), {
-    'DESCRIPTOR': _CALLINFO,
+Call = _reflection.GeneratedProtocolMessageType('Call', (_message.Message,), {
+    'DESCRIPTOR': _CALL,
     '__module__': 'ondewo.vtsi.calls_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.CallInfo)
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.Call)
 })
-_sym_db.RegisterMessage(CallInfo)
+_sym_db.RegisterMessage(Call)
 
-ListCallInfoRequest = _reflection.GeneratedProtocolMessageType('ListCallInfoRequest', (_message.Message,), {
-    'DESCRIPTOR': _LISTCALLINFOREQUEST,
+ListCallsRequest = _reflection.GeneratedProtocolMessageType('ListCallsRequest', (_message.Message,), {
+    'DESCRIPTOR': _LISTCALLSREQUEST,
     '__module__': 'ondewo.vtsi.calls_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallInfoRequest)
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallsRequest)
 })
-_sym_db.RegisterMessage(ListCallInfoRequest)
+_sym_db.RegisterMessage(ListCallsRequest)
 
-ListCallInfoResponse = _reflection.GeneratedProtocolMessageType('ListCallInfoResponse', (_message.Message,), {
-    'DESCRIPTOR': _LISTCALLINFORESPONSE,
+ListCallsResponse = _reflection.GeneratedProtocolMessageType('ListCallsResponse', (_message.Message,), {
+    'DESCRIPTOR': _LISTCALLSRESPONSE,
     '__module__': 'ondewo.vtsi.calls_pb2'
-    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallInfoResponse)
+    # @@protoc_insertion_point(class_scope:ondewo.vtsi.ListCallsResponse)
 })
-_sym_db.RegisterMessage(ListCallInfoResponse)
+_sym_db.RegisterMessage(ListCallsResponse)
 
 AllServicesStatuses = _reflection.GeneratedProtocolMessageType('AllServicesStatuses', (_message.Message,), {
     'DESCRIPTOR': _ALLSERVICESSTATUSES,
     '__module__': 'ondewo.vtsi.calls_pb2'
     # @@protoc_insertion_point(class_scope:ondewo.vtsi.AllServicesStatuses)
 })
 _sym_db.RegisterMessage(AllServicesStatuses)
@@ -475,124 +517,134 @@
 
 _CALLS = DESCRIPTOR.services_by_name['Calls']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
     _SIPCALLERCONFIG_SIPHEADERSENTRY._options = None
     _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_options = b'8\001'
-    _CALLINFOVIEW._serialized_start=7594
-    _CALLINFOVIEW._serialized_end=7631
-    _CALLTYPE._serialized_start=7633
-    _CALLTYPE._serialized_end=7679
-    _BASESERVICECONFIG._serialized_start=246
-    _BASESERVICECONFIG._serialized_end=312
-    _CREDENTIALS._serialized_start=314
-    _CREDENTIALS._serialized_end=367
-    _NLUVTSICONFIG._serialized_start=370
-    _NLUVTSICONFIG._serialized_end=668
-    _T2SVTSICONFIG._serialized_start=670
-    _T2SVTSICONFIG._serialized_end=797
-    _S2TVTSICONFIG._serialized_start=800
-    _S2TVTSICONFIG._serialized_end=948
-    _ASTERISKCONFIG._serialized_start=950
-    _ASTERISKCONFIG._serialized_end=1028
-    _COMMONSERVICESCONFIG._serialized_start=1031
-    _COMMONSERVICESCONFIG._serialized_end=1265
-    _SIPBASECONFIG._serialized_start=1267
-    _SIPBASECONFIG._serialized_end=1307
-    _SIPCALLERCONFIG._serialized_start=1310
-    _SIPCALLERCONFIG._serialized_end=1517
-    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_start=1468
-    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_end=1517
-    _CSIVTSICONFIG._serialized_start=1520
-    _CSIVTSICONFIG._serialized_end=1886
-    _AUDIOOBJECTSTORAGECONFIG._serialized_start=1889
-    _AUDIOOBJECTSTORAGECONFIG._serialized_end=2142
-    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_start=2144
-    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_end=2232
-    _MESSAGEBROKERCONFIG._serialized_start=2235
-    _MESSAGEBROKERCONFIG._serialized_end=2474
-    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_start=2476
-    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_end=2603
-    _RABBITMQCONFIG._serialized_start=2605
-    _RABBITMQCONFIG._serialized_end=2697
-    _MINIOCONFIG._serialized_start=2699
-    _MINIOCONFIG._serialized_end=2819
-    _S2TVTSICALLBACKS._serialized_start=2821
-    _S2TVTSICALLBACKS._serialized_end=2894
-    _NLUVTSICALLBACKS._serialized_start=2896
-    _NLUVTSICALLBACKS._serialized_end=2969
-    _T2SVTSICALLBACKS._serialized_start=2971
-    _T2SVTSICALLBACKS._serialized_end=3044
-    _LISTENER._serialized_start=3047
-    _LISTENER._serialized_end=3210
-    _CALLER._serialized_start=3213
-    _CALLER._serialized_end=3378
-    _STARTLISTENERREQUEST._serialized_start=3381
-    _STARTLISTENERREQUEST._serialized_end=3550
-    _STARTLISTENERRESPONSE._serialized_start=3552
-    _STARTLISTENERRESPONSE._serialized_end=3666
-    _STARTLISTENERSREQUEST._serialized_start=3668
-    _STARTLISTENERSREQUEST._serialized_end=3780
-    _STARTLISTENERSRESPONSE._serialized_start=3783
-    _STARTLISTENERSRESPONSE._serialized_end=3921
-    _STARTCALLERREQUEST._serialized_start=3924
-    _STARTCALLERREQUEST._serialized_end=4095
-    _STARTCALLERRESPONSE._serialized_start=4097
-    _STARTCALLERRESPONSE._serialized_end=4205
-    _STARTCALLERSREQUEST._serialized_start=4207
-    _STARTCALLERSREQUEST._serialized_end=4313
-    _STARTCALLERSRESPONSE._serialized_start=4316
-    _STARTCALLERSRESPONSE._serialized_end=4448
-    _STARTSCHEDULEDCALLERREQUEST._serialized_start=4451
-    _STARTSCHEDULEDCALLERREQUEST._serialized_end=4609
-    _STARTSCHEDULEDCALLERSREQUEST._serialized_start=4612
-    _STARTSCHEDULEDCALLERSREQUEST._serialized_end=4746
-    _STARTSCHEDULEDCALLERSRESPONSE._serialized_start=4749
-    _STARTSCHEDULEDCALLERSRESPONSE._serialized_end=4886
-    _STARTSCHEDULEDCALLERRESPONSE._serialized_start=4889
-    _STARTSCHEDULEDCALLERRESPONSE._serialized_end=5025
-    _SCHEDULEDCALLER._serialized_start=5028
-    _SCHEDULEDCALLER._serialized_end=5245
-    _STOPCALLREQUEST._serialized_start=5247
-    _STOPCALLREQUEST._serialized_end=5310
-    _STOPCALLRESPONSE._serialized_start=5312
-    _STOPCALLRESPONSE._serialized_end=5399
-    _STOPCALLSREQUEST._serialized_start=5401
-    _STOPCALLSREQUEST._serialized_end=5466
-    _STOPCALLSRESPONSE._serialized_start=5468
-    _STOPCALLSRESPONSE._serialized_end=5570
-    _STOPALLCALLSREQUEST._serialized_start=5572
-    _STOPALLCALLSREQUEST._serialized_end=5620
-    _TRANSFERCALLREQUEST._serialized_start=5622
-    _TRANSFERCALLREQUEST._serialized_end=5710
-    _TRANSFERCALLRESPONSE._serialized_start=5712
-    _TRANSFERCALLRESPONSE._serialized_end=5824
-    _TRANSFERCALLSREQUEST._serialized_start=5826
-    _TRANSFERCALLSREQUEST._serialized_end=5941
-    _TRANSFERCALLSRESPONSE._serialized_start=5944
-    _TRANSFERCALLSRESPONSE._serialized_end=6085
-    _GETCALLINFOREQUEST._serialized_start=6087
-    _GETCALLINFOREQUEST._serialized_end=6204
-    _GETCALLINFORESPONSE._serialized_start=6206
-    _GETCALLINFORESPONSE._serialized_end=6312
-    _CALLINFO._serialized_start=6315
-    _CALLINFO._serialized_end=6717
-    _LISTCALLINFOREQUEST._serialized_start=6720
-    _LISTCALLINFOREQUEST._serialized_end=6861
-    _LISTCALLINFORESPONSE._serialized_start=6863
-    _LISTCALLINFORESPONSE._serialized_end=6928
-    _ALLSERVICESSTATUSES._serialized_start=6931
-    _ALLSERVICESSTATUSES._serialized_end=7197
-    _SERVICESTATUS._serialized_start=7199
-    _SERVICESTATUS._serialized_end=7254
-    _GETAUDIOFILEREQUEST._serialized_start=7256
-    _GETAUDIOFILEREQUEST._serialized_end=7367
-    _GETAUDIOFILERESPONSE._serialized_start=7369
-    _GETAUDIOFILERESPONSE._serialized_end=7406
-    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_start=7409
-    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_end=7537
-    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_start=7539
-    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_end=7592
-    _CALLS._serialized_start=7682
-    _CALLS._serialized_end=9048
+    _CALLVIEW._serialized_start=8513
+    _CALLVIEW._serialized_end=8559
+    _CALLTYPE._serialized_start=8561
+    _CALLTYPE._serialized_end=8607
+    _BASESERVICECONFIG._serialized_start=276
+    _BASESERVICECONFIG._serialized_end=342
+    _CREDENTIALS._serialized_start=344
+    _CREDENTIALS._serialized_end=397
+    _NLUVTSICONFIG._serialized_start=400
+    _NLUVTSICONFIG._serialized_end=698
+    _T2SVTSICONFIG._serialized_start=700
+    _T2SVTSICONFIG._serialized_end=827
+    _S2TVTSICONFIG._serialized_start=830
+    _S2TVTSICONFIG._serialized_end=978
+    _ASTERISKCONFIG._serialized_start=980
+    _ASTERISKCONFIG._serialized_end=1058
+    _COMMONSERVICESCONFIG._serialized_start=1061
+    _COMMONSERVICESCONFIG._serialized_end=1295
+    _SIPBASECONFIG._serialized_start=1297
+    _SIPBASECONFIG._serialized_end=1337
+    _SIPCALLERCONFIG._serialized_start=1340
+    _SIPCALLERCONFIG._serialized_end=1547
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_start=1498
+    _SIPCALLERCONFIG_SIPHEADERSENTRY._serialized_end=1547
+    _CSIVTSICONFIG._serialized_start=1550
+    _CSIVTSICONFIG._serialized_end=1916
+    _AUDIOOBJECTSTORAGECONFIG._serialized_start=1919
+    _AUDIOOBJECTSTORAGECONFIG._serialized_end=2172
+    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_start=2174
+    _AUDIOOBJECTSTORAGESERVICESACTIVATIONCONFIG._serialized_end=2262
+    _MESSAGEBROKERCONFIG._serialized_start=2265
+    _MESSAGEBROKERCONFIG._serialized_end=2504
+    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_start=2506
+    _MESSAGEBROKERSERVICESACTIVATIONCONFIG._serialized_end=2633
+    _RABBITMQCONFIG._serialized_start=2635
+    _RABBITMQCONFIG._serialized_end=2727
+    _MINIOCONFIG._serialized_start=2729
+    _MINIOCONFIG._serialized_end=2849
+    _S2TVTSICALLBACKS._serialized_start=2851
+    _S2TVTSICALLBACKS._serialized_end=2924
+    _NLUVTSICALLBACKS._serialized_start=2926
+    _NLUVTSICALLBACKS._serialized_end=2999
+    _T2SVTSICALLBACKS._serialized_start=3001
+    _T2SVTSICALLBACKS._serialized_end=3074
+    _LISTENER._serialized_start=3077
+    _LISTENER._serialized_end=3240
+    _CALLER._serialized_start=3243
+    _CALLER._serialized_end=3408
+    _STARTLISTENERREQUEST._serialized_start=3411
+    _STARTLISTENERREQUEST._serialized_end=3580
+    _STARTLISTENERRESPONSE._serialized_start=3582
+    _STARTLISTENERRESPONSE._serialized_end=3696
+    _STARTLISTENERSREQUEST._serialized_start=3698
+    _STARTLISTENERSREQUEST._serialized_end=3810
+    _STARTLISTENERSRESPONSE._serialized_start=3813
+    _STARTLISTENERSRESPONSE._serialized_end=3951
+    _STARTCALLERREQUEST._serialized_start=3954
+    _STARTCALLERREQUEST._serialized_end=4125
+    _STARTCALLERRESPONSE._serialized_start=4127
+    _STARTCALLERRESPONSE._serialized_end=4235
+    _STARTCALLERSREQUEST._serialized_start=4237
+    _STARTCALLERSREQUEST._serialized_end=4343
+    _STARTCALLERSRESPONSE._serialized_start=4346
+    _STARTCALLERSRESPONSE._serialized_end=4478
+    _LISTCALLERSREQUEST._serialized_start=4480
+    _LISTCALLERSREQUEST._serialized_end=4567
+    _LISTCALLERSRESPONSE._serialized_start=4569
+    _LISTCALLERSRESPONSE._serialized_end=4628
+    _GETCALLERREQUEST._serialized_start=4630
+    _GETCALLERREQUEST._serialized_end=4689
+    _LISTLISTENERSREQUEST._serialized_start=4691
+    _LISTLISTENERSREQUEST._serialized_end=4780
+    _LISTLISTENERSRESPONSE._serialized_start=4782
+    _LISTLISTENERSRESPONSE._serialized_end=4872
+    _GETLISTENERREQUEST._serialized_start=4874
+    _GETLISTENERREQUEST._serialized_end=4935
+    _STARTSCHEDULEDCALLERREQUEST._serialized_start=4938
+    _STARTSCHEDULEDCALLERREQUEST._serialized_end=5096
+    _STARTSCHEDULEDCALLERSREQUEST._serialized_start=5099
+    _STARTSCHEDULEDCALLERSREQUEST._serialized_end=5233
+    _STARTSCHEDULEDCALLERSRESPONSE._serialized_start=5236
+    _STARTSCHEDULEDCALLERSRESPONSE._serialized_end=5373
+    _STARTSCHEDULEDCALLERRESPONSE._serialized_start=5376
+    _STARTSCHEDULEDCALLERRESPONSE._serialized_end=5512
+    _SCHEDULEDCALLER._serialized_start=5515
+    _SCHEDULEDCALLER._serialized_end=5732
+    _STOPCALLREQUEST._serialized_start=5734
+    _STOPCALLREQUEST._serialized_end=5797
+    _STOPCALLRESPONSE._serialized_start=5799
+    _STOPCALLRESPONSE._serialized_end=5886
+    _STOPCALLSREQUEST._serialized_start=5888
+    _STOPCALLSREQUEST._serialized_end=5953
+    _STOPCALLSRESPONSE._serialized_start=5955
+    _STOPCALLSRESPONSE._serialized_end=6057
+    _STOPALLCALLSREQUEST._serialized_start=6059
+    _STOPALLCALLSREQUEST._serialized_end=6107
+    _TRANSFERCALLREQUEST._serialized_start=6109
+    _TRANSFERCALLREQUEST._serialized_end=6197
+    _TRANSFERCALLRESPONSE._serialized_start=6199
+    _TRANSFERCALLRESPONSE._serialized_end=6311
+    _TRANSFERCALLSREQUEST._serialized_start=6313
+    _TRANSFERCALLSREQUEST._serialized_end=6428
+    _TRANSFERCALLSRESPONSE._serialized_start=6431
+    _TRANSFERCALLSRESPONSE._serialized_end=6572
+    _GETCALLREQUEST._serialized_start=6574
+    _GETCALLREQUEST._serialized_end=6697
+    _CALL._serialized_start=6700
+    _CALL._serialized_end=7441
+    _LISTCALLSREQUEST._serialized_start=7444
+    _LISTCALLSREQUEST._serialized_end=7767
+    _LISTCALLSRESPONSE._serialized_start=7769
+    _LISTCALLSRESPONSE._serialized_end=7847
+    _ALLSERVICESSTATUSES._serialized_start=7850
+    _ALLSERVICESSTATUSES._serialized_end=8116
+    _SERVICESTATUS._serialized_start=8118
+    _SERVICESTATUS._serialized_end=8173
+    _GETAUDIOFILEREQUEST._serialized_start=8175
+    _GETAUDIOFILEREQUEST._serialized_end=8286
+    _GETAUDIOFILERESPONSE._serialized_start=8288
+    _GETAUDIOFILERESPONSE._serialized_end=8325
+    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_start=8328
+    _GETFULLCONVERSATIONAUDIOFILEREQUEST._serialized_end=8456
+    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_start=8458
+    _GETFULLCONVERSATIONAUDIOFILERESPONSE._serialized_end=8511
+    _CALLS._serialized_start=8610
+    _CALLS._serialized_end=10250
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/vtsi/calls_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/vtsi/calls_pb2_grpc.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,24 +21,44 @@
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallerResponse.FromString,
         )
         self.StartCallers = channel.unary_unary(
             '/ondewo.vtsi.Calls/StartCallers',
             request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersResponse.FromString,
         )
+        self.ListCallers = channel.unary_unary(
+            '/ondewo.vtsi.Calls/ListCallers',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallersResponse.FromString,
+        )
+        self.GetCaller = channel.unary_unary(
+            '/ondewo.vtsi.Calls/GetCaller',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallerRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.Caller.FromString,
+        )
         self.StartListener = channel.unary_unary(
             '/ondewo.vtsi.Calls/StartListener',
             request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerResponse.FromString,
         )
         self.StartListeners = channel.unary_unary(
             '/ondewo.vtsi.Calls/StartListeners',
             request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersResponse.FromString,
         )
+        self.ListListeners = channel.unary_unary(
+            '/ondewo.vtsi.Calls/ListListeners',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListListenersRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListListenersResponse.FromString,
+        )
+        self.GetListener = channel.unary_unary(
+            '/ondewo.vtsi.Calls/GetListener',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetListenerRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.Listener.FromString,
+        )
         self.StartScheduledCaller = channel.unary_unary(
             '/ondewo.vtsi.Calls/StartScheduledCaller',
             request_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerResponse.FromString,
         )
         self.StartScheduledCallers = channel.unary_unary(
             '/ondewo.vtsi.Calls/StartScheduledCallers',
@@ -66,23 +86,23 @@
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallResponse.FromString,
         )
         self.TransferCalls = channel.unary_unary(
             '/ondewo.vtsi.Calls/TransferCalls',
             request_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsResponse.FromString,
         )
-        self.GetCallInfo = channel.unary_unary(
-            '/ondewo.vtsi.Calls/GetCallInfo',
-            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoResponse.FromString,
-        )
-        self.ListCallInfo = channel.unary_unary(
-            '/ondewo.vtsi.Calls/ListCallInfo',
-            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoRequest.SerializeToString,
-            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoResponse.FromString,
+        self.GetCall = channel.unary_unary(
+            '/ondewo.vtsi.Calls/GetCall',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.Call.FromString,
+        )
+        self.ListCalls = channel.unary_unary(
+            '/ondewo.vtsi.Calls/ListCalls',
+            request_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallsRequest.SerializeToString,
+            response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallsResponse.FromString,
         )
         self.GetAudioFile = channel.unary_unary(
             '/ondewo.vtsi.Calls/GetAudioFile',
             request_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileRequest.SerializeToString,
             response_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileResponse.FromString,
         )
         self.GetFullConversationAudioFile = channel.unary_unary(
@@ -110,28 +130,56 @@
     def StartCallers(self, request, context):
         """start multiple ondewo-sip callers instances for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListCallers(self, request, context):
+        """lists all available callers
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetCaller(self, request, context):
+        """gets a caller
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def StartListener(self, request, context):
         """start single listener instance for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def StartListeners(self, request, context):
         """start multiple ondewo-sip listeners instances for a specific nlu-project.
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
+    def ListListeners(self, request, context):
+        """lists all available listeners
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
+    def GetListener(self, request, context):
+        """gets a listener
+        """
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details('Method not implemented!')
+        raise NotImplementedError('Method not implemented!')
+
     def StartScheduledCaller(self, request, context):
         """start multiple ondewo-sip callers instances with schedules
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
@@ -175,22 +223,22 @@
     def TransferCalls(self, request, context):
         """Transfer a call from a listener to another
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def GetCallInfo(self, request, context):
+    def GetCall(self, request, context):
         """get call log for single call instance
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
-    def ListCallInfo(self, request, context):
+    def ListCalls(self, request, context):
         """get call log for all call instances
         """
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
     def GetAudioFile(self, request, context):
@@ -216,24 +264,44 @@
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallerResponse.SerializeToString,
         ),
         'StartCallers': grpc.unary_unary_rpc_method_handler(
             servicer.StartCallers,
             request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartCallersResponse.SerializeToString,
         ),
+        'ListCallers': grpc.unary_unary_rpc_method_handler(
+            servicer.ListCallers,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallersRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallersResponse.SerializeToString,
+        ),
+        'GetCaller': grpc.unary_unary_rpc_method_handler(
+            servicer.GetCaller,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallerRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.Caller.SerializeToString,
+        ),
         'StartListener': grpc.unary_unary_rpc_method_handler(
             servicer.StartListener,
             request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenerResponse.SerializeToString,
         ),
         'StartListeners': grpc.unary_unary_rpc_method_handler(
             servicer.StartListeners,
             request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartListenersResponse.SerializeToString,
         ),
+        'ListListeners': grpc.unary_unary_rpc_method_handler(
+            servicer.ListListeners,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListListenersRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListListenersResponse.SerializeToString,
+        ),
+        'GetListener': grpc.unary_unary_rpc_method_handler(
+            servicer.GetListener,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetListenerRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.Listener.SerializeToString,
+        ),
         'StartScheduledCaller': grpc.unary_unary_rpc_method_handler(
             servicer.StartScheduledCaller,
             request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.StartScheduledCallerResponse.SerializeToString,
         ),
         'StartScheduledCallers': grpc.unary_unary_rpc_method_handler(
             servicer.StartScheduledCallers,
@@ -261,23 +329,23 @@
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallResponse.SerializeToString,
         ),
         'TransferCalls': grpc.unary_unary_rpc_method_handler(
             servicer.TransferCalls,
             request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.TransferCallsResponse.SerializeToString,
         ),
-        'GetCallInfo': grpc.unary_unary_rpc_method_handler(
-            servicer.GetCallInfo,
-            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoResponse.SerializeToString,
-        ),
-        'ListCallInfo': grpc.unary_unary_rpc_method_handler(
-            servicer.ListCallInfo,
-            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoRequest.FromString,
-            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoResponse.SerializeToString,
+        'GetCall': grpc.unary_unary_rpc_method_handler(
+            servicer.GetCall,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetCallRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.Call.SerializeToString,
+        ),
+        'ListCalls': grpc.unary_unary_rpc_method_handler(
+            servicer.ListCalls,
+            request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallsRequest.FromString,
+            response_serializer=ondewo_dot_vtsi_dot_calls__pb2.ListCallsResponse.SerializeToString,
         ),
         'GetAudioFile': grpc.unary_unary_rpc_method_handler(
             servicer.GetAudioFile,
             request_deserializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileRequest.FromString,
             response_serializer=ondewo_dot_vtsi_dot_calls__pb2.GetAudioFileResponse.SerializeToString,
         ),
         'GetFullConversationAudioFile': grpc.unary_unary_rpc_method_handler(
@@ -328,14 +396,48 @@
         return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartCallers',
                                              ondewo_dot_vtsi_dot_calls__pb2.StartCallersRequest.SerializeToString,
                                              ondewo_dot_vtsi_dot_calls__pb2.StartCallersResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListCallers(request,
+                    target,
+                    options=(),
+                    channel_credentials=None,
+                    call_credentials=None,
+                    insecure=False,
+                    compression=None,
+                    wait_for_ready=None,
+                    timeout=None,
+                    metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/ListCallers',
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallersRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallersResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetCaller(request,
+                  target,
+                  options=(),
+                  channel_credentials=None,
+                  call_credentials=None,
+                  insecure=False,
+                  compression=None,
+                  wait_for_ready=None,
+                  timeout=None,
+                  metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetCaller',
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetCallerRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.Caller.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def StartListener(request,
                       target,
                       options=(),
                       channel_credentials=None,
                       call_credentials=None,
                       insecure=False,
                       compression=None,
@@ -362,14 +464,48 @@
         return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/StartListeners',
                                              ondewo_dot_vtsi_dot_calls__pb2.StartListenersRequest.SerializeToString,
                                              ondewo_dot_vtsi_dot_calls__pb2.StartListenersResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
+    def ListListeners(request,
+                      target,
+                      options=(),
+                      channel_credentials=None,
+                      call_credentials=None,
+                      insecure=False,
+                      compression=None,
+                      wait_for_ready=None,
+                      timeout=None,
+                      metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/ListListeners',
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListListenersRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListListenersResponse.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
+    def GetListener(request,
+                    target,
+                    options=(),
+                    channel_credentials=None,
+                    call_credentials=None,
+                    insecure=False,
+                    compression=None,
+                    wait_for_ready=None,
+                    timeout=None,
+                    metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetListener',
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetListenerRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.Listener.FromString,
+                                             options, channel_credentials,
+                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+
+    @staticmethod
     def StartScheduledCaller(request,
                              target,
                              options=(),
                              channel_credentials=None,
                              call_credentials=None,
                              insecure=False,
                              compression=None,
@@ -481,44 +617,44 @@
         return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/TransferCalls',
                                              ondewo_dot_vtsi_dot_calls__pb2.TransferCallsRequest.SerializeToString,
                                              ondewo_dot_vtsi_dot_calls__pb2.TransferCallsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def GetCallInfo(request,
-                    target,
-                    options=(),
-                    channel_credentials=None,
-                    call_credentials=None,
-                    insecure=False,
-                    compression=None,
-                    wait_for_ready=None,
-                    timeout=None,
-                    metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetCallInfo',
-                                             ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_calls__pb2.GetCallInfoResponse.FromString,
+    def GetCall(request,
+                target,
+                options=(),
+                channel_credentials=None,
+                call_credentials=None,
+                insecure=False,
+                compression=None,
+                wait_for_ready=None,
+                timeout=None,
+                metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/GetCall',
+                                             ondewo_dot_vtsi_dot_calls__pb2.GetCallRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.Call.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
-    def ListCallInfo(request,
-                     target,
-                     options=(),
-                     channel_credentials=None,
-                     call_credentials=None,
-                     insecure=False,
-                     compression=None,
-                     wait_for_ready=None,
-                     timeout=None,
-                     metadata=None):
-        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/ListCallInfo',
-                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoRequest.SerializeToString,
-                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallInfoResponse.FromString,
+    def ListCalls(request,
+                  target,
+                  options=(),
+                  channel_credentials=None,
+                  call_credentials=None,
+                  insecure=False,
+                  compression=None,
+                  wait_for_ready=None,
+                  timeout=None,
+                  metadata=None):
+        return grpc.experimental.unary_unary(request, target, '/ondewo.vtsi.Calls/ListCalls',
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallsRequest.SerializeToString,
+                                             ondewo_dot_vtsi_dot_calls__pb2.ListCallsResponse.FromString,
                                              options, channel_credentials,
                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def GetAudioFile(request,
                      target,
                      options=(),
```

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/vtsi/client/client.py` & `ondewo-vtsi-client-6.4.0/ondewo/vtsi/client/client.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/vtsi/projects_pb2.py` & `ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from google.protobuf import reflection as _reflection
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aondewo/vtsi/projects.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa5\x03\n\x0bVtsiProject\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x13\n\x0bmax_callers\x18\x03 \x01(\x05\x12\x15\n\rmax_listeners\x18\x04 \x01(\x05\x12\x36\n\x10\x61sterisk_configs\x18\x05 \x01(\x0b\x32\x1c.ondewo.vtsi.AsteriskConfigs\x12;\n\x13vtsi_project_status\x18\x06 \x01(\x0e\x32\x1e.ondewo.vtsi.VtsiProjectStatus\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bmodified_by\x18\t \x01(\t\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x61\x63tive_callers\x18\x0b \x01(\x05\x12\x18\n\x10\x61\x63tive_listeners\x18\x0c \x01(\x05\x12\x15\n\rasterisk_port\x18\r \x01(\x05\"\xc1\x01\n\x18\x41steriskConfigsVariables\x12\x1a\n\x12sip_trunk_username\x18\x01 \x01(\t\x12\x1a\n\x12sip_trunk_password\x18\x02 \x01(\t\x12\x16\n\x0esip_trunk_host\x18\x03 \x01(\t\x12\x17\n\x0ftransfer_number\x18\x04 \x01(\t\x12\x1c\n\x14transfer_number_host\x18\x05 \x01(\t\x12\x1e\n\x16sip_trunk_phone_number\x18\x06 \x01(\t\"\x9c\x01\n\x14\x41steriskConfigsFiles\x12\x1c\n\x14sip_conf_file_string\x18\x01 \x01(\t\x12#\n\x1b\x65xtensions_conf_file_string\x18\x02 \x01(\t\x12\x1f\n\x17queues_conf_file_string\x18\x03 \x01(\t\x12 \n\x18modules_conf_file_string\x18\x04 \x01(\t\"\x86\x02\n\x0f\x41steriskConfigs\x12K\n\x1a\x61sterisk_configs_variables\x18\x01 \x01(\x0b\x32%.ondewo.vtsi.AsteriskConfigsVariablesH\x00\x12\x43\n\x16\x61sterisk_configs_files\x18\x02 \x01(\x0b\x32!.ondewo.vtsi.AsteriskConfigsFilesH\x00\x12\x30\n&asterisk_configs_target_directory_name\x18\x03 \x01(\tH\x00\x12\x15\n\rasterisk_port\x18\x04 \x01(\x05\x42\x18\n\x16\x61sterisk_configs_oneof\"a\n\x18\x43reateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"b\n\x19\x43reateVtsiProjectResponse\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"%\n\x15GetVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xa5\x01\n\x17ListVtsiProjectsRequest\x12\x37\n\x11vtsi_project_view\x18\x01 \x01(\x0e\x32\x1c.ondewo.vtsi.VtsiProjectView\x12\x12\n\npage_token\x18\x02 \x01(\t\x12=\n\x14vtsi_project_sorting\x18\x03 \x01(\x0b\x32\x1f.ondewo.vtsi.VtsiProjectSorting\"d\n\x18ListVtsiProjectsResponse\x12/\n\rvtsi_projects\x18\x01 \x03(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\xee\x02\n\x12VtsiProjectSorting\x12N\n\rsorting_field\x18\x01 \x01(\x0e\x32\x37.ondewo.vtsi.VtsiProjectSorting.VtsiProjectSortingField\x12\x39\n\x0csorting_mode\x18\x02 \x01(\x0e\x32#.ondewo.vtsi.VtsiProjectSortingMode\"\xcc\x01\n\x17VtsiProjectSortingField\x12\x1b\n\x17NO_VTSI_PROJECT_SORTING\x10\x00\x12\x1d\n\x19SORT_VTSI_PROJECT_BY_NAME\x10\x01\x12%\n!SORT_VTSI_PROJECT_BY_DISPLAY_NAME\x10\x02\x12&\n\"SORT_VTSI_PROJECT_BY_CREATION_DATE\x10\x03\x12&\n\"SORT_VTSI_PROJECT_BY_LAST_MODIFIED\x10\x04\"J\n\x18UpdateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\"@\n\x19UpdateVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65leteVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65leteVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65ployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65ployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"*\n\x1aUndeployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"B\n\x1bUndeployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t*\x8b\x01\n\x11VtsiProjectStatus\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nUNDEPLOYED\x10\x01\x12\x0c\n\x08UPDATING\x10\x02\x12\r\n\tDEPLOYING\x10\x03\x12\x0c\n\x08\x44\x45PLOYED\x10\x04\x12\x0f\n\x0bUNDEPLOYING\x10\x05\x12\x0c\n\x08\x44\x45LETING\x10\x06\x12\x0b\n\x07\x44\x45LETED\x10\x07*7\n\x16VtsiProjectSortingMode\x12\r\n\tASCENDING\x10\x00\x12\x0e\n\nDESCENDING\x10\x01*\x8e\x01\n\x0fVtsiProjectView\x12!\n\x1dVTSI_PROJECT_VIEW_UNSPECIFIED\x10\x00\x12\x1a\n\x16VTSI_PROJECT_VIEW_FULL\x10\x01\x12\x1d\n\x19VTSI_PROJECT_VIEW_SHALLOW\x10\x02\x12\x1d\n\x19VTSI_PROJECT_VIEW_MINIMUM\x10\x03\x32\xb5\x05\n\x08Projects\x12\x62\n\x11\x43reateVtsiProject\x12%.ondewo.vtsi.CreateVtsiProjectRequest\x1a&.ondewo.vtsi.CreateVtsiProjectResponse\x12N\n\x0eGetVtsiProject\x12\".ondewo.vtsi.GetVtsiProjectRequest\x1a\x18.ondewo.vtsi.VtsiProject\x12\x62\n\x11UpdateVtsiProject\x12%.ondewo.vtsi.UpdateVtsiProjectRequest\x1a&.ondewo.vtsi.UpdateVtsiProjectResponse\x12\x62\n\x11\x44\x65leteVtsiProject\x12%.ondewo.vtsi.DeleteVtsiProjectRequest\x1a&.ondewo.vtsi.DeleteVtsiProjectResponse\x12\x62\n\x11\x44\x65ployVtsiProject\x12%.ondewo.vtsi.DeployVtsiProjectRequest\x1a&.ondewo.vtsi.DeployVtsiProjectResponse\x12h\n\x13UndeployVtsiProject\x12\'.ondewo.vtsi.UndeployVtsiProjectRequest\x1a(.ondewo.vtsi.UndeployVtsiProjectResponse\x12_\n\x10ListVtsiProjects\x12$.ondewo.vtsi.ListVtsiProjectsRequest\x1a%.ondewo.vtsi.ListVtsiProjectsResponseb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1aondewo/vtsi/projects.proto\x12\x0bondewo.vtsi\x1a\x1cgoogle/protobuf/struct.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"\xa5\x03\n\x0bVtsiProject\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x14\n\x0c\x64isplay_name\x18\x02 \x01(\t\x12\x13\n\x0bmax_callers\x18\x03 \x01(\x05\x12\x15\n\rmax_listeners\x18\x04 \x01(\x05\x12\x36\n\x10\x61sterisk_configs\x18\x05 \x01(\x0b\x32\x1c.ondewo.vtsi.AsteriskConfigs\x12;\n\x13vtsi_project_status\x18\x06 \x01(\x0e\x32\x1e.ondewo.vtsi.VtsiProjectStatus\x12\x12\n\ncreated_by\x18\x07 \x01(\t\x12.\n\ncreated_at\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x13\n\x0bmodified_by\x18\t \x01(\t\x12/\n\x0bmodified_at\x18\n \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x16\n\x0e\x61\x63tive_callers\x18\x0b \x01(\x05\x12\x18\n\x10\x61\x63tive_listeners\x18\x0c \x01(\x05\x12\x15\n\rasterisk_port\x18\r \x01(\x05\"\xc1\x01\n\x18\x41steriskConfigsVariables\x12\x1a\n\x12sip_trunk_username\x18\x01 \x01(\t\x12\x1a\n\x12sip_trunk_password\x18\x02 \x01(\t\x12\x16\n\x0esip_trunk_host\x18\x03 \x01(\t\x12\x17\n\x0ftransfer_number\x18\x04 \x01(\t\x12\x1c\n\x14transfer_number_host\x18\x05 \x01(\t\x12\x1e\n\x16sip_trunk_phone_number\x18\x06 \x01(\t\"\x9c\x01\n\x14\x41steriskConfigsFiles\x12\x1c\n\x14sip_conf_file_string\x18\x01 \x01(\t\x12#\n\x1b\x65xtensions_conf_file_string\x18\x02 \x01(\t\x12\x1f\n\x17queues_conf_file_string\x18\x03 \x01(\t\x12 \n\x18modules_conf_file_string\x18\x04 \x01(\t\"\x86\x02\n\x0f\x41steriskConfigs\x12K\n\x1a\x61sterisk_configs_variables\x18\x01 \x01(\x0b\x32%.ondewo.vtsi.AsteriskConfigsVariablesH\x00\x12\x43\n\x16\x61sterisk_configs_files\x18\x02 \x01(\x0b\x32!.ondewo.vtsi.AsteriskConfigsFilesH\x00\x12\x30\n&asterisk_configs_target_directory_name\x18\x03 \x01(\tH\x00\x12\x15\n\rasterisk_port\x18\x04 \x01(\x05\x42\x18\n\x16\x61sterisk_configs_oneof\"a\n\x18\x43reateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"b\n\x19\x43reateVtsiProjectResponse\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x15\n\rerror_message\x18\x02 \x01(\t\"%\n\x15GetVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"\xd7\x01\n\x17ListVtsiProjectsRequest\x12\x37\n\x11vtsi_project_view\x18\x01 \x01(\x0e\x32\x1c.ondewo.vtsi.VtsiProjectView\x12\x17\n\npage_token\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x42\n\x14vtsi_project_sorting\x18\x03 \x01(\x0b\x32\x1f.ondewo.vtsi.VtsiProjectSortingH\x01\x88\x01\x01\x42\r\n\x0b_page_tokenB\x17\n\x15_vtsi_project_sorting\"d\n\x18ListVtsiProjectsResponse\x12/\n\rvtsi_projects\x18\x01 \x03(\x0b\x32\x18.ondewo.vtsi.VtsiProject\x12\x17\n\x0fnext_page_token\x18\x02 \x01(\t\"\x9b\x03\n\x12VtsiProjectSorting\x12S\n\rsorting_field\x18\x01 \x01(\x0e\x32\x37.ondewo.vtsi.VtsiProjectSorting.VtsiProjectSortingFieldH\x00\x88\x01\x01\x12>\n\x0csorting_mode\x18\x02 \x01(\x0e\x32#.ondewo.vtsi.VtsiProjectSortingModeH\x01\x88\x01\x01\"\xcc\x01\n\x17VtsiProjectSortingField\x12\x1b\n\x17NO_VTSI_PROJECT_SORTING\x10\x00\x12\x1d\n\x19SORT_VTSI_PROJECT_BY_NAME\x10\x01\x12%\n!SORT_VTSI_PROJECT_BY_DISPLAY_NAME\x10\x02\x12&\n\"SORT_VTSI_PROJECT_BY_CREATION_DATE\x10\x03\x12&\n\"SORT_VTSI_PROJECT_BY_LAST_MODIFIED\x10\x04\x42\x10\n\x0e_sorting_fieldB\x0f\n\r_sorting_mode\"J\n\x18UpdateVtsiProjectRequest\x12.\n\x0cvtsi_project\x18\x01 \x01(\x0b\x32\x18.ondewo.vtsi.VtsiProject\"@\n\x19UpdateVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65leteVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65leteVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"(\n\x18\x44\x65ployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"@\n\x19\x44\x65ployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t\"*\n\x1aUndeployVtsiProjectRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"B\n\x1bUndeployVtsiProjectResponse\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x15\n\rerror_message\x18\x02 \x01(\t*\x8b\x01\n\x11VtsiProjectStatus\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x0e\n\nUNDEPLOYED\x10\x01\x12\x0c\n\x08UPDATING\x10\x02\x12\r\n\tDEPLOYING\x10\x03\x12\x0c\n\x08\x44\x45PLOYED\x10\x04\x12\x0f\n\x0bUNDEPLOYING\x10\x05\x12\x0c\n\x08\x44\x45LETING\x10\x06\x12\x0b\n\x07\x44\x45LETED\x10\x07*7\n\x16VtsiProjectSortingMode\x12\r\n\tASCENDING\x10\x00\x12\x0e\n\nDESCENDING\x10\x01*\x8e\x01\n\x0fVtsiProjectView\x12!\n\x1dVTSI_PROJECT_VIEW_UNSPECIFIED\x10\x00\x12\x1a\n\x16VTSI_PROJECT_VIEW_FULL\x10\x01\x12\x1d\n\x19VTSI_PROJECT_VIEW_SHALLOW\x10\x02\x12\x1d\n\x19VTSI_PROJECT_VIEW_MINIMUM\x10\x03\x32\xb5\x05\n\x08Projects\x12\x62\n\x11\x43reateVtsiProject\x12%.ondewo.vtsi.CreateVtsiProjectRequest\x1a&.ondewo.vtsi.CreateVtsiProjectResponse\x12N\n\x0eGetVtsiProject\x12\".ondewo.vtsi.GetVtsiProjectRequest\x1a\x18.ondewo.vtsi.VtsiProject\x12\x62\n\x11UpdateVtsiProject\x12%.ondewo.vtsi.UpdateVtsiProjectRequest\x1a&.ondewo.vtsi.UpdateVtsiProjectResponse\x12\x62\n\x11\x44\x65leteVtsiProject\x12%.ondewo.vtsi.DeleteVtsiProjectRequest\x1a&.ondewo.vtsi.DeleteVtsiProjectResponse\x12\x62\n\x11\x44\x65ployVtsiProject\x12%.ondewo.vtsi.DeployVtsiProjectRequest\x1a&.ondewo.vtsi.DeployVtsiProjectResponse\x12h\n\x13UndeployVtsiProject\x12\'.ondewo.vtsi.UndeployVtsiProjectRequest\x1a(.ondewo.vtsi.UndeployVtsiProjectResponse\x12_\n\x10ListVtsiProjects\x12$.ondewo.vtsi.ListVtsiProjectsRequest\x1a%.ondewo.vtsi.ListVtsiProjectsResponseb\x06proto3')
 
 _VTSIPROJECTSTATUS = DESCRIPTOR.enum_types_by_name['VtsiProjectStatus']
 VtsiProjectStatus = enum_type_wrapper.EnumTypeWrapper(_VTSIPROJECTSTATUS)
 _VTSIPROJECTSORTINGMODE = DESCRIPTOR.enum_types_by_name['VtsiProjectSortingMode']
 VtsiProjectSortingMode = enum_type_wrapper.EnumTypeWrapper(_VTSIPROJECTSORTINGMODE)
 _VTSIPROJECTVIEW = DESCRIPTOR.enum_types_by_name['VtsiProjectView']
 VtsiProjectView = enum_type_wrapper.EnumTypeWrapper(_VTSIPROJECTVIEW)
@@ -184,20 +184,20 @@
 })
 _sym_db.RegisterMessage(UndeployVtsiProjectResponse)
 
 _PROJECTS = DESCRIPTOR.services_by_name['Projects']
 if _descriptor._USE_C_DESCRIPTORS == False:
 
     DESCRIPTOR._options = None
-    _VTSIPROJECTSTATUS._serialized_start=2498
-    _VTSIPROJECTSTATUS._serialized_end=2637
-    _VTSIPROJECTSORTINGMODE._serialized_start=2639
-    _VTSIPROJECTSORTINGMODE._serialized_end=2694
-    _VTSIPROJECTVIEW._serialized_start=2697
-    _VTSIPROJECTVIEW._serialized_end=2839
+    _VTSIPROJECTSTATUS._serialized_start=2593
+    _VTSIPROJECTSTATUS._serialized_end=2732
+    _VTSIPROJECTSORTINGMODE._serialized_start=2734
+    _VTSIPROJECTSORTINGMODE._serialized_end=2789
+    _VTSIPROJECTVIEW._serialized_start=2792
+    _VTSIPROJECTVIEW._serialized_end=2934
     _VTSIPROJECT._serialized_start=107
     _VTSIPROJECT._serialized_end=528
     _ASTERISKCONFIGSVARIABLES._serialized_start=531
     _ASTERISKCONFIGSVARIABLES._serialized_end=724
     _ASTERISKCONFIGSFILES._serialized_start=727
     _ASTERISKCONFIGSFILES._serialized_end=883
     _ASTERISKCONFIGS._serialized_start=886
@@ -205,33 +205,33 @@
     _CREATEVTSIPROJECTREQUEST._serialized_start=1150
     _CREATEVTSIPROJECTREQUEST._serialized_end=1247
     _CREATEVTSIPROJECTRESPONSE._serialized_start=1249
     _CREATEVTSIPROJECTRESPONSE._serialized_end=1347
     _GETVTSIPROJECTREQUEST._serialized_start=1349
     _GETVTSIPROJECTREQUEST._serialized_end=1386
     _LISTVTSIPROJECTSREQUEST._serialized_start=1389
-    _LISTVTSIPROJECTSREQUEST._serialized_end=1554
-    _LISTVTSIPROJECTSRESPONSE._serialized_start=1556
-    _LISTVTSIPROJECTSRESPONSE._serialized_end=1656
-    _VTSIPROJECTSORTING._serialized_start=1659
-    _VTSIPROJECTSORTING._serialized_end=2025
-    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_start=1821
-    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_end=2025
-    _UPDATEVTSIPROJECTREQUEST._serialized_start=2027
-    _UPDATEVTSIPROJECTREQUEST._serialized_end=2101
-    _UPDATEVTSIPROJECTRESPONSE._serialized_start=2103
-    _UPDATEVTSIPROJECTRESPONSE._serialized_end=2167
-    _DELETEVTSIPROJECTREQUEST._serialized_start=2169
-    _DELETEVTSIPROJECTREQUEST._serialized_end=2209
-    _DELETEVTSIPROJECTRESPONSE._serialized_start=2211
-    _DELETEVTSIPROJECTRESPONSE._serialized_end=2275
-    _DEPLOYVTSIPROJECTREQUEST._serialized_start=2277
-    _DEPLOYVTSIPROJECTREQUEST._serialized_end=2317
-    _DEPLOYVTSIPROJECTRESPONSE._serialized_start=2319
-    _DEPLOYVTSIPROJECTRESPONSE._serialized_end=2383
-    _UNDEPLOYVTSIPROJECTREQUEST._serialized_start=2385
-    _UNDEPLOYVTSIPROJECTREQUEST._serialized_end=2427
-    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_start=2429
-    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_end=2495
-    _PROJECTS._serialized_start=2842
-    _PROJECTS._serialized_end=3535
+    _LISTVTSIPROJECTSREQUEST._serialized_end=1604
+    _LISTVTSIPROJECTSRESPONSE._serialized_start=1606
+    _LISTVTSIPROJECTSRESPONSE._serialized_end=1706
+    _VTSIPROJECTSORTING._serialized_start=1709
+    _VTSIPROJECTSORTING._serialized_end=2120
+    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_start=1881
+    _VTSIPROJECTSORTING_VTSIPROJECTSORTINGFIELD._serialized_end=2085
+    _UPDATEVTSIPROJECTREQUEST._serialized_start=2122
+    _UPDATEVTSIPROJECTREQUEST._serialized_end=2196
+    _UPDATEVTSIPROJECTRESPONSE._serialized_start=2198
+    _UPDATEVTSIPROJECTRESPONSE._serialized_end=2262
+    _DELETEVTSIPROJECTREQUEST._serialized_start=2264
+    _DELETEVTSIPROJECTREQUEST._serialized_end=2304
+    _DELETEVTSIPROJECTRESPONSE._serialized_start=2306
+    _DELETEVTSIPROJECTRESPONSE._serialized_end=2370
+    _DEPLOYVTSIPROJECTREQUEST._serialized_start=2372
+    _DEPLOYVTSIPROJECTREQUEST._serialized_end=2412
+    _DEPLOYVTSIPROJECTRESPONSE._serialized_start=2414
+    _DEPLOYVTSIPROJECTRESPONSE._serialized_end=2478
+    _UNDEPLOYVTSIPROJECTREQUEST._serialized_start=2480
+    _UNDEPLOYVTSIPROJECTREQUEST._serialized_end=2522
+    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_start=2524
+    _UNDEPLOYVTSIPROJECTRESPONSE._serialized_end=2590
+    _PROJECTS._serialized_start=2937
+    _PROJECTS._serialized_end=3630
 # @@protoc_insertion_point(module_scope)
```

### Comparing `ondewo-vtsi-client-6.3.1/ondewo/vtsi/projects_pb2_grpc.py` & `ondewo-vtsi-client-6.4.0/ondewo/vtsi/projects_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/PKG-INFO` & `ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ondewo-vtsi-client
-Version: 6.3.1
+Version: 6.4.0
 Summary: exposes the ondewo-vtsi endpoints in a user-friendly way
 Home-page: https://github.com/ondewo/ondewo-vtsi-client-python
 Author: Ondewo GbmH
 Author-email: office@ondewo.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.3.1 Summary: exposes
+Metadata-Version: 2.1 Name: ondewo-vtsi-client Version: 6.4.0 Summary: exposes
 the ondewo-vtsi endpoints in a user-friendly way Home-page: https://github.com/
 ondewo/ondewo-vtsi-client-python Author: Ondewo GbmH Author-email:
 office@ondewo.com License: UNKNOWN Platform: UNKNOWN Classifier: Programming
 Language :: Python :: 3.8 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 5 - Production/Stable Classifier: Topic ::
 Software Development :: Libraries Requires-Python: >=3 Description-Content-
 Type: text/markdown License-File: LICENSE
```

### Comparing `ondewo-vtsi-client-6.3.1/ondewo_vtsi_client.egg-info/SOURCES.txt` & `ondewo-vtsi-client-6.4.0/ondewo_vtsi_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ondewo-vtsi-client-6.3.1/setup.py` & `ondewo-vtsi-client-6.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
             req_str = f"{req_name} @ {req_url}"
         else:
             req_str = req
         requires.append(req_str)
 
 setup(
     name="ondewo-vtsi-client",
-    version='6.3.1',
+    version='6.4.0',
     author="Ondewo GbmH",
     author_email="office@ondewo.com",
     description="exposes the ondewo-vtsi endpoints in a user-friendly way",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ondewo/ondewo-vtsi-client-python",
     packages=[
```

