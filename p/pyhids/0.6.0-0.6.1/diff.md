# Comparing `tmp/pyhids-0.6.0.tar.gz` & `tmp/pyhids-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhids-0.6.0.tar", max compression
+gzip compressed data, was "pyhids-0.6.1.tar", max compression
```

## Comparing `pyhids-0.6.0.tar` & `pyhids-0.6.1.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rwxr-xr-x   0        0        0    35147 2023-07-21 17:40:28.550202 pyhids-0.6.0/COPYING
--rwxr-xr-x   0        0        0     4718 2023-08-03 12:08:18.728201 pyhids-0.6.0/README.md
--rwxr-xr-x   0        0        0     2853 2023-08-03 11:38:35.125802 pyhids-0.6.0/conf.py
--rw-r--r--   0        0        0        0 2023-07-19 18:15:45.896004 pyhids-0.6.0/pyhids/__init__.py
--rwxr-xr-x   0        0        0     4315 2023-08-02 06:50:21.139800 pyhids-0.6.0/pyhids/genBase.py
--rwxr-xr-x   0        0        0     1770 2023-07-21 17:40:27.914215 pyhids-0.6.0/pyhids/genKeys.py
--rw-r--r--   0        0        0     1349 2023-08-03 11:19:10.142113 pyhids-0.6.0/pyhids/hashlookup.py
--rw-r--r--   0        0        0      850 2023-08-03 12:05:18.302018 pyhids-0.6.0/pyhids/pandora.py
--rwxr-xr-x   0        0        0    10390 2023-08-02 06:50:21.139800 pyhids-0.6.0/pyhids/pyHIDS.py
--rw-r--r--   0        0        0      498 2023-08-03 08:21:41.402626 pyhids-0.6.0/pyhids/utils.py
--rw-r--r--   0        0        0     1206 2023-08-03 12:30:16.477963 pyhids-0.6.0/pyproject.toml
--rw-r--r--   0        0        0     5740 1970-01-01 00:00:00.000000 pyhids-0.6.0/PKG-INFO
+-rwxr-xr-x   0        0        0    35147 2023-07-21 17:40:28.550202 pyhids-0.6.1/COPYING
+-rwxr-xr-x   0        0        0     4005 2023-08-04 04:41:01.610374 pyhids-0.6.1/README.md
+-rw-r--r--   0        0        0        0 2023-07-19 18:16:40.004005 pyhids-0.6.1/bin/__init__.py
+-rw-r--r--   0        0        0     2383 2023-08-03 11:58:42.383028 pyhids-0.6.1/bin/main.py
+-rwxr-xr-x   0        0        0     2853 2023-08-03 11:38:35.125802 pyhids-0.6.1/conf.py
+-rw-r--r--   0        0        0        0 2023-07-19 18:15:45.896004 pyhids-0.6.1/pyhids/__init__.py
+-rwxr-xr-x   0        0        0     4315 2023-08-02 06:50:21.139800 pyhids-0.6.1/pyhids/genBase.py
+-rwxr-xr-x   0        0        0     1770 2023-07-21 17:40:27.914215 pyhids-0.6.1/pyhids/genKeys.py
+-rw-r--r--   0        0        0     1349 2023-08-03 11:19:10.142113 pyhids-0.6.1/pyhids/hashlookup.py
+-rw-r--r--   0        0        0      850 2023-08-03 12:05:18.302018 pyhids-0.6.1/pyhids/pandora.py
+-rwxr-xr-x   0        0        0    10390 2023-08-02 06:50:21.139800 pyhids-0.6.1/pyhids/pyHIDS.py
+-rw-r--r--   0        0        0      498 2023-08-03 08:21:41.402626 pyhids-0.6.1/pyhids/utils.py
+-rw-r--r--   0        0        0     1219 2023-08-04 04:41:19.518259 pyhids-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0     5027 1970-01-01 00:00:00.000000 pyhids-0.6.1/PKG-INFO
```

### Comparing `pyhids-0.6.0/COPYING` & `pyhids-0.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/README.md` & `pyhids-0.6.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: pyhids
+Version: 0.6.1
+Summary: A host-based intrusion detection system.
+Home-page: https://github.com/cedricbonhomme/pyHIDS
+License: GPL-3.0-or-later
+Keywords: hids,security
+Author: Cédric Bonhomme
+Author-email: cedric@cedricbonhomme.org
+Requires-Python: >=3.11,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Topic :: Security
+Requires-Dist: pyhashlookup (>=1.2.1,<2.0.0)
+Requires-Dist: pypandora (>=1.5.0,<2.0.0)
+Requires-Dist: rsa (>=4.9,<5.0)
+Project-URL: Repository, https://github.com/cedricbonhomme/pyHIDS
+Description-Content-Type: text/markdown
+
 ## pyHIDS
 
 ### Presentation
 
 [pyHIDS](https://github.com/cedricbonhomme/pyHIDS) is a
 [HIDS](http://en.wikipedia.org/wiki/Host-based_intrusion_detection_system)
 (host-based intrusion detection system) for verifying the integrity of a system.
@@ -25,22 +51,37 @@
 * alerts can be sent on IRC channels through the
   [irker](https://gitlab.com/esr/irker) IRC client (which should be running as
   a daemon).
 
 
 ### Installation
 
-#### Installation as a command line tool
-
-You can simply use [pipx](https://pypa.github.io/pipx/).
+You can simply use [pipx](https://pypa.github.io/pipx/)
+or [poetry](https://python-poetry.org/).
 
 ```bash
 $ pipx install pyHIDS
 $ export PYHIDS_CONFIG=~/.pyHIDS/conf.cfg
+```
+
+[An example](./conf.cfg-sample) of configuration file is available.
+With this file you can configure:
 
+- the connection to Hashlookup;
+- the connection to Pandora;
+- the connection IRC for the notifications;
+- the SMTP connection for the email notifications;
+- the ist of files to scan;
+- the regular expressions to specify files to scan in a folder;
+- the command's output to check.
+
+
+### Usage
+
+```bash
 $ pyhids gen-keys --size 2048
 Generating 2048 bits RSA keys ...
 Dumping Keys
 Done.
 
 $ pyhids gen-base --sign
 Generating database...
@@ -83,81 +124,30 @@
 [18/07/23 22:34:25] [notice] /bin/pamperspective ok
 [18/07/23 22:34:25] [notice] /bin/pod2usage ok
 [18/07/23 22:34:25] Error(s) : 0
 [18/07/23 22:34:25] Warning(s) : 0
 [18/07/23 22:34:25] HIDS finished.
 ```
 
+
+### Other features
+
 Check for known malicious files with
 [Hashlookup](https://github.com/hashlookup):
 
 ```bash
 $ pyhids hashlookup
 ```
 
-#### From the repository
-
-Get pyHIDS source code and copy the
-sample configuration file:
+Check for known malicious files with
+[Pandora](https://github.com/pandora-analysis):
 
 ```bash
-$ git clone https://github.com/cedricbonhomme/pyHIDS.git
-$ cd pyHIDS/
-$ cp ./conf.cfg-sample ./conf.cfg
-$ poetry install
-```
-
-The same as explained above applies.
-
-
-### Configuration
-
-The configuration file of pyHIDS looks like the following:
-
-```ini
-[hashlookup]
-root_url = https://hashlookup.circl.lu/
-[pandora]
-root_url = https://pandora.circl.lu/
-username = <username>
-password = <password>
-[irc]
-enabled = 0
-channel = irc://irc.libera.chat/#testpyHIDS
-host = localhost
-port = 6697
-[email]
-enabled = 0
-mail_from = pyHIDS@no-reply.com
-mail_to = you_address
-smtp = SMTP_server
-username = your_username
-password = your_password
-[files]
-file1 = /etc/crontab
-file2 = /boot/grub/grub.cfg
-file3 = /etc/shadow
-file4 = /etc/networks
-[rules]
-rule1 = conf$ /etc
-rule2 = list /etc/apt
-rule3 = .* /bin
-[commands]
-iptables = /sbin/iptables -L
-```
-
-Description of the sections:
-
-* *irc*: configure notifications sent via IRC;
-* *email*: configure the email notifications. Set the value of "enabled" to 1
-  to activate notifications;
-* *files*: list of files to scan;
-* *rules*: regular expression to specify files in a folder;
-* *commands*: command's output to check.
-
+$ pyhids pandora
+```
 
 
 ### Automatic execution
 
 Use the time-based job scheduler, Cron, in order to schedule system scans.
 In your shell enter the command:
 
@@ -178,7 +168,8 @@
 
 ### License
 
 [pyHIDS](https://github.com/cedricbonhomme/pyHIDS) is under
 [GPLv3](http://www.gnu.org/licenses/gpl-3.0.txt) license.
 
 Copyright (C) 2010-2023 [Cédric Bonhomme](https://www.cedricbonhomme.org)
+
```

### Comparing `pyhids-0.6.0/conf.py` & `pyhids-0.6.1/conf.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/pyhids/genBase.py` & `pyhids-0.6.1/pyhids/genBase.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/pyhids/genKeys.py` & `pyhids-0.6.1/pyhids/genKeys.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/pyhids/hashlookup.py` & `pyhids-0.6.1/pyhids/hashlookup.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/pyhids/pandora.py` & `pyhids-0.6.1/pyhids/pandora.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/pyhids/pyHIDS.py` & `pyhids-0.6.1/pyhids/pyHIDS.py`

 * *Files identical despite different names*

### Comparing `pyhids-0.6.0/pyproject.toml` & `pyhids-0.6.1/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyHIDS"
-version = "0.6.0"
+version = "0.6.1"
 description = "A host-based intrusion detection system."
 authors = ["Cédric Bonhomme <cedric@cedricbonhomme.org>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 homepage = "https://github.com/cedricbonhomme/pyHIDS"
 repository = "https://github.com/cedricbonhomme/pyHIDS"
@@ -23,14 +23,15 @@
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)"
 ]
 
 include = [
     "README.md",
     "COPYING",
     "conf.py",
+    "bin/*",
 ]
 
 [tool.poetry.scripts]
 pyhids = "bin.main:main"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

