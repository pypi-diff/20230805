# Comparing `tmp/auto-editor-23.4.1.tar.gz` & `tmp/auto-editor-23.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-editor-23.4.1.tar", last modified: Wed Jan 25 17:08:02 2023, max compression
+gzip compressed data, was "auto-editor-23.8.1.tar", last modified: Thu Feb 23 17:58:29 2023, max compression
```

## Comparing `auto-editor-23.4.1.tar` & `auto-editor-23.8.1.tar`

### file list

```diff
@@ -1,65 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.128626 auto-editor-23.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-01-25 17:07:48.000000 auto-editor-23.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-01-25 17:07:48.000000 auto-editor-23.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-01-25 17:08:02.128626 auto-editor-23.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-01-25 17:07:48.000000 auto-editor-23.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.124626 auto-editor-23.4.1/auto_editor/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9928 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15060 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)    12546 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10746 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/ffwrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.124626 auto-editor-23.4.1/auto_editor/formats/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5743 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/formats/final_cut_pro.py
--rw-r--r--   0 runner    (1001) docker     (123)     5100 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/formats/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    15746 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/formats/premiere.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/formats/shotcut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/formats/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/help.py
--rw-r--r--   0 runner    (1001) docker     (123)    44165 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9495 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/make_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.124626 auto-editor-23.4.1/auto_editor/objs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/objs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/objs/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/objs/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     2694 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/objs/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/preview.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.124626 auto-editor-23.4.1/auto_editor/render/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/render/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/render/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/render/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/render/subtitle.py
--rw-r--r--   0 runner    (1001) docker     (123)     9343 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/render/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.124626 auto-editor-23.4.1/auto_editor/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/desc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4772 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/levels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/repl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/subdump.py
--rw-r--r--   0 runner    (1001) docker     (123)    26535 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/subcommands/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/timeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.128626 auto-editor-23.4.1/auto_editor/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/chunks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    12714 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/utils/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/validate_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/vanparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8863 2023-01-25 17:07:49.000000 auto-editor-23.4.1/auto_editor/wavfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-25 17:08:02.124626 auto-editor-23.4.1/auto_editor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-25 17:08:02.000000 auto-editor-23.4.1/auto_editor.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-25 17:08:02.128626 auto-editor-23.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-01-25 17:07:49.000000 auto-editor-23.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-02-23 17:58:18.000000 auto-editor-23.8.1/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-02-23 17:58:18.000000 auto-editor-23.8.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-02-23 17:58:29.891395 auto-editor-23.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-02-23 17:58:18.000000 auto-editor-23.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.887395 auto-editor-23.8.1/auto_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9937 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15257 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12453 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10926 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/ffwrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/auto_editor/formats/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5651 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/formats/final_cut_pro.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7499 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/formats/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15692 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/formats/premiere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/formats/shotcut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/formats/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/help.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51284 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/auto_editor/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/lib/contracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/make_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/auto_editor/objs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/objs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/objs/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/objs/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/preview.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/auto_editor/render/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/render/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4018 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/render/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4356 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/render/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/render/subtitle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/render/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/auto_editor/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/desc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4214 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/levels.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/palet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/subdump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27982 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/subcommands/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/timeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.891395 auto-editor-23.8.1/auto_editor/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/chunks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7692 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2638 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12731 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/utils/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/validate_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9705 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/vanparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8861 2023-02-23 17:58:19.000000 auto-editor-23.8.1/auto_editor/wavfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 17:58:29.887395 auto-editor-23.8.1/auto_editor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7260 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 17:58:29.000000 auto-editor-23.8.1/auto_editor.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 17:58:29.891395 auto-editor-23.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-02-23 17:58:19.000000 auto-editor-23.8.1/setup.py
```

### Comparing `auto-editor-23.4.1/LICENSE` & `auto-editor-23.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/PKG-INFO` & `auto-editor-23.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-editor
-Version: 23.4.1
+Version: 23.8.1
 Summary: Auto-Editor: Effort free video editing!
 Home-page: https://auto-editor.com
 Author: WyattBlue
 Author-email: wyattblue@auto-editor.com
 License: Unlicense
 Project-URL: Bug Tracker, https://github.com/WyattBlue/auto-editor/issues
 Project-URL: Source Code, https://github.com/WyattBlue/auto-editor
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-editor Version: 23.4.1 Summary: Auto-Editor:
+Metadata-Version: 2.1 Name: auto-editor Version: 23.8.1 Summary: Auto-Editor:
 Effort free video editing! Home-page: https://auto-editor.com Author: WyattBlue
 Author-email: wyattblue@auto-editor.com License: Unlicense Project-URL: Bug
 Tracker, https://github.com/WyattBlue/auto-editor/issues Project-URL: Source
 Code, https://github.com/WyattBlue/auto-editor Keywords: video audio media
 editor editing processing nonlinear automatic silence-detect silence-removal
 silence-speedup motion-detection Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video Classifier: License :: Public Domain
```

### Comparing `auto-editor-23.4.1/README.md` & `auto-editor-23.8.1/README.md`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/__main__.py` & `auto-editor-23.8.1/auto_editor/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,15 +276,15 @@
         help="Add extra options for ffmpeg. Must be in quotes",
     )
     parser.add_argument("--version", "-V", flag=True, help="Display version and halt")
     return parser
 
 
 def main() -> None:
-    subcommands = ("test", "info", "levels", "subdump", "desc", "repl")
+    subcommands = ("test", "info", "levels", "subdump", "desc", "repl", "palet")
 
     if len(sys.argv) > 1 and sys.argv[1] in subcommands:
         obj = __import__(
             f"auto_editor.subcommands.{sys.argv[1]}", fromlist=["subcommands"]
         )
         obj.main(sys.argv[2:])
         sys.exit()
```

### Comparing `auto-editor-23.4.1/auto_editor/analyze.py` & `auto-editor-23.8.1/auto_editor/analyze.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 from __future__ import annotations
 
 import json
 import os
 import re
+from dataclasses import dataclass
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from auto_editor import version
 from auto_editor.objs.edit import (
-    Audio,
-    Motion,
-    Pixeldiff,
-    Subtitle,
     audio_builder,
     motion_builder,
     pixeldiff_builder,
     subtitle_builder,
 )
 from auto_editor.objs.util import ParserError, parse_dataclass
 from auto_editor.render.subtitle import SubtitleParser
@@ -27,20 +24,34 @@
 if TYPE_CHECKING:
     from fractions import Fraction
     from typing import Any
 
     from numpy.typing import NDArray
 
     from auto_editor.ffwrapper import FileInfo
-    from auto_editor.interpreter import FileSetup
     from auto_editor.output import Ensure
     from auto_editor.utils.bar import Bar
     from auto_editor.utils.log import Log
 
 
+@dataclass
+class FileSetup:
+    src: FileInfo
+    ensure: Ensure
+    strict: bool
+    tb: Fraction
+    bar: Bar
+    temp: str
+    log: Log
+
+
+class LevelError(Exception):
+    pass
+
+
 def link_nodes(*nodes: Any) -> None:
     for c, n in zip(nodes, nodes[1:]):
         c.link_to(n)
 
 
 def to_threshold(arr: np.ndarray, t: int | float) -> NDArray[np.bool_]:
     return np.fromiter((x >= t for x in arr), dtype=np.bool_)
@@ -56,491 +67,450 @@
             if not active:
                 start_p = j
                 active = True
             # Special case for end.
             if j == len(arr) - 1:
                 if j - start_p < lim:
                     arr[start_p : j + 1] = with_
-        else:
-            if active:
-                if j - start_p < lim:
-                    arr[start_p:j] = with_
-                active = False
+        elif active:
+            if j - start_p < lim:
+                arr[start_p:j] = with_
+            active = False
 
 
-def get_media_length(
-    ensure: Ensure, src: FileInfo, tb: Fraction, temp: str, log: Log
-) -> int:
-    if src.audios:
-        if (arr := read_cache(src, tb, "audio", {"stream": 0}, temp)) is not None:
-            return len(arr)
+def obj_tag(tag: str, tb: Fraction, obj: dict[str, Any]) -> str:
+    key = f"{tag}:{tb}:"
+    for k, v in obj.items():
+        key += f"{k}={v},"
 
-        sr, samples = read(ensure.audio(f"{src.path.resolve()}", src.label, stream=0))
-        samp_count = len(samples)
-        del samples
+    key = key[:-1]  # remove unnecessary char
+    return key
 
-        samp_per_ticks = sr / tb
-        ticks = int(samp_count / samp_per_ticks)
-        log.debug(f"Audio Length: {ticks}")
-        log.debug(f"... without rounding: {float(samp_count / samp_per_ticks)}")
-        return ticks
 
-    # If there's no audio, get length in video metadata.
-    import av
+class Levels:
+    def __init__(
+        self, ensure: Ensure, src: FileInfo, tb: Fraction, bar: Bar, temp: str, log: Log
+    ):
+        self.ensure = ensure
+        self.src = src
+        self.tb = tb
+        self.bar = bar
+        self.temp = temp
+        self.log = log
+
+    @property
+    def media_length(self) -> int:
+        if self.src.audios:
+            if (arr := self.read_cache("audio", {"stream": 0})) is not None:
+                return len(arr)
+
+            sr, samples = read(
+                self.ensure.audio(
+                    f"{self.src.path.resolve()}", self.src.label, stream=0
+                )
+            )
+            samp_count = len(samples)
+            del samples
 
-    av.logging.set_level(av.logging.PANIC)
+            samp_per_ticks = sr / self.tb
+            ticks = int(samp_count / samp_per_ticks)
+            self.log.debug(f"Audio Length: {ticks}")
+            self.log.debug(
+                f"... without rounding: {float(samp_count / samp_per_ticks)}"
+            )
+            return ticks
 
-    with av.open(f"{src.path}") as cn:
-        if len(cn.streams.video) < 1:
-            log.error("Could not get media duration")
+        # If there's no audio, get length in video metadata.
+        import av
 
-        video = cn.streams.video[0]
-        dur = int(video.duration * video.time_base * tb)
-        log.debug(f"Video duration: {dur}")
+        av.logging.set_level(av.logging.PANIC)
 
-    return dur
+        with av.open(f"{self.src.path}") as cn:
+            if len(cn.streams.video) < 1:
+                self.log.error("Could not get media duration")
 
+            video = cn.streams.video[0]
+            dur = int(video.duration * video.time_base * self.tb)
+            self.log.debug(f"Video duration: {dur}")
 
-def get_all(
-    ensure: Ensure, src: FileInfo, tb: Fraction, temp: str, log: Log
-) -> NDArray[np.bool_]:
-    return np.zeros(get_media_length(ensure, src, tb, temp, log), dtype=np.bool_)
+        return dur
 
+    def none(self) -> NDArray[np.bool_]:
+        return np.ones(self.media_length, dtype=np.bool_)
 
-def get_none(
-    ensure: Ensure, src: FileInfo, tb: Fraction, temp: str, log: Log
-) -> NDArray[np.bool_]:
-    return np.ones(get_media_length(ensure, src, tb, temp, log), dtype=np.bool_)
+    def all(self) -> NDArray[np.bool_]:
+        return np.zeros(self.media_length, dtype=np.bool_)
 
+    def read_cache(self, tag: str, obj: dict[str, Any]) -> None | np.ndarray:
+        workfile = os.path.join(
+            os.path.dirname(self.temp), f"ae-{version}", "cache.json"
+        )
 
-def _dict_tag(tag: str, tb: Fraction, obj: Any) -> tuple[str, dict]:
-    if isinstance(obj, dict):
-        obj_dict = obj.copy()
-    else:
-        obj_dict = obj.__dict__.copy()
-    if "threshold" in obj_dict:
-        del obj_dict["threshold"]
+        try:
+            with open(workfile) as file:
+                cache = json.load(file)
+        except Exception:
+            return None
 
-    key = f"{tag}:{tb}:"
-    for k, v in obj_dict.items():
-        key += f"{k}={v},"
-    key = key[:-1]
+        if f"{self.src.path.resolve()}" not in cache:
+            return None
 
-    return key, obj_dict
+        key = obj_tag(tag, self.tb, obj)
 
+        if key not in (root := cache[f"{self.src.path.resolve()}"]):
+            return None
 
-def read_cache(
-    src: FileInfo, tb: Fraction, tag: str, obj: Any, temp: str
-) -> None | np.ndarray:
+        return np.asarray(root[key]["arr"], dtype=root[key]["type"])
 
-    workfile = os.path.join(os.path.dirname(temp), f"ae-{version}", "cache.json")
+    def cache(self, tag: str, obj: dict[str, Any], arr: np.ndarray) -> np.ndarray:
+        workdur = os.path.join(os.path.dirname(self.temp), f"ae-{version}")
+        workfile = os.path.join(workdur, "cache.json")
+        if not os.path.exists(workdur):
+            os.mkdir(workdur)
 
-    try:
-        with open(workfile) as file:
-            cache = json.load(file)
-    except Exception:
-        return None
+        key = obj_tag(tag, self.tb, obj)
 
-    if f"{src.path.resolve()}" not in cache:
-        return None
+        try:
+            with open(workfile) as file:
+                json_object = json.load(file)
+        except Exception:
+            json_object = {}
+
+        entry = {
+            "type": str(arr.dtype),
+            "arr": arr.tolist(),
+        }
 
-    key, obj_dict = _dict_tag(tag, tb, obj)
+        src_key = f"{self.src.path}"
 
-    if key not in (root := cache[f"{src.path.resolve()}"]):
-        return None
+        if src_key in json_object:
+            json_object[src_key][key] = entry
+        else:
+            json_object[src_key] = {key: entry}
 
-    return np.asarray(root[key]["arr"], dtype=root[key]["type"])
+        with open(os.path.join(workdur, "cache.json"), "w") as file:
+            file.write(json.dumps(json_object))
 
+        return arr
 
-def cache(
-    tag: str, tb: Fraction, obj: Any, arr: np.ndarray, src: FileInfo, temp: str
-) -> np.ndarray:
+    def audio(self, s: int) -> NDArray[np.float_]:
+        if s > len(self.src.audios) - 1:
+            raise LevelError(f"audio: audio stream '{s}' does not exist.")
 
-    workdur = os.path.join(os.path.dirname(temp), f"ae-{version}")
-    workfile = os.path.join(workdur, "cache.json")
-    if not os.path.exists(workdur):
-        os.mkdir(workdur)
+        if (arr := self.read_cache("audio", {"stream": s})) is not None:
+            return arr
 
-    key, obj_dict = _dict_tag(tag, tb, obj)
+        sr, samples = read(
+            self.ensure.audio(f"{self.src.path.resolve()}", self.src.label, s)
+        )
 
-    try:
-        with open(workfile) as file:
-            json_object = json.load(file)
-    except Exception:
-        json_object = {}
-
-    entry = {
-        "type": str(arr.dtype),
-        "arr": arr.tolist(),
-    }
+        if len(samples) == 0:
+            raise LevelError(f"audio: audio stream '{s}' has length of 0.")
 
-    src_key = f"{src.path}"
+        def get_max_volume(s: np.ndarray) -> float:
+            return max(float(np.max(s)), -float(np.min(s)))
 
-    if src_key in json_object:
-        json_object[src_key][key] = entry
-    else:
-        json_object[src_key] = {key: entry}
+        max_volume = get_max_volume(samples)
+        self.log.debug(f"Max volume: {max_volume}")
 
-    with open(os.path.join(workdur, "cache.json"), "w") as file:
-        file.write(json.dumps(json_object))
+        samp_count = samples.shape[0]
+        samp_per_ticks = sr / self.tb
 
-    return arr
+        audio_ticks = int(samp_count / samp_per_ticks)
+        self.log.debug(f"analyze: Audio Length: {audio_ticks}")
+        self.log.debug(f"... no rounding: {float(samp_count / samp_per_ticks)}")
 
+        self.bar.start(audio_ticks, "Analyzing audio volume")
 
-def audio_levels(
-    ensure: Ensure,
-    src: FileInfo,
-    s: int,
-    tb: Fraction,
-    bar: Bar,
-    strict: bool,
-    temp: str,
-    log: Log,
-) -> NDArray[np.float_]:
+        threshold_list = np.zeros((audio_ticks), dtype=np.float_)
 
-    if s > len(src.audios) - 1:
-        if strict:
-            log.error(f"Audio stream '{s}' does not exist.")
-        return np.zeros(get_media_length(ensure, src, tb, temp, log), dtype=np.float_)
+        if max_volume == 0:  # Prevent dividing by zero
+            return threshold_list
 
-    if (arr := read_cache(src, tb, "audio", {"stream": s}, temp)) is not None:
-        return arr
+        # Determine when audio is silent or loud.
+        for i in range(audio_ticks):
+            if i % 500 == 0:
+                self.bar.tick(i)
 
-    sr, samples = read(ensure.audio(f"{src.path.resolve()}", src.label, s))
+            start = int(i * samp_per_ticks)
+            end = min(int((i + 1) * samp_per_ticks), samp_count)
 
-    def get_max_volume(s: np.ndarray) -> float:
-        return max(float(np.max(s)), -float(np.min(s)))
+            threshold_list[i] = get_max_volume(samples[start:end]) / max_volume
 
-    max_volume = get_max_volume(samples)
-    log.debug(f"Max volume: {max_volume}")
+        self.bar.end()
+        return self.cache("audio", {"stream": s}, threshold_list)
 
-    samp_count = samples.shape[0]
-    samp_per_ticks = sr / tb
+    def subtitle(
+        self,
+        patterns: str,
+        stream: int,
+        ignore_case: bool,
+        max_count: int | None,
+    ) -> NDArray[np.bool_]:
+        if stream >= len(self.src.subtitles):
+            raise LevelError(f"subtitle: subtitle stream '{stream}' does not exist.")
 
-    audio_ticks = int(samp_count / samp_per_ticks)
-    log.debug(f"analyze: Audio Length: {audio_ticks}")
-    log.debug(f"... no rounding: {float(samp_count / samp_per_ticks)}")
+        try:
+            flags = re.IGNORECASE if ignore_case else 0
+            pattern = re.compile(patterns, flags)
+            del patterns  # make sure we don't accidentally use it
+        except re.error as e:
+            self.log.error(e)
 
-    bar.start(audio_ticks, "Analyzing audio volume")
+        sub_file = self.ensure.subtitle(
+            f"{self.src.path.resolve()}", self.src.label, stream=stream
+        )
+        parser = SubtitleParser(self.tb)
 
-    threshold_list = np.zeros((audio_ticks), dtype=np.float_)
+        with open(sub_file) as file:
+            parser.parse(file.read(), "webvtt")
 
-    if max_volume == 0:  # Prevent dividing by zero
-        return threshold_list
+        # stackoverflow.com/questions/9662346/python-code-to-remove-html-tags-from-a-string
+        def cleanhtml(raw_html: str) -> str:
+            cleanr = re.compile("<.*?>")
+            return re.sub(cleanr, "", raw_html)
 
-    # Determine when audio is silent or loud.
-    for i in range(audio_ticks):
-        if i % 500 == 0:
-            bar.tick(i)
+        if not parser.contents:
+            self.log.error("subtitle has no valid entries")
 
-        start = int(i * samp_per_ticks)
-        end = min(int((i + 1) * samp_per_ticks), samp_count)
+        result = np.zeros((parser.contents[-1].end), dtype=np.bool_)
 
-        threshold_list[i] = get_max_volume(samples[start:end]) / max_volume
+        count = 0
+        for content in parser.contents:
+            if max_count is not None and count >= max_count:
+                break
 
-    bar.end()
-    return cache("audio", tb, {"stream": s}, threshold_list, src, temp)
+            line = cleanhtml(content.after.strip())
+            if line and re.search(pattern, line):
+                result[content.start : content.end] = 1
+                count += 1
 
+        return result
 
-def subtitle_levels(
-    ensure: Ensure,
-    src: FileInfo,
-    sobj: Any,
-    tb: Fraction,
-    bar: Bar,
-    strict: bool,
-    temp: str,
-    log: Log,
-) -> NDArray[np.bool_]:
+    def motion(self, s: int, blur: int, width: int) -> NDArray[np.float_]:
+        import av
+        from PIL import ImageChops, ImageFilter
 
-    if sobj.stream >= len(src.subtitles):
-        if not strict:
-            return np.zeros(
-                get_media_length(ensure, src, tb, temp, log), dtype=np.float_
-            )
-        log.error(f"Subtitle stream '{sobj.stream}' does not exist.")
+        av.logging.set_level(av.logging.PANIC)
 
-    try:
-        flags = re.IGNORECASE if sobj.ignore_case else 0
-        pattern = re.compile(sobj.pattern, flags)
-    except re.error as e:
-        log.error(e)
+        mobj = {"stream": s, "width": width, "blur": blur}
+
+        if s >= len(self.src.videos):
+            raise LevelError(f"motion: video stream '{s}' does not exist.")
+
+        if (arr := self.read_cache("motion", mobj)) is not None:
+            return arr
 
-    sub_file = ensure.subtitle(f"{src.path.resolve()}", src.label, stream=sobj.stream)
-    parser = SubtitleParser(tb)
+        container = av.open(f"{self.src.path}", "r")
 
-    with open(sub_file) as file:
-        parser.parse(file.read(), "webvtt")
+        stream = container.streams.video[s]
+        stream.thread_type = "AUTO"
 
