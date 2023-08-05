# Comparing `tmp/bimmer_connected-0.9.5.tar.gz` & `tmp/bimmer_connected-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bimmer_connected-0.9.5.tar", last modified: Wed Jun 22 11:55:31 2022, max compression
+gzip compressed data, was "bimmer_connected-0.9.6.tar", last modified: Sat Jun 25 07:44:27 2022, max compression
```

## Comparing `bimmer_connected-0.9.5.tar` & `bimmer_connected-0.9.6.tar`

### file list

```diff
@@ -1,151 +1,138 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.612770 bimmer_connected-0.9.5/
--rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.584770 bimmer_connected-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.584770 bimmer_connected-0.9.5/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.588770 bimmer_connected-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/workflows/lock.yml
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (121)      395 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/workflows/stale.yml
--rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)      403 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      819 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/ChangeLog
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     8378 2022-06-22 11:55:31.612770 bimmer_connected-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7317 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.588770 bimmer_connected-0.9.5/bimmer_connected/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/account.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.588770 bimmer_connected-0.9.5/bimmer_connected/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    15793 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     3496 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/api/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/api/regions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3698 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/api/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    11244 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     2416 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/const.py
--rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/coord_convert.py
--rw-r--r--   0 runner    (1001) docker     (121)     4091 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/models.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     3295 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.592770 bimmer_connected-0.9.5/bimmer_connected/vehicle/
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4538 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/charging_profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     3640 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/doors_windows.py
--rw-r--r--   0 runner    (1001) docker     (121)     7542 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/fuel_and_battery.py
--rw-r--r--   0 runner    (1001) docker     (121)     3869 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/location.py
--rw-r--r--   0 runner    (1001) docker     (121)     9982 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/remote_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     4046 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)    12467 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)     9546 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/bimmer_connected/vehicle/vehicle_status.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.588770 bimmer_connected-0.9.5/bimmer_connected.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8378 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/pbr.json
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-22 11:55:31.000000 bimmer_connected-0.9.5/bimmer_connected.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.592770 bimmer_connected-0.9.5/docs/
--rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.592770 bimmer_connected-0.9.5/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.600770 bimmer_connected-0.9.5/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/_static/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)  1601424 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/_static/Intercepting Flutter traffic on Android (ARMv8) – NVISO Labs.pdf
--rw-r--r--   0 runner    (1001) docker     (121)  2954479 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/_static/Intercepting Flutter traffic on iOS – NVISO Labs.pdf
--rw-r--r--   0 runner    (1001) docker     (121)  2852017 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/_static/Intercepting traffic from Android Flutter applications – NVISO Labs.pdf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.600770 bimmer_connected-0.9.5/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/_templates/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5320 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.604770 bimmer_connected-0.9.5/docs/source/development/
--rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/development/fingerprints_in_homeassistant.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6768 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/development/reverse_engineering_mybmw.rst
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.604770 bimmer_connected-0.9.5/docs/source/module/
--rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/module/account.rst
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/module/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/module/const.rst
--rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/module/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/module/utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/module/vehicle.rst
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/docs/source/readme.rst
--rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/requirements-test.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)       37 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-06-22 11:55:31.612770 bimmer_connected-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.604770 bimmer_connected-0.9.5/test/
--rw-r--r--   0 runner    (1001) docker     (121)    10760 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.584770 bimmer_connected-0.9.5/test/responses/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.604770 bimmer_connected-0.9.5/test/responses/F11/
--rw-r--r--   0 runner    (1001) docker     (121)     8937 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/F11/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.604770 bimmer_connected-0.9.5/test/responses/F31/
--rw-r--r--   0 runner    (1001) docker     (121)     9079 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/F31/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.604770 bimmer_connected-0.9.5/test/responses/F44/
--rw-r--r--   0 runner    (1001) docker     (121)     7697 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/F44/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/F45/
--rw-r--r--   0 runner    (1001) docker     (121)     9550 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/F45/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/F48/
--rw-r--r--   0 runner    (1001) docker     (121)     8848 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/F48/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/G01/
--rw-r--r--   0 runner    (1001) docker     (121)    12703 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G01/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/G05/
--rw-r--r--   0 runner    (1001) docker     (121)    11886 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G05/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/G08/
--rw-r--r--   0 runner    (1001) docker     (121)    11985 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G08/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/G21/
--rw-r--r--   0 runner    (1001) docker     (121)     3214 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G21/charging-sessions_0.json
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G21/charging-statistics_0.json
--rw-r--r--   0 runner    (1001) docker     (121)    29411 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G21/json_export.json
--rw-r--r--   0 runner    (1001) docker     (121)    16226 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G21/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/G23/
--rw-r--r--   0 runner    (1001) docker     (121)    16260 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G23/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/G30/
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G30/charging-sessions_0.json
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G30/charging-statistics_0.json
--rw-r--r--   0 runner    (1001) docker     (121)    11304 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/G30/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/I01_NOREX/
--rw-r--r--   0 runner    (1001) docker     (121)      582 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/I01_NOREX/charging-sessions_0.json
--rw-r--r--   0 runner    (1001) docker     (121)      354 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/I01_NOREX/charging-statistics_0.json
--rw-r--r--   0 runner    (1001) docker     (121)     9745 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/I01_NOREX/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.608770 bimmer_connected-0.9.5/test/responses/I01_REX/
--rw-r--r--   0 runner    (1001) docker     (121)      356 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/I01_REX/charging-statistics_1.json
--rw-r--r--   0 runner    (1001) docker     (121)    11520 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/I01_REX/vehicles_v2_bmw_0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.612770 bimmer_connected-0.9.5/test/responses/auth/
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/auth_cn_login_error.json
--rw-r--r--   0 runner    (1001) docker     (121)      600 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/auth_cn_login_pwd.json
--rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/auth_cn_publickey.json
--rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/auth_error_internal_error.txt
--rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/auth_error_wrong_password.json
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/auth_token.json
--rw-r--r--   0 runner    (1001) docker     (121)      346 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/authorization_response.json
--rw-r--r--   0 runner    (1001) docker     (121)      746 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/auth/oauth_config.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-22 11:55:31.612770 bimmer_connected-0.9.5/test/responses/remote_services/
--rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/remote_services/eadrax_service_delivered.json
--rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/remote_services/eadrax_service_error.json
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/remote_services/eadrax_service_eventposition.json
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/remote_services/eadrax_service_executed.json
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/remote_services/eadrax_service_initiated.json
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/responses/remote_services/eadrax_service_pending.json
--rw-r--r--   0 runner    (1001) docker     (121)    19996 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_account.py
--rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3281 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_deprecated_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)    13167 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_deprecated_vehicle_status.py
--rw-r--r--   0 runner    (1001) docker     (121)     8971 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_remote_services.py
--rw-r--r--   0 runner    (1001) docker     (121)     3042 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7703 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_vehicle.py
--rw-r--r--   0 runner    (1001) docker     (121)    14244 2022-06-22 11:55:15.000000 bimmer_connected-0.9.5/test/test_vehicle_status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/
+-rw-r--r--   0 runner    (1001) docker     (121)      274 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)       79 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.455039 bimmer_connected-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.455039 bimmer_connected-0.9.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)     3159 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1040 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1424 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      124 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.459039 bimmer_connected-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     1696 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1064 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/workflows/lock.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      395 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/workflows/stale.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     3992 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      403 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       50 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (121)     3328 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      819 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/ChangeLog
+-rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     8378 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7317 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.459039 bimmer_connected-0.9.6/bimmer_connected/
+-rw-r--r--   0 runner    (1001) docker     (121)      459 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5519 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/account.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.459039 bimmer_connected-0.9.6/bimmer_connected/api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15793 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3534 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1287 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/api/regions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3698 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/api/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10920 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/cli.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2540 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/const.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4253 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/coord_convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4609 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.459039 bimmer_connected-0.9.6/bimmer_connected/vehicle/
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4011 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/charging_profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3805 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/doors_windows.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6609 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/fuel_and_battery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3879 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9982 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/remote_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4075 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11703 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9219 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/bimmer_connected/vehicle/vehicle_status.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.459039 bimmer_connected-0.9.6/bimmer_connected.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8378 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3941 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       63 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/pbr.json
+-rw-r--r--   0 runner    (1001) docker     (121)       37 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-25 07:44:27.000000 bimmer_connected-0.9.6/bimmer_connected.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.459039 bimmer_connected-0.9.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)      617 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.463039 bimmer_connected-0.9.6/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.467039 bimmer_connected-0.9.6/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/_static/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)  1601424 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/_static/Intercepting Flutter traffic on Android (ARMv8) – NVISO Labs.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)  2954479 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/_static/Intercepting Flutter traffic on iOS – NVISO Labs.pdf
+-rw-r--r--   0 runner    (1001) docker     (121)  2852017 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/_static/Intercepting traffic from Android Flutter applications – NVISO Labs.pdf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/_templates/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5320 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/docs/source/development/
+-rw-r--r--   0 runner    (1001) docker     (121)     2275 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/development/fingerprints_in_homeassistant.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6768 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/development/reverse_engineering_mybmw.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/docs/source/module/
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/module/account.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/module/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/module/const.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      166 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/module/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/module/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1464 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/module/vehicle.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       29 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/docs/source/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      384 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/requirements-test.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)       37 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/test/
+-rw-r--r--   0 runner    (1001) docker     (121)    10903 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.455039 bimmer_connected-0.9.6/test/responses/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/test/responses/F31/
+-rw-r--r--   0 runner    (1001) docker     (121)     4030 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/F31/state_WBA00000000000F31_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1190 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/F31/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/test/responses/G01/
+-rw-r--r--   0 runner    (1001) docker     (121)     7005 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/G01/state_WBA00000000DEMO04_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)      903 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/G01/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/test/responses/G20/
+-rw-r--r--   0 runner    (1001) docker     (121)     5552 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/G20/state_WBA00000000DEMO03_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/G20/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/test/responses/G23/
+-rw-r--r--   0 runner    (1001) docker     (121)     6669 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/G23/state_WBA00000000DEMO02_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1310 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/G23/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.471039 bimmer_connected-0.9.6/test/responses/I01_NOREX/
+-rw-r--r--   0 runner    (1001) docker     (121)     5908 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/I01_NOREX/state_WBY000000NOREXI01_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1181 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/I01_NOREX/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/test/responses/I01_REX/
+-rw-r--r--   0 runner    (1001) docker     (121)     5906 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/I01_REX/state_WBY00000000REXI01_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/I01_REX/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/test/responses/I20/
+-rw-r--r--   0 runner    (1001) docker     (121)     6847 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/I20/state_WBA00000000DEMO01_0.json
+-rw-r--r--   0 runner    (1001) docker     (121)     1608 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/I20/vehicles_v2_bmw_0.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/test/responses/auth/
+-rw-r--r--   0 runner    (1001) docker     (121)      139 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/auth_cn_login_error.json
+-rw-r--r--   0 runner    (1001) docker     (121)      600 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/auth_cn_login_pwd.json
+-rw-r--r--   0 runner    (1001) docker     (121)      406 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/auth_cn_publickey.json
+-rw-r--r--   0 runner    (1001) docker     (121)       21 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/auth_error_internal_error.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      200 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/auth_error_wrong_password.json
+-rw-r--r--   0 runner    (1001) docker     (121)      194 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/auth_token.json
+-rw-r--r--   0 runner    (1001) docker     (121)      346 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/authorization_response.json
+-rw-r--r--   0 runner    (1001) docker     (121)      746 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/auth/oauth_config.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-25 07:44:27.475040 bimmer_connected-0.9.6/test/responses/remote_services/
+-rw-r--r--   0 runner    (1001) docker     (121)       35 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/remote_services/eadrax_service_delivered.json
+-rw-r--r--   0 runner    (1001) docker     (121)       92 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/remote_services/eadrax_service_error.json
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/remote_services/eadrax_service_eventposition.json
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/remote_services/eadrax_service_executed.json
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/remote_services/eadrax_service_initiated.json
+-rw-r--r--   0 runner    (1001) docker     (121)       33 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/responses/remote_services/eadrax_service_pending.json
+-rw-r--r--   0 runner    (1001) docker     (121)    20440 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1469 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2885 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_deprecated_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10839 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_deprecated_vehicle_status.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8979 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_remote_services.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8546 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_vehicle.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12629 2022-06-25 07:44:17.000000 bimmer_connected-0.9.6/test/test_vehicle_status.py
```

### Comparing `bimmer_connected-0.9.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `bimmer_connected-0.9.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/ISSUE_TEMPLATE/config.yml` & `bimmer_connected-0.9.6/.github/ISSUE_TEMPLATE/config.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/PULL_REQUEST_TEMPLATE.md` & `bimmer_connected-0.9.6/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/workflows/codeql-analysis.yml` & `bimmer_connected-0.9.6/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/workflows/lock.yml` & `bimmer_connected-0.9.6/.github/workflows/lock.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/workflows/pythonpublish.yml` & `bimmer_connected-0.9.6/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/workflows/stale.yml` & `bimmer_connected-0.9.6/.github/workflows/stale.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.github/workflows/test.yml` & `bimmer_connected-0.9.6/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/.pre-commit-config.yaml` & `bimmer_connected-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/CODE_OF_CONDUCT.md` & `bimmer_connected-0.9.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/CONTRIBUTING.md` & `bimmer_connected-0.9.6/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/LICENSE` & `bimmer_connected-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/PKG-INFO` & `bimmer_connected-0.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimmer_connected
-Version: 0.9.5
+Version: 0.9.6
 Summary: Library to read data from the BMW Connected Drive portal
 Home-page: https://github.com/bimmerconnected/bimmer_connected
 Author: gerard33, rikroe
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/bimmerconnected/bimmer_connected/issues
 Project-URL: Documentation, https://bimmer-connected.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/bimmerconnected/bimmer_connected
```

### Comparing `bimmer_connected-0.9.5/README.rst` & `bimmer_connected-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/bimmer_connected/account.py` & `bimmer_connected-0.9.6/bimmer_connected/account.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import List, Optional
 
 import httpx
 
 from bimmer_connected.api.authentication import MyBMWAuthentication
 from bimmer_connected.api.client import MyBMWClient, MyBMWClientConfiguration
 from bimmer_connected.api.regions import Regions
-from bimmer_connected.const import VEHICLES_URL, CarBrands
+from bimmer_connected.const import VEHICLE_STATE_URL, VEHICLES_URL, CarBrands
 from bimmer_connected.models import GPSPosition
 from bimmer_connected.utils import deprecated
 from bimmer_connected.vehicle import MyBMWVehicle
 
 VALID_UNTIL_OFFSET = datetime.timedelta(seconds=10)
 
 _LOGGER = logging.getLogger(__name__)
@@ -57,31 +57,43 @@
                 use_metric_units=use_metric_units,
             )
 
     async def get_vehicles(self) -> None:
         """Retrieve vehicle data from BMW servers."""
         _LOGGER.debug("Getting vehicle list")
 
+        fetched_at = datetime.datetime.now(datetime.timezone.utc)
+
         async with MyBMWClient(self.config) as client:
-            vehicles_request_params = {
-                "apptimezone": self.utcdiff,
-                "appDateTime": int(datetime.datetime.now().timestamp() * 1000),
-                "tireGuardMode": "ENABLED",
-            }
             vehicles_responses: List[httpx.Response] = [
                 await client.get(
                     VEHICLES_URL,
-                    params=vehicles_request_params,
-                    headers=client.generate_default_header(brand),
+                    headers={
+                        **client.generate_default_header(brand),
+                        "bmw-current-date": fetched_at.isoformat(),
+                    },
                 )
                 for brand in CarBrands
             ]
 
             for response in vehicles_responses:
                 for vehicle_dict in response.json():
