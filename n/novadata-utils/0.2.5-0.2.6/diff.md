# Comparing `tmp/novadata_utils-0.2.5.tar.gz` & `tmp/novadata_utils-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novadata_utils-0.2.5.tar", last modified: Sat May 20 14:16:37 2023, max compression
+gzip compressed data, was "novadata_utils-0.2.6.tar", last modified: Sat Aug  5 14:43:14 2023, max compression
```

## Comparing `novadata_utils-0.2.5.tar` & `novadata_utils-0.2.6.tar`

### file list

```diff
@@ -1,60 +1,71 @@
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/LICENSE
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1179 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      734 2023-05-20 14:16:14.000000 novadata_utils-0.2.5/README.md
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/admin/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/admin/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     4435 2023-05-20 14:12:24.000000 novadata_utils-0.2.5/novadata_utils/admin/novadata_model_admin.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/apps.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/auth/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/auth/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/auth/login_username_email.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/forms/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/forms/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/functions/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      177 2023-04-16 18:28:57.000000 novadata_utils-0.2.5/novadata_utils/functions/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2186 2023-04-16 18:28:38.000000 novadata_utils-0.2.5/novadata_utils/functions/get_prop.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2979 2023-04-16 18:28:07.000000 novadata_utils-0.2.5/novadata_utils/functions/props_dict.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.5/novadata_utils/functions/transform_field.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/managers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/managers/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils/middlewares/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/middlewares/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/migrations/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/migrations/0001_initial.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/migrations/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/models/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/models/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1188 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/models/novadata_model.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/redirect/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/redirect/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/redirect/reverse_lazy_plus.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/save/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/save/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/save/create_logs.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/save/get_changes.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/serializers/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/serializers/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1934 2023-04-16 16:54:07.000000 novadata_utils-0.2.5/novadata_utils/serializers/novadata_model_serializer.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/signals/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/signals/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/templatetags/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/templatetags/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/tests/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/tests/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/urls.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/views/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/views/__init__.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/novadata_utils/viewsets/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.5/novadata_utils/viewsets/__init__.py
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     5457 2023-04-16 18:25:27.000000 novadata_utils-0.2.5/novadata_utils/viewsets/novadata_model_viewset.py
-drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-05-20 14:16:37.614249 novadata_utils-0.2.5/novadata_utils.egg-info/
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1179 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/PKG-INFO
--rw-rw-r--   0 flavio    (1000) flavio    (1000)     1366 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      147 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/requires.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-05-20 14:16:37.000000 novadata_utils-0.2.5/novadata_utils.egg-info/top_level.txt
--rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-05-20 14:16:37.618249 novadata_utils-0.2.5/setup.cfg
--rw-rw-r--   0 flavio    (1000) flavio    (1000)      913 2023-05-20 14:16:34.000000 novadata_utils-0.2.5/setup.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.439248 novadata_utils-0.2.6/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1066 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/LICENSE
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1450 2023-08-05 14:43:14.439248 novadata_utils-0.2.6/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1025 2023-08-05 14:42:56.000000 novadata_utils-0.2.6/README.md
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.431248 novadata_utils-0.2.6/novadata_utils/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       60 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/admin/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/admin/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     5197 2023-07-10 18:07:32.000000 novadata_utils-0.2.6/novadata_utils/admin/novadata_model_admin.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      219 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/apps.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/auth/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       92 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/auth/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      729 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/auth/login_username_email.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/breadcrumbs/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      229 2023-08-05 13:47:22.000000 novadata_utils-0.2.6/novadata_utils/breadcrumbs/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2468 2023-08-05 13:53:56.000000 novadata_utils-0.2.6/novadata_utils/breadcrumbs/crud_breadcrumbs.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      411 2023-08-05 13:51:05.000000 novadata_utils-0.2.6/novadata_utils/breadcrumbs/items.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      196 2023-08-05 13:51:23.000000 novadata_utils-0.2.6/novadata_utils/breadcrumbs/make_breadcrumb.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      473 2023-08-05 13:54:08.000000 novadata_utils-0.2.6/novadata_utils/breadcrumbs/make_item_breadcrumb.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/forms/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       99 2023-08-05 13:44:07.000000 novadata_utils-0.2.6/novadata_utils/forms/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      765 2023-08-05 13:43:46.000000 novadata_utils-0.2.6/novadata_utils/forms/gerenciar_inline_form.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/functions/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      177 2023-04-16 18:28:57.000000 novadata_utils-0.2.6/novadata_utils/functions/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2334 2023-07-10 18:09:06.000000 novadata_utils-0.2.6/novadata_utils/functions/get_prop.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     3474 2023-07-10 18:19:50.000000 novadata_utils-0.2.6/novadata_utils/functions/props_dict.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      416 2023-04-10 14:19:49.000000 novadata_utils-0.2.6/novadata_utils/functions/transform_field.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/managers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/managers/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/middlewares/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/middlewares/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/migrations/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1232 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/migrations/0001_initial.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/migrations/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/models/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       76 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/models/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1217 2023-08-05 13:29:02.000000 novadata_utils-0.2.6/novadata_utils/models/novadata_model.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/redirect/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       87 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/redirect/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1130 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/redirect/reverse_lazy_plus.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/save/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      130 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/save/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1749 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/save/create_logs.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2152 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/save/get_changes.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/serializers/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      107 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/serializers/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     2019 2023-06-02 13:54:16.000000 novadata_utils-0.2.6/novadata_utils/serializers/novadata_model_serializer.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/signals/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       20 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/signals/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/templatetags/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/templatetags/__init__.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/tests/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        0 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/tests/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       58 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/urls.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.435248 novadata_utils-0.2.6/novadata_utils/utils/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       93 2023-08-05 13:49:06.000000 novadata_utils-0.2.6/novadata_utils/utils/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      177 2023-08-05 13:49:21.000000 novadata_utils-0.2.6/novadata_utils/utils/camel_to_snake_case.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.439248 novadata_utils-0.2.6/novadata_utils/views/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       73 2023-08-05 13:46:44.000000 novadata_utils-0.2.6/novadata_utils/views/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      727 2023-08-05 13:46:17.000000 novadata_utils-0.2.6/novadata_utils/views/novadata_view.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.439248 novadata_utils-0.2.6/novadata_utils/viewsets/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       98 2023-04-04 12:57:52.000000 novadata_utils-0.2.6/novadata_utils/viewsets/__init__.py
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     6102 2023-08-05 14:15:28.000000 novadata_utils-0.2.6/novadata_utils/viewsets/novadata_model_viewset.py
+drwxrwxr-x   0 flavio    (1000) flavio    (1000)        0 2023-08-05 14:43:14.431248 novadata_utils-0.2.6/novadata_utils.egg-info/
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1450 2023-08-05 14:43:14.000000 novadata_utils-0.2.6/novadata_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)     1746 2023-08-05 14:43:14.000000 novadata_utils-0.2.6/novadata_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)        1 2023-08-05 14:43:14.000000 novadata_utils-0.2.6/novadata_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      147 2023-08-05 14:43:14.000000 novadata_utils-0.2.6/novadata_utils.egg-info/requires.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       15 2023-08-05 14:43:14.000000 novadata_utils-0.2.6/novadata_utils.egg-info/top_level.txt
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)       38 2023-08-05 14:43:14.439248 novadata_utils-0.2.6/setup.cfg
+-rw-rw-r--   0 flavio    (1000) flavio    (1000)      913 2023-08-05 14:33:53.000000 novadata_utils-0.2.6/setup.py
```

### Comparing `novadata_utils-0.2.5/LICENSE` & `novadata_utils-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.5/README.md` & `novadata_utils-0.2.6/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # novadata utils
-Pacote para facilitar o seu dia a dia como programador Django.
+Package to facilitate your day to day as a Django developer.
 
 ## Getting Started