-    # stackoverflow.com/questions/9662346/python-code-to-remove-html-tags-from-a-string
-    def cleanhtml(raw_html: str) -> str:
-        cleanr = re.compile("<.*?>")
-        return re.sub(cleanr, "", raw_html)
-
-    if not parser.contents:
-        log.error("subtitle has no valid entries")
-
-    result = np.zeros((parser.contents[-1].end), dtype=np.bool_)
-
-    count = 0
-    for content in parser.contents:
-        if sobj.max_count is not None and count >= sobj.max_count:
-            break
-
-        line = cleanhtml(content.after.strip())
-        if line and re.search(pattern, line):
-            result[content.start : content.end] = 1
-            count += 1
-
-    return result
-
-
-def motion_levels(
-    ensure: Ensure,
-    src: FileInfo,
-    mobj: Any,
-    tb: Fraction,
-    bar: Bar,
-    strict: bool,
-    temp: str,
-    log: Log,
-) -> NDArray[np.float_]:
-    import av
-    from PIL import ImageChops, ImageFilter
-
-    av.logging.set_level(av.logging.PANIC)
-
-    if mobj.stream >= len(src.videos):
-        if not strict:
-            return np.zeros(
-                get_media_length(ensure, src, tb, temp, log), dtype=np.float_
+        if stream.duration is None:
+            inaccurate_dur = 1
+        else:
+            inaccurate_dur = int(
+                stream.duration * stream.time_base * stream.average_rate
             )
-        log.error(f"Video stream '{mobj.stream}' does not exist.")
 
-    if (arr := read_cache(src, tb, "motion", mobj, temp)) is not None:
-        return arr
+        self.bar.start(inaccurate_dur, "Analyzing motion")
 
-    container = av.open(f"{src.path}", "r")
+        prev_image = None
+        image = None
+        total_pixels = self.src.videos[0].width * self.src.videos[0].height
+        index = 0
+
+        graph = av.filter.Graph()
+        link_nodes(
+            graph.add_buffer(template=stream),
+            graph.add("scale", f"{width}:-1"),
+            graph.add("buffersink"),
+        )
+        graph.configure()
 
-    stream = container.streams.video[mobj.stream]
-    stream.thread_type = "AUTO"
+        threshold_list = np.zeros((1024), dtype=np.float_)
 
-    if stream.duration is None:
-        inaccurate_dur = 1
-    else:
-        inaccurate_dur = int(stream.duration * stream.time_base * stream.average_rate)
+        for unframe in container.decode(stream):
+            graph.push(unframe)
+            frame = graph.pull()
 
-    bar.start(inaccurate_dur, "Analyzing motion")
+            prev_image = image
 
-    prev_image = None
-    image = None
-    total_pixels = src.videos[0].width * src.videos[0].height
-    index = 0
-
-    graph = av.filter.Graph()
-    link_nodes(
-        graph.add_buffer(template=stream),
-        graph.add("scale", f"{mobj.width}:-1"),
-        graph.add("buffersink"),
-    )
-    graph.configure()
-
-    threshold_list = np.zeros((1024), dtype=np.float_)
-
-    for unframe in container.decode(stream):
-        graph.push(unframe)
-        frame = graph.pull()
-
-        prev_image = image
-
-        index = int(frame.time * tb)
-        bar.tick(index)
-
-        if index > len(threshold_list) - 1:
-            threshold_list = np.concatenate(
-                (threshold_list, np.zeros((len(threshold_list)), dtype=np.float_)),
-                axis=0,
-            )
+            index = int(frame.time * self.tb)
+            self.bar.tick(index)
 
-        image = frame.to_image().convert("L")
+            if index > len(threshold_list) - 1:
+                threshold_list = np.concatenate(
+                    (threshold_list, np.zeros((len(threshold_list)), dtype=np.float_)),
+                    axis=0,
+                )
 
-        if mobj.blur > 0:
-            image = image.filter(ImageFilter.GaussianBlur(radius=mobj.blur))
+            image = frame.to_image().convert("L")
 
-        if prev_image is not None:
-            count = np.count_nonzero(ImageChops.difference(prev_image, image))
+            if blur > 0:
+                image = image.filter(ImageFilter.GaussianBlur(radius=blur))
 
-            threshold_list[index] = count / total_pixels
-
-    bar.end()
-    result = threshold_list[:index]
-    del threshold_list
-
-    return cache("motion", tb, mobj, result, src, temp)
-
-
-def pixeldiff_levels(
-    ensure: Ensure,
-    src: FileInfo,
-    pobj: Any,
-    tb: Fraction,
-    bar: Bar,
-    strict: bool,
-    temp: str,
-    log: Log,
-) -> NDArray[np.uint64]:
-    import av
-    from PIL import ImageChops
-
-    av.logging.set_level(av.logging.PANIC)
-
-    if pobj.stream >= len(src.videos):
-        if not strict:
-            return np.zeros(
-                get_media_length(ensure, src, tb, temp, log), dtype=np.uint64
-            )
-        log.error(f"Video stream '{pobj.stream}' does not exist.")
+            if prev_image is not None:
+                count = np.count_nonzero(ImageChops.difference(prev_image, image))
 
-    if (arr := read_cache(src, tb, "pixeldiff", pobj, temp)) is not None:
-        return arr
+                threshold_list[index] = count / total_pixels
 
-    container = av.open(f"{src.path}", "r")
+        self.bar.end()
+        result = threshold_list[:index]
+        del threshold_list
 
-    stream = container.streams.video[pobj.stream]
-    stream.thread_type = "AUTO"
+        return self.cache("motion", mobj, result)
 
-    if stream.duration is None:
-        inaccurate_dur = 1
-    else:
-        inaccurate_dur = int(stream.duration * stream.time_base * stream.average_rate)
+    def pixeldiff(self, s: int) -> NDArray[np.uint64]:
+        import av
+        from PIL import ImageChops
+
+        av.logging.set_level(av.logging.PANIC)
 
-    bar.start(inaccurate_dur, "Analyzing pixel diffs")
+        pobj = {"stream": s}
 
-    prev_image = None
-    image = None
-    index = 0
+        if s >= len(self.src.videos):
+            raise LevelError(f"pixeldiff: video stream '{s}' does not exist.")
 
-    threshold_list = np.zeros((1024), dtype=np.uint64)
+        if (arr := self.read_cache("pixeldiff", pobj)) is not None:
+            return arr
 
-    for frame in container.decode(stream):
-        prev_image = image
+        container = av.open(f"{self.src.path}", "r")
 
-        index = int(frame.time * tb)
-        bar.tick(index)
+        stream = container.streams.video[s]
+        stream.thread_type = "AUTO"
 
-        if index > len(threshold_list) - 1:
-            threshold_list = np.concatenate(
-                (threshold_list, np.zeros((len(threshold_list)), dtype=np.uint64)),
-                axis=0,
+        if stream.duration is None:
+            inaccurate_dur = 1
+        else:
+            inaccurate_dur = int(
+                stream.duration * stream.time_base * stream.average_rate
             )
 
-        image = frame.to_image()
+        self.bar.start(inaccurate_dur, "Analyzing pixel diffs")
 
-        if prev_image is not None:
-            threshold_list[index] = np.count_nonzero(
-                ImageChops.difference(prev_image, image)
-            )
+        prev_image = None
+        image = None
+        index = 0
+
+        threshold_list = np.zeros((1024), dtype=np.uint64)
 
-    bar.end()
-    result = threshold_list[:index]
-    del threshold_list
+        for frame in container.decode(stream):
+            prev_image = image
 
-    return cache("pixeldiff", tb, pobj, result, src, temp)
+            index = int(frame.time * self.tb)
+            self.bar.tick(index)
+
+            if index > len(threshold_list) - 1:
+                threshold_list = np.concatenate(
+                    (threshold_list, np.zeros((len(threshold_list)), dtype=np.uint64)),
+                    axis=0,
+                )
+
+            image = frame.to_image()
+
+            if prev_image is not None:
+                threshold_list[index] = np.count_nonzero(
+                    ImageChops.difference(prev_image, image)
+                )
+
+        self.bar.end()
+        result = threshold_list[:index]
+        del threshold_list
+
+        return self.cache("pixeldiff", pobj, result)
 
 
 def edit_method(val: str, filesetup: FileSetup) -> NDArray[np.bool_]:
+    assert isinstance(filesetup, FileSetup)
     src = filesetup.src
     tb = filesetup.tb
     ensure = filesetup.ensure
     strict = filesetup.strict
     bar = filesetup.bar
     temp = filesetup.temp
     log = filesetup.log
 
     if ":" in val:
         method, attrs = val.split(":", 1)
     else:
         method, attrs = val, ""
 
-    if method == "none":
-        return get_none(ensure, src, tb, temp, log)
-
-    if method == "all":
-        return get_all(ensure, src, tb, temp, log)
-
     def my_var_f(name: str, val: str, coerce: Any) -> Any:
         if src.videos:
             if name in ("x", "width"):
                 return pos((val, src.videos[0].width))
             if name in ("y", "height"):
                 return pos((val, src.videos[0].height))
         return coerce(val)
 
-    if method == "audio":
-        try:
-            aobj = parse_dataclass(attrs, (Audio, audio_builder))
-        except ParserError as e:
-            log.error(e)
-
-        s = aobj.stream
-        if s == "all":
-            total_list: NDArray[np.bool_] | None = None
-            for s in range(len(src.audios)):
-                audio_list = to_threshold(
-                    audio_levels(ensure, src, s, tb, bar, strict, temp, log),
-                    aobj.threshold,
-                )
-                if total_list is None:
-                    total_list = audio_list
-                else:
-                    total_list = boolop(total_list, audio_list, np.logical_or)
-            if total_list is None:
-                if strict:
-                    log.error("Input has no audio streams.")
-                stream_data = get_all(ensure, src, tb, temp, log)
-            else:
-                stream_data = total_list
-        else:
-            stream_data = to_threshold(
-                audio_levels(ensure, src, s, tb, bar, strict, temp, log),
-                aobj.threshold,
-            )
+    builder_map = {
+        "audio": audio_builder,
+        "motion": motion_builder,
+        "pixeldiff": pixeldiff_builder,
+        "subtitle": subtitle_builder,
+    }
 
-        def st(val: int | str) -> int:
-            if isinstance(val, str):
-                return round(float(val) * tb)
-            return val
+    levels = Levels(ensure, src, tb, bar, temp, log)
 
-        mut_remove_small(stream_data, st(aobj.minclip), replace=1, with_=0)
-        mut_remove_small(stream_data, st(aobj.mincut), replace=0, with_=1)
+    if method == "none":
+        return levels.none()
+    if method == "all":
+        return levels.all()
 
-        return stream_data
+    try:
+        obj = parse_dataclass(attrs, builder_map[method])
+    except ParserError as e:
+        log.error(e)
 
-    if method == "motion":
-        try:
-            mobj = parse_dataclass(attrs, (Motion, motion_builder), my_var_f)
-        except ParserError as e:
-            log.error(e)
-        return to_threshold(
-            motion_levels(ensure, src, mobj, tb, bar, strict, temp, log),
-            mobj.threshold,
-        )
+    try:
+        if method == "audio":
+            s = obj["stream"]
+            if s == "all":
+                total_list: NDArray[np.bool_] | None = None
+                for s in range(len(src.audios)):
+                    audio_list = to_threshold(levels.audio(s), obj["threshold"])
+                    if total_list is None:
+                        total_list = audio_list
+                    else:
+                        total_list = boolop(total_list, audio_list, np.logical_or)
 
-    if method == "subtitle":
-        try:
-            sobj = parse_dataclass(attrs, (Subtitle, subtitle_builder))
-        except ParserError as e:
-            log.error(e)
+                if total_list is None:
+                    if strict:
+                        log.error("Input has no audio streams.")
+                    stream_data = levels.all()
+                else:
+                    stream_data = total_list
+            else:
+                stream_data = to_threshold(levels.audio(s), obj["threshold"])
 
-        return subtitle_levels(ensure, src, sobj, tb, bar, strict, temp, log)
+            def st(val: int | str) -> int:
+                if isinstance(val, str):
+                    return round(float(val) * tb)
+                return val
+
+            mut_remove_small(stream_data, st(obj["minclip"]), replace=1, with_=0)
+            mut_remove_small(stream_data, st(obj["mincut"]), replace=0, with_=1)
+
+            return stream_data
+
+        if method == "motion":
+            return to_threshold(
+                levels.motion(obj["stream"], obj["blur"], obj["width"]),
+                obj["threshold"],
+            )
+        if method == "pixeldiff":
+            return to_threshold(levels.pixeldiff(obj["stream"]), obj["threshold"])
 
-    if method == "pixeldiff":
-        try:
-            pobj = parse_dataclass(attrs, (Pixeldiff, pixeldiff_builder), my_var_f)
-        except ParserError as e:
+        if method == "subtitle":
+            return levels.subtitle(
+                obj["pattern"],
+                obj["stream"],
+                obj["ignore_case"],
+                obj["max_count"],
+            )
+    except LevelError as e:
+        if strict:
             log.error(e)
-        return to_threshold(
-            pixeldiff_levels(ensure, src, pobj, tb, bar, strict, temp, log),
-            pobj.threshold,
-        )
 
+        return levels.all()
     raise ValueError("Unreachable")
```

### Comparing `auto-editor-23.4.1/auto_editor/edit.py` & `auto-editor-23.8.1/auto_editor/edit.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,60 @@
 from __future__ import annotations
 
 import os
 from typing import Any
 
 from auto_editor.ffwrapper import FFmpeg, FileInfo
 from auto_editor.make_layers import make_timeline
-from auto_editor.objs.export import (
-    ExAudio,
-    ExClipSequence,
-    ExDefault,
-    ExFinalCutPro,
-    ExJson,
-    Exports,
-    ExPremiere,
-    ExShotCut,
-    ExTimeline,
-)
-from auto_editor.objs.util import Attr, ParserError, parse_dataclass
+from auto_editor.objs.util import Attr, Attrs, ParserError, parse_dataclass
 from auto_editor.output import Ensure, mux_quality_media
 from auto_editor.render.audio import make_new_audio
 from auto_editor.render.subtitle import make_new_subtitles
 from auto_editor.render.video import render_av
 from auto_editor.timeline import timeline_builder, v1, v3
 from auto_editor.utils.bar import Bar
 from auto_editor.utils.chunks import Chunk, Chunks
 from auto_editor.utils.container import Container, container_constructor
 from auto_editor.utils.log import Log, Timer
 from auto_editor.utils.types import Args
 
 
 def set_output(
     out: str | None, _export: str | None, src: FileInfo | None, log: Log
-) -> tuple[str, Exports]:
-
-    export = None if _export is None else parse_export(_export, log)
-
+) -> tuple[str, dict[str, Any]]:
     if src is None:
         root, ext = "out", ".mp4"
     else:
         root, ext = os.path.splitext(str(src.path) if out is None else out)
         if ext == "":
             ext = src.path.suffix
 
-    if export is None:
+    if _export is None:
         if ext == ".xml":
-            export = ExPremiere()
+            export = {"export": "premiere"}
         elif ext == ".fcpxml":
-            export = ExFinalCutPro()
+            export = {"export": "final-cut-pro"}
         elif ext == ".mlt":
-            export = ExShotCut()
+            export = {"export": "shotcut"}
         elif ext == ".json":
-            export = ExJson()
+            export = {"export": "json"}
         else:
-            export = ExDefault()
+            export = {"export": "default"}
+    else:
+        export = parse_export(_export, log)
 
-    if isinstance(export, ExPremiere):
-        ext = ".xml"
-    if isinstance(export, ExFinalCutPro):
-        ext = ".fcpxml"
-    if isinstance(export, ExShotCut):
-        ext = ".mlt"
-    if isinstance(export, ExJson):
-        ext = ".json"
-    if isinstance(export, ExAudio):
-        ext = ".wav"
+    ext_map = {
+        "premiere": ".xml",
+        "final-cut-pro": ".fcpxml",
+        "shotcut": ".mlt",
+        "json": ".json",
+        "audio": ".wav",
+    }
+    if export["export"] in ext_map:
+        ext = ext_map[export["export"]]
 
     if out is None:
         return f"{root}_ALTERED{ext}", export
 
     return f"{root}{ext}", export
 
 
@@ -136,15 +123,14 @@
 
     return codec
 
 
 def make_sources(
     paths: list[str], ffmpeg: FFmpeg, log: Log
 ) -> tuple[dict[str, FileInfo], list[int]]:
-
     used_paths: dict[str, int] = {}
     sources: dict[str, FileInfo] = {}
     inputs: list[int] = []
 
     i = 0
     for path in paths:
         if path in used_paths:
@@ -153,45 +139,46 @@
             sources[str(i)] = FileInfo(path, ffmpeg, log, str(i))
             inputs.append(i)
             used_paths[path] = i
             i += 1
     return sources, inputs
 
 
-def parse_export(export: str, log: Log) -> Exports:
+def parse_export(export: str, log: Log) -> dict[str, Any]:
     exploded = export.split(":", maxsplit=1)
     if len(exploded) == 1:
-        name, attrs = exploded[0], ""
+        name, text = exploded[0], ""
     else:
-        name, attrs = exploded
+        name, text = exploded
 
-    parsing: dict[str, tuple[Any, list[Attr]]] = {
-        "default": (ExDefault, []),
-        "premiere": (ExPremiere, [Attr("name", str, None)]),
-        "final-cut-pro": (ExFinalCutPro, [Attr("name", str, None)]),
-        "shotcut": (ExShotCut, []),
-        "json": (ExJson, timeline_builder),
-        "timeline": (ExTimeline, timeline_builder),
-        "audio": (ExAudio, []),
-        "clip-sequence": (ExClipSequence, []),
+    parsing: dict[str, Attrs] = {
+        "default": Attrs("default"),
+        "premiere": Attrs("premiere", Attr("name", str, None)),
+        "final-cut-pro": Attrs("final-cut-pro", Attr("name", str, None)),
+        "shotcut": Attrs("shotcut"),
+        "json": timeline_builder,
+        "timeline": timeline_builder,
+        "audio": Attrs("audio"),
+        "clip-sequence": Attrs("clip-sequence"),
     }
 
     if name in parsing:
         try:
-            return parse_dataclass(attrs, parsing[name])
+            _tmp = parse_dataclass(text, parsing[name])
+            _tmp["export"] = name
+            return _tmp
         except ParserError as e:
             log.error(e)
 
     log.error(f"'{name}': Export must be [{', '.join([s for s in parsing.keys()])}]")
 
 
 def edit_media(
     paths: list[str], ffmpeg: FFmpeg, args: Args, temp: str, log: Log
 ) -> None:
-
     timer = Timer(args.quiet)
     bar = Bar(args.progress)
     tl = None
 
     if paths:
         path_ext = os.path.splitext(paths[0])[1].lower()
         if path_ext == ".xml":
@@ -217,16 +204,17 @@
         else:
             sources, inputs = make_sources(paths, ffmpeg, log)
             src = None if not inputs else sources[str(inputs[0])]
 
     del paths
 
     output, export = set_output(args.output_file, args.export, src, log)
+    assert "export" in export
 
-    if isinstance(export, ExTimeline):
+    if export["export"] == "timeline":
         log.quiet = True
         timer.quiet = True
 
     if not args.preview:
         log.conwrite("Starting")
 
         if os.path.isdir(output):
@@ -256,45 +244,45 @@
                 cmd.extend([os.path.join(temp, f"{s}s.{sub.ext}")])
             ffmpeg.run(cmd)
 
         tl = make_timeline(
             sources, inputs, ffmpeg, ensure, args, samplerate, bar, temp, log
         )
 
-    if isinstance(export, ExTimeline):
+    if export["export"] == "timeline":
         from auto_editor.formats.json import make_json_timeline
 
-        make_json_timeline(export, 0, tl, log)
+        make_json_timeline(export["api"], 0, tl, log)
         return
 
     if args.preview:
         from auto_editor.preview import preview
 
         preview(ensure, tl, temp, log)
         return
 
-    if isinstance(export, ExJson):
+    if export["export"] == "json":
         from auto_editor.formats.json import make_json_timeline
 
-        make_json_timeline(export, output, tl, log)
+        make_json_timeline(export["api"], output, tl, log)
         return
 
-    if isinstance(export, ExPremiere):
+    if export["export"] == "premiere":
         from auto_editor.formats.premiere import premiere_write_xml
 
-        premiere_write_xml(export, ensure, output, tl)
+        premiere_write_xml(export["name"], ensure, output, tl)
         return
 
-    if isinstance(export, ExFinalCutPro):
+    if export["export"] == "final-cut-pro":
         from auto_editor.formats.final_cut_pro import fcp_xml
 
-        fcp_xml(export, output, tl)
+        fcp_xml(export["name"], output, tl)
         return
 
-    if isinstance(export, ExShotCut):
+    if export["export"] == "shotcut":
         from auto_editor.formats.shotcut import shotcut_write_mlt
 
         shotcut_write_mlt(output, tl)
         return
 
     out_ext = os.path.splitext(output)[1].replace(".", "")
 
@@ -350,15 +338,15 @@
             tl.tb,
             args,
             src,
             temp,
             log,
         )
 
-    if isinstance(export, ExClipSequence):
+    if export["export"] == "clip-sequence":
         if tl.v1 is None:
             log.error("Timeline to complex to use clip-sequence export")
 
         sources = {"0": tl.v1.source}
 
         from auto_editor.make_layers import clipify, make_av
         from auto_editor.utils.func import append_filename
@@ -391,15 +379,15 @@
             make_media(my_timeline, append_filename(output, f"-{clip_num}"))
             clip_num += 1
     else:
         make_media(tl, output)
 
     timer.stop()
 
-    if not args.no_open and isinstance(export, (ExDefault, ExAudio, ExClipSequence)):
+    if not args.no_open and export["export"] in ("default", "audio", "clip-sequence"):
         if args.player is None:
             from auto_editor.utils.func import open_with_system_default
 
             open_with_system_default(output, log)
         else:
             import subprocess
             from shlex import split
```

### Comparing `auto-editor-23.4.1/auto_editor/ffwrapper.py` & `auto-editor-23.8.1/auto_editor/ffwrapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,15 +80,14 @@
     def run_check_errors(
         self,
         cmd: list[str],
         log: Log,
         show_out: bool = False,
         path: str | None = None,
     ) -> None:
-
         process = self.Popen(cmd, stdin=PIPE, stdout=PIPE, stderr=PIPE)
         _, stderr = process.communicate()
 
         if process.stdin is not None:
             process.stdin.close()
         output = stderr.decode("utf-8", "replace")
 
@@ -151,14 +150,15 @@
     lang: str | None
 
 
 @dataclass
 class AudioStream:
     codec: str
     samplerate: int
+    channels: int
     duration: str | None
     bitrate: str | None
     lang: str | None
 
 
 @dataclass
 class SubtitleStream:
@@ -326,12 +326,17 @@
                         color_transfer,
                         br,
                         lang,
                     )
                 )
             if codec_type == "audio":
                 sr = int(stream["sample_rate"])
