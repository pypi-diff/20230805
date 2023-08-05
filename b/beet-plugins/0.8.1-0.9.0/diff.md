# Comparing `tmp/beet_plugins-0.8.1.tar.gz` & `tmp/beet_plugins-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beet_plugins-0.8.1.tar", max compression
+gzip compressed data, was "beet_plugins-0.9.0.tar", max compression
```

## Comparing `beet_plugins-0.8.1.tar` & `beet_plugins-0.9.0.tar`

### file list

```diff
@@ -1,20 +1,22 @@
--rw-r--r--   0        0        0     1063 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/LICENSE
--rw-r--r--   0        0        0       21 2023-08-04 02:25:52.052177 beet_plugins-0.8.1/beet_plugins/__init__.py
--rw-r--r--   0        0        0     9845 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/latest_snapshot.py
--rw-r--r--   0        0        0     3119 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/nbt_literals.py
--rw-r--r--   0        0        0     4270 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/resources/latest_snapshot.json
--rw-r--r--   0        0        0     3747 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/root_location.py
--rw-r--r--   0        0        0     1921 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/scoreboard.py
--rw-r--r--   0        0        0      548 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/chunk.bolt
--rw-r--r--   0        0        0      524 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/data.bolt
--rw-r--r--   0        0        0     2434 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/dynamic_pos.bolt
--rw-r--r--   0        0        0      576 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/entity.bolt
--rw-r--r--   0        0        0      312 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/functions.bolt
--rw-r--r--   0        0        0      690 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/lantern.bolt
--rw-r--r--   0        0        0     1059 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/math.bolt
--rw-r--r--   0        0        0      399 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/objectives.bolt
--rw-r--r--   0        0        0      917 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/path.bolt
--rw-r--r--   0        0        0      339 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils/tags.bolt
--rw-r--r--   0        0        0      242 2023-08-04 02:25:11.347715 beet_plugins-0.8.1/beet_plugins/utils.py
--rw-r--r--   0        0        0      660 2023-08-04 02:25:52.060177 beet_plugins-0.8.1/pyproject.toml
--rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 beet_plugins-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/LICENSE
+-rw-r--r--   0        0        0       21 2023-08-05 19:52:21.125951 beet_plugins-0.9.0/beet_plugins/__init__.py
+-rw-r--r--   0        0        0     9845 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/latest_snapshot.py
+-rw-r--r--   0        0        0     3119 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/nbt_literals.py
+-rw-r--r--   0        0        0     4270 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/resources/latest_snapshot.json
+-rw-r--r--   0        0        0     3747 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/root_location.py
+-rw-r--r--   0        0        0     1921 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/scoreboard.py
+-rw-r--r--   0        0        0      548 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/chunk.bolt
+-rw-r--r--   0        0        0      554 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/data.bolt
+-rw-r--r--   0        0        0     1877 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/db.bolt
+-rw-r--r--   0        0        0     2434 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/dynamic_pos.bolt
+-rw-r--r--   0        0        0      576 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/entity.bolt
+-rw-r--r--   0        0        0      312 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/functions.bolt
+-rw-r--r--   0        0        0      690 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/lantern.bolt
+-rw-r--r--   0        0        0     1058 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/math.bolt
+-rw-r--r--   0        0        0      416 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/objectives.bolt
+-rw-r--r--   0        0        0      927 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/path.bolt
+-rw-r--r--   0        0        0      339 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/tags.bolt
+-rw-r--r--   0        0        0     2233 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils/uuid.bolt
+-rw-r--r--   0        0        0      242 2023-08-05 19:51:42.181644 beet_plugins-0.9.0/beet_plugins/utils.py
+-rw-r--r--   0        0        0      660 2023-08-05 19:52:21.129951 beet_plugins-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0      461 1970-01-01 00:00:00.000000 beet_plugins-0.9.0/PKG-INFO
```

### Comparing `beet_plugins-0.8.1/LICENSE` & `beet_plugins-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/latest_snapshot.py` & `beet_plugins-0.9.0/beet_plugins/latest_snapshot.py`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/nbt_literals.py` & `beet_plugins-0.9.0/beet_plugins/nbt_literals.py`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/resources/latest_snapshot.json` & `beet_plugins-0.9.0/beet_plugins/resources/latest_snapshot.json`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/root_location.py` & `beet_plugins-0.9.0/beet_plugins/root_location.py`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/scoreboard.py` & `beet_plugins-0.9.0/beet_plugins/scoreboard.py`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/utils/chunk.bolt` & `beet_plugins-0.9.0/beet_plugins/utils/chunk.bolt`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/utils/dynamic_pos.bolt` & `beet_plugins-0.9.0/beet_plugins/utils/dynamic_pos.bolt`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/utils/entity.bolt` & `beet_plugins-0.9.0/beet_plugins/utils/entity.bolt`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/utils/lantern.bolt` & `beet_plugins-0.9.0/beet_plugins/utils/lantern.bolt`

 * *Files identical despite different names*

### Comparing `beet_plugins-0.8.1/beet_plugins/utils/math.bolt` & `beet_plugins-0.9.0/beet_plugins/utils/math.bolt`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from bolt_expressions import Expression, Scoreboard
 from ./path import root
+from ./objectives import temp_obj
 
-temp = Scoreboard(Expression.opts.temp_objective, prefixed_obj=False)
-
-input = temp["$input"]
-output = temp["$output"]
-scale_factor = temp["$scale_factor"]
+input = temp_obj["$input"]
+output = temp_obj["$output"]
+scale_factor = temp_obj["$scale_factor"]
 
 #
  #/ INPUT - The value to be taken the square root.
  #/         Can be a LITERAL, a SCORE or an EXPRESSION.
  #/ SCALE - The amount of DIGITS after the
  #/         DECIMAL POINT of the OUTPUT SCORE
- #/ RETURN score #output temp
+ #/ RETURN score #output temp_obj
  #/
  #/ Examples
  #/ obj["@s"] = sqrt(64)  # @s is 8
  #/ obj["@s"] = sqrt(64, scale=1) # @s is 80 (8.0)
  #/ obj["@s"] = sqrt( obj["@s"] * 3, scale=2 ) # @s is 1549 (15.49)
 def sqrt(value, scale=1):
-    temp["$input"] = value * scale
+    temp_obj["$input"] = value * scale
     execute function root("math/sqrt/solve"):
-        test = temp["$test"]
+        test = temp_obj["$test"]
         output = 0
         increment = 32768 # not a score
         for i in range(16):
             test = output + increment
             test *= test
-            if score $test temp <= $input temp:
+            if score $test temp_obj <= $input temp_obj:
                 output += increment
             increment //= 2
-    return temp["$output"]
+    return temp_obj["$output"]
```

### Comparing `beet_plugins-0.8.1/beet_plugins/utils/path.bolt` & `beet_plugins-0.9.0/beet_plugins/utils/path.bolt`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 from bolt import Runtime
 
 runtime = ctx.inject(Runtime)
 project_root = generate_path('')
 
 def current():
-    return runtime.get_path()
+    return runtime.modules.current_path
 
 def root(args):
     if not isinstance(args, (list, tuple)):
         args = [ args ]
     args = map(str, args)
     if project_root.endswith(":"):
         return project_root + '/'.join(args)
```

### Comparing `beet_plugins-0.8.1/pyproject.toml` & `beet_plugins-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "beet-plugins"
-version = "0.8.1"
+version = "0.9.0"
 description = ""
 authors = ["TheWii <67249660+TheWii@users.noreply.github.com>"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 bolt = ">=0.37.0"
 bolt-expressions = ">=0.12.2"
```

