# Comparing `tmp/numbers_parser-4.4.0.tar.gz` & `tmp/numbers_parser-4.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numbers_parser-4.4.0.tar", max compression
+gzip compressed data, was "numbers_parser-4.4.1.tar", max compression
```

## Comparing `numbers_parser-4.4.0.tar` & `numbers_parser-4.4.1.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.4.0/LICENSE.rst
--rw-r--r--   0        0        0    23217 2023-08-04 06:26:31.735290 numbers_parser-4.4.0/README.md
--rw-r--r--   0        0        0     2130 2023-08-04 06:48:45.358692 numbers_parser-4.4.0/pyproject.toml
--rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.4.0/src/numbers_parser/__init__.py
--rw-r--r--   0        0        0     4336 2023-08-02 13:30:28.000000 numbers_parser-4.4.0/src/numbers_parser/_cat_numbers.py
--rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.4.0/src/numbers_parser/_unpack_numbers.py
--rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.4.0/src/numbers_parser/bullets.py
--rw-r--r--   0        0        0    25629 2023-08-04 06:45:07.855203 numbers_parser-4.4.0/src/numbers_parser/cell.py
--rw-r--r--   0        0        0    28815 2023-08-04 06:26:26.428210 numbers_parser-4.4.0/src/numbers_parser/cell_storage.py
--rw-r--r--   0        0        0     1900 2023-08-04 06:22:03.075998 numbers_parser-4.4.0/src/numbers_parser/constants.py
--rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.4.0/src/numbers_parser/containers.py
--rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.4.0/src/numbers_parser/data/empty.numbers
--rw-r--r--   0        0        0    20435 2023-08-02 13:27:23.000000 numbers_parser-4.4.0/src/numbers_parser/document.py
--rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.4.0/src/numbers_parser/exceptions.py
--rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.4.0/src/numbers_parser/experimental.py
--rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.4.0/src/numbers_parser/file.py
--rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.4.0/src/numbers_parser/formula.py
--rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_pb2.py
--rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_sos_pb2.py
--rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_pb2.py
--rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_pb2.py
--rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py
--rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.4.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
--rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.4.0/src/numbers_parser/generated/TSCEArchives_pb2.py
--rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.4.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py
--rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
--rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
--rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_pb2.py
--rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
--rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
--rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.4.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
--rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_pb2.py
--rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py
--rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.4.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py
--rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_pb2.py
--rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py
--rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.4.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
--rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.4.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
--rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.4.0/src/numbers_parser/generated/TSPMessages_pb2.py
--rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_pb2.py
--rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py
--rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_pb2.py
--rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py
--rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.4.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py
--rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.4.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
--rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_pb2.py
--rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
--rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.4.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
--rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.4.0/src/numbers_parser/generated/__init__.py
--rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.4.0/src/numbers_parser/generated/fontmap.py
--rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.4.0/src/numbers_parser/generated/functionmap.py
--rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.4.0/src/numbers_parser/iwafile.py
--rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.4.0/src/numbers_parser/mapping.py
--rw-r--r--   0        0        0    91156 2023-08-04 06:41:22.104247 numbers_parser-4.4.0/src/numbers_parser/model.py
--rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.4.0/src/numbers_parser/numbers_uuid.py
--rw-r--r--   0        0        0    24433 1970-01-01 00:00:00.000000 numbers_parser-4.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1050 2022-06-23 17:13:17.000000 numbers_parser-4.4.1/LICENSE.rst
+-rw-r--r--   0        0        0    23217 2023-08-04 06:26:31.735290 numbers_parser-4.4.1/README.md
+-rw-r--r--   0        0        0     2130 2023-08-05 14:11:42.204167 numbers_parser-4.4.1/pyproject.toml
+-rw-r--r--   0        0        0     2081 2023-07-23 15:54:51.138965 numbers_parser-4.4.1/src/numbers_parser/__init__.py
+-rw-r--r--   0        0        0     4336 2023-08-02 13:30:28.000000 numbers_parser-4.4.1/src/numbers_parser/_cat_numbers.py
+-rw-r--r--   0        0        0     5784 2023-07-23 15:54:51.177251 numbers_parser-4.4.1/src/numbers_parser/_unpack_numbers.py
+-rw-r--r--   0        0        0     2616 2023-05-20 02:42:59.000000 numbers_parser-4.4.1/src/numbers_parser/bullets.py
+-rw-r--r--   0        0        0    25629 2023-08-04 06:45:07.855203 numbers_parser-4.4.1/src/numbers_parser/cell.py
+-rw-r--r--   0        0        0    29077 2023-08-04 13:45:04.678377 numbers_parser-4.4.1/src/numbers_parser/cell_storage.py
+-rw-r--r--   0        0        0     1900 2023-08-04 06:22:03.075998 numbers_parser-4.4.1/src/numbers_parser/constants.py
+-rw-r--r--   0        0        0     4239 2023-07-14 19:05:10.687308 numbers_parser-4.4.1/src/numbers_parser/containers.py
+-rwxr-xr-x   0        0        0    90316 2023-07-31 12:19:08.304273 numbers_parser-4.4.1/src/numbers_parser/data/empty.numbers
+-rw-r--r--   0        0        0    20685 2023-08-05 14:09:43.860076 numbers_parser-4.4.1/src/numbers_parser/document.py
+-rw-r--r--   0        0        0      663 2022-10-17 17:39:14.019486 numbers_parser-4.4.1/src/numbers_parser/exceptions.py
+-rw-r--r--   0        0        0      374 2023-07-16 14:30:53.391296 numbers_parser-4.4.1/src/numbers_parser/experimental.py
+-rw-r--r--   0        0        0     3683 2023-07-23 15:54:51.189959 numbers_parser-4.4.1/src/numbers_parser/file.py
+-rw-r--r--   0        0        0    10665 2023-07-14 19:05:10.689467 numbers_parser-4.4.1/src/numbers_parser/formula.py
+-rw-r--r--   0        0        0    16007 2023-07-23 16:06:40.954866 numbers_parser-4.4.1/src/numbers_parser/generated/TNArchives_pb2.py
+-rw-r--r--   0        0        0     1215 2023-07-23 16:06:40.955183 numbers_parser-4.4.1/src/numbers_parser/generated/TNArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18271 2023-07-23 16:06:40.955417 numbers_parser-4.4.1/src/numbers_parser/generated/TNCommandArchives_pb2.py
+-rw-r--r--   0        0        0     1857 2023-07-23 16:06:40.955655 numbers_parser-4.4.1/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    17361 2023-07-23 16:06:40.955915 numbers_parser-4.4.1/src/numbers_parser/generated/TSAArchives_pb2.py
+-rw-r--r--   0        0        0     2033 2023-07-23 16:06:40.956132 numbers_parser-4.4.1/src/numbers_parser/generated/TSAArchives_sos_pb2.py
+-rw-r--r--   0        0        0     3907 2023-07-23 16:06:40.956319 numbers_parser-4.4.1/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py
+-rw-r--r--   0        0        0    64955 2023-07-23 16:06:40.956672 numbers_parser-4.4.1/src/numbers_parser/generated/TSCEArchives_pb2.py
+-rw-r--r--   0        0        0    11162 2023-07-23 16:06:40.957188 numbers_parser-4.4.1/src/numbers_parser/generated/TSCH3DArchives_pb2.py
+-rw-r--r--   0        0        0     8655 2023-07-23 16:06:40.957541 numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_Common_pb2.py
+-rw-r--r--   0        0        0    46323 2023-07-23 16:06:40.957794 numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py
+-rw-r--r--   0        0        0    22717 2023-07-23 16:06:40.958066 numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_pb2.py
+-rw-r--r--   0        0        0    63730 2023-07-23 16:06:40.958325 numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_sos_pb2.py
+-rw-r--r--   0        0        0    27446 2023-07-23 16:06:40.958670 numbers_parser-4.4.1/src/numbers_parser/generated/TSCHCommandArchives_pb2.py
+-rw-r--r--   0        0        0    30051 2023-07-23 16:06:40.959087 numbers_parser-4.4.1/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py
+-rw-r--r--   0        0        0    40151 2023-07-23 16:06:40.959435 numbers_parser-4.4.1/src/numbers_parser/generated/TSDArchives_pb2.py
+-rw-r--r--   0        0        0     6022 2023-07-23 16:06:40.959684 numbers_parser-4.4.1/src/numbers_parser/generated/TSDArchives_sos_pb2.py
+-rw-r--r--   0        0        0    29192 2023-07-23 16:06:40.959950 numbers_parser-4.4.1/src/numbers_parser/generated/TSDCommandArchives_pb2.py
+-rw-r--r--   0        0        0    53520 2023-07-23 16:06:40.960332 numbers_parser-4.4.1/src/numbers_parser/generated/TSKArchives_pb2.py
+-rw-r--r--   0        0        0     1941 2023-07-23 16:06:40.960544 numbers_parser-4.4.1/src/numbers_parser/generated/TSKArchives_sos_pb2.py
+-rw-r--r--   0        0        0    18142 2023-07-23 16:06:40.960804 numbers_parser-4.4.1/src/numbers_parser/generated/TSPArchiveMessages_pb2.py
+-rw-r--r--   0        0        0     2024 2023-07-23 16:06:40.961046 numbers_parser-4.4.1/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py
+-rw-r--r--   0        0        0    12611 2023-07-23 16:06:40.961302 numbers_parser-4.4.1/src/numbers_parser/generated/TSPMessages_pb2.py
+-rw-r--r--   0        0        0     9717 2023-07-23 16:06:40.961563 numbers_parser-4.4.1/src/numbers_parser/generated/TSSArchives_pb2.py
+-rw-r--r--   0        0        0     2842 2023-07-23 16:06:40.961856 numbers_parser-4.4.1/src/numbers_parser/generated/TSSArchives_sos_pb2.py
+-rw-r--r--   0        0        0    88532 2023-07-23 16:06:40.962320 numbers_parser-4.4.1/src/numbers_parser/generated/TSTArchives_pb2.py
+-rw-r--r--   0        0        0    12597 2023-07-23 16:06:40.962544 numbers_parser-4.4.1/src/numbers_parser/generated/TSTArchives_sos_pb2.py
+-rw-r--r--   0        0        0    59523 2023-07-23 16:06:40.963108 numbers_parser-4.4.1/src/numbers_parser/generated/TSTCommandArchives_pb2.py
+-rw-r--r--   0        0        0    12644 2023-07-23 16:06:40.963347 numbers_parser-4.4.1/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py
+-rw-r--r--   0        0        0    58663 2023-07-23 16:06:40.963755 numbers_parser-4.4.1/src/numbers_parser/generated/TSWPArchives_pb2.py
+-rw-r--r--   0        0        0    28840 2023-07-23 16:06:40.964041 numbers_parser-4.4.1/src/numbers_parser/generated/TSWPArchives_sos_pb2.py
+-rw-r--r--   0        0        0    25441 2023-07-23 16:06:40.964356 numbers_parser-4.4.1/src/numbers_parser/generated/TSWPCommandArchives_pb2.py
+-rw-r--r--   0        0        0        0 2023-07-23 16:06:40.970289 numbers_parser-4.4.1/src/numbers_parser/generated/__init__.py
+-rw-r--r--   0        0        0    22604 2023-07-23 16:06:33.784957 numbers_parser-4.4.1/src/numbers_parser/generated/fontmap.py
+-rw-r--r--   0        0        0     6082 2023-07-23 16:06:33.032684 numbers_parser-4.4.1/src/numbers_parser/generated/functionmap.py
+-rw-r--r--   0        0        0    11868 2023-07-23 15:54:51.253681 numbers_parser-4.4.1/src/numbers_parser/iwafile.py
+-rw-r--r--   0        0        0    32117 2023-07-23 16:07:16.807745 numbers_parser-4.4.1/src/numbers_parser/mapping.py
+-rw-r--r--   0        0        0    91399 2023-08-05 14:10:35.446358 numbers_parser-4.4.1/src/numbers_parser/model.py
+-rw-r--r--   0        0        0     2642 2023-07-23 15:54:51.198744 numbers_parser-4.4.1/src/numbers_parser/numbers_uuid.py
+-rw-r--r--   0        0        0    24433 1970-01-01 00:00:00.000000 numbers_parser-4.4.1/PKG-INFO
```

### Comparing `numbers_parser-4.4.0/LICENSE.rst` & `numbers_parser-4.4.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/README.md` & `numbers_parser-4.4.1/README.md`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/pyproject.toml` & `numbers_parser-4.4.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 description = "Read and write Apple Numbers spreadsheets"
 documentation = "https://github.com/masaccio/numbers-parser/blob/main/README.md"
 license = "MIT"
 name = "numbers-parser"
 packages = [{include = "numbers_parser", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/numbers-parser"
-version = "4.4.0"
+version = "4.4.1"
 
 [tool.poetry.scripts]
 cat-numbers = "numbers_parser._cat_numbers:main"
 unpack-numbers = "numbers_parser._unpack_numbers:main"
 
 [tool.poetry.dependencies]
 compact-json = "^1.1.3"
```

