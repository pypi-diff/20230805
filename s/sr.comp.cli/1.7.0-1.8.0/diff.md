# Comparing `tmp/sr.comp.cli-1.7.0.tar.gz` & `tmp/sr.comp.cli-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sr.comp.cli-1.7.0.tar", last modified: Sat Feb 18 23:08:06 2023, max compression
+gzip compressed data, was "dist/sr.comp.cli-1.8.0.tar", last modified: Sat Aug  5 16:21:11 2023, max compression
```

## Comparing `sr.comp.cli-1.7.0.tar` & `sr.comp.cli-1.8.0.tar`

### file list

```diff
@@ -1,63 +1,62 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2176 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      789 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      419 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      943 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1789 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr/comp/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr/comp/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5201 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/add_delay.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1673 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/awards.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2538 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/command_line.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1611 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/delay.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9780 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/deploy.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1303 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/fetch.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4518 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/for_each_match.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4307 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5986 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/core.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3215 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/loading.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/teams_mapping.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/types.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1439 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/knocked_out_teams.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10090 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/league_scheduler.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/lighting_controller.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/list_midi_ports.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/match_order_teams.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10717 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/print_schedule.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3715 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/schedule_league.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1821 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/scorer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/shift_matches.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2410 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/show_league_table.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2359 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/show_schedule.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1673 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/summary.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1803 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/top_match_points.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2287 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/update_layout.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      821 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/validate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1595 2023-02-18 23:07:56.000000 sr.comp.cli-1.7.0/sr/comp/cli/yaml_round_trip.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2176 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1458 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/namespace_packages.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       26 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/sr.comp.cli.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/venv/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-02-18 23:08:06.000000 sr.comp.cli-1.7.0/venv/bin/
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      615 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2html.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      737 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2html4.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2html5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      814 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2latex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      637 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2man.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      803 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2odt.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1741 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2odt_prepstyles.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      622 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2pseudoxml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      658 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2s5.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      894 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2xetex.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      623 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rst2xml.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      691 2023-02-18 23:08:05.000000 sr.comp.cli-1.7.0/venv/bin/rstpep2html.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2176 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      789 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      970 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1809 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr/comp/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr/comp/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5256 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/add_delay.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1728 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/awards.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2631 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/command_line.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/delay.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9781 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/deploy.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1304 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/fetch.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4518 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/for_each_match.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4482 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5986 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/core.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3215 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/loading.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2819 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/teams_mapping.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      691 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/types.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/knocked_out_teams.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10090 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/league_scheduler.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5114 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/lighting_controller.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      583 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/list_midi_ports.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1508 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/match_order_teams.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11039 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/print_schedule.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3770 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/schedule_league.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1825 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/scorer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1748 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/shift_matches.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2411 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/show_league_table.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3344 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/show_schedule.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1674 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/summary.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1804 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/top_match_points.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2363 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/update_layout.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/validate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1622 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/yaml_round_trip.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2861 2023-08-05 16:21:01.000000 sr.comp.cli-1.8.0/sr/comp/cli/youtube_chapters.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2176 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1477 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       58 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       11 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      170 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/sr.comp.cli.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/venv/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-08-05 16:21:11.000000 sr.comp.cli-1.8.0/venv/bin/
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      625 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2html.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      747 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2html4.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1082 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2html5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      824 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2latex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      647 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2man.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      813 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2odt.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      619 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2odt_prepstyles.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      632 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2pseudoxml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      668 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2s5.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      904 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2xetex.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      633 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rst2xml.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      701 2023-08-05 16:21:09.000000 sr.comp.cli-1.8.0/venv/bin/rstpep2html.py
```

### Comparing `sr.comp.cli-1.7.0/PKG-INFO` & `sr.comp.cli-1.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sr.comp.cli
-Version: 1.7.0
+Version: 1.8.0
 Summary: Command line tools for interacting with the state of the Student Robotics Competition
 Home-page: UNKNOWN
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp-cli.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp-cli
```

### Comparing `sr.comp.cli-1.7.0/README.rst` & `sr.comp.cli-1.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/setup.cfg` & `sr.comp.cli-1.8.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -25,14 +25,15 @@
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

