# Comparing `tmp/djangoldp_babelfish-1.0.8.tar.gz` & `tmp/djangoldp_babelfish-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangoldp_babelfish-1.0.8.tar", last modified: Wed Aug  2 10:30:20 2023, max compression
+gzip compressed data, was "djangoldp_babelfish-1.0.9.tar", last modified: Wed Aug  2 10:34:02 2023, max compression
```

## Comparing `djangoldp_babelfish-1.0.8.tar` & `djangoldp_babelfish-1.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:30:20.985194 djangoldp_babelfish-1.0.8/
--rw-r--r--   0 root         (0) root         (0)      335 2023-08-02 10:30:20.985194 djangoldp_babelfish-1.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1979 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:30:20.981193 djangoldp_babelfish-1.0.8/djangoldp_babelfish/
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-08-02 10:30:18.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/admin.py
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/apps.py
--rw-rw-rw-   0 root         (0) root         (0)      222 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/djangoldp_urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:30:20.981193 djangoldp_babelfish-1.0.8/djangoldp_babelfish/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:30:20.981193 djangoldp_babelfish-1.0.8/djangoldp_babelfish/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/management/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:30:20.981193 djangoldp_babelfish-1.0.8/djangoldp_babelfish/migrations/
--rw-rw-rw-   0 root         (0) root         (0)     1938 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/migrations/0001_initial.py
--rw-rw-rw-   0 root         (0) root         (0)      559 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2966 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3236 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish/views.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:30:20.981193 djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/
--rw-r--r--   0 root         (0) root         (0)      335 2023-08-02 10:30:20.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      671 2023-08-02 10:30:20.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 10:30:20.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2023-08-02 10:30:20.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-08-02 10:30:20.000000 djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      662 2023-08-02 10:30:20.985194 djangoldp_babelfish-1.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       61 2023-08-02 10:30:01.000000 djangoldp_babelfish-1.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1979 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/djangoldp_babelfish/
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-08-02 10:33:59.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/admin.py
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/apps.py
+-rw-rw-rw-   0 root         (0) root         (0)      222 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/djangoldp_urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/djangoldp_babelfish/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 10:33:44.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/djangoldp_babelfish/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 10:33:44.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/management/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/djangoldp_babelfish/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1938 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/migrations/0001_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)      559 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-08-02 10:33:44.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2959 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3236 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish/views.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      335 2023-08-02 10:34:02.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      671 2023-08-02 10:34:02.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-02 10:34:02.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2023-08-02 10:34:02.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-08-02 10:34:02.000000 djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      662 2023-08-02 10:34:02.469864 djangoldp_babelfish-1.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       61 2023-08-02 10:33:43.000000 djangoldp_babelfish-1.0.9/setup.py
```

### Comparing `djangoldp_babelfish-1.0.8/README.md` & `djangoldp_babelfish-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.8/djangoldp_babelfish/migrations/0001_initial.py` & `djangoldp_babelfish-1.0.9/djangoldp_babelfish/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.8/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py` & `djangoldp_babelfish-1.0.9/djangoldp_babelfish/migrations/0002_auto_20230720_1705.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.8/djangoldp_babelfish/models.py` & `djangoldp_babelfish-1.0.9/djangoldp_babelfish/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         }
 
         try:
             response = requests.post(create_user_url, headers=headers, data=json.dumps(data))
             babelfish_profile_info = response.json()
 
             # Save the BabelFish user credentials to the user's profile
-            profile = BabelfishProfile.objects.get_or_create(user=instance)
+            profile = BabelfishProfile.objects.create(user=instance)
             profile.babelfish_user_id = babelfish_profile_info.get('user-id')
             profile.organisation_id = babelfish_profile_info.get('organization-id')
             profile.client_id = babelfish_profile_info.get('oauth').get('client-id')
             profile.client_secret = babelfish_profile_info.get('oauth').get('client-secret')
             profile.save()
         except Exception as e:
             print(e)
```

### Comparing `djangoldp_babelfish-1.0.8/djangoldp_babelfish/views.py` & `djangoldp_babelfish-1.0.9/djangoldp_babelfish/views.py`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.8/djangoldp_babelfish.egg-info/SOURCES.txt` & `djangoldp_babelfish-1.0.9/djangoldp_babelfish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangoldp_babelfish-1.0.8/setup.cfg` & `djangoldp_babelfish-1.0.9/setup.cfg`

 * *Files identical despite different names*

