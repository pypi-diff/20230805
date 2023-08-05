# Comparing `tmp/sr.comp-1.8.1.tar.gz` & `tmp/sr.comp-1.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sr.comp-1.8.1.tar", last modified: Sun Mar 26 15:20:22 2023, max compression
+gzip compressed data, was "dist/sr.comp-1.8.2.tar", last modified: Sat Aug  5 16:17:09 2023, max compression
```

## Comparing `sr.comp-1.8.1.tar` & `sr.comp-1.8.2.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3371 2023-03-26 15:20:22.000000 sr.comp-1.8.1/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1786 2023-03-26 15:20:12.000000 sr.comp-1.8.1/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      416 2023-03-26 15:20:12.000000 sr.comp-1.8.1/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1228 2023-03-26 15:20:22.000000 sr.comp-1.8.1/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-03-26 15:20:12.000000 sr.comp-1.8.1/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/sr/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/sr/comp/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/arenas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/comp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7424 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/automatic_scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4963 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/base_scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1826 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/seeding.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2207 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/stable_random.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4846 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/knockout_scheduler/static_scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/match_period.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5662 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/match_period_clock.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17211 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/matches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10123 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/raw_compstate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18161 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/scores.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1287 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/teams.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2961 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15453 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/validation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8323 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/venue.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4497 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/winners.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1315 2023-03-26 15:20:12.000000 sr.comp-1.8.1/sr/comp/yaml_loader.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/sr.comp.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3371 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-03-26 15:20:21.000000 sr.comp-1.8.1/sr.comp.egg-info/zip-safe
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/venv/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-03-26 15:20:22.000000 sr.comp-1.8.1/venv/bin/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      615 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2html.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      737 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2html4.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2html5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      814 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2latex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      637 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2man.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      803 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2odt.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1741 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      622 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      658 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2s5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      894 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2xetex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      623 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rst2xml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      691 2023-03-26 15:20:20.000000 sr.comp-1.8.1/venv/bin/rstpep2html.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3401 2023-08-05 16:17:09.000000 sr.comp-1.8.2/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1816 2023-08-05 16:16:59.000000 sr.comp-1.8.2/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      400 2023-08-05 16:16:59.000000 sr.comp-1.8.2/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1280 2023-08-05 16:17:09.000000 sr.comp-1.8.2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1603 2023-08-05 16:16:59.000000 sr.comp-1.8.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr/comp/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1582 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/arenas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3101 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/comp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      264 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7424 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/automatic_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4937 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/base_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1826 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/seeding.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2207 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/stable_random.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4846 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/knockout_scheduler/static_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/match_period.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5662 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/match_period_clock.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17211 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/matches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10123 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/raw_compstate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18161 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/scores.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1287 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/teams.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2961 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15453 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/validation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8323 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/venue.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4497 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/winners.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1315 2023-08-05 16:16:59.000000 sr.comp-1.8.2/sr/comp/yaml_loader.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3401 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1076 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       86 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:17:09.000000 sr.comp-1.8.2/sr.comp.egg-info/zip-safe
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/venv/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:17:09.000000 sr.comp-1.8.2/venv/bin/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      625 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2html.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      747 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2html4.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2html5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      824 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2latex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      647 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2man.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      813 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2odt.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      619 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      632 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      668 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2s5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      904 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      633 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rst2xml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      701 2023-08-05 16:17:07.000000 sr.comp-1.8.2/venv/bin/rstpep2html.py
```

### Comparing `sr.comp-1.8.1/PKG-INFO` & `sr.comp-1.8.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: sr.comp
-Version: 1.8.1
+Version: 1.8.2
 Summary: Reliable software for running robotics competitions
 Home-page: https://github.com/PeterJCLaw/srcomp/wiki
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/srcomp/issues
 Description: SRComp
         ======
         
         |Build Status| |Docs Status|
         