+                    # Get the detailed vehicle state
+                    state_response = await client.get(
+                        VEHICLE_STATE_URL.format(vin=vehicle_dict["vin"]),
+                        headers=response.request.headers,  # Reuse the same headers as used to get vehicle list
+                    )
+
+                    # Add state information to vehicle_dict
+                    vehicle_dict.update(state_response.json())
+
+                    # Add unit information
+                    vehicle_dict["is_metric"] = self.config.use_metric_units
+                    vehicle_dict["fetched_at"] = fetched_at
+
                     # If vehicle already exists, just update it's state
                     existing_vehicle = self.get_vehicle(vehicle_dict["vin"])
                     if existing_vehicle:
                         existing_vehicle.update_state(vehicle_dict)
                     else:
                         self.vehicles.append(MyBMWVehicle(self, vehicle_dict))
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/api/authentication.py` & `bimmer_connected-0.9.6/bimmer_connected/api/authentication.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/bimmer_connected/api/client.py` & `bimmer_connected-0.9.6/bimmer_connected/api/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,8 +78,9 @@
             "x-user-agent": X_USER_AGENT.format(
                 brand=(brand or CarBrands.BMW),
                 app_version=get_app_version(self.config.authentication.region),
                 region=self.config.authentication.region.value,
             ),
             **get_correlation_id(),
             "bmw-units-preferences": "d=KM;v=L" if self.config.use_metric_units else "d=MI;v=G",
+            "24-hour-format": "true",
         }
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/api/regions.py` & `bimmer_connected-0.9.6/bimmer_connected/api/regions.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/bimmer_connected/api/utils.py` & `bimmer_connected-0.9.6/bimmer_connected/api/utils.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/bimmer_connected/cli.py` & `bimmer_connected-0.9.6/bimmer_connected/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,16 @@
 from pathlib import Path
 
 import httpx
 
 from bimmer_connected.account import MyBMWAccount
 from bimmer_connected.api.client import MyBMWClient
 from bimmer_connected.api.regions import get_region_from_name, valid_regions
-from bimmer_connected.const import CarBrands
 from bimmer_connected.utils import MyBMWJSONEncoder
 from bimmer_connected.vehicle import MyBMWVehicle, VehicleViewDirection
-from bimmer_connected.vehicle.vehicle import HV_BATTERY_DRIVE_TRAINS, DriveTrainType
 
 TEXT_VIN = "Vehicle Identification Number"
 
 
 def main_parser() -> argparse.ArgumentParser:
     """Creates the ArgumentParser with all relevant subparsers."""
     logging.basicConfig(level=logging.DEBUG)
@@ -132,28 +130,26 @@
 
     account = MyBMWAccount(args.username, args.password, get_region_from_name(args.region), log_responses=time_dir)
     if args.lat and args.lng:
         account.set_observer_position(args.lat, args.lng)
     await account.get_vehicles()
 
     # Patching in new My BMW endpoints for fingerprinting
-    async with MyBMWClient(account.config, brand=CarBrands.BMW) as client:
-        vehicles_v2 = await client.get("/eadrax-vcs/v2/vehicles")
-
-        for vehicle in vehicles_v2.json():
-            await client.get(
-                f"/eadrax-vcs/v2/vehicles/{vehicle['vin']}/state",
-                headers={"bmw-current-date": datetime.utcnow().isoformat(), "24-hour-format": "true"},
-            )
+    async with MyBMWClient(account.config) as client:
+        for vehicle in account.vehicles:
             try:
-                if DriveTrainType(vehicle["attributes"]["driveTrain"]) in HV_BATTERY_DRIVE_TRAINS:
+                if vehicle.has_electric_drivetrain:
                     await client.get(
-                        f"/eadrax-crccs/v1/vehicles/{vehicle['vin']}",
+                        f"/eadrax-crccs/v1/vehicles/{vehicle.vin}",
                         params={"fields": "charging-profile", "has_charging_settings_capabilities": True},
-                        headers={"bmw-current-date": datetime.utcnow().isoformat(), "24-hour-format": "true"},
+                        headers={
+                            **client.generate_default_header(vehicle.brand),
+                            "bmw-current-date": datetime.utcnow().isoformat(),
+                            "24-hour-format": "true",
+                        },
                     )
             except httpx.HTTPStatusError:
                 pass
 
     print(f"fingerprint of the vehicles written to {time_dir}")
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/const.py` & `bimmer_connected-0.9.6/bimmer_connected/const.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 
 class CarBrands(str, Enum):
     """Car brands supported by the MyBMW API."""
 
     @classmethod
     def _missing_(cls, value):
+        value = next(iter(value.split("_")))
         for member in cls:
             if member.value == value.lower():
                 return member
         raise ValueError(f"'{value}' is not a valid {cls.__name__}")
 
     BMW = "bmw"
     MINI = "mini"
@@ -56,25 +57,29 @@
 
 AUTH_CHINA_PUBLIC_KEY_URL = "/eadrax-coas/v1/cop/publickey"
 AUTH_CHINA_LOGIN_URL = "/eadrax-coas/v2/login/pwd"
 AUTH_CHINA_TOKEN_URL = "/eadrax-coas/v1/oauth/token"
 
 OAUTH_CONFIG_URL = "/eadrax-ucs/v1/presentation/oauth/config"
 
-VEHICLES_URL = "/eadrax-vcs/v1/vehicles"
+VEHICLES_URL = "/eadrax-vcs/v2/vehicles"
+VEHICLE_STATE_URL = VEHICLES_URL + "/{vin}/state"
 
 REMOTE_SERVICE_BASE_URL = "/eadrax-vrccs/v2/presentation/remote-commands"
 REMOTE_SERVICE_URL = REMOTE_SERVICE_BASE_URL + "/{vin}/{service_type}"
 REMOTE_SERVICE_STATUS_URL = REMOTE_SERVICE_BASE_URL + "/eventStatus?eventId={event_id}"
 REMOTE_SERVICE_POSITION_URL = REMOTE_SERVICE_BASE_URL + "/eventPosition?eventId={event_id}"
 
 VEHICLE_IMAGE_URL = "/eadrax-ics/v3/presentation/vehicles/{vin}/images?carView={view}"
 VEHICLE_POI_URL = "/eadrax-dcs/v1/send-to-car/send-to-car"
 
 VEHICLE_CHARGING_STATISTICS_URL = "/eadrax-chs/v1/charging-statistics"
 VEHICLE_CHARGING_SESSIONS_URL = "/eadrax-chs/v1/charging-sessions"
 
-SERVICE_PROPERTIES = "properties"
-SERVICE_STATUS = "status"
 SERVICE_CHARGING_STATISTICS_URL = "CHARGING_STATISTICS"
 SERVICE_CHARGING_SESSIONS_URL = "CHARGING_SESSIONS"
 SERVICE_CHARGING_PROFILE = "CHARGING_PROFILE"
+
+
+ATTR_STATE = "state"
+ATTR_CAPABILITIES = "capabilities"
+ATTR_ATTRIBUTES = "attributes"
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/coord_convert.py` & `bimmer_connected-0.9.6/bimmer_connected/coord_convert.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/bimmer_connected/models.py` & `bimmer_connected-0.9.6/bimmer_connected/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,27 @@
 from enum import Enum
 from typing import Dict, List, NamedTuple, Optional, Tuple, Union
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class StrEnum(str, Enum):
-    """A string enumeration of type `(str, Enum)`. All members are compared via `upper()`."""
+    """A string enumeration of type `(str, Enum)`. All members are compared via `upper()`. Defaults to UNKNOWN."""
 
     @classmethod
     def _missing_(cls, value):
+        has_unknown = False
         for member in cls:
+            if member.value.upper() == "UNKNOWN":
+                has_unknown = True
             if member.value.upper() == value.upper():
                 return member
+        if has_unknown:
+            _LOGGER.warning("'%s' is not a valid '%s'", value, cls.__name__)
+            return getattr(cls, "UNKNOWN")
         raise ValueError(f"'{value}' is not a valid {cls.__name__}")
 
 
 @dataclass
 class VehicleDataBase:
     """A base class for parsing and storing complex vehicle data."""
 
@@ -115,7 +121,12 @@
 
 
 class ValueWithUnit(NamedTuple):
     """A value with a corresponding unit."""
 
     value: Optional[Union[int, float]]
     unit: Optional[str]
+
+    # def __add__(self, other: "ValueWithUnit"):
+    #     if self.unit != other.unit or not other:
+    #         raise ValueError("Both values must have the same unit!")
+    #     return ValueWithUnit(self.value + other.value, self.unit)
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/utils.py` & `bimmer_connected-0.9.6/bimmer_connected/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -83,7 +83,22 @@
                 replacement_text,
             )
             return func(*args, **kwargs)
 
         return _func_wrapper
 
     return decorator
+
+
+def to_camel_case(input_str: str) -> str:
+    """Converts SNAKE_CASE or snake_case to camelCase."""
+
+    retval = ""
+    flag_upper = False
+    for curr in input_str.lower():
+        if not curr.isalnum():
+            if curr == "_":
+                flag_upper = True
+            continue
+        retval = retval + (curr.upper() if flag_upper else curr)
+        flag_upper = False
+    return retval
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/charging_profile.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/charging_profile.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,58 +1,60 @@
 """Models the charging profiles of a vehicle."""
 
 import datetime
 import logging
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional
 
+from bimmer_connected.const import ATTR_STATE
 from bimmer_connected.models import StrEnum, VehicleDataBase
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ChargingMode(StrEnum):
     """Charging mode of electric vehicle."""
 
-    IMMEDIATE_CHARGING = "immediateCharging"
-    DELAYED_CHARGING = "delayedCharging"
+    IMMEDIATE_CHARGING = "IMMEDIATE_CHARGING"
+    DELAYED_CHARGING = "DELAYED_CHARGING"
+    UNKNOWN = "UNKNOWN"
 
 
 class ChargingPreferences(StrEnum):
     """Charging preferences of electric vehicle."""
 
-    NO_PRESELECTION = "noPreSelection"
-    CHARGING_WINDOW = "chargingWindow"
+    NO_PRESELECTION = "NO_PRESELECTION"
+    CHARGING_WINDOW = "CHARGING_WINDOW"
+    UNKNOWN = "UNKNOWN"
 
 
 class TimerTypes(StrEnum):
     """Different timer types."""
 
-    TWO_WEEKS = "twoWeeksTimer"
-    ONE_WEEK = "weeklyPlanner"
-    OVERRIDE_TIMER = "overrideTimer"
+    TWO_WEEKS = "TWO_WEEKS_TIMER"
+    ONE_WEEK = "WEEKLY_PLANNER"
+    OVERRIDE_TIMER = "OVERRIDE_TIMER"
+    UNKNOWN = "UNKNOWN"
 
 
 class ChargingWindow:
     """A charging window."""
 
     def __init__(self, window_dict: dict):
         self._window_dict = window_dict
 
     @property
     def start_time(self) -> datetime.time:
         """Start of the charging window."""
-        # end of reductionOfChargeCurrent == start of charging window
-        return datetime.time(int(self._window_dict["end"]["hour"]), int(self._window_dict["end"]["minute"]))
+        return datetime.time(int(self._window_dict["start"]["hour"]), int(self._window_dict["start"]["minute"]))
 
     @property
     def end_time(self) -> datetime.time:
         """End of the charging window."""
-        # start of reductionOfChargeCurrent == end of charging window
-        return datetime.time(int(self._window_dict["start"]["hour"]), int(self._window_dict["start"]["minute"]))
+        return datetime.time(int(self._window_dict["end"]["hour"]), int(self._window_dict["end"]["minute"]))
 
 
 class DepartureTimer:
     """A departure timer."""
 
     def __init__(self, timer_dict: dict):
         self._timer_dict: Dict = timer_dict
@@ -103,36 +105,18 @@
     """Returns the preferred charging mode."""
 
     @classmethod
     def _parse_vehicle_data(cls, vehicle_data: Dict) -> Dict:
         """Parse doors and windows."""
         retval: Dict[str, Any] = {}
 
-        if "status" not in vehicle_data or "chargingProfile" not in vehicle_data["status"]:
-            if vehicle_data["capabilities"]["isChargingPlanSupported"]:
-                _LOGGER.error("Unable to read data from `status.chargingProfile`.")
-            return retval
-
-        charging_profile = vehicle_data["status"]["chargingProfile"]
-
-        retval["is_pre_entry_climatization_enabled"] = (
-            bool(charging_profile["climatisationOn"]) if "" in charging_profile else None
-        )
-        retval["departure_times"] = [DepartureTimer(t) for t in charging_profile.get("departureTimes", [])]
-        retval["preferred_charging_window"] = (
-            ChargingWindow(charging_profile["reductionOfChargeCurrent"])
-            if "reductionOfChargeCurrent" in charging_profile
-            else None
-        )
-        retval["timer_type"] = (
-            TimerTypes(charging_profile["chargingControlType"]) if "chargingControlType" in charging_profile else None
-        )
-        retval["charging_preferences"] = (
-            ChargingPreferences(charging_profile["chargingPreference"])
-            if "chargingPreference" in charging_profile
-            else None
-        )
-        retval["charging_mode"] = (
-            ChargingMode(charging_profile["chargingMode"]) if "chargingMode" in charging_profile else None
-        )
+        if ATTR_STATE in vehicle_data and "chargingProfile" in vehicle_data[ATTR_STATE]:
+            charging_profile = vehicle_data[ATTR_STATE]["chargingProfile"]
+
+            retval["is_pre_entry_climatization_enabled"] = bool(charging_profile.get("climatisationOn", False))
+            retval["departure_times"] = [DepartureTimer(t) for t in charging_profile.get("departureTimes", [])]
+            retval["preferred_charging_window"] = ChargingWindow(charging_profile.get("reductionOfChargeCurrent", {}))
+            retval["timer_type"] = TimerTypes(charging_profile.get("chargingControlType", "UNKNOWN"))
+            retval["charging_preferences"] = ChargingPreferences(charging_profile.get("chargingPreference", "UNKNOWN"))
+            retval["charging_mode"] = ChargingMode(charging_profile.get("chargingMode", "UNKNOWN"))
 
         return retval
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/doors_windows.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/doors_windows.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 """Models the state of a vehicle."""
 
 import logging
 from dataclasses import dataclass, field
 from typing import Any, Dict, List
 
+from bimmer_connected.const import ATTR_STATE
 from bimmer_connected.models import StrEnum, VehicleDataBase
+from bimmer_connected.utils import to_camel_case
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class LidState(StrEnum):
     """Possible states of the hatch, trunk, doors, windows, sun roof."""
 
@@ -57,46 +59,50 @@
 @dataclass
 class DoorsAndWindows(VehicleDataBase):  # pylint:disable=too-many-instance-attributes
     """Provides an accessible version of `properties.doorsAndWindows`."""
 
     door_lock_state: LockState = LockState.UNKNOWN
     """Get state of the door locks."""
 
-    convertible_top: LidState = LidState.UNKNOWN
-    """Get state of the convertible roof."""
-
     lids: List[Lid] = field(default_factory=list)
     """All lids (doors+hood+trunk) of the car."""
 
     windows: List[Window] = field(default_factory=list)
     """All windows (doors+sunroof) of the car."""
 
     @classmethod
     def _parse_vehicle_data(cls, vehicle_data: Dict) -> Dict:
         """Parse doors and windows."""
         retval: Dict[str, Any] = {}
 
