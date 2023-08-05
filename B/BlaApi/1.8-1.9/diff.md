# Comparing `tmp/BlaApi-1.8.tar.gz` & `tmp/BlaApi-1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BlaApi-1.8.tar", last modified: Thu Jul 13 20:05:24 2023, max compression
+gzip compressed data, was "BlaApi-1.9.tar", last modified: Sat Aug  5 00:50:28 2023, max compression
```

## Comparing `BlaApi-1.8.tar` & `BlaApi-1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-13 20:05:24.508015 BlaApi-1.8/
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-13 20:05:24.497015 BlaApi-1.8/BlaApi/
--rw-r--r--   0 muddi     (1000) muddi     (1001)       26 2023-06-24 11:54:49.000000 BlaApi-1.8/BlaApi/__init__.py
--rw-r--r--   0 muddi     (1000) muddi     (1001)     8231 2023-07-13 20:04:42.000000 BlaApi-1.8/BlaApi/client.py
-drwxr-xr-x   0 muddi     (1000) muddi     (1001)        0 2023-07-13 20:05:24.505015 BlaApi-1.8/BlaApi.egg-info/
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)      211 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/SOURCES.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        1 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/dependency_links.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)       33 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/requires.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)        7 2023-07-13 20:05:23.000000 BlaApi-1.8/BlaApi.egg-info/top_level.txt
--rw-r--r--   0 muddi     (1000) muddi     (1001)     1669 2023-06-22 17:58:15.000000 BlaApi-1.8/LICENSE
--rw-r--r--   0 muddi     (1000) muddi     (1001)     5485 2023-07-13 20:05:24.506015 BlaApi-1.8/PKG-INFO
--rw-r--r--   0 muddi     (1000) muddi     (1001)     4851 2023-06-26 11:18:41.000000 BlaApi-1.8/README.md
--rw-r--r--   0 muddi     (1000) muddi     (1001)       38 2023-07-13 20:05:24.508015 BlaApi-1.8/setup.cfg
--rw-r--r--   0 muddi     (1000) muddi     (1001)     3596 2023-07-13 20:05:13.000000 BlaApi-1.8/setup.py
+drwxr-xr-x   0 linus     (1000) linus     (1000)        0 2023-08-05 00:50:28.303130 BlaApi-1.9/
+drwxr-xr-x   0 linus     (1000) linus     (1000)        0 2023-08-05 00:50:28.301130 BlaApi-1.9/BlaApi/
+-rw-r--r--   0 linus     (1000) linus     (1000)       26 2023-08-05 00:48:56.000000 BlaApi-1.9/BlaApi/__init__.py
+-rw-r--r--   0 linus     (1000) linus     (1000)     8778 2023-08-05 00:48:56.000000 BlaApi-1.9/BlaApi/client.py
+drwxr-xr-x   0 linus     (1000) linus     (1000)        0 2023-08-05 00:50:28.302130 BlaApi-1.9/BlaApi.egg-info/
+-rw-r--r--   0 linus     (1000) linus     (1000)     5485 2023-08-05 00:50:28.000000 BlaApi-1.9/BlaApi.egg-info/PKG-INFO
+-rw-r--r--   0 linus     (1000) linus     (1000)      211 2023-08-05 00:50:28.000000 BlaApi-1.9/BlaApi.egg-info/SOURCES.txt
+-rw-r--r--   0 linus     (1000) linus     (1000)        1 2023-08-05 00:50:28.000000 BlaApi-1.9/BlaApi.egg-info/dependency_links.txt
+-rw-r--r--   0 linus     (1000) linus     (1000)       33 2023-08-05 00:50:28.000000 BlaApi-1.9/BlaApi.egg-info/requires.txt
+-rw-r--r--   0 linus     (1000) linus     (1000)        7 2023-08-05 00:50:28.000000 BlaApi-1.9/BlaApi.egg-info/top_level.txt
+-rw-r--r--   0 linus     (1000) linus     (1000)     1669 2023-08-05 00:48:56.000000 BlaApi-1.9/LICENSE
+-rw-r--r--   0 linus     (1000) linus     (1000)     5485 2023-08-05 00:50:28.302130 BlaApi-1.9/PKG-INFO
+-rw-r--r--   0 linus     (1000) linus     (1000)     4851 2023-08-05 00:48:56.000000 BlaApi-1.9/README.md
+-rw-r--r--   0 linus     (1000) linus     (1000)       38 2023-08-05 00:50:28.303130 BlaApi-1.9/setup.cfg
+-rw-r--r--   0 linus     (1000) linus     (1000)     3596 2023-08-05 00:50:21.000000 BlaApi-1.9/setup.py
```

### Comparing `BlaApi-1.8/BlaApi/client.py` & `BlaApi-1.9/BlaApi/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -98,30 +98,40 @@
         if not isinstance(notification_ids, list): # error check
             raise ValueError("Notification IDs must be passed as a list")
         
         for notification_id in notification_ids:
             # Construct API endpoint URL
             endpoint = "diaryDetails"
             api_url = f"https://beaconlightacademy.edu.pk/app/restapi.php?endpoint={endpoint}&accessToken={self.token}&appUserNotificationId={notification_id}"
