# Comparing `tmp/vika-1.3.0.tar.gz` & `tmp/vika-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/vika-1.3.0.tar", last modified: Tue Jul 11 07:06:35 2023, max compression
+gzip compressed data, was "vika-1.3.1.tar", last modified: Sat Aug  5 07:56:57 2023, max compression
```

## Comparing `vika-1.3.0.tar` & `vika-1.3.1.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)    14924 2023-07-11 07:06:27.000000 vika-1.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-07-11 07:06:35.000000 vika-1.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      827 2023-07-11 07:06:27.000000 vika-1.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/space/
--rw-r--r--   0 runner    (1001) docker     (122)      937 2023-07-11 07:06:27.000000 vika-1.3.0/vika/space/space_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-07-11 07:06:27.000000 vika-1.3.0/vika/space/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2150 2023-07-11 07:06:27.000000 vika-1.3.0/vika/space/space.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/datasheet/
--rw-r--r--   0 runner    (1001) docker     (122)      889 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/datasheet_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)    10632 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/datasheet.py
--rw-r--r--   0 runner    (1001) docker     (122)      167 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4139 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/query_set.py
--rw-r--r--   0 runner    (1001) docker     (122)     8957 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/record_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4618 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/field_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     3184 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/record.py
--rw-r--r--   0 runner    (1001) docker     (122)      323 2023-07-11 07:06:27.000000 vika-1.3.0/vika/datasheet/view_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)     4165 2023-07-11 07:06:27.000000 vika-1.3.0/vika/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-11 07:06:27.000000 vika-1.3.0/vika/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/node/
--rw-r--r--   0 runner    (1001) docker     (122)       28 2023-07-11 07:06:27.000000 vika-1.3.0/vika/node/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1880 2023-07-11 07:06:27.000000 vika-1.3.0/vika/node/node_manager.py
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-07-11 07:06:27.000000 vika-1.3.0/vika/const.py
--rw-r--r--   0 runner    (1001) docker     (122)       47 2023-07-11 07:06:27.000000 vika-1.3.0/vika/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/types/
--rw-r--r--   0 runner    (1001) docker     (122)      544 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/node.py
--rw-r--r--   0 runner    (1001) docker     (122)     1151 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/embedlink.py
--rw-r--r--   0 runner    (1001) docker     (122)     3282 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/response.py
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1817 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/unit_model.py
--rw-r--r--   0 runner    (1001) docker     (122)      347 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/view.py
--rw-r--r--   0 runner    (1001) docker     (122)     5147 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/field.py
--rw-r--r--   0 runner    (1001) docker     (122)      608 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/record.py
--rw-r--r--   0 runner    (1001) docker     (122)      148 2023-07-11 07:06:27.000000 vika-1.3.0/vika/types/space.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-07-11 07:06:27.000000 vika-1.3.0/vika/request.py
--rw-r--r--   0 runner    (1001) docker     (122)     1924 2023-07-11 07:06:27.000000 vika-1.3.0/vika/apitable.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika/unit/
--rw-r--r--   0 runner    (1001) docker     (122)     3390 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/team.py
--rw-r--r--   0 runner    (1001) docker     (122)      107 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1495 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/member.py
--rw-r--r--   0 runner    (1001) docker     (122)     1694 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/unit.py
--rw-r--r--   0 runner    (1001) docker     (122)     2729 2023-07-11 07:06:27.000000 vika-1.3.0/vika/unit/role.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/test/
--rw-r--r--   0 runner    (1001) docker     (122)      958 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (122)      917 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_datasheet.py
--rw-r--r--   0 runner    (1001) docker     (122)     1099 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_delete_field.py
--rw-r--r--   0 runner    (1001) docker     (122)     1465 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      967 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      971 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_delete_records.py
--rw-r--r--   0 runner    (1001) docker     (122)     2624 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_update_records.py
--rw-r--r--   0 runner    (1001) docker     (122)      607 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_spaces.py
--rw-r--r--   0 runner    (1001) docker     (122)      970 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_fields.py
--rw-r--r--   0 runner    (1001) docker     (122)      658 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_get_views.py
--rw-r--r--   0 runner    (1001) docker     (122)     1284 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_field.py
--rw-r--r--   0 runner    (1001) docker     (122)      919 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_upload_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-07-11 07:06:27.000000 vika-1.3.0/test/test_create_embed_link.py
--rw-r--r--   0 runner    (1001) docker     (122)    17993 2023-07-11 07:06:35.000000 vika-1.3.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)        5 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)    17993 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1263 2023-07-11 07:06:35.000000 vika-1.3.0/vika.egg-info/SOURCES.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.986277 vika-1.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1066 2023-08-05 07:56:30.000000 vika-1.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    15335 2023-08-05 07:56:57.986277 vika-1.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14924 2023-08-05 07:56:30.000000 vika-1.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-08-05 07:56:57.986277 vika-1.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      847 2023-08-05 07:56:30.000000 vika-1.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.978277 vika-1.3.1/test/
+-rw-r--r--   0 root         (0) root         (0)      384 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_apitable.py
+-rw-r--r--   0 root         (0) root         (0)      917 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_create_datasheet.py
+-rw-r--r--   0 root         (0) root         (0)     2016 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_create_embed_link.py
+-rw-r--r--   0 root         (0) root         (0)     1284 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_create_field.py
+-rw-r--r--   0 root         (0) root         (0)      958 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_create_records.py
+-rw-r--r--   0 root         (0) root         (0)     1099 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_delete_field.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_delete_records.py
+-rw-r--r--   0 root         (0) root         (0)      970 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_get_fields.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_get_nodes.py
+-rw-r--r--   0 root         (0) root         (0)     1465 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_get_records.py
+-rw-r--r--   0 root         (0) root         (0)      607 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_get_spaces.py
+-rw-r--r--   0 root         (0) root         (0)      658 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_get_views.py
+-rw-r--r--   0 root         (0) root         (0)     3876 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_unit.py
+-rw-r--r--   0 root         (0) root         (0)     2624 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_update_records.py
+-rw-r--r--   0 root         (0) root         (0)      919 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_upload_file.py
+-rw-r--r--   0 root         (0) root         (0)      967 2023-08-05 07:56:30.000000 vika-1.3.1/test/test_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.978277 vika-1.3.1/vika/
+-rw-r--r--   0 root         (0) root         (0)       47 2023-08-05 07:56:30.000000 vika-1.3.1/vika/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-08-05 07:56:30.000000 vika-1.3.1/vika/apitable.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-08-05 07:56:30.000000 vika-1.3.1/vika/const.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.982277 vika-1.3.1/vika/datasheet/
+-rw-r--r--   0 root         (0) root         (0)      167 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10632 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/datasheet.py
+-rw-r--r--   0 root         (0) root         (0)      889 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/datasheet_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4618 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/field_manager.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/query_set.py
+-rw-r--r--   0 root         (0) root         (0)     3184 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/record.py
+-rw-r--r--   0 root         (0) root         (0)     8957 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/record_manager.py
+-rw-r--r--   0 root         (0) root         (0)      323 2023-08-05 07:56:30.000000 vika-1.3.1/vika/datasheet/view_manager.py
+-rw-r--r--   0 root         (0) root         (0)      971 2023-08-05 07:56:30.000000 vika-1.3.1/vika/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.982277 vika-1.3.1/vika/node/
+-rw-r--r--   0 root         (0) root         (0)       28 2023-08-05 07:56:30.000000 vika-1.3.1/vika/node/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1880 2023-08-05 07:56:30.000000 vika-1.3.1/vika/node/node_manager.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-08-05 07:56:30.000000 vika-1.3.1/vika/request.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.982277 vika-1.3.1/vika/space/
+-rw-r--r--   0 root         (0) root         (0)       50 2023-08-05 07:56:30.000000 vika-1.3.1/vika/space/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2150 2023-08-05 07:56:30.000000 vika-1.3.1/vika/space/space.py
+-rw-r--r--   0 root         (0) root         (0)      937 2023-08-05 07:56:30.000000 vika-1.3.1/vika/space/space_manager.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.982277 vika-1.3.1/vika/types/
+-rw-r--r--   0 root         (0) root         (0)      179 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/embedlink.py
+-rw-r--r--   0 root         (0) root         (0)     5147 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/field.py
+-rw-r--r--   0 root         (0) root         (0)      544 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/node.py
+-rw-r--r--   0 root         (0) root         (0)      608 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/record.py
+-rw-r--r--   0 root         (0) root         (0)     3282 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/response.py
+-rw-r--r--   0 root         (0) root         (0)      148 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/space.py
+-rw-r--r--   0 root         (0) root         (0)     1817 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/unit_model.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-08-05 07:56:30.000000 vika-1.3.1/vika/types/view.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.986277 vika-1.3.1/vika/unit/
+-rw-r--r--   0 root         (0) root         (0)      107 2023-08-05 07:56:30.000000 vika-1.3.1/vika/unit/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2023-08-05 07:56:30.000000 vika-1.3.1/vika/unit/member.py
+-rw-r--r--   0 root         (0) root         (0)     2729 2023-08-05 07:56:30.000000 vika-1.3.1/vika/unit/role.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-08-05 07:56:30.000000 vika-1.3.1/vika/unit/team.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-08-05 07:56:30.000000 vika-1.3.1/vika/unit/unit.py
+-rw-r--r--   0 root         (0) root         (0)     4165 2023-08-05 07:56:30.000000 vika-1.3.1/vika/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-08-05 07:56:57.978277 vika-1.3.1/vika.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    15335 2023-08-05 07:56:57.000000 vika-1.3.1/vika.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1311 2023-08-05 07:56:57.000000 vika-1.3.1/vika.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-08-05 07:56:57.000000 vika-1.3.1/vika.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-08-05 07:56:57.000000 vika-1.3.1/vika.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-08-05 07:56:57.000000 vika-1.3.1/vika.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `vika-1.3.0/README.md` & `vika-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/setup.py` & `vika-1.3.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,9 +20,9 @@
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.6",
-    install_requires=["requests", "pydantic", "environs"],
+    install_requires=["requests<=2.31.0", "pydantic==1.7", "environs<=9.5.0"],
 )
```