-        if "properties" not in vehicle_data or "doorsAndWindows" not in vehicle_data["status"]:
-            _LOGGER.error("Unable to read data from `properties.doorsAndWindows`.")
-            return retval
-
-        doors_and_windows = vehicle_data["properties"]["doorsAndWindows"]
-
-        retval["lids"] = [
-            Lid(k, v) for k, v in doors_and_windows.items() if k in ["hood", "trunk"] and v != LidState.INVALID
-        ] + [Lid(k, v) for k, v in doors_and_windows["doors"].items() if v != LidState.INVALID]
-
-        retval["windows"] = [Window(k, v) for k, v in doors_and_windows["windows"].items() if v != LidState.INVALID]
-        if "moonroof" in doors_and_windows:
-            retval["windows"].append(Window("moonroof", doors_and_windows["moonroof"]))
-
-        if "convertibleTop" in doors_and_windows:
-            retval["convertible_top"] = LidState(doors_and_windows["convertibleTop"])
-
-        retval["door_lock_state"] = LockState(vehicle_data["status"]["doorsGeneralState"].upper())
+        if ATTR_STATE in vehicle_data:
+            if "doorsState" in vehicle_data[ATTR_STATE]:
+                retval["lids"] = [
+                    Lid(k, v)
+                    for k, v in vehicle_data[ATTR_STATE]["doorsState"].items()
+                    if k not in ["combinedState", "combinedSecurityState"] and v != LidState.INVALID
+                ]
+                retval["door_lock_state"] = LockState(
+                    vehicle_data[ATTR_STATE]["doorsState"].get("combinedSecurityState", "UNKNOWN")
+                )
+
+            if "windowsState" in vehicle_data[ATTR_STATE]:
+                retval["windows"] = [
+                    Window(k, v)
+                    for k, v in vehicle_data[ATTR_STATE]["windowsState"].items()
+                    if k not in ["combinedState"] and v != LidState.INVALID
+                ]
+
+            if "roofState" in vehicle_data[ATTR_STATE]:
+                retval["lids"].append(
+                    Lid(
+                        to_camel_case(vehicle_data[ATTR_STATE]["roofState"]["roofStateType"]),
+                        vehicle_data[ATTR_STATE]["roofState"]["roofState"],
+                    )
+                )
 
         return retval
 
     @property
     def open_lids(self) -> List[Lid]:
         """Get all open lids of the car."""
         return [lid for lid in self.lids if not lid.is_closed]
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/location.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/location.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Generals models used for bimmer_connected."""
 
 import datetime
 import logging
 from dataclasses import dataclass
 from typing import Any, Dict, Optional
 
-from bimmer_connected.const import Regions
+from bimmer_connected.const import ATTR_ATTRIBUTES, ATTR_STATE, Regions
 from bimmer_connected.coord_convert import gcj2wgs
 from bimmer_connected.models import GPSPosition, VehicleDataBase
 from bimmer_connected.utils import parse_datetime
 
 _LOGGER = logging.getLogger(__name__)
 
 
@@ -38,19 +38,19 @@
 
     @classmethod
     def _parse_vehicle_data(cls, vehicle_data: Dict):
         date_dummy = datetime.datetime(1970, 1, 1, tzinfo=datetime.timezone.utc)
 
         retval: Dict[str, Any] = {}
         retval["vehicle_update_timestamp"] = max(
-            parse_datetime(vehicle_data.get("properties", {}).get("lastUpdatedAt")) or date_dummy,
-            parse_datetime(vehicle_data.get("status", {}).get("lastUpdatedAt")) or date_dummy,
+            parse_datetime(vehicle_data.get(ATTR_STATE, {}).get("lastFetched")) or date_dummy,
+            parse_datetime(vehicle_data.get(ATTR_ATTRIBUTES, {}).get("lastFetched")) or date_dummy,
         )
-        if "properties" in vehicle_data and "vehicleLocation" in vehicle_data["properties"]:
-            location = vehicle_data["properties"]["vehicleLocation"]
+        if ATTR_STATE in vehicle_data and "location" in vehicle_data[ATTR_STATE]:
+            location = vehicle_data[ATTR_STATE]["location"]
             retval["location"] = GPSPosition(location["coordinates"]["latitude"], location["coordinates"]["longitude"])
             retval["heading"] = location["heading"]
         return retval
 
     def _update_after_parse(self, parsed: Dict) -> Dict:
         """Updates parsed vehicle data with attributes stored in class if needed."""
         retval = parsed
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/remote_services.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/remote_services.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/reports.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/reports.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,46 @@
 """Models the state of a vehicle."""
 
 import datetime
 import logging
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Optional
 
+from bimmer_connected.const import ATTR_STATE
 from bimmer_connected.models import StrEnum, ValueWithUnit, VehicleDataBase
 from bimmer_connected.utils import parse_datetime
 
 _LOGGER = logging.getLogger(__name__)
 
 
 class ConditionBasedServiceStatus(StrEnum):
     """Status of the condition based services."""
 
     OK = "OK"
     OVERDUE = "OVERDUE"
     PENDING = "PENDING"
+    UNKNOWN = "UNKNOWN"
 
 
 @dataclass
 class ConditionBasedService:  # pylint: disable=too-few-public-methods
     """Entry in the list of condition based services."""
 
     service_type: str
     state: ConditionBasedServiceStatus
     due_date: Optional[datetime.date]
     due_distance: ValueWithUnit
 
-    # pylint:disable=invalid-name,unused-argument,redefined-builtin
+    # pylint:disable=invalid-name,redefined-builtin,too-many-arguments,unused-argument
     @classmethod
-    def from_api_entry(cls, type: str, status: str, dateTime: str = None, distance: Dict = None, **kwargs):
+    def from_api_entry(
+        cls, type: str, status: str, dateTime: str = None, mileage: int = None, is_metric: bool = True, **kwargs
+    ):
         """Parse a condition based service entry from the API format to `ConditionBasedService`."""
-        due_distance = ValueWithUnit(distance["value"], distance["units"]) if distance else ValueWithUnit(None, None)
+        due_distance = ValueWithUnit(mileage, "km" if is_metric else "mi") if mileage else ValueWithUnit(None, None)
         due_date = parse_datetime(dateTime) if dateTime else None
         return cls(type, ConditionBasedServiceStatus(status), due_date, due_distance)
 
 
 @dataclass
 class ConditionBasedServiceReport(VehicleDataBase):
     """Parses and summarizes condition based services (e.g. next oil service)."""
@@ -48,48 +52,48 @@
     """Indicates if a service is required."""
 
     @classmethod
     def _parse_vehicle_data(cls, vehicle_data: Dict) -> Optional[Dict]:
         """Parse doors and windows."""
         retval: Dict[str, Any] = {}
 
-        if "properties" not in vehicle_data or "serviceRequired" not in vehicle_data["properties"]:
-            _LOGGER.error("Unable to read data from `properties.serviceRequired`.")
-            return retval
-
-        messages = vehicle_data["properties"]["serviceRequired"]
-        retval["messages"] = [ConditionBasedService.from_api_entry(**m) for m in messages]
-        retval["is_service_required"] = vehicle_data["properties"]["isServiceRequired"]
+        if ATTR_STATE in vehicle_data and "requiredServices" in vehicle_data[ATTR_STATE]:
+            messages = vehicle_data[ATTR_STATE]["requiredServices"]
+            retval["messages"] = [
+                ConditionBasedService.from_api_entry(**m, is_metric=vehicle_data["is_metric"]) for m in messages
+            ]
+            retval["is_service_required"] = any((m.state != ConditionBasedServiceStatus.OK) for m in retval["messages"])
 
         return retval
 
 
 class CheckControlStatus(StrEnum):
     """Status of the condition based services."""
 
     OK = "OK"
     LOW = "LOW"
     MEDIUM = "MEDIUM"
     HIGH = "HIGH"
     CRITICAL = "CRITICAL"
+    UNKNOWN = "UNKNOWN"
 
 
 @dataclass
 class CheckControlMessage:
     """Check control message sent from the server."""
 
     description_short: str
-    description_long: str
+    description_long: Optional[str]
     state: CheckControlStatus
 
-    # pylint:disable=invalid-name,unused-argument
+    # pylint:disable=invalid-name,redefined-builtin,unused-argument
     @classmethod
-    def from_api_entry(cls, title: str, longDescription: str, state: str, **kwargs):
+    def from_api_entry(cls, type: str, severity: str, longDescription: str = None, **kwargs):
         """Parses a check control entry from the API format to `CheckControlMessage`."""
-        return cls(title, longDescription, CheckControlStatus(state))
+        return cls(type, longDescription, CheckControlStatus(severity))
 
 
 @dataclass
 class CheckControlMessageReport(VehicleDataBase):
     """Parses and summarizes check control messages (e.g. low tire pressure)."""
 
     messages: List[CheckControlMessage] = field(default_factory=list)
@@ -99,16 +103,13 @@
     """Indicates if check control messages are present."""
 
     @classmethod
     def _parse_vehicle_data(cls, vehicle_data: Dict) -> Optional[Dict]:
         """Parse doors and windows."""
         retval: Dict[str, Any] = {}
 
-        if "status" not in vehicle_data or "checkControlMessages" not in vehicle_data["status"]:
-            _LOGGER.error("Unable to read data from `status.checkControlMessages`.")
-            return retval
-
-        messages = vehicle_data["status"]["checkControlMessages"]
-        retval["messages"] = [CheckControlMessage.from_api_entry(**m) for m in messages if m["state"] != "OK"]
-        retval["has_check_control_messages"] = vehicle_data["status"]["checkControlMessagesGeneralState"] != "No Issues"
+        if ATTR_STATE in vehicle_data and "checkControlMessages" in vehicle_data[ATTR_STATE]:
+            messages = vehicle_data[ATTR_STATE]["checkControlMessages"]
+            retval["messages"] = [CheckControlMessage.from_api_entry(**m) for m in messages if m["severity"] != "OK"]
+            retval["has_check_control_messages"] = len(retval["messages"]) > 0
 
         return retval
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/vehicle.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/vehicle.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Models state and remote services of one vehicle."""
 import datetime
 import logging
-from typing import TYPE_CHECKING, Dict, List, Optional, Tuple, Type
+from typing import TYPE_CHECKING, List, Optional, Tuple, Type
 
 from bimmer_connected.api.client import MyBMWClient
-from bimmer_connected.const import SERVICE_PROPERTIES, SERVICE_STATUS, VEHICLE_IMAGE_URL, CarBrands
+from bimmer_connected.const import ATTR_ATTRIBUTES, ATTR_CAPABILITIES, ATTR_STATE, VEHICLE_IMAGE_URL, CarBrands
 from bimmer_connected.models import StrEnum, ValueWithUnit
 from bimmer_connected.utils import deprecated, parse_datetime
 from bimmer_connected.vehicle.charging_profile import ChargingProfile
 from bimmer_connected.vehicle.doors_windows import DoorsAndWindows
 from bimmer_connected.vehicle.fuel_and_battery import FuelAndBattery
 from bimmer_connected.vehicle.location import VehicleLocation
 from bimmer_connected.vehicle.remote_services import RemoteServices
@@ -27,21 +27,21 @@
     """Different types of drive trains."""
 
     COMBUSTION = "COMBUSTION"
     PLUGIN_HYBRID = "PLUGIN_HYBRID"  # PHEV
     ELECTRIC = "ELECTRIC"
     ELECTRIC_WITH_RANGE_EXTENDER = "ELECTRIC_WITH_RANGE_EXTENDER"
     HYBRID = "HYBRID"  # mild hybrids
