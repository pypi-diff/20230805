# Comparing `tmp/ykenan_file-0.2.0.tar.gz` & `tmp/ykenan_file-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ykenan_file-0.2.0.tar", last modified: Sat Aug  5 03:12:10 2023, max compression
+gzip compressed data, was "ykenan_file-0.2.1.tar", last modified: Sat Aug  5 03:26:06 2023, max compression
```

## Comparing `ykenan_file-0.2.0.tar` & `ykenan_file-0.2.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 03:12:10.088964 ykenan_file-0.2.0/
--rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.2.0/LICENSE
--rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0      827 2023-08-05 03:12:10.087964 ykenan_file-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.2.0/README.md
--rw-rw-rw-   0        0        0      716 2023-08-05 03:10:51.000000 ykenan_file-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       65 2023-08-05 02:46:54.000000 ykenan_file-0.2.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 03:12:10.088964 ykenan_file-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 03:12:10.054964 ykenan_file-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 03:12:10.073963 ykenan_file-0.2.0/src/ykenan_file/
--rw-rw-rw-   0        0        0      274 2023-08-05 03:10:51.000000 ykenan_file-0.2.0/src/ykenan_file/__init__.py
--rw-rw-rw-   0        0        0    10534 2023-08-05 03:02:02.000000 ykenan_file-0.2.0/src/ykenan_file/_create_.py
--rw-rw-rw-   0        0        0     3593 2023-08-05 03:02:02.000000 ykenan_file-0.2.0/src/ykenan_file/_read_.py
--rw-rw-rw-   0        0        0    12602 2023-08-05 02:55:46.000000 ykenan_file-0.2.0/src/ykenan_file/_static_method_.py
--rw-rw-rw-   0        0        0     3953 2023-08-05 03:10:51.000000 ykenan_file-0.2.0/src/ykenan_file/_thread_file_.py
--rw-rw-rw-   0        0        0      293 2023-08-05 02:46:54.000000 ykenan_file-0.2.0/src/ykenan_file/_util_.py
-drwxrwxrwx   0        0        0        0 2023-08-05 03:12:10.086962 ykenan_file-0.2.0/src/ykenan_file.egg-info/
--rw-rw-rw-   0        0        0      827 2023-08-05 03:12:10.000000 ykenan_file-0.2.0/src/ykenan_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-08-05 03:12:10.000000 ykenan_file-0.2.0/src/ykenan_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 03:12:10.000000 ykenan_file-0.2.0/src/ykenan_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2023-08-05 03:12:10.000000 ykenan_file-0.2.0/src/ykenan_file.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-05 03:12:10.000000 ykenan_file-0.2.0/src/ykenan_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 03:26:06.937523 ykenan_file-0.2.1/
+-rw-rw-rw-   0        0        0     1067 2023-03-12 01:42:12.000000 ykenan_file-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       67 2023-03-17 07:56:10.000000 ykenan_file-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      827 2023-08-05 03:26:06.936523 ykenan_file-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-05-10 10:51:14.000000 ykenan_file-0.2.1/README.md
+-rw-rw-rw-   0        0        0      716 2023-08-05 03:25:32.000000 ykenan_file-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       65 2023-08-05 02:46:54.000000 ykenan_file-0.2.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 03:26:06.937523 ykenan_file-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 03:26:06.914523 ykenan_file-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 03:26:06.923522 ykenan_file-0.2.1/src/ykenan_file/
+-rw-rw-rw-   0        0        0      274 2023-08-05 03:10:51.000000 ykenan_file-0.2.1/src/ykenan_file/__init__.py
+-rw-rw-rw-   0        0        0    10534 2023-08-05 03:02:02.000000 ykenan_file-0.2.1/src/ykenan_file/_create_.py
+-rw-rw-rw-   0        0        0     3593 2023-08-05 03:02:02.000000 ykenan_file-0.2.1/src/ykenan_file/_read_.py
+-rw-rw-rw-   0        0        0    12602 2023-08-05 02:55:46.000000 ykenan_file-0.2.1/src/ykenan_file/_static_method_.py
+-rw-rw-rw-   0        0        0     3992 2023-08-05 03:23:50.000000 ykenan_file-0.2.1/src/ykenan_file/_thread_file_.py
+-rw-rw-rw-   0        0        0      293 2023-08-05 02:46:54.000000 ykenan_file-0.2.1/src/ykenan_file/_util_.py
+drwxrwxrwx   0        0        0        0 2023-08-05 03:26:06.935523 ykenan_file-0.2.1/src/ykenan_file.egg-info/
+-rw-rw-rw-   0        0        0      827 2023-08-05 03:26:06.000000 ykenan_file-0.2.1/src/ykenan_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-08-05 03:26:06.000000 ykenan_file-0.2.1/src/ykenan_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 03:26:06.000000 ykenan_file-0.2.1/src/ykenan_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2023-08-05 03:26:06.000000 ykenan_file-0.2.1/src/ykenan_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-05 03:26:06.000000 ykenan_file-0.2.1/src/ykenan_file.egg-info/top_level.txt
```

### Comparing `ykenan_file-0.2.0/LICENSE` & `ykenan_file-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.0/PKG-INFO` & `ykenan_file-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan_file
-Version: 0.2.0
+Version: 0.2.1
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `ykenan_file-0.2.0/pyproject.toml` & `ykenan_file-0.2.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=42", "ykenan-log>=0.2.0", "pandas>=1.5.3", "requests>=2.30.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "ykenan_file"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
     { name = "Yu Zhengmin", email = "3236170161@qq.com" },
 ]
 keywords = ["ykenan", "file", "read", "write"]
 description = "File read and write operations"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `ykenan_file-0.2.0/src/ykenan_file/_create_.py` & `ykenan_file-0.2.1/src/ykenan_file/_create_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.0/src/ykenan_file/_read_.py` & `ykenan_file-0.2.1/src/ykenan_file/_read_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.0/src/ykenan_file/_static_method_.py` & `ykenan_file-0.2.1/src/ykenan_file/_static_method_.py`

 * *Files identical despite different names*

### Comparing `ykenan_file-0.2.0/src/ykenan_file/_thread_file_.py` & `ykenan_file-0.2.1/src/ykenan_file/_thread_file_.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,26 +87,28 @@
         i: int = 0
         while True:
             if future.done():
                 self.results.append(future.result())
                 break
             else:
                 i += 1
-                await sleep(1)
+                sleep(1)
                 if i > self.wait_number:
                     break
 
     def run(self):
         for task in as_completed(self.tasks):
             task.add_done_callback(self.get_result)
 
     def get_files(self):
-        file_size: int = len(list(self.files))
+        file_size: int = 0
+        if self.files is not None:
+            file_size: int = len(list(self.files))
 
-        if self.base_path is None or self.files is None or file_size == 0:
+        if self.base_path is None and file_size == 0:
             self.log.error("At least one of the `base_path` and `files` parameters has a parameter")
             raise ValueError("At least one of the `base_path` and `files` parameters has a parameter")
 
         new_files = []
         if isinstance(self.base_path, path):
             new_files = self.static_method.get_files_path(self.base_path)
         return new_files
```

### Comparing `ykenan_file-0.2.0/src/ykenan_file.egg-info/PKG-INFO` & `ykenan_file-0.2.1/src/ykenan_file.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ykenan-file
-Version: 0.2.0
+Version: 0.2.1
 Summary: File read and write operations
 Author-email: Yu Zhengmin <3236170161@qq.com>
 Project-URL: github, https://github.com/YuZhengM/ykenan_file
 Keywords: ykenan,file,read,write
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

