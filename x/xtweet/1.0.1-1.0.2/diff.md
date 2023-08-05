# Comparing `tmp/xtweet-1.0.1-py3-none-any.whl.zip` & `tmp/xtweet-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5079 bytes, number of entries: 9
+Zip file size: 5078 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat       61 b- defN 23-Aug-05 00:50 xtweet/__init__.py
 -rw-rw-rw-  2.0 fat     1676 b- defN 23-Aug-05 01:04 xtweet/main.py
--rw-rw-rw-  2.0 fat     2949 b- defN 23-Aug-05 01:04 xtweet/media.py
+-rw-rw-rw-  2.0 fat     2956 b- defN 23-Aug-05 02:03 xtweet/media.py
 -rw-rw-rw-  2.0 fat      533 b- defN 23-Aug-05 01:56 xtweet/request.py
--rw-rw-rw-  2.0 fat     1094 b- defN 23-Aug-05 01:58 xtweet-1.0.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2712 b- defN 23-Aug-05 01:58 xtweet-1.0.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 01:58 xtweet-1.0.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-05 01:58 xtweet-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      669 b- defN 23-Aug-05 01:58 xtweet-1.0.1.dist-info/RECORD
-9 files, 9793 bytes uncompressed, 3937 bytes compressed:  59.8%
+-rw-rw-rw-  2.0 fat     1094 b- defN 23-Aug-05 02:05 xtweet-1.0.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2712 b- defN 23-Aug-05 02:05 xtweet-1.0.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-05 02:05 xtweet-1.0.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Aug-05 02:05 xtweet-1.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      669 b- defN 23-Aug-05 02:05 xtweet-1.0.2.dist-info/RECORD
+9 files, 9800 bytes uncompressed, 3936 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: xtweet/media.py
 Comment: 
 
 Filename: xtweet/request.py
 Comment: 
 
-Filename: xtweet-1.0.1.dist-info/LICENSE
+Filename: xtweet-1.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: xtweet-1.0.1.dist-info/METADATA
+Filename: xtweet-1.0.2.dist-info/METADATA
 Comment: 
 
-Filename: xtweet-1.0.1.dist-info/WHEEL
+Filename: xtweet-1.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: xtweet-1.0.1.dist-info/top_level.txt
+Filename: xtweet-1.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: xtweet-1.0.1.dist-info/RECORD
+Filename: xtweet-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xtweet/media.py

```diff
@@ -45,15 +45,15 @@
                     response = requests.get(url_photo)
                     if response.status_code == 200:
                         with open(os.path.join(fp, f"{name_file}_{i}.jpg"), 'wb') as f:
                             f.write(response.content)
                     else:
                         raise requests.exceptions.HTTPError(f"No se pudo descargar la imagen {i}. Código de estado: {response.status_code}")
 
-    def download_video(self, fp: str, name_file: str = "video") -> None:
+    def download_video(self, fp: str = './', name_file: str = "video") -> None:
         """
         Descarga el primer video incluido en el tweet, si está disponible.
 
         Args:
             fp (str): Ruta del directorio en el que se guardará el video.
             name_file (str): Nombre del archivo en el que se guardará el video.
         """
```

## Comparing `xtweet-1.0.1.dist-info/LICENSE` & `xtweet-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xtweet-1.0.1.dist-info/METADATA` & `xtweet-1.0.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xtweet
-Version: 1.0.1
+Version: 1.0.2
 Summary: Es una biblioteca que te permite interactuar de manera eficiente con la API de Twitter.
 Home-page: https://github.com/fcoagz/pydolarvenezuela
 Author: Francisco Griman
 Author-email: Francisco Griman <grihardware@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/fcoagz/xtweet
 Project-URL: Bug Tracker, https://github.com/fcoagz/xtweet/issues
```

