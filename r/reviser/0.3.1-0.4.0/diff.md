# Comparing `tmp/reviser-0.3.1.tar.gz` & `tmp/reviser-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reviser-0.3.1.tar", max compression
+gzip compressed data, was "reviser-0.4.0.tar", max compression
```

## Comparing `reviser-0.3.1.tar` & `reviser-0.4.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0     1078 2023-07-20 16:48:02.382369 reviser-0.3.1/LICENSE
--rw-r--r--   0        0        0    40957 2023-07-20 16:48:33.101843 reviser-0.3.1/README.md
--rw-r--r--   0        0        0     2646 2023-07-20 16:48:02.382369 reviser-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      837 2023-07-20 16:48:02.382369 reviser-0.3.1/reviser/__init__.py
--rw-r--r--   0        0        0     4779 2023-07-20 16:48:02.382369 reviser-0.3.1/reviser/bundling/__init__.py
--rw-r--r--   0        0        0     4627 2023-07-20 16:48:02.382369 reviser-0.3.1/reviser/bundling/_installer.py
--rw-r--r--   0        0        0     2854 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/cli.py
--rw-r--r--   0        0        0     1554 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/__init__.py
--rw-r--r--   0        0        0     4766 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/aliaser.py
--rw-r--r--   0        0        0     2391 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/bundler.py
--rw-r--r--   0        0        0      850 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/configer.py
--rw-r--r--   0        0        0     2008 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/deployer.py
--rw-r--r--   0        0        0      636 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/exiter.py
--rw-r--r--   0        0        0     1799 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/helper/__init__.py
--rw-r--r--   0        0        0      198 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/helper/help.jinja2
--rw-r--r--   0        0        0     5192 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/invoker.py
--rw-r--r--   0        0        0     1267 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/lister.py
--rw-r--r--   0        0        0     8355 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/pruner.py
--rw-r--r--   0        0        0      875 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/pusher.py
--rw-r--r--   0        0        0     2470 2023-07-20 16:48:02.383369 reviser-0.3.1/reviser/commands/region_switcher.py
--rw-r--r--   0        0        0     2542 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/reloader.py
--rw-r--r--   0        0        0     4697 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/reporter.py
--rw-r--r--   0        0        0     5377 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/selector.py
--rw-r--r--   0        0        0     1360 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/sheller.py
--rw-r--r--   0        0        0     5008 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/commands/tailer.py
--rw-r--r--   0        0        0     1249 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/__init__.py
--rw-r--r--   0        0        0     4398 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/abstracts.py
--rw-r--r--   0        0        0     2247 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/aws.py
--rw-r--r--   0        0        0     3698 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/__init__.py
--rw-r--r--   0        0        0     9766 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/bundling.py
--rw-r--r--   0        0        0     9624 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/depending.py
--rw-r--r--   0        0        0     3988 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/enviromentals.py
--rw-r--r--   0        0        0     2261 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/imaging.py
--rw-r--r--   0        0        0     3052 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/layering.py
--rw-r--r--   0        0        0     9875 2023-07-20 16:48:02.384369 reviser-0.3.1/reviser/definitions/configurations/targeting.py
--rw-r--r--   0        0        0     3414 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/contexts.py
--rw-r--r--   0        0        0     1126 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/enumerations.py
--rw-r--r--   0        0        0     9689 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/infomatics.py
--rw-r--r--   0        0        0      569 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/definitions/selections.py
--rw-r--r--   0        0        0     2953 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/__init__.py
--rw-r--r--   0        0        0     6390 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/publisher.py
--rw-r--r--   0        0        0     6558 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/updater.py
--rw-r--r--   0        0        0     2382 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/deploying/uploader.py
--rw-r--r--   0        0        0      508 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/__init__.py
--rw-r--r--   0        0        0     4152 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/completions.py
--rw-r--r--   0        0        0     1591 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/runner.py
--rw-r--r--   0        0        0     9638 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/__init__.py
--rw-r--r--   0        0        0      293 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/execution_result.jinja2
--rw-r--r--   0        0        0      514 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/prompt.jinja2
--rw-r--r--   0        0        0      277 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/interactivity/shells/splash.jinja2
--rw-r--r--   0        0        0     4468 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/parsing.py
--rw-r--r--   0        0        0      553 2023-07-20 16:48:02.385369 reviser-0.3.1/reviser/servicer/__init__.py
--rw-r--r--   0        0        0     3403 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/servicer/functioning/__init__.py
--rw-r--r--   0        0        0      334 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/servicer/functioning/echo_versions.jinja2
--rw-r--r--   0        0        0     4098 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/servicer/layering.py
--rw-r--r--   0        0        0     2394 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/templating/__init__.py
--rw-r--r--   0        0        0      260 2023-07-20 16:48:02.386369 reviser-0.3.1/reviser/templating/error.jinja2
--rw-r--r--   0        0        0     1826 2023-07-20 16:48:02.389369 reviser-0.3.1/reviser/utils.py
--rw-r--r--   0        0        0    42379 1970-01-01 00:00:00.000000 reviser-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-08-05 14:40:19.290544 reviser-0.4.0/LICENSE
+-rw-r--r--   0        0        0    40957 2023-08-05 14:40:50.019194 reviser-0.4.0/README.md
+-rw-r--r--   0        0        0     2646 2023-08-05 14:40:19.291544 reviser-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      837 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/__init__.py
+-rw-r--r--   0        0        0     4779 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/bundling/__init__.py
+-rw-r--r--   0        0        0     4929 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/bundling/_installer.py
+-rw-r--r--   0        0        0     2854 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/cli.py
+-rw-r--r--   0        0        0     1554 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/__init__.py
+-rw-r--r--   0        0        0     4766 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/aliaser.py
+-rw-r--r--   0        0        0     2391 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/bundler.py
+-rw-r--r--   0        0        0      850 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/configer.py
+-rw-r--r--   0        0        0     2008 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/deployer.py
+-rw-r--r--   0        0        0      636 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/exiter.py
+-rw-r--r--   0        0        0     1799 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/helper/__init__.py
+-rw-r--r--   0        0        0      198 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/helper/help.jinja2
+-rw-r--r--   0        0        0     5192 2023-08-05 14:40:19.291544 reviser-0.4.0/reviser/commands/invoker.py
+-rw-r--r--   0        0        0     1267 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/lister.py
+-rw-r--r--   0        0        0     8355 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/pruner.py
+-rw-r--r--   0        0        0      875 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/pusher.py
+-rw-r--r--   0        0        0     2470 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/region_switcher.py
+-rw-r--r--   0        0        0     2542 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/reloader.py
+-rw-r--r--   0        0        0     4697 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/reporter.py
+-rw-r--r--   0        0        0     5377 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/selector.py
+-rw-r--r--   0        0        0     1360 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/sheller.py
+-rw-r--r--   0        0        0     5008 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/commands/tailer.py
+-rw-r--r--   0        0        0     1249 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/__init__.py
+-rw-r--r--   0        0        0     5854 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/abstracts.py
+-rw-r--r--   0        0        0     2247 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/aws.py
+-rw-r--r--   0        0        0     3698 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/configurations/__init__.py
+-rw-r--r--   0        0        0     9766 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/configurations/bundling.py
+-rw-r--r--   0        0        0     9838 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/configurations/depending.py
+-rw-r--r--   0        0        0     3988 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/configurations/enviromentals.py
+-rw-r--r--   0        0        0     2261 2023-08-05 14:40:19.292544 reviser-0.4.0/reviser/definitions/configurations/imaging.py
+-rw-r--r--   0        0        0     3052 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/definitions/configurations/layering.py
+-rw-r--r--   0        0        0     9875 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/definitions/configurations/targeting.py
+-rw-r--r--   0        0        0     3414 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/definitions/contexts.py
+-rw-r--r--   0        0        0     1126 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/definitions/enumerations.py
+-rw-r--r--   0        0        0     9689 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/definitions/infomatics.py
+-rw-r--r--   0        0        0      569 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/definitions/selections.py
+-rw-r--r--   0        0        0     2953 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/deploying/__init__.py
+-rw-r--r--   0        0        0     6390 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/deploying/publisher.py
+-rw-r--r--   0        0        0     6558 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/deploying/updater.py
+-rw-r--r--   0        0        0     2382 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/deploying/uploader.py
+-rw-r--r--   0        0        0      508 2023-08-05 14:40:19.293544 reviser-0.4.0/reviser/interactivity/__init__.py
+-rw-r--r--   0        0        0     4152 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/interactivity/completions.py
+-rw-r--r--   0        0        0     1591 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/interactivity/runner.py
+-rw-r--r--   0        0        0     9638 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/interactivity/shells/__init__.py
+-rw-r--r--   0        0        0      293 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/interactivity/shells/execution_result.jinja2
+-rw-r--r--   0        0        0      514 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/interactivity/shells/prompt.jinja2
+-rw-r--r--   0        0        0      277 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/interactivity/shells/splash.jinja2
+-rw-r--r--   0        0        0     4468 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/parsing.py
+-rw-r--r--   0        0        0      553 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/servicer/__init__.py
+-rw-r--r--   0        0        0     3403 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/servicer/functioning/__init__.py
+-rw-r--r--   0        0        0      334 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/servicer/functioning/echo_versions.jinja2
+-rw-r--r--   0        0        0     4098 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/servicer/layering.py
+-rw-r--r--   0        0        0     2394 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/templating/__init__.py
+-rw-r--r--   0        0        0      260 2023-08-05 14:40:19.294544 reviser-0.4.0/reviser/templating/error.jinja2
+-rw-r--r--   0        0        0     1826 2023-08-05 14:40:19.298544 reviser-0.4.0/reviser/utils.py
+-rw-r--r--   0        0        0    42379 1970-01-01 00:00:00.000000 reviser-0.4.0/PKG-INFO
```

### Comparing `reviser-0.3.1/LICENSE` & `reviser-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/README.md` & `reviser-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/pyproject.toml` & `reviser-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "reviser"
-version = "0.3.1"
+version = "0.4.0"
 description = "AWS Lambda function/layer version deployment manager."
 authors = [
   "Scott Ernst <swernst@gmail.com>",
   "Kevin Schiroo",
   "Rigo Silva"
 ]
 license = "MIT"