+    UNKNOWN = "UNKNOWN"
 
 
 #: Set of drive trains that have a combustion engine
 COMBUSTION_ENGINE_DRIVE_TRAINS = {
     DriveTrainType.COMBUSTION,
     DriveTrainType.PLUGIN_HYBRID,
-    DriveTrainType.ELECTRIC_WITH_RANGE_EXTENDER,
 }
 
 #: set of drive trains that have a high voltage battery
 HV_BATTERY_DRIVE_TRAINS = {
     DriveTrainType.PLUGIN_HYBRID,
     DriveTrainType.ELECTRIC,
     DriveTrainType.ELECTRIC_WITH_RANGE_EXTENDER,
@@ -58,25 +58,27 @@
     FRONT = "VehicleInfo"
     # REARSIDE = 'REARSIDE'
     # REAR = 'REAR'
     SIDE = "ChargingHistory"
     # DASHBOARD = 'DASHBOARD'
     # DRIVERDOOR = 'DRIVERDOOR'
     # REARBIRDSEYE = 'REARBIRDSEYE'
+    UNKNOWN = "UNKNOWN"
 
 
 class LscType(StrEnum):
     """Known Values for lsc_type field.
 
     Not really sure, what this value really contains.
     """
 
     NOT_CAPABLE = "NOT_CAPABLE"
     NOT_SUPPORTED = "NOT_SUPPORTED"
     ACTIVATED = "ACTIVATED"
+    UNKNOWN = "UNKNOWN"
 
 
 # pylint: disable=too-many-public-methods,too-many-instance-attributes
 class MyBMWVehicle:
     """Models state and remote services of one vehicle.
 
     :param account: MyBMW account this vehicle belongs to
@@ -118,69 +120,53 @@
                 curr_attr.update_from_vehicle_data(vehicle_data)
 
     # # # # # # # # # # # # # # #
     # Generic attributes
     # # # # # # # # # # # # # # #
 
     @property
-    def _status(self) -> Dict:
-        """A shortcut to `data.status`."""
-        return self.data[SERVICE_STATUS]
-
-    @property
-    def _properties(self) -> Dict:
-        """A shortcut to `data.properties`."""
-        return self.data[SERVICE_PROPERTIES]
-
-    @property
     def brand(self) -> CarBrands:
         """Get the car brand."""
-        return CarBrands(self.data["brand"])
+        return CarBrands(self.data[ATTR_ATTRIBUTES]["brand"])
 
     @property
     def name(self) -> str:
         """Get the name of the vehicle."""
-        return self.data["model"]
+        return self.data[ATTR_ATTRIBUTES]["model"]
 
     @property
     def vin(self) -> str:
         """Get the VIN (vehicle identification number) of the vehicle."""
         return self.data["vin"]
 
     @property
     def drive_train(self) -> DriveTrainType:
         """Get the type of drive train of the vehicle."""
-        return DriveTrainType(self.data["driveTrain"])
+        return DriveTrainType(self.data[ATTR_ATTRIBUTES]["driveTrain"])
 
     @property
     def mileage(self) -> ValueWithUnit:
         """Get the mileage of the vehicle."""
-        current_mileage = self._status.get("currentMileage", {})
-        return ValueWithUnit(current_mileage.get("mileage"), current_mileage.get("units"))
+        return ValueWithUnit(self.data[ATTR_STATE].get("currentMileage", 0), "km" if self.data["is_metric"] else "mi")
 
     @property
     def timestamp(self) -> Optional[datetime.datetime]:
         """Get the timestamp when the data was recorded."""
         timestamps = [
             ts
             for ts in [
-                parse_datetime(str(self._properties.get("lastUpdatedAt"))),
-                parse_datetime(str(self._status.get("lastUpdatedAt"))),
+                parse_datetime(str(self.data[ATTR_ATTRIBUTES].get("lastFetched"))),
+                parse_datetime(str(self.data[ATTR_STATE].get("lastFetched"))),
             ]
             if ts
         ]
         if len(timestamps) == 0:
             return None
         return max(timestamps)
 
-    @property
-    def last_update_reason(self) -> str:
-        """The reason for the last state update."""
-        return self._status["timestampMessage"]
-
     # # # # # # # # # # # # # # #
     # Capabilities & properties
     # # # # # # # # # # # # # # #
 
     @property
     def has_electric_drivetrain(self) -> bool:
         """Return True if vehicle is equipped with a high voltage battery.
@@ -190,108 +176,98 @@
         return self.drive_train in HV_BATTERY_DRIVE_TRAINS
 
     @property
     def has_range_extender_drivetrain(self) -> bool:
         """Return True if vehicle is equipped with a range extender.
 
         In this case we can get the state of the gas tank."""
-        return self.drive_train == DriveTrainType.ELECTRIC and self.fuel_indicator_count == 3
+        return self.drive_train == DriveTrainType.ELECTRIC_WITH_RANGE_EXTENDER
 
     @property
     def has_combustion_drivetrain(self) -> bool:
         """Return True if vehicle is equipped with an internal combustion engine.
 
         In this case we can get the state of the gas tank."""
         return self.drive_train in COMBUSTION_ENGINE_DRIVE_TRAINS
 
     @property
     def is_charging_plan_supported(self) -> bool:
         """Return True if charging control (weekly planner) is available."""
-        return self.data["capabilities"]["isChargingPlanSupported"]
+        return self.data[ATTR_CAPABILITIES].get("isChargingPlanSupported", False)
 
     @property
     def is_vehicle_tracking_enabled(self) -> bool:
         """Return True if vehicle finder is enabled in vehicle."""
-        return self.data["capabilities"]["vehicleFinder"]["isEnabled"]
+        return self.data[ATTR_CAPABILITIES].get("vehicleFinder", False)
 
     @property
     def is_vehicle_active(self) -> bool:
         """Check if the vehicle is active/moving.
 
         If the vehicle was active/moving at the time of the last status update, current position is not available.
         """
-        return self._properties["inMotion"]
+        return False
+
+    @property
+    def lsc_type(self) -> LscType:
+        """Get the lscType of the vehicle.
+
+        Not really sure what that value really means. If it is NOT_CAPABLE, that probably means that the
+        vehicle state will not contain much data.
+        """
+        return LscType(self.data[ATTR_CAPABILITIES].get("lastStateCallState", "NOT_CAPABLE"))
 
     @property
     def is_lsc_enabled(self) -> bool:
         """Return True if LastStateCall is enabled (vehicle automatically updates API)."""
-        return self.data["capabilities"]["lastStateCall"]["lscState"] == "ACTIVATED"
+        return self.data[ATTR_STATE]["isLscSupported"]
 
     @property
     def drive_train_attributes(self) -> List[str]:
         """Get list of attributes available for the drive train of the vehicle.
 
         The list of available attributes depends if on the type of drive train.
         Some attributes only exist for electric/hybrid vehicles, others only if you
         have a combustion engine. Depending on the state of the vehicle, some of
         the attributes might still be None.
         """
         result = ["remaining_range_total", "mileage"]
         if self.has_electric_drivetrain:
             result += [
                 "charging_time_remaining",
-                "charging_start_time",
                 "charging_end_time",
                 "charging_time_label",
                 "charging_status",
                 "connection_status",
                 "remaining_battery_percent",
                 "remaining_range_electric",
                 "last_charging_end_result",
             ]
         if self.has_combustion_drivetrain or self.has_range_extender_drivetrain:
             result += ["remaining_fuel", "remaining_range_fuel", "remaining_fuel_percent"]
         return result
 
     @property
-    def lsc_type(self) -> LscType:
-        """Get the lscType of the vehicle.
-
-        Not really sure what that value really means. If it is NOT_CAPABLE, that probably means that the
-        vehicle state will not contain much data.
-        """
-        return LscType(self.data["capabilities"]["lastStateCall"].get("lscState"))
-
-    @property
     def available_attributes(self) -> List[str]:
         """Get the list of non-drivetrain attributes available for this vehicle."""
         # attributes available in all vehicles
         result = ["gps_position", "vin"]
-        if self.lsc_type == LscType.ACTIVATED:
+        if self.is_lsc_enabled:
             # generic attributes if lsc_type =! NOT_SUPPORTED
             result += self.drive_train_attributes
             result += [
                 "condition_based_services",
                 "check_control_messages",
                 "door_lock_state",
                 "timestamp",
-                "last_update_reason",
             ]
             # required for existing Home Assistant binary sensors
-            result += ["lids", "windows", "convertible_top"]
+            result += ["lids", "windows"]
         return result
 
-    @property
-    def fuel_indicator_count(self) -> int:
-        """Gets the number of fuel indicators.
-
-        Can be used to identify REX vehicles if driveTrain == ELECTRIC.
-        """
-        return len(self._status["fuelIndicators"])
-
     # # # # # # # # # # # # # # #
     # Generic functions
     # # # # # # # # # # # # # # #
 
     async def get_vehicle_image(self, direction: VehicleViewDirection) -> bytes:
         """Get a rendered image of the vehicle.
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected/vehicle/vehicle_status.py` & `bimmer_connected-0.9.6/bimmer_connected/vehicle/vehicle_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,18 +63,18 @@
     @property  # type: ignore[misc]
     @deprecated("vehicle.fuel_and_battery.remaining_fuel")
     def remaining_fuel(self) -> Optional[ValueWithUnit]:
         # pylint:disable=missing-function-docstring
         return self.vehicle.fuel_and_battery.remaining_fuel
 
     @property  # type: ignore[misc]
-    @deprecated("vehicle.fuel_indicator_count")
-    def fuel_indicator_count(self) -> Optional[int]:
+    @deprecated()
+    def fuel_indicator_count(self) -> None:
         # pylint:disable=missing-function-docstring
-        return self.vehicle.fuel_indicator_count
+        return None
 
     @property  # type: ignore[misc]
     @deprecated("vehicle.doors_and_windows.lids")
     def lids(self) -> List["Lid"]:
         # pylint:disable=missing-function-docstring
         return self.vehicle.doors_and_windows.lids
 
@@ -111,18 +111,18 @@
     @property  # type: ignore[misc]
     @deprecated("vehicle.doors_and_windows.door_lock_state")
     def door_lock_state(self) -> "LockState":
         # pylint:disable=missing-function-docstring
         return self.vehicle.doors_and_windows.door_lock_state
 
     @property  # type: ignore[misc]
-    @deprecated("vehicle.last_update_reason")
-    def last_update_reason(self) -> str:
+    @deprecated()
+    def last_update_reason(self) -> None:
         # pylint:disable=missing-function-docstring
-        return self.vehicle.last_update_reason
+        return None
 
     @property  # type: ignore[misc]
     @deprecated()
     def last_charging_end_result(self) -> None:
         # pylint:disable=missing-function-docstring
         return None  # Not available in My BMW
 
@@ -189,30 +189,30 @@
     @property  # type: ignore[misc]
     @deprecated()
     def charging_time_remaining(self) -> None:
         # pylint:disable=missing-function-docstring
         return None
 
     @property  # type: ignore[misc]
-    @deprecated("vehicle.fuel_and_battery.charging_start_time")
-    def charging_start_time(self) -> Optional[datetime.datetime]:
+    @deprecated()
+    def charging_start_time(self) -> None:
         # pylint:disable=missing-function-docstring
-        return self.vehicle.fuel_and_battery.charging_start_time
+        return None
 
     @property  # type: ignore[misc]
     @deprecated("vehicle.fuel_and_battery.charging_end_time")
     def charging_end_time(self) -> Optional[datetime.datetime]:
         # pylint:disable=missing-function-docstring
         return self.vehicle.fuel_and_battery.charging_end_time
 
     @property  # type: ignore[misc]
-    @deprecated("vehicle.fuel_and_battery.charging_time_label")
+    @deprecated()
     def charging_time_label(self) -> Optional[str]:
         # pylint:disable=missing-function-docstring
-        return self.vehicle.fuel_and_battery.charging_time_label
+        return None
 
     @property  # type: ignore[misc]
     @deprecated("vehicle.fuel_and_battery.remaining_battery_percent")
     def charging_level_hv(self) -> Optional[int]:
         # pylint:disable=missing-function-docstring
         return self.vehicle.fuel_and_battery.remaining_battery_percent
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected.egg-info/PKG-INFO` & `bimmer_connected-0.9.6/bimmer_connected.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bimmer-connected
-Version: 0.9.5
+Version: 0.9.6
 Summary: Library to read data from the BMW Connected Drive portal
 Home-page: https://github.com/bimmerconnected/bimmer_connected
 Author: gerard33, rikroe
 License: Apache-2
 Project-URL: Bug Tracker, https://github.com/bimmerconnected/bimmer_connected/issues
 Project-URL: Documentation, https://bimmer-connected.readthedocs.io/en/latest/
 Project-URL: Source Code, https://github.com/bimmerconnected/bimmer_connected
```

### Comparing `bimmer_connected-0.9.5/bimmer_connected.egg-info/SOURCES.txt` & `bimmer_connected-0.9.6/bimmer_connected.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -78,35 +78,28 @@
 test/test_api.py
 test/test_deprecated_vehicle.py
 test/test_deprecated_vehicle_status.py
 test/test_remote_services.py
 test/test_utils.py
 test/test_vehicle.py
 test/test_vehicle_status.py
-test/responses/F11/vehicles_v2_bmw_0.json
+test/responses/F31/state_WBA00000000000F31_0.json
 test/responses/F31/vehicles_v2_bmw_0.json
-test/responses/F44/vehicles_v2_bmw_0.json
-test/responses/F45/vehicles_v2_bmw_0.json
-test/responses/F48/vehicles_v2_bmw_0.json
+test/responses/G01/state_WBA00000000DEMO04_0.json
 test/responses/G01/vehicles_v2_bmw_0.json
-test/responses/G05/vehicles_v2_bmw_0.json
-test/responses/G08/vehicles_v2_bmw_0.json
-test/responses/G21/charging-sessions_0.json
-test/responses/G21/charging-statistics_0.json
-test/responses/G21/json_export.json
-test/responses/G21/vehicles_v2_bmw_0.json
+test/responses/G20/state_WBA00000000DEMO03_0.json
+test/responses/G20/vehicles_v2_bmw_0.json
+test/responses/G23/state_WBA00000000DEMO02_0.json
 test/responses/G23/vehicles_v2_bmw_0.json
-test/responses/G30/charging-sessions_0.json
-test/responses/G30/charging-statistics_0.json
-test/responses/G30/vehicles_v2_bmw_0.json
-test/responses/I01_NOREX/charging-sessions_0.json
-test/responses/I01_NOREX/charging-statistics_0.json
+test/responses/I01_NOREX/state_WBY000000NOREXI01_0.json
 test/responses/I01_NOREX/vehicles_v2_bmw_0.json
-test/responses/I01_REX/charging-statistics_1.json
+test/responses/I01_REX/state_WBY00000000REXI01_0.json
 test/responses/I01_REX/vehicles_v2_bmw_0.json
+test/responses/I20/state_WBA00000000DEMO01_0.json
+test/responses/I20/vehicles_v2_bmw_0.json
 test/responses/auth/auth_cn_login_error.json
 test/responses/auth/auth_cn_login_pwd.json
 test/responses/auth/auth_cn_publickey.json
 test/responses/auth/auth_error_internal_error.txt
 test/responses/auth/auth_error_wrong_password.json
 test/responses/auth/auth_token.json
 test/responses/auth/authorization_response.json
```

### Comparing `bimmer_connected-0.9.5/docs/Makefile` & `bimmer_connected-0.9.6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/_static/Intercepting Flutter traffic on Android (ARMv8) – NVISO Labs.pdf` & `bimmer_connected-0.9.6/docs/source/_static/Intercepting Flutter traffic on Android (ARMv8) – NVISO Labs.pdf`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/_static/Intercepting Flutter traffic on iOS – NVISO Labs.pdf` & `bimmer_connected-0.9.6/docs/source/_static/Intercepting Flutter traffic on iOS – NVISO Labs.pdf`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/_static/Intercepting traffic from Android Flutter applications – NVISO Labs.pdf` & `bimmer_connected-0.9.6/docs/source/_static/Intercepting traffic from Android Flutter applications – NVISO Labs.pdf`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/conf.py` & `bimmer_connected-0.9.6/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/development/fingerprints_in_homeassistant.rst` & `bimmer_connected-0.9.6/docs/source/development/fingerprints_in_homeassistant.rst`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/development/reverse_engineering_mybmw.rst` & `bimmer_connected-0.9.6/docs/source/development/reverse_engineering_mybmw.rst`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/module/api.rst` & `bimmer_connected-0.9.6/docs/source/module/api.rst`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/docs/source/module/vehicle.rst` & `bimmer_connected-0.9.6/docs/source/module/vehicle.rst`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/setup.cfg` & `bimmer_connected-0.9.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/test/__init__.py` & `bimmer_connected-0.9.6/test/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,47 +9,47 @@
 RESPONSE_DIR = Path(__file__).parent / "responses"
 
 TEST_USERNAME = "some_user"
 TEST_PASSWORD = "my_secret"
 TEST_REGION = Regions.REST_OF_WORLD
 TEST_REGION_STRING = "rest_of_world"
 
-VIN_F11 = "some_vin_F11"
-VIN_F31 = "some_vin_F31"
-VIN_F35 = "some_vin_F35"
-VIN_F44 = "some_vin_F44"
-VIN_F45 = "some_vin_F45"
-VIN_F48 = "some_vin_F48"
-VIN_G01 = "some_vin_G01"
-VIN_G05 = "some_vin_G05"
-VIN_G08 = "some_vin_G08"
-VIN_G21 = "some_vin_G21"
-VIN_G23 = "some_vin_G23"
-VIN_G30 = "some_vin_G30"
-VIN_I01_NOREX = "some_vin_I01_NOREX"
-VIN_I01_REX = "some_vin_I01_REX"
+VIN_F31 = "WBA00000000000F31"
+VIN_G01 = "WBA00000000DEMO04"
+VIN_G20 = "WBA00000000DEMO03"
+VIN_G23 = "WBA00000000DEMO02"
+VIN_I01_NOREX = "WBY000000NOREXI01"
+VIN_I01_REX = "WBY00000000REXI01"
+VIN_I20 = "WBA00000000DEMO01"
 
-ALL_FINGERPRINTS: List[Dict] = []
+ALL_FINGERPRINTS: Dict[str, List[Dict]] = {}
+ALL_STATES: Dict[str, Dict] = {}
 
 
 def get_fingerprint_count() -> int:
     """Returns number of loaded vehicles."""
-    return len(ALL_FINGERPRINTS)
+    return len(*ALL_FINGERPRINTS.values())
 
 
 def load_response(path: Union[Path, str]) -> Any:
     """Load a stored response."""
     with open(path, "rb") as file:
         if Path(path).suffix == ".json":
             return json.load(file)
         return file.read().decode("UTF-8")
 
 
-for fingerprint in RESPONSE_DIR.rglob("vehicles_v2_*_0.json"):
-    ALL_FINGERPRINTS.extend(load_response(fingerprint))
+for fingerprint in RESPONSE_DIR.rglob("vehicles_v2_*.json"):
+    brand = fingerprint.stem.split("_")[-2]
+    if brand not in ALL_FINGERPRINTS:
+        ALL_FINGERPRINTS[brand] = []
+    ALL_FINGERPRINTS[brand].extend(load_response(fingerprint))
+
+for state in RESPONSE_DIR.rglob("state_*.json"):
+    ALL_STATES[state.stem.split("_")[-2]] = load_response(state)
 
 
 def get_deprecation_warning_count(caplog):
     """Return all logged DeprecationWarnings."""
     return [r for r in caplog.records if r.levelname == "WARNING" and "DeprecationWarning" in r.message]
```

### Comparing `bimmer_connected-0.9.5/test/responses/auth/auth_cn_login_pwd.json` & `bimmer_connected-0.9.6/test/responses/auth/auth_cn_login_pwd.json`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/test/responses/auth/oauth_config.json` & `bimmer_connected-0.9.6/test/responses/auth/oauth_config.json`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/test/test_account.py` & `bimmer_connected-0.9.6/test/test_account.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """Tests for MyBMWAccount."""
 
 import datetime
 import logging
-from typing import Dict, List
 
 try:
     from unittest import mock
 
     if not hasattr(mock, "AsyncMock"):
         # AsyncMock was only introduced with Python3.8, so we have to use the backported module
         raise ImportError()
@@ -21,20 +20,22 @@
 from bimmer_connected.api.authentication import MyBMWAuthentication, MyBMWLoginRetry
 from bimmer_connected.api.client import MyBMWClient
 from bimmer_connected.api.regions import get_region_from_name
 from bimmer_connected.const import Regions
 from bimmer_connected.models import GPSPosition
 
 from . import (
+    ALL_FINGERPRINTS,
+    ALL_STATES,
     RESPONSE_DIR,
     TEST_PASSWORD,
     TEST_REGION,
     TEST_REGION_STRING,
     TEST_USERNAME,
-    VIN_G21,
+    VIN_G23,
     get_deprecation_warning_count,
     get_fingerprint_count,
     load_response,
 )
 
 
 def authenticate_sideeffect(request: httpx.Request) -> httpx.Response:
@@ -57,19 +58,26 @@
         brand = x_user_agent[1]
     else:
         raise ValueError("x-user-agent not configured correctly!")
 
     # Test if given region is valid
     _ = Regions(x_user_agent[3])
 
-    response_vehicles: List[Dict] = []
-    files = RESPONSE_DIR.rglob(f"vehicles_v2_{brand}_0.json")
-    for file in files:
-        response_vehicles.extend(load_response(file))
-    return httpx.Response(200, json=response_vehicles)
+    return httpx.Response(200, json=ALL_FINGERPRINTS.get(brand, []))
+
+
+def vehicle_state_sideeffect(request: httpx.Request, vin: str) -> httpx.Response:
+    """Returns /vehicles response based on x-user-agent."""
+    x_user_agent = request.headers.get("x-user-agent", "").split(";")
+    assert len(x_user_agent) == 4
+
+    try:
+        return httpx.Response(200, json=ALL_STATES[vin])
+    except KeyError:
+        return httpx.Response(404)
 
 
 def account_mock():
     """Returns mocked adapter for auth."""
     router = respx.mock(assert_all_called=False)
 
     # Login to north_america and rest_of_world
@@ -87,15 +95,18 @@
         200, json=load_response(RESPONSE_DIR / "auth" / "auth_cn_login_pwd.json")
     )
     router.post("/eadrax-coas/v1/oauth/token").respond(
         200, json=load_response(RESPONSE_DIR / "auth" / "auth_token.json")
     )
 
     # Get all vehicle fingerprints
-    router.get("/eadrax-vcs/v1/vehicles").mock(side_effect=vehicles_sideeffect)
+    router.get("/eadrax-vcs/v2/vehicles").mock(side_effect=vehicles_sideeffect)
+
+    # router.get("/eadrax-vcs/v2/vehicles").mock(side_effect=vehicles_sideeffect)
+    router.get(path__regex=r"^/eadrax-vcs/v2/vehicles/(?P<vin>\w+)/state").mock(side_effect=vehicle_state_sideeffect)
 
     return router
 
 
 def get_account(region=None):
     """Returns account without token and vehicles (sync)."""
     return MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, region or TEST_REGION)
@@ -145,15 +156,15 @@
         account = MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, get_region_from_name(TEST_REGION_STRING))
         await account.get_vehicles()
 
         with mock.patch(
             "bimmer_connected.api.authentication.MyBMWAuthentication._refresh_token_row_na",
             wraps=account.config.authentication._refresh_token_row_na,  # pylint: disable=protected-access
         ) as mock_listener:
-            mock_api.get("/eadrax-vcs/v1/vehicles").mock(
+            mock_api.get("/eadrax-vcs/v2/vehicles").mock(
                 side_effect=[httpx.Response(401), *([httpx.Response(200, json=[])] * 10)]
             )
             mock_listener.reset_mock()
             await account.get_vehicles()
 
             assert mock_listener.call_count == 1
             assert account.config.authentication.refresh_token is not None
@@ -218,15 +229,15 @@
         account = MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, get_region_from_name("china"))
         await account.get_vehicles()
 
         with mock.patch(
             "bimmer_connected.api.authentication.MyBMWAuthentication._refresh_token_china",
             wraps=account.config.authentication._refresh_token_china,  # pylint: disable=protected-access
         ) as mock_listener:
-            mock_api.get("/eadrax-vcs/v1/vehicles").mock(
+            mock_api.get("/eadrax-vcs/v2/vehicles").mock(
                 side_effect=[httpx.Response(401), *([httpx.Response(200, json=[])] * 10)]
             )
             mock_listener.reset_mock()
             await account.get_vehicles()
 
             assert mock_listener.call_count == 1
             assert account.config.authentication.refresh_token is not None
@@ -261,16 +272,16 @@
     """Test the login flow."""
     account = MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, get_region_from_name("china"))
     await account.get_vehicles()
 
     assert account.config.authentication.access_token is not None
     assert get_fingerprint_count() == len(account.vehicles)
 
-    vehicle = account.get_vehicle(VIN_G21)
-    assert VIN_G21 == vehicle.vin
+    vehicle = account.get_vehicle(VIN_G23)
+    assert VIN_G23 == vehicle.vin
 
     assert account.get_vehicle("invalid_vin") is None
 
 
 @pytest.mark.asyncio
 async def test_invalid_password():
     """Test parsing the results of an invalid password."""
@@ -321,25 +332,25 @@
 @pytest.mark.asyncio
 async def test_storing_fingerprints(tmp_path):
     """Test the login flow."""
     with account_mock() as mock_api:
         account = MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, TEST_REGION, log_responses=tmp_path)
         await account.get_vehicles()
 
-        mock_api.get("/eadrax-vcs/v1/vehicles").respond(
+        mock_api.get("/eadrax-vcs/v2/vehicles").respond(
             500, text=load_response(RESPONSE_DIR / "auth" / "auth_error_internal_error.txt")
         )
         with pytest.raises(httpx.HTTPStatusError):
             await account.get_vehicles()
 
     files = list(tmp_path.iterdir())
     json_files = [f for f in files if f.suffix == ".json"]
     txt_files = [f for f in files if f.suffix == ".txt"]
 
-    assert len(json_files) == 2
+    assert len(json_files) == (get_fingerprint_count() + 2)
     assert len(txt_files) == 1
 
 
 @pytest.mark.asyncio
 async def test_set_observer_value():
     """Test set_observer_position with valid arguments."""
     account = await get_mocked_account()
@@ -475,15 +486,15 @@
 async def test_429_retry_ok_vehicles(caplog):
     """Test waiting on 429 for vehicles."""
     with account_mock() as mock_api:
         account = MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, TEST_REGION)
 
         json_429 = {"statusCode": 429, "message": "Rate limit is exceeded. Try again in 2 seconds."}
 
-        mock_api.get("/eadrax-vcs/v1/vehicles").mock(
+        mock_api.get("/eadrax-vcs/v2/vehicles").mock(
             side_effect=[
                 httpx.Response(429, json=json_429),
                 httpx.Response(429, json=json_429),
                 *[httpx.Response(200, json=[])] * 2,
             ]
         )
         caplog.set_level(logging.DEBUG)
@@ -503,15 +514,15 @@
 async def test_429_retry_raise_vehicles(caplog):
     """Test waiting on 429 for vehicles and fail if it happens too often."""
     with account_mock() as mock_api:
         account = MyBMWAccount(TEST_USERNAME, TEST_PASSWORD, TEST_REGION)
 
         json_429 = {"statusCode": 429, "message": "Rate limit is exceeded. Try again in 2 seconds."}
 
-        mock_api.get("/eadrax-vcs/v1/vehicles").mock(return_value=httpx.Response(429, json=json_429))
+        mock_api.get("/eadrax-vcs/v2/vehicles").mock(return_value=httpx.Response(429, json=json_429))
         caplog.set_level(logging.DEBUG)
 
         with mock.patch("asyncio.sleep", new_callable=mock.AsyncMock):
             with pytest.raises(httpx.HTTPStatusError):
                 await account.get_vehicles()
 
         log_429 = [
```

### Comparing `bimmer_connected-0.9.5/test/test_api.py` & `bimmer_connected-0.9.6/test/test_api.py`

 * *Files identical despite different names*

### Comparing `bimmer_connected-0.9.5/test/test_deprecated_vehicle.py` & `bimmer_connected-0.9.6/test/test_deprecated_vehicle.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,14 @@
 """Tests for deprecated MyBMWVehicle."""
 import pytest
 
 from bimmer_connected.const import CarBrands
 from bimmer_connected.vehicle.vehicle import ConnectedDriveVehicle
 
-from . import (
-    VIN_F11,
-    VIN_F31,
-    VIN_F35,
-    VIN_F44,
-    VIN_F45,
-    VIN_F48,
-    VIN_G01,
-    VIN_G05,
-    VIN_G08,
-    VIN_G21,
-    VIN_G23,
-    VIN_G30,
-    VIN_I01_NOREX,
-    VIN_I01_REX,
-    get_deprecation_warning_count,
-)
+from . import VIN_F31, VIN_G01, VIN_G20, VIN_G23, VIN_I01_NOREX, VIN_I01_REX, VIN_I20, get_deprecation_warning_count
 from .test_account import get_mocked_account
 
 ATTRIBUTE_MAPPING = {
     "remainingFuel": "remaining_fuel",
     "position": "gps_position",
     "cbsData": "condition_based_services",
     "checkControlMessages": "check_control_messages",
@@ -61,28 +45,21 @@
 
 @pytest.mark.asyncio
 async def test_drive_train_attributes(caplog):
     """Test parsing different attributes of the vehicle."""
     account = await get_mocked_account()
 
     vehicle_drivetrains = {
-        VIN_F11: (True, False, False),
         VIN_F31: (True, False, False),
-        VIN_F35: (True, False, False),
-        VIN_F44: (True, False, False),
-        VIN_F45: (True, True, False),
-        VIN_F48: (True, False, False),
         VIN_G01: (True, True, False),
-        VIN_G05: (True, True, False),
-        VIN_G08: (False, True, False),
-        VIN_G21: (True, True, False),
-        VIN_G23: (True, True, False),
-        VIN_G30: (True, True, False),
+        VIN_G20: (True, False, False),
+        VIN_G23: (False, True, False),
         VIN_I01_NOREX: (False, True, False),
         VIN_I01_REX: (False, True, True),
+        VIN_I20: (False, True, False),
     }
 
     for vehicle in account.vehicles:
         assert vehicle_drivetrains[vehicle.vin][0] == vehicle.has_internal_combustion_engine
         assert vehicle_drivetrains[vehicle.vin][1] == vehicle.has_hv_battery
         assert vehicle_drivetrains[vehicle.vin][2] == vehicle.has_range_extender
```

### Comparing `bimmer_connected-0.9.5/test/test_deprecated_vehicle_status.py` & `bimmer_connected-0.9.6/test/test_deprecated_vehicle_status.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,223 +6,187 @@
 import time_machine
 
 from bimmer_connected.api.regions import get_region_from_name
 from bimmer_connected.vehicle.doors_windows import LidState, LockState
 from bimmer_connected.vehicle.fuel_and_battery import ChargingState
 from bimmer_connected.vehicle.reports import CheckControlStatus, ConditionBasedServiceStatus
 
-from . import VIN_F11, VIN_F31, VIN_F48, VIN_G01, VIN_G08, VIN_G30, VIN_I01_REX, get_deprecation_warning_count
+from . import VIN_F31, VIN_G01, VIN_G20, VIN_G23, VIN_I01_NOREX, VIN_I01_REX, VIN_I20, get_deprecation_warning_count
 from .test_account import get_mocked_account
 
 
 @pytest.mark.asyncio
 async def test_generic(caplog):
     """Test generic attributes."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G23).status
 
-    expected = datetime.datetime(
-        year=2021, month=11, day=11, hour=8, minute=58, second=53, tzinfo=datetime.timezone.utc
-    )
+    expected = datetime.datetime(year=2022, month=6, day=1, hour=19, minute=18, second=54, tzinfo=datetime.timezone.utc)
     assert expected == status.timestamp
 
-    assert 7991 == status.mileage[0]
+    assert 1121 == status.mileage[0]
     assert "km" == status.mileage[1]
 
-    assert (12.3456, 34.5678) == status.gps_position
-    assert 123 == status.gps_heading
+    assert (48.177334, 11.556274) == status.gps_position
+    assert 180 == status.gps_heading
 
     assert status.is_vehicle_active is False
-    assert status.fuel_indicator_count == 3
-    assert status.last_update_reason == "Updated from vehicle 11/12/2021 08:58 AM"
+    assert status.fuel_indicator_count is None
+    assert hasattr(status, "last_update_reason") is True
+    assert status.last_update_reason is None
     assert status.has_parking_light_state is False
 
-    assert len(get_deprecation_warning_count(caplog)) == 9
+    assert len(get_deprecation_warning_count(caplog)) == 10
 
 
 @pytest.mark.asyncio
 async def test_range_combustion_no_info(caplog):
     """Test if the parsing of mileage and range is working"""
     status = (await get_mocked_account()).get_vehicle(VIN_F31).status
 
-    assert (32, "LITERS") == status.remaining_fuel
+    assert (14, "L") == status.remaining_fuel
     assert status.remaining_range_fuel == (None, None)
     assert status.fuel_percent is None
 
     assert status.charging_level_hv is None
     assert status.remaining_range_electric == (None, None)
 
     assert status.remaining_range_total == (None, None)
 
     assert len(get_deprecation_warning_count(caplog)) == 6
 
 
 @pytest.mark.asyncio
 async def test_range_combustion(caplog):
     """Test if the parsing of mileage and range is working"""
-    status = (await get_mocked_account()).get_vehicle(VIN_F48).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G20).status
 