+
+                if "channels" not in stream:
+                    log.error("audio stream has no 'channels' data")
+                c = int(stream["channels"])
+
                 adur = get_attr("duration", stream, default=None)
-                self.audios.append(AudioStream(codec, sr, adur, br, lang))
+                self.audios.append(AudioStream(codec, sr, c, adur, br, lang))
             if codec_type == "subtitle":
                 ext = SUB_EXTS.get(codec, "vtt")
                 self.subtitles.append(SubtitleStream(codec, ext, lang))
```

### Comparing `auto-editor-23.4.1/auto_editor/formats/final_cut_pro.py` & `auto-editor-23.8.1/auto_editor/formats/final_cut_pro.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from __future__ import annotations
 
 from fractions import Fraction
-from typing import TYPE_CHECKING
 
 from auto_editor.ffwrapper import FileInfo
 from auto_editor.timeline import v3
 
 from .utils import indent
 
-if TYPE_CHECKING:
-    from auto_editor.objs.export import ExFinalCutPro
-
 """
 Export a FCPXML 9 file readable with Final Cut Pro 10.4.9 or later.
 
 See docs here:
 https://developer.apple.com/documentation/professional_video_applications/fcpxml_reference
 
 """
@@ -64,30 +60,30 @@
                 total += Fraction(1, 30)
             num = total.numerator
             dem = total.denominator
 
     return f"{num}/{dem}s"
 
 
-def fcp_xml(ex: ExFinalCutPro, output: str, tl: v3) -> None:
+def fcp_xml(_group_name: str | None, output: str, tl: v3) -> None:
     assert tl.v1 is not None
     src = tl.v1.source
     chunks = tl.v1.chunks
     tb = tl.tb
 
     total_dur = chunks[-1][1]
     pathurl = src.path.resolve().as_uri()
     width, height = tl.res
     name = src.path.stem
 
-    if ex.name is None:
+    if _group_name is None:
         is_audio = not src.videos and src.audios
         group_name = f"Auto-Editor {'Audio' if is_audio else 'Video'} Group"
     else:
-        group_name = ex.name
+        group_name = _group_name
 
     colorspace = get_colorspace(src)
 
     with open(output, "w", encoding="utf-8") as outfile:
         outfile.write('<?xml version="1.0" encoding="UTF-8"?>\n')
         outfile.write("<!DOCTYPE fcpxml>\n\n")
         outfile.write('<fcpxml version="1.9">\n')
```

### Comparing `auto-editor-23.4.1/auto_editor/formats/premiere.py` & `auto-editor-23.8.1/auto_editor/formats/premiere.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 from auto_editor.ffwrapper import FFmpeg, FileInfo
 from auto_editor.timeline import ASpace, TlAudio, TlVideo, VSpace, v3
 
 from .utils import Validator, safe_mkdir, show
 
 if TYPE_CHECKING:
-    from auto_editor.objs.export import ExPremiere
     from auto_editor.output import Ensure
     from auto_editor.utils.log import Log
 
 """
 Premiere Pro uses the Final Cut Pro 7 XML Interchange Format
 
 See docs here:
@@ -245,15 +244,15 @@
                 aobjs[t].append(
                     TlAudio(start, dur, file_id, offset, speed=1, volume=1, stream=0)
                 )
 
     return v3(sources, tb, sr, res, "#000", vobjs, aobjs, None)
 
 
-def premiere_write_xml(ex: ExPremiere, ensure: Ensure, output: str, tl: v3) -> None:
+def premiere_write_xml(_name: str | None, ensure: Ensure, output: str, tl: v3) -> None:
     assert tl.v1 is not None
 
     clips = list(filter(lambda c: c[2] != 99999, tl.v1.chunks))
     duration = tl.v1.chunks[-1][1]
 
     src = tl.v1.source
     width, height = tl.res
@@ -270,18 +269,18 @@
         safe_mkdir(fold)
 
         for i in range(1, tracks):
             newtrack = fold / f"{i}.wav"
             move(ensure.audio(f"{src.path.resolve()}", "0", i), newtrack)
             pathurls.append(newtrack.resolve().as_uri())
 
-    if ex.name is None:
+    if _name is None:
         name = f"Auto-Editor {'Audio' if audio_file else 'Video'} Group"
     else:
-        name = ex.name
+        name = _name
 
     xmeml = ET.Element("xmeml", version="4")
     sequence = ET.SubElement(xmeml, "sequence")
     ET.SubElement(sequence, "name").text = name
     ET.SubElement(sequence, "duration").text = str(duration)
     rate = ET.SubElement(sequence, "rate")
     ET.SubElement(rate, "timebase").text = str(timebase)
@@ -301,15 +300,14 @@
     ET.SubElement(vschar, "pixelaspectratio").text = PIXEL_ASPECT_RATIO
 
     if len(src.videos) > 0:
         track = ET.SubElement(video, "track")
 
         total = 0.0
         for j, clip in enumerate(clips):
-
             clip_duration = (clip[1] - clip[0]) / clip[2]
 
             _start = int(total)
             _end = int(total) + int(clip_duration)
             _in = int(clip[0] / clip[2])
             _out = int(clip[1] / clip[2])
 
@@ -378,15 +376,14 @@
     for t in range(tracks):
         track = ET.Element(
             "track", currentExplodedTrackIndex="0", premiereTrackType="Stereo"
         )
 
         total = 0
         for j, clip in enumerate(clips):
-
             clip_duration = (clip[1] - clip[0]) / clip[2]
 
             _start = int(total)
             _end = int(total) + int(clip_duration)
             _in = int(clip[0] / clip[2])
             _out = int(clip[1] / clip[2])
```

### Comparing `auto-editor-23.4.1/auto_editor/formats/shotcut.py` & `auto-editor-23.8.1/auto_editor/formats/shotcut.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 See docs here:
 https://mltframework.org/docs/mltxml/
 
 """
 
 
 def shotcut_read_mlt(path: str, ffmpeg: FFmpeg, log: Log) -> v3:
