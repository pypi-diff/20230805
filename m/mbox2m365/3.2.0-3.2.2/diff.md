# Comparing `tmp/mbox2m365-3.2.0.tar.gz` & `tmp/mbox2m365-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbox2m365-3.2.0.tar", last modified: Mon Jun 19 23:02:20 2023, max compression
+gzip compressed data, was "mbox2m365-3.2.2.tar", last modified: Fri Aug  4 23:21:44 2023, max compression
```

## Comparing `mbox2m365-3.2.0.tar` & `mbox2m365-3.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.891032 mbox2m365-3.2.0/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1551 2023-03-30 20:17:54.000000 mbox2m365-3.2.0/LICENSE
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       26 2023-03-30 20:16:20.000000 mbox2m365-3.2.0/MANIFEST.in
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-06-19 23:02:20.892032 mbox2m365-3.2.0/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 20:02:42.000000 mbox2m365-3.2.0/README.md
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 19:52:19.000000 mbox2m365-3.2.0/README.rst
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.889032 mbox2m365-3.2.0/jobber/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5167 2022-09-19 13:44:42.000000 mbox2m365-3.2.0/jobber/jobber.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.890032 mbox2m365-3.2.0/mbox2m365/
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2022-09-19 20:24:22.000000 mbox2m365-3.2.0/mbox2m365/__init__.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11547 2023-05-30 16:25:03.000000 mbox2m365-3.2.0/mbox2m365/__main__.py
--rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      908 2023-06-19 23:00:20.000000 mbox2m365-3.2.0/mbox2m365/mailSink.py
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    31187 2023-06-19 23:00:20.000000 mbox2m365-3.2.0/mbox2m365/mbox2m365.py
-drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-06-19 23:02:20.891032 mbox2m365-3.2.0/mbox2m365.egg-info/
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/PKG-INFO
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      380 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/SOURCES.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/dependency_links.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/entry_points.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/requires.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-06-19 23:02:20.000000 mbox2m365-3.2.0/mbox2m365.egg-info/top_level.txt
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-06-19 23:00:39.000000 mbox2m365-3.2.0/pyproject.toml
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-06-19 23:02:20.892032 mbox2m365-3.2.0/setup.cfg
--rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      441 2023-03-30 20:18:43.000000 mbox2m365-3.2.0/setup.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-08-04 23:21:44.093866 mbox2m365-3.2.2/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     1551 2023-03-30 20:17:54.000000 mbox2m365-3.2.2/LICENSE
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       26 2023-03-30 20:16:20.000000 mbox2m365-3.2.2/MANIFEST.in
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-08-04 23:21:44.093866 mbox2m365-3.2.2/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 20:02:42.000000 mbox2m365-3.2.2/README.md
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11135 2023-03-30 19:52:19.000000 mbox2m365-3.2.2/README.rst
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-08-04 23:21:44.092866 mbox2m365-3.2.2/jobber/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)     5167 2022-09-19 13:44:42.000000 mbox2m365-3.2.2/jobber/jobber.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-08-04 23:21:44.092866 mbox2m365-3.2.2/mbox2m365/
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)      268 2022-09-19 20:24:22.000000 mbox2m365-3.2.2/mbox2m365/__init__.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11547 2023-05-30 16:25:03.000000 mbox2m365-3.2.2/mbox2m365/__main__.py
+-rwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)     2068 2023-08-04 23:18:40.000000 mbox2m365-3.2.2/mbox2m365/mailSink.py
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    31525 2023-08-04 23:00:02.000000 mbox2m365-3.2.2/mbox2m365/mbox2m365.py
+drwxrwxr-x   0 rudolph  (2090878) fnndsc    (1102)        0 2023-08-04 23:21:44.093866 mbox2m365-3.2.2/mbox2m365.egg-info/
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)    11458 2023-08-04 23:21:44.000000 mbox2m365-3.2.2/mbox2m365.egg-info/PKG-INFO
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      380 2023-08-04 23:21:44.000000 mbox2m365-3.2.2/mbox2m365.egg-info/SOURCES.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)        1 2023-08-04 23:21:44.000000 mbox2m365-3.2.2/mbox2m365.egg-info/dependency_links.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       54 2023-08-04 23:21:44.000000 mbox2m365-3.2.2/mbox2m365.egg-info/entry_points.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       20 2023-08-04 23:21:44.000000 mbox2m365-3.2.2/mbox2m365.egg-info/requires.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)       17 2023-08-04 23:21:44.000000 mbox2m365-3.2.2/mbox2m365.egg-info/top_level.txt
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      260 2023-08-04 23:01:15.000000 mbox2m365-3.2.2/pyproject.toml
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      449 2023-08-04 23:21:44.093866 mbox2m365-3.2.2/setup.cfg
+-rw-rw-r--   0 rudolph  (2090878) fnndsc    (1102)      441 2023-03-30 20:18:43.000000 mbox2m365-3.2.2/setup.py
```

### Comparing `mbox2m365-3.2.0/LICENSE` & `mbox2m365-3.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.0/PKG-INFO` & `mbox2m365-3.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.2.0
+Version: 3.2.2
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `mbox2m365-3.2.0/README.md` & `mbox2m365-3.2.2/README.md`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.0/README.rst` & `mbox2m365-3.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.0/jobber/jobber.py` & `mbox2m365-3.2.2/jobber/jobber.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.0/mbox2m365/__main__.py` & `mbox2m365-3.2.2/mbox2m365/__main__.py`

 * *Files identical despite different names*

### Comparing `mbox2m365-3.2.0/mbox2m365/mbox2m365.py` & `mbox2m365-3.2.2/mbox2m365/mbox2m365.py`

 * *Files 1% similar despite different names*

```diff
@@ -595,16 +595,21 @@
                 # This test was originally predicated on the idea that tallying
                 # occurences across dates and hashes would always match. Sometimes
                 # with attachments, however, it seems the hashes do not. Hence for
                 # now this "dummy" fall through based solely on the date stamp
                 # only.
                 if lists_haveEqualValues(['l_date', 'l_date'], idx):
                     self.ld_m365.append(self.d_m365.copy())