-        Yet Another attempt at some Competition Software for `Student
-        Robotics <http://srobo.org>`__.
+        Reliable software for running robotics competitions, primarily used by
+        `Student Robotics <https://studentrobotics.org>`__.
         
         The `SRComp wiki <https://github.com/PeterJCLaw/srcomp/wiki>`__ provides
         an overview of the suite as a whole.
         
         This repository provides a python API to accessing information about the
         state of the competition. That *compstate* is stored as a collection of
         YAML files in a git repository. This allows the state of the competition
@@ -65,15 +65,15 @@
         **Test**:
         ``./run-tests``
         
         .. |Build Status| image:: https://circleci.com/gh/PeterJCLaw/srcomp/tree/main.svg?style=svg
            :target: https://circleci.com/gh/PeterJCLaw/srcomp/tree/main
         
         .. |Docs Status| image:: https://readthedocs.org/projects/srcomp/badge/?version=latest
-           :target: http://srcomp.readthedocs.org/
+           :target: https://srcomp.readthedocs.org/
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sr.comp-1.8.1/README.rst` & `sr.comp-1.8.2/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 SRComp
 ======
 
 |Build Status| |Docs Status|
 
-Yet Another attempt at some Competition Software for `Student
-Robotics <http://srobo.org>`__.
+Reliable software for running robotics competitions, primarily used by
+`Student Robotics <https://studentrobotics.org>`__.
 
 The `SRComp wiki <https://github.com/PeterJCLaw/srcomp/wiki>`__ provides
 an overview of the suite as a whole.
 
 This repository provides a python API to accessing information about the
 state of the competition. That *compstate* is stored as a collection of
 YAML files in a git repository. This allows the state of the competition
@@ -54,8 +54,8 @@
 **Test**:
 ``./run-tests``
 
 .. |Build Status| image:: https://circleci.com/gh/PeterJCLaw/srcomp/tree/main.svg?style=svg
    :target: https://circleci.com/gh/PeterJCLaw/srcomp/tree/main
 
 .. |Docs Status| image:: https://readthedocs.org/projects/srcomp/badge/?version=latest
-   :target: http://srcomp.readthedocs.org/
+   :target: https://srcomp.readthedocs.org/
```

### Comparing `sr.comp-1.8.1/setup.cfg` & `sr.comp-1.8.2/setup.cfg`

 * *Files 7% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 	tests/dummy
 ignore = 
 	B008
 	C401
 	C405
 	W504
 max_line_length = 95
+noqa-require-code = true
 
 [isort]
 indent = 4
 multi_line_output = 3
 use_parentheses = True
 include_trailing_comma = True
 combine_as_imports = True
@@ -26,14 +27,15 @@
 default_section = THIRDPARTY
 known_first_party = sr.comp
 extra_standard_library = typing_extensions
 sections = FUTURE,STDLIB,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [mypy]
 warn_unused_configs = True
+show_column_numbers = True
 show_error_codes = True
 enable_error_code = ignore-without-code
 exclude = tests/dummy/scoring/
 warn_incomplete_stub = True
 warn_unused_ignores = True
 warn_redundant_casts = True
 no_implicit_optional = True
```

### Comparing `sr.comp-1.8.1/setup.py` & `sr.comp-1.8.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_namespace_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='sr.comp',
-    version='1.8.1',
+    version='1.8.2',
     url='https://github.com/PeterJCLaw/srcomp/wiki',
     project_urls={
         'Documentation': 'https://srcomp.readthedocs.org/',
         'Code': 'https://github.com/PeterJCLaw/srcomp',
         'Issue tracker': 'https://github.com/PeterJCLaw/srcomp/issues',
     },
     packages=find_namespace_packages(exclude=('tests',)),