-    raise NotImplemented
+    raise NotImplementedError
 
 
 def shotcut_write_mlt(output: str, tl: v3) -> None:
     mlt = ET.Element(
         "mlt",
         attrib={
             "LC_NUMERIC": "C",
```

### Comparing `auto-editor-23.4.1/auto_editor/formats/utils.py` & `auto-editor-23.8.1/auto_editor/formats/utils.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/help.py` & `auto-editor-23.8.1/auto_editor/help.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/interpreter.py` & `auto-editor-23.8.1/auto_editor/interpreter.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,136 +1,152 @@
 from __future__ import annotations
 
 import cmath
 import math
 import random
 import sys
-from dataclasses import dataclass
+from difflib import get_close_matches
 from fractions import Fraction
 from functools import reduce
+from time import sleep
 from typing import TYPE_CHECKING
 
 import numpy as np
 
 from auto_editor.analyze import edit_method, mut_remove_small
+from auto_editor.lib.contracts import *
 from auto_editor.utils.func import boolop, mut_margin
 
 if TYPE_CHECKING:
     from typing import Any, Callable, Union
 
     from numpy.typing import NDArray
 
-    from auto_editor.ffwrapper import FileInfo
-    from auto_editor.output import Ensure
-    from auto_editor.utils.bar import Bar
-    from auto_editor.utils.log import Log
-
     Number = Union[int, float, complex, Fraction]
     Real = Union[int, float, Fraction]
     BoolList = NDArray[np.bool_]
+    Env = dict[str, Any]
 
 
 class MyError(Exception):
     pass
 
 
+class ClosingError(MyError):
+    pass
+
+
 def display_dtype(dtype: np.dtype) -> str:
     if dtype.kind == "b":
         return "bool"
 
     if dtype.kind == "i":
         return f"int{dtype.itemsize * 8}"
 
     if dtype.kind == "u":
         return f"uint{dtype.itemsize * 8}"
 
     return f"float{dtype.itemsize * 8}"
 
 
-class Null:
-    def __init__(self) -> None:
-        pass
+class NullType:
+    __slots__ = ()
+
+    def __new__(cls: type[NullType]) -> NullType:
+        return Null
 
     def __eq__(self, obj: object) -> bool:
-        return isinstance(obj, Null)
+        return obj is Null
 
     def __len__(self) -> int:
         return 0
 
     def __next__(self) -> StopIteration:
         raise StopIteration
 
     def __getitem__(self, ref: int | slice) -> None:
         raise IndexError
 
     def __str__(self) -> str:
         return "'()"
 
-    __repr__ = __str__
+    def __copy__(self) -> NullType:
+        return Null
 
+    def __deepcopy__(self, memo: Any) -> NullType:
+        return Null
 
-class PaletObject:
-    __slots__ = "attributes"
+    __repr__ = __str__
 
-    def __init__(self, attrs: dict[str, Any]):
-        self.attributes = attrs
+
+Null = object.__new__(NullType)
 
 
 class Cons:
     __slots__ = ("a", "d")
 
     def __init__(self, a: Any, d: Any):
         self.a = a
         self.d = d
 
     def __repr__(self) -> str:
-        if not isinstance(self.d, (Cons, Null)):
+        if type(self.d) not in (Cons, NullType):
             return f"(cons {self.a} {self.d})"
 
         result = f"({display_str(self.a)}"
         tail = self.d
-        while isinstance(tail, Cons):
-            if not isinstance(tail.d, (Null, Cons)):
+        while type(tail) is Cons:
+            if type(tail.d) not in (Cons, NullType):
                 return f"{result} (cons {tail.a} {tail.d}))"
             result += f" {display_str(tail.a)}"
             tail = tail.d
 
         return f"{result})"
 
     def __eq__(self, obj: object) -> bool:
-        return isinstance(obj, Cons) and self.a == obj.a and self.d == obj.d
+        return type(obj) is Cons and self.a == obj.a and self.d == obj.d
 
-    def __len__(self) -> int:
+    def __len__(self: Cons | NullType) -> int:
         count = 0
-        while isinstance(self, Cons):
+        while type(self) is Cons:
             self = self.d
             count += 1
-        if not isinstance(self, Null):
+        if self is not Null:
             raise MyError("length expects: list?")
         return count
 
     def __next__(self) -> Any:
-        if isinstance(self.d, Cons):
+        if type(self.d) is Cons:
             return self.d
         raise StopIteration
 
-    def __getitem__(self, ref: int | slice) -> Any:
-        if isinstance(ref, int):
+    def __iter__(self) -> Any:
+        while type(self) is Cons:
+            yield self.a
+            self = self.d
+
+    def __getitem__(self, ref: object) -> Any:
+        if type(ref) is not int and type(ref) is not slice:
+            raise MyError(f"ref: not a valid index: {print_str(ref)}")
+
+        if type(ref) is int:
             if ref < 0:
-                raise MyError(f"ref: negative index not allowed")
+                raise MyError(f"ref: negative index not allowed: {ref}")
             pos = ref
             while pos > 0:
                 pos -= 1
                 self = self.d
-                if not isinstance(self, Cons):
-                    raise MyError(f"ref: Index {ref} out of range")
+                if type(self) is not Cons:
+                    raise MyError(f"ref: index out of range: {ref}")
 
             return self.a
 
-        lst: Cons | Null = Null()
+        assert type(ref) is slice
+
+        lst: Cons | NullType = Null
         steps: int = -1
         i: int = 0
 
         do_reverse = True
         start, stop, step = ref.start, ref.stop, ref.step
         if start is None:
             start = 0
@@ -139,85 +155,84 @@
             step = -step
 
             if stop is None:
                 stop = float("inf")
             else:
                 start, stop = stop + 1, start
 
-        while isinstance(self, Cons):
+        while type(self) is Cons:
             if i > stop - 1:
                 break
             if i >= start:
                 steps = (steps + 1) % step
                 if steps == 0:
                     lst = Cons(self.a, lst)
 
             self = self.d
             i += 1
 
         if not do_reverse:
             return lst
 
-        result: Cons | Null = Null()
-        while isinstance(lst, Cons):
+        result: Cons | NullType = Null
+        while type(lst) is Cons:
             result = Cons(lst.a, result)
             lst = lst.d
         return result
 
 
 class Char:
     __slots__ = "val"
 
     def __init__(self, val: str | int):
-        if isinstance(val, int):
+        if type(val) is int:
             self.val: str = chr(val)
         else:
-            assert isinstance(val, str) and len(val) == 1
+            assert type(val) is str and len(val) == 1
             self.val = val
 
     __str__: Callable[[Char], str] = lambda self: self.val
 
     def __repr__(self) -> str:
         names = {" ": "space", "\n": "newline", "\t": "tab"}
         return f"#\\{self.val}" if self.val not in names else f"#\\{names[self.val]}"
 
     def __eq__(self, obj: object) -> bool:
-        return isinstance(obj, Char) and self.val == obj.val
+        return type(obj) is Char and self.val == obj.val
 
     def __radd__(self, obj2: str) -> str:
         return obj2 + self.val
 
 
-class Symbol:
+class Sym:
     __slots__ = ("val", "hash")
 
     def __init__(self, val: str):
         self.val = val
         self.hash = hash(val)
 
-    __str__: Callable[[Symbol], str] = lambda self: self.val
+    __str__: Callable[[Sym], str] = lambda self: self.val
     __repr__ = __str__
 
     def __hash__(self) -> int:
         return self.hash
 
     def __eq__(self, obj: object) -> bool:
-        return isinstance(obj, Symbol) and self.hash == obj.hash
+        return type(obj) is Sym and self.hash == obj.hash
 
 
 ###############################################################################
 #                                                                             #
 #  LEXER                                                                      #
 #                                                                             #
 ###############################################################################
 
-METHODS = ("audio", "motion", "pixeldiff", "subtitle", "none", "all")
 SEC_UNITS = ("s", "sec", "secs", "second", "seconds")
 ID, QUOTE, NUM, BOOL, STR, CHAR = "ID", "QUOTE", "NUM", "BOOL", "STR", "CHAR"
-ARR, SEC, DB, PER = "ARR", "SEC", "DB", "PER"
+METHOD, SEC, DB, PER = "METHOD", "SEC", "DB", "PER"
 LPAREN, RPAREN, LBRAC, RBRAC, LCUR, RCUR, EOF = "(", ")", "[", "]", "{", "}", "EOF"
 
 
 class Token:
     __slots__ = ("type", "value")
 
     def __init__(self, type: str, value: Any):
@@ -385,38 +400,36 @@
                 if self.char in "'`|\\":
                     has_illegal = True
                 self.advance()
 
             if has_illegal:
                 raise MyError(f"Symbol has illegal character(s): {result}")
 
-            for method in METHODS:
+            for method in ("audio", "motion", "pixeldiff", "subtitle", "none", "all"):
                 if result == method or result.startswith(method + ":"):
-                    return Token(ARR, result)
+                    return Token(METHOD, result)
 
             return Token(ID, result)
 
         return Token(EOF, "EOF")
 
 
 ###############################################################################
 #                                                                             #
 #  PARSER                                                                     #
 #                                                                             #
 ###############################################################################
 
 
-class BoolArr:
+class Method:
     __slots__ = "val"
 
     def __init__(self, val: str):
         self.val = val
 
-    __str__: Callable[[BoolArr], str] = lambda self: f"(boolarr {self.val})"
-
 
 class Parser:
     def __init__(self, lexer: Lexer):
         self.lexer = lexer
         self.current_token = self.lexer.get_next_token()
 
     def eat(self, token_type: str) -> None:
@@ -424,47 +437,50 @@
             raise MyError(f"Expected {token_type}, got {self.current_token.type}")
 
         self.current_token = self.lexer.get_next_token()
 
     def expr(self) -> Any:
         token = self.current_token
 
-        if token.type in {CHAR, NUM, STR, BOOL}:
+        if token.type in (CHAR, NUM, STR, BOOL):
             self.eat(token.type)
             return token.value
 
-        matches = {ID: Symbol, ARR: BoolArr}
-        if token.type in matches:
-            self.eat(token.type)
-            return matches[token.type](token.value)
+        if token.type == ID:
+            self.eat(ID)
+            return Sym(token.value)
+
+        if token.type == METHOD:
+            self.eat(METHOD)
+            return Method(token.value)
 
         if token.type == SEC:
             self.eat(SEC)
-            return [Symbol("round"), [Symbol("*"), token.value, Symbol("timebase")]]
+            return [Sym("round"), [Sym("*"), token.value, Sym("timebase")]]
 
         if token.type == DB:
             self.eat(DB)
-            return [Symbol("pow"), 10, [Symbol("/"), token.value, 20]]
+            return [Sym("pow"), 10, [Sym("/"), token.value, 20]]
 
         if token.type == PER:
             self.eat(PER)
-            return [Symbol("/"), token.value, 100.0]
+            return [Sym("/"), token.value, 100.0]
 
         if token.type == QUOTE:
             self.eat(QUOTE)
-            return [Symbol("quote"), self.expr()]
+            return [Sym("quote"), self.expr()]
 
         pars = {LPAREN: RPAREN, LBRAC: RBRAC, LCUR: RCUR}
         if token.type in pars:
             self.eat(token.type)
             closing = pars[token.type]
             childs = []
             while self.current_token.type != closing:
                 if self.current_token.type == EOF:
-                    raise MyError(f"Expected closing '{closing}' before end")
+                    raise ClosingError(f"Expected closing '{closing}' before end")
                 childs.append(self.expr())
 
             self.eat(closing)
             return childs
 
         self.eat(token.type)
         childs = []
@@ -485,172 +501,161 @@
 ###############################################################################
 #                                                                             #
 #  STANDARD LIBRARY                                                           #
 #                                                                             #
 ###############################################################################
 
 
-class Contract:
-    # Convenient flat contract class
-    __slots__ = ("name", "c")
-
-    def __init__(self, name: str, c: Callable[[object], bool]):
-        self.name = name
-        self.c = c
-
-    def __str__(self) -> str:
-        return f"<procedure:{self.name}>"
-
-    __repr__ = __str__
-
-    def __call__(self, v: object) -> bool:
-        return self.c(v)
+def check_contract(c: object, val: object) -> bool:
+    if isinstance(c, Contract):
+        return c(val)
+    if (
+        isinstance(c, Proc)
+        and c.arity[0] < 2
+        and (c.arity[1] is None or c.arity[1] > 0)
+    ):
+        return c(val)
+    if c is True:
+        return val is True
+    if c is False:
+        return val is False
+    if c is Null:
+        return val is Null
+
+    if type(c) is int:
+        return val == c
+    if type(c) in (int, float, Fraction, complex, str, Sym):
+        return val == c
+    raise MyError(f"Invalid contract, got: {print_str(c)}")
+
+
+def is_contract(c: object) -> bool:
+    if isinstance(c, Contract):
+        return True
+    if (
+        isinstance(c, Proc)
+        and c.arity[0] < 2
+        and (c.arity[1] is None or c.arity[1] > 0)
+    ):
+        return True
+    if c is True or c is False or c is Null:
+        return True
+    return type(c) in (int, float, Fraction, complex, str, Sym)
 
 
 def check_args(
     o: str,
     values: list | tuple,
     arity: tuple[int, int | None],
-    types: list[Contract] | None,
+    cont: list[Contract] | None,
 ) -> None:
     lower, upper = arity
     amount = len(values)
     if upper is not None and lower > upper:
         raise ValueError("lower must be less than upper")
-    if lower == upper:
-        if len(values) != lower:
-            raise MyError(f"{o}: Arity mismatch. Expected {lower}, got {amount}")
+    if lower == upper and len(values) != lower:
+        raise MyError(f"{o}: Arity mismatch. Expected {lower}, got {amount}")
 
     if upper is None and amount < lower:
         raise MyError(f"{o}: Arity mismatch. Expected at least {lower}, got {amount}")
     if upper is not None and (amount > upper or amount < lower):
         raise MyError(
             f"{o}: Arity mismatch. Expected between {lower} and {upper}, got {amount}"
         )
 
-    if types is None:
+    if cont is None:
         return
 
     for i, val in enumerate(values):
-        check = types[-1] if i >= len(types) else types[i]
-        if not check(val):
-            raise MyError(f"{o} expects: {' '.join([c.name for c in types])}")
+        check = cont[-1] if i >= len(cont) else cont[i]
+        if not check_contract(check, val):
+            raise MyError(f"{o} expected a {check.name}, got {print_str(val)}")
 
 
-any_p = Contract("any_p", lambda v: True)
 is_proc = Contract("procedure?", lambda v: isinstance(v, (Proc, Contract)))
-is_bool = Contract("boolean?", lambda v: isinstance(v, bool))
-is_pair = Contract("pair?", lambda v: isinstance(v, Cons))
-is_null = Contract("null?", lambda v: isinstance(v, Null))
-is_symbol = Contract("symbol?", lambda v: isinstance(v, Symbol))
-is_str = Contract("string?", lambda v: isinstance(v, str))
-is_char = Contract("char?", lambda v: isinstance(v, Char))
+is_cont = Contract("contract?", is_contract)
 is_iterable = Contract(
     "iterable?",
-    lambda v: isinstance(v, (str, list, dict, range, np.ndarray, Cons, Null)),
+    lambda v: v is Null
+    or type(v) in (str, range, Cons)
+    or isinstance(v, (list, dict, np.ndarray)),
 )
 is_sequence = Contract(
     "sequence?",
-    lambda v: isinstance(v, (str, list, range, np.ndarray, Cons, Null)),
+    lambda v: v is Null
+    or type(v) in (str, range, Cons)
+    or isinstance(v, (list, np.ndarray)),
 )
-is_range = Contract("range?", lambda v: isinstance(v, range))
-is_vector = Contract("vector?", lambda v: isinstance(v, list))
-is_array = Contract("array?", lambda v: isinstance(v, np.ndarray))
 is_boolarr = Contract(
     "bool-array?",
     lambda v: isinstance(v, np.ndarray) and v.dtype.kind == "b",
 )
-is_num = Contract(
-    "number?",
-    lambda v: not isinstance(v, bool)
-    and isinstance(v, (int, float, Fraction, complex)),
+bool_or_barr = Contract(
+    "(or/c bool? bool-array?)",
+    lambda v: type(v) is bool or is_boolarr(v),
 )
-is_real = Contract(
-    "real?", lambda v: not isinstance(v, bool) and isinstance(v, (int, float, Fraction))
-)
-is_int = Contract(
-    "integer?",
-    lambda v: not isinstance(v, bool) and isinstance(v, int),
-)
-is_frac = Contract("fraction?", lambda v: isinstance(v, Fraction))
-is_float = Contract("float?", lambda v: isinstance(v, float))
-us_int = Contract("nonnegative-integer?", lambda v: isinstance(v, int) and v > -1)
-is_hash = Contract("hash?", lambda v: isinstance(v, dict))
-is_void = Contract("void?", lambda v: v is None)
 
 
 def raise_(msg: str) -> None:
     raise MyError(msg)
 
 
 def display_str(val: object) -> str:
     if val is None:
-        return ""
+        return "#<void>"
     if val is True:
         return "#t"
     if val is False:
         return "#f"
-    if isinstance(val, Symbol):
+    if type(val) is Sym:
         return val.val
-    if isinstance(val, str):
+    if type(val) is str:
         return val
+    if type(val) is Char:
+        return f"{val}"
+    if type(val) is range:
+        return "#<range>"
+    if type(val) is complex:
+        join = "" if val.imag < 0 else "+"
+        return f"{val.real}{join}{val.imag}i"
+
     if isinstance(val, Fraction):
         return f"{val.numerator}/{val.denominator}"
-    if isinstance(val, Symbol):
-        return val.val
     if isinstance(val, list):
         if not val:
             return "#()"
         result = f"#({display_str(val[0])}"
         for item in val[1:]:
             result += f" {display_str(item)}"
         return result + ")"
-    if isinstance(val, range):
-        return "#<range>"
     if isinstance(val, np.ndarray):
         kind = val.dtype.kind
         result = f"(array '{display_dtype(val.dtype)}"
         if kind == "b":
             for item in val:
                 result += " 1" if item else " 0"
         else:
             for item in val:
                 result += f" {item}"
         return result + ")"
-    if isinstance(val, complex):
-        join = "" if val.imag < 0 else "+"
-        return f"{val.real}{join}{val.imag}i"
 
     return f"{val!r}"
 
 
 def print_str(val: object) -> str:
-    if isinstance(val, (Symbol, list, Cons)):
-        return "'" + display_str(val)
-    if isinstance(val, str):
+    if type(val) is str:
         return f'"{val}"'
+    if type(val) is Char:
+        return f"{val!r}"
+    if type(val) is Sym or type(val) is Cons or isinstance(val, list):
+        return f"'{display_str(val)}"
 
     return display_str(val)
 
 
-def display(val: Any) -> None:
-    if result := display_str(val):
-        sys.stdout.write(result)
-
-
-def displayln(val: Any) -> None:
-    if result := display_str(val):
-        sys.stdout.write(result + "\n")
-
-
-def palet_print(val: Any) -> None:
-    if result := print_str(val):
-        sys.stdout.write(result)
-
-
 def is_equal(a: object, b: object) -> bool:
     if isinstance(a, np.ndarray) and isinstance(b, np.ndarray):
         return np.array_equal(a, b)
     return type(a) == type(b) and a == b
 
 
 def equal_num(*values: object) -> bool:
@@ -684,38 +689,14 @@
     if r.imag == 0:
         if int(r.real) == r.real:
             return int(r.real)
         return r.real
     return r
 
 
-def _not(val: Any) -> bool | BoolList:
-    if is_boolarr(val):
-        return np.logical_not(val)
-    if is_bool(val):
-        return not val
-    raise MyError("not expects: boolean? or bool-array?")
-
-
-def _and(*vals: Any) -> bool | BoolList:
-    if is_boolarr(vals[0]):
-        check_args("and", vals, (2, None), [is_boolarr])
-        return reduce(lambda a, b: boolop(a, b, np.logical_and), vals)
-    check_args("and", vals, (1, None), [is_bool])
-    return reduce(lambda a, b: a and b, vals)
-
-
-def _or(*vals: Any) -> bool | BoolList:
-    if is_boolarr(vals[0]):
-        check_args("or", vals, (2, None), [is_boolarr])
-        return reduce(lambda a, b: boolop(a, b, np.logical_or), vals)
-    check_args("or", vals, (1, None), [is_bool])
-    return reduce(lambda a, b: a or b, vals)
-
-
 def _xor(*vals: Any) -> bool | BoolList:
     if is_boolarr(vals[0]):
         check_args("xor", vals, (2, None), [is_boolarr])
         return reduce(lambda a, b: boolop(a, b, np.logical_xor), vals)
     check_args("xor", vals, (2, None), [is_bool])
     return reduce(lambda a, b: a ^ b, vals)
 
@@ -739,43 +720,43 @@
     if isinstance(val, complex):
         join = "" if val.imag < 0 else "+"
         return f"{val.real}{join}{val.imag}i"
     return f"{val}"
 
 
 dtype_map = {
-    Symbol("bool"): np.bool_,
-    Symbol("int8"): np.int8,
-    Symbol("int16"): np.int16,
-    Symbol("int32"): np.int32,
-    Symbol("int64"): np.int64,
-    Symbol("uint8"): np.uint8,
-    Symbol("uint16"): np.uint16,
-    Symbol("uint32"): np.uint32,
-    Symbol("uint64"): np.uint64,
-    Symbol("float32"): np.float32,
-    Symbol("float64"): np.float64,
+    Sym("bool"): np.bool_,
+    Sym("int8"): np.int8,
+    Sym("int16"): np.int16,
+    Sym("int32"): np.int32,
+    Sym("int64"): np.int64,
+    Sym("uint8"): np.uint8,
+    Sym("uint16"): np.uint16,
+    Sym("uint32"): np.uint32,
+    Sym("uint64"): np.uint64,
+    Sym("float32"): np.float32,
+    Sym("float64"): np.float64,
 }
 
 
-def _dtype_to_np(dtype: Symbol) -> type[np.generic]:
+def _dtype_to_np(dtype: Sym) -> type[np.generic]:
     np_dtype = dtype_map.get(dtype)
     if np_dtype is None:
         raise MyError(f"Invalid array dtype: {dtype}")
     return np_dtype
 
 
-def array_proc(dtype: Symbol, *vals: Any) -> np.ndarray:
+def array_proc(dtype: Sym, *vals: Any) -> np.ndarray:
     try:
         return np.array(vals, dtype=_dtype_to_np(dtype))
     except OverflowError:
         raise MyError(f"number too large to be converted to {dtype}")
 
 
-def make_array(dtype: Symbol, size: int, v: int = 0) -> np.ndarray:
+def make_array(dtype: Sym, size: int, v: int = 0) -> np.ndarray:
     try:
         return np.array([v] * size, dtype=_dtype_to_np(dtype))
     except OverflowError:
         raise MyError(f"number too large to be converted to {dtype}")
 
 
 def minclip(oarr: BoolList, _min: int) -> BoolList:
@@ -801,41 +782,41 @@
         start, end = a, b
 
     arr = np.copy(oarr)
     mut_margin(arr, start, end)
     return arr
 
 
-def _list(*values: Any) -> Cons | Null:
-    result: Cons | Null = Null()
+def _list(*values: Any) -> Cons | NullType:
+    result: Cons | NullType = Null
     for val in reversed(values):
         result = Cons(val, result)
     return result
 
 
 # convert nested vectors to nested lists
-def deep_list(vec: list) -> Cons | Null:
-    result: Cons | Null = Null()
+def deep_list(vec: list) -> Cons | NullType:
+    result: Cons | NullType = Null
     for val in reversed(vec):
         if isinstance(val, list):
             val = deep_list(val)
         result = Cons(val, result)
     return result
 
 
-def list_to_vector(val: Cons | Null) -> list:
+def list_to_vector(val: Cons | NullType) -> list:
     result = []
-    while isinstance(val, Cons):
+    while type(val) is Cons:
         result.append(val.a)
         val = val.d
     return result
 
 
-def vector_to_list(values: list) -> Cons | Null:
-    result: Cons | Null = Null()
+def vec_to_list(values: list) -> Cons | NullType:
+    result: Cons | NullType = Null
     for val in reversed(values):
         result = Cons(val, result)
     return result
 
 
 def vector_set(vec: list, pos: int, v: Any) -> None:
     try:
@@ -845,73 +826,63 @@
 
 
 def vector_extend(vec: list, *more_vecs: list) -> None:
     for more in more_vecs:
         vec.extend(more)
 
 
-def string_to_list(s: str) -> Cons | Null:
-    return vector_to_list([Char(s) for s in s])
-
-
 def is_list(val: Any) -> bool:
-    while isinstance(val, Cons):
+    while type(val) is Cons:
         val = val.d
-    return isinstance(val, Null)
-
+    return val is Null
 
-def palet_random(*args: int) -> int | float:
-    if not args:
-        return random.random()
 
-    if args[0] < 1:
-        raise MyError(f"random: arg1 ({args[0]}) must be greater than zero")
-
-    if len(args) == 1:
-        return random.randrange(0, args[0])
-
-    if args[0] >= args[1]:
-        raise MyError(f"random: arg2 ({args[1]}) must be greater than arg1")
-    return random.randrange(args[0], args[1])
+def randrange(*args: int) -> int:
+    try:
+        return random.randrange(*args)
+    except ValueError:
+        raise MyError("randrange: got empty range")
 
 
-def palet_map(proc: Proc, seq: str | list | range | NDArray | Cons | Null) -> Any:
+def palet_map(proc: Proc, seq: str | list | range | NDArray | Cons | NullType) -> Any:
+    if type(seq) is str:
+        return str(map(proc.proc, seq))
     if isinstance(seq, (list, range)):
         return list(map(proc.proc, seq))
-    if isinstance(seq, str):
-        return str(map(proc.proc, seq))
 
     if isinstance(seq, np.ndarray):
         if proc.arity[0] != 0:
-            raise MyError(f"map: procedure must take at least one arg")
+            raise MyError("map: procedure must take at least one arg")
         check_args(proc.name, [0], (1, 1), None)
         return proc.proc(seq)
 
-    result: Cons | Null = Null()
-    while isinstance(seq, Cons):
+    result: Cons | NullType = Null
+    while type(seq) is Cons:
         result = Cons(proc.proc(seq.a), result)
         seq = seq.d
     return result[::-1]
 
 
-def apply(proc: Proc, seq: str | list | range | Cons | Null) -> Any:
-    if isinstance(seq, (Cons, Null)):
+def apply(proc: Proc, seq: str | list | range | Cons | NullType) -> Any:
+    if isinstance(seq, (Cons, NullType)):
         return reduce(proc.proc, list_to_vector(seq))
     return reduce(proc.proc, seq)
 
 
 def ref(seq: Any, ref: int) -> Any:
     try:
-        return Char(seq[ref]) if isinstance(seq, str) else seq[ref]
+        return Char(seq[ref]) if type(seq) is str else seq[ref]
+    except KeyError:
+        raise MyError(f"ref: Invalid key: {print_str(ref)}")
     except IndexError:
-        raise MyError(f"ref: Invalid index {ref}")
+        raise MyError(f"ref: Invalid index: {print_str(ref)}")
 
 
 def p_slice(
-    seq: str | list | range | NDArray | Cons | Null,
+    seq: str | list | range | NDArray | Cons | NullType,
     start: int = 0,
     end: int | None = None,
     step: int = 1,
 ) -> Any:
     if end is None:
         end = len(seq)
 
@@ -920,123 +891,663 @@
 
 def splice(
     arr: NDArray, v: int, start: int | None = None, end: int | None = None
 ) -> None:
     arr[start:end] = v
 
 
-def stream_to_list(s: range) -> Cons | Null:
-    result: Cons | Null = Null()
+def stream_to_list(s: range) -> Cons | NullType:
+    result: Cons | NullType = Null
     for item in reversed(s):
         result = Cons(item, result)
     return result
 
 
 def palet_hash(*args: Any) -> dict:
     result = {}
     if len(args) % 2 == 1:
         raise MyError("hash: number of args must be even")
     for key, item in zip(args[0::2], args[1::2]):
         result[key] = item
     return result
 
 
+def andc(*cs: object) -> Proc:
+    return Proc(
+        "flat-and/c", lambda v: all([check_contract(c, v) for c in cs]), (1, 1), [any_p]
+    )
+
+
+def orc(*cs: object) -> Proc:
+    return Proc(
+        "flat-or/c", lambda v: any([check_contract(c, v) for c in cs]), (1, 1), [any_p]
+    )
+
+
+def notc(c: object) -> Proc:
+    return Proc("flat-not/c", lambda v: not check_contract(c, v), (1, 1), [any_p])
+
+
 ###############################################################################
 #                                                                             #
 #  ENVIRONMENT                                                                #
 #                                                                             #
 ###############################################################################
 
 
-@dataclass
 class Proc:
-    name: str
-    proc: Callable
-    arity: tuple[int, int | None] = (1, None)
-    contracts: list[Any] | None = None
+    __slots__ = ("name", "proc", "arity", "contracts")
+
+    def __init__(
+        self,
+        name: str,
+        proc: Callable,
+        arity: tuple[int, int | None] = (1, None),
+        contracts: list[Any] | None = None,
+    ):
+        self.name = name
+        self.proc = proc
+        self.arity = arity
+        self.contracts = contracts
 
     def __str__(self) -> str:
         return f"#<procedure:{self.name}>"
 
     __repr__ = __str__
 
-    def __call__(self, *vals: Any) -> Any:
-        return self.proc(*vals)
+    def __call__(self, *args: Any) -> Any:
+        return self.proc(*args)
 
 
-class UserProc:
+class UserProc(Proc):
     """A user-defined procedure."""
 
+    __slots__ = ("parms", "body", "name", "arity", "contracts")
+
     def __init__(
-        self, name: str, env: dict[str, Any], visit_f: Any, parms: list, body: list
+        self,
+        name: str,
+        parms: list,
+        body: list,
+        contracts: list[Any] | None = None,
+        eat_last: bool = False,
     ):
-        self.visit_f = visit_f
         self.parms = list(map(str, parms))
         self.body = body
-        self.env = env
-
         self.name = name
-        self.arity = len(parms), len(parms)
-        self.contracts = None
 
-    def __str__(self) -> str:
-        return f"#<procedure:{self.name}>"
+        if eat_last:
+            self.arity: tuple[int, int | None] = len(parms) - 1, None
+        else:
+            self.arity = len(parms), len(parms)
 
-    __repr__ = __str__
+        self.contracts = contracts
 
     def __call__(self, *args: Any) -> Any:
-        self.env.update(zip(self.parms, args))
-        return self.visit_f(self.body[-1])
+        saved_env: Env = {}
+        for item in self.parms:
+            if item in env:
+                saved_env[item] = env[item]
+
+        if self.arity[1] is None:
+            largs = list(args)
+            args = tuple([largs[len(self.parms) - 1 :]])
+
+        env.update(zip(self.parms, args))
+        for item in self.body[0:-1]:
+            my_eval(env, item)
+        result = my_eval(env, self.body[-1])
+
+        for item in self.parms:
+            del env[item]
+        env.update(saved_env)
+        return result
+
+
+class Syntax:
+    __slots__ = "syn"
+
+    def __init__(self, syn: Callable[[Env, list], Any]):
+        self.syn = syn
+
+    def __call__(self, env: Env, node: list) -> Any:
+        return self.syn(env, node)
+
+    __str__: Callable[[Syntax], str] = lambda self: "#<syntax>"
+    __repr__ = __str__
+
+
+def check_for_syntax(env: Env, node: list) -> Any:
+    name = node[0]
+    if len(node) < 2:
+        raise MyError(f"{name}: bad syntax")
+
+    if len(node) == 2:
+        raise MyError(f"{name}: missing body")
+
+    assert isinstance(node[1], list)
+    assert isinstance(node[1][0], list)
+
+    var = node[1][0][0]
+    if type(var) is not Sym:
+        raise MyError(f"{name}: binding must be an identifier")
+    my_iter = my_eval(env, node[1][0][1])
+
+    if not is_iterable(my_iter):
+        if type(my_iter) is int:
+            return var, range(my_iter)
+        raise MyError(f"{name}: got non-iterable in iter slot")
+
+    return var, my_iter
+
+
+def syn_lambda(env: Env, node: list) -> Any:
+    if not isinstance(node[1], list):
+        raise MyError(f"{node[0]}: bad syntax")
+
+    return UserProc("", node[1], node[2:])  # parms, body
+
+
+def syn_define(env: Env, node: list) -> Any:
+    if len(node) < 3:
+        raise MyError(f"{node[0]}: too few args")
+
+    if isinstance(node[1], list):
+        if not node[1] or type(node[1][0]) is not Sym:
+            raise MyError(f"{node[0]}: proc-binding must be an identifier")
+
+        n = node[1][0].val
+
+        eat_last = False
+        if node[1][1:] and node[1][-1] == Sym("..."):
+            eat_last = True
+            parameters = node[1][1:-1]
+        else:
+            parameters = node[1][1:]
+
+        body = node[2:]
+        env[n] = UserProc(n, parameters, body, eat_last=eat_last)
+        return None
+    elif type(node[1]) is not Sym:
+        raise MyError(f"{node[0]}: must be an identifier")
+
+    n = node[1].val
+
+    if len(node) > 3:
+        raise MyError(f"{node[0]}: bad syntax (multiple expressions after identifier)")
+
+    if (
+        isinstance(node[2], list)
+        and node[2]
+        and type(node[2][0]) is Sym
+        and node[2][0].val in ("lambda", "λ")
+    ):
+        parameters = node[2][1]
+        body = node[2][2:]
+        env[n] = UserProc(n, parameters, body)
+    else:
+        for item in node[2:-1]:
+            my_eval(env, item)
+        env[n] = my_eval(env, node[-1])
+
+    return None
+
+
+def syn_definec(env: Env, node: list) -> Any:
+    if len(node) < 3:
+        raise MyError(f"{node[0]}: bad syntax")
+
+    if not isinstance(node[1], list):
+        raise MyError(f"{node[0]} only allows procedure declarations")
+
+    if not node[1] or type(node[1][0]) is not Sym:
+        raise MyError(f"{node[0]}: bad proc-binding syntax")
+
+    n = node[1][0].val
+
+    contracts: list[Proc | Contract] = []
+    parameters: list[Sym] = []
+    for item in node[1][1:]:
+        if len(item) != 2:
+            raise MyError(f"{node[0]}: bad var-binding syntax")
+        if type(item[0]) is not Sym:
+            raise MyError(f"{node[0]}: binding must be identifier")
+
+        parameters.append(item[0])
+        con = my_eval(env, item[1])
+        if not is_cont(con):
+            raise MyError(f"{node[0]}: {print_str(con)} is not a valid contract")
+
+        contracts.append(con)
+
+    env[n] = UserProc(n, parameters, node[2:], contracts)
+    return None
+
+
+def syn_set(env: Env, node: list) -> None:
+    if len(node) != 3:
+        raise MyError(f"{node[0]}: bad syntax")
+    if type(node[1]) is not Sym:
+        raise MyError(f"{node[0]}: must be an identifier")
+
+    name = node[1].val
+    if name not in env:
+        raise MyError(f"{node[0]}: cannot set variable {name} before definition")
+    env[name] = my_eval(env, node[2])
+    return None
+
+
+def syn_for(env: Env, node: list) -> None:
+    var, my_iter = check_for_syntax(env, node)
+
+    for item in my_iter:
+        env[var.val] = item
+        for c in node[2:]:
+            my_eval(env, c)
 
+    return None
 
-env: dict[str, Any] = {
+
+def syn_for_vec(env: Env, node: list) -> list:
+    results = []
+    var, my_iter = check_for_syntax(env, node)
+
+    for item in my_iter:
+        env[var.val] = item
+        results.append([my_eval(env, c) for c in node[2:]][-1])
+
+    return results
+
+
+def syn_if(env: Env, node: list) -> Any:
+    if len(node) != 4:
+        raise MyError(f"{node[0]}: bad syntax")
+    test_expr = my_eval(env, node[1])
+
+    if type(test_expr) is not bool:
+        raise MyError(f"{node[0]}: test-expr arg must be: bool?")
+
+    return my_eval(env, node[2] if test_expr else node[3])
+
+
+def syn_when(env: Env, node: list) -> Any:
+    if len(node) != 3:
+        raise MyError(f"{node[0]}: bad syntax")
+    test_expr = my_eval(env, node[1])
+
+    if type(test_expr) is not bool:
+        raise MyError(f"{node[0]}: test-expr arg must be: bool?")
+
+    return my_eval(env, node[2]) if test_expr else None
+
+
+def syn_cond(env: Env, node: list) -> Any:
+    for test_expr in node[1:]:
+        if not isinstance(test_expr, list) or not test_expr:
+            raise MyError(f"{node[0]}: bad syntax, clause is not a test-value pair")
+
+        if test_expr[0] == Sym("else"):
+            if len(test_expr) == 1:
+                raise MyError(f"{node[0]}: missing expression in else clause")
+            test_clause = True
+        else:
+            test_clause = my_eval(env, test_expr[0])
+            if type(test_clause) is not bool:
+                raise MyError(f"{node[0]}: test-expr must be: bool?")
+
+        if test_clause:
+            if len(test_expr) == 1:
+                return True
+
+            for rest_clause in test_expr[1:-1]:
+                my_eval(env, rest_clause)
+            return my_eval(env, test_expr[-1])
+
+    return None
+
+
+def syn_quote(env: Env, node: list) -> Any:
+    if len(node) != 2:
+        raise MyError("quote: bad syntax")
+
+    if isinstance(node[1], list):
+        return deep_list(node[1])
+    return node[1]
+
+
+def syn_and(env: Env, node: list) -> Any:
+    if len(node) == 1:
+        raise MyError(f"{node[0]}: Arity mismatch: Expected 1. got 0")
+
+    first = my_eval(env, node[1])
+    if first is False:
+        return False
+    if first is True:
+        for n in node[2:]:
+            val = my_eval(env, n)
+            if val is False:
+                return False
+            if val is not True:
+                raise MyError(f"{node[0]} args must be bool?")
+        return True
+
+    if is_boolarr(first):
+        vals = [first] + [my_eval(env, n) for n in node[2:]]
+        check_args(node[0], vals, (2, None), [is_boolarr])
+        return reduce(lambda a, b: boolop(a, b, np.logical_and), vals)
+
+    raise MyError(f"{node[0]} expects (or/c bool? bool-array?)")
+
+
+def syn_or(env: Env, node: list) -> Any:
+    if len(node) == 1:
+        raise MyError(f"{node[0]}: Arity mismatch: Expected 1. got 0")
+
+    first = my_eval(env, node[1])
+    if first is True:
+        return True
+    if first is False:
+        for n in node[2:]:
+            val = my_eval(env, n)
+            if val is True:
+                return True
+            if val is not False:
+                raise MyError(f"{node[0]} args must be bool?")
+        return False
+
+    if is_boolarr(first):
+        vals = [first] + [my_eval(env, n) for n in node[2:]]
+        check_args(node[0], vals, (2, None), [is_boolarr])
+        return reduce(lambda a, b: boolop(a, b, np.logical_or), vals)
+
+    raise MyError(f"{node[0]} expects (or/c bool? bool-array?)")
+
+
+def syn_with_open(env: Env, node: list) -> None:
+    if len(node) < 2:
+        raise MyError(f"{node[0]} has too few args")
+    if len(node[1]) != 2 and len(node[1]) != 3:
+        raise MyError(f"{node[0]} has too many args")
+
+    if type(node[1][0]) is not Sym:
+        raise MyError(f'{node[0]}\'s "as" must be an identifier')
+
+    file_binding = node[1][0].val
+
+    file_name = my_eval(env, node[1][1])
+    if type(file_name) is not str:
+        raise MyError(f"{node[0]} file-name must be string?")
+
+    if len(node[1]) == 3:
+        file_mode = my_eval(env, node[1][2])
+        if type(file_mode) is not Sym:
+            raise MyError(f"{node[0]} file-mode must be symbol?")
+        if file_mode.val not in ("w", "r", "a"):
+            raise MyError(f"{node[0]} file-mode must be (or/c 'w 'r 'a)")
+    else:
+        file_mode = Sym("w")
+
+    with open(file_name, file_mode.val) as file:
+        if file_mode.val == "r":
+            open_file = PaletObject(
+                {
+                    "read": Proc("read", file.read, (0, 0)),
+                    "readlines": Proc("readlines", file.readlines, (0, 0)),
+                }
+            )
+        else:
+            open_file = PaletObject(
+                {"write": Proc("write", file.write, (1, 1), [is_str])}
+            )
+
+        env[file_binding] = open_file
+        for c in node[2:]:
+            my_eval(env, c)
+
+    del env[file_binding]
+    return None
+
+
+class PaletObject:
+    __slots__ = "attributes"
+
+    def __init__(self, attrs: dict[str, Any]):
+        self.attributes = attrs
+
+
+is_obj = Contract(
+    "object?",
+    lambda v: type(v) is str or isinstance(v, (list, Proc, PaletObject)),
+)
+
+
+def get_attrs(obj: object) -> dict[str, Any]:
+    if isinstance(obj, str):
+        return {
+            "split": Proc("split", obj.split, (0, 1)),
+            "strip": Proc("strip", obj.strip, (0, 0)),
+            "repeat": Proc("repeat", lambda a: obj * a, (1, 1), [is_int]),
+            "startswith": Proc("startswith", obj.startswith, (1, 1), [is_str]),
+            "endswith": Proc("endswith", obj.endswith, (1, 1), [is_str]),
+            "replace": Proc("replace", obj.replace, (1, 2), [is_str, is_int]),
+            "@len": Proc("@len", obj.__len__, (0, 0)),
+            "@name": "string",
+        }
+    if isinstance(obj, list):
+
+        def _join(s: str) -> str:
+            try:
+                assert isinstance(obj, list)
+                return s.join(obj)
+            except TypeError:
+                raise MyError("join: every item must be a string")
+
+        return {
+            "repeat": Proc("repeat", lambda a: obj * a, (1, 1), [is_int]),
+            "pop": Proc("pop", obj.pop, (0, 0)),
+            "join": Proc("join", _join, (1, 1), [is_str]),
+            "sort": Proc("sort", obj.sort, (0, 0)),
+            "@len": Proc("@len", obj.__len__, (0, 0)),
+            "@name": "vector",
+        }
+    if isinstance(obj, Proc):
+        return {
+            "arity-min": obj.arity[0],
+            "arity-max": obj.arity[1],
+            "name": obj.name,
+            "@name": "procedure",
+        }
+    if isinstance(obj, Contract):
+        return {
+            "arity-min": 1,
+            "arity-max": 1,
+            "name": obj.name,
+            "@name": "procedure",
+        }
+    if isinstance(obj, PaletObject):
+        return obj.attributes
+    raise MyError("")
+
+
+def syn_dot(env: Env, node: list) -> Any:
+    if len(node) != 3:
+        raise MyError(".: not enough args")
+
+    if not isinstance(node[2], Sym):
+        raise MyError(".: attribute must be an identifier")
+    my_attr = node[2].val
+    my_obj = my_eval(env, node[1])
+
+    try:
+        attrs = get_attrs(my_obj)
+    except MyError:
+        raise MyError(f".: expected an object, got {print_str(my_obj)}")
+    if my_attr not in attrs:
+        if mat := get_close_matches(my_attr, attrs):
+            raise MyError(f".: No such attribute: '{my_attr}'. Did you mean: {mat[0]}")
+        raise MyError(f".: No such attribute: '{my_attr}'")
+    return attrs[my_attr]
+
+
+def my_eval(env: Env, node: object) -> Any:
+    if type(node) is Sym:
+        val = env.get(node.val)
+        if val is None:
+            if mat := get_close_matches(node.val, env):
+                raise MyError(f"'{node.val}' not found. Did you mean: {mat[0]}")
+            raise MyError(f"'{node.val}' not found.")
+        return val
+
+    if isinstance(node, Method):
+        if "@filesetup" not in env:
+            raise MyError("Can't use edit methods if there's no input files")
+        return edit_method(node.val, env["@filesetup"])
+
+    if isinstance(node, list):
+        oper = my_eval(env, node[0])
+        if not callable(oper):
+            """
+            ...No one wants to write (aref a x y) when they could write a[x,y].
+            In this particular case there is a way to finesse our way out of the
+            problem. If we treat data structures as if they were functions on indexes,
+            we could write (a x y) instead, which is even shorter than the Perl form.
+            """
+            if is_iterable(oper):
+                values = [my_eval(env, c) for c in node[1:]]
+                if values:
+                    if isinstance(values[0], str) or len(values) > 1:
+                        raise MyError(f"{node}: Bad ref")
+                    else:
+                        return ref(oper, *values)
+
+            raise MyError(f"{print_str(oper)}, expected procedure")
+
+        if type(oper) is Syntax:
+            return oper(env, node)
+
+        values = [my_eval(env, c) for c in node[1:]]
+        if type(oper) is Contract:
+            check_args(oper.name, values, (1, 1), None)
+        else:
+            check_args(oper.name, values, oper.arity, oper.contracts)
+        return oper(*values)
+
+    return node
+
+
+def syn_eval(env: Env, v: list) -> Any:
+    if len(v) != 2:
+        raise MyError(f"eval: Arity mismatch, expected 1, given {len(v) - 1}")
+
+    node = my_eval(env, v[1])
+    if isinstance(node, list):
+        return my_eval(env, node)
+    if isinstance(node, Cons):
+        return my_eval(env, list_to_vector(node))
+
+    return node
+
+
+def my_write(v: Any) -> None:
+    try:
+        sys.stdout.write(v)
+    except UnicodeEncodeError as e:
+        raise MyError(e)
+    return None
+
+
+env: Env = {
     # constants
     "true": True,
     "false": False,
-    "null": Null(),
+    "null": Null,
     "pi": math.pi,
+    # syntax
+    "lambda": Syntax(syn_lambda),
+    "λ": Syntax(syn_lambda),
+    "define": Syntax(syn_define),
+    "define/c": Syntax(syn_definec),
+    "set!": Syntax(syn_set),
+    "quote": Syntax(syn_quote),
+    "if": Syntax(syn_if),
+    "when": Syntax(syn_when),
+    "cond": Syntax(syn_cond),
+    "with-open": Syntax(syn_with_open),
+    # loops
+    "for": Syntax(syn_for),
+    "for/vector": Syntax(syn_for_vec),
+    # contracts
+    "number?": is_num,
+    "real?": is_real,
+    "int?": is_int,
+    "uint?": is_uint,
+    "nat?": Contract("nat?", lambda v: type(v) is int and v > 0),
+    "float?": is_float,
+    "frac?": is_frac,
+    "any": any_p,
+    "bool?": is_bool,
+    "void?": is_void,
+    "symbol?": (is_symbol := Contract("symbol?", lambda v: type(v) is Sym)),
+    "string?": is_str,
+    "char?": (is_char := Contract("char?", lambda v: type(v) is Char)),
+    "vector?": (is_vector := Contract("vector?", lambda v: isinstance(v, list))),
+    "array?": (is_array := Contract("array?", lambda v: isinstance(v, np.ndarray))),
+    "bool-array?": is_boolarr,
+    "pair?": (is_pair := Contract("pair?", lambda v: type(v) is Cons)),
+    "null?": Contract("null?", lambda v: v is Null),
+    "list?": Contract("list?", is_list),
+    "range?": (is_range := Contract("range?", lambda v: type(v) is range)),
+    "iterable?": is_iterable,
+    "sequence?": is_sequence,
+    "procedure?": is_proc,
+    "contract?": is_cont,
+    "hash?": (is_hash := Contract("hash?", lambda v: isinstance(v, dict))),
     # actions
     "begin": Proc("begin", lambda *x: x[-1] if x else None, (0, None)),
-    "display": Proc("display", display, (1, 1)),
-    "displayln": Proc("display", displayln, (1, 1)),
-    "print": Proc("print", palet_print, (1, 1)),
-    "exit": Proc("exit", sys.exit, (0, None)),
+    "display": Proc("display", lambda v: my_write(display_str(v)), (1, 1)),
+    "displayln": Proc("displayln", lambda v: my_write(display_str(v) + "\n"), (1, 1)),
+    "print": Proc("print", lambda v: my_write(print_str(v)), (1, 1)),
+    "println": Proc("println", lambda v: my_write(print_str(v) + "\n"), (1, 1)),
+    "exit": Proc("exit", sys.exit, (0, 1), [is_uint]),
     "error": Proc("error", raise_, (1, 1), [is_str]),
-    "void": Proc("void", lambda: None, (0, 0)),
-    "void?": is_void,
+    "sleep": Proc("sleep", sleep, (1, 1), [lambda t: is_int(t) or is_float(t)]),
+    # void
+    "void": Proc("void", lambda *v: None, (0, 0)),
+    # control / b-arrays
+    "not": Proc(
+        "not",
+        lambda v: not v if type(v) is bool else np.logical_not(v),
+        (1, 1),
+        [bool_or_barr],
+    ),
+    "and": Syntax(syn_and),
+    "or": Syntax(syn_or),
+    "xor": Proc("xor", _xor, (2, None), [bool_or_barr]),
     # booleans
-    "boolean?": is_bool,
     ">": Proc(">", lambda a, b: a > b, (2, 2), [is_real, is_real]),
     ">=": Proc(">=", lambda a, b: a >= b, (2, 2), [is_real, is_real]),
     "<": Proc("<", lambda a, b: a < b, (2, 2), [is_real, is_real]),
     "<=": Proc("<=", lambda a, b: a <= b, (2, 2), [is_real, is_real]),
     "=": Proc("=", equal_num, (1, None), [is_num]),
     "eq?": Proc("eq?", lambda a, b: a is b, (2, 2)),
     "equal?": Proc("equal?", is_equal, (2, 2)),
-    "not": Proc("not", _not, (1, 1)),
-    "and": Proc("and", _and, (1, None)),
-    "or": Proc("or", _or, (1, None)),
-    "xor": Proc("xor", _xor, (2, None)),
-    # number predicates
-    "number?": is_num,
-    "real?": is_real,
-    "integer?": is_int,
-    "nonnegative-integer?": us_int,
-    "float?": is_float,
-    "fraction?": is_frac,
-    "positive?": Proc("positive?", lambda v: v > 0, (1, 1), [is_real]),
-    "negative?": Proc("negative?", lambda v: v < 0, (1, 1), [is_real]),
-    "zero?": Proc("zero?", lambda v: v == 0, (1, 1), [is_num]),
+    "zero?": UserProc("zero?", ["z"], [[Sym("="), Sym("z"), 0]], [is_num]),
+    "positive?": UserProc("positive?", ["x"], [[Sym(">"), Sym("x"), 0]], [is_real]),
+    "negative?": UserProc("negative?", ["x"], [[Sym("<"), Sym("x"), 0]], [is_real]),
+    "even?": UserProc(
+        "even?", ["n"], [[Sym("zero?"), [Sym("mod"), Sym("n"), 2]]], [is_int]
+    ),
+    "odd?": UserProc("odd?", ["n"], [[Sym("not"), [Sym("even?"), Sym("n")]]], [is_int]),
     # numbers
     "+": Proc("+", lambda *v: sum(v), (0, None), [is_num]),
     "-": Proc("-", minus, (1, None), [is_num]),
     "*": Proc("*", mul, (0, None), [is_num]),
     "/": Proc("/", div, (1, None), [is_num]),
-    "add1": Proc("add1", lambda v: v + 1, (1, 1), [is_num]),
-    "sub1": Proc("sub1", lambda v: v - 1, (1, 1), [is_num]),
+    "add1": Proc("add1", lambda z: z + 1, (1, 1), [is_num]),
+    "sub1": Proc("sub1", lambda z: z - 1, (1, 1), [is_num]),
     "sqrt": Proc("sqrt", _sqrt, (1, 1), [is_num]),
     "real-part": Proc("real-part", lambda v: v.real, (1, 1), [is_num]),
     "imag-part": Proc("imag-part", lambda v: v.imag, (1, 1), [is_num]),
     # reals
     "pow": Proc("pow", pow, (2, 2), [is_real]),
     "exp": Proc("exp", math.exp, (1, 1), [is_real]),
     "abs": Proc("abs", abs, (1, 1), [is_real]),
@@ -1045,339 +1556,109 @@
     "round": Proc("round", round, (1, 1), [is_real]),
     "max": Proc("max", lambda *v: max(v), (1, None), [is_real]),
     "min": Proc("min", lambda *v: min(v), (1, None), [is_real]),
     "sin": Proc("sin", math.sin, (1, 1), [is_real]),
     "cos": Proc("cos", math.cos, (1, 1), [is_real]),
     "log": Proc("log", math.log, (1, 2), [is_real, is_real]),
     "tan": Proc("tan", math.tan, (1, 1), [is_real]),
-    "mod": Proc("mod", lambda a, b: a % b, (2, 2), [is_int, is_int]),
-    "random": Proc("random", palet_random, (0, 2), [is_int]),
+    "mod": Proc("mod", lambda a, b: a % b, (2, 2), [is_int]),
+    "modulo": Proc("modulo", lambda a, b: a % b, (2, 2), [is_int]),
+    "random": Proc("random", random.random, (0, 0)),
+    "randrange": Proc("randrange", randrange, (1, 3), [is_int, is_int, int_not_zero]),
     # symbols
-    "symbol?": is_symbol,
     "symbol->string": Proc("symbol->string", str, (1, 1), [is_symbol]),
-    "string->symbol": Proc("string->symbol", Symbol, (1, 1), [is_str]),
+    "string->symbol": Proc("string->symbol", Sym, (1, 1), [is_str]),
     # strings
-    "string?": is_str,
-    "char?": is_char,
     "string": Proc("string", string_append, (0, None), [is_char]),
     "string-append": Proc("string-append", string_append, (0, None), [is_str]),
     "string-upcase": Proc("string-upcase", str.upper, (1, 1), [is_str]),
     "string-downcase": Proc("string-downcase", str.lower, (1, 1), [is_str]),
     "string-titlecase": Proc("string-titlecase", str.title, (1, 1), [is_str]),
-    "char->integer": Proc("char->integer", lambda c: ord(c.val), (1, 1), [is_char]),
-    "integer->char": Proc("integer->char", Char, (1, 1), [is_int]),
+    "char->int": Proc("char->int", lambda c: ord(c.val), (1, 1), [is_char]),
+    "int->char": Proc("int->char", Char, (1, 1), [is_int]),
+    "~a": Proc("~a", lambda *v: "".join([display_str(a) for a in v]), (0, None)),
+    "~s": Proc("~s", lambda *v: " ".join([display_str(a) for a in v]), (0, None)),
+    "~v": Proc("~v", lambda *v: " ".join([print_str(a) for a in v]), (0, None)),
     # vectors
-    "vector?": is_vector,
     "vector": Proc("vector", lambda *a: list(a), (0, None)),
     "make-vector": Proc(
-        "make-vector", lambda size, a=0: [a] * size, (1, 2), [us_int, any_p]
+        "make-vector", lambda size, a=0: [a] * size, (1, 2), [is_uint, any_p]
     ),
     "vector-append": Proc("vector-append", vector_append, (0, None), [is_vector]),
     "vector-pop!": Proc("vector-pop!", list.pop, (1, 1), [is_vector]),
     "vector-add!": Proc("vector-add!", list.append, (2, 2), [is_vector, any_p]),
     "vector-set!": Proc("vector-set!", vector_set, (3, 3), [is_vector, is_int, any_p]),
     "vector-extend!": Proc("vector-extend!", vector_extend, (2, None), [is_vector]),
     # cons/list
-    "pair?": is_pair,
-    "null?": is_null,
     "cons": Proc("cons", Cons, (2, 2)),
     "car": Proc("car", lambda val: val.a, (1, 1), [is_pair]),
     "cdr": Proc("cdr", lambda val: val.d, (1, 1), [is_pair]),
-    "list?": is_list,
+    "caar": UserProc("caar", ["v"], [[Sym("car"), [Sym("car"), Sym("v")]]]),
+    "cadr": UserProc("cdar", ["v"], [[Sym("car"), [Sym("cdr"), Sym("v")]]]),
+    "cdar": UserProc("cdar", ["v"], [[Sym("cdr"), [Sym("car"), Sym("v")]]]),
+    "cddr": UserProc("cddr", ["v"], [[Sym("cdr"), [Sym("cdr"), Sym("v")]]]),
     "list": Proc("list", _list, (0, None)),
-    "list-ref": Proc("list-ref", ref, (2, 2), [is_pair, us_int]),
+    "list-ref": Proc("list-ref", ref, (2, 2), [is_pair, is_uint]),
     # arrays
-    "array?": is_array,
     "array": Proc("array", array_proc, (2, None), [is_symbol, is_real]),
-    "make-array": Proc("make-array", make_array, (2, 3), [is_symbol, us_int, is_real]),
+    "make-array": Proc("make-array", make_array, (2, 3), [is_symbol, is_uint, is_real]),
     "array-splice!": Proc(
         "array-splice!", splice, (2, 4), [is_array, is_real, is_int, is_int]
     ),
     "count-nonzero": Proc("count-nonzero", np.count_nonzero, (1, 1), [is_array]),
     # bool arrays
-    "bool-array?": is_boolarr,
     "bool-array": Proc(
-        "bool-array", lambda *a: np.array(a, dtype=np.bool_), (1, None), [us_int]
+        "bool-array", lambda *a: np.array(a, dtype=np.bool_), (1, None), [is_uint]
     ),
     "margin": Proc("margin", margin, (2, 3), None),
-    "mincut": Proc("mincut", mincut, (2, 2), [is_int, is_boolarr]),
-    "minclip": Proc("minclip", minclip, (2, 2), [is_int, is_boolarr]),
+    "mincut": Proc("mincut", mincut, (2, 2), [is_boolarr, is_uint]),
+    "minclip": Proc("minclip", minclip, (2, 2), [is_boolarr, is_uint]),
     # ranges
-    "range?": is_range,
-    "range": Proc("range", range, (1, 3), [is_real, is_real, is_real]),
+    "range": Proc("range", range, (1, 3), [is_int, is_int, int_not_zero]),
     # generic iterables
-    "iterable?": is_iterable,
-    "sequence?": is_sequence,
     "length": Proc("length", len, (1, 1), [is_iterable]),
     "reverse": Proc("reverse", lambda v: v[::-1], (1, 1), [is_sequence]),
     "ref": Proc("ref", ref, (2, 2), [is_iterable, is_int]),
     "slice": Proc("slice", p_slice, (2, 4), [is_sequence, is_int]),
     # procedures
-    "procedure?": is_proc,
-    "map": Proc("map", palet_map, (2, 2), [is_proc, is_iterable]),
-    "apply": Proc("apply", apply, (2, 2), [is_proc, is_iterable]),
+    "map": Proc("map", palet_map, (2, 2), [is_proc, is_sequence]),
+    "apply": Proc("apply", apply, (2, 2), [is_proc, is_sequence]),
+    "and/c": Proc("and/c", andc, (1, None), [is_cont]),
+    "or/c": Proc("or/c", orc, (1, None), [is_cont]),
+    "not/c": Proc("not/c", notc, (1, 1), [is_cont]),
     # hashs
-    "hash?": is_hash,
     "hash": Proc("hash", palet_hash),
     "has-key?": Proc("has-key?", lambda h, k: k in h, (2, 2), [is_hash, any_p]),
     # conversions
     "number->string": Proc("number->string", number_to_string, (1, 1), [is_num]),
-    "string->list": Proc("string->list", string_to_list, (1, 1), [is_str]),
+    "string->list": Proc(
+        "string->list", lambda s: vec_to_list([Char(c) for c in s]), (1, 1), [is_str]
+    ),
     "string->vector": Proc(
         "string->vector", lambda s: [Char(c) for c in s], (1, 1), [is_str]
     ),
     "list->vector": Proc("list->vector", list_to_vector, (1, 1), [is_pair]),
-    "vector->list": Proc("vector->list", vector_to_list, (1, 1), [is_vector]),
+    "vector->list": Proc("vector->list", vec_to_list, (1, 1), [is_vector]),
     "range->list": Proc("range->list", stream_to_list, (1, 1), [is_range]),
     "range->vector": Proc("range->vector", list, (1, 1), [is_range]),
-    # predicates
-    "any": any_p,
+    # objects
+    "object?": is_obj,
+    "attrs": Proc("attrs", lambda v: list(get_attrs(v).keys()), (1, 1), [is_obj]),
+    ".": Syntax(syn_dot),
+    # reflection
+    "eval": Syntax(syn_eval),
+    "var-exists?": Proc("var-exists?", lambda sym: sym.val in env, (1, 1), [is_symbol]),
 }
 
 
 ###############################################################################
 #                                                                             #
 #  INTERPRETER                                                                #
 #                                                                             #
 ###############################################################################
 
 
-@dataclass
-class FileSetup:
-    src: FileInfo
-    ensure: Ensure
-    strict: bool
-    tb: Fraction
-    bar: Bar
-    temp: str
-    log: Log
-
-
-class Interpreter:
-    def __init__(
-        self, env: dict[str, Any], parser: Parser, filesetup: FileSetup | None
-    ):
-        self.parser = parser
-        self.filesetup = filesetup
-
-        if filesetup is not None:
-            env["timebase"] = filesetup.tb
-
-        self.env = env
-
-    def visit(self, node: Any) -> Any:
-        if isinstance(node, Symbol):
-            val = self.env.get(node.val)
-            if val is None:
-                raise MyError(f"{node.val} is undefined")
-            return val
-
-        if isinstance(node, BoolArr):
-            if self.filesetup is None:
-                raise MyError("Can't use edit methods if there's no input files")
-            return edit_method(node.val, self.filesetup)
-
-        if isinstance(node, list):
-            if not node:
-                raise MyError("(): Missing procedure expression")
-
-            name = node[0].val if isinstance(node[0], Symbol) else ""
-
-            def check_for_syntax(name: str, node: list) -> Any:
-                if len(node) < 2:
-                    raise MyError(f"{name}: bad syntax")
-
-                if len(node) == 2:
-                    raise MyError(f"{name}: missing body")
-
-                assert isinstance(node[1], list)
-                assert isinstance(node[1][0], list)
-
-                var = node[1][0][0]
-                if not isinstance(var, Symbol):
-                    raise MyError(f"{name}: binding must be an identifier")
-                my_iter = self.visit(node[1][0][1])
-
-                if not is_iterable(my_iter):
-                    if isinstance(my_iter, int):
-                        return var, range(my_iter)
-                    raise MyError(f"{name}: got non-iterable in iter slot")
-
-                return var, my_iter
-
-            if name == "lambda" or name == "λ":
-                if not isinstance(node[1], list):
-                    raise MyError("lambda: bad syntax")
-
-                parameters = node[1]
-                body = node[2:]
-                return UserProc("", self.env, self.visit, parameters, body)
-
-            if name == "define":
-                if len(node) < 3:
-                    raise MyError("define: bad syntax")
-
-                if not isinstance(node[1], Symbol):
-                    raise MyError("define: Must be an identifier")
-
-                if isinstance(node[2], list):
-                    if node[2][0] == Symbol("lambda") or node[2][0] == Symbol("λ"):
-                        parameters = node[2][1]
-                        body = node[2][2:]
-                    else:
-                        parameters = node[2]
-                        body = node[3:]
-                    n = node[1].val
-                    self.env[n] = UserProc(n, self.env, self.visit, parameters, body)
-                else:
-                    self.env[node[1].val] = self.visit(node[2])
-                return None
-
-            if name == "set!":
-                if len(node) != 3:
-                    raise MyError("set!: bad syntax")
-                if not isinstance(node[1], Symbol):
-                    raise MyError("set!: Must be an identifier")
-
-                symbol = node[1].val
-                if symbol not in self.env:
-                    raise MyError(f"Cannot set variable {symbol} before definition")
-                self.env[symbol] = self.visit(node[2])
-                return None
-
-            if name == "for":
-                var, my_iter = check_for_syntax("for", node)
-                for item in my_iter:
-                    self.env[var.val] = item
-                    for c in node[2:]:
-                        self.visit(c)
-                return None
-
-            if name == "for/vector":
-                results = []
-                var, my_iter = check_for_syntax("for", node)
-                for item in my_iter:
-                    self.env[var.val] = item
-                    results.append([self.visit(c) for c in node[2:]][-1])
-
-                del self.env[var.val]
-                return results
-
-            if name == "if":
-                if len(node) != 4:
-                    raise MyError("if: bad syntax")
-                test_expr = self.visit(node[1])
-                if not isinstance(test_expr, bool):
-                    raise MyError(f"if: test-expr arg must be: boolean?")
-                if test_expr:
-                    return self.visit(node[2])
-                return self.visit(node[3])
-
-            if name == "when":
-                if len(node) != 3:
-                    raise MyError("when: bad syntax")
-                test_expr = self.visit(node[1])
-                if not isinstance(test_expr, bool):
-                    raise MyError(f"when: test-expr arg must be: boolean?")
-                if test_expr:
-                    return self.visit(node[2])
-                return None
-
-            if name == "quote":
-                if len(node) != 2:
-                    raise MyError("quote: bad syntax")
-
-                if isinstance(node[1], list):
-                    return deep_list(node[1])
-                return node[1]
-
-            if name == "with-open":
-                if len(node) < 2:
-                    raise MyError("with-open: wrong number of args")
-                if len(node[1]) != 2 and len(node[1]) != 3:
-                    raise MyError("with-open: wrong number of args")
-
-                if not isinstance(node[1][0], Symbol):
-                    raise MyError("with-open: as must be an identifier")
-
-                file_binding = node[1][0].val
-
-                file_name = self.visit(node[1][1])
-                if not isinstance(file_name, str):
-                    raise MyError("with-open: file name must be string?")
-
-                if len(node[1]) == 3:
-                    file_mode = self.visit(node[1][2])
-                    if not isinstance(file_mode, Symbol):
-                        raise MyError("with-open: file-mode must be a symbol?")
-                    if file_mode not in (Symbol("w"), Symbol("a"), Symbol("r")):
-                        raise MyError("with-open: file mode must be either: 'w 'r 'a")
-                else:
-                    file_mode = Symbol("w")
-
-                with open(file_name, file_mode.val) as file:
-                    if file_mode.val == "r":
-                        open_file = PaletObject(
-                            {
-                                "read": Proc("read", file.read, (0, 0)),
-                                "readlines": Proc("readlines", file.readlines, (0, 0)),
-                            }
-                        )
-                    else:
-                        open_file = PaletObject(
-                            {"write": Proc("write", file.write, (1, 1), [is_str])}
-                        )
-
-                    self.env[file_binding] = open_file
-                    for c in node[2:]:
-                        self.visit(c)
-
-                del self.env[file_binding]
-                return None
-
-            if name == ".":
-                if len(node) != 3:
-                    raise MyError(".: not enough args")
-
-                my_obj = self.visit(node[1])
-                if not isinstance(my_obj, PaletObject):
-                    raise MyError(f".: expected an object, got {my_obj}")
-
-                if not isinstance(node[2], Symbol):
-                    raise MyError(".: attribute must be an identifier")
-                my_attr = node[2].val
-
-                if my_attr not in my_obj.attributes:
-                    raise MyError(f".: No such attribute: {my_attr}")
-
-                return my_obj.attributes[my_attr]
-
-            oper = self.visit(node[0])
-
-            if not callable(oper):
-                """
-                ...No one wants to write (aref a x y) when they could write a[x,y].
-
-                In this particular case there is a way to finesse our way out of the
-                problem. If we treat data structures as if they were functions on indexes,
-                we could write (a x y) instead, which is even shorter than the Perl form.
-                """
-                if is_iterable(oper):
-                    values = [self.visit(c) for c in node[1:]]
-                    return ref(oper, *values)
-
-                raise MyError(f"{oper}, expected procedure")
-
-            values = [self.visit(c) for c in node[1:]]
-            if isinstance(oper, Contract):
-                check_args(oper.name, values, (1, 1), None)
-            else:
-                check_args(oper.name, values, oper.arity, oper.contracts)
-            return oper(*values)
-
-        return node
-
-    def interpret(self) -> Any:
-        result = []
-        while self.parser.current_token.type not in (EOF, RPAREN, RBRAC, RCUR):
-            result.append(self.visit(self.parser.expr()))
-        return result
+def interpret(env: Env, parser: Parser) -> Any:
+    result = []
+    while parser.current_token.type not in (EOF, RPAREN, RBRAC, RCUR):
+        result.append(my_eval(env, parser.expr()))
+    return result
```

### Comparing `auto-editor-23.4.1/auto_editor/make_layers.py` & `auto-editor-23.8.1/auto_editor/make_layers.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,36 @@
 
 import os
 from fractions import Fraction
 from typing import TYPE_CHECKING, Any, NamedTuple
 
 import numpy as np
 
+from auto_editor.analyze import FileSetup
 from auto_editor.ffwrapper import FFmpeg, FileInfo
-from auto_editor.interpreter import (
-    FileSetup,
-    Interpreter,
-    Lexer,
-    MyError,
-    Parser,
-    env,
-    is_boolarr,
-)
-from auto_editor.objs.util import ParserError, parse_dataclass
+from auto_editor.interpreter import Lexer, MyError, Parser, env, interpret, is_boolarr
+from auto_editor.objs.util import ParserError, parse_with_palet
 from auto_editor.timeline import (
     ASpace,
     TlAudio,
     TlVideo,
     Visual,
     VSpace,
     audio_objects,
     v1,
     v3,
     visual_objects,
 )
 from auto_editor.utils.chunks import Chunks, chunkify, chunks_len, merge_chunks
 from auto_editor.utils.func import mut_margin
-from auto_editor.utils.types import Args, CoerceError, pos, time
+from auto_editor.utils.types import Args, CoerceError, time
 
 if TYPE_CHECKING:
     from numpy.typing import NDArray
 
-    from auto_editor.ffwrapper import FileInfo
     from auto_editor.output import Ensure
     from auto_editor.utils.bar import Bar
     from auto_editor.utils.log import Log
     from auto_editor.utils.types import Margin
 
     BoolList = NDArray[np.bool_]
 
@@ -71,15 +63,14 @@
 
     return clips
 
 
 def make_av(
     all_clips: list[list[Clip]], sources: dict[str, FileInfo], _inputs: list[int]
 ) -> tuple[VSpace, ASpace]:
-
     if len(_inputs) > 1000:
         raise ValueError("Number of file inputs can't be greater than 1000")
 
     inputs = [str(i) for i in _inputs]
     vtl: VSpace = []
     atl: ASpace = [[] for _ in range(max(len(sources[i].audios) for i in inputs))]
 
@@ -98,23 +89,23 @@
 
 
 def run_interpreter(
     text: str,
     filesetup: FileSetup,
     log: Log,
 ) -> NDArray[np.bool_]:
-
     try:
-        lexer = Lexer(text)
-        parser = Parser(lexer)
+        parser = Parser(Lexer(text))
         if log.is_debug:
             log.debug(f"edit: {parser}")
 
-        interpreter = Interpreter(env, parser, filesetup)
-        results = interpreter.interpret()
+        env["timebase"] = filesetup.tb
+        env["@filesetup"] = filesetup
+
+        results = interpret(env, parser)
     except (MyError, ZeroDivisionError) as e:
         log.error(e)
 
     if len(results) == 0:
         log.error("Expression in --edit must return a bool-array")
 
     result = results[-1]
@@ -132,15 +123,14 @@
     ensure: Ensure,
     args: Args,
     sr: int,
     bar: Bar,
     temp: str,
     log: Log,
 ) -> v3:
-
     inp = None if not inputs else sources[str(inputs[0])]
 
     if inp is None:
         tb, res = Fraction(30), (1920, 1080)
     else:
         tb = inp.get_fps() if args.frame_rate is None else args.frame_rate
         res = inp.get_res() if args.resolution is None else args.resolution
@@ -186,50 +176,32 @@
 
         sources[label] = FileInfo(path, ffmpeg, log, label)
 
     v1_compatiable = None if inp is None else v1(inp, chunks)
     tl = v3(sources, tb, sr, res, args.background, vclips, aclips, v1_compatiable)
 
     w, h = res
-
-    def my_var_f(name: str, val: Any, coerce: Any) -> Any:
-        if name in ("x", "width"):
-            return pos((val, res[0]))
-        if name in ("y", "height"):
-            return pos((val, res[1]))
-        if name in ("start", "dur", "offset"):
-            if isinstance(val, int):
-                return val
-            if val == "start":
-                return 0
-            if val == "end":
-                return tl.end
-            _val = time(val)
-            if isinstance(_val, str):
-                return round(float(_val) * tl.tb)
-            return _val
-        return coerce(val)
-
     pool: list[Visual] = []
     apool: list[TlAudio] = []
 
+    env["start"] = 0
+    env["end"] = tl.end
+
     for obj_attrs_str in args.add:
         exploded = obj_attrs_str.split(":", 1)
         obj_s = exploded[0]
         attrs = "" if len(exploded) == 1 else exploded[1]
 
         try:
             if obj_s in visual_objects:
-                pool.append(
-                    parse_dataclass(attrs, visual_objects[obj_s], my_var_f, True)
-                )
+                dic_obj = parse_with_palet(attrs, visual_objects[obj_s][1], env)
+                pool.append(visual_objects[obj_s][0](**dic_obj))
             elif obj_s in audio_objects:
-                apool.append(
-                    parse_dataclass(attrs, audio_objects[obj_s], my_var_f, True)
-                )
+                dic_obj = parse_with_palet(attrs, audio_objects[obj_s][1], env)
+                apool.append(audio_objects[obj_s][0](**dic_obj))
             else:
                 log.error(f"Unknown timeline object: '{obj_s}'")
         except (ParserError, CoerceError) as e:
             log.error(e)
 
     for vobj in pool:
         tl.v.append([vobj])
```

### Comparing `auto-editor-23.4.1/auto_editor/output.py` & `auto-editor-23.8.1/auto_editor/output.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,14 @@
     output_path: str,
     tb: Fraction,
     args: Args,
     src: FileInfo,
     temp: str,
     log: Log,
 ) -> None:
-
     v_tracks = len(visual_output)
     a_tracks = len(audio_output)
     s_tracks = len(sub_output)
 
     cmd = ["-hide_banner", "-y", "-i", f"{src.path}"]
 
     same_container = src.path.suffix == os.path.splitext(output_path)[1]
```

### Comparing `auto-editor-23.4.1/auto_editor/preview.py` & `auto-editor-23.8.1/auto_editor/preview.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
 from fractions import Fraction
 from statistics import fmean, median
 
-from auto_editor.analyze import get_media_length
+from auto_editor.analyze import Levels
 from auto_editor.output import Ensure
 from auto_editor.timeline import v3
+from auto_editor.utils.bar import Bar
 from auto_editor.utils.func import to_timecode
 from auto_editor.utils.log import Log
 
 
 def time_frame(title: str, ticks: float, tb: Fraction, per: str | None = None) -> None:
     tc = to_timecode(ticks / tb, "ass")
 
@@ -46,15 +47,16 @@
 def preview(ensure: Ensure, tl: v3, temp: str, log: Log) -> None:
     log.conwrite("")
     tb = tl.tb
 
     # Calculate input videos length
     in_len = 0
     for src in tl.sources.values():
-        in_len += get_media_length(ensure, src, tl.tb, temp, log)
+        levels = Levels(ensure, src, tb, Bar("none"), temp, log).media_length
+        in_len += levels
 
     out_len = tl.out_len()
 
     diff = out_len - in_len
 
     print("\nlength:")
     time_frame("input", in_len, tb, per="100.0%")
```

### Comparing `auto-editor-23.4.1/auto_editor/render/audio.py` & `auto-editor-23.8.1/auto_editor/render/audio.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/render/image.py` & `auto-editor-23.8.1/auto_editor/render/image.py`

 * *Files 10% similar despite different names*

```diff
@@ -58,19 +58,32 @@
 
 
 def render_image(
     frame: av.VideoFrame, obj: Visual, font_cache: FontCache, img_cache: ImgCache
 ) -> av.VideoFrame:
     img = frame.to_image().convert("RGBA")
 
+    def z(h: int, x: int | float) -> int:
+        if isinstance(x, float):
+            return round(h * x)
+        return x
+
+    x = z(frame.width, obj.x)
+    y = z(frame.height, obj.y)
+
+    if isinstance(obj, (TlRect, TlEllipse)):
+        w = z(frame.width, obj.width)
+        h = z(frame.height, obj.height)
+
     if isinstance(obj, TlEllipse):
         # Adding +1 to width makes Ellipse look better.
-        obj_img = Image.new("RGBA", (obj.width + 1, obj.height), (255, 255, 255, 0))
+        obj_img = Image.new("RGBA", (w + 1, h), (255, 255, 255, 0))
     if isinstance(obj, TlRect):
-        obj_img = Image.new("RGBA", (obj.width, obj.height), (255, 255, 255, 0))
+        obj_img = Image.new("RGBA", (w, h), (255, 255, 255, 0))
+
     if isinstance(obj, TlImage):
         obj_img = img_cache[obj.src]
         if obj.stroke > 0:
             obj_img = ImageOps.expand(obj_img, border=obj.stroke, fill=obj.strokecolor)
 
     if isinstance(obj, TlText):
         obj_img = Image.new("RGBA", img.size)
@@ -91,23 +104,23 @@
             align=obj.align,
             stroke_width=obj.stroke,
             stroke_fill=obj.strokecolor,
         )
 
     if isinstance(obj, TlRect):
         draw.rectangle(
-            (0, 0, obj.width, obj.height),
+            (0, 0, w, h),
             fill=obj.fill,
             width=obj.stroke,
             outline=obj.strokecolor,
         )
 
     if isinstance(obj, TlEllipse):
         draw.ellipse(
-            (0, 0, obj.width, obj.height),
+            (0, 0, w, h),
             fill=obj.fill,
             width=obj.stroke,
             outline=obj.strokecolor,
         )
 
     # Do Anti-Aliasing
     obj_img = obj_img.resize((obj_img.size[0] * 3, obj_img.size[1] * 3))
@@ -120,11 +133,11 @@
     )
     obj_img = ImageChops.multiply(
         obj_img,
         Image.new("RGBA", obj_img.size, (255, 255, 255, int(obj.opacity * 255))),
     )
     img.paste(
         obj_img,
-        apply_anchor(obj.x, obj.y, obj_img.size[0], obj_img.size[1], obj.anchor),
+        apply_anchor(x, y, obj_img.size[0], obj_img.size[1], obj.anchor),
         obj_img,
     )
     return frame.from_image(img)
