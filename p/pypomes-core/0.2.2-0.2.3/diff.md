# Comparing `tmp/pypomes_core-0.2.2.tar.gz` & `tmp/pypomes_core-0.2.3.tar.gz`

## Comparing `pypomes_core-0.2.2.tar` & `pypomes_core-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,21 @@
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/__init__.py
--rw-r--r--   0        0        0     2321 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/datetime_pomes.py
--rw-r--r--   0        0        0    27324 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/dict_pomes.py
--rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/email_pomes.py
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/encoding_pomes.py
--rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/env_pomes.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/exception_pomes.py
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/file_pomes.py
--rw-r--r--   0        0        0     8572 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/http_pomes.py
--rw-r--r--   0        0        0     2017 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/json_pomes.py
--rw-r--r--   0        0        0     6296 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/list_pomes.py
--rw-r--r--   0        0        0     6755 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/logging_pomes.py
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/str_pomes.py
--rw-r--r--   0        0        0    20320 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/validation_pomes.py
--rw-r--r--   0        0        0     2687 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/src/pypomes_core/xml_pomes.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/.gitignore
--rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/LICENSE
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/README.md
--rw-r--r--   0        0        0      827 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      726 2020-02-02 00:00:00.000000 pypomes_core-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     5834 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/.ruff.toml
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/__init__.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/datetime_pomes.py
+-rw-r--r--   0        0        0    27417 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/dict_pomes.py
+-rw-r--r--   0        0        0     1553 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/email_pomes.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/encoding_pomes.py
+-rw-r--r--   0        0        0     2770 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/env_pomes.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/exception_pomes.py
+-rw-r--r--   0        0        0     1266 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/file_pomes.py
+-rw-r--r--   0        0        0     9280 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/http_pomes.py
+-rw-r--r--   0        0        0     1977 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/json_pomes.py
+-rw-r--r--   0        0        0     6273 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/list_pomes.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/logging_pomes.py
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/str_pomes.py
+-rw-r--r--   0        0        0    20451 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/validation_pomes.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/src/pypomes_core/xml_pomes.py
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/.gitignore
+-rw-r--r--   0        0        0     1086 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/LICENSE
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/README.md
+-rw-r--r--   0        0        0      848 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      754 2020-02-02 00:00:00.000000 pypomes_core-0.2.3/PKG-INFO
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/__init__.py` & `pypomes_core-0.2.3/src/pypomes_core/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,105 +1,110 @@
 from .datetime_pomes import (
     DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
     DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
-    date_reformat, date_parse, datetime_parse
+    TIMEZONE_LOCAL, TIMEZONE_UTC,
+    date_reformat, date_parse, datetime_parse,
 )
 from .dict_pomes import (
     dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
     dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
-    dict_get_keys, dict_from_object, dict_from_list, dict_replace_value, dict_pop_value
+    dict_get_keys, dict_from_object, dict_from_list, dict_replace_value, dict_pop_value,
 )
 from .email_pomes import (
-    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER, email_send
+    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER, email_send,
 )
 from .encoding_pomes import (
-    encode_ascii_hex, decode_ascii_hex
+    encode_ascii_hex, decode_ascii_hex,
 )
 from .env_pomes import (
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float
+    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float, env_get_path,
 )
 from .exception_pomes import (
-    exc_format
+    exc_format,
 )
 from .file_pomes import (
-    file_from_request
+    file_from_request,
 )
 from .http_pomes import (
+    HTTP_DELETE_TIMEOUT, HTTP_GET_TIMEOUT, HTTP_POST_TIMEOUT, HTTP_PUT_TIMEOUT,
     MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
     MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
     MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
     http_status_name, http_status_description,
-    http_json_from_form, http_json_from_request, http_json_from_get, http_json_from_post
+    http_json_from_form, http_json_from_request, http_json_from_get, http_json_from_post,
 )
 from .json_pomes import (
-    json_normalize_dict, json_normalize_iterable
+    json_normalize_dict, json_normalize_iterable,
 )
 from .list_pomes import (
     list_compare, list_flatten, list_unflatten,
-    list_find_coupled, list_elem_starting_with, list_transform
+    list_find_coupled, list_elem_starting_with, list_transform,
 )
 from .logging_pomes import (
     LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
     LOGGING_FILE_PATH, LOGGING_FILE_MODE, PYPOMES_LOGGER,
-    logging_log_msgs, logging_get_entries
+    logging_log_msgs, logging_get_entries,
 )
 from .str_pomes import (
-    str_between, str_split_on_mark, str_find_whitespace
+    str_between, str_split_on_mark, str_find_whitespace,
 )
 from .validation_pomes import (
     VALIDATION_MSG_LANGUAGE, VALIDATION_MSG_PREFIX,
     validate_value, validate_bool, validate_int, validate_float, validate_str,
     validate_date, validate_datetime, validate_ints, validate_strs,
-    validate_format_error, validate_format_errors
+    validate_format_error, validate_format_errors,
 )
 from .xml_pomes import (
-    XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
+    XML_FILE_HEADER, xml_to_dict, xml_normalize_keys,
 )
 
 __all__ = [
     # datetime_pomes
-    DATE_FORMAT_STD, DATE_FORMAT_COMPACT, DATE_FORMAT_INV,
-    DATETIME_FORMAT_STD, DATETIME_FORMAT_COMPACT, DATETIME_FORMAT_INV,
-    date_reformat, date_parse, datetime_parse,
+    "DATE_FORMAT_STD", "DATE_FORMAT_COMPACT", "DATE_FORMAT_INV",
+    "DATETIME_FORMAT_STD", "DATETIME_FORMAT_COMPACT", "DATETIME_FORMAT_INV",
+    "TIMEZONE_LOCAL", "TIMEZONE_UTC",
+    "date_reformat", "date_parse", "datetime_parse",
     # dict_pomes
-    dict_has_key_chain, dict_get_value, dict_set_value, dict_reduce,
-    dict_listify, dict_transform, dict_merge, dict_coalesce, dict_get_key,
-    dict_get_keys, dict_from_object, dict_from_list, dict_replace_value, dict_pop_value,
+    "dict_has_key_chain", "dict_get_value", "dict_set_value", "dict_reduce",
+    "dict_listify", "dict_transform", "dict_merge", "dict_coalesce", "dict_get_key",
+    "dict_get_keys", "dict_from_object", "dict_from_list", "dict_replace_value", "dict_pop_value",
     # email_pomes
-    EMAIL_ACCOUNT, EMAIL_PWD, EMAIL_PORT, EMAIL_SERVER, email_send,
+    "EMAIL_ACCOUNT", "EMAIL_PWD", "EMAIL_PORT", "EMAIL_SERVER", "email_send",
     # encoding_pomes
-    encode_ascii_hex, decode_ascii_hex,
+    "encode_ascii_hex", "decode_ascii_hex",
     # env_pomes
-    APP_PREFIX, env_get_str, env_get_int, env_get_bool, env_get_float,
+    "APP_PREFIX", "env_get_str", "env_get_int", "env_get_bool", "env_get_float", "env_get_path",
     # exception_pomes
-    exc_format,
+    "exc_format",
     # file_pomes
-    file_from_request,
+    "file_from_request",
     # http_pomes
-    MIMETYPE_BINARY, MIMETYPE_CSS, MIMETYPE_CSV, MIMETYPE_HTML, MIMETYPE_JAVASCRIPT,
-    MIMETYPE_JSON, MIMETYPE_MULTIPART, MIMETYPE_PDF, MIMETYPE_PKCS7, MIMETYPE_SOAP,
-    MIMETYPE_TEXT, MIMETYPE_URLENCODED, MIMETYPE_XML, MIMETYPE_ZIP,
-    http_status_name, http_status_description,
-    http_json_from_form, http_json_from_request,
-    http_json_from_get, http_json_from_post,
+    "HTTP_DELETE_TIMEOUT", "HTTP_GET_TIMEOUT", "HTTP_POST_TIMEOUT", "HTTP_PUT_TIMEOUT",
+    "MIMETYPE_BINARY", "MIMETYPE_CSS", "MIMETYPE_CSV", "MIMETYPE_HTML", "MIMETYPE_JAVASCRIPT",
+    "MIMETYPE_JSON", "MIMETYPE_MULTIPART", "MIMETYPE_PDF", "MIMETYPE_PKCS7", "MIMETYPE_SOAP",
+    "MIMETYPE_TEXT", "MIMETYPE_URLENCODED", "MIMETYPE_XML", "MIMETYPE_ZIP",
+    "http_status_name", "http_status_description",
+    "http_json_from_form", "http_json_from_request",
+    "http_json_from_get", "http_json_from_post",
     # json_pomes
-    json_normalize_dict, json_normalize_iterable,
+    "json_normalize_dict", "json_normalize_iterable",
     # list_pomes
-    list_compare, list_flatten, list_unflatten,
-    list_find_coupled, list_elem_starting_with, list_transform,
+    "list_compare", "list_flatten", "list_unflatten",
+    "list_find_coupled", "list_elem_starting_with", "list_transform",
     # logging_pomes
-    LOGGING_ID, LOGGING_LEVEL, LOGGING_FORMAT, LOGGING_STYLE,
-    LOGGING_FILE_PATH, LOGGING_FILE_MODE, PYPOMES_LOGGER,
-    logging_log_msgs, logging_get_entries,
+    "LOGGING_ID", "LOGGING_LEVEL", "LOGGING_FORMAT", "LOGGING_STYLE",
+    "LOGGING_FILE_PATH", "LOGGING_FILE_MODE", "PYPOMES_LOGGER",
+    "logging_log_msgs", "logging_get_entries",
     # validation_pomes
-    VALIDATION_MSG_LANGUAGE, VALIDATION_MSG_PREFIX,
-    validate_value, validate_bool, validate_int, validate_float, validate_str,
-    validate_date, validate_datetime, validate_ints, validate_strs,
-    validate_format_error, validate_format_errors,
+    "VALIDATION_MSG_LANGUAGE", "VALIDATION_MSG_PREFIX",
+    "validate_value", "validate_bool", "validate_int", "validate_float", "validate_str",
+    "validate_date", "validate_datetime", "validate_ints", "validate_strs",
+    "validate_format_error", "validate_format_errors",
     # str_pomes
-    str_between, str_split_on_mark, str_find_whitespace,
+    "str_between", "str_split_on_mark", "str_find_whitespace",
     # xml_pomes
-    XML_FILE_HEADER, xml_to_dict, xml_normalize_keys
+    "XML_FILE_HEADER", "xml_to_dict", "xml_normalize_keys",
 ]
 
