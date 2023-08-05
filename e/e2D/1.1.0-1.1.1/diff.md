# Comparing `tmp/e2D-1.1.0.tar.gz` & `tmp/e2D-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "e2D-1.1.0.tar", last modified: Fri Aug  4 23:05:03 2023, max compression
+gzip compressed data, was "e2D-1.1.1.tar", last modified: Sat Aug  5 00:14:26 2023, max compression
```

## Comparing `e2D-1.1.0.tar` & `e2D-1.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 23:05:03.032089 e2D-1.1.0/
--rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     9505 2023-08-04 23:05:03.033086 e2D-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     8910 2023-08-04 22:06:56.000000 e2D-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 23:05:03.011880 e2D-1.1.0/e2D/
--rw-rw-rw-   0        0        0    59067 2023-08-04 22:09:11.000000 e2D-1.1.0/e2D/__init__.py
--rw-rw-rw-   0        0        0    10261 2023-08-04 22:54:26.000000 e2D-1.1.0/e2D/envs.py
--rw-rw-rw-   0        0        0     5306 2023-08-04 22:26:19.000000 e2D-1.1.0/e2D/utils.py
-drwxrwxrwx   0        0        0        0 2023-08-04 23:05:03.031094 e2D-1.1.0/e2D.egg-info/
--rw-rw-rw-   0        0        0     9505 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-08-04 23:05:02.000000 e2D-1.1.0/e2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-08-04 23:05:03.034083 e2D-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 00:14:26.422592 e2D-1.1.1/
+-rw-rw-rw-   0        0        0     1087 2023-07-31 14:47:36.000000 e2D-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     9505 2023-08-05 00:14:26.422592 e2D-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     8910 2023-08-04 22:06:56.000000 e2D-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 00:14:26.406973 e2D-1.1.1/e2D/
+-rw-rw-rw-   0        0        0    58532 2023-08-05 00:07:54.000000 e2D-1.1.1/e2D/__init__.py
+-rw-rw-rw-   0        0        0    10261 2023-08-04 22:54:26.000000 e2D-1.1.1/e2D/envs.py
+-rw-rw-rw-   0        0        0     5306 2023-08-04 22:26:19.000000 e2D-1.1.1/e2D/utils.py
+drwxrwxrwx   0        0        0        0 2023-08-05 00:14:26.422592 e2D-1.1.1/e2D.egg-info/
+-rw-rw-rw-   0        0        0     9505 2023-08-05 00:14:26.000000 e2D-1.1.1/e2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-08-05 00:14:26.000000 e2D-1.1.1/e2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 00:14:26.000000 e2D-1.1.1/e2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-08-05 00:14:26.000000 e2D-1.1.1/e2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-08-05 00:14:26.000000 e2D-1.1.1/e2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      106 2023-07-31 15:05:25.000000 e2D-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-08-05 00:14:26.422592 e2D-1.1.1/setup.cfg
```

### Comparing `e2D-1.1.0/LICENSE` & `e2D-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `e2D-1.1.0/PKG-INFO` & `e2D-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-1.1.0/README.md` & `e2D-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `e2D-1.1.0/e2D/__init__.py` & `e2D-1.1.1/e2D/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -718,26 +718,14 @@
         else:
             center = self.__normalize__(center)
         translated = self - center
         cos_angle = _mt.cos(angle)
         sin_angle = _mt.sin(angle)
         return Vector2D(translated.x * cos_angle - translated.y * sin_angle, translated.x * sin_angle + translated.y * cos_angle) + center
 
-    def __eq__(self, other:"float|int|Vector2D|V2|list|tuple") -> bool:
-        other = self.__normalize__(other)
-        return self.x == other.x and self.y == other.y
-
-    def __ne__(self, other:"float|int|Vector2D|V2|list|tuple") -> bool:
-        return not self.__eq__(other)
-
-#######################################################################################################################################
-#######################################################################################################################################
-#######################################################################################################################################
-#######################################################################################################################################
-
     def no_zero_div_error(self:"Vector2D|V2", n:"int|float|Vector2D|V2", error_mode:str="zero") -> "Vector2D|V2":
         """
         # Handle division between the Vector2D other and a numeric value or another Vector2D other.
 
         ## Parameters:
             n (int|float or Vector2D): The numeric value or Vector2D other for division.
             error_mode (str, optional): The mode to handle division by zero scenarios.
@@ -839,14 +827,23 @@
     
     def __itruediv__(self:"V2|Vector2D", other:"float|int|Vector2D|V2|list|tuple") -> "Vector2D":
         other = self.__normalize__(other)
         self.x /= other.x
         self.y /= other.y
         return self
 
+    def __eq__(self, other) -> bool:
+        if not isinstance(other, Vector2D|V2|list|tuple):
+            return False
+        other = self.__normalize__(other)
+        return self.x == other.x and self.y == other.y
+
+    def __ne__(self, other) -> bool:
+        return not self.__eq__(other)
+
     def __abs__(self:"V2|Vector2D") -> "Vector2D|V2":
         return Vector2D(abs(self.x), abs(self.y))
 
     def __round__(self:"V2|Vector2D", n:int|float=1) -> "Vector2D|V2":
         return Vector2D(round(self.x / n) * n, round(self.y / n) * n)
 
     def __floor__(self:"V2|Vector2D", n:int|float=1) -> "Vector2D|V2":
```

### Comparing `e2D-1.1.0/e2D/envs.py` & `e2D-1.1.1/e2D/envs.py`

 * *Files identical despite different names*

### Comparing `e2D-1.1.0/e2D/utils.py` & `e2D-1.1.1/e2D/utils.py`

 * *Files identical despite different names*

### Comparing `e2D-1.1.0/e2D.egg-info/PKG-INFO` & `e2D-1.1.1/e2D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: e2D
-Version: 1.1.0
+Version: 1.1.1
 Summary: Python library for 2D games. Streamlines dev with keyboard/mouse input, vector calculations, color manipulation, and collision detection. Simplify game creation and unleash creativity!
 Home-page: https://github.com/marick-py/e2D
 Author: Riccardo Mariani
 Author-email: ricomari2006@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `e2D-1.1.0/setup.cfg` & `e2D-1.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2065 3244 0d0a 7665 7273 696f 6e20   = e2D..version 
-00000020: 3d20 312e 312e 300d 0a61 7574 686f 7220  = 1.1.0..author 
+00000020: 3d20 312e 312e 310d 0a61 7574 686f 7220  = 1.1.1..author 
 00000030: 3d20 5269 6363 6172 646f 204d 6172 6961  = Riccardo Maria
 00000040: 6e69 0d0a 6175 7468 6f72 5f65 6d61 696c  ni..author_email
 00000050: 203d 2072 6963 6f6d 6172 6932 3030 3640   = ricomari2006@
 00000060: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
 00000070: 6970 7469 6f6e 203d 2050 7974 686f 6e20  iption = Python 
 00000080: 6c69 6272 6172 7920 666f 7220 3244 2067  library for 2D g
 00000090: 616d 6573 2e20 5374 7265 616d 6c69 6e65  ames. Streamline
```

