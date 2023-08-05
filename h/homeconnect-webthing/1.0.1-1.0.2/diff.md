# Comparing `tmp/homeconnect_webthing-1.0.1.tar.gz` & `tmp/homeconnect_webthing-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "homeconnect_webthing-1.0.1.tar", last modified: Tue Jul 25 04:33:05 2023, max compression
+gzip compressed data, was "homeconnect_webthing-1.0.2.tar", last modified: Sat Aug  5 07:00:18 2023, max compression
```

## Comparing `homeconnect_webthing-1.0.1.tar` & `homeconnect_webthing-1.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/homeconnect_webthing/
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/app.py
--rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/appliances.py
--rw-r--r--   0 runner    (1001) docker     (123)    26282 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/appliances_webthing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3381 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/auth_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6944 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/eventstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/homeconnect.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/homeconnect_webthing/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2411 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-25 04:33:05.000000 homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-25 04:32:53.000000 homeconnect_webthing-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-25 04:33:05.050764 homeconnect_webthing-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:00:18.646225 homeconnect_webthing-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-05 07:00:18.646225 homeconnect_webthing-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:00:18.646225 homeconnect_webthing-1.0.2/homeconnect_webthing/
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9201 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35865 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/appliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26282 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/appliances_webthing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3198 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/auth_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7025 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/eventstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5773 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/homeconnect.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/homeconnect_webthing/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 07:00:18.646225 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-08-05 07:00:18.000000 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-08-05 07:00:18.000000 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 07:00:18.000000 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-08-05 07:00:18.000000 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-08-05 07:00:18.000000 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-08-05 07:00:18.000000 homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-08-05 07:00:05.000000 homeconnect_webthing-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-08-05 07:00:18.650225 homeconnect_webthing-1.0.2/setup.cfg
```

### Comparing `homeconnect_webthing-1.0.1/LICENSE` & `homeconnect_webthing-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/PKG-INFO` & `homeconnect_webthing-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,14 @@
-Metadata-Version: 2.1
-Name: homeconnect_webthing
-Version: 1.0.1
-Summary: Homeconnect WebThing adapter
-Author: Gregor Roth
-Author-email: gregor.roth@web.de
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # homeconnect_webthing
-A webthing adapter of HomeConnect smart home appliances.
+A webthing adapter for HomeConnect smart home devices.
 