```

### Comparing `sr.comp-1.8.1/sr/comp/arenas.py` & `sr.comp-1.8.2/sr/comp/arenas.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/comp.py` & `sr.comp-1.8.2/sr/comp/comp.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/knockout_scheduler/automatic_scheduler.py` & `sr.comp-1.8.2/sr/comp/knockout_scheduler/automatic_scheduler.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/knockout_scheduler/base_scheduler.py` & `sr.comp-1.8.2/sr/comp/knockout_scheduler/base_scheduler.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,16 +82,15 @@
         """
 
         for arena_matches in self.schedule.matches:
             for match in arena_matches.values():
                 if match.type != MatchType.league:
                     continue
 
-                if (match.arena, match.num) not in \
-                        self.scores.league.game_points:
+                if (match.arena, match.num) not in self.scores.league.game_points:
                     return False
 
         return True
 
     @staticmethod
     def get_match_display_name(
         rounds_remaining: int,
```

### Comparing `sr.comp-1.8.1/sr/comp/knockout_scheduler/seeding.py` & `sr.comp-1.8.2/sr/comp/knockout_scheduler/seeding.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/knockout_scheduler/stable_random.py` & `sr.comp-1.8.2/sr/comp/knockout_scheduler/stable_random.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/knockout_scheduler/static_scheduler.py` & `sr.comp-1.8.2/sr/comp/knockout_scheduler/static_scheduler.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/match_period.py` & `sr.comp-1.8.2/sr/comp/match_period.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/match_period_clock.py` & `sr.comp-1.8.2/sr/comp/match_period_clock.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/matches.py` & `sr.comp-1.8.2/sr/comp/matches.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/raw_compstate.py` & `sr.comp-1.8.2/sr/comp/raw_compstate.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/scores.py` & `sr.comp-1.8.2/sr/comp/scores.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/teams.py` & `sr.comp-1.8.2/sr/comp/teams.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/types.py` & `sr.comp-1.8.2/sr/comp/types.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/validation.py` & `sr.comp-1.8.2/sr/comp/validation.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/venue.py` & `sr.comp-1.8.2/sr/comp/venue.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/winners.py` & `sr.comp-1.8.2/sr/comp/winners.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr/comp/yaml_loader.py` & `sr.comp-1.8.2/sr/comp/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/sr.comp.egg-info/PKG-INFO` & `sr.comp-1.8.2/sr.comp.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 1.2
 Name: sr.comp
-Version: 1.8.1
+Version: 1.8.2
 Summary: Reliable software for running robotics competitions
 Home-page: https://github.com/PeterJCLaw/srcomp/wiki
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp
 Project-URL: Issue tracker, https://github.com/PeterJCLaw/srcomp/issues
 Description: SRComp
         ======
         
         |Build Status| |Docs Status|
         
-        Yet Another attempt at some Competition Software for `Student
-        Robotics <http://srobo.org>`__.
+        Reliable software for running robotics competitions, primarily used by
+        `Student Robotics <https://studentrobotics.org>`__.
         
         The `SRComp wiki <https://github.com/PeterJCLaw/srcomp/wiki>`__ provides
         an overview of the suite as a whole.
         
         This repository provides a python API to accessing information about the
         state of the competition. That *compstate* is stored as a collection of
         YAML files in a git repository. This allows the state of the competition
@@ -65,15 +65,15 @@
         **Test**:
         ``./run-tests``
         
         .. |Build Status| image:: https://circleci.com/gh/PeterJCLaw/srcomp/tree/main.svg?style=svg
            :target: https://circleci.com/gh/PeterJCLaw/srcomp/tree/main
         
         .. |Docs Status| image:: https://readthedocs.org/projects/srcomp/badge/?version=latest
-           :target: http://srcomp.readthedocs.org/
+           :target: https://srcomp.readthedocs.org/
         
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `sr.comp-1.8.1/sr.comp.egg-info/SOURCES.txt` & `sr.comp-1.8.2/sr.comp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/venv/bin/rst2html.py` & `sr.comp-1.8.2/venv/bin/rst2html.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2html.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2html.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates (X)HTML documents from standalone reStructuredText '
                'sources.  ' + default_description)
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2html4.py` & `sr.comp-1.8.2/venv/bin/rst2html4.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2html4.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2html4.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing (X)HTML.
 
 The output conforms to XHTML 1.0 transitional
 and almost to HTML 4.01 transitional (except for closing empty tags).
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates (X)HTML documents from standalone reStructuredText '
                'sources.  ' + default_description)
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2html5.py` & `sr.comp-1.8.2/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `sr.comp-1.8.1/venv/bin/rst2latex.py` & `sr.comp-1.8.2/venv/bin/rst2latex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2latex.py 8956 2022-01-20 10:11:44Z milde $
+# $Id: rst2latex.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing LaTeX.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline
 
 description = ('Generates LaTeX documents from standalone reStructuredText '
                'sources. '
                'Reads from <source> (default is stdin) and writes to '
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2man.py` & `sr.comp-1.8.2/venv/bin/rst2man.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 This module provides a simple command line interface that uses the
 man page writer to output from ReStructuredText source.
 """
 
 import locale
 try:
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 from docutils.writers import manpage
 
 description = ("Generates plain unix manual documents.  "
                + default_description)
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2odt.py` & `sr.comp-1.8.2/venv/bin/rst2odt.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2odt.py 8994 2022-01-29 16:28:17Z milde $
+# $Id: rst2odt.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Dave Kuhlman <dkuhlman@rexx.com>
 # Copyright: This module has been placed in the public domain.
 
 """
 A front end to the Docutils Publisher, producing OpenOffice documents.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline_to_binary, default_description
 from docutils.writers.odf_odt import Writer, Reader
 
 
 description = ('Generates OpenDocument/OpenOffice/ODF documents from '
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2pseudoxml.py` & `sr.comp-1.8.2/venv/bin/rst2pseudoxml.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2pseudoxml.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2pseudoxml.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing pseudo-XML.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates pseudo-XML from standalone reStructuredText '
                'sources (for testing purposes).  ' + default_description)
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2s5.py` & `sr.comp-1.8.2/venv/bin/rst2s5.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2s5.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rst2s5.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Chris Liechti <cliechti@gmx.net>
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing HTML slides using
 the S5 template system.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
 description = ('Generates S5 (X)HTML slideshow documents from standalone '
                'reStructuredText sources.  ' + default_description)
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2xetex.py` & `sr.comp-1.8.2/venv/bin/rst2xetex.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2xetex.py 8956 2022-01-20 10:11:44Z milde $
+# $Id: rst2xetex.py 9115 2022-07-28 17:06:24Z milde $
 # Author: Guenter Milde
 # Copyright: This module has been placed in the public domain.
 
 """
 A minimal front end to the Docutils Publisher, producing Lua/XeLaTeX code.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline
 
 description = ('Generates LaTeX documents from standalone reStructuredText '
                'sources for compilation with the Unicode-aware TeX variants '
                'XeLaTeX or LuaLaTeX. '
```

### Comparing `sr.comp-1.8.1/venv/bin/rst2xml.py` & `sr.comp-1.8.2/venv/bin/rstpep2html.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #!/home/circleci/project/venv/bin/python3
 
-# $Id: rst2xml.py 8927 2022-01-03 23:50:05Z milde $
+# $Id: rstpep2html.py 9115 2022-07-28 17:06:24Z milde $
 # Author: David Goodger <goodger@python.org>
 # Copyright: This module has been placed in the public domain.
 
 """
-A minimal front end to the Docutils Publisher, producing Docutils XML.
+A minimal front end to the Docutils Publisher, producing HTML from PEP
+(Python Enhancement Proposal) documents.
 """
 
 try:
     import locale
     locale.setlocale(locale.LC_ALL, '')
-except:
+except Exception:
     pass
 
 from docutils.core import publish_cmdline, default_description
 
 
-description = ('Generates Docutils-native XML from standalone '
-               'reStructuredText sources.  ' + default_description)
+description = ('Generates (X)HTML from reStructuredText-format PEP files.  '
+               + default_description)
 
-publish_cmdline(writer_name='xml', description=description)
+publish_cmdline(reader_name='pep', writer_name='pep_html',
+                description=description)
```

