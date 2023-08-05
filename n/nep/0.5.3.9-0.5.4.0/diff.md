# Comparing `tmp/nep-0.5.3.9.tar.gz` & `tmp/nep-0.5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\nep-0.5.3.9.tar", last modified: Thu May 13 10:23:39 2021, max compression
+gzip compressed data, was "dist\nep-0.5.4.0.tar", last modified: Sat Aug  5 01:08:27 2023, max compression
```

## Comparing `nep-0.5.3.9.tar` & `nep-0.5.4.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2021-05-13 10:23:39.000000 nep-0.5.3.9/
--rw-rw-rw-   0        0        0     1086 2020-01-04 15:03:06.000000 nep-0.5.3.9/LICENSE
-drwxrwxrwx   0        0        0        0 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep/
--rw-rw-rw-   0        0        0     2034 2020-01-04 15:03:06.000000 nep-0.5.3.9/nep/broker.py
--rw-rw-rw-   0        0        0     6518 2020-06-27 13:35:30.000000 nep-0.5.3.9/nep/client.py
--rw-rw-rw-   0        0        0    10589 2020-06-27 13:35:50.000000 nep-0.5.3.9/nep/helpers.py
--rw-rw-rw-   0        0        0    13468 2021-05-13 10:22:36.000000 nep-0.5.3.9/nep/master.py
--rw-rw-rw-   0        0        0    19342 2020-02-27 09:36:34.000000 nep-0.5.3.9/nep/node.py
--rw-rw-rw-   0        0        0    15281 2020-08-23 15:44:30.000000 nep-0.5.3.9/nep/publisher.py
--rw-rw-rw-   0        0        0     5743 2020-01-04 15:03:06.000000 nep-0.5.3.9/nep/respondent.py
--rw-rw-rw-   0        0        0     8152 2020-01-04 15:03:06.000000 nep-0.5.3.9/nep/server.py
--rw-rw-rw-   0        0        0    18674 2020-09-01 07:28:21.000000 nep-0.5.3.9/nep/subscriber.py
--rw-rw-rw-   0        0        0     5925 2020-01-04 15:03:06.000000 nep-0.5.3.9/nep/surveyor.py
--rw-rw-rw-   0        0        0      305 2020-01-04 15:03:06.000000 nep-0.5.3.9/nep/__init__.py
-drwxrwxrwx   0        0        0        0 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep.egg-info/
--rw-rw-rw-   0        0        0        1 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      771 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       17 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep.egg-info/requires.txt
--rw-rw-rw-   0        0        0      328 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        4 2021-05-13 10:23:39.000000 nep-0.5.3.9/nep.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      771 2021-05-13 10:23:39.000000 nep-0.5.3.9/PKG-INFO
--rw-rw-rw-   0        0        0      213 2020-01-05 05:14:19.000000 nep-0.5.3.9/README.md
--rw-rw-rw-   0        0        0       42 2021-05-13 10:23:39.000000 nep-0.5.3.9/setup.cfg
--rw-rw-rw-   0        0        0      889 2021-05-13 10:23:05.000000 nep-0.5.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:08:27.000000 nep-0.5.4.0/
+-rw-rw-rw-   0        0        0     1086 2022-11-10 00:27:47.000000 nep-0.5.4.0/LICENSE
+-rw-rw-rw-   0        0        0     1764 2023-08-05 01:08:27.000000 nep-0.5.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1001 2023-08-05 01:08:20.000000 nep-0.5.4.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep/
+-rw-rw-rw-   0        0        0      305 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/__init__.py
+-rw-rw-rw-   0        0        0     2034 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/broker.py
+-rw-rw-rw-   0        0        0     6518 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/client.py
+-rw-rw-rw-   0        0        0    10589 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/helpers.py
+-rw-rw-rw-   0        0        0    13466 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/master.py
+-rw-rw-rw-   0        0        0    19342 2023-08-05 00:08:59.000000 nep-0.5.4.0/nep/node.py
+-rw-rw-rw-   0        0        0    15555 2023-08-05 00:46:34.000000 nep-0.5.4.0/nep/publisher.py
+-rw-rw-rw-   0        0        0     5743 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/respondent.py
+-rw-rw-rw-   0        0        0     8152 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/server.py
+-rw-rw-rw-   0        0        0    20981 2023-08-05 00:51:46.000000 nep-0.5.4.0/nep/subscriber.py
+-rw-rw-rw-   0        0        0     5925 2022-11-10 00:27:47.000000 nep-0.5.4.0/nep/surveyor.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep.egg-info/
+-rw-rw-rw-   0        0        0     1764 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      329 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-05 01:08:27.000000 nep-0.5.4.0/nep.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 01:08:27.000000 nep-0.5.4.0/setup.cfg
+-rw-rw-rw-   0        0        0     1029 2023-08-05 01:05:58.000000 nep-0.5.4.0/setup.py
```

### Comparing `nep-0.5.3.9/LICENSE` & `nep-0.5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/nep/broker.py` & `nep-0.5.4.0/nep/broker.py`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/nep/client.py` & `nep-0.5.4.0/nep/client.py`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/nep/helpers.py` & `nep-0.5.4.0/nep/helpers.py`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/nep/master.py` & `nep-0.5.4.0/nep/master.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
             msg = {'topic':topic, 'port': self.current_port,  'ip': self.IP, 'socket':node_request["socket"],"state":"success"}
             pass
 
         if "language" in node_request:
             if node_request["language"] == "C++":
                 cmsg = msg.copy()
                 cmsg["port"] = str(cmsg["port"] )
-                self.server.send_info(cmsg)
+                self.server.send_info(msg)
         
         else:
             self.server.send_info(msg)
 
         self.topic_register[topic]["nodes"] = {node_request['node']:{'socket':node_request["socket"], 'pid':"n.a.",'ip': self.IP}}
         
         if "pid" in node_request:
@@ -198,15 +198,15 @@
             else:
                 msg = {'topic':topic, 'port': port, 'ip': self.IP, 'socket':socket_, "state":"success"}
 
             if "language" in node_request:
                 if node_request["language"] == "C++":
                     cmsg = msg.copy()
                     cmsg["port"] = str(cmsg["port"] )
-                    self.server.send_info(cmsg)
+                    self.server.send_info(msg)
         
             else:
                 self.server.send_info(msg)
 
             if "pid" in node_request:
                 self.topic_register[topic]["nodes"][node_request['node']] = {'socket':node_request["socket"], 'pid':node_request["pid"], 'ip': self.IP}
             else:
```

