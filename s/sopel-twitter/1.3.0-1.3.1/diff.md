# Comparing `tmp/sopel-twitter-1.3.0.tar.gz` & `tmp/sopel-twitter-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sopel-twitter-1.3.0.tar", last modified: Wed Jul 26 00:27:47 2023, max compression
+gzip compressed data, was "sopel-twitter-1.3.1.tar", last modified: Sat Aug  5 07:23:42 2023, max compression
```

## Comparing `sopel-twitter-1.3.0.tar` & `sopel-twitter-1.3.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/
--rw-------   0 u0_a687  (10687)    10687     1022 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/COPYING
--rw-------   0 u0_a687  (10687)    10687      161 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/MANIFEST.in
--rw-------   0 u0_a687  (10687)    10687     3024 2023-07-26 00:25:55.000000 sopel-twitter-1.3.0/NEWS
--rw-------   0 u0_a687  (10687)    10687     5888 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/PKG-INFO
--rw-------   0 u0_a687  (10687)    10687     2290 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/README.md
--rw-------   0 u0_a687  (10687)    10687        0 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/dev-requirements.txt
--rw-------   0 u0_a687  (10687)    10687      694 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/setup.cfg
--rwx------   0 u0_a687  (10687)    10687      889 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/setup.py
-drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/sopel_twitter/
--rw-------   0 u0_a687  (10687)    10687    10485 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/sopel_twitter/__init__.py
-drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/sopel_twitter.egg-info/
--rw-------   0 u0_a687  (10687)    10687     5888 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/PKG-INFO
--rw-------   0 u0_a687  (10687)    10687      400 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/SOURCES.txt
--rw-------   0 u0_a687  (10687)    10687        1 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/dependency_links.txt
--rw-------   0 u0_a687  (10687)    10687       40 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/entry_points.txt
--rw-------   0 u0_a687  (10687)    10687        1 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/not-zip-safe
--rw-------   0 u0_a687  (10687)    10687       31 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/requires.txt
--rw-------   0 u0_a687  (10687)    10687       20 2023-07-26 00:27:47.000000 sopel-twitter-1.3.0/sopel_twitter.egg-info/top_level.txt
-drwx------   0 u0_a687  (10687)    10687        0 2023-07-26 00:27:47.601035 sopel-twitter-1.3.0/tests/
--rw-------   0 u0_a687  (10687)    10687       15 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/tests/__init__.py
--rw-------   0 u0_a687  (10687)    10687      296 2023-07-26 00:20:50.000000 sopel-twitter-1.3.0/tests/test_twitter.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-08-05 07:23:42.374728 sopel-twitter-1.3.1/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     1022 2023-07-19 19:28:24.000000 sopel-twitter-1.3.1/COPYING
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      161 2023-07-19 19:28:24.000000 sopel-twitter-1.3.1/MANIFEST.in
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     3345 2023-08-05 06:12:24.000000 sopel-twitter-1.3.1/NEWS
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     6196 2023-08-05 07:23:42.374728 sopel-twitter-1.3.1/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     2257 2023-07-31 09:08:02.000000 sopel-twitter-1.3.1/README.md
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        0 2023-07-19 19:28:24.000000 sopel-twitter-1.3.1/dev-requirements.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      694 2023-08-05 07:23:42.374728 sopel-twitter-1.3.1/setup.cfg
+-rwxr-xr-x   0 dgw       (1000) dgw       (1000)      889 2023-07-19 19:28:24.000000 sopel-twitter-1.3.1/setup.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-08-05 07:23:42.374728 sopel-twitter-1.3.1/sopel_twitter/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)    11067 2023-08-05 06:03:04.000000 sopel-twitter-1.3.1/sopel_twitter/__init__.py
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-08-05 07:23:42.374728 sopel-twitter-1.3.1/sopel_twitter.egg-info/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)     6196 2023-08-05 07:23:42.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/PKG-INFO
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      400 2023-08-05 07:23:42.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/SOURCES.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-08-05 07:23:42.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/dependency_links.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       41 2023-08-05 07:23:42.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/entry_points.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)        1 2023-07-19 19:31:03.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/not-zip-safe
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       31 2023-08-05 07:23:42.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/requires.txt
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       20 2023-08-05 07:23:42.000000 sopel-twitter-1.3.1/sopel_twitter.egg-info/top_level.txt
+drwxr-xr-x   0 dgw       (1000) dgw       (1000)        0 2023-08-05 07:23:42.374728 sopel-twitter-1.3.1/tests/
+-rw-r--r--   0 dgw       (1000) dgw       (1000)       15 2023-07-19 19:28:24.000000 sopel-twitter-1.3.1/tests/__init__.py
+-rw-r--r--   0 dgw       (1000) dgw       (1000)      296 2023-07-19 19:28:24.000000 sopel-twitter-1.3.1/tests/test_twitter.py
```

### Comparing `sopel-twitter-1.3.0/COPYING` & `sopel-twitter-1.3.1/COPYING`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.3.0/NEWS` & `sopel-twitter-1.3.1/NEWS`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Changes between 1.3.0 and 1.3.1
+===============================
+
+Changed:
+* Use updated `tweety-ns` with option to specify session JSON storage location (#51)
+  * Now stored in Sopel's `homedir`
+  * See README for shell commands suggested for cleaning up the old ones
+
+Fixed:
+* Handle new `DeniedLogin` exception (#52)
+
+
 Changes between 1.2.0 and 1.3.0
 ===============================
 
 Breaking:
 * **Login with username/password is now required**
   * Creating a throwaway Twitter account is recommended
```

### Comparing `sopel-twitter-1.3.0/PKG-INFO` & `sopel-twitter-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Description-Content-Type: text/markdown
 License-File: COPYING
@@ -58,24 +59,24 @@
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
 # Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
 ### Important note
 
-The library this plugin uses for Twitter data access stores its login session
-data in **the current working directory**. For Sopel, that is the directory
-from which the `sopel` command is run.
-
-A future library release promises to add support for specifying where to store
-session data, at which point this plugin will be updated to use the `homedir`
-of Sopel's configuration (`~/.sopel` by default). You will be able to locate
-the old session files by running e.g. `find / -type f -name
-'sopel-twitter*.json' 2>/dev/null`. (Running `find` on `/` tends to output
-numerous "Permission denied" errors, so suppressing stderr is recommended.)
+The library this plugin uses for Twitter data access previously stored its
+login session data in **the current working directory**. For Sopel, that was
+the directory from which the `sopel` command was run.
+
+As of sopel-twitter 1.3.1, a newer library version became available with
+support for storing session data in Sopel's `homedir` instead. You can clean
+up the old session files left behind by sopel-twitter 1.3.0 by running e.g.
+`find / -type f -name 'sopel-twitter*.json' 2>/dev/null`. (Running `find` on
+`/` tends to output numerous "Permission denied" errors, so suppressing stderr
+is recommended.)
 
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
 
@@ -83,14 +84,26 @@
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
 
+Changes between 1.3.0 and 1.3.1
+===============================
+
+Changed:
+* Use updated `tweety-ns` with option to specify session JSON storage location (#51)
+  * Now stored in Sopel's `homedir`
+  * See README for shell commands suggested for cleaning up the old ones
+
+Fixed:
+* Handle new `DeniedLogin` exception (#52)
+
+
 Changes between 1.2.0 and 1.3.0
 ===============================
 
 Breaking:
 * **Login with username/password is now required**
   * Creating a throwaway Twitter account is recommended
 
@@ -225,7 +238,9 @@
 
 
 Changes between 0.1.0 and 0.1.1
 ===============================
 
 Fixed:
 * Unicode on Python 3
+
+
```

### Comparing `sopel-twitter-1.3.0/README.md` & `sopel-twitter-1.3.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -42,24 +42,24 @@
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
 # Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
 ### Important note
 
-The library this plugin uses for Twitter data access stores its login session
-data in **the current working directory**. For Sopel, that is the directory
-from which the `sopel` command is run.
-
-A future library release promises to add support for specifying where to store
-session data, at which point this plugin will be updated to use the `homedir`
-of Sopel's configuration (`~/.sopel` by default). You will be able to locate
-the old session files by running e.g. `find / -type f -name
-'sopel-twitter*.json' 2>/dev/null`. (Running `find` on `/` tends to output
-numerous "Permission denied" errors, so suppressing stderr is recommended.)
+The library this plugin uses for Twitter data access previously stored its
+login session data in **the current working directory**. For Sopel, that was
+the directory from which the `sopel` command was run.
+
+As of sopel-twitter 1.3.1, a newer library version became available with
+support for storing session data in Sopel's `homedir` instead. You can clean
+up the old session files left behind by sopel-twitter 1.3.0 by running e.g.
+`find / -type f -name 'sopel-twitter*.json' 2>/dev/null`. (Running `find` on
+`/` tends to output numerous "Permission denied" errors, so suppressing stderr
+is recommended.)
 
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
```

### Comparing `sopel-twitter-1.3.0/setup.cfg` & `sopel-twitter-1.3.1/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sopel-twitter
-version = 1.3.0
+version = 1.3.1
 description = A Twitter plugin for Sopel
 author = dgw
 author_email = dgw@technobabbl.es
 url = https://github.com/sopel-irc/sopel-twitter
 license = Eiffel Forum License, version 2
 classifiers = 
 	Intended Audience :: Developers
@@ -15,15 +15,15 @@
 
 [options]
 packages = find:
 zip_safe = false
 include_package_data = true
 install_requires = 
 	sopel>=7.1,<9
-	tweety-ns~=0.9.0
+	tweety-ns~=0.9.6
 
 [options.entry_points]
 sopel.plugins = 
 	twitter = sopel_twitter
 
 [egg_info]
 tag_build =
```

### Comparing `sopel-twitter-1.3.0/setup.py` & `sopel-twitter-1.3.1/setup.py`

 * *Files identical despite different names*

### Comparing `sopel-twitter-1.3.0/sopel_twitter/__init__.py` & `sopel-twitter-1.3.1/sopel_twitter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 A Twitter plugin for Sopel
 """
 from __future__ import unicode_literals, absolute_import, division, print_function
 
 from datetime import datetime
 import json
+import os.path
 import re
 
 from tweety import Twitter, exceptions_ as tweety_errors
 
 from sopel import plugin, tools
 from sopel.config.types import (
     BooleanAttribute,
@@ -54,15 +55,23 @@
 
 def setup(bot):
     bot.config.define_section('twitter', TwitterSection)
 
 
 def _get_tweety_session_name(bot):
     """Return a session name for this plugin + bot config."""
-    return "sopel-twitter.{}".format(bot.settings.basename)
+    return os.path.join(
+        _get_tweety_session_path(bot),
+        "{}.sopel-twitter".format(bot.settings.basename)
+    )
+
+
+def _get_tweety_session_path(bot):
+    """Return the path to where this plugin's sessions should live."""
+    return os.path.expanduser(bot.settings.homedir)
 
 
 def get_preferred_media_item_link(item):
     """
     Guess the most useful link for a given piece of embedded media.
 
     :param item: a single Media object from Tweety
@@ -199,14 +208,17 @@
         app.connect()
 
         if not app.session.logged_in:
             # existing session not present
             app.sign_in(bot.settings.twitter.username, bot.settings.twitter.password)
 
         tweet = app.tweet_detail(id_)
+    except tweety_errors.DeniedLogin:
+        bot.say("Twitter wouldn't let me log in. Please try again later. If this issue persists, contact my owner.")
+        return
     except tweety_errors.InvalidCredentials:
         bot.say("Can't authenticate with Twitter. Please ask my owner to check my credentials.")
         return
     except tweety_errors.AuthenticationRequired:
         bot.say("That content requires authentication; sorry!")
         return
     except tweety_errors.RateLimitReached:
@@ -249,14 +261,17 @@
         app.connect()
 
         if not app.session.logged_in:
             # existing session not present
             app.sign_in(bot.settings.twitter.username, bot.settings.twitter.password)
 
         user = app.get_user_info(sn)
+    except tweety_errors.DeniedLogin:
+        bot.say("Twitter wouldn't let me log in. Please try again later. If this issue persists, contact my owner.")
+        return
     except tweety_errors.InvalidCredentials:
         bot.say("Can't authenticate with Twitter. Please ask my owner to check my credentials.")
         return
     except tweety_errors.UserNotFound:
         bot.say("User not found.")
         return
     except tweety_errors.UserProtected:
```

### Comparing `sopel-twitter-1.3.0/sopel_twitter.egg-info/PKG-INFO` & `sopel-twitter-1.3.1/sopel_twitter.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sopel-twitter
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Twitter plugin for Sopel
 Home-page: https://github.com/sopel-irc/sopel-twitter
 Author: dgw
 Author-email: dgw@technobabbl.es
 License: Eiffel Forum License, version 2
+Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: Eiffel Forum License (EFL)
 Classifier: License :: OSI Approved :: Eiffel Forum License
 Classifier: Topic :: Communications :: Chat :: Internet Relay Chat
 Description-Content-Type: text/markdown
 License-File: COPYING
@@ -58,24 +59,24 @@
     nitter.net
 # Optional: What other domains should we treat like twitter domains?
 # Default: fxtwitter.com, vxtwitter.com, nitter.net
 ```
 
 ### Important note
 
-The library this plugin uses for Twitter data access stores its login session
-data in **the current working directory**. For Sopel, that is the directory
-from which the `sopel` command is run.
-
-A future library release promises to add support for specifying where to store
-session data, at which point this plugin will be updated to use the `homedir`
-of Sopel's configuration (`~/.sopel` by default). You will be able to locate
-the old session files by running e.g. `find / -type f -name
-'sopel-twitter*.json' 2>/dev/null`. (Running `find` on `/` tends to output
-numerous "Permission denied" errors, so suppressing stderr is recommended.)
+The library this plugin uses for Twitter data access previously stored its
+login session data in **the current working directory**. For Sopel, that was
+the directory from which the `sopel` command was run.
+
+As of sopel-twitter 1.3.1, a newer library version became available with
+support for storing session data in Sopel's `homedir` instead. You can clean
+up the old session files left behind by sopel-twitter 1.3.0 by running e.g.
+`find / -type f -name 'sopel-twitter*.json' 2>/dev/null`. (Running `find` on
+`/` tends to output numerous "Permission denied" errors, so suppressing stderr
+is recommended.)
 
 ## Usage
 
 Just send a link to a tweet or profile!
 
 You can also retrieve a user's info with the `.twitinfo` command:
 
@@ -83,14 +84,26 @@
 < Wiz> .twitinfo NASA
 < Sopel> [Twitter] NASA (@NASA) ✔️ | Pale Blue Dot | http://www.nasa.gov/
          | 204 friends, 46,602,251 followers | 65,377 tweets, 13,040 ♥s
          | Joined: 2007-12-19 - 20:20:32UTC | There's space for everybody. ✨
 ```
 
 
+Changes between 1.3.0 and 1.3.1
+===============================
+
+Changed:
+* Use updated `tweety-ns` with option to specify session JSON storage location (#51)
+  * Now stored in Sopel's `homedir`
+  * See README for shell commands suggested for cleaning up the old ones
+
+Fixed:
+* Handle new `DeniedLogin` exception (#52)
+
+
 Changes between 1.2.0 and 1.3.0
 ===============================
 
 Breaking:
 * **Login with username/password is now required**
   * Creating a throwaway Twitter account is recommended
 
@@ -225,7 +238,9 @@
 
 
 Changes between 0.1.0 and 0.1.1
 ===============================
 
 Fixed:
 * Unicode on Python 3
+
+
```

