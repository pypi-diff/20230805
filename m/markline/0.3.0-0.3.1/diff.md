# Comparing `tmp/markline-0.3.0.tar.gz` & `tmp/markline-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markline-0.3.0.tar", max compression
+gzip compressed data, was "markline-0.3.1.tar", max compression
```

## Comparing `markline-0.3.0.tar` & `markline-0.3.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1069 2023-05-27 10:24:23.478139 markline-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1398 2023-05-27 10:24:23.478139 markline-0.3.0/README.md
--rw-r--r--   0        0        0    27809 2023-05-27 10:24:23.478139 markline-0.3.0/markline/__init__.py
--rw-r--r--   0        0        0      604 2023-05-27 10:24:23.478139 markline-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2106 1970-01-01 00:00:00.000000 markline-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-08-05 02:55:58.563283 markline-0.3.1/LICENSE.md
+-rw-r--r--   0        0        0     1458 2023-08-05 02:55:58.563283 markline-0.3.1/README.md
+-rw-r--r--   0        0        0    27909 2023-08-05 02:55:58.567283 markline-0.3.1/markline/__init__.py
+-rw-r--r--   0        0        0      604 2023-08-05 02:55:58.567283 markline-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 markline-0.3.1/PKG-INFO
```

### Comparing `markline-0.3.0/LICENSE.md` & `markline-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `markline-0.3.0/README.md` & `markline-0.3.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# <img src="img/markline.svg" width="200">
+# <img src="https://raw.githubusercontent.com/hughcameron/markline/main/img/markline.svg" width="200">
 
 **Markline** converts HTML to Markdown and supports transformation methods borrowed from data engineering concepts. The goal of this project is to provide a simple API that renders HTML to Markdown for note management applications such as [Logseq](https://logseq.com).
 
 
 ## Getting Started
 
 ### Installation
```

### Comparing `markline-0.3.0/markline/__init__.py` & `markline-0.3.1/markline/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -587,14 +587,15 @@
                 If provided, a value is returned from each element. Defaults to None.
             get_text (bool, optional): Whether to return the text of each element. Defaults to False.
             version (str, optional): Version of the HTML content to select from. Defaults to "draft".
         Returns:
             element.ResultSet: ResultSet of elements from query.
         """
         markup = getattr(self, version)
+        results = []
         if isinstance(loc, TagLocator):
             results = markup.find_all(*loc)
         if isinstance(loc, CSSLocator):
             results = markup.select(*loc)
         if isinstance(loc, str):
             loc = CSSLocator(loc)
             results = markup.select(*loc)
@@ -659,14 +660,16 @@
         While the filter() method is used to remove non-matching elements,
         the drop() method is used to remove matching elements from the draft.
 
         Args:
             loc (CSSLocator | TagLocator | str): One or more locators of matching elements to drop.
         """
         for loc in locations:
+            if isinstance(loc, list):
+                self.drop(*loc)
             for result in self.select_all(loc):
                 result.decompose()
         return self
 
     def prepend(self, *elements: element.Tag) -> None:
         """Prepend HTML elements to the draft.
 
@@ -740,15 +743,15 @@
 
         Returns:
             str: Pandoc formatted output.
         """
         return pypandoc.convert_text(
             source=self.draft.prettify(),
             format=input_format,
-            to="md",
+            to=output_format,
             extra_args=output_options,
         )
 
     def to_html(self, filepath: str = None) -> str:
         """Render the draft as HTML.
         If a filepath is provided, the HTML content is written to the file.
```

### Comparing `markline-0.3.0/pyproject.toml` & `markline-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "markline"
-version = "0.3.0"
+version = "0.3.1"
 description = "Convert Markup to Markdown with a transformation pipeline."
 authors = ["Hugh Cameron <hescameron+githubprojects@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/hughcameron/markline"
 repository = "https://github.com/hughcameron/markline"
 readme = "README.md"
```

### Comparing `markline-0.3.0/PKG-INFO` & `markline-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markline
-Version: 0.3.0
+Version: 0.3.1
 Summary: Convert Markup to Markdown with a transformation pipeline.
 Home-page: https://github.com/hughcameron/markline
 License: MIT
 Author: Hugh Cameron
 Author-email: hescameron+githubprojects@gmail.com
 Requires-Python: >=3.10.6,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: furl (>=2.1.3,<3.0.0)
 Requires-Dist: httpx (>=0.24.1,<0.25.0)
 Requires-Dist: pypandoc (>=1.11,<2.0)
 Project-URL: Repository, https://github.com/hughcameron/markline
 Description-Content-Type: text/markdown
 
-# <img src="img/markline.svg" width="200">
+# <img src="https://raw.githubusercontent.com/hughcameron/markline/main/img/markline.svg" width="200">
 
 **Markline** converts HTML to Markdown and supports transformation methods borrowed from data engineering concepts. The goal of this project is to provide a simple API that renders HTML to Markdown for note management applications such as [Logseq](https://logseq.com).
 
 
 ## Getting Started
 
 ### Installation
```

