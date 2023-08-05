# Comparing `tmp/mkdocs-git-revision-date-plugin-blame-0.1.2.tar.gz` & `tmp/mkdocs-git-revision-date-plugin-blame-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.2.tar", last modified: Sat Aug  5 18:31:13 2023, max compression
+gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.3.tar", last modified: Sat Aug  5 20:05:47 2023, max compression
```

## Comparing `mkdocs-git-revision-date-plugin-blame-0.1.2.tar` & `mkdocs-git-revision-date-plugin-blame-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 18:31:13.010343 mkdocs-git-revision-date-plugin-blame-0.1.2/
--rw-rw-rw-   0        0        0      378 2023-08-05 18:31:13.008331 mkdocs-git-revision-date-plugin-blame-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 18:31:12.960331 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/
--rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/__init__.py
--rw-rw-rw-   0        0        0      605 2023-07-29 18:27:49.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/gitTest.py
--rw-rw-rw-   0        0        0     2535 2023-07-29 19:01:44.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/plugin.py
--rw-rw-rw-   0        0        0      310 2023-07-29 18:58:17.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/util.py
-drwxrwxrwx   0        0        0        0 2023-08-05 18:31:13.005807 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/
--rw-rw-rw-   0        0        0      378 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-08-05 18:31:12.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 18:31:13.011345 mkdocs-git-revision-date-plugin-blame-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-08-05 18:25:42.000000 mkdocs-git-revision-date-plugin-blame-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 20:05:47.460117 mkdocs-git-revision-date-plugin-blame-0.1.3/
+-rw-rw-rw-   0        0        0      378 2023-08-05 20:05:47.460117 mkdocs-git-revision-date-plugin-blame-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 20:05:47.444530 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin/
+-rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin/__init__.py
+-rw-rw-rw-   0        0        0     1544 2023-08-05 19:46:19.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin/gitTest.py
+-rw-rw-rw-   0        0        0     2648 2023-08-05 19:00:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin/plugin.py
+-rw-rw-rw-   0        0        0     2024 2023-08-05 20:02:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin/util.py
+drwxrwxrwx   0        0        0        0 2023-08-05 20:05:47.460117 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-08-05 20:05:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-08-05 20:05:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 20:05:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-08-05 20:05:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-08-05 20:05:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-08-05 20:05:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 20:05:47.460117 mkdocs-git-revision-date-plugin-blame-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-08-05 20:04:04.000000 mkdocs-git-revision-date-plugin-blame-0.1.3/setup.py
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.2/README.md` & `mkdocs-git-revision-date-plugin-blame-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin/plugin.py` & `mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 
     def on_page_markdown(self, markdown, page, config, files):
         if not self.enabled:
             return markdown
 
         revision_date = self.util.get_revision_date_for_file(page.file.abs_src_path)
 
+
+        # TODO: if the file has no git logs, it could be empty. default to date the file was created instead?
         if not revision_date:
             revision_date = datetime.now().date().strftime('%Y-%m-%d')
             print('WARNING -  %s has no git logs, revision date defaulting to today\'s date' % page.file.src_path)
 
         if self.config['as_datetime']:
             revision_date = datetime.strptime(revision_date,'%Y-%m-%d')
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.2/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt` & `mkdocs-git-revision-date-plugin-blame-0.1.3/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.2/setup.py` & `mkdocs-git-revision-date-plugin-blame-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-git-revision-date-plugin-blame',
-    version='0.1.2',
+    version='0.1.3',
     description='MkDocs plugin for setting revision date from git per markdown file using blame.',
     keywords='mkdocs git meta yaml frontmatter',
     url='https://github.com/codyprupp/mkdocs-git-revision-date-plugin',
     author='Cody Rupp',
     author_email='crupp@ucsd.edu',
     license='MIT',
     license_files = ('LICENSE'),
```