```

### Comparing `auto-editor-23.4.1/auto_editor/render/subtitle.py` & `auto-editor-23.8.1/auto_editor/render/subtitle.py`

 * *Files 0% similar despite different names*

```diff
@@ -85,15 +85,14 @@
         for cut in reversed(chunks):
             the_speed = cut[2]
             speed_factor = 1 if the_speed == 99999 else 1 - (1 / the_speed)
 
             new_content = []
             for content in self.contents:
                 if cut[0] <= content.end and cut[1] > content.start:
-
                     diff = int(
                         (min(cut[1], content.end) - max(cut[0], content.start))
                         * speed_factor
                     )
                     if content.start > cut[0]:
                         content.start -= diff
                         content.end -= diff
```

### Comparing `auto-editor-23.4.1/auto_editor/render/video.py` & `auto-editor-23.8.1/auto_editor/render/video.py`

 * *Files 1% similar despite different names*

```diff
@@ -62,15 +62,14 @@
     tl: v3,
     args: Args,
     bar: Bar,
     ctr: Container,
     temp: str,
     log: Log,
 ) -> tuple[str, bool]:
-
     if not tl.sources:
         if "0" in tl.sources:
             src: FileInfo | None = tl.sources["0"]
         else:
             src = next(iter(tl.sources.items()))[1]
     else:
         src = None
