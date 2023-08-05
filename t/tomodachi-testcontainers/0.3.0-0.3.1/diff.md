# Comparing `tmp/tomodachi_testcontainers-0.3.0.tar.gz` & `tmp/tomodachi_testcontainers-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomodachi_testcontainers-0.3.0.tar", max compression
+gzip compressed data, was "tomodachi_testcontainers-0.3.1.tar", max compression
```

## Comparing `tomodachi_testcontainers-0.3.0.tar` & `tomodachi_testcontainers-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.3.0/LICENSE
--rw-r--r--   0        0        0    26880 2023-07-31 18:13:07.890597 tomodachi_testcontainers-0.3.0/README.md
--rw-r--r--   0        0        0     3997 2023-08-03 07:36:53.880150 tomodachi_testcontainers-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/__init__.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/clients/__init__.py
--rw-r--r--   0        0        0     3487 2023-07-31 18:13:07.895096 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/clients/snssqs_client.py
--rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/__init__.py
--rw-r--r--   0        0        0     3944 2023-07-31 18:13:07.895679 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/common.py
--rw-r--r--   0        0        0     1942 2023-08-03 07:36:44.798845 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/localstack.py
--rw-r--r--   0        0        0     2345 2023-08-03 07:36:44.799109 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/moto.py
--rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/sftp.py
--rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/tomodachi.py
--rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/py.typed
--rw-r--r--   0        0        0     1394 2023-07-31 18:13:07.896643 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/__init__.py
--rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/assertions.py
--rw-r--r--   0        0        0     1121 2023-08-03 07:36:44.799354 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/async_probes.py
--rw-r--r--   0        0        0     2312 2023-07-31 18:13:07.897004 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
--rw-r--r--   0        0        0     2126 2023-08-02 12:29:30.549037 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py
--rw-r--r--   0        0        0     1594 2023-07-31 12:23:17.273453 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
--rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
--rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/utils.py
--rw-r--r--   0        0        0    28110 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-07-23 09:35:29.084747 tomodachi_testcontainers-0.3.1/LICENSE
+-rw-r--r--   0        0        0    26880 2023-07-31 18:13:07.890597 tomodachi_testcontainers-0.3.1/README.md
+-rw-r--r--   0        0        0     3997 2023-08-05 09:23:46.580495 tomodachi_testcontainers-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086660 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.086809 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/clients/__init__.py
+-rw-r--r--   0        0        0     3953 2023-08-05 09:15:34.195694 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/clients/snssqs_client.py
+-rw-r--r--   0        0        0      618 2023-07-23 10:30:40.087330 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/__init__.py
+-rw-r--r--   0        0        0     3944 2023-07-31 18:13:07.895679 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/common.py
+-rw-r--r--   0        0        0     1942 2023-08-03 07:36:44.798845 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/localstack.py
+-rw-r--r--   0        0        0     2345 2023-08-05 09:22:32.578276 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/moto.py
+-rw-r--r--   0        0        0     3129 2023-07-27 14:17:21.583523 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/sftp.py
+-rw-r--r--   0        0        0      930 2023-07-27 14:17:21.583737 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/tomodachi.py
+-rw-r--r--   0        0        0        0 2023-07-23 10:30:40.088391 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/py.typed
+-rw-r--r--   0        0        0     1394 2023-07-31 18:13:07.896643 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/__init__.py
+-rw-r--r--   0        0        0      503 2023-07-23 10:30:40.088800 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/assertions.py
+-rw-r--r--   0        0        0     1121 2023-08-03 07:36:44.799354 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/async_probes.py
+-rw-r--r--   0        0        0     2312 2023-07-31 18:13:07.897004 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py
+-rw-r--r--   0        0        0     2126 2023-08-02 12:29:30.549037 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py
+-rw-r--r--   0        0        0     1594 2023-07-31 12:23:17.273453 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py
+-rw-r--r--   0        0        0      609 2023-07-29 08:49:13.269030 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py
+-rw-r--r--   0        0        0      323 2023-07-23 10:30:40.089565 tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/utils.py
+-rw-r--r--   0        0        0    28110 1970-01-01 00:00:00.000000 tomodachi_testcontainers-0.3.1/PKG-INFO
```

### Comparing `tomodachi_testcontainers-0.3.0/LICENSE` & `tomodachi_testcontainers-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/README.md` & `tomodachi_testcontainers-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/pyproject.toml` & `tomodachi_testcontainers-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomodachi-testcontainers"
-version = "0.3.0"
+version = "0.3.1"
 description = "Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing."
 authors = ["Filips Nastins <nastinsfilips@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 homepage = "https://github.com/filipsnastins/tomodachi-testcontainers"
 repository = "https://github.com/filipsnastins/tomodachi-testcontainers"
```

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/clients/snssqs_client.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/clients/snssqs_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,24 +4,39 @@
 from types_aiobotocore_sns import SNSClient
 from types_aiobotocore_sqs import SQSClient
 from types_aiobotocore_sqs.literals import QueueAttributeFilterType, QueueAttributeNameType
 
 MessageType = TypeVar("MessageType")
 
 
-class TomodachiSNSSQSEnvelope(Protocol):
+class TomodachiSNSSQSEnvelopeStatic(Protocol):
     @classmethod
-    async def build_message(cls: "TomodachiSNSSQSEnvelope", service: Any, topic: str, data: Any, **kwargs: Any) -> str:
+    async def build_message(
+        cls: "TomodachiSNSSQSEnvelopeStatic", service: Any, topic: str, data: Any, **kwargs: Any
+    ) -> str:
         ...
 
     @classmethod
-    async def parse_message(cls: "TomodachiSNSSQSEnvelope", payload: str, **kwargs: Any) -> Union[dict, tuple]:
+    async def parse_message(cls: "TomodachiSNSSQSEnvelopeStatic", payload: str, **kwargs: Any) -> Union[dict, tuple]:
         ...
 
 
+class TomodachiSNSSQSEnvelopeInstance(Protocol):
+    async def build_message(
+        self: "TomodachiSNSSQSEnvelopeInstance", service: Any, topic: str, data: Any, **kwargs: Any
+    ) -> str:
+        ...
+
+    async def parse_message(self: "TomodachiSNSSQSEnvelopeInstance", payload: str, **kwargs: Any) -> Union[dict, tuple]:
+        ...
+
+
+TomodachiSNSSQSEnvelope = Union[TomodachiSNSSQSEnvelopeStatic, TomodachiSNSSQSEnvelopeInstance]
+
+
 async def subscribe_to(sns_client: SNSClient, sqs_client: SQSClient, topic: str, queue: str) -> None:
     """Subscribe a SQS queue to a SNS topic; create the topic and queue if they don't exist."""
     create_topic_response = await sns_client.create_topic(Name=topic)
     topic_arn = create_topic_response["TopicArn"]
 
     create_queue_response = await sqs_client.create_queue(QueueName=queue)
     queue_url = create_queue_response["QueueUrl"]
@@ -32,21 +47,21 @@
     queue_arn = get_queue_attributes_response["Attributes"]["QueueArn"]
 
     await sns_client.subscribe(TopicArn=topic_arn, Protocol="sqs", Endpoint=queue_arn)
 
 
 async def receive(
     sqs_client: SQSClient,
-    queue_name: str,
+    queue: str,
     envelope: TomodachiSNSSQSEnvelope,
     message_type: Type[MessageType],
     max_messages: int = 10,
 ) -> List[MessageType]:
     """Receive messages from a SQS queue."""
-    get_queue_url_response = await sqs_client.get_queue_url(QueueName=queue_name)
+    get_queue_url_response = await sqs_client.get_queue_url(QueueName=queue)
     queue_url = get_queue_url_response["QueueUrl"]
 
     received_messages_response = await sqs_client.receive_message(QueueUrl=queue_url, MaxNumberOfMessages=max_messages)
     received_messages = received_messages_response.get("Messages")
     if not received_messages:
         return []
 
@@ -55,15 +70,15 @@
         payload = json.loads(received_message["Body"])["Message"]
         parsed_message = await envelope.parse_message(payload=payload, proto_class=message_type)
         parsed_messages.append(parsed_message[0]["data"])
         await sqs_client.delete_message(QueueUrl=queue_url, ReceiptHandle=received_message["ReceiptHandle"])
     return parsed_messages
 
 
-async def publish(sns_client: SNSClient, topic: str, data: Any, envelope: TomodachiSNSSQSEnvelope) -> None:
+async def publish(sns_client: SNSClient, topic: str, data: Any, envelope: TomodachiSNSSQSEnvelopeStatic) -> None:
     """Publish a message to a SNS topic."""
     message = await envelope.build_message(service={}, topic=topic, data=data)
 
     list_topics_response = await sns_client.list_topics()
     topic_arn = next((v["TopicArn"] for v in list_topics_response["Topics"] if v["TopicArn"].endswith(topic)), None)
     if not topic_arn:
         raise ValueError(f"Topic does not exist: {topic}")
```

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/__init__.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/common.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/common.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/localstack.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/localstack.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/moto.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/moto.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/sftp.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/sftp.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/containers/tomodachi.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/containers/tomodachi.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/__init__.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/__init__.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/async_probes.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/async_probes.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/localstack_fixtures.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/localstack_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/moto_fixtures.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/moto_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/sftp_fixtures.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/sftp_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py` & `tomodachi_testcontainers-0.3.1/src/tomodachi_testcontainers/pytest/tomodachi_fixtures.py`

 * *Files identical despite different names*

### Comparing `tomodachi_testcontainers-0.3.0/PKG-INFO` & `tomodachi_testcontainers-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomodachi-testcontainers
-Version: 0.3.0
+Version: 0.3.1
 Summary: Collection of Testcontainers, pytest fixtures and test clients for end-to-end/integration testing for Python Tomodachi framework. A great starting point to learn more about Testcontainers and necessity of integration testing.
 Home-page: https://github.com/filipsnastins/tomodachi-testcontainers
 License: MIT
 Author: Filips Nastins
 Author-email: nastinsfilips@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