### Comparing `vika-1.3.0/vika/space/space_manager.py` & `vika-1.3.1/vika/space/space_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/space/space.py` & `vika-1.3.1/vika/space/space.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/datasheet/datasheet_manager.py` & `vika-1.3.1/vika/datasheet/datasheet_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/datasheet/datasheet.py` & `vika-1.3.1/vika/datasheet/datasheet.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/datasheet/query_set.py` & `vika-1.3.1/vika/datasheet/query_set.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/datasheet/record_manager.py` & `vika-1.3.1/vika/datasheet/record_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/datasheet/field_manager.py` & `vika-1.3.1/vika/datasheet/field_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/datasheet/record.py` & `vika-1.3.1/vika/datasheet/record.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/utils.py` & `vika-1.3.1/vika/utils.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/exceptions.py` & `vika-1.3.1/vika/exceptions.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/node/node_manager.py` & `vika-1.3.1/vika/node/node_manager.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/types/node.py` & `vika-1.3.1/vika/types/node.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/types/embedlink.py` & `vika-1.3.1/vika/types/embedlink.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/types/response.py` & `vika-1.3.1/vika/types/response.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/types/unit_model.py` & `vika-1.3.1/vika/types/unit_model.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/types/field.py` & `vika-1.3.1/vika/types/field.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/types/record.py` & `vika-1.3.1/vika/types/record.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/request.py` & `vika-1.3.1/vika/request.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/apitable.py` & `vika-1.3.1/vika/apitable.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/unit/team.py` & `vika-1.3.1/vika/unit/team.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/unit/member.py` & `vika-1.3.1/vika/unit/member.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika/unit/unit.py` & `vika-1.3.1/vika/unit/unit.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,28 +12,26 @@
     def __init__(self, space: 'Space'):
         self._space = space
 
     def _describe_member_endpoint(self, unit_id: str):
         return urljoin(self._space.apitable.api_base,
                        f"/fusion/v1/spaces/{self._space.id}/members/{unit_id}")
 
