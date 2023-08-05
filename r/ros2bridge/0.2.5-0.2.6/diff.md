# Comparing `tmp/ros2bridge-0.2.5.tar.gz` & `tmp/ros2bridge-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ros2bridge-0.2.5.tar", last modified: Thu Mar 16 05:33:49 2023, max compression
+gzip compressed data, was "ros2bridge-0.2.6.tar", last modified: Sat Aug  5 09:26:00 2023, max compression
```

## Comparing `ros2bridge-0.2.5.tar` & `ros2bridge-0.2.6.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.405141 ros2bridge-0.2.5/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)    35149 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/LICENSE
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      130 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/MANIFEST.in
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     7630 2023-03-16 05:33:49.405141 ros2bridge-0.2.5/PKG-INFO
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     5144 2023-03-10 05:40:44.000000 ros2bridge-0.2.5/README.md
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1255 2023-03-16 05:13:01.000000 ros2bridge-0.2.5/pyproject.toml
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       27 2023-03-16 05:27:03.000000 ros2bridge-0.2.5/requirement.txt
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       93 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/requirements_dev.txt
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      972 2023-03-16 05:33:49.405141 ros2bridge-0.2.5/setup.cfg
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       70 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/setup.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.385141 ros2bridge-0.2.5/src/
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      147 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      834 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/__main__.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/bridge_exceptions/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       48 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/bridge_exceptions/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      362 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/bridge_exceptions/operation_exception.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      434 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/bridge_exceptions/websocket_exception.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/features/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       79 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/features/__init__.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/operations/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       76 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/operations/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4883 2023-03-16 05:24:58.000000 ros2bridge-0.2.5/src/ros2bridge/operations/action_client.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3192 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/operations/publisher.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3107 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/operations/service_client.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3861 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/operations/subscriber.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/protocols/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      109 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/protocols/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      828 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/protocols/operations.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2362 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/protocols/ws_server.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/py.typed
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/qos_profile/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       74 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/qos_profile/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1873 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/qos_profile/profiles.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2201 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/qos_profile/qos_profile.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3112 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/qos_profile/validate_qos.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/ros/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       96 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/ros/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1484 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/ros/bridge_node.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2543 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/ros2bridge.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/server/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      175 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/server/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2001 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/server/register_client.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2349 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/server/route_message.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4586 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/server/ws_server.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge/utils/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      104 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/utils/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     6586 2023-03-16 05:25:50.000000 ros2bridge-0.2.5/src/ros2bridge/utils/data_parser.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1441 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/src/ros2bridge/utils/settings.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/src/ros2bridge.egg-info/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     7630 2023-03-16 05:33:49.000000 ros2bridge-0.2.5/src/ros2bridge.egg-info/PKG-INFO
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1993 2023-03-16 05:33:49.000000 ros2bridge-0.2.5/src/ros2bridge.egg-info/SOURCES.txt
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)        1 2023-03-16 05:33:49.000000 ros2bridge-0.2.5/src/ros2bridge.egg-info/dependency_links.txt
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      123 2023-03-16 05:33:49.000000 ros2bridge-0.2.5/src/ros2bridge.egg-info/requires.txt
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       11 2023-03-16 05:33:49.000000 ros2bridge-0.2.5/src/ros2bridge.egg-info/top_level.txt
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/tests/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       37 2023-03-11 04:35:35.000000 ros2bridge-0.2.5/tests/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1427 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/conftest.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/tests/test_action_client/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3531 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_action_client/test_navigate.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2694 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_action_client/test_path_pose_navmsg.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4165 2023-03-16 05:08:39.000000 ros2bridge-0.2.5/tests/test_action_client/ttest_follow_waypoints.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/tests/test_publisher/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2817 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_publisher/test_twist_msg.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/tests/test_srv_client/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      653 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_srv_client/test_amcl_srv.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2249 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_srv_client/test_map_srv.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/tests/test_subscriber/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3143 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_subscriber/test_string_msg.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1620 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_subscriber/test_turtlebot_amcl.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.395141 ros2bridge-0.2.5/tests/test_websocket/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      467 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/test_websocket/test_connection.py
-drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-03-16 05:33:49.405141 ros2bridge-0.2.5/tests/utils/
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       31 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/utils/__init__.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4392 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/utils/action_client_helper.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      158 2023-03-11 03:47:44.000000 ros2bridge-0.2.5/tests/utils/config.json
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      853 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/utils/pre_post.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3171 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/utils/service_client_helper.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2774 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tests/utils/subscriber_helper.py
--rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      418 2023-03-10 05:30:55.000000 ros2bridge-0.2.5/tox.ini
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)    35149 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/LICENSE
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      130 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/MANIFEST.in
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     7733 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/PKG-INFO
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     5239 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/README.md
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1255 2023-08-05 09:16:51.000000 ros2bridge-0.2.6/pyproject.toml
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       14 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/requirement.txt
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      106 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/requirements_dev.txt
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      972 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/setup.cfg
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       70 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/setup.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.882581 ros2bridge-0.2.6/src/
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      147 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      834 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/__main__.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/bridge_exceptions/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       48 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/bridge_exceptions/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      362 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/bridge_exceptions/operation_exception.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      434 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/bridge_exceptions/websocket_exception.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/features/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       79 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/features/__init__.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/operations/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       76 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/operations/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4883 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/operations/action_client.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3192 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/operations/publisher.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3107 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/operations/service_client.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3861 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/operations/subscriber.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/protocols/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      109 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/protocols/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      828 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/protocols/operations.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2362 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/protocols/ws_server.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/py.typed
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/qos_profile/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       74 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/qos_profile/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1873 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/qos_profile/profiles.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2201 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/qos_profile/qos_profile.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3112 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/qos_profile/validate_qos.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/ros/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       96 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/ros/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1484 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/ros/bridge_node.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2543 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/ros2bridge.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/server/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      175 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/server/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2001 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/server/register_client.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2349 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/server/route_message.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4586 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/server/ws_server.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge/utils/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      104 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/utils/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     6586 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/utils/data_parser.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1441 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/src/ros2bridge/utils/settings.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/src/ros2bridge.egg-info/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     7733 2023-08-05 09:26:00.000000 ros2bridge-0.2.6/src/ros2bridge.egg-info/PKG-INFO
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1993 2023-08-05 09:26:00.000000 ros2bridge-0.2.6/src/ros2bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)        1 2023-08-05 09:26:00.000000 ros2bridge-0.2.6/src/ros2bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      123 2023-08-05 09:26:00.000000 ros2bridge-0.2.6/src/ros2bridge.egg-info/requires.txt
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       11 2023-08-05 09:26:00.000000 ros2bridge-0.2.6/src/ros2bridge.egg-info/top_level.txt
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       37 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1427 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/conftest.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/test_action_client/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3531 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_action_client/test_navigate.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2694 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_action_client/test_path_pose_navmsg.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4165 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_action_client/ttest_follow_waypoints.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/test_publisher/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2817 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_publisher/test_twist_msg.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/test_srv_client/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      653 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_srv_client/test_amcl_srv.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2249 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_srv_client/test_map_srv.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/test_subscriber/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3143 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_subscriber/test_string_msg.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     1620 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_subscriber/test_turtlebot_amcl.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/test_websocket/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      467 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/test_websocket/test_connection.py
+drwxr-xr-x   0 bonnybk   (1000) bonnybk   (1000)        0 2023-08-05 09:26:00.893414 ros2bridge-0.2.6/tests/utils/
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)       31 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/utils/__init__.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     4392 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/utils/action_client_helper.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      158 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/utils/config.json
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      853 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/utils/pre_post.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     3171 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/utils/service_client_helper.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)     2774 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tests/utils/subscriber_helper.py
+-rw-r--r--   0 bonnybk   (1000) bonnybk   (1000)      418 2023-08-05 09:16:11.000000 ros2bridge-0.2.6/tox.ini
```

### Comparing `ros2bridge-0.2.5/LICENSE` & `ros2bridge-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/PKG-INFO` & `ros2bridge-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ros2bridge
-Version: 0.2.5
+Version: 0.2.6
 Summary: A bridge between websocket and DDS of ROS 2
 Home-page: https://github.com/bonnybabukachappilly/ros2bridge
 Author: Bonny Babu
 Author-email: bonnybabukachappilly@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Description: # ROS WEBSOCKET BRIDGE
         
         ![version](https://img.shields.io/badge/Version-ROS%202%20FOXY-informational)
         ![license](https://img.shields.io/badge/license-GNU%20v3.0-blue)
         
         ## Overview
         
-        This is a package for converting ROS 2 DDS to websocket. This project was inspired by [rosbridge_suite](https://github.com/RobotWebTools/rosbridge_suite) by [Robo Web Tools](https://github.com/RobotWebTools). The implemented features are not for specific topics or services but all available ros interfaces. It's in early development, and not all interfaces are tested. Any bug reported will be fixed in upcoming releases.
+        This is a package for converting ROS 2 DDS to WebSocket. This project was inspired by [rosbridge_suite](https://github.com/RobotWebTools/rosbridge_suite) by [Robo Web Tools](https://github.com/RobotWebTools). The implemented features are not for specific topics or services but all available ros interfaces. It's in early development, and not all interfaces are tested. Any bug reported will be fixed in upcoming releases.
         
-        When using the suite, I faced issues with ROS 2 and couldn't find a way to move forward. So I decided to create another which is not advanced as the suite but gets my job done. I decided to package it and publish it on PyPI for easy availability to others and learning purposes. The code I use is different, and the features are not the same. The client libraries for the suite won't work because this is not a suite clone.
+        When using the suite, I faced issues with ROS 2 and couldn't find a way to move forward. So I decided to create another which is not advanced as the suite but gets my job done. I decided to package it and publish it on PyPI for easy availability to others and for learning purposes. The code I use is different, and the features are not the same. The client libraries for the suite won't work because this is not a suite clone.
         
         **Note: This project is not a suite clone. The architecture and implementation are different. Not all the features of the suite are not available in this project.**
         
         ## Requirements
         
         ----
         
@@ -42,28 +42,29 @@
         ```bash
         python3 -m ros2bridge
         
         ```
         
         **optional parameters:**
         
-        * -p, --port : For specific port. Default is 9020
-        * -n, --ngrok : By default, websocket is hosted on local-IP. If this flag is set ws is hosted internally
+        * -p, --port: For specific port. Default is 9020
+        * -n, --ngrok: WebSocket is hosted on local IP by default. If this flag is set ws are hosted internally
         
         **NOTE: for using custom ros interface source that workspace before running the bridge.**
         
         ## Available ROS Interfaces
         
         ----
         
         * Publisher
-        
-        **TODO :**
-        
         * Subscriber
+        * Service Client
+        * Action Client
+        
+        **TODO:**
         * Service Server
         * Action Server
         
         ## Request structure
         
         ----
         
@@ -75,45 +76,45 @@
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
             "message": "<message>"
         }
         ```
         
         * type eg: 'std_msgs/String'
-        * message eg: {"data" : "HELLO WORLD !"}
-        * NOTE: message should be in the format of message type
+        * message eg: {"data": "HELLO WORLD !"}
+        * NOTE: the message should be in the format of the message type
         
         ### Subscriber
         
         ```json
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
         }
         ```
         
         * type eg: 'std_msgs/String'
         
-        NOTE: Subscribed message will return in this format.
+        NOTE: Subscribed messages will return in this format.
         
         ```json
         
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
             "message": "<message>"
         }
         ```
         
         * type eg: 'std_msgs/String'
-        * message eg: {"data" : "HELLO WORLD !"}
+        * message eg: {"data": "HELLO WORLD !"}
         
-        NOTE: To unsubscribe from a topic send following message to server
+        NOTE: To unsubscribe from a topic send the following message to the server
         
         ```json
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
             "unsubscribe": true
@@ -144,103 +145,103 @@
             "srv_name": "/<service_name>",
             "srv_type": "<service_parent>/<service_type>",
             "message": "<message>"
         
         }
         ```
         
-        * NOTE: message should be in the format of service type
+        * NOTE: the message should be in the format of the service type
         
         ### ACTION CLIENT
         
-        For creating a action client
+        For creating an action client
         
         ```json
         {
             "operation": "action_client",
             "action": "create",
             "action_name": "/<action_name>",
             "action_type": "<action_parent>/<action_type>"
         }
         ```
         
-        For calling a action client
+        For calling an action client
         
         ```json
         {
             "operation": "action_client",
             "action": "call",
             "action_name": "/<action_name>",
             "action_type": "<action_parent>/<action_type>",
             "message": "<message>"
         }
         ```
         
-        * NOTE: message should be in the format of action type
+        * NOTE: the message should be in the format of action type
         
-        Feedback from calling a action client
+        Feedback from calling an action client
         
         ```json
         {
             "operation": "action_client",
             "action": "call",
             "action_response": "<action_response>",
             "action_name": "/<action_name>",
             "action_type": "<action_parent>/<action_type>",
             "message": "<message>"
         
         }
         ```
         
-        * NOTE: message should be in the format of action type.
-        * NOTE: action_response will be any of 'response', 'feedback', 'result'.
+        * NOTE: the message should be in the format of action type.
+        * NOTE: action_response will be any of 'response', 'feedback', or 'result'.
         
         ### QOS PROFILE
         
-        Added QoS profile to subscription.
-        No validation of QoS is added and no error is send back to client.
+        I added a QoS profile to the subscription.
+        No validation of QoS is added and no error is sent back to the client.
         
-        Available QoS settings for subscriber:
+        Available QoS settings for subscribers:
         
         * QoSReliabilityPolicy
         * QoSDurabilityPolicy
         * QoSHistoryPolicy
         
-        For creating a Qos Profile add following in addition to above request syntax
+        For creating a Qos Profile add the following in addition to the above request syntax
         
         ```json
