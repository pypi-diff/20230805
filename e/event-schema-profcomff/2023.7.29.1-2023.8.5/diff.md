# Comparing `tmp/event_schema_profcomff-2023.7.29.1.tar.gz` & `tmp/event_schema_profcomff-2023.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "event_schema_profcomff-2023.7.29.1.tar", last modified: Sat Jul 29 13:19:01 2023, max compression
+gzip compressed data, was "event_schema_profcomff-2023.8.5.tar", last modified: Sat Aug  5 19:21:42 2023, max compression
```

## Comparing `event_schema_profcomff-2023.7.29.1.tar` & `event_schema_profcomff-2023.8.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/event_schema/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/event_schema/auth/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/auth/user_login.py
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/event_schema/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-29 13:19:01.000000 event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-29 13:19:01.626484 event_schema_profcomff-2023.7.29.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-29 13:18:47.000000 event_schema_profcomff-2023.7.29.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:21:42.303895 event_schema_profcomff-2023.8.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-05 19:21:42.303895 event_schema_profcomff-2023.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:21:42.299895 event_schema_profcomff-2023.8.5/event_schema/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/event_schema/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:21:42.299895 event_schema_profcomff-2023.8.5/event_schema/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/event_schema/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/event_schema/auth/user_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/event_schema/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 19:21:42.303895 event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-08-05 19:21:42.000000 event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-08-05 19:21:42.000000 event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 19:21:42.000000 event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 19:21:42.000000 event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-08-05 19:21:42.000000 event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 19:21:42.303895 event_schema_profcomff-2023.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-08-05 19:21:31.000000 event_schema_profcomff-2023.8.5/setup.py
```

### Comparing `event_schema_profcomff-2023.7.29.1/LICENSE` & `event_schema_profcomff-2023.8.5/LICENSE`

 * *Files identical despite different names*

### Comparing `event_schema_profcomff-2023.7.29.1/PKG-INFO` & `event_schema_profcomff-2023.8.5/event_schema_profcomff.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
-Name: event_schema_profcomff
-Version: 2023.7.29.1
+Name: event-schema-profcomff
+Version: 2023.8.5
 Home-page: https://github.com/profcomff/event-schema
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Библиотека для хранения общих JSON-схем
 
 ## Использование
 ```python
-from event_schema.auth import UserLogin
+from event_schema.auth import UserLogin, UserLoginKey
 from confluent_kafka import Producer
 
 some_data = {} ## insert your data here
 kafka_config = {}
 
 producer = Producer(**kafka_config)
 
 new = UserLogin(**some_data)
+new_key = UserLoginKey(user_id=42)
 
-producer.produce(topic="topic_name", value=new.model_dump_json())
+producer.produce(topic="topic_name", key=new_key.model_dump_json(), value=new.model_dump_json())
+producer.flush()
 ```
```

### Comparing `event_schema_profcomff-2023.7.29.1/event_schema_profcomff.egg-info/PKG-INFO` & `event_schema_profcomff-2023.8.5/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
-Name: event-schema-profcomff
-Version: 2023.7.29.1
+Name: event_schema_profcomff
+Version: 2023.8.5
 Home-page: https://github.com/profcomff/event-schema
 Author: Semyon Grigoriev
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Библиотека для хранения общих JSON-схем
 
 ## Использование
 ```python
-from event_schema.auth import UserLogin
+from event_schema.auth import UserLogin, UserLoginKey
 from confluent_kafka import Producer
 
 some_data = {} ## insert your data here
 kafka_config = {}
 
 producer = Producer(**kafka_config)
 
 new = UserLogin(**some_data)
+new_key = UserLoginKey(user_id=42)
 
-producer.produce(topic="topic_name", value=new.model_dump_json())
+producer.produce(topic="topic_name", key=new_key.model_dump_json(), value=new.model_dump_json())
+producer.flush()
 ```
```