```

### Comparing `reviser-0.3.1/reviser/__init__.py` & `reviser-0.4.0/reviser/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/bundling/__init__.py` & `reviser-0.4.0/reviser/bundling/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/bundling/_installer.py` & `reviser-0.4.0/reviser/bundling/_installer.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,25 +5,30 @@
 import shutil
 import subprocess
 import typing
 
 from reviser import definitions
 
 
-def _install_pip_package(name: str, site_packages: pathlib.Path):
+def _install_pip_package(
+    name: str,
+    site_packages: pathlib.Path,
+    arguments: typing.Optional[typing.List[str]] = None,
+):
     """Install the specified pip package."""
     cmd = [
         "python",
         "-m",
         "pip",
         "install",
         "--upgrade",
         name,
         "-t",
         f'"{site_packages}"',
+        *(arguments or []),
     ]
     print(" ".join(cmd).replace(" -", "\n  -"))
     os.system(" ".join(cmd))
 
 
 def _install_pipper_package(
     name: str,
@@ -43,30 +48,30 @@
     ]
     print(" ".join(cmd).replace(" -", "\n  -"))
     subprocess.run(cmd, env=env, check=True)
 
 
 def _install_poetry(dependency: "definitions.PoetryDependency"):
     """Install poetry dependencies in the target's site packages."""
