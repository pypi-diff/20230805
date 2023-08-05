# Comparing `tmp/mqtt-recorder-1.2.0.tar.gz` & `tmp/mqtt-recorder-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/mqtt-recorder-1.2.0.tar", last modified: Wed Oct 28 20:16:05 2020, max compression
+gzip compressed data, was "mqtt-recorder-1.3.0.tar", last modified: Sat Aug  5 15:26:26 2023, max compression
```

## Comparing `mqtt-recorder-1.2.0.tar` & `mqtt-recorder-1.3.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 arpad     (1000) arpad     (1000)        0 2020-10-28 20:16:05.090152 mqtt-recorder-1.2.0/
--rw-rw-r--   0 arpad     (1000) arpad     (1000)     2895 2020-10-28 20:16:05.090152 mqtt-recorder-1.2.0/PKG-INFO
--rw-rw-r--   0 arpad     (1000) arpad     (1000)     2286 2020-10-28 20:05:09.000000 mqtt-recorder-1.2.0/README.md
-drwxrwxr-x   0 arpad     (1000) arpad     (1000)        0 2020-10-28 20:16:05.090152 mqtt-recorder-1.2.0/mqtt_recorder/
--rw-rw-r--   0 arpad     (1000) arpad     (1000)        0 2020-10-28 20:05:09.000000 mqtt-recorder-1.2.0/mqtt_recorder/__init__.py
--rw-rw-r--   0 arpad     (1000) arpad     (1000)     2931 2020-10-28 20:05:09.000000 mqtt-recorder-1.2.0/mqtt_recorder/__main__.py
--rw-rw-r--   0 arpad     (1000) arpad     (1000)     4037 2020-10-28 20:05:09.000000 mqtt-recorder-1.2.0/mqtt_recorder/recorder.py
-drwxrwxr-x   0 arpad     (1000) arpad     (1000)        0 2020-10-28 20:16:05.090152 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/
--rw-rw-r--   0 arpad     (1000) arpad     (1000)     2895 2020-10-28 20:16:04.000000 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/PKG-INFO
--rw-rw-r--   0 arpad     (1000) arpad     (1000)      320 2020-10-28 20:16:05.000000 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/SOURCES.txt
--rw-rw-r--   0 arpad     (1000) arpad     (1000)        1 2020-10-28 20:16:04.000000 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/dependency_links.txt
--rw-rw-r--   0 arpad     (1000) arpad     (1000)       63 2020-10-28 20:16:04.000000 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/entry_points.txt
--rw-rw-r--   0 arpad     (1000) arpad     (1000)       15 2020-10-28 20:16:04.000000 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/requires.txt
--rw-rw-r--   0 arpad     (1000) arpad     (1000)       14 2020-10-28 20:16:04.000000 mqtt-recorder-1.2.0/mqtt_recorder.egg-info/top_level.txt
--rw-rw-r--   0 arpad     (1000) arpad     (1000)       38 2020-10-28 20:16:05.090152 mqtt-recorder-1.2.0/setup.cfg
--rw-rw-r--   0 arpad     (1000) arpad     (1000)      595 2020-10-28 20:09:30.000000 mqtt-recorder-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:26:26.344440 mqtt-recorder-1.3.0/
+-rw-rw-rw-   0        0        0     1083 2023-08-04 22:19:10.000000 mqtt-recorder-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0     4072 2023-08-05 15:26:26.344440 mqtt-recorder-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2525 2023-08-05 15:06:20.000000 mqtt-recorder-1.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 15:26:26.308293 mqtt-recorder-1.3.0/mqtt_recorder/
+-rw-rw-rw-   0        0        0        0 2023-08-04 22:19:10.000000 mqtt-recorder-1.3.0/mqtt_recorder/__init__.py
+-rw-rw-rw-   0        0        0     3417 2023-08-05 15:06:20.000000 mqtt-recorder-1.3.0/mqtt_recorder/__main__.py
+-rw-rw-rw-   0        0        0     4331 2023-08-05 15:06:20.000000 mqtt-recorder-1.3.0/mqtt_recorder/recorder.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:26:26.336391 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/
+-rw-rw-rw-   0        0        0     4072 2023-08-05 15:26:26.000000 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2023-08-05 15:26:26.000000 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 15:26:26.000000 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2023-08-05 15:26:26.000000 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-08-05 15:26:26.000000 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-08-05 15:26:26.000000 mqtt-recorder-1.3.0/mqtt_recorder.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      563 2023-08-05 15:22:50.000000 mqtt-recorder-1.3.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 15:26:26.344440 mqtt-recorder-1.3.0/setup.cfg
```

### Comparing `mqtt-recorder-1.2.0/PKG-INFO` & `mqtt-recorder-1.3.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,54 +1,45 @@
-Metadata-Version: 2.1
-Name: mqtt-recorder
-Version: 1.2.0
-Summary: MQTT recorder tool
-Home-page: https://github.com/rpdswtk/mqtt_recorder
-Author: RPDSWTK
-License: UNKNOWN
-Description: # MQTT Recorder
-        
-        Simple cli tool for recording and replaying MQTT messages.
-        
-        # Install
-        
-        `pip install mqtt-recorder`
-        
-        ## Usage
-        |   Argument   |                        Description                       | Required | Default |
-        |:------------:|:--------------------------------------------------------:|----------|:-------:|
-        | -h, --help   | Show help                                                |          |         |
-        | --host       | MQTT broker address                                      |     x    |         |
-        | --port       | MQTT broker port                                         |          | 1883    |
-        | --mode       | mode: record/replay                                      |     x    |         |
-        | --file       | output/input csv file                                    |     x    |         |
-        | --loop       | looping replay                                           |          | false   |
-        | --qos        | Quality of Service that will be used for subscriptions   |          | 0       |
-        | --topics     | json file containing selected topics for subscriptions   |          | null    |
-        | --enable_ssl | True to enable MQTTs support, False otherwise            |          | False   |
-        | --ca_cert    | Path to the Certificate Authority certificate files      |          | None    |
-        | --certfile   | Path to the client certificate                           |          | None    |
-        | --keyfile    | Path to the client private key                           |          | None    |
-        | --username   | MQTT broker username                                     |          | None    |
-        | --password   | MQTT broker password                                     |          | None    |
-        | --encode_b64 | True to store message payloads as base64 encoded strings |          | False   |
-        ### Recording
-        #### Subscribing to every topic
-        `mqtt-recorder --host localhost --mode record --file recording.csv`
-        #### Subscribing to selected topics
-        `mqtt-recorder --host localhost --mode record --file test.csv --topics topics.json`<br>
-        Topics can be selected using a json file.
-        Example
-        ```json
-        {
-            "topics": [
-                "/myhome/groundfloor/livingroom/temperature",
-                "USA/California/San Francisco/Silicon Valley"
-            ]
-        }
-        ```
-        ### Replaying
-        `mqtt-recorder --host localhost --mode replay --file test.csv`
-        
-Platform: UNKNOWN
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
+# MQTT Recorder
+
+Simple cli tool for recording and replaying MQTT messages.
+
+# Install
+
+`pip install mqtt-recorder`
+
+## Usage
+|   Argument   |                        Description                       | Required | Default |
+|:------------:|:--------------------------------------------------------:|----------|:-------:|
+| -h, --help   | Show help                                                |          |         |
+| --host       | MQTT broker address                                      |     x    |         |
+| --port       | MQTT broker port                                         |          | 1883    |
+| --client_id  | MQTT Client ID                                           |          |         |
+| --mode       | mode: record/replay                                      |     x    |         |
+| --file       | output/input csv file                                    |     x    |         |
+| --loop       | looping replay                                           |          | false   |
+| --qos        | Quality of Service that will be used for subscriptions   |          | 0       |
+| --topics     | json file containing selected topics for subscriptions   |          | null    |
+| --enable_ssl | True to enable MQTTs support, False otherwise            |          | False   |
+| --tls_insecure| If certs is self-generated, change to True              |          | False   |
+| --ca_cert    | Path to the Certificate Authority certificate files      |          | None    |
+| --certfile   | Path to the client certificate                           |          | None    |
+| --keyfile    | Path to the client private key                           |          | None    |
+| --username   | MQTT broker username                                     |          | None    |
+| --password   | MQTT broker password                                     |          | None    |
+| --encode_b64 | True to store message payloads as base64 encoded strings |          | False   |
+### Recording
+#### Subscribing to every topic
+`mqtt-recorder --host localhost --mode record --file recording.csv`
+#### Subscribing to selected topics
+`mqtt-recorder --host localhost --mode record --file test.csv --topics topics.json`<br>
+Topics can be selected using a json file.
+Example
+```json
+{
+    "topics": [
+        "/myhome/groundfloor/livingroom/temperature",
+        "USA/California/San Francisco/Silicon Valley"
+    ]
+}
+```
+### Replaying
+`mqtt-recorder --host localhost --mode replay --file test.csv`
```

### Comparing `mqtt-recorder-1.2.0/mqtt_recorder/recorder.py` & `mqtt-recorder-1.3.0/mqtt_recorder/recorder.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,110 +1,112 @@
-import paho.mqtt.client as mqtt
-import logging
-import time
-import base64
-import csv
-import json
-from tqdm import tqdm
-
-logging.basicConfig(
-    level=logging.DEBUG, 
-    format='[%(asctime)s] - %(name)s - %(levelname)s - %(message)s'
-)
-logger = logging.getLogger('MQTTRecorder')
-
-class SslContext():
-
-    def __init__(self, enable, ca_cert, certfile, keyfile):
-        self.enable = enable
-        self.ca_cert = ca_cert
-        self.certfile = certfile
-        self.keyfile = keyfile
-
-
-class MqttRecorder:
-
-    def __init__(self, host: str, port: int, file_name: str, username: str,
-                 password: str, sslContext: SslContext, encode_b64: bool):
-        self.__recording = False
-        self.__messages = list()
-        self.__file_name = file_name
-        self.__last_message_time = None
-        self.__encode_b64 = encode_b64
-        self.__client = mqtt.Client()
-        self.__client.on_connect = self.__on_connect
-        self.__client.on_message = self.__on_message
-        if username is not None:
-            self.__client.username_pw_set(username, password)
-        if sslContext.enable:
-            self.__client.tls_set(sslContext.ca_cert, sslContext.certfile, sslContext.keyfile)
-        
-        self.__client.connect(host=host, port=port)
-        self.__client.loop_start()
-
-
-    def start_recording(self, topics_file: str, qos: int=0):
-        self.__last_message_time = time.time()
-        if topics_file:
-            with open(topics_file) as json_file:
-                data = json.load(json_file)
-                for topic in data['topics']:
-                    self.__client.subscribe(topic, qos=qos)
-        else:
-            self.__client.subscribe('#', qos=qos)
-        self.__recording = True
-
-    def start_replay(self, loop: bool):
-        def decode_payload(payload, encode_b64):
-            return base64.b64decode(payload) if encode_b64 else payload
-
-        with open(self.__file_name, newline='') as csvfile:
-            logger.info('Starting replay')
-            first_message = True
-            reader = csv.reader(csvfile)
-            messages = list(reader)
-            while True:
-                for row in tqdm(messages, desc='MQTT REPLAY'):
-                    if not first_message:
-                        time.sleep(float(row[5]))
-                    else:
-                        first_message = False
-                    mqtt_payload = decode_payload(row[1], self.__encode_b64)
-                    retain = False if row[3] == '0' else True
-                    self.__client.publish(topic=row[0], payload=mqtt_payload,
-                                          qos=int(row[2]), retain=retain)
-                logger.info('End of replay')
-                if loop:
-                    logger.info('Restarting replay')
-                    time.sleep(1)
-                else:
-                    break
-
-
-    def stop_recording(self):
-        self.__client.loop_stop()
-        logger.info('Recording stopped')
-        self.__recording = False
-        logger.info('Saving messages to output file')
-        with open(self.__file_name, 'w', newline='') as csvfile:
-            writer = csv.writer(csvfile)
-            for message in self.__messages:
-                writer.writerow(message)
-
-
-    def __on_connect(self, client, userdata, flags, rc):
-        logger.info("Connected to broker!")
-
-
-    def __on_message(self, client, userdata, msg):
-        def encode_payload(payload, encode_b64):
-            return base64.b64encode(msg.payload).decode() if encode_b64 else payload.decode()
-
-        if self.__recording:
-            logger.info("[MQTT Message received] Topic: %s QoS: %s Retain: %s",
-                        msg.topic, msg.qos, msg.retain)
-            time_now = time.time()
-            time_delta = time_now - self.__last_message_time
-            payload = encode_payload(msg.payload, self.__encode_b64)
-            row = [msg.topic, payload, msg.qos, msg.retain, time_now, time_delta]
-            self.__messages.append(row)
-            self.__last_message_time = time_now
+import paho.mqtt.client as mqtt
+import logging
+import time
+import base64
+import csv
+import json
+from tqdm import tqdm
+
+logging.basicConfig(
+    level=logging.DEBUG, 
+    format='[%(asctime)s] - %(name)s - %(levelname)s - %(message)s'
+)
+logger = logging.getLogger('MQTTRecorder')
+
+class SslContext():
+
+    def __init__(self, enable, ca_cert, certfile, keyfile, tls_insecure):
+        self.enable = enable
+        self.ca_cert = ca_cert
+        self.certfile = certfile
+        self.keyfile = keyfile
+        self.tls_insecure = tls_insecure
+
+
+class MqttRecorder:
+
+    def __init__(self, host: str, port: int, client_id: str, file_name: str, username: str,
+                 password: str, sslContext: SslContext, encode_b64: bool):
+        self.__recording = False
+        self.__messages = list()
+        self.__file_name = file_name
+        self.__last_message_time = None
+        self.__encode_b64 = encode_b64
+        self.__client = mqtt.Client(client_id=client_id)
+        self.__client.on_connect = self.__on_connect
+        self.__client.on_message = self.__on_message
+        if username is not None:
+            self.__client.username_pw_set(username, password)
+        if sslContext.enable:
+            self.__client.tls_set(sslContext.ca_cert, sslContext.certfile, sslContext.keyfile)
+            if sslContext.tls_insecure is True:
+                self.__client.tls_insecure_set(True)
+        self.__client.connect(host=host, port=port)
+        self.__client.loop_start()
+
+
+    def start_recording(self, topics_file: str, qos: int=0):
+        self.__last_message_time = time.time()
+        if topics_file:
+            with open(topics_file) as json_file:
+                data = json.load(json_file)
+                for topic in data['topics']:
+                    self.__client.subscribe(topic, qos=qos)
+        else:
+            self.__client.subscribe('#', qos=qos)
+        self.__recording = True
+
+    def start_replay(self, loop: bool):
+        def decode_payload(payload, encode_b64):
+            return base64.b64decode(payload) if encode_b64 else payload
+
+        with open(self.__file_name, newline='') as csvfile:
+            logger.info('Starting replay')
+            first_message = True
+            reader = csv.reader(csvfile)
+            messages = list(reader)
+            while True:
+                for row in tqdm(messages, desc='MQTT REPLAY'):
+                    if not first_message:
+                        time.sleep(float(row[5]))
+                    else:
+                        first_message = False
+                    mqtt_payload = decode_payload(row[1], self.__encode_b64)
+                    retain = False if row[3] == '0' else True
+                    self.__client.publish(topic=row[0], payload=mqtt_payload,
+                                          qos=int(row[2]), retain=retain)
+                logger.info('End of replay')
+                if loop:
+                    logger.info('Restarting replay')
+                    time.sleep(1)
+                else:
+                    break
+
+
+    def stop_recording(self):
+        self.__client.loop_stop()
+        logger.info('Recording stopped')
+        self.__recording = False
+        logger.info('Saving messages to output file')
+        with open(self.__file_name, 'w', newline='') as csvfile:
+            writer = csv.writer(csvfile)
+            for message in self.__messages:
+                writer.writerow(message)
+
+
+    def __on_connect(self, client, userdata, flags, rc):
+        logger.info("Connected to broker!")
+
+
+    def __on_message(self, client, userdata, msg):
+        def encode_payload(payload, encode_b64):
+            return base64.b64encode(msg.payload).decode() if encode_b64 else payload.decode()
+
+        if self.__recording:
+            logger.info("[MQTT Message received] Topic: %s QoS: %s Retain: %s",
+                        msg.topic, msg.qos, msg.retain)
+            time_now = time.time()
+            time_delta = time_now - self.__last_message_time
+            payload = encode_payload(msg.payload, self.__encode_b64)
+            row = [msg.topic, payload, msg.qos, msg.retain, time_now, time_delta]
+            self.__messages.append(row)
+            self.__last_message_time = time_now
```