```

### Comparing `auto-editor-23.4.1/auto_editor/subcommands/desc.py` & `auto-editor-23.8.1/auto_editor/subcommands/desc.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/subcommands/info.py` & `auto-editor-23.8.1/auto_editor/subcommands/info.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,15 @@
     bitrate: str | None
     lang: str | None
 
 
 class AudioJson(TypedDict):
     codec: str
     samplerate: int
+    channels: int
     duration: str | None
     bitrate: str | None
     lang: str | None
 
 
 class SubtitleJson(TypedDict):
     codec: str
@@ -155,14 +156,15 @@
             }
             file_info[file]["video"].append(vid)
 
         for track, a in enumerate(src.audios):
             aud: AudioJson = {
                 "codec": a.codec,
                 "samplerate": a.samplerate,
+                "channels": a.channels,
                 "duration": a.duration,
                 "bitrate": a.bitrate,
                 "lang": a.lang,
             }
             file_info[file]["audio"].append(aud)
 
         for track, s_stream in enumerate(src.subtitles):
```

### Comparing `auto-editor-23.4.1/auto_editor/subcommands/levels.py` & `auto-editor-23.8.1/auto_editor/subcommands/levels.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from __future__ import annotations
 
 import sys
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Any
 
 import numpy as np
 
-from auto_editor.analyze import (
-    audio_levels,
-    motion_levels,
-    pixeldiff_levels,
-    subtitle_levels,
-)
+from auto_editor.analyze import Levels
 from auto_editor.ffwrapper import FFmpeg, FileInfo
 from auto_editor.objs.edit import (
     audio_builder,
     motion_builder,
     pixeldiff_builder,
     subtitle_builder,
 )
