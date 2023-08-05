# Comparing `tmp/pkscreener-0.4.20230805.15.tar.gz` & `tmp/pkscreener-0.4.20230805.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkscreener-0.4.20230805.15.tar", last modified: Sat Aug  5 01:08:02 2023, max compression
+gzip compressed data, was "pkscreener-0.4.20230805.16.tar", last modified: Sat Aug  5 01:53:51 2023, max compression
```

## Comparing `pkscreener-0.4.20230805.15.tar` & `pkscreener-0.4.20230805.16.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:02.663079 pkscreener-0.4.20230805.15/
--rw-rw-rw-   0        0        0     1086 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/LICENSE
--rw-rw-rw-   0        0        0     1091 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/LICENSE-Screenipy
--rw-rw-rw-   0        0        0    21320 2023-08-05 01:08:02.663079 pkscreener-0.4.20230805.15/PKG-INFO
--rw-rw-rw-   0        0        0    20419 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/README.md
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:02.647540 pkscreener-0.4.20230805.15/pkscreener/
--rw-rw-rw-   0        0        0     8992 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/Telegram.py
--rw-rw-rw-   0        0        0      404 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:02.663079 pkscreener-0.4.20230805.15/pkscreener/classes/
--rw-rw-rw-   0        0        0     1014 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Archiver.py
--rw-rw-rw-   0        0        0     3470 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Backtest.py
--rw-rw-rw-   0        0        0    10065 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/CandlePatterns.py
--rw-rw-rw-   0        0        0      473 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Changelog.py
--rw-rw-rw-   0        0        0      391 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/ColorText.py
--rw-rw-rw-   0        0        0    11723 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/ConfigManager.py
--rw-rw-rw-   0        0        0     9348 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Fetcher.py
--rw-rw-rw-   0        0        0    14101 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/MenuOptions.py
--rw-rw-rw-   0        0        0     6368 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/OtaUpdater.py
--rw-rw-rw-   0        0        0    23216 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/ParallelProcessing.py
--rw-rw-rw-   0        0        0    11684 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Pktalib.py
--rw-rw-rw-   0        0        0     4796 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/PortfolioTracker.py
--rw-rw-rw-   0        0        0    49373 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Screener.py
--rw-rw-rw-   0        0        0      947 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/SuppressOutput.py
--rw-rw-rw-   0        0        0      649 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/UserChoice.py
--rw-rw-rw-   0        0        0    30737 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/Utility.py
--rw-rw-rw-   0        0        0       26 2023-08-05 01:07:56.000000 pkscreener-0.4.20230805.15/pkscreener/classes/__init__.py
--rw-rw-rw-   0        0        0    11228 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/log.py
--rw-rw-rw-   0        0        0     4038 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/classes/multiprocessing_logging.py
--rw-rw-rw-   0        0        0    45776 2023-08-05 01:04:36.000000 pkscreener-0.4.20230805.15/pkscreener/globals.py
--rw-rw-rw-   0        0        0    27552 2023-08-05 01:04:37.000000 pkscreener-0.4.20230805.15/pkscreener/pkscreenerbot.py
--rw-rw-rw-   0        0        0     7755 2023-08-05 01:04:37.000000 pkscreener-0.4.20230805.15/pkscreener/pkscreenercli.py
-drwxrwxrwx   0        0        0        0 2023-08-05 01:08:02.647540 pkscreener-0.4.20230805.15/pkscreener.egg-info/
--rw-rw-rw-   0        0        0    21320 2023-08-05 01:08:02.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1057 2023-08-05 01:08:02.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 01:08:02.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-08-05 01:08:02.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-08-05 01:07:58.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      585 2023-08-05 01:08:02.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-08-05 01:08:02.000000 pkscreener-0.4.20230805.15/pkscreener.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-08-05 01:08:02.663079 pkscreener-0.4.20230805.15/setup.cfg
--rw-rw-rw-   0        0        0     2583 2023-08-05 01:04:37.000000 pkscreener-0.4.20230805.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:53:51.629811 pkscreener-0.4.20230805.16/
+-rw-rw-rw-   0        0        0     1086 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/LICENSE
+-rw-rw-rw-   0        0        0     1091 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/LICENSE-Screenipy
+-rw-rw-rw-   0        0        0    21320 2023-08-05 01:53:51.629811 pkscreener-0.4.20230805.16/PKG-INFO
+-rw-rw-rw-   0        0        0    20419 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/README.md
+drwxrwxrwx   0        0        0        0 2023-08-05 01:53:51.614187 pkscreener-0.4.20230805.16/pkscreener/
+-rw-rw-rw-   0        0        0     8992 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/Telegram.py
+-rw-rw-rw-   0        0        0      404 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:53:51.629811 pkscreener-0.4.20230805.16/pkscreener/classes/
+-rw-rw-rw-   0        0        0     1014 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Archiver.py
+-rw-rw-rw-   0        0        0     3470 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Backtest.py
+-rw-rw-rw-   0        0        0    10065 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/CandlePatterns.py
+-rw-rw-rw-   0        0        0      473 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Changelog.py
+-rw-rw-rw-   0        0        0      391 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/ColorText.py
+-rw-rw-rw-   0        0        0    11723 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/ConfigManager.py
+-rw-rw-rw-   0        0        0     9348 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Fetcher.py
+-rw-rw-rw-   0        0        0    14101 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/MenuOptions.py
+-rw-rw-rw-   0        0        0     6368 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/OtaUpdater.py
+-rw-rw-rw-   0        0        0    23216 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/ParallelProcessing.py
+-rw-rw-rw-   0        0        0    11684 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Pktalib.py
+-rw-rw-rw-   0        0        0     4796 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/PortfolioTracker.py
+-rw-rw-rw-   0        0        0    49373 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Screener.py
+-rw-rw-rw-   0        0        0      947 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/SuppressOutput.py
+-rw-rw-rw-   0        0        0      649 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/UserChoice.py
+-rw-rw-rw-   0        0        0    30737 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/Utility.py
+-rw-rw-rw-   0        0        0       26 2023-08-05 01:53:45.000000 pkscreener-0.4.20230805.16/pkscreener/classes/__init__.py
+-rw-rw-rw-   0        0        0    11228 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/log.py
+-rw-rw-rw-   0        0        0     4038 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/classes/multiprocessing_logging.py
+-rw-rw-rw-   0        0        0    45776 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/globals.py
+-rw-rw-rw-   0        0        0    27552 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/pkscreenerbot.py
+-rw-rw-rw-   0        0        0     7755 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/pkscreener/pkscreenercli.py
+drwxrwxrwx   0        0        0        0 2023-08-05 01:53:51.614187 pkscreener-0.4.20230805.16/pkscreener.egg-info/
+-rw-rw-rw-   0        0        0    21320 2023-08-05 01:53:51.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1057 2023-08-05 01:53:51.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 01:53:51.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-08-05 01:53:51.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-08-05 01:53:47.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      585 2023-08-05 01:53:51.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-08-05 01:53:51.000000 pkscreener-0.4.20230805.16/pkscreener.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-08-05 01:53:51.629811 pkscreener-0.4.20230805.16/setup.cfg
+-rw-rw-rw-   0        0        0     2583 2023-08-05 01:49:44.000000 pkscreener-0.4.20230805.16/setup.py
```

### Comparing `pkscreener-0.4.20230805.15/LICENSE` & `pkscreener-0.4.20230805.16/LICENSE`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/LICENSE-Screenipy` & `pkscreener-0.4.20230805.16/LICENSE-Screenipy`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/PKG-INFO` & `pkscreener-0.4.20230805.16/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.4.20230805.15
+Version: 0.4.20230805.16
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.4.20230805.15.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.4.20230805.16.zip
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-Screenipy
 
 
 # PKScreener
 
