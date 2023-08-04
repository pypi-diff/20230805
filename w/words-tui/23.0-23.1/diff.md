# Comparing `tmp/words_tui-23.0.tar.gz` & `tmp/words_tui-23.1.tar.gz`

## Comparing `words_tui-23.0.tar` & `words_tui-23.1.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 words_tui-23.0/.DS_Store
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/__about__.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/__init__.py
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/__main__.py
--rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/cli/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/tui/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/tui/app.css
--rw-r--r--   0        0        0     2393 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/tui/app.py
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/tui/db.py
--rw-r--r--   0        0        0    48046 2020-02-02 00:00:00.000000 words_tui-23.0/src/words_tui/tui/text_editor.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 words_tui-23.0/tests/__init__.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 words_tui-23.0/.gitignore
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 words_tui-23.0/LICENSE.txt
--rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 words_tui-23.0/README.md
--rw-r--r--   0        0        0     3234 2020-02-02 00:00:00.000000 words_tui-23.0/pyproject.toml
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 words_tui-23.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 words_tui-23.1/.DS_Store
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 words_tui-23.1/CHANGELOG.md
+-rw-r--r--   0        0        0      209 2020-02-02 00:00:00.000000 words_tui-23.1/__token__
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 words_tui-23.1/.vscode/launch.json
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/__about__.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/__init__.py
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/__main__.py
+-rw-r--r--   0        0        0      609 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/cli/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/tui/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/tui/app.css
+-rw-r--r--   0        0        0     2301 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/tui/app.py
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/tui/db.py
+-rw-r--r--   0        0        0    48046 2020-02-02 00:00:00.000000 words_tui-23.1/src/words_tui/tui/text_editor.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 words_tui-23.1/tests/__init__.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 words_tui-23.1/.gitignore
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 words_tui-23.1/LICENSE.txt
+-rw-r--r--   0        0        0     1207 2020-02-02 00:00:00.000000 words_tui-23.1/README.md
+-rw-r--r--   0        0        0     3308 2020-02-02 00:00:00.000000 words_tui-23.1/pyproject.toml
+-rw-r--r--   0        0        0     2277 2020-02-02 00:00:00.000000 words_tui-23.1/PKG-INFO
```

### Comparing `words_tui-23.0/.DS_Store` & `words_tui-23.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `words_tui-23.0/src/words_tui/cli/__init__.py` & `words_tui-23.1/src/words_tui/cli/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,11 +8,11 @@
 from words_tui.__about__ import __version__
 from words_tui.tui.app import WordsTui
 from words_tui.tui.db import init_db
 
 
 @click.group(context_settings={"help_option_names": ["-h", "--help"]}, invoke_without_command=True)
 @click.version_option(version=__version__, prog_name="words-tui")
-@click.option("--db", "-d", envvar="WORDS_TUI_DB", default=Path.home() / ".write-tui.db", help="Database file to use")
+@click.option("--db", "-d", envvar="WORDS_TUI_DB", default=Path.home() / ".words-tui.db", help="Database file to use")
 def words_tui(db: str):
     init_db(db)
     WordsTui().run()
```

### Comparing `words_tui-23.0/src/words_tui/tui/app.py` & `words_tui-23.1/src/words_tui/tui/app.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import datetime
 
 from textual.app import App, ComposeResult
 from textual.widgets import Footer, Static
 
-from words_tui.tui.db import Post
+from words_tui.tui.db import Post, get_posts
 from words_tui.tui.text_editor import TextEditor
 
 
 def get_post_icon(post: Post) -> str:
     if len(post.content.split()) > 300:
         return "✅"
     elif post.created_date.date() == datetime.date.today():
@@ -25,14 +25,15 @@
                 f"{len(post.content.split()):5}/300",
             ],
         )
     )
 
 
 def get_sidebar_text(posts: list[Post]) -> str:
+    posts = get_posts()
     return "[bold] # Date      Words/Goal[/bold]\n" + "\n".join(map(get_post_summary, posts))
 
 
 class WordsTui(App):
     """A Textual app for writing."""
 
     BINDINGS = [
@@ -40,20 +41,21 @@
     ]
 
     CSS_PATH = "app.css"
 
     def __init__(self, *args, **kwargs) -> None:
         super().__init__(*args, **kwargs)
         # TODO: Find a better place for this
-        self.posts: list[Post] = Post.select().order_by(Post.created_date.desc()).limit(10)
-        todays_post: list[Post] = [post for post in self.posts if post.created_date.date() == datetime.date.today()]
+        self.posts = get_posts()
+        todays_post = [post for post in self.posts if post.created_date.date() == datetime.date.today()]
         if todays_post:
-            self.todays_post = todays_post[0]
+            self.todays_post: Post = todays_post[0]
         else:
-            self.todays_post = Post.create(content="_")
+            self.todays_post: Post = Post.create(content="")
+            self.posts.insert(0, self.todays_post)
 
         self.editor = TextEditor(id="editor")
         self.editor.show_line_numbers = False
         self.editor.load_text(self.todays_post.content)
 
     def on_text_editor_changed(self, _: TextEditor.Changed) -> None:
         self.update_word_count()
@@ -62,19 +64,15 @@
         text_editor = self.query_one(TextEditor)
         sidebar = self.query_one("#sidebar")
 
         text = "\n".join(text_editor.document_lines)
         self.todays_post.content = text
         self.todays_post.save()
 
-        text_editor.load_text(text)
-
-        posts = Post.select().order_by(Post.created_date.desc()).limit(10)
-
-        sidebar.update(get_sidebar_text(posts))
+        sidebar.update(get_sidebar_text())
 
     def compose(self) -> ComposeResult:
         """Create child widgets for the app."""
 
         yield Static(get_sidebar_text(self.posts), id="sidebar")
         yield self.editor
         yield Footer()
```

### Comparing `words_tui-23.0/src/words_tui/tui/text_editor.py` & `words_tui-23.1/src/words_tui/tui/text_editor.py`

 * *Files identical despite different names*

### Comparing `words_tui-23.0/LICENSE.txt` & `words_tui-23.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `words_tui-23.0/README.md` & `words_tui-23.1/README.md`

 * *Files identical despite different names*

### Comparing `words_tui-23.0/pyproject.toml` & `words_tui-23.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   "click", "textual", "peewee", "tree-sitter"
 ]
 
 [project.urls]
 Documentation = "https://github.com/anze3db/words-tui#readme"
 Issues = "https://github.com/anze3db/words-tui/issues"
 Source = "https://github.com/anze3db/words-tui"
+Changelog = "https://github.com/anze3db/words-tui/blob/main/CHANGELOG.md"
 
 [project.scripts]
 words-tui = "words_tui.cli:words_tui"
 
 [tool.hatch.version]
 path = "src/words_tui/__about__.py"
```

### Comparing `words_tui-23.0/PKG-INFO` & `words_tui-23.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: words-tui
-Version: 23.0
+Version: 23.1
 Summary: A TUI (Text User Interface) app for daily writing.
 Project-URL: Documentation, https://github.com/anze3db/words-tui#readme
 Project-URL: Issues, https://github.com/anze3db/words-tui/issues
 Project-URL: Source, https://github.com/anze3db/words-tui
+Project-URL: Changelog, https://github.com/anze3db/words-tui/blob/main/CHANGELOG.md
 Author-email: Anže Pečar <anze@pecar.me>
 License-Expression: MIT
 License-File: LICENSE.txt
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

