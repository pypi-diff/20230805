# Comparing `tmp/streamlit_calendar_semver-0.3.0.tar.gz` & `tmp/streamlit_calendar_semver-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_calendar_semver-0.3.0.tar", max compression
+gzip compressed data, was "streamlit_calendar_semver-0.4.0.tar", max compression
```

## Comparing `streamlit_calendar_semver-0.3.0.tar` & `streamlit_calendar_semver-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,24 @@
--rw-r--r--   0        0        0    11358 2023-08-05 08:28:23.445947 streamlit_calendar_semver-0.3.0/LICENSE
--rw-r--r--   0        0        0     3510 2023-08-05 08:28:23.445947 streamlit_calendar_semver-0.3.0/README.md
--rw-r--r--   0        0        0     1138 2023-08-05 08:28:59.322585 streamlit_calendar_semver-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    10550 2023-08-05 08:28:23.465947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/__init__.py
--rw-r--r--   0        0        0      180 2023-08-05 08:28:23.465947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/.env
--rw-r--r--   0        0        0       67 2023-08-05 08:28:23.465947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/.prettierrc
--rw-r--r--   0        0        0   700872 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/package-lock.json
--rw-r--r--   0        0        0     1426 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/package.json
--rw-r--r--   0        0        0   198404 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/public/bootstrap.min.css
--rw-r--r--   0        0        0      868 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/public/index.html
--rw-r--r--   0        0        0      216 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/src/Calendar.css
--rw-r--r--   0        0        0     3024 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/src/Calendar.tsx
--rw-r--r--   0        0        0      208 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/src/index.tsx
--rw-r--r--   0        0        0       40 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/src/react-app-env.d.ts
--rw-r--r--   0        0        0      494 2023-08-05 08:28:23.469947 streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/tsconfig.json
--rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 streamlit_calendar_semver-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-08-05 08:54:00.960120 streamlit_calendar_semver-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3510 2023-08-05 08:54:00.960120 streamlit_calendar_semver-0.4.0/README.md
+-rw-r--r--   0        0        0     1138 2023-08-05 08:55:40.316574 streamlit_calendar_semver-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    10550 2023-08-05 08:54:00.988120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/__init__.py
+-rw-r--r--   0        0        0      180 2023-08-05 08:54:00.988120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/.env
+-rw-r--r--   0        0        0       67 2023-08-05 08:54:00.988120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/.prettierrc
+-rw-r--r--   0        0        0      374 2023-08-05 08:55:16.728463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/asset-manifest.json
+-rw-r--r--   0        0        0   198404 2023-08-05 08:54:43.956318 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/bootstrap.min.css
+-rw-r--r--   0        0        0      551 2023-08-05 08:55:16.724463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/index.html
+-rw-r--r--   0        0        0      234 2023-08-05 08:55:16.740463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/static/css/main.7ad33fdc.css
+-rw-r--r--   0        0        0      416 2023-08-05 08:55:16.740463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/static/css/main.7ad33fdc.css.map
+-rw-r--r--   0        0        0   790131 2023-08-05 08:55:16.740463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/static/js/main.beb4af9b.js
+-rw-r--r--   0        0        0     1443 2023-08-05 08:55:16.736463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/static/js/main.beb4af9b.js.LICENSE.txt
+-rw-r--r--   0        0        0  2893172 2023-08-05 08:55:16.740463 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/static/js/main.beb4af9b.js.map
+-rw-r--r--   0        0        0   700872 2023-08-05 08:54:41.044305 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/package-lock.json
+-rw-r--r--   0        0        0     1426 2023-08-05 08:54:00.988120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/package.json
+-rw-r--r--   0        0        0   198404 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/public/bootstrap.min.css
+-rw-r--r--   0        0        0      868 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/public/index.html
+-rw-r--r--   0        0        0      216 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/src/Calendar.css
+-rw-r--r--   0        0        0     3024 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/src/Calendar.tsx
+-rw-r--r--   0        0        0      208 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/src/index.tsx
+-rw-r--r--   0        0        0       40 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      494 2023-08-05 08:54:00.992120 streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/tsconfig.json
+-rw-r--r--   0        0        0     4426 1970-01-01 00:00:00.000000 streamlit_calendar_semver-0.4.0/PKG-INFO
```

### Comparing `streamlit_calendar_semver-0.3.0/LICENSE` & `streamlit_calendar_semver-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/README.md` & `streamlit_calendar_semver-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/pyproject.toml` & `streamlit_calendar_semver-0.4.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-calendar-semver"
-version = "0.3.0"
+version = "0.4.0"
 description = "📆 A Streamlit component to show callendar using FullCalendar (https://fullcalendar.io)"
 authors = ["Muhammad Luqman <im.imperativa@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/im-perativa/streamlit-calendar-semver"
 # This is required so the frontend code is properly included in the wheel. 
 include = ["streamlit_calendar_semver/frontend/build/**/*"]
```

### Comparing `streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/__init__.py` & `streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/package-lock.json` & `streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/package.json` & `streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/package.json`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/public/bootstrap.min.css` & `streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/build/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/public/index.html` & `streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/public/index.html`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/streamlit_calendar_semver/frontend/src/Calendar.tsx` & `streamlit_calendar_semver-0.4.0/streamlit_calendar_semver/frontend/src/Calendar.tsx`

 * *Files identical despite different names*

### Comparing `streamlit_calendar_semver-0.3.0/PKG-INFO` & `streamlit_calendar_semver-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-calendar-semver
-Version: 0.3.0
+Version: 0.4.0
 Summary: 📆 A Streamlit component to show callendar using FullCalendar (https://fullcalendar.io)
 Home-page: https://github.com/im-perativa/streamlit-calendar-semver
 License: Apache-2.0
 Keywords: streamlit,streamlit-component
 Author: Muhammad Luqman
 Author-email: im.imperativa@gmail.com
 Requires-Python: >=3.8,<4.0
```