### Comparing `numbers_parser-4.4.0/src/numbers_parser/__init__.py` & `numbers_parser-4.4.1/src/numbers_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/_cat_numbers.py` & `numbers_parser-4.4.1/src/numbers_parser/_cat_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/_unpack_numbers.py` & `numbers_parser-4.4.1/src/numbers_parser/_unpack_numbers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/bullets.py` & `numbers_parser-4.4.1/src/numbers_parser/bullets.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/cell.py` & `numbers_parser-4.4.1/src/numbers_parser/cell.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/cell_storage.py` & `numbers_parser-4.4.1/src/numbers_parser/cell_storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -525,20 +525,16 @@
                 index += 1
         else:
             formatted_value += current_char
             index += 1
     return formatted_value
 
 
-# import inspect
-
-
 def decode_number_format(format, value, name):  # noqa: C901
     """Parse a custom date format string and return a formatted number value"""
-    # cell = inspect.currentframe().f_back.f_back.f_back.f_locals["self"]
     custom_format_string = format.custom_format_string
     value *= format.scale_factor
     if "%" in custom_format_string and format.scale_factor == 1.0:
         # Per cent scale has 100x but % does not
         value *= 100.0
 
     if format.currency_code != "":
@@ -610,16 +606,25 @@
         else:
             int_pad = CellPadding.SPACE
             int_width = len(int_part)
     else:
         int_pad = None
         int_width = num_integers
 
