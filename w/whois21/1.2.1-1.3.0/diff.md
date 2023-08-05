# Comparing `tmp/whois21-1.2.1.tar.gz` & `tmp/whois21-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "whois21-1.2.1.tar", last modified: Tue Jul 11 15:49:38 2023, max compression
+gzip compressed data, was "whois21-1.3.0.tar", last modified: Sat Aug  5 16:24:25 2023, max compression
```

## Comparing `whois21-1.2.1.tar` & `whois21-1.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:49:38.614425 whois21-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-11 15:49:28.000000 whois21-1.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-11 15:49:28.000000 whois21-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-11 15:49:38.614425 whois21-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7776 2023-07-11 15:49:28.000000 whois21-1.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-07-11 15:49:28.000000 whois21-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 15:49:38.614425 whois21-1.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:49:38.614425 whois21-1.2.1/whois21/
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/API.py
--rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/ASN.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/DNS.py
--rw-r--r--   0 runner    (1001) docker     (123)    24017 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-11 15:49:28.000000 whois21-1.2.1/whois21/vcard-map.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 15:49:38.614425 whois21-1.2.1/whois21.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      340 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-11 15:49:38.000000 whois21-1.2.1/whois21.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:24:25.048843 whois21-1.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11351 2023-08-05 16:24:14.000000 whois21-1.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-05 16:24:14.000000 whois21-1.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-08-05 16:24:25.048843 whois21-1.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8305 2023-08-05 16:24:14.000000 whois21-1.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-08-05 16:24:14.000000 whois21-1.3.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 16:24:25.048843 whois21-1.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:24:25.048843 whois21-1.3.0/whois21/
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-08-05 16:24:14.000000 whois21-1.3.0/whois21/API.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6858 2023-08-05 16:24:14.000000 whois21-1.3.0/whois21/ASN.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-08-05 16:24:14.000000 whois21-1.3.0/whois21/DNS.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27003 2023-08-05 16:24:14.000000 whois21-1.3.0/whois21/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-08-05 16:24:14.000000 whois21-1.3.0/whois21/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-08-05 16:24:14.000000 whois21-1.3.0/whois21/vcard-map.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 16:24:25.048843 whois21-1.3.0/whois21.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-08-05 16:24:25.000000 whois21-1.3.0/whois21.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      340 2023-08-05 16:24:25.000000 whois21-1.3.0/whois21.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 16:24:25.000000 whois21-1.3.0/whois21.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-08-05 16:24:25.000000 whois21-1.3.0/whois21.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 16:24:25.000000 whois21-1.3.0/whois21.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-08-05 16:24:25.000000 whois21-1.3.0/whois21.egg-info/top_level.txt
```

### Comparing `whois21-1.2.1/LICENSE` & `whois21-1.3.0/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -182,15 +182,15 @@
       replaced with your own identifying information. (Don't include
       the brackets!)  The text should be enclosed in the appropriate
       comment syntax for the file format. We also recommend that a
       file or class name and description of purpose be included on the
       same "printed page" as the copyright notice for easier
       identification within third-party archives.
 
-   Copyright [yyyy] [name of copyright owner]
+   Copyright [2022-2023] [CodeWriter21]
 
    Licensed under the Apache License, Version 2.0 (the "License");
    you may not use this file except in compliance with the License.
    You may obtain a copy of the License at
 
        http://www.apache.org/licenses/LICENSE-2.0
```

### Comparing `whois21-1.2.1/PKG-INFO` & `whois21-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois21
-Version: 1.2.1
+Version: 1.3.0
 Summary: A simple and easy to use Python package that lets you query whois/RDAP information of a domain/IP.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/whois21
 Project-URL: Donations, https://github.com/MPCodeWriter21/whois21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/whois21
 Keywords: python,python3,CodeWriter21,WHOIS,whois21,RDAP,Registration Data Access Protocol,DNS,ASN