+Follow the step by step below to install and configure the package.
 
-### Dependências
-Django
-Django Rest Framework
+### Dependencies
+Depends on the following packages (which will be installed automatically):
 
-#### Installation
+Django | Django Rest Framework | Django Advanced Filters | Django Admin List Filter Dropdown | Django Object Actions | Django Import Export | Django Crum.
+
+### Installation and configuration
 ```shell
 pip install novadata-utils
 ```
 
 Settings.py:
 ```python
 INSTALLED_APPS = [
@@ -20,28 +22,29 @@
     'django_admin_listfilter_dropdown',
     'django_object_actions',
     'import_export',
     'novadata_utils',
     'rest_framework',
     ...
 ]
+
+# After Django middlewares
+MIDDLEWARE += ('crum.CurrentRequestUserMiddleware',)
 ```
 
-Urls.py principal:
+Main urls.py:
 ```python
 urlpatterns = [
     ...
     path('advanced_filters/', include('advanced_filters.urls')),
     ...
 ]
 ```
 
-MIDDLEWARE += ('crum.CurrentRequestUserMiddleware',)
-```
 
-Rode os seguintes comandos:
+Run migrations:
 ```python
 python manage.py makemigrations
 python manage.py migrate
 ```
 
 ## Features
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `novadata_utils-0.2.5/novadata_utils/admin/novadata_model_admin.py` & `novadata_utils-0.2.6/novadata_utils/admin/novadata_model_admin.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 from functools import partial
 