-        "qos" : {
+        "qos": {
             "durability": "<durability>",
             "reliability": "<reliability>",
             "history": "<history>",
         }
         ```
         
-        For options to provide please refer [this docs]('https://docs.ros.org/en/rolling/Concepts/About-Quality-of-Service-Settings.html)
+        For options to provide please refer [to this docs]('https://docs.ros.org/en/rolling/Concepts/About-Quality-of-Service-Settings.html)
         
-        General request will be look like
+        A general request will look like
         
         ```json
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
-            "qos" : {
+            "qos": {
                 "durability": "<durability>",
                 "reliability": "<reliability>",
                 "history": "<history>",
             }
         }
         ```
         
         ## Testing
         
         ----
         
-        For testing using tox, ROS package is required and I haven't find a way to get around it. So testing withing the system.
+        For testing using tox, the ROS package is required and I haven't found a way to get around it. So testing within the system.
         
         * MYPY
         * FLAKE8
         * PYTEST
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ros2bridge-0.2.5/README.md` & `ros2bridge-0.2.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # ROS WEBSOCKET BRIDGE
 
 ![version](https://img.shields.io/badge/Version-ROS%202%20FOXY-informational)
 ![license](https://img.shields.io/badge/license-GNU%20v3.0-blue)
 
 ## Overview
 
-This is a package for converting ROS 2 DDS to websocket. This project was inspired by [rosbridge_suite](https://github.com/RobotWebTools/rosbridge_suite) by [Robo Web Tools](https://github.com/RobotWebTools). The implemented features are not for specific topics or services but all available ros interfaces. It's in early development, and not all interfaces are tested. Any bug reported will be fixed in upcoming releases.
+This is a package for converting ROS 2 DDS to WebSocket. This project was inspired by [rosbridge_suite](https://github.com/RobotWebTools/rosbridge_suite) by [Robo Web Tools](https://github.com/RobotWebTools). The implemented features are not for specific topics or services but all available ros interfaces. It's in early development, and not all interfaces are tested. Any bug reported will be fixed in upcoming releases.
 
-When using the suite, I faced issues with ROS 2 and couldn't find a way to move forward. So I decided to create another which is not advanced as the suite but gets my job done. I decided to package it and publish it on PyPI for easy availability to others and learning purposes. The code I use is different, and the features are not the same. The client libraries for the suite won't work because this is not a suite clone.
+When using the suite, I faced issues with ROS 2 and couldn't find a way to move forward. So I decided to create another which is not advanced as the suite but gets my job done. I decided to package it and publish it on PyPI for easy availability to others and for learning purposes. The code I use is different, and the features are not the same. The client libraries for the suite won't work because this is not a suite clone.
 
 **Note: This project is not a suite clone. The architecture and implementation are different. Not all the features of the suite are not available in this project.**
 
 ## Requirements
 
 ----
 
@@ -34,28 +34,29 @@
 ```bash
 python3 -m ros2bridge
 
 ```
 
 **optional parameters:**
 
-* -p, --port : For specific port. Default is 9020
-* -n, --ngrok : By default, websocket is hosted on local-IP. If this flag is set ws is hosted internally
+* -p, --port: For specific port. Default is 9020
+* -n, --ngrok: WebSocket is hosted on local IP by default. If this flag is set ws are hosted internally
 
 **NOTE: for using custom ros interface source that workspace before running the bridge.**
 
 ## Available ROS Interfaces
 
 ----
 
 * Publisher
-
-**TODO :**
-
 * Subscriber
+* Service Client
+* Action Client
+
+**TODO:**
 * Service Server
 * Action Server
 
 ## Request structure
 
 ----
 
@@ -67,45 +68,45 @@
     "topic": "/<topic_name>",
     "type": "<message_parent>/<message_type>",
     "message": "<message>"
 }
 ```
 
 * type eg: 'std_msgs/String'
-* message eg: {"data" : "HELLO WORLD !"}
-* NOTE: message should be in the format of message type
+* message eg: {"data": "HELLO WORLD !"}
+* NOTE: the message should be in the format of the message type
 
 ### Subscriber
 
 ```json
 {
     "operation": "subscribe",
     "topic": "/<topic_name>",
     "type": "<message_parent>/<message_type>",
 }
 ```
 
 * type eg: 'std_msgs/String'
 
-NOTE: Subscribed message will return in this format.
+NOTE: Subscribed messages will return in this format.
 
 ```json
 
 {
     "operation": "subscribe",
     "topic": "/<topic_name>",
     "type": "<message_parent>/<message_type>",
     "message": "<message>"
 }
 ```
 
 * type eg: 'std_msgs/String'
-* message eg: {"data" : "HELLO WORLD !"}
+* message eg: {"data": "HELLO WORLD !"}
 
-NOTE: To unsubscribe from a topic send following message to server
+NOTE: To unsubscribe from a topic send the following message to the server
 
 ```json
 {
     "operation": "subscribe",
     "topic": "/<topic_name>",
     "type": "<message_parent>/<message_type>",
     "unsubscribe": true
@@ -136,100 +137,100 @@
     "srv_name": "/<service_name>",
     "srv_type": "<service_parent>/<service_type>",
     "message": "<message>"
 
 }
 ```
 
-* NOTE: message should be in the format of service type
+* NOTE: the message should be in the format of the service type
 
 ### ACTION CLIENT
 
-For creating a action client
+For creating an action client
 
 ```json
 {
     "operation": "action_client",
     "action": "create",
     "action_name": "/<action_name>",
     "action_type": "<action_parent>/<action_type>"
 }
 ```
 
-For calling a action client
+For calling an action client
 
 ```json
 {
     "operation": "action_client",
     "action": "call",
     "action_name": "/<action_name>",
     "action_type": "<action_parent>/<action_type>",
     "message": "<message>"
 }
 ```
 
-* NOTE: message should be in the format of action type
+* NOTE: the message should be in the format of action type
 
-Feedback from calling a action client
+Feedback from calling an action client
 
 ```json
 {
     "operation": "action_client",
     "action": "call",
     "action_response": "<action_response>",
     "action_name": "/<action_name>",
     "action_type": "<action_parent>/<action_type>",
     "message": "<message>"
 
 }
 ```
 
-* NOTE: message should be in the format of action type.
-* NOTE: action_response will be any of 'response', 'feedback', 'result'.
+* NOTE: the message should be in the format of action type.
+* NOTE: action_response will be any of 'response', 'feedback', or 'result'.
 
 ### QOS PROFILE
 
-Added QoS profile to subscription.
-No validation of QoS is added and no error is send back to client.
+I added a QoS profile to the subscription.
+No validation of QoS is added and no error is sent back to the client.
 
-Available QoS settings for subscriber:
+Available QoS settings for subscribers:
 
 * QoSReliabilityPolicy
 * QoSDurabilityPolicy
 * QoSHistoryPolicy
 
-For creating a Qos Profile add following in addition to above request syntax
+For creating a Qos Profile add the following in addition to the above request syntax
 
 ```json
-"qos" : {
+"qos": {
     "durability": "<durability>",
     "reliability": "<reliability>",
     "history": "<history>",
 }
 ```
 
-For options to provide please refer [this docs]('https://docs.ros.org/en/rolling/Concepts/About-Quality-of-Service-Settings.html)
+For options to provide please refer [to this docs]('https://docs.ros.org/en/rolling/Concepts/About-Quality-of-Service-Settings.html)
 
-General request will be look like
+A general request will look like
 
 ```json
 {
     "operation": "subscribe",
     "topic": "/<topic_name>",
     "type": "<message_parent>/<message_type>",
-    "qos" : {
+    "qos": {
         "durability": "<durability>",
         "reliability": "<reliability>",
         "history": "<history>",
     }
 }
 ```
 
 ## Testing
 
 ----
 
-For testing using tox, ROS package is required and I haven't find a way to get around it. So testing withing the system.
+For testing using tox, the ROS package is required and I haven't found a way to get around it. So testing within the system.
 
 * MYPY
 * FLAKE8
 * PYTEST
```

### Comparing `ros2bridge-0.2.5/pyproject.toml` & `ros2bridge-0.2.6/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "ros2bridge"
-version = "0.2.5"
+version = "0.2.6"
 description = "A bridge between websocket and DDS of ROS 2"
 readme = "README.md"
 authors = [{ name = "Bonny Babu", email = "bonnybabukachappilly@gmail.com" }]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
```

### Comparing `ros2bridge-0.2.5/setup.cfg` & `ros2bridge-0.2.6/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = ros2bridge
 author = Bonny Babu
 author_email = bonnybabukachappilly@gmail.com
 description = A bridge between websocket and DDS of ROS 2
 long_description = file: README.md
-version = 0.2.5
+version = 0.2.6
 long_description_content_type = text/markdown
 license = GNU GENERAL PUBLIC LICENSE Version 3
 license_file = LICENSE
 url = https://github.com/bonnybabukachappilly/ros2bridge
 classifiers = 
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
```

### Comparing `ros2bridge-0.2.5/src/ros2bridge/__main__.py` & `ros2bridge-0.2.6/src/ros2bridge/__main__.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/operations/action_client.py` & `ros2bridge-0.2.6/src/ros2bridge/operations/action_client.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/operations/publisher.py` & `ros2bridge-0.2.6/src/ros2bridge/operations/publisher.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/operations/service_client.py` & `ros2bridge-0.2.6/src/ros2bridge/operations/service_client.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/operations/subscriber.py` & `ros2bridge-0.2.6/src/ros2bridge/operations/subscriber.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/protocols/operations.py` & `ros2bridge-0.2.6/src/ros2bridge/protocols/operations.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/protocols/ws_server.py` & `ros2bridge-0.2.6/src/ros2bridge/protocols/ws_server.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/qos_profile/profiles.py` & `ros2bridge-0.2.6/src/ros2bridge/qos_profile/profiles.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/qos_profile/qos_profile.py` & `ros2bridge-0.2.6/src/ros2bridge/qos_profile/qos_profile.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/qos_profile/validate_qos.py` & `ros2bridge-0.2.6/src/ros2bridge/qos_profile/validate_qos.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/ros/bridge_node.py` & `ros2bridge-0.2.6/src/ros2bridge/ros/bridge_node.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/ros2bridge.py` & `ros2bridge-0.2.6/src/ros2bridge/ros2bridge.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/server/register_client.py` & `ros2bridge-0.2.6/src/ros2bridge/server/register_client.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/server/route_message.py` & `ros2bridge-0.2.6/src/ros2bridge/server/route_message.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/server/ws_server.py` & `ros2bridge-0.2.6/src/ros2bridge/server/ws_server.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/utils/data_parser.py` & `ros2bridge-0.2.6/src/ros2bridge/utils/data_parser.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge/utils/settings.py` & `ros2bridge-0.2.6/src/ros2bridge/utils/settings.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/src/ros2bridge.egg-info/PKG-INFO` & `ros2bridge-0.2.6/src/ros2bridge.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ros2bridge
-Version: 0.2.5
+Version: 0.2.6
 Summary: A bridge between websocket and DDS of ROS 2
 Home-page: https://github.com/bonnybabukachappilly/ros2bridge
 Author: Bonny Babu
 Author-email: bonnybabukachappilly@gmail.com
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Description: # ROS WEBSOCKET BRIDGE
         
         ![version](https://img.shields.io/badge/Version-ROS%202%20FOXY-informational)
         ![license](https://img.shields.io/badge/license-GNU%20v3.0-blue)
         
         ## Overview
         
-        This is a package for converting ROS 2 DDS to websocket. This project was inspired by [rosbridge_suite](https://github.com/RobotWebTools/rosbridge_suite) by [Robo Web Tools](https://github.com/RobotWebTools). The implemented features are not for specific topics or services but all available ros interfaces. It's in early development, and not all interfaces are tested. Any bug reported will be fixed in upcoming releases.
+        This is a package for converting ROS 2 DDS to WebSocket. This project was inspired by [rosbridge_suite](https://github.com/RobotWebTools/rosbridge_suite) by [Robo Web Tools](https://github.com/RobotWebTools). The implemented features are not for specific topics or services but all available ros interfaces. It's in early development, and not all interfaces are tested. Any bug reported will be fixed in upcoming releases.
         
-        When using the suite, I faced issues with ROS 2 and couldn't find a way to move forward. So I decided to create another which is not advanced as the suite but gets my job done. I decided to package it and publish it on PyPI for easy availability to others and learning purposes. The code I use is different, and the features are not the same. The client libraries for the suite won't work because this is not a suite clone.
+        When using the suite, I faced issues with ROS 2 and couldn't find a way to move forward. So I decided to create another which is not advanced as the suite but gets my job done. I decided to package it and publish it on PyPI for easy availability to others and for learning purposes. The code I use is different, and the features are not the same. The client libraries for the suite won't work because this is not a suite clone.
         
         **Note: This project is not a suite clone. The architecture and implementation are different. Not all the features of the suite are not available in this project.**
         
         ## Requirements
         
         ----
         
@@ -42,28 +42,29 @@
         ```bash
         python3 -m ros2bridge
         
         ```
         
         **optional parameters:**
         
-        * -p, --port : For specific port. Default is 9020
-        * -n, --ngrok : By default, websocket is hosted on local-IP. If this flag is set ws is hosted internally
+        * -p, --port: For specific port. Default is 9020
+        * -n, --ngrok: WebSocket is hosted on local IP by default. If this flag is set ws are hosted internally
         
         **NOTE: for using custom ros interface source that workspace before running the bridge.**
         
         ## Available ROS Interfaces
         
         ----
         
         * Publisher
-        
-        **TODO :**
-        
         * Subscriber
+        * Service Client
+        * Action Client
+        
+        **TODO:**
         * Service Server
         * Action Server
         
         ## Request structure
         
         ----
         
@@ -75,45 +76,45 @@
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
             "message": "<message>"
         }
         ```
         
         * type eg: 'std_msgs/String'
-        * message eg: {"data" : "HELLO WORLD !"}
-        * NOTE: message should be in the format of message type
+        * message eg: {"data": "HELLO WORLD !"}
+        * NOTE: the message should be in the format of the message type
         
         ### Subscriber
         
         ```json
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
         }
         ```
         
         * type eg: 'std_msgs/String'
         
-        NOTE: Subscribed message will return in this format.
+        NOTE: Subscribed messages will return in this format.
         
         ```json
         
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
             "message": "<message>"
         }
         ```
         
         * type eg: 'std_msgs/String'
-        * message eg: {"data" : "HELLO WORLD !"}
+        * message eg: {"data": "HELLO WORLD !"}
         
-        NOTE: To unsubscribe from a topic send following message to server
+        NOTE: To unsubscribe from a topic send the following message to the server
         
         ```json
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
             "unsubscribe": true
@@ -144,103 +145,103 @@
             "srv_name": "/<service_name>",
             "srv_type": "<service_parent>/<service_type>",
             "message": "<message>"
         
         }
         ```
         
-        * NOTE: message should be in the format of service type
+        * NOTE: the message should be in the format of the service type
         
         ### ACTION CLIENT
         
-        For creating a action client
+        For creating an action client
         
         ```json
         {
             "operation": "action_client",
             "action": "create",
             "action_name": "/<action_name>",
             "action_type": "<action_parent>/<action_type>"
         }
         ```
         
-        For calling a action client
+        For calling an action client
         
         ```json
         {
             "operation": "action_client",
             "action": "call",
             "action_name": "/<action_name>",
             "action_type": "<action_parent>/<action_type>",
             "message": "<message>"
         }
         ```
         
-        * NOTE: message should be in the format of action type
+        * NOTE: the message should be in the format of action type
         
-        Feedback from calling a action client
+        Feedback from calling an action client
         
         ```json
         {
             "operation": "action_client",
             "action": "call",
             "action_response": "<action_response>",
             "action_name": "/<action_name>",
             "action_type": "<action_parent>/<action_type>",
             "message": "<message>"
         
         }
         ```
         
-        * NOTE: message should be in the format of action type.
-        * NOTE: action_response will be any of 'response', 'feedback', 'result'.
+        * NOTE: the message should be in the format of action type.
+        * NOTE: action_response will be any of 'response', 'feedback', or 'result'.
         
         ### QOS PROFILE
         
-        Added QoS profile to subscription.
-        No validation of QoS is added and no error is send back to client.
+        I added a QoS profile to the subscription.
+        No validation of QoS is added and no error is sent back to the client.
         
-        Available QoS settings for subscriber:
+        Available QoS settings for subscribers:
         
         * QoSReliabilityPolicy
         * QoSDurabilityPolicy
         * QoSHistoryPolicy
         
-        For creating a Qos Profile add following in addition to above request syntax
+        For creating a Qos Profile add the following in addition to the above request syntax
         
         ```json
-        "qos" : {
+        "qos": {
             "durability": "<durability>",
             "reliability": "<reliability>",
             "history": "<history>",
         }
         ```
         
-        For options to provide please refer [this docs]('https://docs.ros.org/en/rolling/Concepts/About-Quality-of-Service-Settings.html)
+        For options to provide please refer [to this docs]('https://docs.ros.org/en/rolling/Concepts/About-Quality-of-Service-Settings.html)
         
-        General request will be look like
+        A general request will look like
         
         ```json
         {
             "operation": "subscribe",
             "topic": "/<topic_name>",
             "type": "<message_parent>/<message_type>",
-            "qos" : {
+            "qos": {
                 "durability": "<durability>",
                 "reliability": "<reliability>",
                 "history": "<history>",
             }
         }
         ```
         
         ## Testing
         
         ----
         
-        For testing using tox, ROS package is required and I haven't find a way to get around it. So testing withing the system.
+        For testing using tox, the ROS package is required and I haven't found a way to get around it. So testing within the system.
         
         * MYPY
         * FLAKE8
         * PYTEST
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ros2bridge-0.2.5/src/ros2bridge.egg-info/SOURCES.txt` & `ros2bridge-0.2.6/src/ros2bridge.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/conftest.py` & `ros2bridge-0.2.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_action_client/test_navigate.py` & `ros2bridge-0.2.6/tests/test_action_client/test_navigate.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_action_client/test_path_pose_navmsg.py` & `ros2bridge-0.2.6/tests/test_action_client/test_path_pose_navmsg.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_action_client/ttest_follow_waypoints.py` & `ros2bridge-0.2.6/tests/test_action_client/ttest_follow_waypoints.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_publisher/test_twist_msg.py` & `ros2bridge-0.2.6/tests/test_publisher/test_twist_msg.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_srv_client/test_amcl_srv.py` & `ros2bridge-0.2.6/tests/test_srv_client/test_amcl_srv.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_srv_client/test_map_srv.py` & `ros2bridge-0.2.6/tests/test_srv_client/test_map_srv.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_subscriber/test_string_msg.py` & `ros2bridge-0.2.6/tests/test_subscriber/test_string_msg.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/test_subscriber/test_turtlebot_amcl.py` & `ros2bridge-0.2.6/tests/test_subscriber/test_turtlebot_amcl.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/utils/action_client_helper.py` & `ros2bridge-0.2.6/tests/utils/action_client_helper.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/utils/pre_post.py` & `ros2bridge-0.2.6/tests/utils/pre_post.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/utils/service_client_helper.py` & `ros2bridge-0.2.6/tests/utils/service_client_helper.py`

 * *Files identical despite different names*

### Comparing `ros2bridge-0.2.5/tests/utils/subscriber_helper.py` & `ros2bridge-0.2.6/tests/utils/subscriber_helper.py`

 * *Files identical despite different names*

