# Comparing `tmp/microformats-0.3.4.tar.gz` & `tmp/microformats-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microformats-0.3.4.tar", max compression
+gzip compressed data, was "microformats-0.3.5.tar", max compression
```

## Comparing `microformats-0.3.4.tar` & `microformats-0.3.5.tar`

### file list

```diff
@@ -1,17 +1,6 @@
--rw-r--r--   0        0        0     1371 2023-02-11 03:27:49.793277 microformats-0.3.4/LICENSE.mf2py
--rw-r--r--   0        0        0     1361 2023-02-11 03:27:37.185104 microformats-0.3.4/LICENSE.mf2util
--rw-r--r--   0        0        0     1239 2023-02-11 03:26:33.336230 microformats-0.3.4/README.md
--rw-r--r--   0        0        0     1463 2023-02-11 03:14:07.437977 microformats-0.3.4/mf/__init__.py
--rw-r--r--   0        0        0     3727 2023-02-10 04:51:02.491756 microformats-0.3.4/mf/date_util.py
--rw-r--r--   0        0        0    20352 2023-02-10 21:17:41.714338 microformats-0.3.4/mf/parser/__init__.py
--rw-r--r--   0        0        0     5803 2023-02-10 20:39:45.665262 microformats-0.3.4/mf/parser/backcompat/__init__.py
--rw-r--r--   0        0        0    10549 2023-02-10 20:03:24.170957 microformats-0.3.4/mf/parser/backcompat/rules.json
--rw-r--r--   0        0        0      985 2023-02-10 19:52:05.850212 microformats-0.3.4/mf/parser/class_util.py
--rw-r--r--   0        0        0     6030 2023-02-05 02:46:45.353989 microformats-0.3.4/mf/parser/dom_util.py
--rw-r--r--   0        0        0     3197 2023-02-10 20:14:16.496472 microformats-0.3.4/mf/parser/prop_util/__init__.py
--rw-r--r--   0        0        0     6866 2023-02-10 19:48:50.619704 microformats-0.3.4/mf/parser/prop_util/implied.py
--rw-r--r--   0        0        0     3038 2023-02-10 19:24:22.945062 microformats-0.3.4/mf/parser/prop_util/vcp.py
--rw-r--r--   0        0        0    40474 2023-02-11 02:58:05.900410 microformats-0.3.4/mf/util.py
--rw-r--r--   0        0        0      866 2023-02-11 03:27:53.849333 microformats-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2245 1970-01-01 00:00:00.000000 microformats-0.3.4/setup.py
--rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 microformats-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1363 2023-08-05 02:10:45.216705 microformats-0.3.5/LICENSE.mf2util
+-rw-r--r--   0        0        0     1266 2023-02-11 05:53:13.520706 microformats-0.3.5/README.md
+-rw-r--r--   0        0        0    42340 2023-08-05 02:07:31.801851 microformats-0.3.5/mf.py
+-rw-r--r--   0        0        0      826 2023-08-05 03:58:52.556864 microformats-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2121 1970-01-01 00:00:00.000000 microformats-0.3.5/setup.py
+-rw-r--r--   0        0        0     2022 1970-01-01 00:00:00.000000 microformats-0.3.5/PKG-INFO
```

### Comparing `microformats-0.3.4/LICENSE.mf2util` & `microformats-0.3.5/LICENSE.mf2util`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-https://github.com/kylewm/mf2util @b1acd Copyright (c) 2014
+https://github.com/kylewm/mf2util @b1acda6 Copyright (c) 2014
   Kyle Mahan <kyle@kylewm.com> <https://kylewm.com>
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are
 met:
 
 1. Redistributions of source code must retain the above copyright
```

### Comparing `microformats-0.3.4/README.md` & `microformats-0.3.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,41 @@
 [microformats][0] are the simplest way to openly publish contacts, events,
 reviews, recipes, and other structured information on the web.
 
     >>> import mf
     >>> url = "https://alice.example"