+    arguments = [f"{k}={v}" for k, v in dependency.arguments.items() if v is not None]
     for package in dependency.get_package_names() or []:
         print(f'\n[INSTALLING]: "{package}" poetry package')
         _install_pip_package(
-            package,
-            dependency.group.site_packages_directory,
+            package, dependency.group.site_packages_directory, arguments
         )
         print(f'\n[INSTALLED]: "{package}" poetry package')
 
 
 def _install_pip(dependency: "definitions.PipDependency"):
     """Install poetry dependencies in the target's site packages."""
+    arguments = [f"{k}={v}" for k, v in dependency.arguments.items() if v is not None]
     for package in dependency.get_package_names() or []:
         print(f'\n[INSTALLING]: "{package}" pip package')
         _install_pip_package(
-            package,
-            dependency.group.site_packages_directory,
+            package, dependency.group.site_packages_directory, arguments
         )
         print(f'\n[INSTALLED]: "{package}" pip package')
 
 
 def _install_pipper(dependency: "definitions.PipperDependency"):
     """
     Install any pipper dependencies alongside the standard pip site packages.
@@ -80,24 +85,26 @@
         "PIPPER_AWS_SESSION_TOKEN": credentials.token,
     }
     env = copy.copy(os.environ)
     # Depending on what type os session source is used, one or more of
     # these will be None and None values cannot be included in environment
     # variables without raising a TypeError: str expected, not NoneType.
     env.update({k: v for k, v in env_vars.items() if v is not None})
+    additional_kwargs = {
+        "--bucket": dependency.bucket,
+        "--prefix": dependency.prefix,
+    }
+    arguments = [
+        f"{k}={v}"
+        for k, v in {**additional_kwargs, **dependency.arguments}.items()
+        if v is not None
+    ]
 
     for package in dependency.get_package_names():
-        additional_kwargs = {
-            "--bucket": dependency.bucket,
-            "--prefix": dependency.prefix,
-        }
-        arguments = [f"{k}={v}" for k, v in additional_kwargs.items() if v is not None]
-
         print(f'\n[INSTALLING]: "{package}" pipper package')
-
         _install_pipper_package(
             package,
             dependency.group.site_packages_directory,
             typing.cast(dict, env),
             arguments,
         )
         print(f'\n[INSTALLED]: "{package}" pipper package')
```

### Comparing `reviser-0.3.1/reviser/cli.py` & `reviser-0.4.0/reviser/cli.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/__init__.py` & `reviser-0.4.0/reviser/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/aliaser.py` & `reviser-0.4.0/reviser/commands/aliaser.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/bundler.py` & `reviser-0.4.0/reviser/commands/bundler.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/configer.py` & `reviser-0.4.0/reviser/commands/configer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/deployer.py` & `reviser-0.4.0/reviser/commands/deployer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/exiter.py` & `reviser-0.4.0/reviser/commands/exiter.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/helper/__init__.py` & `reviser-0.4.0/reviser/commands/helper/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/invoker.py` & `reviser-0.4.0/reviser/commands/invoker.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/lister.py` & `reviser-0.4.0/reviser/commands/lister.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/pruner.py` & `reviser-0.4.0/reviser/commands/pruner.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/pusher.py` & `reviser-0.4.0/reviser/commands/pusher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/region_switcher.py` & `reviser-0.4.0/reviser/commands/region_switcher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/reloader.py` & `reviser-0.4.0/reviser/commands/reloader.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/reporter.py` & `reviser-0.4.0/reviser/commands/reporter.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/selector.py` & `reviser-0.4.0/reviser/commands/selector.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/sheller.py` & `reviser-0.4.0/reviser/commands/sheller.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/commands/tailer.py` & `reviser-0.4.0/reviser/commands/tailer.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/__init__.py` & `reviser-0.4.0/reviser/definitions/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/abstracts.py` & `reviser-0.4.0/reviser/definitions/abstracts.py`

 * *Files 16% similar despite different names*

```diff
@@ -79,14 +79,56 @@
         as a list in the same fashion as the get_as_list function.
         """
         found_args = next((a for a in args if self.has(*a)), None)
         if found_args is None:
             return default
         return self.get_as_list(*found_args, default=default)
 