### Comparing `nep-0.5.3.9/nep/node.py` & `nep-0.5.4.0/nep/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import sys
 import signal
 import threading
 import simplejson
 import nep
 import zmq
 import atexit
-from zmq.eventloop import ioloop, zmqstream
+from zmq.eventloop.ioloop import IOLoop
 
 
 
 #TODO: bug sending strings there is a space + message in publish-subscriber with ZMQ
 #TODO: unregister topic when closed
 
 
@@ -436,26 +436,25 @@
             msg = {}
             success = False
         return success, msg
 
 
     def spin(self):
         """ Start event loop"""
-        if self.transport  == 'ZMQ':
-            # Event Loop calback option
-            if self.sub_callback != None:
-                stream_sub = zmqstream.ZMQStream(self.sub_socket)
-                stream_sub.on_recv(self.__process_message)
-                ioloop.IOLoop.instance().start()
-        elif self.transport  == 'ROS':
+        if self.transport == 'ZMQ':
+            # Event Loop callback option
+            if self.sub_callback is not None:
+                zmqstream = zmq.eventloop.zmqstream.ZMQStream(self.sub_socket)
+                zmqstream.on_recv(self.__process_message)
+                IOLoop.instance().start()
+        elif self.transport == 'ROS':
             import rospy
             """Function used to spin ROS subscriber"""
             rospy.spin()
-
-        elif  self.transport  == 'ROS2':
+        elif self.transport == 'ROS2':
             import rclpy
             while rclpy.ok():
                 rclpy.spin_once(self.node_ros2)
             # Destroy the node explicitly
             # (optional - otherwise it will be done automatically
             # when the garbage collector destroys the node object)
             self.node_ros2.destroy_node()
```

### Comparing `nep-0.5.3.9/nep/publisher.py` & `nep-0.5.4.0/nep/publisher.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import time
 import os
 import zmq
 import simplejson
 import sys
 import nep
 import base64
+import msgpack
 
 
 
 try:
     import nanomsg
 except ImportError:
     pass
@@ -29,15 +30,15 @@
     import cv2
 except ImportError:
     pass
 
 
 
 class publisher:
-    """ Publisher class used for inter-process comunication between nodes. Supports ZeroMQ, nanomsg and ROS publishers. 
+    """ Publisher class used for inter-process communication between nodes. Supports ZeroMQ, nanomsg and ROS publishers. 
         
         Parameters
         ----------
 
         topic : string 
             Topic name to publish the messages
 
@@ -104,21 +105,18 @@
                 self.mode = self.conf['mode']
             self.__create_NN_publisher()
         else:
             msg = "NEP ERROR: Transport parameter " + self.transport + "is not supported, use instead 'ROS', 'ROS2', 'ZMQ' or 'nanomsg' "
             raise ValueError(msg)
 
     def __create_ROS2_publisher(self):
-
         from std_msgs.msg import String
         self.ros_pub = self.node.create_publisher(String, self.topic)
         self.connected = True
 