-    @property
     def _role_endpoint(self):
         return urljoin(self._space.apitable.api_base,
                        f"/fusion/v1/spaces/{self._space.id}/roles")
 
     def _describe_role_endpoint(self, unit_id: str):
         return urljoin(self._space.apitable.api_base,
                        f"/fusion/v1/spaces/{self._space.id}/roles/{unit_id}")
 
     def _list_role_unit_endpoint(self, unit_id: str):
         return urljoin(self._space.apitable.api_base,
                        f"/fusion/v1/spaces/{self._space.id}/roles/{unit_id}/units")
 
-    @property
     def _team_endpoint(self):
         return urljoin(self._space.apitable.api_base,
                        f"/fusion/v1/spaces/{self._space.id}/teams")
 
     def _describe_team_endpoint(self, unit_id: str):
         return urljoin(self._space.apitable.api_base,
                        f"/fusion/v1/spaces/{self._space.id}/teams/{unit_id}")
```

### Comparing `vika-1.3.0/vika/unit/role.py` & `vika-1.3.1/vika/unit/role.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_create_records.py` & `vika-1.3.1/test/test_create_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_get_nodes.py` & `vika-1.3.1/test/test_get_nodes.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_create_datasheet.py` & `vika-1.3.1/test/test_create_datasheet.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_delete_field.py` & `vika-1.3.1/test/test_delete_field.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_get_records.py` & `vika-1.3.1/test/test_get_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_utils.py` & `vika-1.3.1/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_delete_records.py` & `vika-1.3.1/test/test_delete_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_update_records.py` & `vika-1.3.1/test/test_update_records.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_get_spaces.py` & `vika-1.3.1/test/test_get_spaces.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_get_fields.py` & `vika-1.3.1/test/test_get_fields.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_get_views.py` & `vika-1.3.1/test/test_get_views.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_create_field.py` & `vika-1.3.1/test/test_create_field.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_upload_file.py` & `vika-1.3.1/test/test_upload_file.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/test/test_create_embed_link.py` & `vika-1.3.1/test/test_create_embed_link.py`

 * *Files identical despite different names*

### Comparing `vika-1.3.0/vika.egg-info/SOURCES.txt` & `vika-1.3.1/vika.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,23 @@
+LICENSE
 README.md
 setup.py
+test/test_apitable.py
 test/test_create_datasheet.py
 test/test_create_embed_link.py
 test/test_create_field.py
 test/test_create_records.py
 test/test_delete_field.py
 test/test_delete_records.py
 test/test_get_fields.py
 test/test_get_nodes.py
 test/test_get_records.py
 test/test_get_spaces.py
 test/test_get_views.py
+test/test_unit.py
 test/test_update_records.py
 test/test_upload_file.py
 test/test_utils.py
 vika/__init__.py
 vika/apitable.py
 vika/const.py
 vika/exceptions.py
```

