# Comparing `tmp/python-bale-bot-2.4.6.tar.gz` & `tmp/python-bale-bot-2.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-bale-bot-2.4.6.tar", last modified: Mon Jun 26 09:34:53 2023, max compression
+gzip compressed data, was "python-bale-bot-2.4.7.tar", last modified: Sat Aug  5 15:02:06 2023, max compression
```

## Comparing `python-bale-bot-2.4.6.tar` & `python-bale-bot-2.4.7.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.341871 python-bale-bot-2.4.6/
--rw-rw-rw-   0        0        0    15402 2023-05-07 15:38:30.000000 python-bale-bot-2.4.6/LICENSE
--rw-rw-rw-   0        0        0     3057 2023-06-26 09:34:53.341208 python-bale-bot-2.4.6/PKG-INFO
--rw-rw-rw-   0        0        0     2341 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.133652 python-bale-bot-2.4.6/bale/
--rw-rw-rw-   0        0        0     2072 2023-06-20 15:49:07.000000 python-bale-bot-2.4.6/bale/__init__.py
--rw-rw-rw-   0        0        0      243 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/__main__.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.158670 python-bale-bot-2.4.6/bale/attachments/
--rw-rw-rw-   0        0        0      203 2023-06-20 14:42:57.000000 python-bale-bot-2.4.6/bale/attachments/__init__.py
--rw-rw-rw-   0        0        0     2452 2023-06-26 08:09:14.000000 python-bale-bot-2.4.6/bale/attachments/audio.py
--rw-rw-rw-   0        0        0     2323 2023-06-26 08:48:02.000000 python-bale-bot-2.4.6/bale/attachments/contact.py
--rw-rw-rw-   0        0        0     2307 2023-06-26 08:10:29.000000 python-bale-bot-2.4.6/bale/attachments/document.py
--rw-rw-rw-   0        0        0     4004 2023-06-26 08:40:10.000000 python-bale-bot-2.4.6/bale/attachments/file.py
--rw-rw-rw-   0        0        0     2323 2023-06-26 08:48:02.000000 python-bale-bot-2.4.6/bale/attachments/location.py
--rw-rw-rw-   0        0        0     2269 2023-06-26 08:10:29.000000 python-bale-bot-2.4.6/bale/attachments/photo.py
--rw-rw-rw-   0        0        0     2650 2023-06-26 08:10:29.000000 python-bale-bot-2.4.6/bale/attachments/video.py
--rw-rw-rw-   0        0        0    43778 2023-06-25 18:25:53.000000 python-bale-bot-2.4.6/bale/bot.py
--rw-rw-rw-   0        0        0     3964 2023-05-07 15:38:31.000000 python-bale-bot-2.4.6/bale/callbackquery.py
--rw-rw-rw-   0        0        0    11048 2023-06-20 16:33:57.000000 python-bale-bot-2.4.6/bale/chat.py
--rw-rw-rw-   0        0        0     3934 2023-04-13 11:25:40.000000 python-bale-bot-2.4.6/bale/chatmember.py
--rw-rw-rw-   0        0        0     3740 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/error.py
--rw-rw-rw-   0        0        0    15334 2023-06-26 08:04:21.000000 python-bale-bot-2.4.6/bale/message.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.203717 python-bale-bot-2.4.6/bale/payments/
--rw-rw-rw-   0        0        0       56 2023-04-11 12:58:40.000000 python-bale-bot-2.4.6/bale/payments/__init__.py
--rw-rw-rw-   0        0        0     2131 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/payments/invoice.py
--rw-rw-rw-   0        0        0     1733 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/payments/price.py
--rw-rw-rw-   0        0        0     4402 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/permissions.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.263710 python-bale-bot-2.4.6/bale/request/
--rw-rw-rw-   0        0        0      201 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/request/__init__.py
--rw-rw-rw-   0        0        0    10708 2023-05-17 19:07:05.000000 python-bale-bot-2.4.6/bale/request/http.py
--rw-rw-rw-   0        0        0     1371 2023-04-11 12:44:43.000000 python-bale-bot-2.4.6/bale/request/parser.py
--rw-rw-rw-   0        0        0      123 2023-04-09 22:53:13.000000 python-bale-bot-2.4.6/bale/request/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.276879 python-bale-bot-2.4.6/bale/ui/
--rw-rw-rw-   0        0        0      167 2023-06-26 08:08:10.000000 python-bale-bot-2.4.6/bale/ui/__init__.py
--rw-rw-rw-   0        0        0     4820 2023-06-26 08:20:23.000000 python-bale-bot-2.4.6/bale/ui/components.py
--rw-rw-rw-   0        0        0     2923 2023-06-20 15:49:07.000000 python-bale-bot-2.4.6/bale/ui/inline_keyboard.py
--rw-rw-rw-   0        0        0     1739 2023-06-26 08:24:36.000000 python-bale-bot-2.4.6/bale/ui/menu_keyboard.py
--rw-rw-rw-   0        0        0     6631 2023-04-11 17:56:28.000000 python-bale-bot-2.4.6/bale/update.py
--rw-rw-rw-   0        0        0     5356 2023-04-29 18:54:30.000000 python-bale-bot-2.4.6/bale/updater.py
--rw-rw-rw-   0        0        0     6782 2023-06-20 16:33:57.000000 python-bale-bot-2.4.6/bale/user.py
--rw-rw-rw-   0        0        0      328 2023-05-07 15:38:31.000000 python-bale-bot-2.4.6/bale/utils.py
--rw-rw-rw-   0        0        0      145 2023-06-20 14:42:57.000000 python-bale-bot-2.4.6/bale/version.py
-drwxrwxrwx   0        0        0        0 2023-06-26 09:34:53.338870 python-bale-bot-2.4.6/python_bale_bot.egg-info/
--rw-rw-rw-   0        0        0     3057 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      921 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      155 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-06-26 09:34:52.000000 python-bale-bot-2.4.6/python_bale_bot.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 09:34:53.341871 python-bale-bot-2.4.6/setup.cfg
--rw-rw-rw-   0        0        0     1672 2023-06-20 14:42:57.000000 python-bale-bot-2.4.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.261189 python-bale-bot-2.4.7/
+-rw-rw-rw-   0        0        0    15402 2023-05-07 15:38:30.000000 python-bale-bot-2.4.7/LICENSE
+-rw-rw-rw-   0        0        0     3082 2023-08-05 15:02:06.261189 python-bale-bot-2.4.7/PKG-INFO
+-rw-rw-rw-   0        0        0     2275 2023-08-05 14:55:48.000000 python-bale-bot-2.4.7/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:05.764274 python-bale-bot-2.4.7/bale/
+-rw-rw-rw-   0        0        0     2083 2023-07-12 15:55:46.000000 python-bale-bot-2.4.7/bale/__init__.py
+-rw-rw-rw-   0        0        0      243 2023-04-09 22:53:13.000000 python-bale-bot-2.4.7/bale/__main__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:05.953237 python-bale-bot-2.4.7/bale/attachments/
+-rw-rw-rw-   0        0        0      238 2023-07-12 15:55:46.000000 python-bale-bot-2.4.7/bale/attachments/__init__.py
+-rw-rw-rw-   0        0        0     2472 2023-07-26 15:24:37.000000 python-bale-bot-2.4.7/bale/attachments/audio.py
+-rw-rw-rw-   0        0        0     2335 2023-07-26 15:24:01.000000 python-bale-bot-2.4.7/bale/attachments/contact.py
+-rw-rw-rw-   0        0        0     2307 2023-06-26 08:10:29.000000 python-bale-bot-2.4.7/bale/attachments/document.py
+-rw-rw-rw-   0        0        0     4054 2023-07-26 15:37:49.000000 python-bale-bot-2.4.7/bale/attachments/file.py
+-rw-rw-rw-   0        0        0      707 2023-07-15 15:32:28.000000 python-bale-bot-2.4.7/bale/attachments/input_file.py
+-rw-rw-rw-   0        0        0     2323 2023-06-26 08:48:02.000000 python-bale-bot-2.4.7/bale/attachments/location.py
+-rw-rw-rw-   0        0        0     2269 2023-06-26 08:10:29.000000 python-bale-bot-2.4.7/bale/attachments/photo.py
+-rw-rw-rw-   0        0        0     2650 2023-06-26 08:10:29.000000 python-bale-bot-2.4.7/bale/attachments/video.py
+-rw-rw-rw-   0        0        0    46230 2023-07-15 16:19:28.000000 python-bale-bot-2.4.7/bale/bot.py
+-rw-rw-rw-   0        0        0     3964 2023-05-07 15:38:31.000000 python-bale-bot-2.4.7/bale/callbackquery.py
+-rw-rw-rw-   0        0        0    11264 2023-07-15 16:19:28.000000 python-bale-bot-2.4.7/bale/chat.py
+-rw-rw-rw-   0        0        0     3934 2023-04-13 11:25:40.000000 python-bale-bot-2.4.7/bale/chatmember.py
+-rw-rw-rw-   0        0        0     3689 2023-07-15 13:21:48.000000 python-bale-bot-2.4.7/bale/error.py
+-rw-rw-rw-   0        0        0    15721 2023-07-15 16:19:28.000000 python-bale-bot-2.4.7/bale/message.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.011230 python-bale-bot-2.4.7/bale/payments/
+-rw-rw-rw-   0        0        0       56 2023-04-11 12:58:40.000000 python-bale-bot-2.4.7/bale/payments/__init__.py
+-rw-rw-rw-   0        0        0     2131 2023-04-09 22:53:13.000000 python-bale-bot-2.4.7/bale/payments/invoice.py
+-rw-rw-rw-   0        0        0     1733 2023-04-09 22:53:13.000000 python-bale-bot-2.4.7/bale/payments/price.py
+-rw-rw-rw-   0        0        0     4402 2023-04-09 22:53:13.000000 python-bale-bot-2.4.7/bale/permissions.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.095215 python-bale-bot-2.4.7/bale/request/
+-rw-rw-rw-   0        0        0      201 2023-04-09 22:53:13.000000 python-bale-bot-2.4.7/bale/request/__init__.py
+-rw-rw-rw-   0        0        0    11504 2023-07-26 15:37:49.000000 python-bale-bot-2.4.7/bale/request/http.py
+-rw-rw-rw-   0        0        0     1371 2023-07-15 13:52:07.000000 python-bale-bot-2.4.7/bale/request/parser.py
+-rw-rw-rw-   0        0        0      218 2023-07-12 16:25:08.000000 python-bale-bot-2.4.7/bale/request/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.173202 python-bale-bot-2.4.7/bale/ui/
+-rw-rw-rw-   0        0        0      167 2023-06-26 08:08:10.000000 python-bale-bot-2.4.7/bale/ui/__init__.py
+-rw-rw-rw-   0        0        0     4820 2023-06-26 08:20:23.000000 python-bale-bot-2.4.7/bale/ui/components.py
+-rw-rw-rw-   0        0        0     2923 2023-06-20 15:49:07.000000 python-bale-bot-2.4.7/bale/ui/inline_keyboard.py
+-rw-rw-rw-   0        0        0     1739 2023-06-26 08:24:36.000000 python-bale-bot-2.4.7/bale/ui/menu_keyboard.py
+-rw-rw-rw-   0        0        0     6631 2023-04-11 17:56:28.000000 python-bale-bot-2.4.7/bale/update.py
+-rw-rw-rw-   0        0        0     5356 2023-04-29 18:54:30.000000 python-bale-bot-2.4.7/bale/updater.py
+-rw-rw-rw-   0        0        0     6998 2023-07-15 16:19:28.000000 python-bale-bot-2.4.7/bale/user.py
+-rw-rw-rw-   0        0        0      328 2023-08-05 14:55:50.000000 python-bale-bot-2.4.7/bale/utils.py
+-rw-rw-rw-   0        0        0      145 2023-08-03 16:55:34.000000 python-bale-bot-2.4.7/bale/version.py
+drwxrwxrwx   0        0        0        0 2023-08-05 15:02:06.258187 python-bale-bot-2.4.7/python_bale_bot.egg-info/
+-rw-rw-rw-   0        0        0     3082 2023-08-05 15:02:05.000000 python-bale-bot-2.4.7/python_bale_bot.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-08-05 15:02:05.000000 python-bale-bot-2.4.7/python_bale_bot.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 15:02:05.000000 python-bale-bot-2.4.7/python_bale_bot.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      155 2023-08-05 15:02:05.000000 python-bale-bot-2.4.7/python_bale_bot.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-08-05 15:02:05.000000 python-bale-bot-2.4.7/python_bale_bot.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 15:02:06.262188 python-bale-bot-2.4.7/setup.cfg
+-rw-rw-rw-   0        0        0     1771 2023-08-05 14:55:48.000000 python-bale-bot-2.4.7/setup.py
```

### Comparing `python-bale-bot-2.4.6/LICENSE` & `python-bale-bot-2.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/PKG-INFO` & `python-bale-bot-2.4.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: python-bale-bot
-Version: 2.4.6
+Version: 2.4.7
 Summary: An API wrapper for Bale written in Python
 Home-page: https://github.com/python-bale-bot/python-bale-bot/
 Author: Kian Ahmadian