+            media_url='https://beaconlightacademy.edu.pk/app/uploaded/'
             
             # Send POST request to API endpoint with headers
             response = self.client.post(api_url, headers=self.headers)
             
             #! Raise an error if POST fails
             response.raise_for_status()
             
             # error handling
             if json.loads(response.content).get('success') == False:
                 raise ValueError(json.loads(response.content).get('error'))
             
             # Retrieve diary data from JSON response
             data = json.loads(response.content)['data']
             # parse diary details by converting to markdown
-            data['details'] = markdownify(data.get('details'))
-            
+            # need try except statement because api sometimes returns ambigious ids
+            try:
+                data['details'] = markdownify(data.get('details'))
+            except TypeError:
+                data['details'] = None
+            # append url to attachment id
+            if data.get('attachment'):
+                data['attachment']=f'{media_url}{data.get("attachment")}'
+            # append url to attachment id
+            if data.get('attachment2'):
+                data['attachment2']=f'{media_url}{data.get("attachment2")}'
             output.append(data)
 
         return output
     
     def search_by_student(self, passthru=None, student_id=None):
 
         diary = self.get_diary_list()
@@ -226,8 +236,8 @@
         else:
             for d in diary:
                 if d['bRead'] == been_read:
                     output.append(d['id'])
         if output:
             return output
         else:
-            raise LookupError('No unread/read diaries found.')
+            raise LookupError('No unread/read diaries found.')
```

### Comparing `BlaApi-1.8/BlaApi.egg-info/PKG-INFO` & `BlaApi-1.9/BlaApi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.8
+Version: 1.9
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.8/LICENSE` & `BlaApi-1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BlaApi-1.8/PKG-INFO` & `BlaApi-1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: BlaApi
-Version: 1.8
+Version: 1.9
 Summary: A wrapper for the beacon light api.
 Home-page: https://github.com/me/myproject
 Author: Omer-Farooqui
 Author-email: deaddogfuneral@gmail.com
 License: BSD-4
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

### Comparing `BlaApi-1.8/README.md` & `BlaApi-1.9/README.md`

 * *Files identical despite different names*

### Comparing `BlaApi-1.8/setup.py` & `BlaApi-1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # Package meta-data.
 NAME = 'BlaApi'
 DESCRIPTION = 'A wrapper for the beacon light api.'
 URL = 'https://github.com/me/myproject'
 EMAIL = 'deaddogfuneral@gmail.com'
 AUTHOR = 'Omer-Farooqui'
 REQUIRES_PYTHON = '>=3.7.0'
-VERSION = '1.8'
+VERSION = '1.9'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
      'httpx', 'fake_useragent','markdownify'
 ]
 
 # What packages are optional?
```