+    def get_as_dict(
+        self,
+        *args: str,
+        default: typing.Any = None,
+    ) -> typing.Dict[typing.Any, typing.Any]:
+        """
+        Fetch the value from the data dictionary as a dict.
+
+        None values will be returned as an empty dict. Values that are
+        not dicts will raise an error. If the nested key does not exist,
+        the default will be returned instead, but if the key is explicitly defined as
+        `null` an empty dict is returned instead fo the default.
+        """
+        if self.has(*args):
+            value = self.get(*args, default=default)
+        else:
+            value = default
+
+        if value is None:
+            return {}
+
+        if not isinstance(value, dict):
+            raise ValueError(f"{value} must bve of type dict")
+        return value
+
+    def get_first_as_dict(
+        self,
+        *args: typing.Iterable[str],
+        default: typing.Any = None,
+    ) -> typing.Any:
+        """
+        Fetch the value from the data dictionary in the key-grouped order.
+
+        The default value will be returned if none of the key-group args
+        exist in the data dictionary. If a match is found it will be returned
+        as a dict in the same fashion as the get_as_dict function.
+        """
+        found_args = next((a for a in args if self.has(*a)), None)
+        if found_args is None:
+            return default
+        return self.get_as_dict(*found_args, default=default)
+
     def has(self, *args: str) -> bool:
         """Determine whether or not the nested key exists."""
         value = self.data or {}
         for k in args:
             if k not in value:
                 return False
             value = value[k]