@@ -25,47 +20,19 @@
 from auto_editor.utils.func import setup_tempdir
 from auto_editor.utils.log import Log
 from auto_editor.utils.types import frame_rate, pos
 from auto_editor.vanparse import ArgumentParser
 
 if TYPE_CHECKING:
     from fractions import Fraction
-    from typing import Any
 
     from numpy.typing import NDArray
 
 
 @dataclass
-class Audio:
-    stream: int
-    mincut: int
-    minclip: int
-
-
-@dataclass
-class Motion:
-    stream: int
-    blur: int
-    width: int
-
-
-@dataclass
-class Pixeldiff:
-    stream: int
-
-
-@dataclass
-class Subtitle:
-    pattern: str
-    stream: int
-    ignore_case: bool = False
-    max_count: int | None = None
-
-
-@dataclass
 class LevelArgs:
     input: list[str] = field(default_factory=list)
     edit: str = "audio"
     timebase: Fraction | None = None
     ffmpeg_location: str | None = None
     my_ffmpeg: bool = False
     help: bool = False
@@ -120,64 +87,62 @@
 
     assert "0" in sources
     src = sources["0"]
 
     tb = src.get_fps() if args.timebase is None else args.timebase
     ensure = Ensure(ffmpeg, src.get_samplerate(), temp, log)
 
-    strict = True
-
     if ":" in args.edit:
         method, attrs = args.edit.split(":", 1)
     else:
         method, attrs = args.edit, ""
 
     def my_var_f(name: str, val: str, coerce: Any) -> Any:
         if src.videos:
             if name in ("x", "width"):
                 return pos((val, src.videos[0].width))
             if name in ("y", "height"):
                 return pos((val, src.videos[0].height))
         return coerce(val)
 
     for src in sources.values():
-        if method == "audio":
-            try:
-                aobj = parse_dataclass(attrs, (Audio, audio_builder[1:]))
-            except ParserError as e:
-                log.error(e)
+        method_map = {
+            "audio": audio_builder,
+            "motion": motion_builder,
+            "pixeldiff": pixeldiff_builder,
+            "subtitle": subtitle_builder,
+        }
+        levels = Levels(ensure, src, tb, bar, temp, log)
 
-            print_floats(
-                audio_levels(ensure, src, aobj.stream, tb, bar, strict, temp, log)
-            )
+        if method in method_map:
+            builder = method_map[method]
 
-        elif method == "motion":
             try:
-                mobj = parse_dataclass(attrs, (Motion, motion_builder[1:]), my_var_f)
+                obj = parse_dataclass(attrs, builder)
             except ParserError as e:
                 log.error(e)
 
-            print_floats(motion_levels(ensure, src, mobj, tb, bar, strict, temp, log))
+            if "threshold" in obj:
+                del obj["threshold"]
 
+        if method == "audio":
+            print_floats(levels.audio(obj["stream"]))
+        elif method == "motion":
+            print_floats(levels.motion(obj["stream"], obj["blur"], obj["width"]))
         elif method == "pixeldiff":
-            try:
-                pobj = parse_dataclass(
-                    attrs, (Pixeldiff, pixeldiff_builder[1:]), my_var_f
-                )
-            except ParserError as e:
-                log.error(e)
-
-            print_ints(pixeldiff_levels(ensure, src, pobj, tb, bar, strict, temp, log))
+            print_ints(levels.pixeldiff(obj["stream"]))
         elif method == "subtitle":
-            try:
-                sobj = parse_dataclass(attrs, (Subtitle, subtitle_builder))
-            except ParserError as e:
-                log.error(e)
-
-            print_ints(subtitle_levels(ensure, src, sobj, tb, bar, strict, temp, log))
+            print_ints(
+                levels.subtitle(
+                    obj["pattern"],
+                    obj["stream"],
+                    obj["ignore_case"],
+                    obj["max_count"],
+                )
+            )
         else:
             log.error(f"Method: {method} not supported")
 
     log.cleanup()
 
 
 if __name__ == "__main__":
```

### Comparing `auto-editor-23.4.1/auto_editor/subcommands/repl.py` & `auto-editor-23.8.1/auto_editor/subcommands/subdump.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,113 +1,58 @@
-# type: ignore
-
 from __future__ import annotations
 
+import os
 import sys
+import tempfile
 from dataclasses import dataclass, field
-from fractions import Fraction
 
-import auto_editor
 from auto_editor.ffwrapper import FFmpeg, FileInfo
-from auto_editor.interpreter import (
-    FileSetup,
-    Interpreter,
-    Lexer,
-    MyError,
-    Parser,
-    env,
-    print_str,
-)
-from auto_editor.output import Ensure
-from auto_editor.utils.bar import Bar
-from auto_editor.utils.func import setup_tempdir
 from auto_editor.utils.log import Log
-from auto_editor.utils.types import frame_rate
 from auto_editor.vanparse import ArgumentParser
 
-try:
-    import readline  # noqa
-except ImportError:
-    pass
-
 
 @dataclass
-class REPL_Args:
-    input: list[str] = field(default_factory=list)
-    timebase: Fraction | None = None
+class SubArgs:
     ffmpeg_location: str | None = None
     my_ffmpeg: bool = False
-    temp_dir: str | None = None
     help: bool = False
+    input: list[str] = field(default_factory=list)
 
 
-def repl_options(parser: ArgumentParser) -> ArgumentParser:
+def subdump_options(parser: ArgumentParser) -> ArgumentParser:
     parser.add_required("input", nargs="*")
-    parser.add_argument(
-        "--timebase",
-        "-tb",
-        metavar="NUM",
-        type=frame_rate,
-        help="Set custom timebase",
-    )
     parser.add_argument("--ffmpeg-location", help="Point to your custom ffmpeg file")
     parser.add_argument(
         "--my-ffmpeg",
         flag=True,
         help="Use the ffmpeg on your PATH instead of the one packaged",
     )
-    parser.add_argument(
-        "--temp-dir",
-        metavar="PATH",
-        help="Set where the temporary directory is located",
-    )
     return parser
 
 
 def main(sys_args: list[str] = sys.argv[1:]) -> None:
-    parser = repl_options(ArgumentParser(None))
-    args = parser.parse_args(REPL_Args, sys_args)
+    args = subdump_options(ArgumentParser("subdump")).parse_args(SubArgs, sys_args)
+
+    ffmpeg = FFmpeg(args.ffmpeg_location, args.my_ffmpeg, debug=False)
+
+    temp = tempfile.mkdtemp()
+    log = Log(temp=temp)
+
+    for i, input_file in enumerate(args.input):
+        src = FileInfo(input_file, ffmpeg, log)
+
+        cmd = ["-i", input_file]
+        for s, sub in enumerate(src.subtitles):
+            cmd.extend(["-map", f"0:s:{s}", os.path.join(temp, f"{i}s{s}.{sub.ext}")])
+        ffmpeg.run(cmd)
 
-    if len(args.input) == 0:
-        filesetup = None
-        log = Log(quiet=True)
-    else:
-        temp = setup_tempdir(args.temp_dir, Log())
-        log = Log(quiet=True, temp=temp)
-        ffmpeg = FFmpeg(args.ffmpeg_location, args.my_ffmpeg, False)
-        strict = len(args.input) < 2
-        sources = {}
-        for i, path in enumerate(args.input):
-            sources[str(i)] = FileInfo(path, ffmpeg, log, str(i))
-
-        src = sources["0"]
-        tb = src.get_fps() if args.timebase is None else args.timebase
-        ensure = Ensure(ffmpeg, src.get_samplerate(), temp, log)
-        filesetup = FileSetup(src, ensure, strict, tb, Bar("none"), temp, log)
-
-    print(f"Auto-Editor {auto_editor.version} ({auto_editor.__version__})")
-
-    try:
-        while True:
-            text = input("> ")
-
-            try:
-                lexer = Lexer(text)
-                parser = Parser(lexer)
-            except MyError as e:
-                print(f"error: {e}")
-                continue
-
-            try:
-                interpreter = Interpreter(env, parser, filesetup)
-                for result in interpreter.interpret():
-                    if repr_result := print_str(result):
-                        sys.stdout.write(f"{repr_result}\n")
-            except (MyError, ZeroDivisionError) as e:
-                print(f"error: {e}")
+        for s, sub in enumerate(src.subtitles):
+            print(f"file: {input_file} ({s}:{sub.lang}:{sub.ext})")
+            with open(os.path.join(temp, f"{i}s{s}.{sub.ext}")) as file:
+                print(file.read())
+            print("------")
 
-    except (KeyboardInterrupt, EOFError):
-        print("")
+    log.cleanup()
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `auto-editor-23.4.1/auto_editor/subcommands/test.py` & `auto-editor-23.8.1/auto_editor/subcommands/test.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,29 +4,29 @@
 import os
 import shutil
 import subprocess
 import sys
 from dataclasses import dataclass, field
 from fractions import Fraction
 from time import perf_counter
-from typing import Callable
+from typing import Any, Callable
 
 import numpy as np
 
 from auto_editor.ffwrapper import FFmpeg, FileInfo
 from auto_editor.interpreter import (
     Char,
     Cons,
-    Interpreter,
     Lexer,
     MyError,
     Null,
     Parser,
-    Symbol,
+    Sym,
     env,
+    interpret,
 )
 from auto_editor.utils.log import Log
 from auto_editor.vanparse import ArgumentParser
 
 
 @dataclass
 class TestArgs:
@@ -36,15 +36,15 @@
 
 
 def test_options(parser):
     parser.add_argument("--only", "-n", nargs="*")
     parser.add_required(
         "category",
         nargs=1,
-        choices=("unit", "cli", "sub", "all"),
+        choices=("palet", "cli", "sub", "all"),
         metavar="category [options]",
     )
     return parser
 
 
 def pipe_to_console(cmd: list[str]) -> tuple[int, str, str]:
     process = subprocess.Popen(cmd, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
@@ -104,15 +104,17 @@
     def check(self, cmd: list[str], match=None) -> None:
         returncode, stdout, stderr = pipe_to_console(self.program + cmd)
         if returncode > 0:
             if "Error!" in stderr:
                 if match is not None and match not in stderr:
                     raise Exception(f'Could\'t find "{match}"')
             else:
-                raise Exception(f"Program crashed.\n{stdout}\n{stderr}")
+                raise Exception(
+                    f"Program crashed but should have shown an error.\n{' '.join(cmd)}\n{stdout}\n{stderr}"
+                )
         else:
             raise Exception("Program should not respond with code 0 but did!")
 
 
 def run_tests(tests: list[Callable], args: TestArgs) -> None:
     def clean_all() -> None:
         def clean(the_dir: str) -> None:
@@ -122,15 +124,15 @@
                 if item.endswith("_tracks"):
                     shutil.rmtree(os.path.join(the_dir, item))
 
         clean("resources")
         clean(os.getcwd())
 
     if args.only != []:
-        tests = filter(lambda t: t.__name__ in args.only, tests)
+        tests = list(filter(lambda t: t.__name__ in args.only, tests))
 
     total_time = 0
 
     for passed, test in enumerate(tests):
         start = perf_counter()
 
         try:
@@ -229,24 +231,24 @@
     def add_audio():
         run.main(
             ["example.mp4"],
             [
                 "--source",
                 "snd:resources/wav/pcm-f32le.wav",
                 "--add",
-                "audio:0.3sec,end,snd,volume=0.3",
+                "audio:0.3sec,end,\"snd\",volume=0.3",
             ],
         )
         return run.main(
             ["example.mp4"],
             [
                 "--source",
                 "snd:resources/wav/pcm-f32le.wav",
                 "--add",
-                "audio:2,40,snd,3sec",
+                "audio:2,40,\"snd\",3sec",
             ],
         )
 
     # PR #260
     def high_speed_test():
         return run.main(inputs=["example.mp4"], cmd=["--video-speed", "99998"])
 
@@ -372,15 +374,15 @@
         assert cn.audios[0].samplerate == 48000
 
         return out
 
     def obj_makes_video():
         out = run.main(
             ["resources/new-commentary.mp3"],
-            ["--add", "rectangle:0,30,0,0,300,300,fill=blue"],
+            ["--add", "rectangle:0,30,0,0,300,300,fill=\"blue\""],
             "out.mp4",
         )
         cn = checker.check(out)
         assert len(cn.videos) == 1
         assert len(cn.audios) == 1
         assert cn.videos[0].width == 1920
         assert cn.videos[0].height == 1080
@@ -394,56 +396,56 @@
     def render_video_objs():
         out = run.main(
             ["resources/testsrc.mp4"],
             [
                 "--mark_as_loud",
                 "start,end",
                 "--add",
-                "rectangle:0,30,0,200,100,300,fill=#43FA56,stroke=10",
+                "rectangle:0,30,0,200,100,300,fill=\"#43FA56\",stroke=10",
             ],
         )
 
         # Every element should be visible, order should be preserved.
         run.main(
             ["example.mp4"],
             [
                 "--add",
-                "ellipse:0,30,50%,50%,300,300,fill=red",
-                "rectangle:0,30,500,440,400,200,fill=skyblue",
-                "ellipse:0,30,50%,50%,100,100,fill=darkgreen",
+                "ellipse:0,30,50%,50%,300,300,fill=\"red\"",
+                "rectangle:0,30,500,440,400,200,fill=\"skyblue\"",
+                "ellipse:0,30,50%,50%,100,100,fill=\"darkgreen\"",
                 "--edit",
                 "none",
                 "--cut-out",
                 "30,end",
             ],
         )
 
         # Both ellipses should be visible
         out2 = run.main(
             ["example.mp4"],
             [
                 "--add",
-                "ellipse:0,60,50%,50%,300,300,fill=darkgreen",
-                "ellipse:0,30,50%,50%,200,200,fill=green",
+                "ellipse:0,60,50%,50%,300,300,fill=\"darkgreen\"",
+                "ellipse:0,30,50%,50%,200,200,fill=\"green\"",
                 "--edit",
                 "none",
                 "--cut-out",
                 "60,end",
             ],
         )
 
         return out, out2
 
     def render_text():
         return run.main(
-            ["example.mp4"], ["--add", "text:0,30,This is my text,font=default"]
+            ["example.mp4"], ["--add", "text:0,30,\"This is my text\",font=\"default\""]
         )
 
     def check_font_error():
-        run.check(["example.mp4", "--add", "text:0,30,text,0,0,notafont"], "not found")
+        run.check(["example.mp4", "--add", "text:0,30,\"text\",0,0,\"notafont\""], "not found")
 
     def export():
         results = set()
         all_files = (
             "aac.m4a",
             "alac.m4a",
             "wav/pcm-f32le.wav",
@@ -455,19 +457,20 @@
 
         for test_name in all_files:
             test_file = f"resources/{test_name}"
             results.add(run.main([test_file], []))
             run.main([test_file], ["--edit", "none"])
 
             p_xml = run.main([test_file], ["-exp"])
-            run.main([p_xml], [])
+            results.add(p_xml)
+            results.add(run.main([p_xml], []))
 
-            run.main([test_file], ["-exf"])
-            run.main([test_file], ["-exs"])
-            run.main([test_file], ["--export_as_clip_sequence"])
+            results.add(run.main([test_file], ["-exf"]))
+            results.add(run.main([test_file], ["-exs"]))
+            results.add(run.main([test_file], ["--export_as_clip_sequence"]))
             run.main([test_file], ["--stats"])
 
         return tuple(results)
 
     def codec_tests():
         run.main(["example.mp4"], ["--video_codec", "h264"])
         return run.main(["example.mp4"], ["--audio_codec", "ac3"])
@@ -578,19 +581,19 @@
             ["--edit", "(or (not audio:threshold=4%) (not audio:stream=1))"],
         )
         return out
 
     def edit_negative_tests():
         run.check(
             ["resources/wav/example-cut-s16le.wav", "--edit", "motion"],
-            "Video stream '0' does not exist",
+            "video stream '0' does not ",
         )
         run.check(
             ["resources/only-video/man-on-green-screen.gif", "--edit", "audio"],
-            "Audio stream '0' does not exist",
+            "audio stream '0' does not ",
         )
 
     def yuv442p():
         return run.main(["resources/test_yuv422p.mp4"], [])
 
     #  Issue 280
     def SAR():
@@ -601,16 +604,15 @@
 
     def palet():
         def cases(*cases: tuple[str, Any]) -> None:
             for text, expected in cases:
                 try:
                     parser = Parser(Lexer(text))
                     env["timebase"] = Fraction(30)
-                    interpreter = Interpreter(env, parser, None)
-                    results = interpreter.interpret()
+                    results = interpret(env, parser)
                 except MyError as e:
                     raise ValueError(f"{text}\nMyError: {e}")
 
                 if isinstance(expected, np.ndarray):
                     if not np.array_equal(expected, results[-1]):
                         raise ValueError(f"{text}: Numpy arrays don't match")
                 elif expected != results[-1]:
@@ -645,32 +647,34 @@
             ("(abs -1)", 1),
             ("(round 3.5)", 4),
             ("(round 2.5)", 2),
             ("(ceil 2.1)", 3),
             ("(ceil 2.9)", 3),
             ("(floor 2.1)", 2),
             ("(floor 2.9)", 2),
-            ("(boolean? #t)", True),
-            ("(boolean? #f)", True),
-            ("(boolean? 0)", False),
-            ("(boolean? 1)", False),
-            ("(boolean? false)", True),
-            ("(integer? 2)", True),
-            ("(integer? 3.0)", False),
-            ("(integer? #t)", False),
-            ("(integer? #f)", False),
-            ("(integer? 4/5)", False),
-            ("(integer? 0+2i)", False),
-            ('(integer? "hello")', False),
-            ('(integer? "3")', False),
+            ("(bool? #t)", True),
+            ("(bool? #f)", True),
+            ("(bool? 0)", False),
+            ("(bool? 1)", False),
+            ("(bool? false)", True),
+            ("(int? 2)", True),
+            ("(int? 3.0)", False),
+            ("(int? #t)", False),
+            ("(int? #f)", False),
+            ("(int? 4/5)", False),
+            ("(int? 0+2i)", False),
+            ('(int? "hello")', False),
+            ('(int? "3")', False),
             ("(float? -23.4)", True),
             ("(float? 3.0)", True),
             ("(float? #f)", False),
             ("(float? 4/5)", False),
             ("(float? 21)", False),
+            ("(frac? 4/5)", True),
+            ("(frac? 3.4)", False),
             ('(string-append "Hello" " World")', "Hello World"),
             ('(define apple "Red Wood") apple', "Red Wood"),
             ("(= 1 1.0)", True),
             ("(= 1 2)", False),
             ("(= 2+3i 2+3i 2+3i)", True),
             ("(= 1)", True),
             ("(+)", 0),
@@ -709,33 +713,33 @@
             ("(equal? (list 1 2 3) (list 1 2 3))", True),
             ("(equal? (list 1 2 3) (cons 1 (cons 2 (cons 3 '()))))", True),
             ("(equal? (list 1 2 3) (list 1 2 4))", False),
             (
                 "(or (bool-array 1 0 0) (bool-array 0 0 0 1))",
                 np.array([1, 0, 0, 1], dtype=np.bool_),
             ),
-            ("(quote ())", Null()),
-            ("'()", Null()),
-            ("(quote hello)", Symbol("hello")),
-            ("'hello", Symbol("hello")),
-            ("(quote (3))", Cons(3, Null())),
-            ("'(3)", Cons(3, Null())),
-            ('(quote (3 2 "apple"))', Cons(3, Cons(2, Cons("apple", Null())))),
-            ('\'(3 2 "apple")', Cons(3, Cons(2, Cons("apple", Null())))),
+            ("(quote ())", Null),
+            ("'()", Null),
+            ("(quote hello)", Sym("hello")),
+            ("'hello", Sym("hello")),
+            ("(quote (3))", Cons(3, Null)),
+            ("'(3)", Cons(3, Null)),
+            ('(quote (3 2 "apple"))', Cons(3, Cons(2, Cons("apple", Null)))),
+            ('\'(3 2 "apple")', Cons(3, Cons(2, Cons("apple", Null)))),
             ("(quote +3i)", 3j),
             ("(quote 23.4)", 23.4),
             ('(quote "hello")', "hello"),
-            ("(quote (1 (2 3)))", Cons(1, Cons(Cons(2, Cons(3, Null())), Null()))),
-            ("(list 1 2 3)", Cons(1, Cons(2, Cons(3, Null())))),
+            ("(quote (1 (2 3)))", Cons(1, Cons(Cons(2, Cons(3, Null)), Null))),
+            ("(list 1 2 3)", Cons(1, Cons(2, Cons(3, Null)))),
             ("(list-ref '(0 10 20) 2)", 20),
             ("(list-ref '(0 10 20) 0)", 0),
             ("(car (cons 3 4))", 3),
             ("(car (list 3 4))", 3),
             ("(cdr (cons 3 4))", 4),
-            ("(cdr (list 3 4))", Cons(4, Null())),
+            ("(cdr (list 3 4))", Cons(4, Null)),
             ("(length (list 1 2 3))", 3),
             ("(length '(1 2 3))", 3),
             ("(length (vector 1 2 4))", 3),
             ("(length (list))", 0),
             ("(length '())", 0),
             ("(length (bool-array 0 1 0))", 3),
             ("(equal? (reverse '(0 1 2)) '(2 1 0))", True),
@@ -751,20 +755,49 @@
             ("(for/vector ([i (vector 0 1 2)]) i)", [0, 1, 2]),
             ("(vector -20dB 0dB 20dB)", [0.1, 1, 10]),
             ("(define ca (lambda (r) (* pi (* r r)))) (ca 5)", 78.53981633974483),
             (
                 "(define ca (lambda (r) (void) (* pi (* r r)))) (ca 5)",
                 78.53981633974483,
             ),
-            ("(define my-pow2 (a) (* a a)) (my-pow2 30)", 900),
+            ("(define (my-pow2 a) (* a a)) (my-pow2 30)", 900),
+            ("(define (my-pow2 a) (void) (* a a)) (my-pow2 30)", 900),
+            ("(cond)", None),
+            ("(cond [(positive? -5) 1])", None),
+            ("(cond [(positive? 5) 3])", 3),
+            ("(cond [(positive? 5)])", True),
+            ("(cond [(positive? -5) 1] [else 2])", 2),
+            ("(cond [(positive? -5) 1] [(zero? -5) 2] [(negative? -5) 3])", 3),
+            ("(cond [else 5])", 5),
+            ("(~a 3 4 'a)", "34a"),
+            ("(~s 3 4 'a)", "3 4 a"),
+            ("(~v 3 4 'a)", "3 4 'a"),
+            ("(eval 3)", 3),
+            ('(eval "hello")', "hello"),
+            ("(eval '(+ 3 4))", 7),
+            ("(eval (list + 3 4))", 7),
+            ("(eval (vector + 3 4))", 7),
+            ("(define (my-func x) (define (inner) 4) (+ x (inner))) (my-func 16)", 20),
+            ("(var-exists? 'my-func)", True),
+            ("(var-exists? 'asdf)", False),
+            ("(define (text child ...) child)", None),
+            ("(text)", []),
+            ("(text 1)", [1]),
+            ("(text 2 1)", [2, 1]),
+            ("(text 3 2 1)", [3, 2, 1]),
+            ("((or/c 0 1) 1)", True),
+            ("((or/c 0 1) 2)", False),
+            ("((or/c 0 1) 1)", True),
+            ('((or/c 0 1 string?) "hello")', True),
+            ("((or/c 0 1 string?) 3)", False),
         )
 
     tests = []
 
-    if args.category in ("unit", "all"):
+    if args.category in ("palet", "all"):
         tests.append(palet)
 
     if args.category in ("sub", "all"):
         tests.extend([info, levels, subdump, desc])
 
     if args.category in ("cli", "all"):
         tests.extend(
```

