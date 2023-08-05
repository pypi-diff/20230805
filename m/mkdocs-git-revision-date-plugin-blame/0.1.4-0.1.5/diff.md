# Comparing `tmp/mkdocs-git-revision-date-plugin-blame-0.1.4.tar.gz` & `tmp/mkdocs-git-revision-date-plugin-blame-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.4.tar", last modified: Sat Aug  5 20:24:15 2023, max compression
+gzip compressed data, was "mkdocs-git-revision-date-plugin-blame-0.1.5.tar", last modified: Sat Aug  5 20:28:09 2023, max compression
```

## Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4.tar` & `mkdocs-git-revision-date-plugin-blame-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 20:24:15.292973 mkdocs-git-revision-date-plugin-blame-0.1.4/
--rw-rw-rw-   0        0        0      378 2023-08-05 20:24:15.290965 mkdocs-git-revision-date-plugin-blame-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 20:24:15.263641 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/
--rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/__init__.py
--rw-rw-rw-   0        0        0     1569 2023-08-05 20:22:51.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/gitTest.py
--rw-rw-rw-   0        0        0     2648 2023-08-05 19:00:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/plugin.py
--rw-rw-rw-   0        0        0     2153 2023-08-05 20:23:07.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/util.py
-drwxrwxrwx   0        0        0        0 2023-08-05 20:24:15.289859 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/
--rw-rw-rw-   0        0        0      378 2023-08-05 20:24:15.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      555 2023-08-05 20:24:15.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 20:24:15.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      104 2023-08-05 20:24:15.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       30 2023-08-05 20:24:15.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
--rw-rw-rw-   0        0        0       32 2023-08-05 20:24:15.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-05 20:24:15.292973 mkdocs-git-revision-date-plugin-blame-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0      816 2023-08-05 20:23:22.000000 mkdocs-git-revision-date-plugin-blame-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 20:28:09.153925 mkdocs-git-revision-date-plugin-blame-0.1.5/
+-rw-rw-rw-   0        0        0      378 2023-08-05 20:28:09.152912 mkdocs-git-revision-date-plugin-blame-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     2603 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 20:28:09.137910 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/
+-rw-rw-rw-   0        0        0        0 2023-07-08 18:59:25.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/__init__.py
+-rw-rw-rw-   0        0        0     1569 2023-08-05 20:22:51.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/gitTest.py
+-rw-rw-rw-   0        0        0     2648 2023-08-05 19:00:47.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/plugin.py
+-rw-rw-rw-   0        0        0     2155 2023-08-05 20:25:43.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/util.py
+drwxrwxrwx   0        0        0        0 2023-08-05 20:28:09.150923 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/
+-rw-rw-rw-   0        0        0      378 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      555 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      104 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       30 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       32 2023-08-05 20:28:09.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-05 20:28:09.153925 mkdocs-git-revision-date-plugin-blame-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      816 2023-08-05 20:26:44.000000 mkdocs-git-revision-date-plugin-blame-0.1.5/setup.py
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4/README.md` & `mkdocs-git-revision-date-plugin-blame-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/gitTest.py` & `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/gitTest.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/plugin.py` & `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin/util.py` & `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin/util.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     # NOTE: this implies that a file is "up to date" if the most recent git commit displays a somewhat recent date.
     #   This is not entirely accurate, unless whoever made that commit checked the entire file for discrepancies, which is not always the case.
     #   To fix this, either display a verbose output with every single line of blame, or figure out a way to display the blame for a specific
     #       while hovering over the corresponding text.
     def get_revision_date_for_file(self, path: str):
 
         # get the raw blame for the file
-        repo = git.repo.Repo(os.getcwd)
+        repo = git.repo.Repo(os.getcwd())
         blameIter = repo.blame_incremental(repo.head, path)
 
         blameTimes = []
 
         # extract each blame's date in the form YYYY-MM-DD
         for blame in blameIter:
             rawEpochTime = blame.commit.authored_date # type: ignore (not sure why this gives an error; it works fine)
```

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt` & `mkdocs-git-revision-date-plugin-blame-0.1.5/mkdocs_git_revision_date_plugin_blame.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mkdocs-git-revision-date-plugin-blame-0.1.4/setup.py` & `mkdocs-git-revision-date-plugin-blame-0.1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mkdocs-git-revision-date-plugin-blame',
-    version='0.1.4',
+    version='0.1.5',
     description='MkDocs plugin for setting revision date from git per markdown file using blame.',
     keywords='mkdocs git meta yaml frontmatter',
     url='https://github.com/codyprupp/mkdocs-git-revision-date-plugin',
     author='Cody Rupp',
     author_email='crupp@ucsd.edu',
     license='MIT',
     license_files = ('LICENSE'),
```