```

### Comparing `reviser-0.3.1/reviser/definitions/aws.py` & `reviser-0.4.0/reviser/definitions/aws.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/configurations/__init__.py` & `reviser-0.4.0/reviser/definitions/configurations/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/configurations/bundling.py` & `reviser-0.4.0/reviser/definitions/configurations/bundling.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/configurations/depending.py` & `reviser-0.4.0/reviser/definitions/configurations/depending.py`

 * *Files 5% similar despite different names*

```diff
@@ -141,14 +141,19 @@
         return self.get_first_as_list(["packages"], ["package"], default=[])
 
     @property
     def skip_packages(self) -> typing.List[str]:
         """Get packages that should be skipped during the installation process."""
         return self.get_first_as_list(["skips"], ["skip"], default=[])
 
+    @property
+    def arguments(self) -> typing.Dict[str, str]:
+        """Gets arguments that should be passed during the installation process."""
+        return self.get_first_as_dict(["arguments"], default={})
+
     def get_package_names(self) -> typing.List[str]:
         """List package names to install from the various package sources."""
         return []
 
 
 @dataclasses.dataclass(frozen=True)
 class PipDependency(Dependency):
```

### Comparing `reviser-0.3.1/reviser/definitions/configurations/enviromentals.py` & `reviser-0.4.0/reviser/definitions/configurations/enviromentals.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/configurations/imaging.py` & `reviser-0.4.0/reviser/definitions/configurations/imaging.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/configurations/layering.py` & `reviser-0.4.0/reviser/definitions/configurations/layering.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/configurations/targeting.py` & `reviser-0.4.0/reviser/definitions/configurations/targeting.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/contexts.py` & `reviser-0.4.0/reviser/definitions/contexts.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/enumerations.py` & `reviser-0.4.0/reviser/definitions/enumerations.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/infomatics.py` & `reviser-0.4.0/reviser/definitions/infomatics.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/definitions/selections.py` & `reviser-0.4.0/reviser/definitions/selections.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/deploying/__init__.py` & `reviser-0.4.0/reviser/deploying/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/deploying/publisher.py` & `reviser-0.4.0/reviser/deploying/publisher.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/deploying/updater.py` & `reviser-0.4.0/reviser/deploying/updater.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/deploying/uploader.py` & `reviser-0.4.0/reviser/deploying/uploader.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/interactivity/completions.py` & `reviser-0.4.0/reviser/interactivity/completions.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/interactivity/runner.py` & `reviser-0.4.0/reviser/interactivity/runner.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/interactivity/shells/__init__.py` & `reviser-0.4.0/reviser/interactivity/shells/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/interactivity/shells/prompt.jinja2` & `reviser-0.4.0/reviser/interactivity/shells/prompt.jinja2`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/parsing.py` & `reviser-0.4.0/reviser/parsing.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/servicer/__init__.py` & `reviser-0.4.0/reviser/servicer/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/servicer/functioning/__init__.py` & `reviser-0.4.0/reviser/servicer/functioning/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/servicer/layering.py` & `reviser-0.4.0/reviser/servicer/layering.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/templating/__init__.py` & `reviser-0.4.0/reviser/templating/__init__.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/reviser/utils.py` & `reviser-0.4.0/reviser/utils.py`

 * *Files identical despite different names*

### Comparing `reviser-0.3.1/PKG-INFO` & `reviser-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reviser
-Version: 0.3.1
+Version: 0.4.0
 Summary: AWS Lambda function/layer version deployment manager.
 Home-page: https://gitlab.com/rocket-boosters/reviser
 License: MIT
 Keywords: aws,lambda
 Author: Scott Ernst
 Author-email: swernst@gmail.com
 Requires-Python: >=3.8.0,<3.12.0
```

