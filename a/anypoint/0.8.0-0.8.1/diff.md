# Comparing `tmp/anypoint-0.8.0.tar.gz` & `tmp/anypoint-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anypoint-0.8.0.tar", last modified: Thu Mar  2 16:40:20 2023, max compression
+gzip compressed data, was "anypoint-0.8.1.tar", last modified: Sun Mar  5 23:34:49 2023, max compression
```

## Comparing `anypoint-0.8.0.tar` & `anypoint-0.8.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0       43 2023-01-26 15:38:20.500388 anypoint-0.8.0/.gitignore
--rw-r--r--   0        0        0     1099 2022-05-21 00:47:41.295000 anypoint-0.8.0/LICENSE
--rw-r--r--   0        0        0      751 2022-09-07 21:46:25.244226 anypoint-0.8.0/README.md
--rw-r--r--   0        0        0      131 2023-03-02 16:39:53.051555 anypoint-0.8.0/anypoint/__init__.py
--rw-r--r--   0        0        0     2351 2023-03-02 13:59:25.439392 anypoint-0.8.0/anypoint/anypoint.py
--rw-r--r--   0        0        0        0 2022-08-27 14:54:48.596500 anypoint-0.8.0/anypoint/api/__init__.py
--rw-r--r--   0        0        0      744 2022-10-25 01:24:44.951371 anypoint-0.8.0/anypoint/api/api_manager.py
--rw-r--r--   0        0        0     2864 2022-11-09 03:58:06.056091 anypoint-0.8.0/anypoint/api/application.py
--rw-r--r--   0        0        0      244 2022-08-27 15:04:56.867694 anypoint-0.8.0/anypoint/api/environment.py
--rw-r--r--   0        0        0     1421 2022-09-07 21:46:32.724039 anypoint-0.8.0/anypoint/api/monitoring.py
--rw-r--r--   0        0        0     2272 2023-03-02 16:38:46.733880 anypoint-0.8.0/anypoint/api/mq.py
--rw-r--r--   0        0        0     1374 2022-10-27 16:26:23.957360 anypoint-0.8.0/anypoint/api/organization.py
--rw-r--r--   0        0        0     1540 2022-08-28 14:51:16.009115 anypoint-0.8.0/anypoint/authentication.py
--rw-r--r--   0        0        0       93 2022-06-17 22:51:42.220249 anypoint-0.8.0/anypoint/constants.py
--rw-r--r--   0        0        0        0 2022-06-17 21:08:31.328547 anypoint-0.8.0/anypoint/http_client/__init__.py
--rw-r--r--   0        0        0     2247 2023-03-02 16:11:56.028258 anypoint-0.8.0/anypoint/http_client/client.py
--rw-r--r--   0        0        0        0 2022-06-17 20:51:46.804411 anypoint-0.8.0/anypoint/models/__init__.py
--rw-r--r--   0        0        0     1983 2022-10-25 01:24:56.305742 anypoint-0.8.0/anypoint/models/api.py
--rw-r--r--   0        0        0     2591 2022-11-09 03:56:28.180823 anypoint-0.8.0/anypoint/models/application.py
--rw-r--r--   0        0        0     2808 2023-03-02 16:37:57.538012 anypoint-0.8.0/anypoint/models/destination.py
--rw-r--r--   0        0        0     1717 2023-03-02 16:38:29.249783 anypoint-0.8.0/anypoint/models/environment.py
--rw-r--r--   0        0        0     6061 2022-11-23 14:16:51.793610 anypoint-0.8.0/anypoint/models/organization.py
--rw-r--r--   0        0        0     1506 2022-08-29 14:43:07.718672 anypoint-0.8.0/anypoint/models/statistics.py
--rw-r--r--   0        0        0     1672 2022-06-27 22:28:00.338479 anypoint-0.8.0/anypoint/models/worker.py
--rw-r--r--   0        0        0      146 2022-06-17 22:52:02.909907 anypoint-0.8.0/anypoint/utils.py
--rw-r--r--   0        0        0      424 2022-10-24 23:37:47.032214 anypoint-0.8.0/pyproject.toml
--rw-r--r--   0        0        0        0 2022-06-17 19:46:08.652410 anypoint-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 anypoint-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0       43 2023-01-26 15:38:20.500388 anypoint-0.8.1/.gitignore
+-rw-r--r--   0        0        0     1099 2022-05-21 00:47:41.295000 anypoint-0.8.1/LICENSE
+-rw-r--r--   0        0        0      751 2022-09-07 21:46:25.244226 anypoint-0.8.1/README.md
+-rw-r--r--   0        0        0      131 2023-03-05 23:34:46.472220 anypoint-0.8.1/anypoint/__init__.py
+-rw-r--r--   0        0        0     2351 2023-03-02 13:59:25.439392 anypoint-0.8.1/anypoint/anypoint.py
+-rw-r--r--   0        0        0        0 2022-08-27 14:54:48.596500 anypoint-0.8.1/anypoint/api/__init__.py
+-rw-r--r--   0        0        0      744 2022-10-25 01:24:44.951371 anypoint-0.8.1/anypoint/api/api_manager.py
+-rw-r--r--   0        0        0     2864 2022-11-09 03:58:06.056091 anypoint-0.8.1/anypoint/api/application.py
+-rw-r--r--   0        0        0      244 2022-08-27 15:04:56.867694 anypoint-0.8.1/anypoint/api/environment.py
+-rw-r--r--   0        0        0     1421 2022-09-07 21:46:32.724039 anypoint-0.8.1/anypoint/api/monitoring.py
+-rw-r--r--   0        0        0     2272 2023-03-02 16:38:46.733880 anypoint-0.8.1/anypoint/api/mq.py
+-rw-r--r--   0        0        0     1374 2022-10-27 16:26:23.957360 anypoint-0.8.1/anypoint/api/organization.py
+-rw-r--r--   0        0        0     1540 2022-08-28 14:51:16.009115 anypoint-0.8.1/anypoint/authentication.py
+-rw-r--r--   0        0        0       93 2022-06-17 22:51:42.220249 anypoint-0.8.1/anypoint/constants.py
+-rw-r--r--   0        0        0        0 2022-06-17 21:08:31.328547 anypoint-0.8.1/anypoint/http_client/__init__.py
+-rw-r--r--   0        0        0     2247 2023-03-02 16:11:56.028258 anypoint-0.8.1/anypoint/http_client/client.py
+-rw-r--r--   0        0        0        0 2022-06-17 20:51:46.804411 anypoint-0.8.1/anypoint/models/__init__.py
+-rw-r--r--   0        0        0     1983 2022-10-25 01:24:56.305742 anypoint-0.8.1/anypoint/models/api.py
+-rw-r--r--   0        0        0     2591 2022-11-09 03:56:28.180823 anypoint-0.8.1/anypoint/models/application.py
+-rw-r--r--   0        0        0     3049 2023-03-05 17:20:15.142643 anypoint-0.8.1/anypoint/models/destination.py
+-rw-r--r--   0        0        0     1717 2023-03-02 16:38:29.249783 anypoint-0.8.1/anypoint/models/environment.py
+-rw-r--r--   0        0        0     6061 2022-11-23 14:16:51.793610 anypoint-0.8.1/anypoint/models/organization.py
+-rw-r--r--   0        0        0     1506 2022-08-29 14:43:07.718672 anypoint-0.8.1/anypoint/models/statistics.py
+-rw-r--r--   0        0        0     1672 2022-06-27 22:28:00.338479 anypoint-0.8.1/anypoint/models/worker.py
+-rw-r--r--   0        0        0      146 2022-06-17 22:52:02.909907 anypoint-0.8.1/anypoint/utils.py
+-rw-r--r--   0        0        0      424 2022-10-24 23:37:47.032214 anypoint-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-06-17 19:46:08.652410 anypoint-0.8.1/tests/__init__.py
+-rw-r--r--   0        0        0      330 1970-01-01 00:00:00.000000 anypoint-0.8.1/PKG-INFO
```

### Comparing `anypoint-0.8.0/LICENSE` & `anypoint-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/README.md` & `anypoint-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/anypoint.py` & `anypoint-0.8.1/anypoint/anypoint.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/api/api_manager.py` & `anypoint-0.8.1/anypoint/api/api_manager.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/api/application.py` & `anypoint-0.8.1/anypoint/api/application.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/api/monitoring.py` & `anypoint-0.8.1/anypoint/api/monitoring.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/api/mq.py` & `anypoint-0.8.1/anypoint/api/mq.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/api/organization.py` & `anypoint-0.8.1/anypoint/api/organization.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/authentication.py` & `anypoint-0.8.1/anypoint/authentication.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/http_client/client.py` & `anypoint-0.8.1/anypoint/http_client/client.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/models/api.py` & `anypoint-0.8.1/anypoint/models/api.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/models/application.py` & `anypoint-0.8.1/anypoint/models/application.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/models/destination.py` & `anypoint-0.8.1/anypoint/models/destination.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,17 +35,16 @@
 
 
 class Queue:
     def __init__(self, raw_json):
         # {'destination': 'CUSTOMER-CREATE-SFMC-Q', 'messages': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 144}], 'inflightMessages': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}], 'messagesVisible': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 144}], 'messagesSent': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 57}], 'messagesReceived': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}], 'messagesAcked': [{'date': '2023-03-01T16:34:00.000+00:00', 'value': 0}]}
         self.destination: str = raw_json.get("destination")
         # Grab the value of the first item in the list