-    assert (19, "LITERS") == status.remaining_fuel
-    assert (308, "km") == status.remaining_range_fuel
-    assert status.fuel_percent is None
+    assert (40, "L") == status.remaining_fuel
+    assert (629, "km") == status.remaining_range_fuel
+    assert status.fuel_percent == 80
 
     assert status.charging_level_hv is None
     assert status.remaining_range_electric == (None, None)
 
-    assert (308, "km") == status.remaining_range_total
+    assert (629, "km") == status.remaining_range_total
 
     assert len(get_deprecation_warning_count(caplog)) == 6
 
 
 @pytest.mark.asyncio
 async def test_range_phev(caplog):
     """Test if the parsing of mileage and range is working"""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).status
 
-    assert (11, "LITERS") == status.remaining_fuel
-    assert (107, "km") == status.remaining_range_fuel
-    assert 28 == status.fuel_percent
+    assert (40, "L") == status.remaining_fuel
+    assert (476, "km") == status.remaining_range_fuel
+    assert 80 == status.fuel_percent
 
-    assert 41 == status.charging_level_hv
-    assert (9, "km") == status.remaining_range_electric
+    assert 80 == status.charging_level_hv
+    assert (40, "km") == status.remaining_range_electric
 
-    assert (116, "km") == status.remaining_range_total
+    assert (516, "km") == status.remaining_range_total
 
     assert status.remaining_range_fuel[0] + status.remaining_range_electric[0] == status.remaining_range_total[0]
 
     assert len(get_deprecation_warning_count(caplog)) == 9
 
 
 @pytest.mark.asyncio
 async def test_range_rex(caplog):
     """Test if the parsing of mileage and range is working"""
     status = (await get_mocked_account()).get_vehicle(VIN_I01_REX).status
 
-    assert (5, "LITERS") == status.remaining_fuel
-    assert (64, "km") == status.remaining_range_fuel
+    assert (6, "L") == status.remaining_fuel
+    assert (105, "km") == status.remaining_range_fuel
     assert status.fuel_percent is None
 
-    assert 100 == status.charging_level_hv
-    assert (164, "km") == status.remaining_range_electric
+    assert 82 == status.charging_level_hv
+    assert (174, "km") == status.remaining_range_electric
 
-    assert (228, "km") == status.remaining_range_total
+    assert (279, "km") == status.remaining_range_total
 
     assert status.remaining_range_fuel[0] + status.remaining_range_electric[0] == status.remaining_range_total[0]
 
     assert len(get_deprecation_warning_count(caplog)) == 9
 
 
 @pytest.mark.asyncio
 async def test_range_electric(caplog):
     """Test if the parsing of mileage and range is working"""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G23).status
 
-    assert (0, "LITERS") == status.remaining_fuel
-    assert status.remaining_range_fuel == (None, None)
-    assert status.fuel_percent is None
+    assert (0, "L") == status.remaining_fuel
+    assert status.remaining_range_fuel == (0, "km")
+    assert status.fuel_percent == 0
 
-    assert 50 == status.charging_level_hv
-    assert (179, "km") == status.remaining_range_electric
+    assert 80 == status.charging_level_hv
+    assert (472, "km") == status.remaining_range_electric
 