-from advanced_filters.admin import AdminAdvancedFiltersMixin
+from advanced_filters.admin import (
+    AdminAdvancedFiltersMixin,
+    AdvancedListFilters,
+)
 from django.contrib import admin
 from django_object_actions import DjangoObjectActions
 from import_export.admin import ImportExportMixin
 
 from novadata_utils.functions import get_prop, transform_field
 
 
@@ -36,14 +39,16 @@
 
     auto_search_fields: bool = True
 
     filter_horizontal: list = []
 
     exclude: list = []
 
+    advanced_filter_fields: list = []
+
     def get_list_display(self, request):
         """Retorna a lista de campos que estarão na listagem."""
         super().get_list_display(request)
 
         if not self.list_display:
             model = self.model
             list_display = get_prop(model, "list_display")
@@ -64,15 +69,19 @@
         else:
             return self.search_fields
 
     def get_list_filter(self, request):
         """Retorna a lista de campos que estarão no filtro."""
         super().get_list_filter(request)
 
-        if not self.list_filter:
+        len_is_one = len(self.list_filter) == 1
+        is_advanced_filter = self.list_filter[0] == AdvancedListFilters
+        only_has_advanced_filter = len_is_one and is_advanced_filter
+
+        if not self.list_filter or only_has_advanced_filter:
             model = self.model
             foreign_keys = get_prop(model, "foreign_keys")
             choices_fields = get_prop(model, "choices_fields")
 
             list_filter_fields = get_prop(model, "list_filter")
 
             transform_foreign_keys = partial(
@@ -85,15 +94,15 @@
                 choices_fields,
                 "choices_fields",
             )
 
             list_filter = list(map(transform_foreign_keys, list_filter_fields))
             list_filter = list(map(transform_choices_fields, list_filter))
 
-            return list_filter
+            return list(self.list_filter) + list_filter
         else:
             return self.list_filter
 
     def get_autocomplete_fields(self, request):
         """Retorna a lista de campos que estarão no autocomplete."""
         super().get_autocomplete_fields(request)
 
@@ -136,11 +145,22 @@
             "usuario_atualizacao",
             "created_by",
             "updated_by",
         ]
 
         return exclude_fields
 
+    def get_advanced_filter_fields(self):
+        """Retorna a lista de campos que estarão no advanced filter."""
+        if not self.advanced_filter_fields:
+            model = self.model
+            advanced_filter_fields = get_prop(model, "advanced_filter_fields")
+
+            return advanced_filter_fields
+        else:
+            return self.advanced_filter_fields
+
     def __init__(self, *args, **kwargs):
         """Método para executarmos ações ao iniciar a classe."""
         super().__init__(*args, **kwargs)
         self.filter_horizontal = self.get_filter_horizontal()
+        self.advanced_filter_fields = self.get_advanced_filter_fields()
```

### Comparing `novadata_utils-0.2.5/novadata_utils/auth/login_username_email.py` & `novadata_utils-0.2.6/novadata_utils/auth/login_username_email.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.5/novadata_utils/functions/get_prop.py` & `novadata_utils-0.2.6/novadata_utils/functions/get_prop.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,25 +49,31 @@
         exibidos na listagem do admin. Que são:
             "BigAutoField",
             "BooleanField",
             "CharField",
             "DateField",
             "DateTimeField",
             "DecimalField",
