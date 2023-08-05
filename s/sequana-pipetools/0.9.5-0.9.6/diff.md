# Comparing `tmp/sequana_pipetools-0.9.5.tar.gz` & `tmp/sequana_pipetools-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_pipetools-0.9.5.tar", last modified: Fri Nov 18 15:58:00 2022, max compression
+gzip compressed data, was "dist/sequana_pipetools-0.9.6.tar", last modified: Mon Nov 21 08:51:11 2022, max compression
```

## Comparing `sequana_pipetools-0.9.5.tar` & `sequana_pipetools-0.9.6.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)      113 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    14538 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11352 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/requirements_dev.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools/
--rw-r--r--   0 runner    (1001) docker     (121)      592 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8008 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/completion.py
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/info.py
--rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/misc.py
--rw-r--r--   0 runner    (1001) docker     (121)    20305 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/options.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      830 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/resources/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/resources/local.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      647 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/resources/slurm.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    27348 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/sequana_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/
--rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4682 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/dot_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    16312 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/file_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    13639 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/module.py
--rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/module_finder.py
--rw-r--r--   0 runner    (1001) docker     (121)    17429 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/pipeline_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6295 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/pipeline_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      581 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     8268 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/sequana_pipetools/snaketools/sequana_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    14538 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/sequana_pipetools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-18 15:58:00.000000 sequana_pipetools-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2469 2022-11-18 15:57:57.000000 sequana_pipetools-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (121)      113 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)    15346 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    12005 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       78 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/requirements_dev.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools/
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8008 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/completion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/errors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1587 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/info.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3119 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/misc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20305 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/options.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      830 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/resources/ext.py
+-rw-r--r--   0 runner    (1001) docker     (121)      202 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/resources/local.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      647 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/resources/slurm.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    27270 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/sequana_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6533 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/
+-rw-r--r--   0 runner    (1001) docker     (121)      397 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4682 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/dot_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16312 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/file_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13639 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/module.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4296 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/module_finder.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17429 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/pipeline_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6295 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/pipeline_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      581 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8268 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/sequana_pipetools/snaketools/sequana_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    15346 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1142 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       82 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/sequana_pipetools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 08:51:11.000000 sequana_pipetools-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2498 2022-11-21 08:51:07.000000 sequana_pipetools-0.9.6/setup.py
```

### Comparing `sequana_pipetools-0.9.5/PKG-INFO` & `sequana_pipetools-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana_pipetools
-Version: 0.9.5
+Version: 0.9.6
 Summary: A set of tools to help building or using Sequana pipelines
 Home-page: https://github.com/sequana/sequana_pipetools
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -80,14 +80,25 @@
             :scale: 40%
         
             **Figure 3** New Sequana framework. The library itself with the core, the
             bioinformatics tools is now independent of the pipelines. Besides, the
             pipetools library provide common tools to all pipelines to help in their
             creation/management. For instance, common parser for options.
         
+        and finally, we dropped the rules/ available in Sequana to build an independent package with a set of Snakemake
+        wrappers: These wrappers available on https://github.com/sequana/sequana-wrappers have also the advantage of being tested through continuous integration.
+        
+        .. figure:: https://raw.githubusercontent.com/sequana/sequana_pipetools/main/doc/wrappers.png
+            :scale: 40%
+        
+            **Figure 3** New Sequana framework 2021. The library itself with the core, the
+            bioinformatics tools is now fully independent of the pipelines. 
+        
+        
+        
         
         
         
         Installation
         ============
         
         from pypi website::
@@ -180,14 +191,16 @@
         
         Changelog
         =========
         
         ========= ======================================================================
         Version   Description
         ========= ======================================================================
+        0.9.6     * hotfix on apptainer to be back compatible if no apptainers section
+                    is found in the config file.
         0.9.5     * replaced singularity word by apptainer (--use-aptainer instead of 
                     --use-singularity)
         0.9.4     * If timeout occurs while singularity is downloaded, catch the error
                     remove truncated file.
         0.9.3     * hotfix missing import when checking sequana version
                   * add config2schema utility function for developers
         0.9.2     * Udate asynchronous downloads to use aiohttp