-    # if num_integers == 0 and dec_pad == CellPadding.SPACE:
-    #     dec_pad = CellPadding.ZERO
+    # value_1 = str(value).split(".")[0]
+    # value_2 = sigfig.round(str(value).split(".")[1], sigfig=MAX_SIGNIFICANT_DIGITS, warn=False)
+    # int_pad_space_as_zero = (
+    #     num_integers > 0
+    #     and num_decimals > 0
+    #     and int_pad == CellPadding.SPACE
+    #     and dec_pad is None
+    #     and num_integers > len(value_1)
+    #     and num_decimals > len(value_2)
+    # )
+    int_pad_space_as_zero = False
 
     # Formatting integer zero:
     #   Blank (padded if needed) if int_pad is SPACE and no decimals
     #   No leading zero if:
     #     int_pad is NONE, dec_pad is SPACE
     #     int_pad is SPACE, dec_pad is SPACE
     #     int_pad is SPACE, dec_pad is ZERO
@@ -633,15 +638,15 @@
     elif (
         integer == 0
         and int_pad == CellPadding.SPACE
         and dec_pad is None
         and len(str(decimal)) > num_decimals
     ):
         formatted_value = "".rjust(int_width)
-    elif int_pad == CellPadding.ZERO:
+    elif int_pad_space_as_zero or int_pad == CellPadding.ZERO:
         if format.show_thousands_separator:
             formatted_value = f"{integer:0{int_width},}"
         else:
             formatted_value = f"{integer:0{int_width}}"
     elif int_pad == CellPadding.SPACE:
         if format.show_thousands_separator:
             formatted_value = f"{integer:,}".rjust(int_width)