-This project provides a [webthing API](https://iot.mozilla.org/wot/) to access [HomeConnect devices](https://api-docs.home-connect.com/). 
-Currently, the device types ***Dishwasher***, ***Washer*** and ***Dryer*** are supported only 
+This project provides a [webthing API](https://iot.mozilla.org/wot/) for accessing [HomeConnect devices](https://api-docs.home-connect.com/).
+Currently, only the ***dishwasher***, ***washing machine*** and ***dryer*** device types are supported.
 
-The homeconnect_webthing package exposes a http webthing endpoint for each detected and supported smart home appliances. E.g. 
+The homeconnect_webthing package provides an http webthing endpoint for each detected and supported smart home device. E.g.
 ```
 # webthing has been started on host 192.168.0.23
 curl http://192.168.0.23:8744/0/properties 
 
 {
    "device_name":"Geschirrspüler",
    "device_type":"Dishwasher",
@@ -35,26 +25,26 @@
    "program_hygiene_plus":false,
    "program_extra_try":false,
    "program_start_date":"",
    "program_progress":0
 }
 ```
 
-To install this software you may use [PIP](https://realpython.com/what-is-pip/) package manager such as shown below
+To install this software, you can use the [PIP](https://realpython.com/what-is-pip/) package manager as shown below
 
 **PIP approach**
 ```
 sudo pip3 install homeconnect_webthing
 ```
 
-After this installation you may start the webthing http endpoint inside your python code or via command line using
+After this installation, you can use the Webthing http endpoint in your Python code or from the command line with
 ```
 sudo homeconnect --command listen --port 8744 --refresh_token 9yJ4LXJlZyI6IfVVIiwi...2YXRlIn0= --client_secret FEAE...522BD0 
 ```
-Here, the webthing API will be bound to the local port 8744. Furthermore, the refresh_token and client_secret have to be set. 
-Please refer [HomeConnect Authorization](https://api-docs.home-connect.com/quickstart?#authorization) to get your refresh_token and client_secret
+Here the webthing API is bound to the local port 8744. Also, refresh_token and client_secret must be set.
+Please refer to [HomeConnect Authorization](https://api-docs.home-connect.com/quickstart?#authorization) to obtain your refresh_token and client_secret
 
-Alternatively to the *listen* command, you can use the *register* command to register and start the webthing service as systemd unit.
-By doing this the webthing service will be started automatically on boot. Starting the server manually using the *listen* command is no longer necessary.
+As an alternative to the *list* command, you can also use the *register* command to register and start the webthing service as a systemd entity.
+This way, the webthing service is started automatically at boot time. Starting the server manually with the *listen* command is no longer necessary.
 ```
 sudo homeconnect --command register --port 8744 --refresh_token 9yJ4LXJlZyI6IfVVIiwi...2YXRlIn0= --client_secret FEAE...522BD0
 ```
```

### Comparing `homeconnect_webthing-1.0.1/README.md` & `homeconnect_webthing-1.0.2/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,24 @@
+Metadata-Version: 2.1
+Name: homeconnect_webthing
+Version: 1.0.2
+Summary: Homeconnect WebThing adapter
+Author: Gregor Roth
+Author-email: gregor.roth@web.de
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # homeconnect_webthing
-A webthing adapter of HomeConnect smart home appliances.
+A webthing adapter for HomeConnect smart home devices.
 
-This project provides a [webthing API](https://iot.mozilla.org/wot/) to access [HomeConnect devices](https://api-docs.home-connect.com/). 
-Currently, the device types ***Dishwasher***, ***Washer*** and ***Dryer*** are supported only 
+This project provides a [webthing API](https://iot.mozilla.org/wot/) for accessing [HomeConnect devices](https://api-docs.home-connect.com/).
+Currently, only the ***dishwasher***, ***washing machine*** and ***dryer*** device types are supported.
 
-The homeconnect_webthing package exposes a http webthing endpoint for each detected and supported smart home appliances. E.g. 
+The homeconnect_webthing package provides an http webthing endpoint for each detected and supported smart home device. E.g.
 ```
 # webthing has been started on host 192.168.0.23
 curl http://192.168.0.23:8744/0/properties 
 
 {
    "device_name":"Geschirrspüler",
    "device_type":"Dishwasher",
@@ -25,26 +35,26 @@
    "program_hygiene_plus":false,
    "program_extra_try":false,
    "program_start_date":"",
    "program_progress":0
 }
 ```
 
-To install this software you may use [PIP](https://realpython.com/what-is-pip/) package manager such as shown below
+To install this software, you can use the [PIP](https://realpython.com/what-is-pip/) package manager as shown below
 
 **PIP approach**
 ```
 sudo pip3 install homeconnect_webthing
 ```
 
-After this installation you may start the webthing http endpoint inside your python code or via command line using
+After this installation, you can use the Webthing http endpoint in your Python code or from the command line with
 ```
 sudo homeconnect --command listen --port 8744 --refresh_token 9yJ4LXJlZyI6IfVVIiwi...2YXRlIn0= --client_secret FEAE...522BD0 
 ```
-Here, the webthing API will be bound to the local port 8744. Furthermore, the refresh_token and client_secret have to be set. 
-Please refer [HomeConnect Authorization](https://api-docs.home-connect.com/quickstart?#authorization) to get your refresh_token and client_secret
+Here the webthing API is bound to the local port 8744. Also, refresh_token and client_secret must be set.
+Please refer to [HomeConnect Authorization](https://api-docs.home-connect.com/quickstart?#authorization) to obtain your refresh_token and client_secret
 
-Alternatively to the *listen* command, you can use the *register* command to register and start the webthing service as systemd unit.
-By doing this the webthing service will be started automatically on boot. Starting the server manually using the *listen* command is no longer necessary.
+As an alternative to the *list* command, you can also use the *register* command to register and start the webthing service as a systemd entity.
+This way, the webthing service is started automatically at boot time. Starting the server manually with the *listen* command is no longer necessary.
 ```
 sudo homeconnect --command register --port 8744 --refresh_token 9yJ4LXJlZyI6IfVVIiwi...2YXRlIn0= --client_secret FEAE...522BD0
 ```
```

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/__init__.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/__init__.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/app.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/app.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/appliances.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/appliances.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/appliances_webthing.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/appliances_webthing.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/auth.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/auth.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/eventstream.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/eventstream.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,19 @@
                 self.stream = EventStream(self.uri, self.auth, self.notify_listener, self.read_timeout_sec, self.max_lifetime_sec)
                 EventStreamWatchDog(self.stream, int(self.max_lifetime_sec * 1.1)).start()
                 self.stream.consume()
                 num_trials = 0
             except Exception as e:
                 logging.warning("error has been occurred for event stream " + self.uri + " " + str(e))
                 if num_trials < 3:
-                    wait_time_sec = 5
+                    wait_time_sec = 10
                 elif num_trials < 5:
-                    wait_time_sec = 30
+                    wait_time_sec = 60
+                elif num_trials < 10:
+                    wait_time_sec = 15*60
                 else:
                     wait_time_sec = 60*60
                 logging.info("try reconnect in " + print_duration(wait_time_sec) + " sec...")
                 sleep(wait_time_sec)
                 logging.info("reconnecting")
```

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing/homeconnect.py` & `homeconnect_webthing-1.0.2/homeconnect_webthing/homeconnect.py`

 * *Files identical despite different names*

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/PKG-INFO` & `homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: homeconnect-webthing
-Version: 1.0.1
+Version: 1.0.2
 Summary: Homeconnect WebThing adapter
 Author: Gregor Roth
 Author-email: gregor.roth@web.de
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # homeconnect_webthing
-A webthing adapter of HomeConnect smart home appliances.
+A webthing adapter for HomeConnect smart home devices.
 
-This project provides a [webthing API](https://iot.mozilla.org/wot/) to access [HomeConnect devices](https://api-docs.home-connect.com/). 
-Currently, the device types ***Dishwasher***, ***Washer*** and ***Dryer*** are supported only 
+This project provides a [webthing API](https://iot.mozilla.org/wot/) for accessing [HomeConnect devices](https://api-docs.home-connect.com/).
+Currently, only the ***dishwasher***, ***washing machine*** and ***dryer*** device types are supported.
 
-The homeconnect_webthing package exposes a http webthing endpoint for each detected and supported smart home appliances. E.g. 
+The homeconnect_webthing package provides an http webthing endpoint for each detected and supported smart home device. E.g.
 ```
 # webthing has been started on host 192.168.0.23
 curl http://192.168.0.23:8744/0/properties 
 
 {
    "device_name":"Geschirrspüler",
    "device_type":"Dishwasher",
@@ -35,26 +35,26 @@
    "program_hygiene_plus":false,
    "program_extra_try":false,
    "program_start_date":"",
    "program_progress":0
 }
 ```
 
-To install this software you may use [PIP](https://realpython.com/what-is-pip/) package manager such as shown below
+To install this software, you can use the [PIP](https://realpython.com/what-is-pip/) package manager as shown below
 
 **PIP approach**
 ```
 sudo pip3 install homeconnect_webthing
 ```
 
-After this installation you may start the webthing http endpoint inside your python code or via command line using
+After this installation, you can use the Webthing http endpoint in your Python code or from the command line with
 ```
 sudo homeconnect --command listen --port 8744 --refresh_token 9yJ4LXJlZyI6IfVVIiwi...2YXRlIn0= --client_secret FEAE...522BD0 
 ```
-Here, the webthing API will be bound to the local port 8744. Furthermore, the refresh_token and client_secret have to be set. 
-Please refer [HomeConnect Authorization](https://api-docs.home-connect.com/quickstart?#authorization) to get your refresh_token and client_secret
+Here the webthing API is bound to the local port 8744. Also, refresh_token and client_secret must be set.
+Please refer to [HomeConnect Authorization](https://api-docs.home-connect.com/quickstart?#authorization) to obtain your refresh_token and client_secret
 
-Alternatively to the *listen* command, you can use the *register* command to register and start the webthing service as systemd unit.
-By doing this the webthing service will be started automatically on boot. Starting the server manually using the *listen* command is no longer necessary.
+As an alternative to the *list* command, you can also use the *register* command to register and start the webthing service as a systemd entity.
+This way, the webthing service is started automatically at boot time. Starting the server manually with the *listen* command is no longer necessary.
 ```
 sudo homeconnect --command register --port 8744 --refresh_token 9yJ4LXJlZyI6IfVVIiwi...2YXRlIn0= --client_secret FEAE...522BD0
 ```
```

### Comparing `homeconnect_webthing-1.0.1/homeconnect_webthing.egg-info/SOURCES.txt` & `homeconnect_webthing-1.0.2/homeconnect_webthing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