-
-
     #TODO:also define queue_size
     def __create_ROS_publisher(self):
         """Function used to create a ROS publisher"""
         import rospy
         
         from std_msgs.msg import String
         self.ros_pub = rospy.Publisher(self.topic, String, queue_size=10)
@@ -319,23 +317,33 @@
 
         """
 
         if self.msg_type == "string":
             self.send_string(message)
         elif self.msg_type == "json":
             self.send_json(message)
+        elif self.msg_type == "msgpack":
+            self.send_msgpack(message)
         elif self.msg_type == "image":
             self.send_image(message)
         else:
             message["type"] = self.msg_type
             self.send_json(message)
 
             #msg = "NEP ERROR: msg_type selected '" + str(self.msg_type) + "' non compatible"
             #raise ValueError(msg)
 
+
+    def send_msgpack(self,message):
+        if self.connected:
+            self.sock.send(msgpack.dumps(message))
+        else:
+            print ("NEP ERROR: socket not connected")
+
+
     def send_image(self,message):
         """ Publish a opencv image. 
             
             Parameters
             ----------
             message : image 
                 Image to be sended 
@@ -344,16 +352,14 @@
         ret, jpg = cv2.imencode('.jpg', message)
         encoded = base64.b64encode(jpg.tostring())
         if sys.version_info[0] == 2:
             self.sock.send(self.topic + ' ' + str(encoded))
         else:
             self.sock.send_string(self.topic + ' ' + encoded.decode("utf-8"))
             
-
-        
     
     def send_string(self,message):
         """ Publish a string value. 
             
             Parameters
             ----------
             message : string
```

### Comparing `nep-0.5.3.9/nep/respondent.py` & `nep-0.5.4.0/nep/respondent.py`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/nep/server.py` & `nep-0.5.4.0/nep/server.py`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/nep/subscriber.py` & `nep-0.5.4.0/nep/subscriber.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 import time
 import os
 import zmq
 import simplejson
 import sys
 import nep
 import base64
+import msgpack
 
 
 try:
     import numpy as np
 except ImportError:
     pass
 
@@ -180,20 +181,25 @@
                 # ZeroMQ Context
                 self.context = zmq.Context()
                 # Define the type of context, in this case a subcriber
                 self.sock = self.context.socket(zmq.SUB)
                 # Define subscription and the messages with prefix to accept.
                 # setsockopt obtain the data which message starts with the second argument
                 # Then we obtain data from the topic with that starts with self.topic value
-                if sys.version_info[0] == 2:
-                    self.sock.setsockopt(zmq.SUBSCRIBE, self.topic)
-                    self.sock.setsockopt(zmq.CONFLATE, 1) # Only keeps last mesange in queue
+
+                if self.msg_type =="msgpack":
+                        self.sock.setsockopt(zmq.SUBSCRIBE, b"")
+                        self.sock.setsockopt(zmq.CONFLATE, 1) # Only keeps last message in queue
                 else:
-                    self.sock.setsockopt_string(zmq.SUBSCRIBE, self.topic)
-                    self.sock.setsockopt(zmq.CONFLATE, 1)
+                    if sys.version_info[0] == 2:
+                        self.sock.setsockopt(zmq.SUBSCRIBE, self.topic)
+                        self.sock.setsockopt(zmq.CONFLATE, 1) # Only keeps last message in queue
+                    else:
+                        self.sock.setsockopt_string(zmq.SUBSCRIBE, self.topic)
+                        self.sock.setsockopt(zmq.CONFLATE, 1)
                 
                 self.__connect_ZMQ_socket()
             except:
                 print ("NEP ERROR: socket already in use")
         else:
             print("NEP ERROR: Socket unable to be connected")
 
@@ -316,15 +322,15 @@
         """
         if sys.version_info[0] == 2:
             if str is unicode and isinstance(s, bytes):
                 s = s.decode('utf8')
         return simplejson.loads(s, **kwargs)
 
 
