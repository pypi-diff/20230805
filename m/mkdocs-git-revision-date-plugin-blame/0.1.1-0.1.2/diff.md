# Comparing `tmp/mkdocs-git-revision-date-plugin-blame-0.1.1.tar.gz` & `tmp/mkdocs-git-revision-date-plugin-blame-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.1.tar", last modified: Sat Jul 29 19:10:03 2023, max compression
+gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.2.tar", last modified: Sat Aug  5 18:31:13 2023, max compression
```

## Comparing `mkdocs-git-revision-date-plugin-blame-0.1.1.tar` & `mkdocs-git-revision-date-plugin-blame-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-07-29 19:10:03.765664 mkdocs-git-revision-date-plugin-blame-0.1.1/
--rw-rw-rw-   0        0        0      378 2023-07-29 19:10:03.764663 mkdocs-git-revision-date-plugin-blame-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-29 19:10:03.746581 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/
--rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/__init__.py
--rw-rw-rw-   0        0        0      605 2023-07-29 18:27:49.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/gitTest.py
--rw-rw-rw-   0        0        0     2535 2023-07-29 19:01:44.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/plugin.py
--rw-rw-rw-   0        0        0      310 2023-07-29 18:58:17.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/util.py
-drwxrwxrwx   0        0        0        0 2023-07-29 19:10:03.763662 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/
--rw-rw-rw-   0        0        0      378 2023-07-29 19:10:03.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-07-29 19:10:03.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-29 19:10:03.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      115 2023-07-29 19:10:03.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-07-29 19:10:03.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-07-29 19:10:03.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-29 19:10:03.766663 mkdocs-git-revision-date-plugin-blame-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      827 2023-07-29 19:05:38.000000 mkdocs-git-revision-date-plugin-blame-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:31:13.010343 mkdocs-git-revision-date-plugin-blame-0.1.2/
+-rw-rw-rw-   0        0        0      378 2023-08-05 18:31:13.008331 mkdocs-git-revision-date-plugin-blame-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 18:31:12.960331 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/
+-rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/__init__.py
+-rw-rw-rw-   0        0        0      605 2023-07-29 18:27:49.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/gitTest.py
+-rw-rw-rw-   0        0        0     2535 2023-07-29 19:01:44.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/plugin.py
+-rw-rw-rw-   0        0        0      310 2023-07-29 18:58:17.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/util.py
+drwxrwxrwx   0        0        0        0 2023-08-05 18:31:13.005807 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 18:31:13.011345 mkdocs-git-revision-date-plugin-blame-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-08-05 18:25:42.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/setup.py
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.1/README.md` & `mkdocs-git-revision-date-plugin-blame-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/gitTest.py` & `mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/gitTest.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin/plugin.py` & `mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.1/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt` & `mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.1/setup.py` & `mkdocs-git-revision-date-plugin-blame-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-git-revision-date-plugin-blame',
-    version='0.1.1',
+    version='0.1.2',
     description='MkDocs plugin for setting revision date from git per markdown file using blame.',
     keywords='mkdocs git meta yaml frontmatter',
     url='https://github.com/codyprupp/mkdocs-git-revision-date-plugin',
     author='Cody Rupp',
     author_email='crupp@ucsd.edu',
     license='MIT',
     license_files = ('LICENSE'),
@@ -15,11 +15,11 @@
         'mkdocs>=0.17',
         'GitPython',
         'jinja2'
     ],
     packages=["mkdocs_git_revision_date_plugin"],
     entry_points={
         'mkdocs.plugins': [
-            'git-revision-date-blame = mkdocs_git_revision_date_plugin_blame.plugin:GitRevisionDateBlamePlugin'
+            'git-revision-date-blame = mkdocs_git_revision_date_plugin.plugin:GitRevisionDatePlugin'
         ]
     }
 )
```