-    assert (179, "km") == status.remaining_range_total
+    assert (472, "km") == status.remaining_range_total
 
     assert len(get_deprecation_warning_count(caplog)) == 6
 
 
-@time_machine.travel("2011-11-28 21:28:59 +0000", tick=False)
+@time_machine.travel("2021-11-28 21:28:59 +0000", tick=False)
 @pytest.mark.asyncio
 async def test_charging_end_time(caplog):
     """Test if the parsing of mileage and range is working"""
     account = await get_mocked_account()
-    status = account.get_vehicle(VIN_G08).status
-    assert datetime.datetime(2011, 11, 29, 4, 1, tzinfo=account.timezone) == status.charging_end_time
+    status = account.get_vehicle(VIN_I01_NOREX).status
+    assert datetime.datetime(2021, 11, 28, 23, 27, 59, tzinfo=datetime.timezone.utc) == status.charging_end_time
 
     warnings = [r for r in caplog.records if r.levelname == "WARNING" and "DeprecationWarning" in r.message]
     assert len(warnings) == 1
 
 
 @pytest.mark.asyncio
 async def test_charging_time_label(caplog):
     """Test if the parsing of mileage and range is working"""
     account = await get_mocked_account()
-    status = account.get_vehicle(VIN_G08).status
-    assert "100% at ~04:01 AM" == status.charging_time_label
+    status = account.get_vehicle(VIN_I20).status
+    assert None is status.charging_time_label
 
     assert len(get_deprecation_warning_count(caplog)) == 1
 
 
 @pytest.mark.asyncio
-async def test_charging_end_time_parsing_failure(caplog):
-    """Test if the parsing of mileage and range is working"""
-    account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_G08)
-
-    vehicle.update_state(
-        dict(
-            vehicle.data,
-            **{
-                "status": {
-                    "fuelIndicators": [
-                        {
-                            "chargingStatusIndicatorType": "CHARGING",
-                            "chargingStatusType": "CHARGING",
-                            "infoLabel": "100% at later today...",
-                            "rangeIconId": 59683,
-                            "rangeUnits": "km",
-                            "rangeValue": "179",
-                        }
-                    ]
-                },
-            },
-        )
-    )
-    assert vehicle.status.charging_end_time is None
-    assert "100% at later today..." == vehicle.status.charging_time_label
-
-    errors = [r for r in caplog.records if r.levelname == "ERROR" and "Error parsing charging end time" in r.message]
-    assert len(errors) == 1
-
-    assert len(get_deprecation_warning_count(caplog)) == 2
-
-
-@pytest.mark.asyncio
 async def test_plugged_in_waiting_for_charge_window(caplog):
     """G01 is plugged in but not charging, as its waiting for charging window."""
     # Should be None on G01 as it is only "charging"
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_G01)
+    vehicle = account.get_vehicle(VIN_I01_REX)
 
     assert vehicle.status.charging_end_time is None
-    assert "Starts at ~ 09:00 AM" == vehicle.status.charging_time_label
-    assert ChargingState.PLUGGED_IN == vehicle.status.charging_status
+    assert ChargingState.WAITING_FOR_CHARGING == vehicle.status.charging_status
     assert "CONNECTED" == vehicle.status.connection_status
 