@@ -264,12 +277,13 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sequana_pipetools-0.9.5/README.rst` & `sequana_pipetools-0.9.6/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,25 @@
     :scale: 40%
 
     **Figure 3** New Sequana framework. The library itself with the core, the
     bioinformatics tools is now independent of the pipelines. Besides, the
     pipetools library provide common tools to all pipelines to help in their
     creation/management. For instance, common parser for options.
 
+and finally, we dropped the rules/ available in Sequana to build an independent package with a set of Snakemake
+wrappers: These wrappers available on https://github.com/sequana/sequana-wrappers have also the advantage of being tested through continuous integration.
+
+.. figure:: https://raw.githubusercontent.com/sequana/sequana_pipetools/main/doc/wrappers.png
+    :scale: 40%
+
+    **Figure 3** New Sequana framework 2021. The library itself with the core, the
+    bioinformatics tools is now fully independent of the pipelines. 
+
+
+
 
 
 
 Installation
 ============
 
 from pypi website::
@@ -170,14 +181,16 @@
 
 Changelog
 =========
 
 ========= ======================================================================
 Version   Description
 ========= ======================================================================
+0.9.6     * hotfix on apptainer to be back compatible if no apptainers section
+            is found in the config file.
 0.9.5     * replaced singularity word by apptainer (--use-aptainer instead of 
             --use-singularity)
 0.9.4     * If timeout occurs while singularity is downloaded, catch the error
             remove truncated file.
 0.9.3     * hotfix missing import when checking sequana version
           * add config2schema utility function for developers
 0.9.2     * Udate asynchronous downloads to use aiohttp
```

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/__init__.py` & `sequana_pipetools-0.9.6/sequana_pipetools/__init__.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/completion.py` & `sequana_pipetools-0.9.6/sequana_pipetools/completion.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/errors.py` & `sequana_pipetools-0.9.6/sequana_pipetools/errors.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/info.py` & `sequana_pipetools-0.9.6/sequana_pipetools/info.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/misc.py` & `sequana_pipetools-0.9.6/sequana_pipetools/misc.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/options.py` & `sequana_pipetools-0.9.6/sequana_pipetools/options.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/resources/ext.py` & `sequana_pipetools-0.9.6/sequana_pipetools/resources/ext.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/resources/slurm.yaml` & `sequana_pipetools-0.9.6/sequana_pipetools/resources/slurm.yaml`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/sequana_manager.py` & `sequana_pipetools-0.9.6/sequana_pipetools/sequana_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,18 +57,16 @@
                 def __init__(self):
                     pass
             from sequana_pipetools import SequanaManager
             o = Options()
             pm = SequanaManager(o, "fastqc")
 
 
-        The working_directory is uesd to copy the pipeline in it.
+        The working_directory is used to copy the pipeline in it.
 
