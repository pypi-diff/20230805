# Comparing `tmp/mkdocs-tech-docs-template-0.1.1.tar.gz` & `tmp/mkdocs-tech-docs-template-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-tech-docs-template-0.1.1.tar", last modified: Wed Jul 26 13:06:36 2023, max compression
+gzip compressed data, was "mkdocs-tech-docs-template-0.1.2.tar", last modified: Sat Aug  5 14:04:58 2023, max compression
```

## Comparing `mkdocs-tech-docs-template-0.1.1.tar` & `mkdocs-tech-docs-template-0.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.411674 mkdocs-tech-docs-template-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/docs/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-26 13:06:36.000000 mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.411674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/govuk-crest-2x.png
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/ogl.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/
--rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/dbt.ico
--rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/moj.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-26 13:06:36.415674 mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/
--rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/dbt.png
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/moj.png
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/main.html
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-26 13:06:19.000000 mkdocs-tech-docs-template-0.1.1/tech_docs_template/mkdocs_theme.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.252209 mkdocs-tech-docs-template-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/docs/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.252209 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-08-05 14:04:58.000000 mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/tech_docs_template/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.248209 mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     8884 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/images/govuk-crest-2x.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/images/ogl.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)     4237 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/tech_docs_template/favicons/
+-rw-r--r--   0 runner    (1001) docker     (123)     9662 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/favicons/dbt.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    15086 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/favicons/moj.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 14:04:58.256209 mkdocs-tech-docs-template-0.1.2/tech_docs_template/logos/
+-rw-r--r--   0 runner    (1001) docker     (123)    12764 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/logos/dbt.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/logos/moj.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-05 14:04:42.000000 mkdocs-tech-docs-template-0.1.2/tech_docs_template/mkdocs_theme.yml
```

### Comparing `mkdocs-tech-docs-template-0.1.1/PKG-INFO` & `mkdocs-tech-docs-template-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-tech-docs-template
-Version: 0.1.1
+Version: 0.1.2
 Summary: MkDocs theme that you can use to build technical documentation with a GOV.UK
 Home-page: https://github.com/ministryofjustice/mkdocs-tech-docs-template
 Author: Soumaya Mauthoor
 Author-email: soumaya.mauthoor@justice.gov.uk
 License: MIT
 Keywords: mkdocs,technical,documentation
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-tech-docs-template Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: mkdocs-tech-docs-template Version: 0.1.2 Summary:
 MkDocs theme that you can use to build technical documentation with a GOV.UK
 Home-page: https://github.com/ministryofjustice/mkdocs-tech-docs-template
 Author: Soumaya Mauthoor Author-email: soumaya.mauthoor@justice.gov.uk License:
 MIT Keywords: mkdocs,technical,documentation Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 Provides-Extra: docs --- title: MkDocs Tech Docs Template hide: - navigation -
```

### Comparing `mkdocs-tech-docs-template-0.1.1/docs/README.md` & `mkdocs-tech-docs-template-0.1.2/docs/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/PKG-INFO` & `mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-tech-docs-template
-Version: 0.1.1
+Version: 0.1.2
 Summary: MkDocs theme that you can use to build technical documentation with a GOV.UK
 Home-page: https://github.com/ministryofjustice/mkdocs-tech-docs-template
 Author: Soumaya Mauthoor
 Author-email: soumaya.mauthoor@justice.gov.uk
 License: MIT
 Keywords: mkdocs,technical,documentation
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mkdocs-tech-docs-template Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: mkdocs-tech-docs-template Version: 0.1.2 Summary:
 MkDocs theme that you can use to build technical documentation with a GOV.UK
 Home-page: https://github.com/ministryofjustice/mkdocs-tech-docs-template
 Author: Soumaya Mauthoor Author-email: soumaya.mauthoor@justice.gov.uk License:
 MIT Keywords: mkdocs,technical,documentation Classifier: Programming Language
 :: Python :: 3 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 Provides-Extra: docs --- title: MkDocs Tech Docs Template hide: - navigation -
```

### Comparing `mkdocs-tech-docs-template-0.1.1/mkdocs_tech_docs_template.egg-info/SOURCES.txt` & `mkdocs-tech-docs-template-0.1.2/mkdocs_tech_docs_template.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/setup.cfg` & `mkdocs-tech-docs-template-0.1.2/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 	Operating System :: OS Independent
 
 [options]
 packages = find:
 include_package_data = True
 zip_safe = False
 install_requires = 
-	mkdocs-material >= 9.2
+	mkdocs-material >= 9.2.0b1
 
 [options.entry_points]
 mkdocs.themes = 
 	tech_docs_template = tech_docs_template
 
 [options.extras_require]
 docs =
```

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/govuk-crest-2x.png` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/images/govuk-crest-2x.png`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/images/ogl.png` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/images/ogl.png`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/assets/stylesheets/extra.css` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/assets/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/dbt.ico` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/favicons/dbt.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/favicons/moj.ico` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/favicons/moj.ico`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/dbt.png` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/logos/dbt.png`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/logos/moj.png` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/logos/moj.png`

 * *Files identical despite different names*

### Comparing `mkdocs-tech-docs-template-0.1.1/tech_docs_template/main.html` & `mkdocs-tech-docs-template-0.1.2/tech_docs_template/main.html`

 * *Files identical despite different names*