-                    # pudb.set_trace()
-                    self.ld_m365[idx]['subject']      = get('list', 'key', 'l_subject', idx)
+                    # If there are less "subjects" than messages
+                    # (N messages all with the same subject, use
+                    # the first subject)
+                    try:
+                        self.ld_m365[idx]['subject']      = get('list', 'key', 'l_subject', idx)
+                    except:
+                        self.ld_m365[idx]['subject']      = get('list', 'key', 'l_subject', 0)
                     self.ld_m365[idx]['to']           = recipients_get(get('list', 'value', 'l_date', idx))
                     self.ld_m365[idx]['attachments']  = attachments_get(get('list', 'value', 'l_date', idx))
                     self.ld_m365[idx]['bodyContents'] = get('list', 'key', 'l_body', idx)
                     self.ld_m365[idx]['bodyHash']     = get('list', 'key', 'l_hash', idx)
 
         return {
             'status'        :   b_status,
@@ -654,14 +659,15 @@
 
             m365 outlook mail send -s '%s' -t %s --bodyContents '%s'""" % \
                     (
                       m365message['subject'],
                       m365message['to'],
                       m365message['bodyContents']
                     )
+            str_m365 = ''.join(str_m365.split(r'\r'))
             if len(m365message['attachments']):
                 for attachment in m365message['attachments']:
                     str_m365 += ' --attachment "' + str(self.configPath / Path(attachment)) + '"'
             return str_m365
 
         def txscript_save(str_content) -> None:
             self.transmissionCmd = self.configPath / Path(baseFileName + "_tx.cmd")
```

### Comparing `mbox2m365-3.2.0/mbox2m365.egg-info/PKG-INFO` & `mbox2m365-3.2.2/mbox2m365.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbox2m365
-Version: 3.2.0
+Version: 3.2.2
 Summary: 'Send a message stored within an mbox using m365 (Office365)'
 Home-page: https://github.com/FNNDSC/mbox2m365
 Author: Rudolph Pienaar
 Author-email: rudolph.pienaar@childrens.harvard.edu
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