-[![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
+[![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/pkjmesra/pkscreener/workflow-prod-scans_2.1.yml?logo=github)
 ![github license](https://img.shields.io/pypi/l/gspread?logo=github) [![Downloads](https://static.pepy.tech/personalized-badge/pkscreener?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/pkscreener)
 ![latest download](https://img.shields.io/github/downloads-pre/pkjmesra/pkscreener/latest/total?logo=github)
 [![Documentation](https://readthedocs.org/projects/pkscreener/badge/?version=latest)](https://pkscreener.readthedocs.io/en/latest/?badge=latest) [![Docker Status](https://img.shields.io/docker/automated/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian)
 [![Docker Pulls](https://img.shields.io/docker/pulls/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian) [![3. Production Scan Tests On Dev](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml) [![4. After-Market Data Gen](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml) 
  [![PKScreener Test - New Features](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml/badge.svg?branch=new-features)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml) [![PKScreener Build - New Release](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml)
```

### Comparing `pkscreener-0.4.20230805.15/README.md` & `pkscreener-0.4.20230805.16/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 # PKScreener
 
-[![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
+[![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/pkjmesra/pkscreener/workflow-prod-scans_2.1.yml?logo=github)
 ![github license](https://img.shields.io/pypi/l/gspread?logo=github) [![Downloads](https://static.pepy.tech/personalized-badge/pkscreener?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/pkscreener)
 ![latest download](https://img.shields.io/github/downloads-pre/pkjmesra/pkscreener/latest/total?logo=github)
 [![Documentation](https://readthedocs.org/projects/pkscreener/badge/?version=latest)](https://pkscreener.readthedocs.io/en/latest/?badge=latest) [![Docker Status](https://img.shields.io/docker/automated/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian)
 [![Docker Pulls](https://img.shields.io/docker/pulls/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian) [![3. Production Scan Tests On Dev](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml) [![4. After-Market Data Gen](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml) 
  [![PKScreener Test - New Features](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml/badge.svg?branch=new-features)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml) [![PKScreener Build - New Release](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml)
```

### Comparing `pkscreener-0.4.20230805.15/pkscreener/Telegram.py` & `pkscreener-0.4.20230805.16/pkscreener/Telegram.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/Archiver.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/Archiver.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/Backtest.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/Backtest.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/CandlePatterns.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/CandlePatterns.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/ConfigManager.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/ConfigManager.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/Fetcher.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/Fetcher.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/MenuOptions.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/MenuOptions.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/OtaUpdater.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/OtaUpdater.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/ParallelProcessing.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/ParallelProcessing.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/Pktalib.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/Pktalib.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/PortfolioTracker.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/PortfolioTracker.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/Screener.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/Screener.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/SuppressOutput.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/SuppressOutput.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/UserChoice.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/UserChoice.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/Utility.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/Utility.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/log.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/log.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/classes/multiprocessing_logging.py` & `pkscreener-0.4.20230805.16/pkscreener/classes/multiprocessing_logging.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/globals.py` & `pkscreener-0.4.20230805.16/pkscreener/globals.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/pkscreenerbot.py` & `pkscreener-0.4.20230805.16/pkscreener/pkscreenerbot.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener/pkscreenercli.py` & `pkscreener-0.4.20230805.16/pkscreener/pkscreenercli.py`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener.egg-info/PKG-INFO` & `pkscreener-0.4.20230805.16/pkscreener.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pkscreener
-Version: 0.4.20230805.15
+Version: 0.4.20230805.16
 Summary: A Python-based stock screener for NSE, India with alerts to Telegram Channel (pkscreener)
 Home-page: https://github.com/pkjmesra/pkscreener
 Author: pkjmesra
 Author-email: pkjmesra@gmail.com
 License: OSI Approved (MIT)
-Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.4.20230805.15.zip
+Download-URL: https://github.com/pkjmesra/pkscreener/archive/v0.4.20230805.16.zip
 Keywords: NSE,Technical Indicators,Scanning,Stock Scanners
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
@@ -19,15 +19,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: LICENSE-Screenipy
 
 
 # PKScreener
 
-[![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.2/pkscreenercli.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
+[![MADE-IN-INDIA](https://img.shields.io/badge/MADE%20WITH%20%E2%9D%A4%20IN-INDIA-orange?style=for-the-badge)](https://en.wikipedia.org/wiki/India) [![Windows](https://img.shields.io/badge/Windows-0078D6?style=for-the-badge&logo=windows&logoColor=white)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.exe) [![Linux](https://img.shields.io/badge/Linux-FCC624?style=for-the-badge&logo=linux&logoColor=black)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.bin) [![Mac OS](https://img.shields.io/badge/mac%20os-D3D3D3?style=for-the-badge&logo=apple&logoColor=000000)](https://github.com/pkjmesra/PKScreener/releases/download/0.4/pkscreenercli.run) [![GitHub release (latest by date)](https://img.shields.io/github/v/release/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/releases/latest) [![GitHub all releases](https://img.shields.io/github/downloads/pkjmesra/PKScreener/total?color=Green&label=Downloads&style=for-the-badge)](#) [![GitHub](https://img.shields.io/github/license/pkjmesra/PKScreener?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/main/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/pkjmesra/PKScreener/badge?style=for-the-badge)](https://www.codefactor.io/repository/github/pkjmesra/PKScreener) [![BADGE](https://img.shields.io/badge/PULL%20REQUEST-GUIDELINES-red?style=for-the-badge)](https://github.com/pkjmesra/PKScreener/blob/new-features/CONTRIBUTING.md)
 
 ![main workflow](https://img.shields.io/github/actions/workflow/status/pkjmesra/pkscreener/workflow-prod-scans_2.1.yml?logo=github)
 ![github license](https://img.shields.io/pypi/l/gspread?logo=github) [![Downloads](https://static.pepy.tech/personalized-badge/pkscreener?period=total&units=international_system&left_color=black&right_color=brightgreen&left_text=PyPi%20Downloads)](https://pepy.tech/project/pkscreener)
 ![latest download](https://img.shields.io/github/downloads-pre/pkjmesra/pkscreener/latest/total?logo=github)
 [![Documentation](https://readthedocs.org/projects/pkscreener/badge/?version=latest)](https://pkscreener.readthedocs.io/en/latest/?badge=latest) [![Docker Status](https://img.shields.io/docker/automated/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian)
 [![Docker Pulls](https://img.shields.io/docker/pulls/pkjmesra/pkscreener-debian.svg)](https://hub.docker.com/repository/docker/pkjmesra/pkscreener-debian) [![3. Production Scan Tests On Dev](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-prod-scans_Tests.yml) [![4. After-Market Data Gen](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-download-data.yml) 
  [![PKScreener Test - New Features](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml/badge.svg?branch=new-features)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-test.yml) [![PKScreener Build - New Release](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml/badge.svg)](https://github.com/pkjmesra/PKScreener/actions/workflows/workflow-build-matrix.yml)
```

### Comparing `pkscreener-0.4.20230805.15/pkscreener.egg-info/SOURCES.txt` & `pkscreener-0.4.20230805.16/pkscreener.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/pkscreener.egg-info/requires.txt` & `pkscreener-0.4.20230805.16/pkscreener.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pkscreener-0.4.20230805.15/setup.py` & `pkscreener-0.4.20230805.16/setup.py`

 * *Files identical despite different names*