@@ -67,14 +67,16 @@
 ### Dependencies
 
 + [requests](https://requests.readthedocs.io/en/master/): Used for:
     - Downloading list of whois and RDAP servers.
     - Downloading RDAP information.
 + [importlib_resources](https://importlib-resources.readthedocs.io/en/latest/): Used for:
     - Getting the path to the whois21 package installation directory(for saving server lists).
++ [chardet](https://pypi.org/project/chardet/): Used for:
+    - Detecting the encoding of the whois response.
 + [log21](https://github.com/MPCodeWriter21/log21): Used for:
     - Colorized Logging.
     - Printing collected data in pprint or tree format.
 + [os](https://docs.python.org/3/library/os.html) (A core python module): Used for:
     - Working with files and directories.
 + [socket](https://docs.python.org/3/library/socket.html) (A core python module): Used for:
     - Establishing TCP connection to the whois server.
@@ -92,17 +94,23 @@
     - Type hinting.
 + [re](https://docs.python.org/3/library/re.html) (A core python module): Used for:
     - Matching date-time strings with regular expressions.
 
 Changes
 -------
 
-### 1.2.1
+### 1.3.0
 
-Switched from `setup.py` to `pyproject.toml`.
++ Added the option to specify the encoding to use for encoding and decoding the data in 
+  in WHOIS class.
++ Added the option to customize the behavior of the WHOIS class when it encounters an 
+  error while encoding or decoding data.
++ Added the feature to automatically detect the encoding of _whois_ response to solve
+  decoding issues, such as the one mentioned in issue #2. This is done with the help of
+  [chardet](https://pypi.org/project/chardet/) package.
 
 Usage Examples:
 ---------------
 
 ### CLI Examples
 
 + Example 1: Query whois information of google.com
```

### Comparing `whois21-1.2.1/README.md` & `whois21-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,16 @@
 ### Dependencies
 
 + [requests](https://requests.readthedocs.io/en/master/): Used for:
     - Downloading list of whois and RDAP servers.
     - Downloading RDAP information.
 + [importlib_resources](https://importlib-resources.readthedocs.io/en/latest/): Used for:
     - Getting the path to the whois21 package installation directory(for saving server lists).
++ [chardet](https://pypi.org/project/chardet/): Used for:
+    - Detecting the encoding of the whois response.
 + [log21](https://github.com/MPCodeWriter21/log21): Used for:
     - Colorized Logging.
     - Printing collected data in pprint or tree format.
 + [os](https://docs.python.org/3/library/os.html) (A core python module): Used for:
     - Working with files and directories.
 + [socket](https://docs.python.org/3/library/socket.html) (A core python module): Used for:
     - Establishing TCP connection to the whois server.
@@ -76,17 +78,23 @@
     - Type hinting.
 + [re](https://docs.python.org/3/library/re.html) (A core python module): Used for:
     - Matching date-time strings with regular expressions.
 
 Changes
 -------
 
-### 1.2.1
+### 1.3.0
 
-Switched from `setup.py` to `pyproject.toml`.
++ Added the option to specify the encoding to use for encoding and decoding the data in 
+  in WHOIS class.
++ Added the option to customize the behavior of the WHOIS class when it encounters an 
+  error while encoding or decoding data.
++ Added the feature to automatically detect the encoding of _whois_ response to solve
+  decoding issues, such as the one mentioned in issue #2. This is done with the help of
+  [chardet](https://pypi.org/project/chardet/) package.
 
 Usage Examples:
 ---------------
 
 ### CLI Examples
 
 + Example 1: Query whois information of google.com
```

### Comparing `whois21-1.2.1/whois21/API.py` & `whois21-1.3.0/whois21/API.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.1/whois21/ASN.py` & `whois21-1.3.0/whois21/ASN.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.1/whois21/DNS.py` & `whois21-1.3.0/whois21/DNS.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.1/whois21/__init__.py` & `whois21-1.3.0/whois21/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,25 +4,26 @@
 import re
 import json
 import socket
 from typing import Set, Union, Optional, Sequence
 from datetime import datetime
 
 import log21
+import chardet
 import requests
 import importlib_resources
 
 from whois21.API import lookup_ip_ip_api, batch_lookup_ip_ip_api
 from whois21.ASN import (validate_ip, get_asn_dict, get_asn_services, download_asn_json,
                          ip_registration_data_lookup, ip_registration_data_lookup_)
 from whois21.DNS import (get_dns_dict, get_dns_services, download_dns_json,
                          domain_registration_data_lookup,
                          domain_registration_data_lookup_)
 
-__version__ = '1.2.0'
+__version__ = '1.3.0'
 __github__ = 'https://github.com/MPCodeWriter21/whois21'
 __author__ = 'CodeWriter21'
 __email__ = 'CodeWriter21@gmail.com'
 __license__ = 'Apache License 2.0'
 
 __all__ = [
     '__version__', '__github__', '__author__', '__email__', '__license__',
@@ -69,39 +70,40 @@
 
 
 def get_whois_servers(
     force_download: bool = False, path: Optional[Union[str, os.PathLike]] = None
 ):
     """Returns a dictionary of the whois-servers.txt file.
 
-    :param force_download: If True, the whois-servers.txt file will be downloaded again.
+    :param force_download: If True, the whois-servers.txt file will be
+        downloaded again.
     :param path: The path to the whois-servers.txt file.
     :return: A dictionary of the whois-servers.txt file.
     """
     if not path:
         path = str(importlib_resources.files('whois21') / 'whois-servers.txt')
 
     if not os.path.exists(path) or force_download:
         download_whois_servers(path)
 
-    data = dict()
-    with open(path, 'r') as file:
+    data = {}
+    with open(path, 'r', encoding='utf-8') as file:
         for line in file:
             if line.startswith(';') or ' ' not in line:
                 continue
             key, value = line.split(' ', 1)
             data[key] = value.strip(' \n')
 
     return data
 
 
 whois_servers: dict = {
     'ABUSE_HOST': 'whois.abuse.net',
     # Types of queries: POCs, ownerid, CIDR blocks, IP and AS numbers.
-    'LNICHOST': 'whois.lacnic.net',  
+    'LNICHOST': 'whois.lacnic.net',
     'ai': {'whois.nic.ai'},
     'app': {'whois.nic.google'},
     'ar': {'whois.nic.ar'},
     'by': {'whois.cctld.by'},
     'ca': {'whois.ca.fury.ca'},
     'chat': {'whois.nic.chat'},
     'cl': {'whois.nic.cl'},
@@ -144,63 +146,119 @@
     'website': {'whois.nic.website'},
     'za': {'whois.registry.net.za'}
 }
 
 for _key, _value in get_whois_servers().items():
     whois_servers[_key] = {*whois_servers.get(_key, {}), _value}
 
-with open(str(importlib_resources.files('whois21') / 'vcard-map.json'), 'r') as f:
+with open(str(importlib_resources.files('whois21') / 'vcard-map.json'), 'r',
+          encoding='utf-8') as f:
     vcard_map = json.load(f)
 
 
 class WHOIS:
     __domain: str
     __success: bool = False
     __error: str = ''
     __raw: bytes = b''
     __servers: Set[str] = set()
     __whois_data: dict = {}
     __rdap_data: dict = {}
+    __encode_encoding: str = 'utf-8'
+    __decode_encoding: Optional[str] = None
+    __encoding_errors: str = 'strict'
     timeout: int = 10
 
     def __init__(
         self,
         domain: str,
         servers: Optional[Sequence[str]] = None,
         timeout: int = 10,
         use_rdap: bool = True,
-        force_rdap: bool = False
+        force_rdap: bool = False,
+        encode_encoding: str = 'utf-8',
+        decode_encoding: Optional[str] = None,
+        encoding_errors: str = 'strict',
     ):
-        self.whois(domain, servers, timeout, use_rdap, force_rdap)
+        """Initialize WHOIS object.
+
+        :param domain: Domain name/IP to query.
+        :param servers: List of WHOIS servers to use.
+        :param timeout: Timeout in seconds. (default: 10)
+        :param use_rdap: Use RDAP if available and WHOIS fails.
+        :param force_rdap: Force RDAP usage.
+        :param encode_encoding: Encoding to use for encoding. (default:
+            utf-8)
+        :param decode_encoding: Encoding to use for decoding. (default:
+            AUTODETECT)
+        :param encoding_errors: Encoding error handling. (default:
+            strict)
+        """
+        self.registry_domain_id = None
+        self.registrar_whois_server = None
+        self.registrar_url = None
+        self.updated_date = None
+        self.creation_date = None
+        self.expires_date = None
+        self.registrar_name = None
+        self.registrar_iana_id = None
+        self.registrar_abuse_contact_email = None
+        self.registrar_abuse_contact_phone = None
+        self.status = None
+        self.name_servers = None
+
+        self.whois(
+            domain,
+            servers=servers,
+            timeout=timeout,
+            use_rdap=use_rdap,
+            force_rdap=force_rdap,
+            encode_encoding=encode_encoding,
+            decode_encoding=decode_encoding,
+            encoding_errors=encoding_errors,
+        )
 
     def whois(
         self,
-        domain: str,
+        domain: Optional[str] = None,
+        *,
         servers: Optional[Sequence[str]] = None,
         timeout: int = 10,
         use_rdap: bool = True,
-        force_rdap: bool = False
+        force_rdap: bool = False,
+        encode_encoding: str = 'utf-8',
+        decode_encoding: Optional[str] = None,
+        encoding_errors: str = 'strict',
     ):
         """Queries the whois server for the domain.
 
         :param domain: The domain/ip to query.
         :param servers: The servers to use.
         :param timeout: The timeout in seconds.
         :param use_rdap: If True, the RDAP server will be used if the
-                whois servers don't respond.
+            whois servers don't respond.
         :param force_rdap: If True, the RDAP server will be used even if
-                the whois servers respond.
+            the whois servers respond.
+        :param encode_encoding: Encoding to use for encoding. (default:
+            utf-8)
+        :param decode_encoding: Encoding to use for decoding. (default:
+            AUTODETECT)
+        :param encoding_errors: How to handle encoding errors. (default:
+            strict)
         """
         self.__domain = domain.lower()
         self.__success = False
         self.__servers = set(servers) if servers else set()
         self.__whois_data = {}
         self.timeout = timeout
         self.__error = ''
         self.__raw = b''
+        self.__encode_encoding = encode_encoding
+        self.__decode_encoding = decode_encoding
+        self.__encoding_errors = encoding_errors
 
         if not force_rdap:
             self.__whois()
 
         if (not self.__success and use_rdap) or force_rdap:
             self.__rdap()
 
@@ -277,69 +335,73 @@
         # Send a query to the whois.iana.org server to find the whois server for the
         # domain.
         # Create a socket connection to the whois.iana.org server.
         log21.debug(f'Connecting to {LBLUE}whois.iana.org:43{RESET}...')
         try:
             sock = socket.create_connection(('whois.iana.org', 43))
             sock.settimeout(self.timeout)
-        except socket.error as e:
+        except socket.error as ex:
             log21.debug(
                 f'Error connecting to "{RED}whois.iana.org:43{RESET}": '
-                f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                f'{LRED}{ex.__class__.__name__}: {ex}{RESET}'
             )
             self.__error = (
                 'Error connecting "to whois.iana.org:43": '
-                f'{e.__class__.__name__}: {e}'
+                f'{ex.__class__.__name__}: {ex}'
             )
             return
         # Send the domain name to the whois.iana.org server.
         log21.debug(f'Sending query for {LCYAN}{self.domain}{RESET}...')
         try:
-            sock.send(self.domain.encode('utf-8') + b'\r\n')
-        except socket.error as e:
+            sock.send(
+                self.domain
+                .encode(self.__encode_encoding, errors=self.__encoding_errors) + b'\r\n'
+            )
+        except socket.error as ex:
             log21.debug(
                 f'Error sending query to "{RED}whois.iana.org:43{RESET}": '
-                f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                f'{LRED}{ex.__class__.__name__}: {ex}{RESET}'
             )
             self.__error = (
                 'Error sending query to "whois.iana.org:43": '
-                f'{e.__class__.__name__}: {e}'
+                f'{ex.__class__.__name__}: {ex}'
             )
             return
         # Receive the raw data from the whois.iana.org server.
         self.__raw = b''
         log21.debug('Receiving data...')
         try:
             while True:
                 data = sock.recv(4096)
                 if not data:
                     break
                 self.__raw += data
-        except socket.error as e:
+        except socket.error as ex:
             log21.debug(
                 f'Error receiving data from "{RED}whois.iana.org:43{RESET}": '
-                f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                f'{LRED}{ex.__class__.__name__}: {ex}{RESET}'
             )
             self.__error = (
                 'Error receiving data from "whois.iana.org:43": '
-                f'{e.__class__.__name__}: {e}'
+                f'{ex.__class__.__name__}: {ex}'
             )
             return
         sock.close()
 
         # Checks if we received any data from the whois.iana.org server.
         if not self.__raw:
             log21.debug(f'{LRED}No data received.{RESET}')
             self.__error = 'No data received from whois.iana.org.'
             return
 
         log21.debug('Parsing data: Searching for whois server...')
         # Parse the raw data from the whois.iana.org server and extract the whois
         # server.
-        for line in self.__raw.decode('utf-8').split('\n'):
+        for line in self.__raw.decode(self.__get_decode_encoding(self.__raw),
+                                      errors=self.__encoding_errors).split('\n'):
             if line.startswith('whois:'):
                 self.__servers.add(line[6:].strip())
                 break
         else:
             log21.debug(f'{LRED}No whois server found.{RESET}')
             self.__error = 'No whois server found.'
             log21.debug('Trying to get another whois server...')
@@ -355,78 +417,85 @@
         else:
             if tld in whois_servers:
                 self.__servers.update(whois_servers[tld])
 
             self.__servers.add(tld + '.whois-servers.net')
             self.__servers.add('whois.nic.' + tld)
 
+    # pylint: disable=too-many-branches, too-many-statements, too-many-nested-blocks
     def __call_whois_servers(self):
         # Get the whois information for the domain.
         for whois_server in self.__servers:
             # Create a socket connection to the whois server.
             log21.debug(f'Connecting to {LBLUE}{whois_server}{RESET}...')
             try:
                 sock = socket.create_connection((whois_server, 43))
                 sock.settimeout(self.timeout)
-            except socket.error as e:
+            except socket.error as ex:
                 log21.debug(
                     f'Error connecting to "{RED}{whois_server}{RESET}": '
-                    f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                    f'{LRED}{ex.__class__.__name__}: {ex}{RESET}'
                 )
                 self.__error = (
                     f'Error connecting to "{whois_server}": '
-                    f'{e.__class__.__name__}: {e}'
+                    f'{ex.__class__.__name__}: {ex}'
                 )
                 continue
             # Send the domain name to the whois server.
             log21.debug(f'Sending query for {LCYAN}{self.domain}{RESET}...')
             try:
-                sock.send(self.domain.encode('utf-8') + b'\r\n')
-            except socket.error as e:
+                sock.send(
+                    self.domain
+                    .encode(self.__encode_encoding, errors=self.__encoding_errors) +
+                    b'\r\n'
+                )
+            except socket.error as ex:
                 log21.debug(
                     f'Error sending query to "{RED}{whois_server}{RESET}": '
-                    f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                    f'{LRED}{ex.__class__.__name__}: {ex}{RESET}'
                 )
                 self.__error = (
                     f'Error sending query to "{whois_server}": '
-                    f'{e.__class__.__name__}: {e}'
+                    f'{ex.__class__.__name__}: {ex}'
                 )
                 continue
             # Receive the raw whois data from the whois server.
             self.__raw = b''
             log21.debug('Receiving data...')
             try:
                 while True:
                     data = sock.recv(4096)
                     if not data:
                         break
                     self.__raw += data
-            except socket.error as e:
+            except socket.error as ex:
                 log21.debug(
                     f'Error receiving data from "{RED}{whois_server}{RESET}": '
-                    f'{LRED}{e.__class__.__name__}: {e}{RESET}'
+                    f'{LRED}{ex.__class__.__name__}: {ex}{RESET}'
                 )
                 self.__error = (
                     f'Error receiving data from "{whois_server}": '
-                    f'{e.__class__.__name__}: {e}'
+                    f'{ex.__class__.__name__}: {ex}'
                 )
                 continue
             sock.close()
 
             # Checks if we received any data from the whois server.
             if not self.__raw:
                 log21.debug(f'No data received from {RED}{whois_server}{RESET}.')
                 self.__error = f'No data received from {whois_server}.'
                 continue
             # Parse the raw whois data from the whois server and extract the whois
             # information.
             log21.debug('Parsing data...')
             self.__whois_data = {}
             i = 0
-            lines = self.__raw.decode('utf-8').split('\n')
+            lines = self.__raw.decode(
+                self.__get_decode_encoding(self.__raw), errors=self.__encoding_errors
+            ).split('\n')
             while i < len(lines):
                 line = lines[i]
                 if line.startswith('%') or line.startswith('#'):
                     i += 1
                     continue
                 if ':' in line:
                     key, value = line.split(':', 1)
@@ -466,22 +535,22 @@
             return
 
     def __rdap(self):
         # Get the rdap information for the domain.
         log21.debug('Getting rdap information...')
         try:
             self.__rdap_data = registration_data_lookup(self.domain)
-        except Exception as e:
+        except Exception as ex:  # pylint: disable=broad-except
             log21.debug(
                 f'{LRED}Error{RESET} getting rdap information: '
-                f'{e.__class__.__name__}: {e}'
+                f'{ex.__class__.__name__}: {ex}'
             )
             self.__error = (
                 'Error getting rdap information: '
-                f'{e.__class__.__name__}: {e}'
+                f'{ex.__class__.__name__}: {ex}'
             )
             return
 
         if not self.__rdap_data:
             log21.debug(f'{LRED}No data found.{RESET}')
             self.__error = 'No rdap data found.'
             return
@@ -596,14 +665,19 @@
 
             for _entity in entity_.get('entities', []):
                 handle_entity(prefix, _entity)
 
         for entity in self.__rdap_data.get('entities', []):
             handle_entity('', entity)
 
+    def __get_decode_encoding(self, data):
+        if self.__decode_encoding:
+            return self.__decode_encoding
+        return chardet.detect(data)['encoding']
+
     @property
     def whois_data(self):
         return self.__whois_data
 
     @property
     def rdap_data(self):
         return self.__rdap_data
@@ -625,15 +699,17 @@
         return self.__success
 
     @property
     def error(self):
         return self.__error
 
     def __str__(self):
-        return self.__raw.decode('utf-8')
+        return self.__raw.decode(
+            self.__get_decode_encoding(self.__raw), errors=self.__encoding_errors
+        )
 
     def __repr__(self):
         return f'WHOIS(domain="{self.__domain}", success={self.__success})'
 
     def get(self, key: str, default=None):
         return self.__whois_data.get(key.upper(), default)
```

### Comparing `whois21-1.2.1/whois21/__main__.py` & `whois21-1.3.0/whois21/__main__.py`

 * *Files identical despite different names*

### Comparing `whois21-1.2.1/whois21/vcard-map.json` & `whois21-1.3.0/whois21/vcard-map.json`

 * *Files identical despite different names*

### Comparing `whois21-1.2.1/whois21.egg-info/PKG-INFO` & `whois21-1.3.0/whois21.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whois21
-Version: 1.2.1
+Version: 1.3.0
 Summary: A simple and easy to use Python package that lets you query whois/RDAP information of a domain/IP.
 Author-email: "CodeWriter21(Mehrad Pooryoussof)" <CodeWriter21@gmail.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/MPCodeWriter21/whois21
 Project-URL: Donations, https://github.com/MPCodeWriter21/whois21/blob/master/DONATE.md
 Project-URL: Source, https://github.com/MPCodeWriter21/whois21
 Keywords: python,python3,CodeWriter21,WHOIS,whois21,RDAP,Registration Data Access Protocol,DNS,ASN
@@ -67,14 +67,16 @@
 ### Dependencies
 
 + [requests](https://requests.readthedocs.io/en/master/): Used for:
     - Downloading list of whois and RDAP servers.
     - Downloading RDAP information.
 + [importlib_resources](https://importlib-resources.readthedocs.io/en/latest/): Used for:
     - Getting the path to the whois21 package installation directory(for saving server lists).
++ [chardet](https://pypi.org/project/chardet/): Used for:
+    - Detecting the encoding of the whois response.
 + [log21](https://github.com/MPCodeWriter21/log21): Used for:
     - Colorized Logging.
     - Printing collected data in pprint or tree format.
 + [os](https://docs.python.org/3/library/os.html) (A core python module): Used for:
     - Working with files and directories.
 + [socket](https://docs.python.org/3/library/socket.html) (A core python module): Used for:
     - Establishing TCP connection to the whois server.
@@ -92,17 +94,23 @@
     - Type hinting.
 + [re](https://docs.python.org/3/library/re.html) (A core python module): Used for:
     - Matching date-time strings with regular expressions.
 
 Changes
 -------
 
-### 1.2.1
+### 1.3.0
 
-Switched from `setup.py` to `pyproject.toml`.
++ Added the option to specify the encoding to use for encoding and decoding the data in 
+  in WHOIS class.
++ Added the option to customize the behavior of the WHOIS class when it encounters an 
+  error while encoding or decoding data.
++ Added the feature to automatically detect the encoding of _whois_ response to solve
+  decoding issues, such as the one mentioned in issue #2. This is done with the help of
+  [chardet](https://pypi.org/project/chardet/) package.
 
 Usage Examples:
 ---------------
 
 ### CLI Examples
 
 + Example 1: Query whois information of google.com
```