+            "OneToOneField",
             "ForeignKey",
             "IntegerField" e
             "PositiveIntegerField".
     """
     props = []
     fields = get_fields(model)
     for field in fields:
         field_type = get_field_type(field)
 
         is_original_field = not hasattr(field, "field")
-        if field_type in props_dict[prop] and is_original_field:
+        is_sub_id_field = "_ptr" in field.name
+        if (
+            field_type in props_dict[prop]
+            and is_original_field
+            and not is_sub_id_field
+        ):
             if str:
                 name = f'"{field.name}",'
             else:
                 name = field.name
 
             if annotate_type:
                 props.append({"name": name, "type": field_type})
```

### Comparing `novadata_utils-0.2.5/novadata_utils/functions/props_dict.py` & `novadata_utils-0.2.6/novadata_utils/functions/props_dict.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,15 @@
         "BigAutoField",
         "BooleanField",
         "CharField",
         "DateField",
         "DateTimeField",
         "DecimalField",
         "ForeignKey",
+        "OneToOneField",
         "IntegerField",
         "PositiveIntegerField",
         "ChoicesField",
     ],
     "search_fields": [
         "BigAutoField",
         "CharField",
@@ -27,22 +28,37 @@
         "BooleanField",
         "DateField",
         "DateTimeField",
         "ForeignKey",
         "ChoicesField",
     ],
     "autocomplete_fields": [
+        "OneToOneField",
         "ForeignKey",
     ],
     "list_select_related": [
+        "OneToOneField",
         "ForeignKey",
     ],
     "filter_horizontal": [
         "ManyToManyField",
     ],
+    "advanced_filter_fields": [
+        "BigAutoField",
+        "BooleanField",
+        "CharField",
+        "DateField",
+        "DateTimeField",
+        "DecimalField",
+        "ForeignKey",
+        "OneToOneField",
+        "IntegerField",
+        "PositiveIntegerField",
+        "ChoicesField",
+    ],
     # Generic props
     "foreign_keys": [
         "ForeignKey",
     ],
     "many_to_many": [
         "ManyToManyField",
     ],
@@ -53,25 +69,27 @@
         "DecimalField",
         "IntegerField",
         "PositiveIntegerField",
         "ChoicesField",
         "BooleanField",
         "DateField",
         "DateTimeField",
+        "OneToOneField",
         "ForeignKey",
     ],
     "ordering_fields": [
         "BigAutoField",
         "CharField",
         "DateField",
         "DateTimeField",
         "DecimalField",
         "IntegerField",
         "PositiveIntegerField",
         "BooleanField",
+        "OneToOneField",
         "ForeignKey",
         "ChoicesField",
     ],
     # Viewset sub props
     "BigAutoField": [
         "exact",
         "in",
@@ -146,14 +164,18 @@
     "BooleanField": [
         "exact",
     ],
     "ForeignKey": [
         "exact",
         "isnull",
     ],
+    "OneToOneField": [
+        "exact",
+        "isnull",
+    ],
     "ManyToManyField": [
         "exact",
         "in",
         "isnull",
     ],
     # Especific props
     "choices_fields": [
```

### Comparing `novadata_utils-0.2.5/novadata_utils/migrations/0001_initial.py` & `novadata_utils-0.2.6/novadata_utils/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.5/novadata_utils/models/novadata_model.py` & `novadata_utils-0.2.6/novadata_utils/models/novadata_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from django.contrib.auth.models import User
+from django.conf import settings
 from django.db import models
 
 
 class NovadataModel(models.Model):
     data_criacao = models.DateTimeField(
         verbose_name="Data de criação",
         auto_now_add=True,
@@ -10,23 +10,23 @@
 
     data_atualizacao = models.DateTimeField(
         verbose_name="Data de atualização",
         auto_now=True,
     )
 
     usuario_criacao = models.ForeignKey(
-        User,
+        settings.AUTH_USER_MODEL,
         on_delete=models.SET_NULL,
         verbose_name="Usuário de criação",
         blank=True,
         null=True,
     )
 
     usuario_atualizacao = models.ForeignKey(
-        User,
+        settings.AUTH_USER_MODEL,
         related_name="%(class)s_requests_modified",
         verbose_name="Usuário de atualização",
         on_delete=models.SET_NULL,
         blank=True,
         null=True,
     )
```

### Comparing `novadata_utils-0.2.5/novadata_utils/redirect/reverse_lazy_plus.py` & `novadata_utils-0.2.6/novadata_utils/redirect/reverse_lazy_plus.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.5/novadata_utils/save/create_logs.py` & `novadata_utils-0.2.6/novadata_utils/save/create_logs.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.5/novadata_utils/save/get_changes.py` & `novadata_utils-0.2.6/novadata_utils/save/get_changes.py`

 * *Files identical despite different names*

### Comparing `novadata_utils-0.2.5/novadata_utils/serializers/novadata_model_serializer.py` & `novadata_utils-0.2.6/novadata_utils/serializers/novadata_model_serializer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,18 @@
         """
         Função para retornar só uma parte dos campos.
 
         Se o usuário passar a propriedade fields na querystring, ele vai
         retornar só os campos que foram passados.
         """
         fields = super().get_fields()
-        request = self.context.get("request")
+        request = self.context.get("request", None)
+        if not request or not request.query_params:
+            return fields
+
         param_fields = request.query_params.get("fields", None)
 
         if param_fields:
             list_param_fields = param_fields.split(",")
             trated_param_fields = [
                 field_name.strip() for field_name in list_param_fields
             ]
```

### Comparing `novadata_utils-0.2.5/novadata_utils/viewsets/novadata_model_viewset.py` & `novadata_utils-0.2.6/novadata_utils/viewsets/novadata_model_viewset.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,19 +21,28 @@
 
     ordering_fields: list = None
 
     search_fields: list = None
 
     auto_search_fields: bool = True
 
+    list_select_related: list = None
+
     relation_fields = [
         "OneToOneField",
         "ForeignKey",
     ]
 
+    def get_queryset(self):
+        """Define o queryset."""
+        model = self.serializer_class().Meta.model
+        return model.objects.select_related(
+            *self.list_select_related,
+        ).all()
+
     def get_filterset_fields(self):
         """Retorna os campos de filtro."""
         model = self.serializer_class().Meta.model
         list_filterset_fields = get_prop(
             model,
             "filterset_fields",
             annotate_type=True,
@@ -74,14 +83,24 @@
             type = search_field["type"]
 
             sub_props = props_dict.get(type, [])
             dict_search_fields[name] = sub_props
 
         return dict_search_fields
 
+    def get_list_select_related(self):
+        """Retorna os campos do select_related."""
+        model = self.serializer_class().Meta.model
+        list_select_related = get_prop(
+            model,
+            "list_select_related",
+        )
+
+        return list_select_related
+
     def get_fk_fields(self):
         """Retorna os campos de relacionamento."""
         model = self.serializer_class().Meta.model
         fields = model._meta.get_fields()
         fk_fields = [
             (field.name, field.remote_field.model)
             for field in fields
@@ -171,7 +190,10 @@
             self.filterset_fields = self.get_filterset_fields()
 
         if not self.ordering_fields:
             self.ordering_fields = self.get_ordering_fields()
 
         if self.auto_search_fields and not self.search_fields:
             self.search_fields = self.get_search_fields()
+
+        if not self.list_select_related:
+            self.list_select_related = self.get_list_select_related()
```

### Comparing `novadata_utils-0.2.5/novadata_utils.egg-info/SOURCES.txt` & `novadata_utils-0.2.6/novadata_utils.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,21 @@
 novadata_utils.egg-info/dependency_links.txt
 novadata_utils.egg-info/requires.txt
 novadata_utils.egg-info/top_level.txt
 novadata_utils/admin/__init__.py
 novadata_utils/admin/novadata_model_admin.py
 novadata_utils/auth/__init__.py
 novadata_utils/auth/login_username_email.py
+novadata_utils/breadcrumbs/__init__.py
+novadata_utils/breadcrumbs/crud_breadcrumbs.py
+novadata_utils/breadcrumbs/items.py
+novadata_utils/breadcrumbs/make_breadcrumb.py
+novadata_utils/breadcrumbs/make_item_breadcrumb.py
 novadata_utils/forms/__init__.py
+novadata_utils/forms/gerenciar_inline_form.py
 novadata_utils/functions/__init__.py
 novadata_utils/functions/get_prop.py
 novadata_utils/functions/props_dict.py
 novadata_utils/functions/transform_field.py
 novadata_utils/managers/__init__.py
 novadata_utils/middlewares/__init__.py
 novadata_utils/migrations/0001_initial.py
@@ -30,10 +36,13 @@
 novadata_utils/save/create_logs.py
 novadata_utils/save/get_changes.py
 novadata_utils/serializers/__init__.py
 novadata_utils/serializers/novadata_model_serializer.py
 novadata_utils/signals/__init__.py
 novadata_utils/templatetags/__init__.py
 novadata_utils/tests/__init__.py
+novadata_utils/utils/__init__.py
+novadata_utils/utils/camel_to_snake_case.py
 novadata_utils/views/__init__.py
+novadata_utils/views/novadata_view.py
 novadata_utils/viewsets/__init__.py
 novadata_utils/viewsets/novadata_model_viewset.py
```

### Comparing `novadata_utils-0.2.5/setup.py` & `novadata_utils-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as fh:
     readme = fh.read()
 
 setup(
     name="novadata_utils",
-    version="0.2.5",
+    version="0.2.6",
     url="https://github.com/TimeNovaData/novadata_utils/",
     license="MIT License",
     author="Flávio Silva",
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email="flavio.nogueira.profissional@gmail.com",
     keywords="Django, utils, ndt, novadata, nova data, nova, data",
```