-    def __deserialization(self, info):
+    def __JSONdecoding(self, info):
         """ Separate the topic and the json message from the data received from the ZeroMQ socket. If the deserialization was successful and the message as a python dictionary
             
             Parameters
             ----------
             info : string
                 topic + message received by the ZQM socket 
 
@@ -339,34 +345,98 @@
             msg = self.__loads(info[json0:])
             success = True
         except:
             print("NEP Serialization Error: \n" + str(info) + "\n" + "Is not JSON serializable")
             msg = {}
             success = False
         return success, msg
+    
+
+    def __PACKdecoding(self, info):
+        try:
+            msg = msgpack.unpackb(info)
+            success = True
+        except:
+            print("NEP Serialization Error: \n" + str(info) + "\n" + "Is not MSGPACK serializable")
+            msg = {}
+            success = False
+        return success, msg
+    
+    
+
 
     def listen(self,block_mode = False):
         """ Listen data from publishers
             
             Returns
             -------
             message : string or dict
                 Return message, must be the same type that msg_type
         """
 
         if self.msg_type == "string":
             return self.listen_string(block_mode)
+        elif self.msg_type == "msgpack":
+             return self.listen_msgpack(block_mode)
         elif self.msg_type == "json":
             return self.listen_json(block_mode)
         elif self.msg_type == "image":
             return self.listen_image(block_mode)
         else:
             msg = "NEP ERROR: msg_type selected '" + str(self.msg_type) + "' non compatible"
             raise ValueError(msg)
 
+    def listen_msgpack(self, block_mode =  False):
+        """ Listen for a json message. The operation is by default in non blocking mode
+            
+            Parameters
+            ----------
+
+            block_mode : bool
+                If True, the socket will set in blocking mode, otherwise the socket will be in non blocking mode
+                
+            Returns
+            -------
+
+            success : bool
+                If True the information was obtained inside the timeline in non blocking mode  
+
+            info : dictionary
+                Message obtained
+        """
+         
+        success = False
+        info = {}
+        try:
+            #Blocking mode
+            if block_mode:
+                success, info = self.__PACKdecoding(self.sock.recv())
+                #time.sleep(.001)
+            #Non blocking mode
+            else:
+                if self.transport ==  "ZMQ":
+                    success, info = self.__PACKdecoding(self.sock.recv(flags = zmq.NOBLOCK))
+                elif self.transport ==  "NN" or self.transport ==  "nanomsg":
+                    success, info = self.__PACKdecoding(self.sock.recv(flags=nanomsg.DONTWAIT))
+
+                #time.sleep(.001)
+        #Exeption for non blocking mode timeout
+        except zmq.Again as e:
+            #Nothing to read
+            success = False
+            pass
+
+        #Exeption for non blocking mode timeout
+        except nanomsg.NanoMsgAPIError:
+            #Nothing to read
+            success = False
+            pass
+
+        return  success, info
+
     def listen_image(self, block_mode = False):
         """ Function used to read string data from the sokect. The operation is by default in non blocking mode
 
             Parameters
             ----------
             block_mode : bool
                 If True, the socket will set in blocking mode, otherwise the socket will be in non blocking mode
@@ -472,29 +542,29 @@
          
         success = False
         info = {}
         try:
             #Blocking mode
             if block_mode:
                 if sys.version_info[0] == 2:
-                    success, info = self.__deserialization(self.sock.recv())
+                    success, info = self.__JSONdecoding(self.sock.recv())
                 else:
-                    success,info = self.__deserialization(self.sock.recv_string())
+                    success,info = self.__JSONdecoding(self.sock.recv_string())
 
                 #time.sleep(.001)
             #Non blocking mode
             else:
                 if self.transport ==  "ZMQ":
                     if sys.version_info[0] == 2:
-                        success, info = self.__deserialization(self.sock.recv(flags = zmq.NOBLOCK))
+                        success, info = self.__JSONdecoding(self.sock.recv(flags = zmq.NOBLOCK))
                     else:
-                        success,info = self.__deserialization(self.sock.recv_string(flags = zmq.NOBLOCK))
+                        success,info = self.__JSONdecoding(self.sock.recv_string(flags = zmq.NOBLOCK))
 
                 elif self.transport ==  "NN" or self.transport ==  "nanomsg":
-                    success, info = self.__deserialization(self.sock.recv(flags=nanomsg.DONTWAIT))
+                    success, info = self.__JSONdecoding(self.sock.recv(flags=nanomsg.DONTWAIT))
 
                 #time.sleep(.001)
         #Exeption for non blocking mode timeout
         except zmq.Again as e:
             #Nothing to read
             success = False
             pass
```

### Comparing `nep-0.5.3.9/nep/surveyor.py` & `nep-0.5.4.0/nep/surveyor.py`

 * *Files identical despite different names*

### Comparing `nep-0.5.3.9/setup.py` & `nep-0.5.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 from setuptools import setup
 
-#from distutils.core import setup
+with open("README.rst", "r", encoding="utf-8") as f:
+    long_description = f.read()
 
 setup(
     name='nep',
-    version='0.5.3.9',
+    version='0.5.4.0',
     author='Enrique Coronado',
     author_email='enriquecoronadozu@gmail.mx',
     url='http://enriquecoronadozu.github.io',
-    description='NEP robot programming framework',
+    description='NEP Python libraries',
+    long_description=long_description,
+    long_description_content_type="text/x-rst",
     packages=["nep"],
-    install_requires=['pyzmq','simplejson'],
+    install_requires=['pyzmq','simplejson', 'msgpack'],
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Console",
-        "Intended Audience :: End Users/Desktop",
+        "Intended Audience :: Science/Research",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU Library or Lesser General Public License (LGPL)",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3.6",
         "Topic :: Software Development"
```