-        self.messages = raw_json.get("messages", [{}])[0].get("value")
-        self.inflight_messages = raw_json.get("inflightMessages", [{}])[0].get("value")
-        self.messages_visible = raw_json.get("messagesVisible", [{}])[0].get("value")
-        self.messages_sent = raw_json.get("messagesSent", [{}])[0].get("value")
-        self.messages_received = raw_json.get("messagesReceived", [{}])[0].get("value")
-        self.messages_acked = raw_json.get("messagesAcked", [{}])[0].get("value")
+        self.messages = raw_json.get("messages", [{}])[0].get("value") if raw_json.get("messages") else 0
+        self.inflight_messages = raw_json.get("inflightMessages", [{}])[0].get("value") if raw_json.get("inflightMessages") else 0
+        self.messages_visible = raw_json.get("messagesVisible", [{}])[0].get("value") if raw_json.get("messagesVisible") else 0
+        self.messages_sent = raw_json.get("messagesSent", [{}])[0].get("value") if raw_json.get("messagesSent") else 0
+        self.messages_received = raw_json.get("messagesReceived", [{}])[0].get("value") if raw_json.get("messagesReceived") else 0
+        self.messages_acked = raw_json.get("messagesAcked", [{}])[0].get("value") if raw_json.get("messagesAcked") else 0
 
     def __repr__(self):
         return f"Queue({self.destination}, {self.messages=}, {self.inflight_messages=}, {self.messages_visible=}, {self.messages_sent=}, {self.messages_received=}, {self.messages_acked=})"
-
```

### Comparing `anypoint-0.8.0/anypoint/models/environment.py` & `anypoint-0.8.1/anypoint/models/environment.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/models/organization.py` & `anypoint-0.8.1/anypoint/models/organization.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/models/statistics.py` & `anypoint-0.8.1/anypoint/models/statistics.py`

 * *Files identical despite different names*

### Comparing `anypoint-0.8.0/anypoint/models/worker.py` & `anypoint-0.8.1/anypoint/models/worker.py`

 * *Files identical despite different names*

