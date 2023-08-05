# Comparing `tmp/lora_utils-0.1.0.tar.gz` & `tmp/lora_utils-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lora_utils-0.1.0.tar", max compression
+gzip compressed data, was "lora_utils-0.1.1.tar", max compression
```

## Comparing `lora_utils-0.1.0.tar` & `lora_utils-0.1.1.tar`

### file list

```diff
@@ -1,6 +1,5 @@
--rw-r--r--   0        0        0    16725 2022-03-29 13:56:15.522818 lora_utils-0.1.0/LICENSE
--rw-r--r--   0        0        0       30 2022-03-29 13:56:15.522818 lora_utils-0.1.0/lora_utils/__init__.py
--rw-r--r--   0        0        0     3283 2022-03-29 13:56:15.522818 lora_utils-0.1.0/lora_utils/util.py
--rw-r--r--   0        0        0      328 2022-03-29 14:04:25.370212 lora_utils-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      593 2022-03-29 14:04:35.554705 lora_utils-0.1.0/setup.py
--rw-r--r--   0        0        0      442 2022-03-29 14:04:35.555014 lora_utils-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-08-05 16:05:25.238649 lora_utils-0.1.1/LICENSE
+-rw-r--r--   0        0        0       30 2023-08-05 16:05:25.238649 lora_utils-0.1.1/lora_utils/__init__.py
+-rw-r--r--   0        0        0     3333 2023-08-05 16:05:25.238649 lora_utils-0.1.1/lora_utils/util.py
+-rw-r--r--   0        0        0      346 2023-08-05 16:05:25.238649 lora_utils-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      493 1970-01-01 00:00:00.000000 lora_utils-0.1.1/PKG-INFO
```

### Comparing `lora_utils-0.1.0/LICENSE` & `lora_utils-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lora_utils-0.1.0/lora_utils/util.py` & `lora_utils-0.1.1/lora_utils/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,26 +45,28 @@
         entries = obj[group]
 
         for key in keys:
             if key not in entries:
                 continue
 
             for entry in entries[key]:
-                chunks.update((
-                    _parse_timestamp(entry['virkning']['from']),
-                    _parse_timestamp(entry['virkning']['to']),
-                ))
+                chunks.update(
+                    (
+                        _parse_timestamp(entry["virkning"]["from"]),
+                        _parse_timestamp(entry["virkning"]["to"]),
+                    )
+                )
 
     # sort them, and apply the filter, if given
     chunks = get_date_chunks(chunks)
 
     def filter_list(entries, start, end):
         for entry in entries:
-            entry_start = _parse_timestamp(entry['virkning']['from'])
-            entry_end = _parse_timestamp(entry['virkning']['to'])
+            entry_start = _parse_timestamp(entry["virkning"]["from"])
+            entry_end = _parse_timestamp(entry["virkning"]["to"])
 
             if entry_start < end and entry_end > start:
                 yield entry
 
     # finally, extract chunks corresponding to each cut-off
     for start, end in chunks:
         effect = {
@@ -95,17 +97,17 @@
 
     yield from zip(a, b)
 
 
 def _parse_timestamp(
     timestamp: typing.Union[datetime.datetime, str]
 ) -> datetime.datetime:
-    if timestamp == 'infinity':
+    if timestamp == "infinity":
         dt = datetime.datetime.max
-    elif timestamp == '-infinity':
+    elif timestamp == "-infinity":
         dt = datetime.datetime.min
     elif type(timestamp) == str:
         dt = dateutil.parser.isoparse(timestamp)
     elif type(timestamp) == datetime:
         dt = copy.copy(timestamp)
     else:
         raise TypeError("Invalid parameter {}".format(timestamp))
```