### Comparing `sr.comp.cli-1.7.0/setup.py` & `sr.comp.cli-1.8.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_namespace_packages, setup
 
 with open('README.rst') as f:
     long_description = f.read()
 
 setup(
     name='sr.comp.cli',
-    version='1.7.0',
+    version='1.8.0',
     project_urls={
         'Documentation': 'https://srcomp-cli.readthedocs.org/',
         'Code': 'https://github.com/PeterJCLaw/srcomp-cli',
         'Issue tracker': 'https://github.com/PeterJCLaw/srcomp-cli/issues',
     },
-    packages=find_namespace_packages(exclude=('tests',)),
+    packages=find_namespace_packages(exclude=('docs*', 'script*', 'tests*')),
     namespace_packages=['sr', 'sr.comp'],
     description=(
         "Command line tools for interacting with the state of the Student "
         "Robotics Competition"
     ),
     long_description=long_description,
     author="Student Robotics Competition Software SIG",
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/add_delay.py` & `sr.comp.cli-1.8.0/sr/comp/cli/add_delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,17 +150,19 @@
             "as a number of seconds or a string of the form 1m30s. "
             "Assumes all times are in the current timezone, regardless of input."
         ),
     )
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Add a delay the competition state."
     parser = subparsers.add_parser(
         'add-delay',
-        help="Add a delay the competition state",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument(
         'compstate',
         type=Path,
         help="competition state repository",
     )
     add_arguments(parser)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/awards.py` & `sr.comp.cli-1.8.0/sr/comp/cli/awards.py`

 * *Files 13% similar despite different names*

```diff
@@ -48,13 +48,15 @@
             print(f'  Split between {len(recipients)} teams (a tie):')
             for recipient in recipients:
                 print("  ", format_team(recipient))
         print()
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Show who has been given awards."
     parser = subparsers.add_parser(
         'awards',
-        help="show who has been given awards",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument('compstate', help="competition state repo")
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/command_line.py` & `sr.comp.cli-1.8.0/sr/comp/cli/command_line.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,26 +24,27 @@
     show_league_table,
     show_schedule,
     summary,
     top_match_points,
     update_layout,
     validate,
     yaml_round_trip,
+    youtube_chapters,
 )
 
 
 def add_list_commands(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     def command(settings: argparse.Namespace) -> None:
         commands = subparsers.choices.keys()
         print(" ".join(commands))
 
     help_text = "Lists the available commands; useful for adding " \
-                "auto-completion of command names"
+                "auto-completion of command names."
 
-    parser = subparsers.add_parser('list-commands', help=help_text)
+    parser = subparsers.add_parser('list-commands', help=help_text, description=help_text)
     parser.set_defaults(func=command)
 
 
 def argument_parser() -> argparse.ArgumentParser:
     """A parser for CLI tool command line arguments, from argparse."""
     parser = argparse.ArgumentParser(description="srcomp command-line interface")
     subparsers = parser.add_subparsers(title="commands")
@@ -67,14 +68,15 @@
     show_league_table.add_subparser(subparsers)
     show_schedule.add_subparser(subparsers)
     summary.add_subparser(subparsers)
     top_match_points.add_subparser(subparsers)
     update_layout.add_subparser(subparsers)
     validate.add_subparser(subparsers)
     yaml_round_trip.add_subparser(subparsers)
+    youtube_chapters.add_subparser(subparsers)
 
     return parser
 
 
 def main(args: list[str] | None = None) -> None:
     """Run as the CLI tool."""
     if args is None:
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/delay.py` & `sr.comp.cli-1.8.0/sr/comp/cli/delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         msg = f"Adding {args.how_long} delay at {when}"
         compstate.commit(msg)
 
     deploy.run_deployments(args, compstate, hosts)
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
-    help_msg = "Add and deploy a delay to the competition"
+    help_msg = "Add and deploy a delay to the competition."
     parser = subparsers.add_parser('delay', help=help_msg, description=help_msg)
     parser.add_argument(
         '--no-pull',
         action='store_true',
         help="skips updating to the latest revision",
     )
     deploy.add_options(parser)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/deploy.py` & `sr.comp.cli-1.8.0/sr/comp/cli/deploy.py`

 * *Files 1% similar despite different names*

```diff
@@ -319,15 +319,15 @@
         '--skip-host-check',
         action='store_true',
         help="skips checking the current state of the hosts",
     )
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
-    help_msg = "Deploy a given competition state to all known hosts"
+    help_msg = "Deploy a given competition state to all known hosts."
     parser = subparsers.add_parser(
         'deploy',
         help=help_msg,
         description=help_msg,
     )
     add_options(parser)
     parser.add_argument('compstate', help="competition state repository")
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/fetch.py` & `sr.comp.cli-1.8.0/sr/comp/cli/fetch.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             continue
 
         compstate.fetch(ref_compstate(host), [state], quiet=True)
         print(f"{ENDC}{state} fetched.")
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
-    help_msg = "Fetch the deployed versions from all known hosts"
+    help_msg = "Fetch the deployed versions from all known hosts."
     parser = subparsers.add_parser(
         'fetch',
         help=help_msg,
         description=help_msg,
     )
     parser.add_argument('compstate', help="competition state repository")
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/for_each_match.py` & `sr.comp.cli-1.8.0/sr/comp/cli/for_each_match.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/__init__.py` & `sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,17 @@
 
 Whitespace (other than newlines) within the file is ignored, as is any
 content to the right of a hash character (#), including the hash. As a
 result hash characters may be used to start line comments.
 
 Example schedules for 48, 52 or 56 teams are available  at:
 https://github.com/PeterJCLaw/srobo-schedules/tree/master/seed_schedules
+
+Teams which are marked as having dropped out before the first match being
+scheduled will not be considered for inclusion in the schedule.
 """
 
 from __future__ import annotations
 
 import argparse
 from pathlib import Path
 from typing import Iterable
@@ -99,23 +102,23 @@
     # Save the matches to the file
     loading.dump_league_yaml({**existing_matches, **matches}, league_yaml)
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     parser = subparsers.add_parser(
         'import-schedule',
-        help="Import a league.yaml file from a schedule file",
+        help="Import a league.yaml file from a schedule file.",
         description=__doc__,
         formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument(
         '-i',
         '--ignore-ids',
         type=loading.parse_ids,
-        help="comma separated list of ids to ignore",
+        help="Comma separated list of ids (as present in the schedule file) to ignore.",
     )
     parser.add_argument(
         '--extend',
         default=False,
         action='store_true',
         help=(
             "Whether to replace (the default) or extend the existing league "
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/core.py` & `sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/core.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/loading.py` & `sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/loading.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/teams_mapping.py` & `sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/teams_mapping.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/import_schedule/types.py` & `sr.comp.cli-1.8.0/sr/comp/cli/import_schedule/types.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/knocked_out_teams.py` & `sr.comp.cli-1.8.0/sr/comp/cli/knocked_out_teams.py`

 * *Files 22% similar despite different names*

```diff
@@ -34,17 +34,19 @@
         for tla in teams_out:
             print(tla, comp.teams[tla].name)
         teams_last_round = teams_this_round
         print()
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Show the teams knocked out of each knockout round."
     parser = subparsers.add_parser(
         'knocked-out-teams',
-        help="show the teams knocked out of each knockout round",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument(
         'compstate',
         help="competition state repository",
         type=Path,
     )
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/league_scheduler.py` & `sr.comp.cli-1.8.0/sr/comp/cli/league_scheduler.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/lighting_controller.py` & `sr.comp.cli-1.8.0/sr/comp/cli/lighting_controller.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/list_midi_ports.py` & `sr.comp.cli-1.8.0/sr/comp/cli/list_midi_ports.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/match_order_teams.py` & `sr.comp.cli-1.8.0/sr/comp/cli/match_order_teams.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/print_schedule.py` & `sr.comp.cli-1.8.0/sr/comp/cli/print_schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
+"""
+Produce a PDF shepherding sheet, suitable for printing.
+
+The shepherds file should contain a key called ``shepherds`` which is a list of
+objects containing a ``teams`` and ``colour`` field, with an optional ``name``
+field.
+"""
+
 from __future__ import annotations
 
 import argparse
-from collections import defaultdict
+import collections
 
 
 class ScheduleGenerator:
     def __init__(self, target, arenas, state):
         from reportlab.pdfgen import canvas  # type: ignore[import]
 
         self.canvas = canvas.Canvas(target)
@@ -228,15 +236,15 @@
             include_locations_in_title,
         )
         self.start_page(title)
 
         n = 0
         for slot in period.matches:
             # Build map of shepherd id -> total teams they need to fetch this slot
-            shepherd_counts = defaultdict(int)
+            shepherd_counts = collections.defaultdict(int)
             for match in slot.values():
                 for team in match.teams:
                     num = find_shepherd_number(team)
                     if num is not None:
                         shepherd_counts[num] += 1
 
             if self._match_suitable_for_locations(slot, locations):
@@ -317,15 +325,17 @@
 
     generator.write()
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
     parser = subparsers.add_parser(
         'print-schedule',
-        help="print a shepherding sheet",
+        help=__doc__.strip().splitlines()[0],
+        description=__doc__,
+        formatter_class=argparse.RawDescriptionHelpFormatter,
     )
     parser.add_argument('compstate', help="competition state repository")
     parser.add_argument(
         '-o',
         '--output',
         help="output file",
         type=argparse.FileType('wb'),
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/schedule_league.py` & `sr.comp.cli-1.8.0/sr/comp/cli/schedule_league.py`

 * *Files 3% similar despite different names*

```diff
@@ -74,17 +74,19 @@
         pool.join()
     else:
         output_data = scheduler.run()
         yaml.dump({'matches': output_data}, dest=sys.stdout)
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Generate a schedule for a league."
     parser = subparsers.add_parser(
         'schedule-league',
-        help="generate a schedule for a league",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument(
         'compstate',
         type=Path,
         help="competition state git repository",
     )
     parser.add_argument(
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/scorer.py` & `sr.comp.cli-1.8.0/sr/comp/cli/scorer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-Run the SRComp Scorer UI. Requires sr.comp.scorer to be installed.
+Run the SRComp Scorer UI. Requires ``sr.comp.scorer`` to be installed.
 """
 
 from __future__ import annotations
 
 import argparse
 from typing import cast
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/shift_matches.py` & `sr.comp.cli-1.8.0/sr/comp/cli/shift_matches.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/show_league_table.py` & `sr.comp.cli-1.8.0/sr/comp/cli/show_league_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Show the current state of the league table"""
+"""Show the current state of the league table."""
 
 from __future__ import annotations
 
 import argparse
 from typing import Any, Callable, NamedTuple
 
 from league_ranker import LeaguePoints
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/show_schedule.py` & `sr.comp.cli-1.8.0/sr/comp/cli/show_schedule.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,24 @@
 from __future__ import annotations
 
 import argparse
+import enum
 
 DISPLAY_NAME_WIDTH = 18
 
 
+class SecondsOption(enum.Enum):
+    ALWAYS = 'always'
+    NEVER = 'never'
+    AUTO = 'auto'
+
+    def __str__(self) -> str:
+        return self.value
+
+
 def first(iterable):
     return next(i for i in iterable)
 
 
 def command(settings: argparse.Namespace) -> None:
     import os.path
     from datetime import datetime, timedelta
@@ -36,27 +46,47 @@
 
     def teams_str(teams):
         return ":".join(tla.center(5) if tla else "  -  " for tla in teams)
 
     def print_col(text, last=False):
         print(text, end='|')
 
+    def should_show_seconds() -> bool:
+        if settings.seconds == SecondsOption.ALWAYS:
+            return True
+        if settings.seconds == SecondsOption.NEVER:
+            return False
+
+        assert settings.seconds == SecondsOption.AUTO
+        for slot in matches:
+            for match in slot.values():
+                if match.start_time.second != 0:
+                    return True
+
+        return False
+
+    time_format = '%H:%M'
+    time_space = ""
+    if should_show_seconds():
+        time_format += ':%S'
+        time_space = "   "
+
     empty_teams = teams_str(" " * num_teams_per_arena)
     teams_len = len(empty_teams)
 
-    print_col(" Num Time  ")
+    print_col(f" Num Time  {time_space}")
     for a in comp.arenas.values():
         print_col(a.display_name.center(teams_len))
     print_col("Display Name".center(DISPLAY_NAME_WIDTH))
     print()
 
     arena_ids = comp.arenas.keys()
     for slot in matches:
         m = first(slot.values())
-        print_col(f" {m.num:>3} {m.start_time:%H:%M} ")
+        print_col(f" {m.num:>3} {m.start_time:{time_format}} ")
 
         for a_id in arena_ids:
             if a_id in slot:
                 print_col(teams_str(slot[a_id].teams))
             else:
                 print_col(empty_teams)
 
@@ -65,26 +95,35 @@
         if m in current_matches:
             print(" *")
         else:
             print()
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Show the match schedule."
     parser = subparsers.add_parser(
         'show-schedule',
-        help="show the match schedule",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument(
         'compstate',
         help="competition state repo",
     )
     parser.add_argument(
         '--all',
         action='store_true',
         help="show all matches, not just the upcoming ones (ignores --limit)",
     )
     parser.add_argument(
+        '--seconds',
+        help="show times including seconds",
+        choices=SecondsOption,
+        type=SecondsOption,
+        default=SecondsOption.AUTO,
+    )
+    parser.add_argument(
         '--limit',
         default=15,
         help="how many matches to show (default: %(default)s)",
     )
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/summary.py` & `sr.comp.cli-1.8.0/sr/comp/cli/summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,12 +52,12 @@
     print("Number of games: {} ({})".format(
         sum(games_by_type.values()),
         games_by_type_str,
     ))
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
-    help_msg = "Show summary data about a compstate"
+    help_msg = "Show summary data about a compstate."
 
     parser = subparsers.add_parser('summary', help=help_msg, description=help_msg)
     parser.add_argument('compstate', help="competition state repository")
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/top_match_points.py` & `sr.comp.cli-1.8.0/sr/comp/cli/top_match_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import argparse
 from pathlib import Path
 from typing import DefaultDict
 
 from sr.comp.types import GamePoints, MatchId, TLA
 
-__description__ = "Summaries the teams scoring the most match points"
+__description__ = "Summaries the teams scoring the most match points."
 
 
 def command(settings: argparse.Namespace) -> None:
     from collections import defaultdict
     from itertools import chain
 
     from sr.comp.comp import SRComp
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/update_layout.py` & `sr.comp.cli-1.8.0/sr/comp/cli/update_layout.py`

 * *Files 10% similar despite different names*

```diff
@@ -62,15 +62,19 @@
 
     yaml.dump(layout, dest=layout_yaml)
 
     print("Layout updated. You should consider re-importing the schedule now.")
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
-    parser = subparsers.add_parser('update-layout', help=__doc__)
+    parser = subparsers.add_parser(
+        'update-layout',
+        help=__doc__.strip().splitlines()[0],
+        description=__doc__,
+    )
     parser.add_argument(
         'compstate',
         help="competition state repository",
         type=Path,
     )
     parser.add_argument(
         'teams_list',
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/validate.py` & `sr.comp.cli-1.8.0/sr/comp/cli/validate.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,18 +14,21 @@
     else:
         error_count = validate(comp)
 
     exit(error_count)
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Check that the compstate can be loaded and represents a valid state."
     parser = subparsers.add_parser(
         'validate',
-        help="validate the state of a compstate repository",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument('compstate', help="competition state repository")
     parser.add_argument(
-        '-l', '--lax',
+        '-l',
+        '--lax',
         action='store_true',
         help="only check if it loads, rather than run a validation",
     )
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr/comp/cli/yaml_round_trip.py` & `sr.comp.cli-1.8.0/sr/comp/cli/yaml_round_trip.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def _load() -> ruamel.yaml.YAML:
     global _ryaml
     if _ryaml is None:
         import ruamel.yaml
 
         _ryaml = ruamel.yaml.YAML()
-        _ryaml.version = (1, 1)  # type: ignore[assignment]
+        _ryaml.version = (1, 1)
 
         from sr.comp.yaml_loader import add_time_constructor
         add_time_constructor(_ryaml.Constructor)
 
     return _ryaml
 
 
@@ -50,17 +50,19 @@
 
 def command(settings: argparse.Namespace) -> None:
     fp = settings.file_path
     dump(load(fp), dest=fp)
 
 
 def add_subparser(subparsers: argparse._SubParsersAction[argparse.ArgumentParser]) -> None:
+    help_msg = "Round-trip a yaml file using compstate loading."
     parser = subparsers.add_parser(
         'round-trip',
-        help="Round-trip a yaml file using compstate loading",
+        help=help_msg,
+        description=help_msg,
     )
     parser.add_argument(
         'file_path',
         help="target file to round trip",
         type=Path,
     )
     parser.set_defaults(func=command)
```

### Comparing `sr.comp.cli-1.7.0/sr.comp.cli.egg-info/PKG-INFO` & `sr.comp.cli-1.8.0/sr.comp.cli.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: sr.comp.cli
-Version: 1.7.0
+Version: 1.8.0
 Summary: Command line tools for interacting with the state of the Student Robotics Competition
 Home-page: UNKNOWN
 Author: Student Robotics Competition Software SIG
 Author-email: srobo-devel@googlegroups.com
 License: UNKNOWN
 Project-URL: Documentation, https://srcomp-cli.readthedocs.org/
 Project-URL: Code, https://github.com/PeterJCLaw/srcomp-cli
```

### Comparing `sr.comp.cli-1.7.0/sr.comp.cli.egg-info/SOURCES.txt` & `sr.comp.cli-1.8.0/sr.comp.cli.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.rst
 setup.cfg
 setup.py
-docs/conf.py
 sr.comp.cli.egg-info/PKG-INFO
 sr.comp.cli.egg-info/SOURCES.txt
 sr.comp.cli.egg-info/dependency_links.txt
 sr.comp.cli.egg-info/entry_points.txt
 sr.comp.cli.egg-info/namespace_packages.txt
 sr.comp.cli.egg-info/requires.txt
 sr.comp.cli.egg-info/top_level.txt
@@ -30,14 +29,15 @@
 sr/comp/cli/show_league_table.py
 sr/comp/cli/show_schedule.py
 sr/comp/cli/summary.py
 sr/comp/cli/top_match_points.py
 sr/comp/cli/update_layout.py
 sr/comp/cli/validate.py
 sr/comp/cli/yaml_round_trip.py
+sr/comp/cli/youtube_chapters.py
 sr/comp/cli/import_schedule/__init__.py
 sr/comp/cli/import_schedule/core.py
 sr/comp/cli/import_schedule/loading.py
 sr/comp/cli/import_schedule/teams_mapping.py
 sr/comp/cli/import_schedule/types.py
 venv/bin/rst2html.py
 venv/bin/rst2html4.py
```

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2html.py` & `sr.comp.cli-1.8.0/venv/bin/rst2html.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2html4.py` & `sr.comp.cli-1.8.0/venv/bin/rst2html4.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2html5.py` & `sr.comp.cli-1.8.0/venv/bin/rst2html5.py`

 * *Files identical despite different names*

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2latex.py` & `sr.comp.cli-1.8.0/venv/bin/rst2latex.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2man.py` & `sr.comp.cli-1.8.0/venv/bin/rst2man.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2odt.py` & `sr.comp.cli-1.8.0/venv/bin/rst2odt.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2pseudoxml.py` & `sr.comp.cli-1.8.0/venv/bin/rst2pseudoxml.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2s5.py` & `sr.comp.cli-1.8.0/venv/bin/rst2s5.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2xetex.py` & `sr.comp.cli-1.8.0/venv/bin/rst2xetex.py`

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

### Comparing `sr.comp.cli-1.7.0/venv/bin/rst2xml.py` & `sr.comp.cli-1.8.0/venv/bin/rstpep2html.py`

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