```

### Comparing `numbers_parser-4.4.0/src/numbers_parser/constants.py` & `numbers_parser-4.4.1/src/numbers_parser/constants.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/containers.py` & `numbers_parser-4.4.1/src/numbers_parser/containers.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/data/empty.numbers` & `numbers_parser-4.4.1/src/numbers_parser/data/empty.numbers`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/document.py` & `numbers_parser-4.4.1/src/numbers_parser/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,22 @@
 
     @name.setter
     def name(self, value: str):
         """Set the table's name"""
         self._model.table_name(self._table_id, value)
 
     @property
+    def table_name_enabled(self):
+        return self._model.table_name_enabled(self._table_id)
+
+    @table_name_enabled.setter
+    def table_name_enabled(self, enabled):
+        self._model.table_name_enabled(self._table_id, enabled)
+
+    @property
     def num_header_rows(self) -> int:
         """Return the number of header rows"""
         return self._model.num_header_rows(self._table_id)
 
     @num_header_rows.setter
     def num_header_rows(self, num_headers: int):
         """Return the number of header rows"""
```

### Comparing `numbers_parser-4.4.0/src/numbers_parser/exceptions.py` & `numbers_parser-4.4.1/src/numbers_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/file.py` & `numbers_parser-4.4.1/src/numbers_parser/file.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/formula.py` & `numbers_parser-4.4.1/src/numbers_parser/formula.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TNArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TNArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TNArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TNCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TNCommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSAArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSAArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSAArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSACommandArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCEArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCEArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCH3DArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCH3DArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_Common_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_Common_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_GEN_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCHArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHCommandArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCHCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSCHPreUFFArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSDArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSDArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSDArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSDCommandArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSDCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSKArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSKArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSKArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSPArchiveMessages_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSPArchiveMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSPDatabaseMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSPMessages_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSPMessages_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSSArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSSArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSSArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSTArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSTArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSTArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSTCommandArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSTCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSTStylePropertyArchiving_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSWPArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSWPArchives_sos_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSWPArchives_sos_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/TSWPCommandArchives_pb2.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/TSWPCommandArchives_pb2.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/fontmap.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/fontmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/generated/functionmap.py` & `numbers_parser-4.4.1/src/numbers_parser/generated/functionmap.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/iwafile.py` & `numbers_parser-4.4.1/src/numbers_parser/iwafile.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/mapping.py` & `numbers_parser-4.4.1/src/numbers_parser/mapping.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/src/numbers_parser/model.py` & `numbers_parser-4.4.1/src/numbers_parser/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -317,14 +317,20 @@
 
     def table_name(self, table_id, value=None):
         if value is None:
             return self.objects[table_id].table_name
         else:
             self.objects[table_id].table_name = value
 
+    def table_name_enabled(self, table_id: int, enabled: bool = None):
+        if enabled is not None:
+            self.objects[table_id].table_name_enabled = enabled
+        else:
+            return self.objects[table_id].table_name_enabled
+
     @lru_cache(maxsize=None)
     def table_tiles(self, table_id):
         bds = self.objects[table_id].base_data_store
         return [self.objects[t.tile.identifier] for t in bds.tiles.tiles]
 
     @lru_cache(maxsize=None)
     def custom_format_map(self):
```

### Comparing `numbers_parser-4.4.0/src/numbers_parser/numbers_uuid.py` & `numbers_parser-4.4.1/src/numbers_parser/numbers_uuid.py`

 * *Files identical despite different names*

### Comparing `numbers_parser-4.4.0/PKG-INFO` & `numbers_parser-4.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: numbers-parser
-Version: 4.4.0
+Version: 4.4.1
 Summary: Read and write Apple Numbers spreadsheets
 Home-page: https://github.com/masaccio/numbers-parser
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