-    >>> doc = mf.parse(doc=f'''
+    >>> doc = f'''
     ... <p class=h-card><a href={url}>Alice</a></p>
     ... <ul class=h-feed>
     ... <li class=h-entry>foo
     ... <li class=h-entry>bar
     ... </ul>
-    ... ''', url=url)
+    ... '''
+    >>> page = mf.parse(doc=doc, url=url)
 
-    # TODO >>> dict(doc)
-    # TODO >>> doc.json
+    # TODO >>> dict(page)
+    # TODO >>> page.json
 
-    >>> card = doc["items"][0]
+    >>> card = page["items"][0]
     >>> card["type"]
     ['h-card']
     >>> card["properties"]
     {'name': ['Alice'], 'url': ['https://alice.example']}
-    >>> feed = doc["items"][1]
+    >>> feed = page["items"][1]
     >>> feed["children"][0]["properties"]["name"]
     ['foo']
 
-    >>> mf.util.representative_card(doc, url)
+    >>> mf.util.representative_card(page, url)
     {'name': ['Alice'], 'url': ['https://alice.example']}
-    >>> mf.util.representative_feed(doc, url)["items"][0]["name"]
+    >>> mf.util.representative_feed(page, url)["items"][0]["name"]
     ['foo']
 
-    # TODO >>> doc.representative_card
+    # TODO >>> page.representative_card
     # TODO {'name': ['Alice'], 'url': ['https://alice.example']}
-    # TODO >>> doc.representative_feed["items"][0]["name"]
+    # TODO >>> page.representative_feed["items"][0]["name"]
     # TODO ['foo']
 
 Based upon [`mf2py`][1] and [`mf2util`][2].
 
 [0]: https://microformats.org/wiki/microformats
 [1]: https://github.com/microformats/mf2py
 [2]: https://github.com/kylewm/mf2util
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
 [microformats][0] are the simplest way to openly publish contacts, events,
 reviews, recipes, and other structured information on the web. >>> import mf
->>> url = "https://alice.example" >>> doc = mf.parse(doc=f''' ...
+>>> url = "https://alice.example" >>> doc = f''' ...
 Alice
 ...
     * ...
     * foo ...
     * bar ...
-... ''', url=url) # TODO >>> dict(doc) # TODO >>> doc.json >>> card = doc
-["items"][0] >>> card["type"] ['h-card'] >>> card["properties"] {'name':
-['Alice'], 'url': ['https://alice.example']} >>> feed = doc["items"][1] >>>
-feed["children"][0]["properties"]["name"] ['foo'] >>>
-mf.util.representative_card(doc, url) {'name': ['Alice'], 'url': ['https://
-alice.example']} >>> mf.util.representative_feed(doc, url)["items"][0]["name"]
-['foo'] # TODO >>> doc.representative_card # TODO {'name': ['Alice'], 'url':
-['https://alice.example']} # TODO >>> doc.representative_feed["items"][0]
+... ''' >>> page = mf.parse(doc=doc, url=url) # TODO >>> dict(page) # TODO >>>
+page.json >>> card = page["items"][0] >>> card["type"] ['h-card'] >>> card
+["properties"] {'name': ['Alice'], 'url': ['https://alice.example']} >>> feed =
+page["items"][1] >>> feed["children"][0]["properties"]["name"] ['foo'] >>>
+mf.util.representative_card(page, url) {'name': ['Alice'], 'url': ['https://
+alice.example']} >>> mf.util.representative_feed(page, url)["items"][0]["name"]
+['foo'] # TODO >>> page.representative_card # TODO {'name': ['Alice'], 'url':
+['https://alice.example']} # TODO >>> page.representative_feed["items"][0]
 ["name"] # TODO ['foo'] Based upon [`mf2py`][1] and [`mf2util`][2]. [0]: https:
 //microformats.org/wiki/microformats [1]: https://github.com/microformats/mf2py
 [2]: https://github.com/kylewm/mf2util
```

### Comparing `microformats-0.3.4/mf/util.py` & `microformats-0.3.5/mf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 """
-Utilities for interpreting mf2 data.
+Microformats utilities.
 
 Microformats2 is a general way to mark up any HTML document with
 classes and propeties. This module uses domain-specific assumptions
 about the classes (specifically h-entry and h-event) to extract
 certain interesting properties.
 
 """
 
 import collections
+import datetime
 import re
 import string
 import unicodedata
 from urllib.parse import urljoin
 
 import bs4
 import easyuri
+from mf2py import parse
 
-from . import date_util
+__all__ = ["parse", "representative_card"]
 
 URL_ATTRIBUTES = {
     "a": ["href"],
     "link": ["href"],
     "img": ["src"],
     "audio": ["src"],
     "video": ["src", "poster"],
@@ -119,15 +121,73 @@
     """
     hentry = find_first_entry(parsed)
     result = {}
 
     if hentry:
         for prop in ("published", "updated", "start", "end"):
             date_strs = hentry["properties"].get(prop, [])
-            result[prop] = date_util.parse_dt(" ".join(date_strs))
+            result[prop] = parse_dt(" ".join(date_strs))
+
+
+def parse_dt(s):
+    """The definition for microformats2 dt-* properties are fairly
+    lenient.  This method converts an mf2 date string into either a
+    datetime.date or datetime.datetime object. Datetimes will be naive
+    unless a timezone is specified.
+
+    :param str s: a mf2 string representation of a date or datetime
+    :return: datetime.date or datetime.datetime
+    :raises ValueError: if the string is not recognizable
+    """
+
+    if not s:
+        return None
+
+    s = re.sub(r"\s+", " ", s)
+    date_re = r"(?P<year>\d{4,})-(?P<month>\d{1,2})-(?P<day>\d{1,2})"
+    time_re = r"(?P<hour>\d{1,2}):(?P<minute>\d{2})(:(?P<second>\d{2})(\.(?P<microsecond>\d+))?)?"
+    tz_re = r"(?P<tzz>Z)|(?P<tzsign>[+-])(?P<tzhour>\d{1,2}):?(?P<tzminute>\d{2})"
+    dt_re = f"{date_re}((T| ){time_re} ?({tz_re})?)?$"
+
+    m = re.match(dt_re, s)
+    if not m:
+        raise ValueError(f"unrecognized datetime {s}")
+
+    year = m.group("year")
+    month = m.group("month")
+    day = m.group("day")
+
+    hour = m.group("hour")
+
+    if not hour:
+        return datetime.date(int(year), int(month), int(day))
+
+    minute = m.group("minute") or "00"
+    second = m.group("second") or "00"
+
+    if hour:
+        dt = datetime.datetime(
+            int(year), int(month), int(day), int(hour), int(minute), int(second)
+        )
+    if m.group("tzz"):
+        dt = dt.replace(tzinfo=datetime.timezone.utc)
+    else:
+        tzsign = m.group("tzsign")
+        tzhour = m.group("tzhour")
+        tzminute = m.group("tzminute") or "00"
+
+        if tzsign and tzhour:
+            offset = datetime.timedelta(hours=int(tzhour), minutes=int(tzminute))
+            if tzsign == "-":
+                offset = -offset
+            dt = dt.replace(
+                tzinfo=datetime.timezone(offset, f"{tzsign}{tzhour}:{tzminute}")
+            )
+
+    return dt
 
 
 def get_plain_text(values, strip=True):
     """Get the first value in a list of values that we expect to be plain-text.
     If it is a dict, then return the value of "value".
 
     :param list values: a list of values
@@ -485,15 +545,15 @@
         date_str = get_plain_text(props.get(prop))
         if date_str:
             if want_json:
                 result[prop] = date_str
             else:
                 result[prop + "-str"] = date_str
                 try:
-                    date = date_util.parse_dt(date_str)
+                    date = parse_dt(date_str)
                     if date:
                         result[prop] = date
                 except ValueError:
                     raise ValueError(f"Failed to parse datetime {date_str}")
 
     author = find_author(parsed, source_url, hentry, fetch_mf2_func)
     if author:
```

### Comparing `microformats-0.3.4/pyproject.toml` & `microformats-0.3.5/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 [tool.poetry]
 name = "microformats"
-version = "0.3.4"
+version = "0.3.5"
 description = "tools for microformats production, consumption and analysis"
 readme = "README.md"
 keywords = ["IndieWeb", "microformats"]
 homepage = "https://ragt.ag/code/python-microformats"
 authors = ["Angelo Gladding <angelo@ragt.ag>"]
 license = "BSD-3-Clause"
-packages = [{include="mf"}]
+packages = [{include="mf.py"}]
 
 [tool.poetry.scripts]
 mf = "mf:main"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
-requests = "^2.28.2"
 beautifulsoup4 = "^4.11.2"
-html5lib = "^1.1"
 easyuri = ">=0.1.2"
 txtint = ">=0.1.2"
+mf2py = "^1.1.3"
 
 [tool.poetry.group.dev.dependencies]
 lxml = "^4.9.2"
-gmpg = ">=0.1.3"
-# gmpg = {path="../gmpg", develop=true}
-# easyuri = {path="../easyuri", develop=true}
+gmpg = {path="../gmpg", develop=true}
+easyuri = {path="../easyuri", develop=true}
 
 # [[tool.poetry.source]]
 # name = "main"
 # url = "https://ragt.ag/code/pypi"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `microformats-0.3.4/setup.py` & `microformats-0.3.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,32 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
-packages = \
-['mf', 'mf.parser', 'mf.parser.backcompat', 'mf.parser.prop_util']
-
-package_data = \
-{'': ['*']}
-
+modules = \
+['mf']
 install_requires = \
 ['beautifulsoup4>=4.11.2,<5.0.0',
  'easyuri>=0.1.2',
- 'html5lib>=1.1,<2.0',
- 'requests>=2.28.2,<3.0.0',
+ 'mf2py>=1.1.3,<2.0.0',
  'txtint>=0.1.2']
 
 entry_points = \
 {'console_scripts': ['mf = mf:main']}
 
 setup_kwargs = {
     'name': 'microformats',
-    'version': '0.3.4',
+    'version': '0.3.5',
     'description': 'tools for microformats production, consumption and analysis',
-    'long_description': '[microformats][0] are the simplest way to openly publish contacts, events,\nreviews, recipes, and other structured information on the web.\n\n    >>> import mf\n    >>> url = "https://alice.example"\n    >>> doc = mf.parse(doc=f\'\'\'\n    ... <p class=h-card><a href={url}>Alice</a></p>\n    ... <ul class=h-feed>\n    ... <li class=h-entry>foo\n    ... <li class=h-entry>bar\n    ... </ul>\n    ... \'\'\', url=url)\n\n    # TODO >>> dict(doc)\n    # TODO >>> doc.json\n\n    >>> card = doc["items"][0]\n    >>> card["type"]\n    [\'h-card\']\n    >>> card["properties"]\n    {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n    >>> feed = doc["items"][1]\n    >>> feed["children"][0]["properties"]["name"]\n    [\'foo\']\n\n    >>> mf.util.representative_card(doc, url)\n    {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n    >>> mf.util.representative_feed(doc, url)["items"][0]["name"]\n    [\'foo\']\n\n    # TODO >>> doc.representative_card\n    # TODO {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n    # TODO >>> doc.representative_feed["items"][0]["name"]\n    # TODO [\'foo\']\n\nBased upon [`mf2py`][1] and [`mf2util`][2].\n\n[0]: https://microformats.org/wiki/microformats\n[1]: https://github.com/microformats/mf2py\n[2]: https://github.com/kylewm/mf2util\n',
+    'long_description': '[microformats][0] are the simplest way to openly publish contacts, events,\nreviews, recipes, and other structured information on the web.\n\n    >>> import mf\n    >>> url = "https://alice.example"\n    >>> doc = f\'\'\'\n    ... <p class=h-card><a href={url}>Alice</a></p>\n    ... <ul class=h-feed>\n    ... <li class=h-entry>foo\n    ... <li class=h-entry>bar\n    ... </ul>\n    ... \'\'\'\n    >>> page = mf.parse(doc=doc, url=url)\n\n    # TODO >>> dict(page)\n    # TODO >>> page.json\n\n    >>> card = page["items"][0]\n    >>> card["type"]\n    [\'h-card\']\n    >>> card["properties"]\n    {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n    >>> feed = page["items"][1]\n    >>> feed["children"][0]["properties"]["name"]\n    [\'foo\']\n\n    >>> mf.util.representative_card(page, url)\n    {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n    >>> mf.util.representative_feed(page, url)["items"][0]["name"]\n    [\'foo\']\n\n    # TODO >>> page.representative_card\n    # TODO {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n    # TODO >>> page.representative_feed["items"][0]["name"]\n    # TODO [\'foo\']\n\nBased upon [`mf2py`][1] and [`mf2util`][2].\n\n[0]: https://microformats.org/wiki/microformats\n[1]: https://github.com/microformats/mf2py\n[2]: https://github.com/kylewm/mf2util\n',
     'author': 'Angelo Gladding',
     'author_email': 'angelo@ragt.ag',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://ragt.ag/code/python-microformats',
-    'packages': packages,
-    'package_data': package_data,
+    'py_modules': modules,
     'install_requires': install_requires,
     'entry_points': entry_points,
     'python_requires': '>=3.8,<3.11',
 }
 
 
 setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,33 +1,31 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['mf',
-'mf.parser', 'mf.parser.backcompat', 'mf.parser.prop_util'] package_data = \
-{'': ['*']} install_requires = \ ['beautifulsoup4>=4.11.2,<5.0.0',
-'easyuri>=0.1.2', 'html5lib>=1.1,<2.0', 'requests>=2.28.2,<3.0.0',
-'txtint>=0.1.2'] entry_points = \ {'console_scripts': ['mf = mf:main']}
-setup_kwargs = { 'name': 'microformats', 'version': '0.3.4', 'description':
-'tools for microformats production, consumption and analysis',
+# -*- coding: utf-8 -*- from setuptools import setup modules = \ ['mf']
+install_requires = \ ['beautifulsoup4>=4.11.2,<5.0.0', 'easyuri>=0.1.2',
+'mf2py>=1.1.3,<2.0.0', 'txtint>=0.1.2'] entry_points = \ {'console_scripts':
+['mf = mf:main']} setup_kwargs = { 'name': 'microformats', 'version': '0.3.5',
+'description': 'tools for microformats production, consumption and analysis',
 'long_description': '[microformats][0] are the simplest way to openly publish
 contacts, events,\nreviews, recipes, and other structured information on the
-web.\n\n >>> import mf\n >>> url = "https://alice.example"\n >>> doc = mf.parse
-(doc=f\'\'\'\n ...
+web.\n\n >>> import mf\n >>> url = "https://alice.example"\n >>> doc =
+f\'\'\'\n ...
 Alice
 \n ...
     * \n ...
     * foo\n ...
     * bar\n ...
-\n ... \'\'\', url=url)\n\n # TODO >>> dict(doc)\n # TODO >>> doc.json\n\n >>>
-card = doc["items"][0]\n >>> card["type"]\n [\'h-card\']\n >>> card
-["properties"]\n {\'name\': [\'Alice\'], \'url\': [\'https://
-alice.example\']}\n >>> feed = doc["items"][1]\n >>> feed["children"][0]
-["properties"]["name"]\n [\'foo\']\n\n >>> mf.util.representative_card(doc,
-url)\n {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n >>>
-mf.util.representative_feed(doc, url)["items"][0]["name"]\n [\'foo\']\n\n #
-TODO >>> doc.representative_card\n # TODO {\'name\': [\'Alice\'], \'url\':
-[\'https://alice.example\']}\n # TODO >>> doc.representative_feed["items"][0]
-["name"]\n # TODO [\'foo\']\n\nBased upon [`mf2py`][1] and [`mf2util`][2].\n\n
-[0]: https://microformats.org/wiki/microformats\n[1]: https://github.com/
-microformats/mf2py\n[2]: https://github.com/kylewm/mf2util\n', 'author':
-'Angelo Gladding', 'author_email': 'angelo@ragt.ag', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://ragt.ag/code/python-microformats',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.8,<3.11', } setup(**setup_kwargs)
+\n ... \'\'\'\n >>> page = mf.parse(doc=doc, url=url)\n\n # TODO >>> dict
+(page)\n # TODO >>> page.json\n\n >>> card = page["items"][0]\n >>> card
+["type"]\n [\'h-card\']\n >>> card["properties"]\n {\'name\': [\'Alice\'],
+\'url\': [\'https://alice.example\']}\n >>> feed = page["items"][1]\n >>> feed
+["children"][0]["properties"]["name"]\n [\'foo\']\n\n >>>
+mf.util.representative_card(page, url)\n {\'name\': [\'Alice\'], \'url\':
+[\'https://alice.example\']}\n >>> mf.util.representative_feed(page, url)
+["items"][0]["name"]\n [\'foo\']\n\n # TODO >>> page.representative_card\n #
+TODO {\'name\': [\'Alice\'], \'url\': [\'https://alice.example\']}\n # TODO >>>
+page.representative_feed["items"][0]["name"]\n # TODO [\'foo\']\n\nBased upon
+[`mf2py`][1] and [`mf2util`][2].\n\n[0]: https://microformats.org/wiki/
+microformats\n[1]: https://github.com/microformats/mf2py\n[2]: https://
+github.com/kylewm/mf2util\n', 'author': 'Angelo Gladding', 'author_email':
+'angelo@ragt.ag', 'maintainer': 'None', 'maintainer_email': 'None', 'url':
+'https://ragt.ag/code/python-microformats', 'py_modules': modules,
+'install_requires': install_requires, 'entry_points': entry_points,
+'python_requires': '>=3.8,<3.11', } setup(**setup_kwargs)
```

### Comparing `microformats-0.3.4/PKG-INFO` & `microformats-0.3.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 Metadata-Version: 2.1
 Name: microformats
-Version: 0.3.4
+Version: 0.3.5
 Summary: tools for microformats production, consumption and analysis
 Home-page: https://ragt.ag/code/python-microformats
 License: BSD-3-Clause
 Keywords: IndieWeb,microformats
 Author: Angelo Gladding
 Author-email: angelo@ragt.ag
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: easyuri (>=0.1.2)
-Requires-Dist: html5lib (>=1.1,<2.0)
-Requires-Dist: requests (>=2.28.2,<3.0.0)
+Requires-Dist: mf2py (>=1.1.3,<2.0.0)
 Requires-Dist: txtint (>=0.1.2)
 Description-Content-Type: text/markdown
 
 [microformats][0] are the simplest way to openly publish contacts, events,
 reviews, recipes, and other structured information on the web.
 
     >>> import mf
     >>> url = "https://alice.example"
-    >>> doc = mf.parse(doc=f'''
+    >>> doc = f'''
     ... <p class=h-card><a href={url}>Alice</a></p>
     ... <ul class=h-feed>
     ... <li class=h-entry>foo
     ... <li class=h-entry>bar
     ... </ul>
-    ... ''', url=url)
+    ... '''
+    >>> page = mf.parse(doc=doc, url=url)
 
-    # TODO >>> dict(doc)
-    # TODO >>> doc.json
+    # TODO >>> dict(page)
+    # TODO >>> page.json
 
-    >>> card = doc["items"][0]
+    >>> card = page["items"][0]
     >>> card["type"]
     ['h-card']
     >>> card["properties"]
     {'name': ['Alice'], 'url': ['https://alice.example']}
-    >>> feed = doc["items"][1]
+    >>> feed = page["items"][1]
     >>> feed["children"][0]["properties"]["name"]
     ['foo']
 
-    >>> mf.util.representative_card(doc, url)
+    >>> mf.util.representative_card(page, url)
     {'name': ['Alice'], 'url': ['https://alice.example']}
-    >>> mf.util.representative_feed(doc, url)["items"][0]["name"]
+    >>> mf.util.representative_feed(page, url)["items"][0]["name"]
     ['foo']
 
-    # TODO >>> doc.representative_card
+    # TODO >>> page.representative_card
     # TODO {'name': ['Alice'], 'url': ['https://alice.example']}
-    # TODO >>> doc.representative_feed["items"][0]["name"]
+    # TODO >>> page.representative_feed["items"][0]["name"]
     # TODO ['foo']
 
 Based upon [`mf2py`][1] and [`mf2util`][2].
 
 [0]: https://microformats.org/wiki/microformats
 [1]: https://github.com/microformats/mf2py
 [2]: https://github.com/kylewm/mf2util
```

#### html2text {}

```diff
@@ -1,30 +1,29 @@
-Metadata-Version: 2.1 Name: microformats Version: 0.3.4 Summary: tools for
+Metadata-Version: 2.1 Name: microformats Version: 0.3.5 Summary: tools for
 microformats production, consumption and analysis Home-page: https://ragt.ag/
 code/python-microformats License: BSD-3-Clause Keywords: IndieWeb,microformats
 Author: Angelo Gladding Author-email: angelo@ragt.ag Requires-Python:
 >=3.8,<3.11 Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Requires-Dist: beautifulsoup4
-(>=4.11.2,<5.0.0) Requires-Dist: easyuri (>=0.1.2) Requires-Dist: html5lib
-(>=1.1,<2.0) Requires-Dist: requests (>=2.28.2,<3.0.0) Requires-Dist: txtint
-(>=0.1.2) Description-Content-Type: text/markdown [microformats][0] are the
-simplest way to openly publish contacts, events, reviews, recipes, and other
-structured information on the web. >>> import mf >>> url = "https://
-alice.example" >>> doc = mf.parse(doc=f''' ...
+(>=4.11.2,<5.0.0) Requires-Dist: easyuri (>=0.1.2) Requires-Dist: mf2py
+(>=1.1.3,<2.0.0) Requires-Dist: txtint (>=0.1.2) Description-Content-Type:
+text/markdown [microformats][0] are the simplest way to openly publish
+contacts, events, reviews, recipes, and other structured information on the
+web. >>> import mf >>> url = "https://alice.example" >>> doc = f''' ...
 Alice
 ...
     * ...
     * foo ...
     * bar ...
-... ''', url=url) # TODO >>> dict(doc) # TODO >>> doc.json >>> card = doc
-["items"][0] >>> card["type"] ['h-card'] >>> card["properties"] {'name':
-['Alice'], 'url': ['https://alice.example']} >>> feed = doc["items"][1] >>>
-feed["children"][0]["properties"]["name"] ['foo'] >>>
-mf.util.representative_card(doc, url) {'name': ['Alice'], 'url': ['https://
-alice.example']} >>> mf.util.representative_feed(doc, url)["items"][0]["name"]
-['foo'] # TODO >>> doc.representative_card # TODO {'name': ['Alice'], 'url':
-['https://alice.example']} # TODO >>> doc.representative_feed["items"][0]
+... ''' >>> page = mf.parse(doc=doc, url=url) # TODO >>> dict(page) # TODO >>>
+page.json >>> card = page["items"][0] >>> card["type"] ['h-card'] >>> card
+["properties"] {'name': ['Alice'], 'url': ['https://alice.example']} >>> feed =
+page["items"][1] >>> feed["children"][0]["properties"]["name"] ['foo'] >>>
+mf.util.representative_card(page, url) {'name': ['Alice'], 'url': ['https://
+alice.example']} >>> mf.util.representative_feed(page, url)["items"][0]["name"]
+['foo'] # TODO >>> page.representative_card # TODO {'name': ['Alice'], 'url':
+['https://alice.example']} # TODO >>> page.representative_feed["items"][0]
 ["name"] # TODO ['foo'] Based upon [`mf2py`][1] and [`mf2util`][2]. [0]: https:
 //microformats.org/wiki/microformats [1]: https://github.com/microformats/mf2py
 [2]: https://github.com/kylewm/mf2util
```

