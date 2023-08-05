# Comparing `tmp/tamodify-0.0.6.tar.gz` & `tmp/tamodify-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tamodify-0.0.6.tar", last modified: Tue Nov 15 08:39:37 2022, max compression
+gzip compressed data, was "tamodify-0.1.0.tar", last modified: Sat Aug  5 07:55:08 2023, max compression
```

## Comparing `tamodify-0.0.6.tar` & `tamodify-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 08:39:37.000000 tamodify-0.0.6/
--rwxrw-rw-   0 root         (0) root         (0)     1074 2022-03-26 03:22:28.000000 tamodify-0.0.6/LICENSE
--rwxrw-rw-   0 root         (0) root         (0)       52 2022-11-15 08:36:40.000000 tamodify-0.0.6/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      558 2022-11-15 08:39:37.000000 tamodify-0.0.6/PKG-INFO
--rwxrw-rw-   0 root         (0) root         (0)      127 2022-06-15 02:50:53.000000 tamodify-0.0.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2022-11-15 08:39:37.000000 tamodify-0.0.6/setup.cfg
--rwxrw-rw-   0 root         (0) root         (0)     1062 2022-11-15 08:39:09.000000 tamodify-0.0.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 08:39:37.000000 tamodify-0.0.6/src/
--rw-r--r--   0 root         (0) root         (0)    92145 2021-05-12 23:10:20.000000 tamodify-0.0.6/src/tajk_data.c
--rwxr--r--   0 root         (0) root         (0)      768 2021-05-10 02:54:57.000000 tamodify-0.0.6/src/tajk_data.h
--rwxrw-rw-   0 root         (0) root         (0)     8472 2022-06-19 09:56:50.000000 tamodify-0.0.6/src/tajk_modify.c
--rw-r--r--   0 root         (0) root         (0)     3756 2022-06-19 09:55:36.000000 tamodify-0.0.6/src/tajk_modify.h
--rwxrw-rw-   0 root         (0) root         (0)     3598 2022-07-06 05:23:18.000000 tamodify-0.0.6/src/tamodify.c
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-11-15 08:39:37.000000 tamodify-0.0.6/tamodify.egg-info/
--rw-r--r--   0 root         (0) root         (0)      558 2022-11-15 08:39:37.000000 tamodify-0.0.6/tamodify.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      280 2022-11-15 08:39:37.000000 tamodify-0.0.6/tamodify.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 08:39:37.000000 tamodify-0.0.6/tamodify.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 08:39:37.000000 tamodify-0.0.6/tamodify.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)        9 2022-11-15 08:39:37.000000 tamodify-0.0.6/tamodify.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:55:08.000000 tamodify-0.1.0/
+-rwxrw-rw-   0 root         (0) root         (0)     1074 2022-03-26 03:22:28.000000 tamodify-0.1.0/LICENSE
+-rwxrw-rw-   0 root         (0) root         (0)       52 2022-11-15 08:36:40.000000 tamodify-0.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-05 07:55:08.000000 tamodify-0.1.0/PKG-INFO
+-rwxrw-rw-   0 root         (0) root         (0)      127 2022-06-15 02:50:53.000000 tamodify-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 07:55:08.000000 tamodify-0.1.0/setup.cfg
+-rwxrw-rw-   0 root         (0) root         (0)     2176 2023-08-05 07:55:05.000000 tamodify-0.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:55:08.000000 tamodify-0.1.0/src/
+-rw-r--r--   0 root         (0) root         (0)    92145 2021-05-12 23:10:20.000000 tamodify-0.1.0/src/tajk_data.c
+-rwxr-xr-x   0 root         (0) root         (0)      905 2022-09-05 06:29:10.000000 tamodify-0.1.0/src/tajk_data.h
+-rwxrw-rw-   0 root         (0) root         (0)     8474 2023-08-05 07:27:20.000000 tamodify-0.1.0/src/tajk_modify.c
+-rw-r--r--   0 root         (0) root         (0)     3756 2022-06-19 09:55:36.000000 tamodify-0.1.0/src/tajk_modify.h
+-rwxrw-rw-   0 root         (0) root         (0)     3598 2022-07-06 05:23:18.000000 tamodify-0.1.0/src/tamodify.c
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:55:08.000000 tamodify-0.1.0/tamodify.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      558 2023-08-05 07:55:08.000000 tamodify-0.1.0/tamodify.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      280 2023-08-05 07:55:08.000000 tamodify-0.1.0/tamodify.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 07:55:08.000000 tamodify-0.1.0/tamodify.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-11-15 08:39:37.000000 tamodify-0.1.0/tamodify.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)        9 2023-08-05 07:55:08.000000 tamodify-0.1.0/tamodify.egg-info/top_level.txt
```

### Comparing `tamodify-0.0.6/LICENSE` & `tamodify-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tamodify-0.0.6/PKG-INFO` & `tamodify-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamodify
-Version: 0.0.6
+Version: 0.1.0
 Summary: TA接口文件修改
 Home-page: https://gitee.com/chenc224/ofbdep/tree/master/python
 Author: Chen chuan
 Author-email: 13902950907@139.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `tamodify-0.0.6/src/tajk_data.c` & `tamodify-0.1.0/src/tajk_data.c`

 * *Files identical despite different names*

### Comparing `tamodify-0.0.6/src/tajk_modify.c` & `tamodify-0.1.0/src/tajk_modify.c`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     return 0;
 }
 
 static int readhead(char *t,int cd)   {//´Ó»º³åÇø¶ÁÈë×Ö·û´®£¬Çå¿ÕÄ©Î²µÄ¿Õ¸ñ
     strcpy(t,"");
     if(readline())return 1;
     strncpy(t,tam->linedata,cd);
-    t[cd]=0;
+    t[cd-1]=0;
     srtrim(t);
     return tamodify_write();
 }
 
 static void default_perrinfo(int retcode,const wchar_t *errinfo){//ÓÃ»§¿É×Ô¶¨ÒåÒ»¸öÊä³ö´íÎóÐÅÏ¢µÄº¯Êý£¬²»¶¨ÒåÔòÊ¹ÓÃÕâ¸ö¿Õº¯Êý
 }
```

### Comparing `tamodify-0.0.6/src/tajk_modify.h` & `tamodify-0.1.0/src/tajk_modify.h`

 * *Files identical despite different names*

### Comparing `tamodify-0.0.6/src/tamodify.c` & `tamodify-0.1.0/src/tamodify.c`

 * *Files identical despite different names*

### Comparing `tamodify-0.0.6/tamodify.egg-info/PKG-INFO` & `tamodify-0.1.0/tamodify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tamodify
-Version: 0.0.6
+Version: 0.1.0
 Summary: TA接口文件修改
 Home-page: https://gitee.com/chenc224/ofbdep/tree/master/python
 Author: Chen chuan
 Author-email: 13902950907@139.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

