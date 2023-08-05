# Comparing `tmp/freetar-0.1.5.tar.gz` & `tmp/freetar-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freetar-0.1.5.tar", max compression
+gzip compressed data, was "freetar-0.1.6.tar", max compression
```

## Comparing `freetar-0.1.5.tar` & `freetar-0.1.6.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2023-04-01 10:41:21.268315 freetar-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-08-05 19:29:51.378461 freetar-0.1.5/freetar/__init__.py
--rw-r--r--   0        0        0     1199 2023-08-05 19:39:57.804774 freetar-0.1.5/freetar/backend.py
--rw-r--r--   0        0        0     1710 2023-08-05 19:52:36.767843 freetar-0.1.5/freetar/templates/base.html
--rw-r--r--   0        0        0     4965 2023-08-05 19:40:18.928216 freetar-0.1.5/freetar/templates/index.html
--rw-r--r--   0        0        0     4015 2023-08-05 19:51:56.417667 freetar-0.1.5/freetar/ug.py
--rw-r--r--   0        0        0      557 2023-08-05 19:53:08.281314 freetar-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 freetar-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-01 10:41:21.268315 freetar-0.1.6/README.md
+-rw-r--r--   0        0        0     1373 2023-08-05 20:13:30.473844 freetar-0.1.6/freetar/backend.py
+-rw-r--r--   0        0        0     2484 2023-08-05 20:39:48.741484 freetar-0.1.6/freetar/static/custom.js
+-rw-r--r--   0        0        0    26135 2023-08-05 19:56:02.105488 freetar-0.1.6/freetar/static/guitar.png
+-rw-r--r--   0        0        0     1826 2023-08-05 20:08:53.349132 freetar-0.1.6/freetar/templates/base.html
+-rw-r--r--   0        0        0     3237 2023-08-05 20:37:34.557493 freetar-0.1.6/freetar/templates/index.html
+-rw-r--r--   0        0        0     4015 2023-08-05 19:51:56.417667 freetar-0.1.6/freetar/ug.py
+-rw-r--r--   0        0        0      557 2023-08-05 20:43:02.582427 freetar-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 freetar-0.1.6/PKG-INFO
```

### Comparing `freetar-0.1.5/LICENSE` & `freetar-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `freetar-0.1.5/freetar/backend.py` & `freetar-0.1.6/freetar/backend.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,14 +28,20 @@
 def show_tab(artist: str, song: str):
     tab = ug_tab(f"{artist}/{song}")
     return render_template("index.html",
                            tab=tab,
                            title=f"{tab.artist_name} - {tab.song_name}")
 
 
+@app.route("/favs")
+def show_favs():
+    return render_template("index.html",
+                           title=f"Freetar - Favorites",
+                           favs=True)
+
 def main():
     host = "0.0.0.0"
     port = 22000
     if __name__ == '__main__':
         app.run(debug=True,
                 host=host,
                 port=port)
```

### Comparing `freetar-0.1.5/freetar/templates/base.html` & `freetar-0.1.6/freetar/templates/base.html`

 * *Files 6% similar despite different names*

```diff
@@ -12,26 +12,32 @@
 
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
 
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
 
 
     <title>{{ title or "Welcome to Freetar" }}</title>
+
+
+    <link rel="icon" type="image/png" href="/static/guitar.png"/>
+
+
   </head>
   <body>
 
       <h2>&nbsp;</h2>
 <div class="container">
 
     
     {% block content %}
     {% endblock %}
 
 </div>
 
+    <script src="/static/custom.js"></script>
 
     <!-- Optional JavaScript; choose one of the two! -->
 
     <!-- Option 1: Bootstrap Bundle with Popper -->
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
 
     <!-- Option 2: Separate Popper and Bootstrap JS -->
```

### Comparing `freetar-0.1.5/freetar/ug.py` & `freetar-0.1.6/freetar/ug.py`

 * *Files identical despite different names*

### Comparing `freetar-0.1.5/pyproject.toml` & `freetar-0.1.6/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freetar"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 repository = "https://github.com/kmille/freetar"
 homepage = "https://github.com/kmille/freetar"
```

### Comparing `freetar-0.1.5/PKG-INFO` & `freetar-0.1.6/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freetar
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/kmille/freetar
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