-    assert len(get_deprecation_warning_count(caplog)) == 4
+    assert len(get_deprecation_warning_count(caplog)) == 3
 
 
 @pytest.mark.asyncio
 async def test_condition_based_services(caplog):
     """Test condition based service messages."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G23).status
 
     cbs = status.condition_based_services
     assert 3 == len(cbs)
     assert ConditionBasedServiceStatus.OK == cbs[0].state
-    expected_cbs0 = datetime.datetime(year=2022, month=8, day=1, tzinfo=datetime.timezone.utc)
+    expected_cbs0 = datetime.datetime(year=2024, month=5, day=1, tzinfo=datetime.timezone.utc)
     assert expected_cbs0 == cbs[0].due_date
-    assert (25000, "KILOMETERS") == cbs[0].due_distance
+    assert (50000, "km") == cbs[0].due_distance
 
     assert ConditionBasedServiceStatus.OK == cbs[1].state
-    expected_cbs1 = datetime.datetime(year=2023, month=8, day=1, tzinfo=datetime.timezone.utc)
+    expected_cbs1 = datetime.datetime(year=2024, month=5, day=1, tzinfo=datetime.timezone.utc)
     assert expected_cbs1 == cbs[1].due_date
-    assert (None, None) == cbs[1].due_distance
+    assert (50000, "km") == cbs[1].due_distance
 
     assert ConditionBasedServiceStatus.OK == cbs[2].state
-    expected_cbs2 = datetime.datetime(year=2024, month=8, day=1, tzinfo=datetime.timezone.utc)
+    expected_cbs2 = datetime.datetime(year=2024, month=5, day=1, tzinfo=datetime.timezone.utc)
     assert expected_cbs2 == cbs[2].due_date
-    assert (60000, "KILOMETERS") == cbs[2].due_distance
+    assert (50000, "km") == cbs[2].due_distance
 
     assert status.are_all_cbs_ok is True
 
     assert len(get_deprecation_warning_count(caplog)) == 2
 
 
 @pytest.mark.asyncio
@@ -236,90 +200,74 @@
     assert len(get_deprecation_warning_count(caplog)) == 2
 
 
 @pytest.mark.asyncio
 async def test_parse_gcj02_position(caplog):
     """Test conversion of GCJ02 to WGS84 for china."""
     account = await get_mocked_account(get_region_from_name("china"))
-    vehicle = account.get_vehicle(VIN_F48)
+    vehicle = account.get_vehicle(VIN_G01)
     vehicle.update_state(
         dict(
             vehicle.data,
             **{
-                "properties": {
-                    "vehicleLocation": {
+                "state": {
+                    "location": {
                         "address": {"formatted": "some_formatted_address"},
                         "coordinates": {"latitude": 39.83492, "longitude": 116.23221},
                         "heading": 123,
                     },
                     "lastUpdatedAt": "2021-11-14T20:20:21Z",
-                },
-                "status": {
-                    "FuelAndBattery": [],
-                    "lastUpdatedAt": "2021-11-14T20:20:21Z",
-                },
+                }
             },
         )
     )
     assert (39.8337, 116.22617) == (round(vehicle.status.gps_position[0], 5), round(vehicle.status.gps_position[1], 5))
 
     assert len(get_deprecation_warning_count(caplog)) == 2
 
 
 @pytest.mark.asyncio
-async def test_parse_g08(caplog):
-    """Test if the parsing of the attributes is working."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).status
-
-    assert (179, "km") == status.remaining_range_electric
-    assert (179, "km") == status.remaining_range_total
-    assert ChargingState.CHARGING == status.charging_status
-    assert 50 == status.charging_level_hv
-
-    assert len(get_deprecation_warning_count(caplog)) == 4
-
-
-@pytest.mark.asyncio
 async def test_lids(caplog):
     """Test features around lids."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30).status
+    # status = (await get_mocked_account()).get_vehicle(VIN_G30).status
 
-    assert 6 == len(list(status.lids))
-    assert 3 == len(list(status.open_lids))
-    assert status.all_lids_closed is False
+    # assert 6 == len(list(status.lids))
+    # assert 3 == len(list(status.open_lids))
+    # assert status.all_lids_closed is False
 
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G23).status
 
     for lid in status.lids:
         assert LidState.CLOSED == lid.state
     assert status.all_lids_closed is True
+    assert 0 == len(status.open_lids)
     assert 6 == len(list(status.lids))
 
-    assert len(get_deprecation_warning_count(caplog)) == 6
+    assert len(get_deprecation_warning_count(caplog)) == 4
 
 
 @pytest.mark.asyncio
 async def test_windows_g31(caplog):
     """Test features around windows."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).status
 
     for window in status.windows:
         assert LidState.CLOSED == window.state
 
     assert 5 == len(list(status.windows))
     assert 0 == len(list(status.open_windows))
     assert status.all_windows_closed is True
 
     assert len(get_deprecation_warning_count(caplog)) == 4
 
 
 @pytest.mark.asyncio
 async def test_door_locks(caplog):
     """Test the door locks."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).status
 
     assert LockState.LOCKED == status.door_lock_state
 
     status = (await get_mocked_account()).get_vehicle(VIN_I01_REX).status
 
     assert LockState.UNLOCKED == status.door_lock_state
 
@@ -329,43 +277,31 @@
 @pytest.mark.asyncio
 async def test_check_control_messages(caplog):
     """Test handling of check control messages.
 
     F11 is the only vehicle with active Check Control Messages, so we only expect to get something there.
     However we have no vehicle with issues in check control.
     """
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_F11)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G01)
     assert vehicle.status.has_check_control_messages is True
 
     ccms = vehicle.status.check_control_messages
-    assert 2 == len(ccms)
-
-    assert CheckControlStatus.MEDIUM == ccms[0].state
-    assert (
-        "Charge by driving for longer periods or use external charger. "
-        "Functions requiring battery will be switched off."
-    ) == ccms[0].description_long
-
-    assert "Battery discharged: Start engine" == ccms[0].description_short
-
-    assert CheckControlStatus.LOW == ccms[1].state
-    assert (
-        "System unable to monitor tire pressure. Check tire pressures manually. "
-        "Continued driving possible. Consult service center."
-    ) == ccms[1].description_long
+    assert 1 == len(ccms)
 
-    assert "Flat Tire Monitor (FTM) inactive" == ccms[1].description_short
+    assert CheckControlStatus.LOW == ccms[0].state
+    assert "ENGINE_OIL" == ccms[0].description_short
+    assert None is ccms[0].description_long
 
     assert len(get_deprecation_warning_count(caplog)) == 2
 
 
 @pytest.mark.asyncio
 async def test_functions_without_data(caplog):
     """Test functions that do not return any result anymore."""
-    status = (await get_mocked_account()).get_vehicle(VIN_F11).status
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).status
 
     assert status.last_charging_end_result is None
     assert status.parking_lights is None
     assert status.are_parking_lights_on is None
     assert status.max_range_electric is None
     assert status.charging_time_remaining is None
     assert status.charging_start_time is None
```

### Comparing `bimmer_connected-0.9.5/test/test_remote_services.py` & `bimmer_connected-0.9.6/test/test_remote_services.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 import httpx
 import pytest
 import time_machine
 
 from bimmer_connected.vehicle import remote_services
 from bimmer_connected.vehicle.remote_services import ExecutionState, RemoteServiceStatus
 
-from . import RESPONSE_DIR, VIN_F45, load_response
+from . import RESPONSE_DIR, VIN_G23, load_response
 from .test_account import account_mock, get_mocked_account
 
 _RESPONSE_INITIATED = RESPONSE_DIR / "remote_services" / "eadrax_service_initiated.json"
 _RESPONSE_PENDING = RESPONSE_DIR / "remote_services" / "eadrax_service_pending.json"
 _RESPONSE_DELIVERED = RESPONSE_DIR / "remote_services" / "eadrax_service_delivered.json"
 _RESPONSE_EXECUTED = RESPONSE_DIR / "remote_services" / "eadrax_service_executed.json"
 _RESPONSE_ERROR = RESPONSE_DIR / "remote_services" / "eadrax_service_error.json"
@@ -107,15 +107,15 @@
         ("VEHICLE_FINDER", "trigger_remote_vehicle_finder", False),
         ("HORN_BLOW", "trigger_remote_horn", False),
         ("SEND_POI", "trigger_send_poi", False),
         ("CHARGE_NOW", "trigger_charge_now", True),
     ]
 
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
 
     for service, call, triggers_update in services:
         with mock.patch(
             "bimmer_connected.account.MyBMWAccount.get_vehicles", new_callable=mock.AsyncMock
         ) as mock_listener:
             mock_listener.reset_mock()
 
@@ -134,15 +134,15 @@
 @pytest.mark.asyncio
 async def test_get_remote_service_status():
     """Test get_remove_service_status method."""
     # pylint: disable=protected-access
     remote_services._POLLING_CYCLE = 0
 
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
 
     with remote_services_mock() as mock_api:
         mock_api.post("/eadrax-vrccs/v2/presentation/remote-commands/eventStatus", params={"eventId": mock.ANY}).mock(
             side_effect=[
                 httpx.Response(500),
                 httpx.Response(200, text="You can't parse this..."),
                 httpx.Response(200, json=load_response(_RESPONSE_ERROR)),
@@ -161,20 +161,20 @@
 @pytest.mark.asyncio
 async def test_get_remote_position():
     """Test getting position from remote service."""
     remote_services._POLLING_CYCLE = 0  # pylint: disable=protected-access
 
     account = await get_mocked_account()
     account.set_observer_position(1.0, 0.0)
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
     status = vehicle.status
 
     # Check original position
-    assert (12.3456, 34.5678) == status.gps_position
-    assert 123 == status.gps_heading
+    assert (48.177334, 11.556274) == status.gps_position
+    assert 180 == status.gps_heading
 
     # Check updated position
     await vehicle.remote_services.trigger_remote_vehicle_finder()
     assert (123.456, 34.5678) == status.gps_position
     assert 121 == status.gps_heading
 
     # Position should still be from vehicle finder after status update
@@ -186,15 +186,15 @@
 @remote_services_mock()
 @pytest.mark.asyncio
 async def test_get_remote_position_fail_without_observer(caplog):
     """Test getting position from remote service."""
     remote_services._POLLING_CYCLE = 0  # pylint: disable=protected-access
 
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
 
     await vehicle.remote_services.trigger_remote_vehicle_finder()
     errors = [
         r
         for r in caplog.records
         if r.levelname == "ERROR"
         and "Unknown position: Set observer position to retrieve vehicle coordinates" in r.message
@@ -206,41 +206,41 @@
 @pytest.mark.asyncio
 async def test_fail_with_timeout():
     """Test failing after timeout was reached."""
     remote_services._POLLING_CYCLE = 1  # pylint: disable=protected-access
     remote_services._POLLING_TIMEOUT = 2  # pylint: disable=protected-access
 
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
 
     with pytest.raises(TimeoutError):
         await vehicle.remote_services.trigger_remote_light_flash()
 
 
 @time_machine.travel("2020-01-01", tick=False)
 @remote_services_mock()
 @pytest.mark.asyncio
 async def test_get_remote_position_too_old():
     """Test remote service position being ignored as vehicle status is newer."""
     remote_services._POLLING_CYCLE = 0  # pylint: disable=protected-access
 
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
     status = vehicle.status
 
     await vehicle.remote_services.trigger_remote_vehicle_finder()
 
-    assert (12.3456, 34.5678) == status.gps_position
-    assert 123 == status.gps_heading
+    assert (48.177334, 11.556274) == status.gps_position
+    assert 180 == status.gps_heading
 
 
 @remote_services_mock()
 @pytest.mark.asyncio
 async def test_poi():
     """Test get_remove_service_status method."""
     remote_services._POLLING_CYCLE = 0  # pylint: disable=protected-access
 
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_F45)
+    vehicle = account.get_vehicle(VIN_G23)
 
     with pytest.raises(TypeError):
         await vehicle.remote_services.trigger_send_poi({"lat": 12.34})
```

### Comparing `bimmer_connected-0.9.5/test/test_utils.py` & `bimmer_connected-0.9.6/test/test_utils.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,83 +1,55 @@
 """Tests for utils."""
 import datetime
 import json
-import os
 import sys
-import time
-from unittest import mock
+
+try:
+    import zoneinfo
+except ImportError:
+    from backports import zoneinfo  # type: ignore[import, no-redef]
 
 import pytest
 import time_machine
 
+from bimmer_connected.models import ValueWithUnit
 from bimmer_connected.utils import MyBMWJSONEncoder, get_class_property_names, parse_datetime
 
-from . import RESPONSE_DIR, VIN_G21, get_deprecation_warning_count
+from . import VIN_G23
 from .test_account import get_mocked_account
 
 
 @pytest.mark.asyncio
 async def test_drive_train():
     """Tests available attribute."""
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_G21)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G23)
     assert [
         "available_attributes",
         "brand",
         "drive_train",
         "drive_train_attributes",
-        "fuel_indicator_count",
         "has_combustion_drivetrain",
         "has_electric_drivetrain",
         "has_hv_battery",
         "has_internal_combustion_engine",
         "has_range_extender",
         "has_range_extender_drivetrain",
         "has_weekly_planner_service",
         "is_charging_plan_supported",
         "is_lsc_enabled",
         "is_vehicle_active",
         "is_vehicle_tracking_enabled",
-        "last_update_reason",
         "lsc_type",
         "mileage",
         "name",
         "timestamp",
         "vin",
     ] == get_class_property_names(vehicle)
 
 
-@time_machine.travel("2011-11-28 21:28:59 +0000", tick=False)
-@pytest.mark.asyncio
-async def test_to_json(caplog):
-    """Test serialization to JSON."""
-    with mock.patch("bimmer_connected.account.MyBMWAccount.timezone", new_callable=mock.PropertyMock) as mock_timezone:
-        # Force UTC
-        os.environ["TZ"] = "UTC"
-        time.tzset()
-        mock_timezone.return_value = datetime.timezone.utc
-
-        account = await get_mocked_account()
-        vehicle = account.get_vehicle(VIN_G21)
-
-        # Unset UTC after vehicle has been loaded
-        del os.environ["TZ"]
-        time.tzset()
-
-        with open(RESPONSE_DIR / "G21" / "json_export.json", "rb") as file:
-            expected = file.read().decode("UTF-8")
-
-        expected_lines = expected.splitlines()
-        actual_lines = json.dumps(vehicle, cls=MyBMWJSONEncoder, indent=4).splitlines()
-
-        for i in range(max(len(expected_lines), len(actual_lines))):
-            assert expected_lines[i] == actual_lines[i], f"line {i+1}"
-
-        assert len(get_deprecation_warning_count(caplog)) == 0
-
-
 def test_parse_datetime(caplog):
     """Test datetime parser."""
 
     dt_without_milliseconds = datetime.datetime(2021, 11, 12, 13, 14, 15, tzinfo=datetime.timezone.utc)
 
     assert dt_without_milliseconds == parse_datetime("2021-11-12T13:14:15.567Z")
 
@@ -87,7 +59,44 @@
         # Don't test timezone parsing on Python 3.6 (not supported there)
         assert dt_without_milliseconds == parse_datetime("2021-11-12T16:14:15+03:00")
 
     unparseable_datetime = "2021-14-12T13:14:15Z"
     assert parse_datetime(unparseable_datetime) is None
     errors = [r for r in caplog.records if r.levelname == "ERROR" and unparseable_datetime in r.message]
     assert len(errors) == 1
+
+
+@time_machine.travel(
+    datetime.datetime(2011, 11, 28, tzinfo=zoneinfo.ZoneInfo("America/Los_Angeles")),
+    tick=False,
+)
+@pytest.mark.asyncio
+async def test_account_timezone():
+    """Test the timezone in MyBMWAccount."""
+    # mocking the timezone doesn't work with the time_machine<2.7.1 on Python 3.6
+    if sys.version_info > (3, 7):
+        account = await get_mocked_account()
+        assert account.utcdiff == 960
+
+
+def test_json_encoder():
+    """Test the MyBMWJSONEncoder."""
+    encoded = json.dumps(
+        {
+            "datetime": datetime.datetime(2022, 6, 2, 22, 19, 34, 123456),
+            "date": datetime.date(2022, 6, 2),
+            "value": ValueWithUnit(17, "mi"),
+            "list": [
+                {
+                    "value_int": 1,
+                    "value_str": "string",
+                },
+                zoneinfo.ZoneInfo("America/Los_Angeles"),
+            ],
+        },
+        cls=MyBMWJSONEncoder,
+    )
+
+    assert (
+        '{"datetime": "2022-06-02T22:19:34.123456", "date": "2022-06-02", "value": [17, "mi"],'
+        ' "list": [{"value_int": 1, "value_str": "string"}, "America/Los_Angeles"]}'
+    ) == encoded
```

### Comparing `bimmer_connected-0.9.5/test/test_vehicle.py` & `bimmer_connected-0.9.6/test/test_vehicle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,16 @@
 """Tests for MyBMWVehicle."""
 import pytest
 
-from bimmer_connected.const import CarBrands
+from bimmer_connected.const import ATTR_ATTRIBUTES, ATTR_STATE, CarBrands
 from bimmer_connected.models import GPSPosition, StrEnum, VehicleDataBase
 from bimmer_connected.vehicle import DriveTrainType, VehicleViewDirection
+from bimmer_connected.vehicle.reports import CheckControlMessageReport
 
-from . import (
-    VIN_F11,
-    VIN_F31,
-    VIN_F35,
-    VIN_F44,
-    VIN_F45,
-    VIN_F48,
-    VIN_G01,
-    VIN_G05,
-    VIN_G08,
-    VIN_G21,
-    VIN_G23,
-    VIN_G30,
-    VIN_I01_NOREX,
-    VIN_I01_REX,
-    get_deprecation_warning_count,
-)
+from . import VIN_F31, VIN_G01, VIN_G20, VIN_G23, VIN_I01_NOREX, VIN_I01_REX, VIN_I20, get_deprecation_warning_count
 from .test_account import account_mock, get_mocked_account
 
 ATTRIBUTE_MAPPING = {
     "remainingFuel": "remaining_fuel",
     "position": "gps_position",
     "cbsData": "condition_based_services",
     "checkControlMessages": "check_control_messages",
@@ -41,17 +26,29 @@
     "chargingTimeRemaining": "charging_time_remaining",
 }
 
 
 @pytest.mark.asyncio
 async def test_drive_train(caplog):
     """Tests around drive_train attribute."""
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_G21)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_F31)
+    assert DriveTrainType.COMBUSTION == vehicle.drive_train
+
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G01)
     assert DriveTrainType.PLUGIN_HYBRID == vehicle.drive_train
 
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G23)
+    assert DriveTrainType.ELECTRIC == vehicle.drive_train
+
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_I01_NOREX)
+    assert DriveTrainType.ELECTRIC == vehicle.drive_train
+
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_I01_REX)
+    assert DriveTrainType.ELECTRIC_WITH_RANGE_EXTENDER == vehicle.drive_train
+
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_parsing_attributes(caplog):
     """Test parsing different attributes of the vehicle."""
     account = await get_mocked_account()
@@ -71,28 +68,21 @@
 
 @pytest.mark.asyncio
 async def test_drive_train_attributes(caplog):
     """Test parsing different attributes of the vehicle."""
     account = await get_mocked_account()
 
     vehicle_drivetrains = {
-        VIN_F11: (True, False, False),
         VIN_F31: (True, False, False),
-        VIN_F35: (True, False, False),
-        VIN_F44: (True, False, False),
-        VIN_F45: (True, True, False),
-        VIN_F48: (True, False, False),
         VIN_G01: (True, True, False),
-        VIN_G05: (True, True, False),
-        VIN_G08: (False, True, False),
-        VIN_G21: (True, True, False),
-        VIN_G23: (True, True, False),
-        VIN_G30: (True, True, False),
+        VIN_G20: (True, False, False),
+        VIN_G23: (False, True, False),
         VIN_I01_NOREX: (False, True, False),
         VIN_I01_REX: (False, True, True),
+        VIN_I20: (False, True, False),
     }
 
     for vehicle in account.vehicles:
         assert vehicle_drivetrains[vehicle.vin][0] == vehicle.has_combustion_drivetrain
         assert vehicle_drivetrains[vehicle.vin][1] == vehicle.has_electric_drivetrain
         assert vehicle_drivetrains[vehicle.vin][2] == vehicle.has_range_extender_drivetrain
 
@@ -119,15 +109,15 @@
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_get_is_tracking_enabled(caplog):
     """Test setting observer position"""
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_F11)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_I01_REX)
     assert vehicle.is_vehicle_tracking_enabled is False
 
     vehicle = (await get_mocked_account()).get_vehicle(VIN_F31)
     assert vehicle.is_vehicle_tracking_enabled is True
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
@@ -136,74 +126,68 @@
 async def test_available_attributes(caplog):
     """Check that available_attributes returns exactly the arguments we have in our test data."""
     account = await get_mocked_account()
 
     vehicle = account.get_vehicle(VIN_F31)
     assert ["gps_position", "vin"] == vehicle.available_attributes
 
-    vehicle = account.get_vehicle(VIN_G08)
+    vehicle = account.get_vehicle(VIN_G01)
     assert [
         "gps_position",
         "vin",
         "remaining_range_total",
         "mileage",
         "charging_time_remaining",
-        "charging_start_time",
         "charging_end_time",
         "charging_time_label",
         "charging_status",
         "connection_status",
         "remaining_battery_percent",
         "remaining_range_electric",
         "last_charging_end_result",
+        "remaining_fuel",
+        "remaining_range_fuel",
+        "remaining_fuel_percent",
         "condition_based_services",
         "check_control_messages",
         "door_lock_state",
         "timestamp",
-        "last_update_reason",
         "lids",
         "windows",
-        "convertible_top",
     ] == vehicle.available_attributes
 
-    vehicle = account.get_vehicle(VIN_G30)
+    vehicle = account.get_vehicle(VIN_G23)
     assert [
         "gps_position",
         "vin",
         "remaining_range_total",
         "mileage",
         "charging_time_remaining",
-        "charging_start_time",
         "charging_end_time",
         "charging_time_label",
         "charging_status",
         "connection_status",
         "remaining_battery_percent",
         "remaining_range_electric",
         "last_charging_end_result",
-        "remaining_fuel",
-        "remaining_range_fuel",
-        "remaining_fuel_percent",
         "condition_based_services",
         "check_control_messages",
         "door_lock_state",
         "timestamp",
-        "last_update_reason",
         "lids",
         "windows",
-        "convertible_top",
     ] == vehicle.available_attributes
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_vehicle_image(caplog):
     """Test vehicle image request."""
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_G05)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G01)
 
     with account_mock() as mock_api:
         mock_api.get(
             path__regex=r"(.*)/eadrax-ics/v3/presentation/vehicles/\w*/images",
             params={"carView": "VehicleInfo"},
             headers={"accept": "image/png"},
         ).respond(200, content="png_image")
@@ -212,41 +196,61 @@
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_no_timestamp():
     """Test no timestamp available."""
     vehicle = (await get_mocked_account()).get_vehicle(VIN_F31)
-    vehicle._properties.pop("lastUpdatedAt")  # pylint: disable=protected-access
-    vehicle._status.pop("lastUpdatedAt")  # pylint: disable=protected-access
+    vehicle.data[ATTR_STATE].pop("lastFetched")  # pylint: disable=protected-access
+    vehicle.data[ATTR_ATTRIBUTES].pop("lastFetched")  # pylint: disable=protected-access
 
     assert vehicle.timestamp is None
 
 
-def test_strenum():
+def test_strenum(caplog):
     """Tests StrEnum."""
 
     class TestEnum(StrEnum):
         """Test StrEnum."""
 
         HELLO = "HELLO"
 
     assert TestEnum("hello") == TestEnum.HELLO
     assert TestEnum("HELLO") == TestEnum.HELLO
 
     with pytest.raises(ValueError):
         TestEnum("WORLD")
 
+    class TestEnumUnkown(StrEnum):
+        """Test StrEnum with UNKNOWN value."""
+
+        HELLO = "HELLO"
+        UNKNOWN = "UNKNOWN"
+
+    assert TestEnumUnkown("hello") == TestEnumUnkown.HELLO
+    assert TestEnumUnkown("HELLO") == TestEnumUnkown.HELLO
+
+    assert len([r for r in caplog.records if r.levelname == "WARNING"]) == 0
+    assert TestEnumUnkown("WORLD") == TestEnumUnkown.UNKNOWN
+    assert len([r for r in caplog.records if r.levelname == "WARNING"]) == 1
+
 
 def test_vehiclebasedata():
     """Tests VehicleBaseData."""
     with pytest.raises(NotImplementedError):
         VehicleDataBase._parse_vehicle_data({})  # pylint: disable=protected-access
 
+    # CheckControlMessageReport does not override parent methods from_vehicle_data()
+    ccmr = CheckControlMessageReport.from_vehicle_data(
+        {"state": {"checkControlMessages": [{"severity": "LOW", "type": "ENGINE_OIL"}]}}
+    )
+    assert len(ccmr.messages) == 1
+
 
 def test_gpsposition():
     """Tests around GPSPosition."""
     pos = GPSPosition(1.0, 2.0)
     assert pos == GPSPosition(1, 2)
     assert pos == {"latitude": 1.0, "longitude": 2.0}
     assert pos == (1, 2)
     assert pos != "(1, 2)"
+    assert pos[0] == 1
```

### Comparing `bimmer_connected-0.9.5/test/test_vehicle_status.py` & `bimmer_connected-0.9.6/test/test_vehicle_status.py`

 * *Files 15% similar despite different names*

```diff
@@ -7,274 +7,240 @@
 
 from bimmer_connected.api.regions import get_region_from_name
 from bimmer_connected.vehicle.doors_windows import LidState, LockState
 from bimmer_connected.vehicle.fuel_and_battery import ChargingState, FuelAndBattery
 from bimmer_connected.vehicle.location import VehicleLocation
 from bimmer_connected.vehicle.reports import CheckControlStatus, ConditionBasedServiceStatus
 
-from . import VIN_F11, VIN_F31, VIN_F48, VIN_G01, VIN_G08, VIN_G23, VIN_G30, VIN_I01_REX, get_deprecation_warning_count
+from . import VIN_F31, VIN_G01, VIN_G20, VIN_G23, VIN_I01_NOREX, VIN_I01_REX, get_deprecation_warning_count
 from .test_account import get_mocked_account
 
 
 @pytest.mark.asyncio
 async def test_generic(caplog):
     """Test generic attributes."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30)
+    status = (await get_mocked_account()).get_vehicle(VIN_G23)
 
-    expected = datetime.datetime(
-        year=2021, month=11, day=11, hour=8, minute=58, second=53, tzinfo=datetime.timezone.utc
-    )
+    expected = datetime.datetime(year=2022, month=6, day=1, hour=19, minute=18, second=54, tzinfo=datetime.timezone.utc)
     assert expected == status.timestamp
 
-    assert 7991 == status.mileage[0]
+    assert 1121 == status.mileage[0]
     assert "km" == status.mileage[1]
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_range_combustion_no_info(caplog):
     """Test if the parsing of mileage and range is working"""
     vehicle = (await get_mocked_account()).get_vehicle(VIN_F31)
     status = vehicle.fuel_and_battery
 
-    assert (32, "LITERS") == status.remaining_fuel
+    assert (14, "L") == status.remaining_fuel
     assert status.remaining_range_fuel == (None, None)
     assert status.remaining_fuel_percent is None
 
     assert status.remaining_battery_percent is None
     assert status.remaining_range_electric == (None, None)
 
     assert status.remaining_range_total == (None, None)
 
     status_from_vehicle_data = FuelAndBattery.from_vehicle_data(vehicle.data)
     status_from_vehicle_data.account_timezone = status.account_timezone
     assert status_from_vehicle_data == status
     assert FuelAndBattery.from_vehicle_data({}) is None
 
-    # pylint: disable=protected-access
-    assert FuelAndBattery._parse_to_tuple({"rangeValue": "seventeen", "rangeUnit": "mi"}) == (None, None)
-
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_range_combustion(caplog):
     """Test if the parsing of mileage and range is working"""
-    status = (await get_mocked_account()).get_vehicle(VIN_F48).fuel_and_battery
+    status = (await get_mocked_account()).get_vehicle(VIN_G20).fuel_and_battery
 
-    assert (19, "LITERS") == status.remaining_fuel
-    assert (308, "km") == status.remaining_range_fuel
-    assert status.remaining_fuel_percent is None
+    assert (40, "L") == status.remaining_fuel
+    assert (629, "km") == status.remaining_range_fuel
+    assert status.remaining_fuel_percent == 80
 
     assert status.remaining_battery_percent is None
     assert status.remaining_range_electric == (None, None)
 