-
-        .. todo:: allows options to be None and fill it with miminum contents
         """
         # the logger must be defined here because from a pipeline, it may not
         # have been defined yet.
         try:
             logger.setLevel(options.level)
         except AttributeError:
             logger.warning("Your pipeline does not have a level option.")
@@ -584,16 +582,16 @@
 
         # for back compatibility, we scan the pipeline looking for container that start with http
         for included_file in included_files:
             suburls = self._get_section_content(Path(self.module.snakefile).parent / included_file, "container:")
             suburls = [x for x in suburls if x.startswith("http")]
             urls.extend(suburls)
 
-        # but more generally, we ish to retrieve the containers URLs from the config file
-        apps = self.config.config.get("apptainers", [])
+        # but more generally, we wish to retrieve the containers URLs from the config file
+        apps = self.config.config.get("apptainers", {})
         urls.extend((x for x in apps.values() if x.strip()))
 
         # make sure there are unique URLs
         urls = set(urls)
 
         # guarantess that output filename to be saved have the same
         # unique ID as those expected by snakemake
```

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/slurm.py` & `sequana_pipetools-0.9.6/sequana_pipetools/slurm.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/dot_parser.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/dot_parser.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/file_factory.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/file_factory.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/module.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/module.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/module_finder.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/module_finder.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/pipeline_manager.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/pipeline_manager.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/pipeline_utils.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/profile.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/profile.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools/snaketools/sequana_config.py` & `sequana_pipetools-0.9.6/sequana_pipetools/snaketools/sequana_config.py`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools.egg-info/PKG-INFO` & `sequana_pipetools-0.9.6/sequana_pipetools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sequana-pipetools
-Version: 0.9.5
+Version: 0.9.6
 Summary: A set of tools to help building or using Sequana pipelines
 Home-page: https://github.com/sequana/sequana_pipetools
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
@@ -80,14 +80,25 @@
             :scale: 40%
         
             **Figure 3** New Sequana framework. The library itself with the core, the
             bioinformatics tools is now independent of the pipelines. Besides, the
             pipetools library provide common tools to all pipelines to help in their
             creation/management. For instance, common parser for options.
         
+        and finally, we dropped the rules/ available in Sequana to build an independent package with a set of Snakemake
+        wrappers: These wrappers available on https://github.com/sequana/sequana-wrappers have also the advantage of being tested through continuous integration.
+        
+        .. figure:: https://raw.githubusercontent.com/sequana/sequana_pipetools/main/doc/wrappers.png
+            :scale: 40%
+        
+            **Figure 3** New Sequana framework 2021. The library itself with the core, the
+            bioinformatics tools is now fully independent of the pipelines. 
+        
+        
+        
         
         
         
         Installation
         ============
         
         from pypi website::
@@ -180,14 +191,16 @@
         
         Changelog
         =========
         
         ========= ======================================================================
         Version   Description
         ========= ======================================================================
+        0.9.6     * hotfix on apptainer to be back compatible if no apptainers section
+                    is found in the config file.
         0.9.5     * replaced singularity word by apptainer (--use-aptainer instead of 
                     --use-singularity)
         0.9.4     * If timeout occurs while singularity is downloaded, catch the error
                     remove truncated file.
         0.9.3     * hotfix missing import when checking sequana version
                   * add config2schema utility function for developers
         0.9.2     * Udate asynchronous downloads to use aiohttp
@@ -264,12 +277,13 @@
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
```

### Comparing `sequana_pipetools-0.9.5/sequana_pipetools.egg-info/SOURCES.txt` & `sequana_pipetools-0.9.6/sequana_pipetools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sequana_pipetools-0.9.5/setup.py` & `sequana_pipetools-0.9.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 
 _MAJOR = 0
 _MINOR = 9
-_MICRO = 5
+_MICRO = 6
 version = f"{_MAJOR}.{_MINOR}.{_MICRO}"
 release = f"{_MAJOR}.{_MINOR}"
 
 metainfo = {
     "authors": {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     "version": version,
     "license": "new BSD",
@@ -21,14 +21,15 @@
         "Intended Audience :: End Users/Desktop",
         "Intended Audience :: Science/Research",
         "License :: OSI Approved :: BSD License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Scientific/Engineering :: Bio-Informatics",
         "Topic :: Scientific/Engineering :: Information Analysis",
         "Topic :: Scientific/Engineering :: Mathematics",
         "Topic :: Scientific/Engineering :: Physics",
     ],
 }
@@ -51,15 +52,15 @@
     # package installation
     packages=find_packages(exclude=["tests*"]),
     install_requires=open("requirements.txt").read(),
     tests_require=["pytest", "coverage", "pytest-cov", "sequana_fastqc"],
     # This is recursive include of data files
     exclude_package_data={"": ["__pycache__"]},
     package_data={
-        "": ["*.yaml", "*.rules", "*.json", "requirements.txt", "*png", "fastq_screen.conf"],
+        "": ["*.yaml", "*.rules", "*.json", "requirements.txt", "*png"],
     },
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "sequana_completion=sequana_pipetools.completion:main",
             "sequana_slurm_status=sequana_pipetools.slurm:main",
         ]
```

