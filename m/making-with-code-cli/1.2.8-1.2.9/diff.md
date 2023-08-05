# Comparing `tmp/making_with_code_cli-1.2.8.tar.gz` & `tmp/making_with_code_cli-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "making_with_code_cli-1.2.8.tar", max compression
+gzip compressed data, was "making_with_code_cli-1.2.9.tar", max compression
```

## Comparing `making_with_code_cli-1.2.8.tar` & `making_with_code_cli-1.2.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.8/README.md
--rw-r--r--   0        0        0     8031 2023-07-13 17:44:41.302864 making_with_code_cli-1.2.8/making_with_code_cli/cli.py
--rw-r--r--   0        0        0    16558 2023-07-14 12:45:01.156845 making_with_code_cli-1.2.8/making_with_code_cli/cli_setup.py
--rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.8/making_with_code_cli/curriculum.py
--rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.8/making_with_code_cli/errors.py
--rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/__init__.py
--rw-r--r--   0        0        0     1613 2023-07-02 18:57:59.595603 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/base_backend.py
--rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_backend.py
--rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_org_backend.py
--rw-r--r--   0        0        0     4048 2023-07-11 16:15:54.845783 making_with_code_cli-1.2.8/making_with_code_cli/git_backend/mwc_backend.py
--rw-r--r--   0        0        0      727 2023-07-12 20:28:47.118456 making_with_code_cli-1.2.8/making_with_code_cli/git_wrapper.py
--rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.8/making_with_code_cli/helpers.py
--rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.8/making_with_code_cli/mwc_accounts_api.py
--rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.8/making_with_code_cli/settings.py
--rw-r--r--   0        0        0     1702 2023-07-13 17:41:17.791340 making_with_code_cli-1.2.8/making_with_code_cli/styles.py
--rw-r--r--   0        0        0      663 2023-07-14 12:45:08.415566 making_with_code_cli-1.2.8/pyproject.toml
--rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1342 2023-05-30 14:14:06.604035 making_with_code_cli-1.2.9/README.md
+-rw-r--r--   0        0        0     8031 2023-07-13 17:44:41.302864 making_with_code_cli-1.2.9/making_with_code_cli/cli.py
+-rw-r--r--   0        0        0    16558 2023-07-14 12:45:01.156845 making_with_code_cli-1.2.9/making_with_code_cli/cli_setup.py
+-rw-r--r--   0        0        0      551 2023-07-10 19:39:26.763192 making_with_code_cli-1.2.9/making_with_code_cli/curriculum.py
+-rw-r--r--   0        0        0      658 2023-07-10 20:30:48.777211 making_with_code_cli-1.2.9/making_with_code_cli/errors.py
+-rw-r--r--   0        0        0      276 2023-06-05 20:21:54.165003 making_with_code_cli-1.2.9/making_with_code_cli/git_backend/__init__.py
+-rw-r--r--   0        0        0     1881 2023-07-19 15:26:02.958402 making_with_code_cli-1.2.9/making_with_code_cli/git_backend/base_backend.py
+-rw-r--r--   0        0        0     3461 2023-06-05 20:20:21.178737 making_with_code_cli-1.2.9/making_with_code_cli/git_backend/github_backend.py
+-rw-r--r--   0        0        0     3845 2023-06-05 20:21:08.636148 making_with_code_cli-1.2.9/making_with_code_cli/git_backend/github_org_backend.py
+-rw-r--r--   0        0        0     4020 2023-07-19 15:02:58.543439 making_with_code_cli-1.2.9/making_with_code_cli/git_backend/mwc_backend.py
+-rw-r--r--   0        0        0      727 2023-07-12 20:28:47.118456 making_with_code_cli-1.2.9/making_with_code_cli/git_wrapper.py
+-rw-r--r--   0        0        0      266 2023-05-30 14:14:06.615290 making_with_code_cli-1.2.9/making_with_code_cli/helpers.py
+-rw-r--r--   0        0        0     1526 2023-07-10 20:12:17.374391 making_with_code_cli-1.2.9/making_with_code_cli/mwc_accounts_api.py
+-rw-r--r--   0        0        0     1629 2023-05-30 14:14:06.616770 making_with_code_cli-1.2.9/making_with_code_cli/settings.py
+-rw-r--r--   0        0        0     1702 2023-07-13 17:41:17.791340 making_with_code_cli-1.2.9/making_with_code_cli/styles.py
+-rw-r--r--   0        0        0      663 2023-07-19 15:26:29.584693 making_with_code_cli-1.2.9/pyproject.toml
+-rw-r--r--   0        0        0     2096 1970-01-01 00:00:00.000000 making_with_code_cli-1.2.9/PKG-INFO
```

### Comparing `making_with_code_cli-1.2.8/README.md` & `making_with_code_cli-1.2.9/README.md`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/cli.py` & `making_with_code_cli-1.2.9/making_with_code_cli/cli.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/cli_setup.py` & `making_with_code_cli-1.2.9/making_with_code_cli/cli_setup.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/curriculum.py` & `making_with_code_cli-1.2.9/making_with_code_cli/curriculum.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/errors.py` & `making_with_code_cli-1.2.9/making_with_code_cli/errors.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/base_backend.py` & `making_with_code_cli-1.2.9/making_with_code_cli/git_backend/base_backend.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from pathlib import Path
 from subprocess import run, CalledProcessError
 import click
 from making_with_code_cli.helpers import cd
 from making_with_code_cli.cli_setup import WORK_DIR_PERMISSIONS
 from making_with_code_cli.styles import (
     address,
+    info,
     confirm,
     error,
 )
 
 class GitBackend:
     """Base class interface to backend git server.
     All Making With Code deployments are backed by a git server, but the nature of the
@@ -28,17 +29,21 @@
 
     def update(self, module, modpath):
         if (modpath / ".git").is_dir():
             with cd(modpath):
                 relpath = self.relative_path(modpath)
                 try:
                     click.echo(address(f"Checking {relpath} for updates.", preformatted=True))
-                    run("git pull", shell=True, check=True)
+                    gitresult = run("git pull", shell=True, check=True, capture_output=True,
+                            text=True)
+                    click.echo(info(gitresult.stdout))
                     if Path("pyproject.toml").exists():
-                        run("poetry update", shell=True, check=True)
+                        result = run("poetry install", shell=True, check=True, 
+                                capture_output=True, text=True)
+                        click.echo(info(result.stdout))
                 except CalledProcessError as e:
                     click.echo(error(f"There was a problem updating {relpath}. Ask a teacher."))
                     raise e
 
     def work_dir(self):
         return Path(self.settings['work_dir'])
```

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_backend.py` & `making_with_code_cli-1.2.9/making_with_code_cli/git_backend/github_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/github_org_backend.py` & `making_with_code_cli-1.2.9/making_with_code_cli/git_backend/github_org_backend.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/git_backend/mwc_backend.py` & `making_with_code_cli-1.2.9/making_with_code_cli/git_backend/mwc_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     within scope.
     """
 
     MWC_GIT_PROTOCOL = "https"
     MWC_GIT_SERVER = "git.makingwithcode.org"
 
     def init_module(self, module, modpath):
-        """Creates the named repo from a template, or clones an existing repo. 
+        """Creates the named repo from a template. 
         """
         self.check_settings()
         server, repo_owner, repo_name = self.parse_repo_url(module["repo_url"])
 
         if modpath.exists():
             self.relocate_existing_directory(modpath)
         if not self.user_has_repo(repo_name):
```

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/git_wrapper.py` & `making_with_code_cli-1.2.9/making_with_code_cli/git_wrapper.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/mwc_accounts_api.py` & `making_with_code_cli-1.2.9/making_with_code_cli/mwc_accounts_api.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/settings.py` & `making_with_code_cli-1.2.9/making_with_code_cli/settings.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/making_with_code_cli/styles.py` & `making_with_code_cli-1.2.9/making_with_code_cli/styles.py`

 * *Files identical despite different names*

### Comparing `making_with_code_cli-1.2.8/pyproject.toml` & `making_with_code_cli-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "making-with-code-cli"
-version = "1.2.8"
+version = "1.2.9"
 description = "Courseware for Making With Code"
 authors = ["Chris Proctor <chris@chrisproctor.net>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/cproctor/making-with-code-courseware"
 
 [tool.poetry.dependencies]
```

### Comparing `making_with_code_cli-1.2.8/PKG-INFO` & `making_with_code_cli-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: making-with-code-cli
-Version: 1.2.8
+Version: 1.2.9
 Summary: Courseware for Making With Code
 Home-page: https://github.com/cproctor/making-with-code-courseware
 License: MIT
 Author: Chris Proctor
 Author-email: chris@chrisproctor.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