-__version__ = "0.2.1"
-__version_info__ = (0, 2, 2)
+from importlib.metadata import version
+__version__ = version("pypomes_core")
+__version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/datetime_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/datetime_pomes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,25 @@
+import pytz
 from datetime import date, datetime
 from dateutil import parser
 from typing import Final
 
+from .env_pomes import APP_PREFIX, env_get_str
+
 # some useful date/datetime formats
 DATE_FORMAT_STD: Final[str] = "%m/%d/%Y"
 DATE_FORMAT_COMPACT: Final[str] = "%Y%m%d"
 DATE_FORMAT_INV: Final[str] = "%Y-%m-%d"
 DATETIME_FORMAT_STD: Final[str] = "%m/%d/%Y %H:%M:%S"
 DATETIME_FORMAT_COMPACT: Final[str] = "%Y%m%d%H%M%S"
 DATETIME_FORMAT_INV: Final[str] = "%Y-%m-%d %H:%M:%S"
 
+TIMEZONE_LOCAL: pytz.BaseTzInfo = pytz.timezone(env_get_str(f"{APP_PREFIX}_TIMEZONE_LOCAL", "America/Sao_Paulo"))
+TIMEZONE_UTC: pytz.BaseTzInfo = pytz.UTC
+
 
 def date_reformat(dt_str: str, to_format: str, **kwargs: any) -> str:
     """
     Convert the date in *dt_str* to the format especified in *to_format*.
 
     The argument *dt_str* must represent a valid date, with or without time-of-day information.
     The argument *to_format* must be a valid format for *date* ou *datetime*.
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/dict_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/dict_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import inspect
-import types
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    import types
 
 
 def dict_has_key_chain(source: dict, key_chain: list[str]) -> bool:
     """
     Indicate the existence of an element in *source* pointed to by the nested keys chain *[keys[0]: ... :keys[n]*.
 
     The path up to he last key in the chain must point to an existing element.
@@ -81,14 +84,16 @@
         # dos the key refer to an elemenent in a list ?
         if key[-1] == "]":
             # yes, retrieve it
             pos: int = key.find("[")
             inx: int = int(key[pos+1:-1])
             result = result.get(key[:pos])
 
+            result = result[inx] if isinstance(result, list) and len(result) > inx else None
+
             # is it possible to proceed ?
             if isinstance(result, list) and len(result) > inx:
                 # yes, proceed
                 result = result[inx]
             else:
                 # no, abort the operation
                 result = None
@@ -367,17 +372,17 @@
                     # o item da lista é um dicionário ?
                     if isinstance(in_dict, dict):
                         # sim, coalesça-o recursivamente
                         dict_coalesce(in_dict, key_chain[inx + 1:])
                 # termina a operação
                 curr_dict = None
                 break
-            else:
-                # não, prossiga com o valor associado a key
-                curr_dict = curr_dict.get(key)
+
+            # prossiga com o valor associado a key
+            curr_dict = curr_dict.get(key)
 
         # curr_dict é um dicionário contendo a penúltima chave ?
         if isinstance(curr_dict, dict) and \
            isinstance(curr_dict.get(key_chain[-2]), list):
             # sim, prossiga com o coalescimento
             penultimate_elem: list[dict] = curr_dict.pop(key_chain[-2])
             penultimate_list: list[dict] = []
@@ -463,17 +468,17 @@
                     # o item da lista é um dicionário ?
                     if isinstance(in_dict, dict):
                         # sim, reduza-o recursivamente
                         dict_reduce(in_dict, key_chain[inx + 1:])
                 # termine a operação
                 curr_dict = None
                 break
-            else:
-                # não, prossiga com o valor associado a key
-                curr_dict = curr_dict.get(key)
+
+            # prossiga com o valor associado a key
+            curr_dict = curr_dict.get(key)
 
         last_key: str = key_chain[-1]
         # curr_dict contem um dicionário associado a last_key ?
         if isinstance(curr_dict, dict) and \
            isinstance(curr_dict.get(last_key), dict):
             # sim, prossiga com a redução
             last: dict = curr_dict.pop(last_key)
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/email_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/email_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.2/src/pypomes_core/encoding_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/encoding_pomes.py`

 * *Files 8% similar despite different names*

```diff
@@ -71,17 +71,15 @@
         shift: int = 2
         match next_byte:
             case b"x":
                 # "\x" prefixa um character denotado por string hexadecimal ("\x00" a "\xff")
                 # HAZARD: chars intermediários necessários - int(byte) quebra para byte > b"\x09"
                 upper_char: str = source[pos2+2:pos2+3].decode()
                 lower_char: str = source[pos2+3:pos2+4].decode()
-                # print(upper_char, lower_char)
                 int_val: int = 16 * int(upper_char, base=16) + int(lower_char, base=16)
-                # int_val = int.from_bytes(source[pos2+2:pos2+4], "big")
                 byte_val = bytes([int_val])
                 shift = 4
             case b"n":
                 byte_val = b"\x0A"                  # LF, \n - line feed
             case b"r":
                 byte_val = b"\x0D"                  # CR, \r - carriage return
             case b"t":
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/env_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/env_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import os
+from pathlib import Path
 
 
 def env_get_str(key: str, def_value: str = None) -> str:
     """
     Retrieve and return the string value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
-    :return: The int value associated with the key
+    :return: The str value associated with the key
     """
     result: str
     try:
         result = os.environ[key]
     except (KeyError, TypeError):
         result = def_value
 
@@ -20,15 +21,15 @@
 
 def env_get_bool(key: str, def_value: bool = None) -> bool:
     """
     Retrieve and return the boolean value defined for *key* in the current operating environment.
 
     :param key: The key the value is associated with
     :param def_value: The default value to return, if the key has not been defined
-    :return: The boolean value associated with the key
+    :return: The bool value associated with the key
     """
     result: bool
     try:
         result = bool(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
@@ -65,9 +66,26 @@
         result = int(os.environ[key])
     except (KeyError, TypeError):
         result = def_value
 
     return result
 
 
+def env_get_path(key: str, def_value: Path = None) -> Path:
+    """
+    Retrieve and return the string value defined for *key* in the current operating environment.
+
+    :param key: The key the value is associated with
+    :param def_value: The default value to return, if the key has not been defined
+    :return: The path value associated with the key
+    """
+    result: Path
+    try:
+        result = Path(os.environ[key])
+    except (KeyError, TypeError):
+        result = def_value
+
+    return result
+
+
 # the prefix to the names of the environment variables
 APP_PREFIX = env_get_str("PYPOMES_APP_PREFIX", "PYPOMES")
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/exception_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/exception_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from types import TracebackType
 import os
-import traceback
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    import traceback
 
 
 def exc_format(exc: Exception,
                exc_info: tuple[type[BaseException], BaseException, TracebackType]) -> str:
     """
     Format the error message resulting from the exception raised in execution time.
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/file_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/file_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 from flask import Request
-from werkzeug.datastructures import FileStorage
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from werkzeug.datastructures import FileStorage
 
 
 def file_from_request(request: Request, file_name: str = None, file_seq: int = 0) -> bytes:
     """
     Retrieve and return the contents of the file returned in the response to a request.
 
     The file may be referred to by its name (*file_name*), or if no name is specified,
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/http_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/http_pomes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 import logging
 import requests
 import sys
 from flask import Request
 from typing import Final
 from werkzeug.exceptions import BadRequest
 
+from .env_pomes import APP_PREFIX, env_get_int
 from .exception_pomes import exc_format
 
 # https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status
 
+HTTP_DELETE_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_DELETE_TIMEOUT", 10)
+HTTP_GET_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_GET_TIMEOUT", 10)
+HTTP_POST_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_POST_TIMEOUT", 10)
+HTTP_PUT_TIMEOUT: Final[int] = env_get_int(f"{APP_PREFIX}_HTTP_PUT_TIMEOUT", 10)
+
 MIMETYPE_BINARY: Final[str] = "application/octet-stream"
 MIMETYPE_CSS: Final[str] = "text/css"
 MIMETYPE_CSV: Final[str] = "text/csv"
 MIMETYPE_HTML: Final[str] = "text/html"
 MIMETYPE_JAVASCRIPT: Final[str] = "text/javascript"
 MIMETYPE_JSON: Final[str] = "application/json"
 MIMETYPE_MULTIPART: Final[str] = "multipart/form-data"
@@ -194,30 +200,26 @@
     """
     Return the name of the status message identified to by *status_code*.
 
     :param status_code: the code of the status
     :return: the corresponding name given to the status
     """
     item: dict = __HTTP_STATUS.get(status_code, {"name": "Unknown status code"})
-    result = f"HTTP status code {status_code}: {item.get('name')}"
-                                                             
-    return result
+    return f"HTTP status code {status_code}: {item.get('name')}"
 
 
 def http_status_description(status_code: int) -> str:
     """
     Return the description of the status message identified to by *status_code*.
 
     :param status_code: the code of the status
     :return: the corresponding status description
     """
     item: dict = __HTTP_STATUS.get(status_code, {"description": "Unknown status code"})
-    result = f"HTTP status code {status_code}: {item.get('description')}"
-
-    return result
+    return f"HTTP status code {status_code}: {item.get('description')}"
 
 
 def http_json_from_form(request: Request) -> dict:
     """
     Build and return a *dict* containing the *key-value* pairs of the form parameters found in *request*.
 
     :param request: the HTTP request
@@ -248,83 +250,90 @@
         result: dict = request.get_json()
     except BadRequest:
         resp: str = request.get_data(as_text=True)
         # does the request contain input data ?
         if len(resp) > 0:
             # yes, possibly mal-fomed JSON
             raise
+
     return result
 
 
 def http_json_from_get(errors: list[str], url: str, headers: dict = None,
-                       params: dict = None, logger: logging.Logger = None) -> dict:
+                       params: dict = None, timeout: int = HTTP_GET_TIMEOUT,
+                       logger: logging.Logger = None) -> dict:
     """
     Retrieve a *JSON* string by issuing a *GET* request to the given *url*.
 
     The contents of the *JSON* string are returned as a *dict* .
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
     :param params: optional parameters
+    :param timeout: timeout, in seconds (defaults to HTTP_GET_TIMEOUT - use None to omit)
     :param logger: optional logger to log the operation with
     :return: the contents of the JSON string
     """
     if logger is not None:
         logger.info(f"Invoking GET: '{url}'")
 
     # initialize the return variable
     result: dict | None = None
 
     try:
         response: requests.Response = requests.get(url=url,
                                                    headers=headers,
-                                                   params=params)
+                                                   params=params,
+                                                   timeout=timeout)
         if logger is not None:
             logger.info(f"Invoked '{url}', status: '{http_status_name(response.status_code)}'")
         result = response.json()
     except Exception as e:
         msg: str = f"Error invoking '{url}': '{exc_format(e, sys.exc_info())}'"
         if logger is not None:
             logger.info(msg)
         errors.append(msg)
 
     return result
 
 
 def http_json_from_post(errors: list[str], url: str, headers: dict = None, params: dict = None,
-                        data: dict = None, json: dict = None, logger: logging.Logger = None) -> dict:
+                        data: dict = None, json: dict = None, timeout: int = HTTP_GET_TIMEOUT,
+                        logger: logging.Logger = None) -> dict:
     """
     Retrieve a *JSON* string by issuing a *POST* request to the given *url*.
 
     The contents of the *JSON* string are returned as a *dict* .
     The request might contain *headers* and *parameters*.
 
     :param errors: incidental error messages
     :param url: the destination URL
     :param headers: optional headers
     :param params: optional parameters
     :param data: optionaL data to send in the body of the request
     :param json: optional JSON to send in the body of the request
+    :param timeout: timeout, in seconds (defaults to HTTP_GET_TIMEOUT - use None to omit)
     :param logger: optional logger to log the operation with
     :return: the contents of the JSON string
     """
     if logger is not None:
         logger.info(f"Invoking POST: '{url}'")
 
     # initialize the return variable
     result: dict | None = None
 
     try:
         response: requests.Response = requests.post(url=url,
                                                     headers=headers,
                                                     data=data,
                                                     json=json,
-                                                    params=params)
+                                                    params=params,
+                                                    timeout=timeout)
         if logger is not None:
             logger.info(f"Invoked '{url}', status: '{http_status_name(response.status_code)}'")
         result = response.json()
     except Exception as e:
         msg: str = f"Error invoking '{url}': '{exc_format(e, sys.exc_info())}'"
         if logger is not None:
             logger.info(msg)
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/json_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/json_pomes.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     HAZARD: depending on the type of object contained in *source*, the final result may not be serializable.
 
     :param source: the dict to be made serializable
     """
     for key, value in source.items():
         if isinstance(value, dict):
             json_normalize_dict(value)
-        elif isinstance(value, bytes) or isinstance(value, bytearray):
+        elif isinstance(value, bytes | bytearray):
             source[key] = base64.b64encode(value).decode()
         elif isinstance(value, Iterable) and not isinstance(value, str):
             source[key] = json_normalize_iterable(value)
 
 
 def json_normalize_iterable(source: Iterable) -> list[any]:
     """
@@ -37,15 +37,15 @@
     :return
     """
     result: list[any] = []
     for value in source:
         if isinstance(value, dict):
             json_normalize_dict(value)
             result.append(value)
-        elif isinstance(value, bytes) or isinstance(value, bytearray):
+        elif isinstance(value, bytes | bytearray):
             result.append(base64.b64encode(value).decode())
         elif isinstance(value, Iterable) and not isinstance(value, str):
             result.append(json_normalize_iterable(value))
         else:
             result.append(value)
 
     return result
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/list_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/list_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,17 +39,15 @@
 
     :param source: a lista de strings
     :return: a string concatenada
     """
     result: str = ""
     for item in source:
         result += "." + item
-    result = result[1:]
-
-    return result
+    return result[1:]
 
 
 def list_unflatten(source: str) -> list[str]:
     """
     Transforma uma *str* contendo elementos concatenados por "." em uma lista de *str*.
 
     Essa lista contem os sub_elementos extraídos. Exemplos:
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/logging_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/logging_pomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import logging
-import os
 import tempfile
-from datetime import datetime
 from dateutil import parser
 from io import BytesIO
+from pathlib import Path
 from typing import Final, Literal, TextIO
 from .datetime_pomes import DATETIME_FORMAT_INV
-from .env_pomes import APP_PREFIX, env_get_str
+from .env_pomes import APP_PREFIX, env_get_str, env_get_path
+
+from typing import TYPE_CHECKING
+if TYPE_CHECKING:
+    from datetime import datetime
 
 
 def __get_logging_level(level: Literal["debug", "info", "warning", "error", "critical"]) -> int:
     """
     Translate the log severity string *level* into the *logging*'s internal logging severity value.
 
     :param level: the string log severity
@@ -36,17 +39,16 @@
 
 LOGGING_ID: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_ID", f"{APP_PREFIX}")
 LOGGING_FORMAT: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FORMAT",
                                          "{asctime} {levelname:1.1} {thread:5d} "
                                          "{module:20.20} {funcName:20.20} {lineno:3d} {message}")
 LOGGING_STYLE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_STYLE", "{")
 
-LOGGING_FILE_PATH: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_PATH",
-                                            os.path.join(tempfile.gettempdir(),
-                                                         f"{APP_PREFIX}.log"))
+LOGGING_FILE_PATH: Final[Path] = env_get_path(f"{APP_PREFIX}_LOGGING_FILE_PATH",
+                                              Path(tempfile.gettempdir()) / f"{APP_PREFIX}.log")
 LOGGING_FILE_MODE: Final[str] = env_get_str(f"{APP_PREFIX}_LOGGING_FILE_MODE", "a")
 
 # define and configure the logger
 PYPOMES_LOGGER: Final[logging.Logger] = logging.getLogger(LOGGING_ID)
 
 # define the logging severity level
 # noinspection PyTypeChecker
@@ -63,15 +65,15 @@
 for _handler in logging.root.handlers:
     _handler.addFilter(logging.Filter(LOGGING_ID))
 
 
 def logging_get_entries(errors: list[str],
                         log_level:  Literal["debug", "info", "warning", "error", "critical"] = None,
                         log_from: str = None, log_to: str = None,
-                        file_path: str = LOGGING_FILE_PATH) -> BytesIO:
+                        file_path: Path = LOGGING_FILE_PATH) -> BytesIO:
     """
     Extract and return all entries in *PYPOMES_LOGGER*'s logging file.
 
     The extraction meets the criteria specified by *log_level* and by the inclusive interval *[log_from, log_to]*.
 
     :param errors: errors eventually generated during execution
     :param log_level: the logging level (defaults to all levels)
@@ -99,23 +101,23 @@
     if log_to is not None:
         to_stamp = parser.parse(log_to)
         if to_stamp is None or \
            (from_stamp is not None and from_stamp > to_stamp):
             errors.append(f"Value '{to_stamp}' of 'to' attribute invalid")
 
     # does the log file exist ?
-    if not os.path.exists(file_path):
+    if not Path.exists(file_path):
         # no, report the error
         errors.append(f"File '{file_path}' not found")
 
     # any error ?
     if len(errors) == 0:
         # no, proceed
         result = BytesIO()
-        with open(file_path) as f:
+        with Path.open(file_path) as f:
             line: str = f.readline()
             while line:
                 items: list[str] = line.split(maxsplit=3)
                 # noinspection PyTypeChecker
                 msg_level: int = __get_logging_level(items[2])
                 if msg_level >= logging_level:
                     timestamp: datetime = parser.parse(f"{items[0]} {items[1]}")
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/str_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/str_pomes.py`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.2/src/pypomes_core/validation_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/validation_pomes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from datetime import date, datetime
 from typing import Final
+from .datetime_pomes import TIMEZONE_LOCAL
 from .env_pomes import APP_PREFIX, env_get_str
 
 VALIDATION_MSG_LANGUAGE: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_LANGUAGE", "pt")
 VALIDATION_MSG_PREFIX: Final[str] = env_get_str(f"{APP_PREFIX}_VALIDATION_MSG_PREFIX", APP_PREFIX)
 
 
 def validate_value(val: str | int | float, min_val: int = None,
@@ -167,15 +168,15 @@
 
     # retrieve the value
     result: float | None = scheme.get(suffix)
 
     # validate it
     if result is None:
         result = default
-    elif isinstance(result, str) or isinstance(result, int):
+    elif isinstance(result, str | int):
         try:
             result = float(result)
         except ValueError:
             result = None
             stat = __format_error(18, result, "int")
 
     if result is not None and not isinstance(result, float):
@@ -254,15 +255,15 @@
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         date_str: str = scheme[suffix]
         result = date_parse(date_str, dayfirst=day_first)
         if result is None:
             stat = __format_error(11, date_str)
-        elif result > datetime.now().date():
+        elif result > datetime.now(TIMEZONE_LOCAL).date():
             stat = __format_error(19, date_str)
     except KeyError:
         if isinstance(default, bool) and default:
             stat = __format_error(10)
         elif isinstance(default, date):
             result = default
 
@@ -295,15 +296,15 @@
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         date_str: str = scheme[suffix]
         result = datetime_parse(date_str, dayfirst=day_first)
         if result is None:
             stat = __format_error(21, date_str)
-        elif result > datetime.now():
+        elif result > datetime.now(TIMEZONE_LOCAL):
             stat = __format_error(18, date_str)
     except KeyError:
         if isinstance(default, bool) and default:
             stat = __format_error(10)
         elif isinstance(default, datetime):
             result = default
 
@@ -331,25 +332,25 @@
     result: list[any] | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         values: list[any] = scheme[suffix]
         if isinstance(values, list):
             result = []
-            if len(values) == 0:
-                raise KeyError
-            else:
+            if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, int):
                         stat: str = validate_value(value, min_val, max_val)
                     else:
                         stat: str = __format_error(18, value, "int")
                     if stat is not None:
                         errors.append(f"{stat} @{attr}[{inx+1}]")
+            elif mandatory:
+                errors.append(__format_error(10, f"@{attr}"))
         else:
             errors.append(__format_error(18, result, "list", f"@{attr}"))
     except (KeyError, TypeError):
         if mandatory:
             errors.append(__format_error(10, f"@{attr}"))
 
     return result
@@ -373,25 +374,25 @@
     result: list[any] | None = None
     pos: int = attr.rfind(".") + 1
     suffix: str = attr[pos:]
     try:
         values: list[any] = scheme[suffix]
         if isinstance(values, list):
             result = []
-            if len(values) == 0:
-                raise KeyError
-            else:
+            if len(values) > 0:
                 for inx, value in enumerate(values):
                     result.append(value)
                     if isinstance(value, str):
                         stat: str = validate_value(value, min_length, max_length)
                     else:
                         stat: str = __format_error(18, value, "str")
                     if stat is not None:
                         errors.append(f"{stat} @{attr}[{inx+1}]")
+            elif mandatory:
+                errors.append(__format_error(11, f"@{attr}"))
         else:
             errors.append(__format_error(18, result, "list", f"@{attr}"))
     except (KeyError, TypeError):
         if mandatory:
             errors.append(__format_error(11, f"@{attr}"))
 
     return result
```

### Comparing `pypomes_core-0.2.2/src/pypomes_core/xml_pomes.py` & `pypomes_core-0.2.3/src/pypomes_core/xml_pomes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from pathlib import Path
 from typing import Final
 from xmltodict3 import XmlTextToDict
 
 XML_FILE_HEADER: Final[str] = '<?xml version="1.0" encoding="UTF-8" ?>'
 
 
 def xml_normalize_keys(source: dict) -> dict:
@@ -60,19 +61,17 @@
     """
     # file_data é o próprio conteúdo XML ?
     if isinstance(file_data, bytes):
         # sim
         file_bytes: bytes = file_data
     else:  # elif isinstance(file_date, str):
         # não, obtenha-o do arquivo
-        with open(file_data, "rb") as f:
+        with Path.open(Path(file_data), "rb") as f:
             file_bytes: bytes = f.read()
 
     # converte o XML em dict
     xml_data = XmlTextToDict(xml_text=file_bytes.decode(),
                              ignore_namespace=True)
     result: dict = xml_data.get_dict()
 
     # normaliza o dict, removendo namespaces e prefixos "@" e "#" nos nomes das chaves
-    result = xml_normalize_keys(result)
-
-    return result
+    return xml_normalize_keys(result)
```

### Comparing `pypomes_core-0.2.2/LICENSE` & `pypomes_core-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pypomes_core-0.2.2/pyproject.toml` & `pypomes_core-0.2.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "hatchling"
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "pypomes_core"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="GT Nunes", email="wisecoder01@gmail.com" }
 ]
 description = "A collection of Python pomes, pennyeach (core modules)"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
@@ -18,14 +18,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent"
 ]
 dependencies = [
     "Flask>=2.3.2",
     "pip>=23.2.1",
     "python-dateutil>=2.8.2",
+    "pytz>=2023.3",
     "requests>=2.31.0",
     "setuptools>=68.0.0",
     "wheel>=0.41.0",
     "xmltodict3>=0.0.4"
 ]
 
 [project.urls]
```

### Comparing `pypomes_core-0.2.2/PKG-INFO` & `pypomes_core-0.2.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: pypomes_core
-Version: 0.2.2
+Version: 0.2.3
 Summary: A collection of Python pomes, pennyeach (core modules)
 Project-URL: Homepage, https://github.com/TheWiseCoder/PyPomes-Core
 Project-URL: Bug Tracker, https://github.com/TheWiseCoder/PyPomes-Core/issues
 Author-email: GT Nunes <wisecoder01@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: flask>=2.3.2
 Requires-Dist: pip>=23.2.1
 Requires-Dist: python-dateutil>=2.8.2
+Requires-Dist: pytz>=2023.3
 Requires-Dist: requests>=2.31.0
 Requires-Dist: setuptools>=68.0.0
 Requires-Dist: wheel>=0.41.0
 Requires-Dist: xmltodict3>=0.0.4
```