### Comparing `auto-editor-23.4.1/auto_editor/timeline.py` & `auto-editor-23.8.1/auto_editor/timeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,27 +1,18 @@
 from __future__ import annotations
 
 from dataclasses import dataclass
 from fractions import Fraction
 from typing import Union
 
 from auto_editor.ffwrapper import FileInfo
-from auto_editor.objs.util import Attr, Required
+from auto_editor.lib.contracts import *
+from auto_editor.objs.util import Attr, Attrs, Required, smallAttr, smallAttrs
 from auto_editor.utils.chunks import Chunks, v2Chunks
-from auto_editor.utils.types import (
-    Align,
-    align,
-    anchor,
-    color,
-    db_number,
-    natural,
-    number,
-    src,
-    threshold,
-)
+from auto_editor.utils.types import Align
 
 
 @dataclass
 class v1:
     """
     v1 timeline constructor
     timebase is always the source's average fps
@@ -95,16 +86,16 @@
     name: str = "audio"
 
 
 @dataclass
 class _Visual(Tl):
     start: int
     dur: int
-    x: int
-    y: int
+    x: int | float
+    y: int | float
     anchor: str
     opacity: float
     rotate: float
     stroke: int
     strokecolor: str
 
 
@@ -136,78 +127,94 @@
 class TlEllipse(_Visual):
     width: int
     height: int
     fill: str
     name: str = "ellipse"
 
 
-video_builder = [
-    Attr("start", natural, Required),
-    Attr("dur", natural, Required),
-    Attr("src", src, Required),
-    Attr("offset", natural, 0),
-    Attr("speed", number, 1),
-    Attr("stream", natural, 0),
-]
-audio_builder = [
-    Attr("start", natural, Required),
-    Attr("dur", natural, Required),
-    Attr("src", src, Required),
-    Attr("offset", natural, 0),
-    Attr("speed", number, 1),
-    Attr("volume", db_number, 1),
-    Attr("stream", natural, 0),
-]
-text_builder = [
-    Attr("start", natural, Required),
-    Attr("dur", natural, Required),
-    Attr("content", lambda s: s.replace("\\n", "\n").replace("\\;", ","), Required),
-    Attr("x", int, "50%"),
-    Attr("y", int, "50%"),
-    Attr("font", str, "Arial"),
-    Attr("size", natural, 55),
-    Attr("align", align, "left"),
-    Attr("opacity", threshold, 1),
-    Attr("anchor", anchor, "ce"),
-    Attr("rotate", number, 0),
-    Attr("fill", str, "#FFF"),
-    Attr("stroke", natural, 0),
-    Attr("strokecolor", color, "#000"),
-]
-
-img_builder = [
-    Attr("start", natural, Required),
-    Attr("dur", natural, Required),
-    Attr("src", src, Required),
-    Attr("x", int, "50%"),
-    Attr("y", int, "50%"),
-    Attr("opacity", threshold, 1),
-    Attr("anchor", anchor, "ce"),
-    Attr("rotate", number, 0),
-    Attr("stroke", natural, 0),
-    Attr("strokecolor", color, "#000"),
-]
-
-rect_builder = [
-    Attr("start", natural, Required),
-    Attr("dur", natural, Required),
-    Attr("x", int, Required),
-    Attr("y", int, Required),
-    Attr("width", int, Required),
-    Attr("height", int, Required),
-    Attr("opacity", threshold, 1),
-    Attr("anchor", anchor, "ce"),
-    Attr("rotate", number, 0),
-    Attr("fill", color, "#c4c4c4"),
-    Attr("stroke", natural, 0),
-    Attr("strokecolor", color, "#000"),
-]
+video_builder = smallAttrs(
+    "video",
+    smallAttr("start", Required, is_uint),
+    smallAttr("dur", Required, is_uint),
+    smallAttr("src", Required, any_p),
+    smallAttr("offset", 0, is_int),
+    smallAttr("speed", 1, is_real),
+    smallAttr("stream", 0, is_uint),
+)
+audio_builder = smallAttrs(
+    "audio",
+    smallAttr("start", Required, is_uint),
+    smallAttr("dur", Required, is_uint),
+    smallAttr("src", Required, any_p),
+    smallAttr("offset", 0, is_int),
+    smallAttr("speed", 1, is_real),
+    smallAttr("volume", 1, is_real),
+    smallAttr("stream", 0, is_uint),
+)
+text_builder = smallAttrs(
+    "text",
+    smallAttr("start", Required, is_uint),
+    smallAttr("dur", Required, is_uint),
+    smallAttr("content", Required, is_str),
+    smallAttr("x", 0.5, is_real),
+    smallAttr("y", 0.5, is_real),
+    smallAttr("font", "Arial", is_str),
+    smallAttr("size", 55, is_uint),
+    smallAttr("align", "left", is_str),
+    smallAttr("opacity", 1, is_threshold),
+    smallAttr("anchor", "ce", is_str),
+    smallAttr("rotate", 0, is_real),
+    smallAttr("fill", "#FFF", is_str),
+    smallAttr("stroke", 0, is_uint),
+    smallAttr("strokecolor", "#000", is_str),
+)
+
+img_builder = smallAttrs(
+    "image",
+    smallAttr("start", Required, is_uint),
+    smallAttr("dur", Required, is_uint),
+    smallAttr("src", Required, any_p),
+    smallAttr("x", 0.5, is_real),
+    smallAttr("y", 0.5, is_real),
+    smallAttr("opacity", 1, is_threshold),
+    smallAttr("anchor", "ce", is_str),
+    smallAttr("rotate", 0, is_real),
+    smallAttr("stroke", 0, is_uint),
+    smallAttr("strokecolor", "#000", is_str),
+)
+
+rect_builder = smallAttrs(
+    "rect",
+    smallAttr("start", Required, is_uint),
+    smallAttr("dur", Required, is_uint),
+    smallAttr("x", Required, is_real),
+    smallAttr("y", Required, is_real),
+    smallAttr("width", Required, is_real),
+    smallAttr("height", Required, is_real),
+    smallAttr("opacity", 1, is_threshold),
+    smallAttr("anchor", "ce", is_str),
+    smallAttr("rotate", 0, is_real),
+    smallAttr("fill", "#c4c4c4", is_str),
+    smallAttr("stroke", 0, is_uint),
+    smallAttr("strokecolor", "#000", is_str),
+)
 ellipse_builder = rect_builder
+visual_objects = {
+    "rectangle": (TlRect, rect_builder),
+    "ellipse": (TlEllipse, ellipse_builder),
+    "text": (TlText, text_builder),
+    "image": (TlImage, img_builder),
+    "video": (TlVideo, video_builder),
+}
+
+audio_objects = {
+    "audio": (TlAudio, audio_builder),
+}
 
-timeline_builder = [Attr("api", str, "3.0.0")]
+timeline_builder = Attrs("timeline", Attr("api", str, "3.0.0"))
 
 Visual = Union[TlText, TlImage, TlRect, TlEllipse]
 VLayer = list[Union[TlVideo, Visual]]
 VSpace = list[VLayer]
 
 ALayer = list[TlAudio]
 ASpace = list[ALayer]
@@ -281,20 +288,7 @@
                 "samplerate": self.sr,
                 "sources": sources,
                 "background": self.background,
                 "v": v,
                 "a": a,
             },
         }
-
-
-visual_objects = {
-    "rectangle": (TlRect, rect_builder),
-    "ellipse": (TlEllipse, ellipse_builder),
-    "text": (TlText, text_builder),
-    "image": (TlImage, img_builder),
-    "video": (TlVideo, video_builder),
-}
-
-audio_objects = {
-    "audio": (TlAudio, audio_builder),
-}
```

### Comparing `auto-editor-23.4.1/auto_editor/utils/bar.py` & `auto-editor-23.8.1/auto_editor/utils/bar.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/utils/chunks.py` & `auto-editor-23.8.1/auto_editor/utils/chunks.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 Chunk = tuple[int, int, float]
 Chunks = list[Chunk]
 
 v2Chunk = tuple[int, int, float, int]
 v2Chunks = list[v2Chunk]
 
+
 # Turn long silent/loud array to formatted chunk list.
 # Example: [1, 1, 1, 2, 2], {1: 1.0, 2: 1.5} => [(0, 3, 1.0), (3, 5, 1.5)]
 def chunkify(arr: NDArray, smap: dict[int, float]) -> Chunks:
     arr_length = len(arr)
 
     chunks = []
     start = 0
```

### Comparing `auto-editor-23.4.1/auto_editor/utils/container.py` & `auto-editor-23.8.1/auto_editor/utils/container.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/utils/encoder.py` & `auto-editor-23.8.1/auto_editor/utils/encoder.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/utils/func.py` & `auto-editor-23.8.1/auto_editor/utils/func.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/utils/log.py` & `auto-editor-23.8.1/auto_editor/utils/log.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/utils/types.py` & `auto-editor-23.8.1/auto_editor/utils/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -216,15 +216,15 @@
     raise CoerceError("Align must be 'left', 'right', or 'center'")
 
 
 Stream = Union[int, Literal["all"]]
 
 
 def stream(val: str) -> Stream:
-    if val == "all":
+    if val == "all" or val == "'all":
         return "all"
     return natural(val)
 
 
 def color(val: str) -> str:
     """
     Convert a color str into an RGB tuple
```

### Comparing `auto-editor-23.4.1/auto_editor/validate_input.py` & `auto-editor-23.8.1/auto_editor/validate_input.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/vanparse.py` & `auto-editor-23.8.1/auto_editor/vanparse.py`

 * *Files identical despite different names*

### Comparing `auto-editor-23.4.1/auto_editor/wavfile.py` & `auto-editor-23.8.1/auto_editor/wavfile.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
     format_tag: int,
     channels: int,
     bit_depth: int,
     en: Endian,
     block_align: int,
     data_size: int | None,
 ) -> AudioData:
-
     size: int = struct.unpack(f"{en}I", fid.read(4))[0]
     if data_size is not None:
         # size is only 32-bits here, so get real size from header.
         size = data_size
 
     bytes_per_sample = block_align // channels
     n_samples = size // bytes_per_sample
@@ -122,15 +121,14 @@
     if data := fid.read(4):
         size = struct.unpack(f"{en}I", data)[0]
         fid.seek(size, 1)
         _handle_pad_byte(fid, size)
 
 
 def _read_rf64_chunk(fid: io.BufferedReader) -> tuple[int, int, Endian]:
-
     # https://tech.ebu.ch/docs/tech/tech3306v1_0.pdf
     # https://www.itu.int/dms_pubrec/itu-r/rec/bs/R-REC-BS.2088-1-201910-I!!PDF-E.pdf
 
     heading = fid.read(12)
     if heading != b"\xff\xff\xff\xffWAVEds64":
         raise ValueError(f"Wrong heading: {heading!r}")
```

### Comparing `auto-editor-23.4.1/auto_editor.egg-info/PKG-INFO` & `auto-editor-23.8.1/auto_editor.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-editor
-Version: 23.4.1
+Version: 23.8.1
 Summary: Auto-Editor: Effort free video editing!
 Home-page: https://auto-editor.com
 Author: WyattBlue
 Author-email: wyattblue@auto-editor.com
 License: Unlicense
 Project-URL: Bug Tracker, https://github.com/WyattBlue/auto-editor/issues
 Project-URL: Source Code, https://github.com/WyattBlue/auto-editor
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: auto-editor Version: 23.4.1 Summary: Auto-Editor:
+Metadata-Version: 2.1 Name: auto-editor Version: 23.8.1 Summary: Auto-Editor:
 Effort free video editing! Home-page: https://auto-editor.com Author: WyattBlue
 Author-email: wyattblue@auto-editor.com License: Unlicense Project-URL: Bug
 Tracker, https://github.com/WyattBlue/auto-editor/issues Project-URL: Source
 Code, https://github.com/WyattBlue/auto-editor Keywords: video audio media
 editor editing processing nonlinear automatic silence-detect silence-removal
 silence-speedup motion-detection Classifier: Topic :: Multimedia :: Sound/Audio
 Classifier: Topic :: Multimedia :: Video Classifier: License :: Public Domain
```

### Comparing `auto-editor-23.4.1/auto_editor.egg-info/SOURCES.txt` & `auto-editor-23.8.1/auto_editor.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -25,27 +25,29 @@
 auto_editor.egg-info/zip-safe
 auto_editor/formats/__init__.py
 auto_editor/formats/final_cut_pro.py
 auto_editor/formats/json.py
 auto_editor/formats/premiere.py
 auto_editor/formats/shotcut.py
 auto_editor/formats/utils.py
+auto_editor/lib/__init__.py
+auto_editor/lib/contracts.py
 auto_editor/objs/__init__.py
 auto_editor/objs/edit.py
-auto_editor/objs/export.py
 auto_editor/objs/util.py
 auto_editor/render/__init__.py
 auto_editor/render/audio.py
 auto_editor/render/image.py
 auto_editor/render/subtitle.py
 auto_editor/render/video.py
 auto_editor/subcommands/__init__.py
 auto_editor/subcommands/desc.py
 auto_editor/subcommands/info.py
 auto_editor/subcommands/levels.py
+auto_editor/subcommands/palet.py
 auto_editor/subcommands/repl.py
 auto_editor/subcommands/subdump.py
 auto_editor/subcommands/test.py
 auto_editor/utils/__init__.py
 auto_editor/utils/bar.py
 auto_editor/utils/chunks.py
 auto_editor/utils/container.py
```

### Comparing `auto-editor-23.4.1/setup.py` & `auto-editor-23.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import re
 
 from setuptools import find_packages, setup
 
 
 def pip_version():
-    with open("auto_editor/__init__.py") as f:
-        version_content = f.read()
+    with open("auto_editor/__init__.py") as f: version_content = f.read()
 
     version_match = re.search(
         r"^__version__ = ['\"]([^'\"]*)['\"]", version_content, re.M
     )
 
     if version_match:
         return version_match.group(1)
@@ -38,15 +37,15 @@
     "silence-detect silence-removal silence-speedup motion-detection",
     packages=find_packages(),
     zip_safe=True,
     install_requires=[
         "numpy>=1.22.0",
         "pillow==9.4.0",
         "av==10.0.0",
-        "ae-ffmpeg==1.1.1",
+        "ae-ffmpeg==1.1.*",
     ],
     python_requires=">=3.9",
     classifiers=[
         "Topic :: Multimedia :: Sound/Audio",
         "Topic :: Multimedia :: Video",
         "License :: Public Domain",
         "License :: OSI Approved :: The Unlicense (Unlicense)",
```

