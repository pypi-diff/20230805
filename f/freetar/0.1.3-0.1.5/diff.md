# Comparing `tmp/freetar-0.1.3.tar.gz` & `tmp/freetar-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "freetar-0.1.3.tar", max compression
+gzip compressed data, was "freetar-0.1.5.tar", max compression
```

## Comparing `freetar-0.1.3.tar` & `freetar-0.1.5.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2023-04-01 10:41:21.268315 freetar-0.1.3/README.md
--rw-r--r--   0        0        0     1049 2023-05-23 18:11:27.344236 freetar-0.1.3/freetar/backend.py
--rw-r--r--   0        0        0     1669 2023-05-23 17:55:05.049736 freetar-0.1.3/freetar/templates/base.html
--rw-r--r--   0        0        0     5083 2023-05-23 18:02:54.775254 freetar-0.1.3/freetar/templates/index.html
--rw-r--r--   0        0        0     4012 2023-05-23 18:29:26.139014 freetar-0.1.3/freetar/ug.py
--rw-r--r--   0        0        0      557 2023-05-23 18:29:54.242471 freetar-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 freetar-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-04-01 10:41:21.264981 freetar-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2023-04-01 10:41:21.268315 freetar-0.1.5/README.md
+-rw-r--r--   0        0        0        0 2023-08-05 19:29:51.378461 freetar-0.1.5/freetar/__init__.py
+-rw-r--r--   0        0        0     1199 2023-08-05 19:39:57.804774 freetar-0.1.5/freetar/backend.py
+-rw-r--r--   0        0        0     1710 2023-08-05 19:52:36.767843 freetar-0.1.5/freetar/templates/base.html
+-rw-r--r--   0        0        0     4965 2023-08-05 19:40:18.928216 freetar-0.1.5/freetar/templates/index.html
+-rw-r--r--   0        0        0     4015 2023-08-05 19:51:56.417667 freetar-0.1.5/freetar/ug.py
+-rw-r--r--   0        0        0      557 2023-08-05 19:53:08.281314 freetar-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 freetar-0.1.5/PKG-INFO
```

### Comparing `freetar-0.1.3/LICENSE` & `freetar-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `freetar-0.1.3/freetar/backend.py` & `freetar-0.1.5/freetar/backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from flask import Flask, render_template, request
 
-from .ug import ug_search, ug_tab
+from freetar.ug import ug_search, ug_tab
 import waitress
 
 app = Flask(__name__)
 
 
 @app.route("/")
 def index():
@@ -16,22 +16,24 @@
     search_term = request.args.get("search_term")
     if search_term:
         search_results = ug_search(search_term)
     else:
         search_results = []
     return render_template("index.html",
                            search_term=search_term,
-                           search_results=search_results)
+                           title=f"Freetar - Search: {search_term}",
+                           search_results=search_results,)
 
 
 @app.route("/tab/<artist>/<song>")
 def show_tab(artist: str, song: str):
     tab = ug_tab(f"{artist}/{song}")
     return render_template("index.html",
-                           tab=tab)
+                           tab=tab,
+                           title=f"{tab.artist_name} - {tab.song_name}")
 
 
 def main():
     host = "0.0.0.0"
     port = 22000
     if __name__ == '__main__':
         app.run(debug=True,
```

### Comparing `freetar-0.1.3/freetar/templates/base.html` & `freetar-0.1.5/freetar/templates/base.html`

 * *Files 12% similar despite different names*

```diff
@@ -11,36 +11,35 @@
 
 
     <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">
 
     <script src="https://ajax.googleapis.com/ajax/libs/jquery/3.6.3/jquery.min.js"></script>
 
 
-    <title>Hello, world!</title>
+    <title>{{ title or "Welcome to Freetar" }}</title>
   </head>
   <body>
-    <h1>Hello, world!</h1>
-
 
+      <h2>&nbsp;</h2>
 <div class="container">
 
-
+    
     {% block content %}
     {% endblock %}
 
-
 </div>
 
 
     <!-- Optional JavaScript; choose one of the two! -->
 
     <!-- Option 1: Bootstrap Bundle with Popper -->
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-MrcW6ZMFYlzcLA8Nl+NtUVF0sA7MsXsP1UyJoMp4YLEuNSfAP+JcXn/tWtIaxVXM" crossorigin="anonymous"></script>
 
     <!-- Option 2: Separate Popper and Bootstrap JS -->
     <!--
     <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.9.2/dist/umd/popper.min.js" integrity="sha384-IQsoLXl5PILFhosVNubq5LC7Qb9DXgDA9i+tQ8Zj3iwWAwPtgFTxbJ8NT4GN1R8p" crossorigin="anonymous"></script>
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0-alpha3/dist/js/bootstrap.bundle.min.js" integrity="sha384-ENjdO4Dr2bkBIFxQpeoTz1HIcje39Wm4jDKdf19U8gI4ddQ3GYNS7NTKfAdVQSZe" crossorigin="anonymous"></script>
 
     -->
+      <h2>&nbsp;</h2>
   </body>
 </html>
```

#### html2text {}

```diff
@@ -1,8 +1,9 @@
 
 
 
 
-****** Hello, world! ******
+*****   *****
 {% block content %} {% endblock %}
 
 
+*****   *****
```

### Comparing `freetar-0.1.3/freetar/templates/index.html` & `freetar-0.1.5/freetar/templates/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -11,19 +11,14 @@
   
 <div class="col-md-2">
     <button type="submit" class="btn btn-primary">Search</button>
     <button type="button" class="btn btn-primary" onclick="$('#search_term').val('')" >Clear</button>
 </div>
 </form>
       
-<i class="fa fa-regular fa-star"></i>
-<i class="fa fa-star"></i>
-<i class="fa fa-star" style="color: #ffae00;"></i>
-
-
 {% if search_results is defined %}
     <table id="results" class="table">
       <thead>
         <tr>
           <th scope="col">artist</th>
           <th scope="col">song</th>
           <th scope="col">rating</th>
```

### Comparing `freetar-0.1.3/freetar/ug.py` & `freetar-0.1.5/freetar/ug.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
 
     def fix_tab(self):
         tab = self.tab
         tab = tab.replace("\r\n", "</br>")
         tab = tab.replace(" ", "&nbsp;")
         tab = tab.replace("[tab]", "")
         tab = tab.replace("[/tab]", "")
-        tab = re.sub(r'\[ch\](\w+)\[\/ch\]', r'<strong>\1</strong>', tab)
+        tab = re.sub(r'\[ch\]([#\w]+)\[\/ch\]', r'<strong>\1</strong>', tab)
         self.tab = tab
 
 
 def ug_search(value: str):
     resp = requests.get(f"https://www.ultimate-guitar.com/search.php?search_type=title&value={quote(value)}")
     bs = BeautifulSoup(resp.text, 'html.parser')
     # data can be None
```

### Comparing `freetar-0.1.3/pyproject.toml` & `freetar-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "freetar"
-version = "0.1.3"
+version = "0.1.5"
 description = ""
 authors = ["kmille <github@androidloves.me>"]
 readme = "README.md"
 repository = "https://github.com/kmille/freetar"
 homepage = "https://github.com/kmille/freetar"
```

### Comparing `freetar-0.1.3/PKG-INFO` & `freetar-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: freetar
-Version: 0.1.3
+Version: 0.1.5
 Summary: 
 Home-page: https://github.com/kmille/freetar
 Author: kmille
 Author-email: github@androidloves.me
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

