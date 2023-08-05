# Comparing `tmp/zfl_data-0.0.1.tar.gz` & `tmp/zfl_data-0.0.2.tar.gz`

## Comparing `zfl_data-0.0.1.tar` & `zfl_data-0.0.2.tar`

### file list

```diff
@@ -1,34 +1,25 @@
--rwxr-xr-x   0        0        0      626 2020-02-02 00:00:00.000000 zfl_data-0.0.1/manage.py
--rwxr-xr-x   0        0        0       88 2020-02-02 00:00:00.000000 zfl_data-0.0.1/requirements.txt
--rwxr-xr-x   0        0        0     1020 2020-02-02 00:00:00.000000 zfl_data-0.0.1/.github/workflows/publish.yml
--rwxr-xr-x   0        0        0     1036 2020-02-02 00:00:00.000000 zfl_data-0.0.1/.github/workflows/test.yml
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.1/config/__init__.py
--rwxr-xr-x   0        0        0     3754 2020-02-02 00:00:00.000000 zfl_data-0.0.1/config/settings.py
--rwxr-xr-x   0        0        0      793 2020-02-02 00:00:00.000000 zfl_data-0.0.1/config/urls.py
--rwxr-xr-x   0        0        0      389 2020-02-02 00:00:00.000000 zfl_data-0.0.1/config/wsgi.py
--rwxr-xr-x   0        0        0       22 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/__init__.py
--rwxr-xr-x   0        0        0      142 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/admin.py
--rwxr-xr-x   0        0        0      126 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/apps.py
--rwxr-xr-x   0        0        0      949 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/models.py
--rwxr-xr-x   0        0        0      930 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/tests.py
--rwxr-xr-x   0        0        0      207 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/urls.py
--rwxr-xr-x   0        0        0     2941 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/views.py
--rwxr-xr-x   0        0        0     3083 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/management/commands/analytics_api.py
--rwxr-xr-x   0        0        0     1984 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/management/commands/updates.py
--rwxr-xr-x   0        0        0     2297 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0001_initial.py
--rwxr-xr-x   0        0        0      667 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0002_webdata.py
--rwxr-xr-x   0        0        0      318 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0003_remove_webdata_user_date.py
--rwxr-xr-x   0        0        0      503 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0004_godate.py
--rwxr-xr-x   0        0        0      597 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0005_auto_20200727_1146.py
--rwxr-xr-x   0        0        0      363 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0006_auto_20200808_1206.py
--rwxr-xr-x   0        0        0      615 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0007_googleaccess.py
--rwxr-xr-x   0        0        0      639 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/0008_auto_20210327_0952.py
--rwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/migrations/__init__.py
--rwxr-xr-x   0        0        0      118 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/static/data/css/data-style.css
--rwxr-xr-x   0        0        0     3424 2020-02-02 00:00:00.000000 zfl_data-0.0.1/data/templates/data/index.html
--rwxr-xr-x   0        0        0     1206 2020-02-02 00:00:00.000000 zfl_data-0.0.1/templates/base.html
--rwxr-xr-x   0        0        0       97 2020-02-02 00:00:00.000000 zfl_data-0.0.1/.gitignore
--rwxr-xr-x   0        0        0     1101 2020-02-02 00:00:00.000000 zfl_data-0.0.1/LICENSE.txt
--rwxr-xr-x   0        0        0      519 2020-02-02 00:00:00.000000 zfl_data-0.0.1/README.md
--rwxr-xr-x   0        0        0     3439 2020-02-02 00:00:00.000000 zfl_data-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 zfl_data-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/__init__.py
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/admin.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/apps.py
+-rw-r--r--   0        0        0      949 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/models.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/tests.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/urls.py
+-rw-r--r--   0        0        0     2941 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/views.py
+-rw-r--r--   0        0        0     3083 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/management/commands/analytics_api.py
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/management/commands/updates.py
+-rw-r--r--   0        0        0     2297 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0001_initial.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0002_webdata.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0003_remove_webdata_user_date.py
+-rw-r--r--   0        0        0      503 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0004_godate.py
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0005_auto_20200727_1146.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0006_auto_20200808_1206.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0007_googleaccess.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/0008_auto_20210327_0952.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/static/data/css/data-style.css
+-rw-r--r--   0        0        0     3424 2020-02-02 00:00:00.000000 zfl_data-0.0.2/data/templates/data/index.html
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 zfl_data-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1101 2020-02-02 00:00:00.000000 zfl_data-0.0.2/LICENSE.txt
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 zfl_data-0.0.2/README.md
+-rw-r--r--   0        0        0     3435 2020-02-02 00:00:00.000000 zfl_data-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1539 2020-02-02 00:00:00.000000 zfl_data-0.0.2/PKG-INFO
```