-License: MIT License
-Project-URL: Documentation, https://docs.python-bale-bot.ir/en/master/
-Project-URL: Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html
+Author-email: devs@python-bale-bot.ir
+License: LGPLv2
+Download-URL: https://pypi.org/project/python-bale-bot/
+Project-URL: Documentation, https://docs.python-bale-bot.ir/en/stable/
+Project-URL: Changelog, https:///docs.python-bale-bot.ir/en/stable/whats_new.html
 Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
-Keywords: bale,bale-bot,framework,bot
+Keywords: bale bale-bot framework bot
 Platform: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 # python-bale-bot
 
 <div align='center'>
-<img width="600" src="https://media.discordapp.net/attachments/943584615841554463/1087119645850468352/banner.png?width=691&height=109" alt="python-bale-bot image">
+<img width="600" src="https://python-bale-bot.ir/assets/images/banner.png" alt="python-bale-bot image">
 <br>
 <b style='margin-bottom:20px;'>An API wrapper for Bale written in Python. </b>
 <br>
 
-[![Python Version](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://pypi.org/p/python-bale-bot)
+[![Python Version](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://python.org)
 [![PyPi Version](https://img.shields.io/pypi/v/python-bale-bot?color=blue&label=pypi&style=plastic)](https://pypi.org/p/python-bale-bot)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/deacf2bc3f13492d944e329ac19ac0d1)](https://www.codacy.com/gh/python-bale-bot/python-bale-bot/dashboard)
 [![python-bale-bot score](https://snyk.io/advisor/python/python-bale-bot/badge.svg)](https://snyk.io/advisor/python/python-bale-bot)
-[![Project License](https://img.shields.io/github/license/python-bale-bot/python-bale-bot?style=plastic)](https://opensource.org/licenses/MIT)
+[![Project License](https://img.shields.io/github/license/python-bale-bot/python-bale-bot?style=plastic)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
 [![API Version](https://img.shields.io/badge/Bale%20API-1.0-blue?style=plastic)](https://dev.bale.ai/api)
-[![Documentation Status](https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable)](https://python-bale-bot.rtfd.org/)
+[![Documentation Status](https://readthedocs.org/projects/python-bale-bot/badge/?version=stable)](https://docs.python-bale-bot.ir/)
 
 </div>
 
 ## Installing
 <div align='center'><p><b>You can install or update <code>python-bale-bot</code> via:</b></p></div>
 
 ### PyPi:
@@ -48,15 +50,15 @@
 ```
 $ git clone https://github.com/python-bale-bot/python-bale-bot
 $ cd python-bale-bot
 $ python setup.py install
 ```
 
 ## Documentation
-<p><b>The <a href="https://python-bale-bot.readthedocs.io/en/master">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
+<p><b>The <a href="https://docs.python-bale-bot.ir/en/stable">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
 
 
 ## Contact to Developers
 [![Email](https://img.shields.io/badge/Email-python--bale--bot@googlegroups.com-green?logo=Gmail&logoColor=white)](mailto:python-bale-bot@googlegroups.com)
 [![Discord](https://img.shields.io/badge/Support_Server-bYHEzyDe2j-green?logo=Discord&logoColor=white)](https://discord.gg/bYHEzyDe2j)
 [![Our Site](https://img.shields.io/badge/Our_site-python--bale--bot.ir-green?logo=GitHub&logoColor=white)](https://python-bale-bot.ir)
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.6 Summary: An API
+Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.7 Summary: An API
 wrapper for Bale written in Python Home-page: https://github.com/python-bale-
-bot/python-bale-bot/ Author: Kian Ahmadian License: MIT License Project-URL:
-Documentation, https://docs.python-bale-bot.ir/en/master/ Project-URL:
-Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html Project-
-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
-Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
-Keywords: bale,bale-bot,framework,bot Platform: Windows Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: docs License-File:
-LICENSE # python-bale-bot
+bot/python-bale-bot/ Author: Kian Ahmadian Author-email: devs@python-bale-
+bot.ir License: LGPLv2 Download-URL: https://pypi.org/project/python-bale-bot/
+Project-URL: Documentation, https://docs.python-bale-bot.ir/en/stable/ Project-
+URL: Changelog, https:///docs.python-bale-bot.ir/en/stable/whats_new.html
+Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/
+issues Project-URL: Source Code, https://github.com/python-bale-bot/python-
+bale-bot/ Keywords: bale bale-bot framework bot Platform: Windows Requires-
+Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: docs
+License-File: LICENSE # python-bale-bot
                            [python-bale-bot image]
                   An API wrapper for Bale written in Python.
             [![Python Version](https://img.shields.io/badge/Python-
- 3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://pypi.org/p/
- python-bale-bot) [![PyPi Version](https://img.shields.io/pypi/v/python-bale-
+3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://python.org) [!
+           [PyPi Version](https://img.shields.io/pypi/v/python-bale-
 bot?color=blue&label=pypi&style=plastic)](https://pypi.org/p/python-bale-bot)
          [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
  deacf2bc3f13492d944e329ac19ac0d1)](https://www.codacy.com/gh/python-bale-bot/
  python-bale-bot/dashboard) [![python-bale-bot score](https://snyk.io/advisor/
 python/python-bale-bot/badge.svg)](https://snyk.io/advisor/python/python-bale-
 bot) [![Project License](https://img.shields.io/github/license/python-bale-bot/
-  python-bale-bot?style=plastic)](https://opensource.org/licenses/MIT) [![API
-   Version](https://img.shields.io/badge/Bale%20API-1.0-blue?style=plastic)]
-  (https://dev.bale.ai/api) [![Documentation Status](https://readthedocs.org/
-   projects/python-telegram-bot/badge/?version=stable)](https://python-bale-
-                                bot.rtfd.org/)
+python-bale-bot?style=plastic)](https://www.gnu.org/licenses/old-licenses/gpl-
+   2.0.en.html) [![API Version](https://img.shields.io/badge/Bale%20API-1.0-
+blue?style=plastic)](https://dev.bale.ai/api) [![Documentation Status](https://
+   readthedocs.org/projects/python-bale-bot/badge/?version=stable)](https://
+                           docs.python-bale-bot.ir/)
 ## Installing
                 You can install or update python-bale-bot via:
 ### PyPi: ``` $ pip install python-bale-bot -U ``` ### Git: ``` $ git clone
 https://github.com/python-bale-bot/python-bale-bot $ cd python-bale-bot $
 python setup.py install ``` ## Documentation
 The package_documentation is the technical reference for python-bale-bot. It
 contains descriptions of all available classes, modules, methods and arguments
```

### Comparing `python-bale-bot-2.4.6/README.md` & `python-bale-bot-2.4.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # python-bale-bot
 
 <div align='center'>
-<img width="600" src="https://media.discordapp.net/attachments/943584615841554463/1087119645850468352/banner.png?width=691&height=109" alt="python-bale-bot image">
+<img width="600" src="https://python-bale-bot.ir/assets/images/banner.png" alt="python-bale-bot image">
 <br>
 <b style='margin-bottom:20px;'>An API wrapper for Bale written in Python. </b>
 <br>
 
-[![Python Version](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://pypi.org/p/python-bale-bot)
+[![Python Version](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://python.org)
 [![PyPi Version](https://img.shields.io/pypi/v/python-bale-bot?color=blue&label=pypi&style=plastic)](https://pypi.org/p/python-bale-bot)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/deacf2bc3f13492d944e329ac19ac0d1)](https://www.codacy.com/gh/python-bale-bot/python-bale-bot/dashboard)
 [![python-bale-bot score](https://snyk.io/advisor/python/python-bale-bot/badge.svg)](https://snyk.io/advisor/python/python-bale-bot)
-[![Project License](https://img.shields.io/github/license/python-bale-bot/python-bale-bot?style=plastic)](https://opensource.org/licenses/MIT)
+[![Project License](https://img.shields.io/github/license/python-bale-bot/python-bale-bot?style=plastic)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
 [![API Version](https://img.shields.io/badge/Bale%20API-1.0-blue?style=plastic)](https://dev.bale.ai/api)
-[![Documentation Status](https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable)](https://python-bale-bot.rtfd.org/)
+[![Documentation Status](https://readthedocs.org/projects/python-bale-bot/badge/?version=stable)](https://docs.python-bale-bot.ir/)
 
 </div>
 
 ## Installing
 <div align='center'><p><b>You can install or update <code>python-bale-bot</code> via:</b></p></div>
 
 ### PyPi:
@@ -30,14 +30,14 @@
 ```
 $ git clone https://github.com/python-bale-bot/python-bale-bot
 $ cd python-bale-bot
 $ python setup.py install
 ```
 
 ## Documentation
-<p><b>The <a href="https://python-bale-bot.readthedocs.io/en/master">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
+<p><b>The <a href="https://docs.python-bale-bot.ir/en/stable">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
 
 
 ## Contact to Developers
 [![Email](https://img.shields.io/badge/Email-python--bale--bot@googlegroups.com-green?logo=Gmail&logoColor=white)](mailto:python-bale-bot@googlegroups.com)
 [![Discord](https://img.shields.io/badge/Support_Server-bYHEzyDe2j-green?logo=Discord&logoColor=white)](https://discord.gg/bYHEzyDe2j)
 [![Our Site](https://img.shields.io/badge/Our_site-python--bale--bot.ir-green?logo=GitHub&logoColor=white)](https://python-bale-bot.ir)
```

#### html2text {}

```diff
@@ -1,24 +1,24 @@
 # python-bale-bot
                            [python-bale-bot image]
                   An API wrapper for Bale written in Python.
             [![Python Version](https://img.shields.io/badge/Python-
- 3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://pypi.org/p/
- python-bale-bot) [![PyPi Version](https://img.shields.io/pypi/v/python-bale-
+3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://python.org) [!
+           [PyPi Version](https://img.shields.io/pypi/v/python-bale-
 bot?color=blue&label=pypi&style=plastic)](https://pypi.org/p/python-bale-bot)
          [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
  deacf2bc3f13492d944e329ac19ac0d1)](https://www.codacy.com/gh/python-bale-bot/
  python-bale-bot/dashboard) [![python-bale-bot score](https://snyk.io/advisor/
 python/python-bale-bot/badge.svg)](https://snyk.io/advisor/python/python-bale-
 bot) [![Project License](https://img.shields.io/github/license/python-bale-bot/
-  python-bale-bot?style=plastic)](https://opensource.org/licenses/MIT) [![API
-   Version](https://img.shields.io/badge/Bale%20API-1.0-blue?style=plastic)]
-  (https://dev.bale.ai/api) [![Documentation Status](https://readthedocs.org/
-   projects/python-telegram-bot/badge/?version=stable)](https://python-bale-
-                                bot.rtfd.org/)
+python-bale-bot?style=plastic)](https://www.gnu.org/licenses/old-licenses/gpl-
+   2.0.en.html) [![API Version](https://img.shields.io/badge/Bale%20API-1.0-
+blue?style=plastic)](https://dev.bale.ai/api) [![Documentation Status](https://
+   readthedocs.org/projects/python-bale-bot/badge/?version=stable)](https://
+                           docs.python-bale-bot.ir/)
 ## Installing
                 You can install or update python-bale-bot via:
 ### PyPi: ``` $ pip install python-bale-bot -U ``` ### Git: ``` $ git clone
 https://github.com/python-bale-bot/python-bale-bot $ cd python-bale-bot $
 python setup.py install ``` ## Documentation
 The package_documentation is the technical reference for python-bale-bot. It
 contains descriptions of all available classes, modules, methods and arguments
```

### Comparing `python-bale-bot-2.4.6/bale/__init__.py` & `python-bale-bot-2.4.7/bale/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 from .version import __version__
 from .request import HTTPClient, Route, ResponseStatusCode, ResponseParser
 from .ui import InlineKeyboard, MenuKeyboard, RemoveMenuKeyboard, Components
-from .attachments import File, Audio, ContactMessage, Location, Photo, Document, Video
+from .attachments import File, Audio, ContactMessage, Location, Photo, Document, Video, InputFile
 from .payments import Price, Invoice
 from .user import User
 from .attachments.contact import ContactMessage
 from .chat import Chat, ChatType
 from .message import Message
 from .permissions import Permissions
 from .chatmember import ChatMember, ChatMemberStatus
```

### Comparing `python-bale-bot-2.4.6/bale/attachments/audio.py` & `python-bale-bot-2.4.7/bale/attachments/audio.py`

 * *Files 17% similar despite different names*

```diff
@@ -54,9 +54,9 @@
         super().__init__(self.__FILE_TYPE__, file_id, file_size, mime_type, bot, duration=duration, title=title)
 
         self.duration = duration
         self.title = title
 
     @classmethod
     def from_dict(cls, data, bot: "Bot"):
-        return cls(file_id=data["file_id"], duration=data["duration"], file_size=data["file_size"], title=data["title"],
-                   mime_type=data["mime_type"], bot=bot)
+        return cls(file_id=data.get("file_id"), duration=data.get("duration"), file_size=data.get("file_size"), title=data.get("title"),
+                   mime_type=data.get("mime_type"), bot=bot)
```

### Comparing `python-bale-bot-2.4.6/bale/attachments/contact.py` & `python-bale-bot-2.4.7/bale/attachments/contact.py`

 * *Files 9% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     def __init__(self, phone_number: int, first_name: str = None, last_name: str = None):
         self.phone_number = phone_number
         self.first_name = first_name
         self.last_name = last_name
 
     @classmethod
     def from_dict(cls, data: dict):
-        return cls(first_name=data["first_name"], last_name=data["last_name"], phone_number=data["phone_number"])
+        return cls(first_name=data.get("first_name"), last_name=data.get("last_name"), phone_number=data.get("phone_number"))
 
     def to_dict(self):
         data = {"phone_number": self.phone_number, "first_name": self.first_name, "last_name": self.last_name}
 
         return data
 
     def __eq__(self, other):
```

### Comparing `python-bale-bot-2.4.6/bale/attachments/document.py` & `python-bale-bot-2.4.7/bale/attachments/document.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/attachments/file.py` & `python-bale-bot-2.4.7/bale/attachments/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
-from typing import TYPE_CHECKING, NoReturn
+from typing import TYPE_CHECKING, NoReturn, Optional
 from io import BufferedIOBase
 
 if TYPE_CHECKING:
     from bale import Bot
 
 
 class File:
@@ -52,15 +52,15 @@
         "file_type",
         "file_id",
         "file_size",
         "mime_type",
         "extra",
         "bot"
     )
-    def __init__(self, file_type, file_id, file_size, mime_type, bot: "Bot", **kwargs):
+    def __init__(self, file_type: str, file_id: str, file_size: Optional[int], mime_type: Optional[str], bot: "Bot", **kwargs):
         self.file_type = file_type
         self.file_id = file_id
         self.file_size = file_size
         self.mime_type = mime_type
         self.extra = kwargs
         self.bot = bot
```

### Comparing `python-bale-bot-2.4.6/bale/attachments/location.py` & `python-bale-bot-2.4.7/bale/attachments/location.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/attachments/photo.py` & `python-bale-bot-2.4.7/bale/attachments/photo.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/attachments/video.py` & `python-bale-bot-2.4.7/bale/attachments/video.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/bot.py` & `python-bale-bot-2.4.7/bale/bot.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 """
 from __future__ import annotations
 import asyncio
 from typing import Callable, Dict, Tuple, List, Optional
 from builtins import enumerate, reversed
 from .error import NotFound, InvalidToken
 from bale import (Message, Update, User, Components, RemoveMenuKeyboard, Chat, Price, ChatMember, HTTPClient, Updater,
-                  Photo, Document, Location, ContactMessage, Video, Audio)
+                  Photo, Document, Location, ContactMessage, Video, Audio, InputFile)
 
 __all__ = (
     "Bot"
 )
 
 
 class _Loop:
@@ -69,15 +69,15 @@
         "http",
         "_closed",
         "updater"
     )
 
     def __init__(self, token: str, **kwargs):
         if not isinstance(token, str):
-            raise InvalidToken("token must be type of the str")
+            raise InvalidToken()
         self.loop = _loop
         self.token = token
         self.http: HTTPClient = HTTPClient(self.loop, token)
         self._user = None
         self.events: Dict[str, List[Callable]] = {}
         self.listeners: Dict[str, List[Tuple[asyncio.Future, Callable[..., bool]]]] = {}
         self._closed = False
@@ -327,26 +327,29 @@
                 "message_id param must be type of str or int"
             )
 
         response = await self.http.forward_message(str(chat_id), str(from_chat_id), str(message_id))
         return Message.from_dict(data=response.result, bot=self)
 
     async def send_document(self, chat_id: str | int, document: bytes | str | "Document", *,
+                            file_name: Optional[str] = None,
                             caption: Optional[str] = None,
                             reply_to_message_id: Optional[str | int] = None) -> "Message":
         """This service is used to send document.
 
         Parameters
         ----------
         chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
         document: :class:`bytes` | :class:`str` | :class:`bale.Document`
-            File to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
+                File to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
+        file_name: :class:`str`
+                Additional interface options. file name to send.
         caption: Optional[:class:`str`]
-            Document caption.
+                Document caption.
         reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
             :class:`bale.Message`
                 The Message.
@@ -366,36 +369,53 @@
             )
 
         if not isinstance(document, (bytes, str, Document)):
             raise TypeError(
                 "document param must be type of bytes, str or Document"
             )
 
+        if file_name:
+            if not isinstance(file_name, str):
+                raise TypeError(
+                    "file_name param must be type of str"
+                )
+            if isinstance(document, (str, Document)):
+                raise TypeError(
+                    "file_name param should only be used when you are uploading a file!"
+                )
+
         if reply_to_message_id and not isinstance(reply_to_message_id, Message):
             raise TypeError(
                 "reply_to_message_id param must be type of Message"
             )
 
+        if caption and not isinstance(caption, str):
+            raise TypeError(
+                "caption param must be type of str"
+            )
+
         if isinstance(document, Document):
             document = document.file_id
 
-        response = await self.http.send_document(chat_id, document, caption=caption,
+        response = await self.http.send_document(chat_id, [InputFile('document', file_name, document).to_file_form_payload()], caption=caption,
                                                  reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_photo(self, chat_id: str | int, photo: bytes | str | "Photo", *, caption: Optional[str] = None,
+    async def send_photo(self, chat_id: str | int, photo: bytes | str | "Photo", *, file_name: Optional[str] = None, caption: Optional[str] = None,
                          reply_to_message_id: Optional[str | int] = None) -> "Message":
         """This service is used to send photo.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             photo: :class:`bytes` | :class:`str` | :class:`bale.Photo`
                 Photo to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
+            file_name: :class:`str`
+                Additional interface options. file name to send.
             caption: Optional[:class:`str`]
                 Photo caption.
             reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
@@ -420,38 +440,50 @@
             raise TypeError(
                 "photo param must be type of bytes, str or Photo"
             )
 
         if isinstance(photo, Photo):
             photo = photo.file_id
 
+        if file_name:
+            if not isinstance(file_name, str):
+                raise TypeError(
+                    "file_name param must be type of str"
+                )
+            if isinstance(photo, (str, Photo)):
+                raise TypeError(
+                    "file_name param should only be used when you are uploading a file!"
+                )
+
         if reply_to_message_id and not isinstance(reply_to_message_id, (str, int)):
             raise TypeError(
                 "reply_to_message_id param must be type of str or int"
             )
 
         if caption and not isinstance(caption, str):
             raise TypeError(
                 "caption param must be type of str"
             )
 
-        response = await self.http.send_photo(str(chat_id), photo, caption=caption,
+        response = await self.http.send_photo(str(chat_id), [InputFile('photo', file_name, photo).to_file_form_payload()], caption=caption,
                                               reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_audio(self, chat_id: str | int, audio: bytes | str | "Audio", *, caption: Optional[str] = None,
+    async def send_audio(self, chat_id: str | int, audio: bytes | str | "Audio", *, file_name: Optional[str] = None, caption: Optional[str] = None,
                          reply_to_message_id: Optional[str | int] = None) -> "Message":
         """This service is used to send Audio.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             audio: :class:`bytes` | :class:`str` | :class:`bale.Audio`
                 Audio file to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
+            file_name: :class:`str`
+                Additional interface options. file name to send.
             caption: Optional[:class:`str`]
                 Audio caption.
             reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
@@ -476,38 +508,50 @@
             raise TypeError(
                 "audio param must be type of bytes, str or Audio"
             )
 
         if isinstance(audio, Audio):
             audio = audio.file_id
 
+        if file_name:
+            if not isinstance(file_name, str):
+                raise TypeError(
+                    "file_name param must be type of str"
+                )
+            if isinstance(audio, (str, Audio)):
+                raise TypeError(
+                    "file_name param should only be used when you are uploading a file!"
+                )
+
         if reply_to_message_id and not isinstance(reply_to_message_id, (str, int)):
             raise TypeError(
                 "reply_to_message_id param must be type of str or int"
             )
 
         if caption and not isinstance(caption, str):
             raise TypeError(
                 "caption param must be type of str"
             )
 
-        response = await self.http.send_audio(str(chat_id), audio, caption=caption,
+        response = await self.http.send_audio(str(chat_id), [InputFile('audio', file_name, audio).to_file_form_payload()], caption=caption,
                                               reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
-    async def send_video(self, chat_id: str | int, video: bytes | str | "Photo", *, caption: Optional[str] = None,
+    async def send_video(self, chat_id: str | int, video: bytes | str | "Photo", *, file_name: Optional[str] = None, caption: Optional[str] = None,
                          reply_to_message_id: Optional[str | int] = None) -> "Message":
         """This service is used to send Video.
 
         Parameters
         ----------
             chat_id: :class:`str` | :class:`int`
                 Unique identifier for the target chat or username of the target channel (in the format @channelusername).
             video: :class:`bytes` | :class:`str` | :class:`bale.Photo`
                 Video to send. Pass a file_id as String to send a file that exists on the Bale servers (recommended), pass an HTTP URL as a String for Bale to get a file from the Internet, or upload a new one.
+            file_name: :class:`str`
+                Additional interface options. file name to send.
             caption: Optional[:class:`str`]
                 Video caption.
             reply_to_message_id: Optional[:class:`str` | :class:`int`]
                 Additional interface options. An object for an inline keyboard, custom reply keyboard, instructions to remove reply keyboard or to force a reply from the user.
 
         Returns
         --------
@@ -532,25 +576,35 @@
             raise TypeError(
                 "video param must be type of bytes, str or Video"
             )
 
         if isinstance(video, Video):
             video = video.file_id
 
+        if file_name:
+            if not isinstance(file_name, str):
+                raise TypeError(
+                    "file_name param must be type of str"
+                )
+            if isinstance(video, (str, Video)):
+                raise TypeError(
+                    "file_name param should only be used when you are uploading a file!"
+                )
+
         if reply_to_message_id and not isinstance(reply_to_message_id, (str, int)):
             raise TypeError(
                 "reply_to_message_id param must be type of str or int"
             )
 
         if caption and not isinstance(caption, str):
             raise TypeError(
                 "caption param must be type of str"
             )
 
-        response = await self.http.send_video(str(chat_id), video, caption=caption,
+        response = await self.http.send_video(str(chat_id), [InputFile('video', file_name, video).to_file_form_payload()], caption=caption,
                                               reply_to_message_id=reply_to_message_id)
         return Message.from_dict(data=response.result, bot=self)
 
     async def send_location(self, chat_id: str | int, location: "Location") -> "Message":
         """Use this method to send point on the map.
 
         Parameters
```

### Comparing `python-bale-bot-2.4.6/bale/callbackquery.py` & `python-bale-bot-2.4.7/bale/callbackquery.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/chat.py` & `python-bale-bot-2.4.7/bale/chat.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,37 +144,37 @@
 
     async def send(self, text: str, components: Optional["Components" | "RemoveMenuKeyboard"] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_message`.
         """
         return await self.bot.send_message(self.chat_id, text, components=components)
 
-    async def send_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
+    async def send_document(self, document: bytes | str | "Document", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_document`.
         """
-        return await self.bot.send_document(self.chat_id, document, caption=caption)
+        return await self.bot.send_document(self.chat_id, document, file_name=file_name, caption=caption)
 
-    async def send_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
+    async def send_photo(self, photo: bytes | str | "Photo", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
         """
-        return await self.bot.send_photo(self.chat_id, photo, caption=caption)
+        return await self.bot.send_photo(self.chat_id, photo, file_name=file_name, caption=caption)
 
-    async def send_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
+    async def send_video(self, video: bytes | str | "Video", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
         """
-        return await self.bot.send_video(self.chat_id, video, caption=caption)
+        return await self.bot.send_video(self.chat_id, video, file_name=file_name, caption=caption)
 
-    async def send_audio(self, audio: bytes | str | "Audio", *, caption: Optional[str] = None):
+    async def send_audio(self, audio: bytes | str | "Audio", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_audio`.
         """
-        return await self.bot.send_audio(self.chat_id, audio, caption=caption)
+        return await self.bot.send_audio(self.chat_id, audio, file_name=file_name, caption=caption)
 
     async def send_location(self, location: "Location"):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_location`.
         """
         return await self.bot.send_location(self.chat_id, location)
```

### Comparing `python-bale-bot-2.4.6/bale/chatmember.py` & `python-bale-bot-2.4.7/bale/chatmember.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/error.py` & `python-bale-bot-2.4.7/bale/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
 class HTTPClientError:
     USER_OR_CHAT_NOT_FOUND = "no such group or user"
+    TOKEN_NOT_FOUND = "Token not found"
     RATE_LIMIT = "bot limit exceed"
     LOCAL_RATE_LIMIT = "local_rate_limited"
     PERMISSION_DENIED = "permission_denied"
 
 class BaleError(Exception):
     """
     Base exception class for python-bale-bot
@@ -56,18 +57,16 @@
 
 class InvalidToken(BaleError):
     """
     An exception where the server says the Token is Invalid
     """
     __slots__ = ("_message",)
 
-    def __init__(self, message):
-        self._message = message
-
-        super().__init__("Invalid Token" if self._message is not None else self._message)
+    def __init__(self):
+        super().__init__("Invalid Token")
 
 
 class APIError(BaleError):
     """
     Exception that's raised for when status code 400 occurs and Error is Unknown.
     Subclass of :exc:`BaleError`
     """
```

### Comparing `python-bale-bot-2.4.6/bale/message.py` & `python-bale-bot-2.4.7/bale/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -233,40 +233,44 @@
 
     async def forward(self, chat_id: str | int):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.forward_message`.
         """
         return await self.bot.forward_message(chat_id, self.chat_id, self.message_id)
 
-    async def reply_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
+    async def reply_document(self, document: bytes | str | "Document", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_document`.
         """
         return await self.bot.send_document(self.chat_id, document, caption=caption,
+                                            file_name=file_name,
                                             reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def reply_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
+    async def reply_photo(self, photo: bytes | str | "Photo", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
         """
         return await self.bot.send_photo(self.chat_id, photo, caption=caption,
+                                         file_name=file_name,
                                          reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def reply_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
+    async def reply_video(self, video: bytes | str | "Video", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
         """
         return await self.bot.send_video(self.chat_id, video, caption=caption,
+                                         file_name=file_name,
                                          reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
-    async def reply_audio(self, audio: bytes | str | "Audio", *, caption: Optional[str] = None):
+    async def reply_audio(self, audio: bytes | str | "Audio", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_audio`.
         """
         return await self.bot.send_video(self.chat_id, audio, caption=caption,
+                                         file_name=file_name,
                                          reply_to_message_id=self.message_id if not self.chat.type.is_group_chat() else None)
 
     async def edit(self, text: str, *, components: "Components" | "RemoveMenuKeyboard" = None) -> Message:
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.edit_message`
         """
         return await self.bot.edit_message(self.chat_id, self.message_id, text, components=components)
```

### Comparing `python-bale-bot-2.4.6/bale/payments/invoice.py` & `python-bale-bot-2.4.7/bale/payments/invoice.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/payments/price.py` & `python-bale-bot-2.4.7/bale/payments/price.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/permissions.py` & `python-bale-bot-2.4.7/bale/permissions.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/request/http.py` & `python-bale-bot-2.4.7/bale/request/http.py`

 * *Files 11% similar despite different names*

```diff
@@ -17,20 +17,21 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 """
+from typing import Dict, List
 from bale.version import BALE_API_BASE_URL, BALE_API_FILE_URL
 import asyncio
 import aiohttp
-from ..error import (NetworkError, TimeOut, NotFound, Forbidden, APIError, BaleError, HTTPClientError, RateLimited, HTTPException)
+from ..error import (NetworkError, TimeOut, NotFound, Forbidden, APIError, BaleError, HTTPClientError, RateLimited, HTTPException, InvalidToken)
 from .parser import ResponseParser
-from .utils import ResponseStatusCode
+from .utils import ResponseStatusCode, to_json
 
 __all__ = ("HTTPClient", "Route")
 
 class Route:
 	"""Route Class for http"""
 	__slots__ = (
 		"method",
@@ -60,14 +61,18 @@
 	)
 
 	def __init__(self, loop, token):
 		self.__session = None
 		self._loop: asyncio.AbstractEventLoop = loop
 		self.token = token
 
+	@property
+	def user_agent(self) -> str:
+		return "python-bale-bot (https://python-bale-bot.ir): An API wrapper for Bale written in Python"
+
 	def is_closed(self):
 		return self.__session is None
 
 	@property
 	def loop(self):
 		return self._loop
 
@@ -88,17 +93,37 @@
 
 	async def close(self):
 		"""Close Session connection"""
 		if self.__session:
 			await self.__session.close()
 			self.__session = None
 
-	async def request(self, route: Route, **kwargs):
+	async def request(self, route: Route, *, form: List[Dict] = None, **kwargs):
 		url = route.url
 		method = route.method
+		headers = { 'User-Agent': self.user_agent }
+
+		if 'json' in kwargs:
+			headers['Content-Type'] = 'application/json'
+			kwargs['data'] = to_json(kwargs.pop('json'))
+
+
+		if form:
+			form_data = aiohttp.FormData()
+			for file_payload in form:
+				form_data.add_field(**file_payload, content_type= "multipart/form-data")
+			if 'data' in kwargs:
+				_data = kwargs.pop('data')
+				for param in _data:
+					form_data.add_field(param, _data[param])
+
+			kwargs['data'] = form_data
+
+		kwargs['headers'] = headers
+
 		for tries in range(5):
 			try:
 				async with self.__session.request(method=method, url=url, **kwargs) as response:
 					response: aiohttp.ClientResponse = response
 					parsed_response = await ResponseParser.from_response(response)
 					if response.status == ResponseStatusCode.OK:
 						return parsed_response
@@ -113,14 +138,16 @@
 							if tries >= 4:
 								raise RateLimited()
 
 							await asyncio.sleep((1 + tries) * 2)
 							continue
 						elif parsed_response.description == HTTPClientError.PERMISSION_DENIED:
 							raise Forbidden()
+						elif parsed_response.description == HTTPClientError.TOKEN_NOT_FOUND:
+							raise InvalidToken()
 
 						raise APIError(
 								str(parsed_response.error_code), parsed_response.description
 							)
 			except aiohttp.ClientConnectorError as error:
 				raise NetworkError(str(error))
 			except aiohttp.ServerTimeoutError:
@@ -161,77 +188,73 @@
 			"chat_id": chat_id,
 			"from_chat_id": from_chat_id,
 			"message_id": message_id
 		}
 
 		return self.request(Route("POST", "forwardMessage", self.token), json=payload)
 
-	def send_document(self, chat_id, document, *, caption=None, reply_to_message_id=None):
+	def send_document(self, chat_id, form, *, caption=None, reply_to_message_id=None):
 		payload = {
-			"chat_id": chat_id,
-			"document": document
+			"chat_id": chat_id
 		}
 		if caption:
 			payload["caption"] = caption
 
 		if reply_to_message_id:
 			payload["reply_to_message_id"] = reply_to_message_id
 
-		return self.request(Route("POST", "Senddocument", self.token), data=payload)
+		return self.request(Route("POST", "sendDocument", self.token), data=payload, form=form)
 
-	def send_photo(self, chat_id, photo, *, caption=None, reply_to_message_id=None):
+	def send_photo(self, chat_id, form, *, caption=None, reply_to_message_id=None):
 		payload = {
-			"chat_id": chat_id,
-			"photo": photo
+			"chat_id": chat_id
 		}
 		if caption:
 			payload["caption"] = caption
 		if reply_to_message_id:
 			payload["reply_to_message_id"] = reply_to_message_id
 
-		return self.request(Route("POST", "SendPhoto", self.token), data=payload)
+		return self.request(Route("POST", "SendPhoto", self.token), data=payload, form=form)
 
-	def send_video(self, chat_id, video, *, caption=None, reply_to_message_id=None):
+	def send_video(self, chat_id, form, *, caption=None, reply_to_message_id=None):
 		payload = {
-			"chat_id": chat_id,
-			"video": video
+			"chat_id": chat_id
 		}
 		if caption:
 			payload["caption"] = caption
 		if reply_to_message_id:
 			payload["reply_to_message_id"] = reply_to_message_id
 
-		return self.request(Route("POST", "sendVideo", self.token), data=payload)
+		return self.request(Route("POST", "sendVideo", self.token), data=payload, form=form)
 
-	def send_audio(self, chat_id, audio, *, caption=None, duration=None, title=None, reply_to_message_id=None):
+	def send_audio(self, chat_id, form, *, caption=None, duration=None, title=None, reply_to_message_id=None):
 		payload = {
-			"chat_id": chat_id,
-			"audio": audio
+			"chat_id": chat_id
 		}
 		if caption:
 			payload["caption"] = caption
 		if duration:
 			payload["duration"] = duration
 		if title:
 			payload["title"] = title
 		if reply_to_message_id:
 			payload["reply_to_message_id"] = reply_to_message_id
 
-		return self.request(Route("POST", "SendAudio", self.token), data=payload)
+		return self.request(Route("POST", "SendAudio", self.token), data=payload, form=form)
 
 	def send_contact(self, chat_id, phone_number, first_name, *, last_name):
 		payload = {
 			"chat_id": chat_id,
 			"phone_number": phone_number,
 			"first_name": first_name
 		}
 		if last_name:
 			payload["last_name"] = last_name
 
-		return self.request(Route("POST", "SendContact", self.token), data=payload)
+		return self.request(Route("POST", "sendContact", self.token), data=payload)
 
 	def send_invoice(self, chat_id, title, description, provider_token, prices, photo_url=None, need_name=False, need_phone_number=False, need_email=False, need_shipping_address=False, is_flexible=True):
 		payload = {"chat_id": chat_id, "title": title, "description": description, "provider_token": provider_token, "prices": prices}
 		if photo_url:
 			payload["photo_url"] = photo_url
 		payload["need_name"] = need_name
 		payload["need_phone_number"] = need_phone_number
@@ -258,43 +281,43 @@
 		return self.request(Route("POST", "editMessageText", self.token), json=payload)
 
 	def delete_message(self, chat_id, message_id):
 		payload = {
 			"chat_id": chat_id,
 			"message_id": message_id
 		}
-		return self.request(Route("GET", "deletemessage", self.token), params=payload)
+		return self.request(Route("GET", "deleteMessage", self.token), json=payload)
 
 	def get_updates(self, offset=None, limit=None):
 		payload = {}
 		if offset:
 			payload["offset"] = offset
 		if limit:
 			payload["limit"] = limit
-		return self.request(Route("POST", "getupdates", self.token), json=payload)
+		return self.request(Route("POST", "getUpdates", self.token), json=payload)
 
 	def delete_webhook(self):
 		return self.request(Route("GET", "deleteWebhook", self.token))
 
 	def get_bot(self):
-		return self.request(Route("GET", "getme", self.token))
+		return self.request(Route("GET", "getMe", self.token))
 
 	def get_chat(self, chat_id):
-		return self.request(Route("GET", "getchat", self.token), params=dict(chat_id=chat_id))
+		return self.request(Route("GET", "getChat", self.token), json=dict(chat_id=chat_id))
 
 	def leave_chat(self, chat_id):
-		return self.request(Route("GET", "leaveChat", self.token), params=dict(chat_id=chat_id))
+		return self.request(Route("GET", "leaveChat", self.token), json=dict(chat_id=chat_id))
 
 	def get_chat_administrators(self, chat_id):
-		return self.request(Route("GET", "getChatAdministrators", self.token), params=dict(chat_id=chat_id))
+		return self.request(Route("GET", "getChatAdministrators", self.token), json=dict(chat_id=chat_id))
 
 	def get_chat_members_count(self, chat_id):
-		return self.request(Route("GET", "getChatMemberCount", self.token), params=dict(chat_id=chat_id))
+		return self.request(Route("GET", "getChatMemberCount", self.token), json=dict(chat_id=chat_id))
 
 	def get_chat_member(self, chat_id, member_id):
-		return self.request(Route("GET", "getChatMember", self.token), params=dict(chat_id=chat_id, user_id=member_id))
+		return self.request(Route("GET", "getChatMember", self.token), json=dict(chat_id=chat_id, user_id=member_id))
 
 	def ban_chat_member(self, chat_id, member_id):
-		return self.request(Route("POST", "banChatMember", self.token), params=dict(chat_id=chat_id, user_id=member_id))
+		return self.request(Route("POST", "banChatMember", self.token), json=dict(chat_id=chat_id, user_id=member_id))
 
 	def invite_to_chat(self, chat_id, user_id):
-		return self.request(Route("GET", "InviteUser", self.token), json=dict(chat_id=chat_id, user_id=user_id))
+		return self.request(Route("GET", "inviteUser", self.token), json=dict(chat_id=chat_id, user_id=user_id))
```

### Comparing `python-bale-bot-2.4.6/bale/request/parser.py` & `python-bale-bot-2.4.7/bale/request/parser.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/ui/components.py` & `python-bale-bot-2.4.7/bale/ui/components.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/ui/inline_keyboard.py` & `python-bale-bot-2.4.7/bale/ui/inline_keyboard.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/ui/menu_keyboard.py` & `python-bale-bot-2.4.7/bale/ui/menu_keyboard.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/update.py` & `python-bale-bot-2.4.7/bale/update.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/updater.py` & `python-bale-bot-2.4.7/bale/updater.py`

 * *Files identical despite different names*

### Comparing `python-bale-bot-2.4.6/bale/user.py` & `python-bale-bot-2.4.7/bale/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -73,37 +73,37 @@
 
     async def send(self, text: str, components: Optional["Components" | "RemoveMenuKeyboard"] =None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_message`.
         """
         return await self.bot.send_message(self.chat_id, text, components=components)
 
-    async def send_document(self, document: bytes | str | "Document", *, caption: Optional[str] = None):
+    async def send_document(self, document: bytes | str | "Document", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_document`.
         """
-        return await self.bot.send_document(self.chat_id, document, caption=caption)
+        return await self.bot.send_document(self.chat_id, document, file_name=file_name, caption=caption)
 
-    async def send_photo(self, photo: bytes | str | "Photo", *, caption: Optional[str] = None):
+    async def send_photo(self, photo: bytes | str | "Photo", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_photo`.
         """
-        return await self.bot.send_photo(self.chat_id, photo, caption=caption)
+        return await self.bot.send_photo(self.chat_id, photo, file_name=file_name, caption=caption)
 
-    async def send_video(self, video: bytes | str | "Video", *, caption: Optional[str] = None):
+    async def send_video(self, video: bytes | str | "Video", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_video`.
         """
-        return await self.bot.send_video(self.chat_id, video, caption=caption)
+        return await self.bot.send_video(self.chat_id, video, file_name=file_name, caption=caption)
 
-    async def send_audio(self, audio: bytes | str | "Audio", *, caption: Optional[str] = None):
+    async def send_audio(self, audio: bytes | str | "Audio", *, file_name: Optional[str] = None, caption: Optional[str] = None):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_audio`.
         """
-        return await self.bot.send_audio(self.chat_id, audio, caption=caption)
+        return await self.bot.send_audio(self.chat_id, audio, file_name=file_name, caption=caption)
 
     async def send_location(self, location: "Location"):
         """
         For the documentation of the arguments, please see :meth:`bale.Bot.send_location`.
         """
         return await self.bot.send_location(self.chat_id, location)
```

### Comparing `python-bale-bot-2.4.6/python_bale_bot.egg-info/PKG-INFO` & `python-bale-bot-2.4.7/python_bale_bot.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 Metadata-Version: 2.1
 Name: python-bale-bot
-Version: 2.4.6
+Version: 2.4.7
 Summary: An API wrapper for Bale written in Python
 Home-page: https://github.com/python-bale-bot/python-bale-bot/
 Author: Kian Ahmadian
-License: MIT License
-Project-URL: Documentation, https://docs.python-bale-bot.ir/en/master/
-Project-URL: Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html
+Author-email: devs@python-bale-bot.ir
+License: LGPLv2
+Download-URL: https://pypi.org/project/python-bale-bot/
+Project-URL: Documentation, https://docs.python-bale-bot.ir/en/stable/
+Project-URL: Changelog, https:///docs.python-bale-bot.ir/en/stable/whats_new.html
 Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
 Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
-Keywords: bale,bale-bot,framework,bot
+Keywords: bale bale-bot framework bot
 Platform: Windows
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
 
 # python-bale-bot
 
 <div align='center'>
-<img width="600" src="https://media.discordapp.net/attachments/943584615841554463/1087119645850468352/banner.png?width=691&height=109" alt="python-bale-bot image">
+<img width="600" src="https://python-bale-bot.ir/assets/images/banner.png" alt="python-bale-bot image">
 <br>
 <b style='margin-bottom:20px;'>An API wrapper for Bale written in Python. </b>
 <br>
 
-[![Python Version](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://pypi.org/p/python-bale-bot)
+[![Python Version](https://img.shields.io/badge/Python-3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://python.org)
 [![PyPi Version](https://img.shields.io/pypi/v/python-bale-bot?color=blue&label=pypi&style=plastic)](https://pypi.org/p/python-bale-bot)
 [![Codacy Badge](https://app.codacy.com/project/badge/Grade/deacf2bc3f13492d944e329ac19ac0d1)](https://www.codacy.com/gh/python-bale-bot/python-bale-bot/dashboard)
 [![python-bale-bot score](https://snyk.io/advisor/python/python-bale-bot/badge.svg)](https://snyk.io/advisor/python/python-bale-bot)
-[![Project License](https://img.shields.io/github/license/python-bale-bot/python-bale-bot?style=plastic)](https://opensource.org/licenses/MIT)
+[![Project License](https://img.shields.io/github/license/python-bale-bot/python-bale-bot?style=plastic)](https://www.gnu.org/licenses/old-licenses/gpl-2.0.en.html)
 [![API Version](https://img.shields.io/badge/Bale%20API-1.0-blue?style=plastic)](https://dev.bale.ai/api)
-[![Documentation Status](https://readthedocs.org/projects/python-telegram-bot/badge/?version=stable)](https://python-bale-bot.rtfd.org/)
+[![Documentation Status](https://readthedocs.org/projects/python-bale-bot/badge/?version=stable)](https://docs.python-bale-bot.ir/)
 
 </div>
 
 ## Installing
 <div align='center'><p><b>You can install or update <code>python-bale-bot</code> via:</b></p></div>
 
 ### PyPi:
@@ -48,15 +50,15 @@
 ```
 $ git clone https://github.com/python-bale-bot/python-bale-bot
 $ cd python-bale-bot
 $ python setup.py install
 ```
 
 ## Documentation
-<p><b>The <a href="https://python-bale-bot.readthedocs.io/en/master">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
+<p><b>The <a href="https://docs.python-bale-bot.ir/en/stable">package documentation</a> is the technical reference for python-bale-bot. It contains descriptions of all available classes, modules, methods and arguments as well as the changelog.</b></p>
 
 
 ## Contact to Developers
 [![Email](https://img.shields.io/badge/Email-python--bale--bot@googlegroups.com-green?logo=Gmail&logoColor=white)](mailto:python-bale-bot@googlegroups.com)
 [![Discord](https://img.shields.io/badge/Support_Server-bYHEzyDe2j-green?logo=Discord&logoColor=white)](https://discord.gg/bYHEzyDe2j)
 [![Our Site](https://img.shields.io/badge/Our_site-python--bale--bot.ir-green?logo=GitHub&logoColor=white)](https://python-bale-bot.ir)
```

#### html2text {}

```diff
@@ -1,33 +1,34 @@
-Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.6 Summary: An API
+Metadata-Version: 2.1 Name: python-bale-bot Version: 2.4.7 Summary: An API
 wrapper for Bale written in Python Home-page: https://github.com/python-bale-
-bot/python-bale-bot/ Author: Kian Ahmadian License: MIT License Project-URL:
-Documentation, https://docs.python-bale-bot.ir/en/master/ Project-URL:
-Changelog, https:///docs.python-bale-bot.ir/en/master/whats_new.html Project-
-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/issues
-Project-URL: Source Code, https://github.com/python-bale-bot/python-bale-bot/
-Keywords: bale,bale-bot,framework,bot Platform: Windows Requires-Python: >=3.8
-Description-Content-Type: text/markdown Provides-Extra: docs License-File:
-LICENSE # python-bale-bot
+bot/python-bale-bot/ Author: Kian Ahmadian Author-email: devs@python-bale-
+bot.ir License: LGPLv2 Download-URL: https://pypi.org/project/python-bale-bot/
+Project-URL: Documentation, https://docs.python-bale-bot.ir/en/stable/ Project-
+URL: Changelog, https:///docs.python-bale-bot.ir/en/stable/whats_new.html
+Project-URL: Bug Tracker, https://github.com/python-bale-bot/python-bale-bot/
+issues Project-URL: Source Code, https://github.com/python-bale-bot/python-
+bale-bot/ Keywords: bale bale-bot framework bot Platform: Windows Requires-
+Python: >=3.8 Description-Content-Type: text/markdown Provides-Extra: docs
+License-File: LICENSE # python-bale-bot
                            [python-bale-bot image]
                   An API wrapper for Bale written in Python.
             [![Python Version](https://img.shields.io/badge/Python-
- 3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://pypi.org/p/
- python-bale-bot) [![PyPi Version](https://img.shields.io/pypi/v/python-bale-
+3.8_|_3.9_|_3.10_|_3.11_-red?logo=python&style=plastic)](https://python.org) [!
+           [PyPi Version](https://img.shields.io/pypi/v/python-bale-
 bot?color=blue&label=pypi&style=plastic)](https://pypi.org/p/python-bale-bot)
          [![Codacy Badge](https://app.codacy.com/project/badge/Grade/
  deacf2bc3f13492d944e329ac19ac0d1)](https://www.codacy.com/gh/python-bale-bot/
  python-bale-bot/dashboard) [![python-bale-bot score](https://snyk.io/advisor/
 python/python-bale-bot/badge.svg)](https://snyk.io/advisor/python/python-bale-
 bot) [![Project License](https://img.shields.io/github/license/python-bale-bot/
-  python-bale-bot?style=plastic)](https://opensource.org/licenses/MIT) [![API
-   Version](https://img.shields.io/badge/Bale%20API-1.0-blue?style=plastic)]
-  (https://dev.bale.ai/api) [![Documentation Status](https://readthedocs.org/
-   projects/python-telegram-bot/badge/?version=stable)](https://python-bale-
-                                bot.rtfd.org/)
+python-bale-bot?style=plastic)](https://www.gnu.org/licenses/old-licenses/gpl-
+   2.0.en.html) [![API Version](https://img.shields.io/badge/Bale%20API-1.0-
+blue?style=plastic)](https://dev.bale.ai/api) [![Documentation Status](https://
+   readthedocs.org/projects/python-bale-bot/badge/?version=stable)](https://
+                           docs.python-bale-bot.ir/)
 ## Installing
                 You can install or update python-bale-bot via:
 ### PyPi: ``` $ pip install python-bale-bot -U ``` ### Git: ``` $ git clone
 https://github.com/python-bale-bot/python-bale-bot $ cd python-bale-bot $
 python setup.py install ``` ## Documentation
 The package_documentation is the technical reference for python-bale-bot. It
 contains descriptions of all available classes, modules, methods and arguments
```

### Comparing `python-bale-bot-2.4.6/python_bale_bot.egg-info/SOURCES.txt` & `python-bale-bot-2.4.7/python_bale_bot.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 bale/utils.py
 bale/version.py
 bale/attachments/__init__.py
 bale/attachments/audio.py
 bale/attachments/contact.py
 bale/attachments/document.py
 bale/attachments/file.py
+bale/attachments/input_file.py
 bale/attachments/location.py
 bale/attachments/photo.py
 bale/attachments/video.py
 bale/payments/__init__.py
 bale/payments/invoice.py
 bale/payments/price.py
 bale/request/__init__.py
```