-    assert (308, "km") == status.remaining_range_total
+    assert (629, "km") == status.remaining_range_total
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_range_phev(caplog):
     """Test if the parsing of mileage and range is working"""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30).fuel_and_battery
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).fuel_and_battery
 
-    assert (11, "LITERS") == status.remaining_fuel
-    assert (107, "km") == status.remaining_range_fuel
-    assert 28 == status.remaining_fuel_percent
+    assert (40, "L") == status.remaining_fuel
+    assert (476, "km") == status.remaining_range_fuel
+    assert 80 == status.remaining_fuel_percent
 
-    assert 41 == status.remaining_battery_percent
-    assert (9, "km") == status.remaining_range_electric
+    assert 80 == status.remaining_battery_percent
+    assert (40, "km") == status.remaining_range_electric
 
-    assert (116, "km") == status.remaining_range_total
+    assert (516, "km") == status.remaining_range_total
 
     assert status.remaining_range_fuel[0] + status.remaining_range_electric[0] == status.remaining_range_total[0]
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_range_rex(caplog):
     """Test if the parsing of mileage and range is working"""
     status = (await get_mocked_account()).get_vehicle(VIN_I01_REX).fuel_and_battery
 
-    assert (5, "LITERS") == status.remaining_fuel
-    assert (64, "km") == status.remaining_range_fuel
+    assert (6, "L") == status.remaining_fuel
+    assert (105, "km") == status.remaining_range_fuel
     assert status.remaining_fuel_percent is None
 
-    assert 100 == status.remaining_battery_percent
-    assert (164, "km") == status.remaining_range_electric
+    assert 82 == status.remaining_battery_percent
+    assert (174, "km") == status.remaining_range_electric
 
-    assert (228, "km") == status.remaining_range_total
+    assert (279, "km") == status.remaining_range_total
 
     assert status.remaining_range_fuel[0] + status.remaining_range_electric[0] == status.remaining_range_total[0]
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_range_electric(caplog):
     """Test if the parsing of mileage and range is working"""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).fuel_and_battery
+    status = (await get_mocked_account()).get_vehicle(VIN_G23).fuel_and_battery
 
-    assert (0, "LITERS") == status.remaining_fuel
-    assert status.remaining_range_fuel == (None, None)
-    assert status.remaining_fuel_percent is None
+    assert (0, "L") == status.remaining_fuel
+    assert status.remaining_range_fuel == (0, "km")
+    assert status.remaining_fuel_percent == 0
 
-    assert 50 == status.remaining_battery_percent
-    assert (179, "km") == status.remaining_range_electric
+    assert 80 == status.remaining_battery_percent
+    assert (472, "km") == status.remaining_range_electric
 
-    assert (179, "km") == status.remaining_range_total
+    assert (472, "km") == status.remaining_range_total
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
-@time_machine.travel("2011-11-28 21:28:59 +0000", tick=False)
+@time_machine.travel("2021-11-28 21:28:59 +0000", tick=False)
 @pytest.mark.asyncio
 async def test_charging_end_time(caplog):
     """Test if the parsing of mileage and range is working"""
     account = await get_mocked_account()
-    status = account.get_vehicle(VIN_G08).fuel_and_battery
-    assert datetime.datetime(2011, 11, 29, 4, 1, tzinfo=account.timezone) == status.charging_end_time
-
-    assert len(get_deprecation_warning_count(caplog)) == 0
-
-
-@pytest.mark.asyncio
-async def test_charging_time_label(caplog):
-    """Test if the parsing of mileage and range is working"""
-    account = await get_mocked_account()
-    status = account.get_vehicle(VIN_G08).fuel_and_battery
-    assert "100% at ~04:01 AM" == status.charging_time_label
-
-    assert len(get_deprecation_warning_count(caplog)) == 0
-
-
-@pytest.mark.asyncio
-async def test_charging_end_time_parsing_failure(caplog):
-    """Test if the parsing of mileage and range is working"""
-    account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_G08)
+    vehicle = account.get_vehicle(VIN_I01_NOREX)
 
-    vehicle.update_state(
-        dict(
-            vehicle.data,
-            **{
-                "status": {
-                    "fuelIndicators": [
-                        {
-                            "chargingStatusIndicatorType": "CHARGING",
-                            "chargingStatusType": "CHARGING",
-                            "infoLabel": "100% at later today...",
-                            "rangeIconId": 59683,
-                            "rangeUnits": "km",
-                            "rangeValue": "179",
-                        }
-                    ]
-                },
-            },
-        )
+    assert vehicle.fuel_and_battery.charging_end_time == datetime.datetime(
+        2021, 11, 28, 23, 27, 59, tzinfo=datetime.timezone.utc
     )
-    assert vehicle.fuel_and_battery.charging_end_time is None
-    assert "100% at later today..." == vehicle.fuel_and_battery.charging_time_label
-
-    errors = [r for r in caplog.records if r.levelname == "ERROR" and "Error parsing charging end time" in r.message]
-    assert len(errors) == 1
+    assert vehicle.fuel_and_battery.charging_status == ChargingState.CHARGING
+    assert vehicle.fuel_and_battery.is_charger_connected is True
+    assert vehicle.fuel_and_battery.charging_start_time is None
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
+@time_machine.travel("2021-11-28 17:28:59 +0000", tick=False)
 @pytest.mark.asyncio
 async def test_plugged_in_waiting_for_charge_window(caplog):
-    """G01 is plugged in but not charging, as its waiting for charging window."""
-    # Should be None on G01 as it is only "charging"
+    """I01_REX is plugged in but not charging, as its waiting for charging window."""
     account = await get_mocked_account()
-    vehicle = account.get_vehicle(VIN_G01)
+    vehicle = account.get_vehicle(VIN_I01_REX)
 
     assert vehicle.fuel_and_battery.charging_end_time is None
-    assert "Starts at ~ 09:00 AM" == vehicle.fuel_and_battery.charging_time_label
-    assert ChargingState.PLUGGED_IN == vehicle.fuel_and_battery.charging_status
+    assert vehicle.fuel_and_battery.charging_status == ChargingState.WAITING_FOR_CHARGING
     assert vehicle.fuel_and_battery.is_charger_connected is True
+    assert vehicle.fuel_and_battery.charging_start_time == datetime.datetime(
+        2021, 11, 28, 18, 1, tzinfo=account.timezone
+    )
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_condition_based_services(caplog):
     """Test condition based service messages."""
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_G30)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G23)
 
     cbs = vehicle.condition_based_services.messages
     assert 3 == len(cbs)
     assert ConditionBasedServiceStatus.OK == cbs[0].state
-    expected_cbs0 = datetime.datetime(year=2022, month=8, day=1, tzinfo=datetime.timezone.utc)
+    expected_cbs0 = datetime.datetime(year=2024, month=5, day=1, tzinfo=datetime.timezone.utc)
     assert expected_cbs0 == cbs[0].due_date
-    assert (25000, "KILOMETERS") == cbs[0].due_distance
+    assert (50000, "km") == cbs[0].due_distance
 
     assert ConditionBasedServiceStatus.OK == cbs[1].state
-    expected_cbs1 = datetime.datetime(year=2023, month=8, day=1, tzinfo=datetime.timezone.utc)
+    expected_cbs1 = datetime.datetime(year=2024, month=5, day=1, tzinfo=datetime.timezone.utc)
     assert expected_cbs1 == cbs[1].due_date
-    assert (None, None) == cbs[1].due_distance
+    assert (50000, "km") == cbs[1].due_distance
 
     assert ConditionBasedServiceStatus.OK == cbs[2].state
-    expected_cbs2 = datetime.datetime(year=2024, month=8, day=1, tzinfo=datetime.timezone.utc)
+    expected_cbs2 = datetime.datetime(year=2024, month=5, day=1, tzinfo=datetime.timezone.utc)
     assert expected_cbs2 == cbs[2].due_date
-    assert (60000, "KILOMETERS") == cbs[2].due_distance
+    assert (50000, "km") == cbs[2].due_distance
 
     assert vehicle.condition_based_services.is_service_required is False
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_position_generic(caplog):
     """Test generic attributes."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30)
+    status = (await get_mocked_account()).get_vehicle(VIN_G23)
 
-    assert (12.3456, 34.5678) == status.vehicle_location.location
-    assert 123 == status.vehicle_location.heading
+    assert (48.177334, 11.556274) == status.vehicle_location.location
+    assert 180 == status.vehicle_location.heading
 
     assert VehicleLocation.from_vehicle_data(status.data).location == status.vehicle_location.location
 
     assert VehicleLocation.from_vehicle_data({}) is None
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
+async def test_vehicle_active(caplog):
+    """Test that vehicle_active is always False."""
+    account = await get_mocked_account()
+
+    for vehicle in account.vehicles:
+        assert vehicle.is_vehicle_active is False
+
+    assert len(get_deprecation_warning_count(caplog)) == 0
+
+
+@pytest.mark.asyncio
 async def test_parse_f31_no_position(caplog):
     """Test parsing of F31 data with position tracking disabled in the vehicle."""
     vehicle = (await get_mocked_account()).get_vehicle(VIN_F31)
 
     assert vehicle.vehicle_location.location == (None, None)
     assert vehicle.vehicle_location.heading is None
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
 async def test_parse_gcj02_position(caplog):
     """Test conversion of GCJ02 to WGS84 for china."""
     account = await get_mocked_account(get_region_from_name("china"))
-    vehicle = account.get_vehicle(VIN_F48)
+    vehicle = account.get_vehicle(VIN_G01)
 
     vehicle_test_data = {
-        "properties": {
-            "vehicleLocation": {
+        "state": {
+            "location": {
                 "address": {"formatted": "some_formatted_address"},
                 "coordinates": {"latitude": 39.83492, "longitude": 116.23221},
                 "heading": 123,
             },
             "lastUpdatedAt": "2021-11-14T20:20:21Z",
         },
-        "status": {
-            "FuelAndBattery": [],
-            "lastUpdatedAt": "2021-11-14T20:20:21Z",
-        },
     }
 
     vehicle.update_state(dict(vehicle.data, **vehicle_test_data))
 
     # Update twice to test against slowly crawling position due to GCJ02 to WGS84 conversion
     vehicle.update_state(dict(vehicle.data, **vehicle_test_data))
 
@@ -283,82 +249,60 @@
         round(vehicle.vehicle_location.location[1], 5),
     )
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
-async def test_parse_g08(caplog):
-    """Test if the parsing of the attributes is working."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).fuel_and_battery
-
-    assert (179, "km") == status.remaining_range_electric
-    assert (179, "km") == status.remaining_range_total
-    assert ChargingState.CHARGING == status.charging_status
-    assert 50 == status.remaining_battery_percent
-
-    assert len(get_deprecation_warning_count(caplog)) == 0
-
-
-# def test_missing_attribute(caplog):
-#     """Test if error handling is working correctly."""
-#     account = unittest.mock.MagicMock(MyBMWAccount)
-#     state = VehicleState(account, None)
-#     state._attributes[SERVICE_STATUS] = {}
-#     assert status.mileage is None
-
-
-@pytest.mark.asyncio
 async def test_lids(caplog):
     """Test features around lids."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G30).doors_and_windows
+    # status = (await get_mocked_account()).get_vehicle(VIN_G01).doors_and_windows
 
-    assert 6 == len(list(status.lids))
-    assert 3 == len(list(status.open_lids))
-    assert status.all_lids_closed is False
+    # assert 6 == len(list(status.lids))
+    # assert 3 == len(list(status.open_lids))
+    # assert status.all_lids_closed is False
 
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).doors_and_windows
+    status = (await get_mocked_account()).get_vehicle(VIN_G23).doors_and_windows
 
     for lid in status.lids:
         assert LidState.CLOSED == lid.state
     assert status.all_lids_closed is True
     assert 6 == len(list(status.lids))
 
+    status = (await get_mocked_account()).get_vehicle(VIN_I01_REX).doors_and_windows
+
+    for lid in status.lids:
+        assert LidState.CLOSED == lid.state
+    assert status.all_lids_closed is True
+    assert 7 == len(list(status.lids))
+
+    assert status.lids[-1].name == "sunRoof"
+
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
-async def test_windows_g31(caplog):
+async def test_windows_g01(caplog):
     """Test features around windows."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).doors_and_windows
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).doors_and_windows
 
     for window in status.windows:
         assert LidState.CLOSED == window.state
 
     assert 5 == len(list(status.windows))
     assert 0 == len(list(status.open_windows))
     assert status.all_windows_closed is True
 
     assert len(get_deprecation_warning_count(caplog)) == 0
 
 
 @pytest.mark.asyncio
-async def test_convertible_roof_g23(caplog):
-    """Test features around windows."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G23).doors_and_windows
-
-    assert status.convertible_top == LidState.OPEN
-
-    assert len(get_deprecation_warning_count(caplog)) == 0
-
-
-@pytest.mark.asyncio
 async def test_door_locks(caplog):
     """Test the door locks."""
-    status = (await get_mocked_account()).get_vehicle(VIN_G08).doors_and_windows
+    status = (await get_mocked_account()).get_vehicle(VIN_G01).doors_and_windows
 
     assert LockState.LOCKED == status.door_lock_state
 
     status = (await get_mocked_account()).get_vehicle(VIN_I01_REX).doors_and_windows
 
     assert LockState.UNLOCKED == status.door_lock_state
 
@@ -368,30 +312,40 @@
 @pytest.mark.asyncio
 async def test_check_control_messages(caplog):
     """Test handling of check control messages.
 
     F11 is the only vehicle with active Check Control Messages, so we only expect to get something there.
     However we have no vehicle with issues in check control.
     """
-    vehicle = (await get_mocked_account()).get_vehicle(VIN_F11)
+    vehicle = (await get_mocked_account()).get_vehicle(VIN_G01)
     assert vehicle.check_control_messages.has_check_control_messages is True
 
     ccms = vehicle.check_control_messages.messages
-    assert 2 == len(ccms)
+    assert 1 == len(ccms)
+
+    assert CheckControlStatus.LOW == ccms[0].state
+    assert "ENGINE_OIL" == ccms[0].description_short
+    assert None is ccms[0].description_long
+
+    assert len(get_deprecation_warning_count(caplog)) == 0
+
+
+@pytest.mark.asyncio
+async def test_charging_profile(caplog):
+    """Test parsing of the charing profile"""
+
+    charging_profile = (await get_mocked_account()).get_vehicle(VIN_I01_REX).charging_profile
+    assert charging_profile.is_pre_entry_climatization_enabled is False
+
+    departure_timer = charging_profile.departure_times[0]
+    assert departure_timer.timer_id == 1
+    assert departure_timer.start_time == datetime.time(7, 35)
+    assert departure_timer.action == "DEACTIVATE"
+    assert departure_timer.weekdays == ["MONDAY", "TUESDAY", "WEDNESDAY", "THURSDAY", "FRIDAY"]
 
-    assert CheckControlStatus.MEDIUM == ccms[0].state
-    assert (
-        "Charge by driving for longer periods or use external charger. "
-        "Functions requiring battery will be switched off."
-    ) == ccms[0].description_long
-
-    assert "Battery discharged: Start engine" == ccms[0].description_short
-
-    assert CheckControlStatus.LOW == ccms[1].state
-    assert (
-        "System unable to monitor tire pressure. Check tire pressures manually. "
-        "Continued driving possible. Consult service center."
-    ) == ccms[1].description_long
+    assert charging_profile.departure_times[3].start_time is None
 
-    assert "Flat Tire Monitor (FTM) inactive" == ccms[1].description_short
+    charging_window = charging_profile.preferred_charging_window
+    assert charging_window.start_time == datetime.time(18, 1)
+    assert charging_window.end_time == datetime.time(1, 30)
 
     assert len(get_deprecation_warning_count(caplog)) == 0
```