### Comparing `zfl_data-0.0.1/data/models.py` & `zfl_data-0.0.2/data/models.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/tests.py` & `zfl_data-0.0.2/data/tests.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,32 +1,29 @@
-﻿import datetime
+﻿from datetime import datetime, timezone
 
-from django.test import TestCase # type: ignore
-from django.urls import reverse # type: ignore
+from django.test import TestCase  # type: ignore
+from django.urls import reverse  # type: ignore
 
 from .models import GoogleAccess
 
 
 class GoogleAccessModelTests(TestCase):
     def test_access_data_str_method(self):
         """
         GoogleAccessモデルのstrメソッドテスト
         """
-        time = datetime.datetime(2023, 8, 4).date()
+        time = datetime(2023, 8, 4, tzinfo=timezone.utc).date()
         access_data = GoogleAccess.objects.create(
-                date_data=time,
-                access_data=1,
+            date_data=time,
+            access_data=1,
         )
         self.assertEqual(access_data.__str__(), "2023-08-04")
-        print(access_data.__str__())
-        print('---------')
+
 
 class IndexTest(TestCase):
     def test_data_pageview(self):
         """
         /data/の表示テスト
         """
         response = self.client.get(reverse("data:index"))
         self.assertEqual(response.status_code, 200)
         self.assertContains(response, "現在チャートはありません")
-
-
```

### Comparing `zfl_data-0.0.1/data/views.py` & `zfl_data-0.0.2/data/views.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/management/commands/analytics_api.py` & `zfl_data-0.0.2/data/management/commands/analytics_api.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/management/commands/updates.py` & `zfl_data-0.0.2/data/management/commands/updates.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/migrations/0001_initial.py` & `zfl_data-0.0.2/data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/migrations/0002_webdata.py` & `zfl_data-0.0.2/data/migrations/0002_webdata.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/migrations/0005_auto_20200727_1146.py` & `zfl_data-0.0.2/data/migrations/0005_auto_20200727_1146.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/migrations/0007_googleaccess.py` & `zfl_data-0.0.2/data/migrations/0007_googleaccess.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/migrations/0008_auto_20210327_0952.py` & `zfl_data-0.0.2/data/migrations/0008_auto_20210327_0952.py`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/data/templates/data/index.html` & `zfl_data-0.0.2/data/templates/data/index.html`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/LICENSE.txt` & `zfl_data-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/README.md` & `zfl_data-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `zfl_data-0.0.1/pyproject.toml` & `zfl_data-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -125,11 +125,11 @@
   "S105", "S106", "S107",
   # Ignore complexity
   "C901", "PLR0911", "PLR0912", "PLR0913", "PLR0915",
 ]
 
 # ビルド実行時に含めるファイルと含めないファイルの設定
 # 以下は配布用Djangoアプリに対しての設定
-# [tool.hatch.build]
-# include = ["data/*"]
+[tool.hatch.build]
+include = ["data/*"]
 # exclude = ["data/migrations/*"]
```

### Comparing `zfl_data-0.0.1/PKG-INFO` & `zfl_data-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfl-data
-Version: 0.0.1
+Version: 0.0.2
 Summary: 'data on zfl'
 Project-URL: Documentation, https://github.com/unknown/Appのパッケージ名#readme
 Project-URL: Issues, https://github.com/unknown/Appのパッケージ名/issues
 Project-URL: Source, https://github.com/unknown/Appのパッケージ名
 Author-email: You are name <example@gmail.com>
 License-Expression: MIT
 License-File: LICENSE.txt
```

