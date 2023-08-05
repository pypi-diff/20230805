# Comparing `tmp/sats_receiver-0.1.19.tar.gz` & `tmp/sats_receiver-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sats_receiver-0.1.19.tar", last modified: Wed May 31 20:26:30 2023, max compression
+gzip compressed data, was "sats_receiver-0.1.76.tar", last modified: Sat Aug  5 11:30:50 2023, max compression
```

## Comparing `sats_receiver-0.1.19.tar` & `sats_receiver-0.1.76.tar`

### file list

```diff
@@ -1,40 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14787 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2250 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/async_signal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/gr_modules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2490 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/demodulators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/prober.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/epb/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    11719 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/gr_modules/receiver.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/librtlsdr.py
--rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/observer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver/systems/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/systems/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16969 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/systems/apt.py
--rw-r--r--   0 runner    (1001) docker     (123)    16710 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/systems/sstv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/tle.py
--rw-r--r--   0 runner    (1001) docker     (123)    10774 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/sats_receiver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/sats_receiver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15367 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-31 20:26:30.000000 sats_receiver-0.1.19/sats_receiver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:30.700879 sats_receiver-0.1.19/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/test_async_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6509 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/test_decoders.py
--rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-05-31 20:26:18.000000 sats_receiver-0.1.19/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16931 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.283702 sats_receiver-0.1.76/sats_receiver/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2380 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1631 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/async_signal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.283702 sats_receiver-0.1.76/sats_receiver/gr_modules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20095 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4310 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/demodulators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.283702 sats_receiver-0.1.76/sats_receiver/gr_modules/epb/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/epb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/epb/prober.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/epb/sstv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15363 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12001 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/gr_modules/receiver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/librtlsdr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9517 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6515 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/observer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.283702 sats_receiver-0.1.76/sats_receiver/systems/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20357 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/apt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/sats_receiver/systems/satellites/
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/sats_receiver/systems/satellites/demodulators/
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/demodulators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/sats_receiver/systems/satellites/filereceivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/filereceivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4232 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/filereceivers/geoscan.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/sats_receiver/systems/satellites/telemetry/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/telemetry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/telemetry/geoscan_tlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/satellites/telemetry/usp_tlm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/systems/sstv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/tle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10824 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/sats_receiver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.283702 sats_receiver-0.1.76/sats_receiver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17511 2023-08-05 11:30:50.000000 sats_receiver-0.1.76/sats_receiver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-08-05 11:30:50.000000 sats_receiver-0.1.76/sats_receiver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-05 11:30:50.000000 sats_receiver-0.1.76/sats_receiver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-05 11:30:50.000000 sats_receiver-0.1.76/sats_receiver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-08-05 11:30:50.000000 sats_receiver-0.1.76/sats_receiver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:50.287702 sats_receiver-0.1.76/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/tests/test_async_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14387 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/tests/test_decoders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/tests/test_demodulators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13099 2023-08-05 11:30:37.000000 sats_receiver-0.1.76/tests/test_utils.py
```

### Comparing `sats_receiver-0.1.19/LICENSE` & `sats_receiver-0.1.76/LICENSE`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.19/PKG-INFO` & `sats_receiver-0.1.76/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: sats_receiver
-Version: 0.1.19
-Summary: Satellites data receiver based on GNU Radio
-Home-page: https://github.com/baskiton/sats-receiver
-Author: Alexander Baskikh
-Author-email: baskiton@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Communications :: Ham Radio
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Sats Receiver
 [![PyPI](https://img.shields.io/pypi/v/sats-receiver?logo=python&logoColor=white)][pypi_proj]
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/sats-receiver?logo=python&logoColor=white)][pypi_proj]
 [![PyPI - License](https://img.shields.io/pypi/l/sats-receiver?logo=open-source-initiative&logoColor=white)][license]  
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/tests.yml?label=tests&logo=github)][tests]
 [![Codecov branch](https://img.shields.io/codecov/c/gh/baskiton/sats-receiver/dev?logo=codecov)][codecov]
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/pypi-upload.yml?label=upload&logo=github)][upload]
@@ -31,25 +14,26 @@
 
 Satellites data receiver based on GNURadio
 
 <!-- TOC -->
 * [About](#About)
 * [Requirements](#Requirements)
 * [Installation](#Installation)
-  * [Linux](#Linux)
-  * [Windows](#Windows)
+  * [From source](#From-source)
+  * [From PYPI](#From-PYPI)
 * [Usage](#Usage)
 * [Configure](#Configure)
   * [observer](#observer)
   * [tle](#tle)
   * [receivers](#receivers)
     * [sats](#sats)
       * [frequencies](#frequencies)
         * [modulations](#modulations)
         * [decoders](#decoders)
+          * [gr-satellites](#gr-satellites)
 * [Map Shapes](#Map-Shapes)
   * [shapes](#shapes)
   * [points](#points)
 <!-- TOC -->
 
 
 
@@ -69,36 +53,41 @@
 ### Requirements
 The program has only been tested on Linux. Work on Windows is not guaranteed!
 * Python>=3.10 (or lower, see below)
 * GNURadio>=3.10 (or lower if gr-soapy installed); GUI-modules is not required
 * librtlsdr (if you use RTL-SDR)
 
 ### Installation
-First [install gnuradio](https://wiki.gnuradio.org/index.php?title=InstallingGR)
+I recommended to use miniconda. So, first of all,
+[install it.](https://docs.conda.io/en/latest/miniconda.html#linux-installers)
 
-#### Linux
-  If you need a virtual environment (recommended), you need to create it
-  with the `--system-site-packages` option
-  ```
-  python3 -m venv --system-site-packages venv
-  source venv/bin/activate
-  pip install sats-receiver
-  ```
-
-#### Windows
-  After install `radioconda`, launch a terminal by running "Conda Prompt"
-  in the "radioconda" directory in the Start menu and type
-  ```
-  pip install sats-receiver
-  ```
+#### From source
+```commandline
+cd sats-receiver
+conda create -n sats-receiver-env
+conda activate sats-receiver-env
+conda config --env --add channels conda-forge
+conda config --env --set channel_priority strict
+conda env update -f environment.yml
+pip install -r requirements.txt
+```
+
+#### From PYPI
+```commandline
+conda create -n sats-receiver-env python
+conda activate sats-receiver-env
+conda config --env --add channels conda-forge
+conda config --env --set channel_priority strict
+conda install gnuradio gnuradio-satellites
+pip install sats-receiver
+```
 
 ### Usage
-* in Linux if a virtual environment has been created:  
-  `source venv/bin/activate`
-* in Windows launch "Conda Prompt" terminal
+First, activate conda environment:  
+`conda activate sats-receiver-env`
 
 `python -u -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
 * `config` Config file path. See [Configure](#Configure)
 * `-h, --help` Help message
 * `--log LOG` Logging level, INFO default
 * `--sysu SYSU` System Usages debug info timeout in seconds, 1 hour default
 
@@ -152,14 +141,15 @@
 | samp_rate        | Number          | Receiver sample rate, Hz                                                                                                                                                           |
 | output_directory | String          | Directory to save received files. You also might specify `~` symbol to specify User home directory                                                                                 |
 | sats             | Array of Object | List of Satellites configurations (see [sats](#sats))                                                                                                                              |
 | enabled          | Boolean         | _Optional._ Enable or Disable this Receiver. `true` by default                                                                                                                     |
 | serial           | String          | _Optional._ Serial number of the receiver. Empty by default                                                                                                                        |
 | biast            | Boolean         | _Optional._ Bias-T enable/disable (only for RTL-SDR at this time). `false` by default. **WARNING! Be careful when enabling this option! Use only if you know what it is and why!** |
 | gain             | Boolean         | _Optional._ Receiver gain, dB. `0` by default                                                                                                                                      |
+| freq_correction  | Number          | _Optional._ Receiver frequency correction. `0.0` by default                                                                                                                        |
 
 
 #### sats
 Each satellite object contain:
 
 | Field         | Type            | Description                                                                                                |
 |:--------------|:----------------|:-----------------------------------------------------------------------------------------------------------|
@@ -169,60 +159,75 @@
 | min_elevation | Number          | _Optional._ Elevation angle above the horizon, degrees. `0` by default. Negative number is equivalent to 0 |
 | doppler       | Boolean         | _Optional._ Enable/Disable doppler correction. `true` by default                                           |
 
 
 #### frequencies
 Each frequency object contain:
 
-| Field           | Type    | Description                                                                       |
-|:----------------|:--------|:----------------------------------------------------------------------------------|
-| freq            | Number  | Basic signal frequency, Hz                                                        |
-| bandwidth       | Number  | Received signal bandwidth, Hz                                                     |
-| enabled         | Boolean | _Optional._ Enable/Disable this frequency. `true` by default                      |
-| freq_correction | Boolean | _Optional._ Correction for basic frequency, Hz. `0` by default                    |
-| mode            | String  | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default |
-| decode          | String  | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default          |
-| qpsk_baudrate   | Number  | _Required only for **QPSK** mode._ QPSK Baudrate, bps                             |
-| qpsk_excess_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Excess bandwidth. `0.35` by default      |
-| qpsk_ntaps      | Integer | _Optional. Only for **QPSK** mode._ QPSK number of taps. `33` by default          |
-| qpsk_costas_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Costas bandwidth. `0.005` by default     |
-| sstv_wsr        | Number  | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default   |
-| sstv_sync       | Number  | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default            |
+| Field           | Type            | Description                                                                            |
+|:----------------|:----------------|:---------------------------------------------------------------------------------------|
+| freq            | Number          | Basic signal frequency, Hz                                                             |
+| bandwidth       | Number          | Received signal bandwidth, Hz                                                          |
+| enabled         | Boolean         | _Optional._ Enable/Disable this frequency. `true` by default                           |
+| subname         | String          | _Optional._ Subname added to result filename. Empty by default                         |
+| freq_correction | Boolean         | _Optional._ Correction for basic frequency, Hz. `0` by default                         |
+| mode            | String          | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default      |
+| decode          | String          | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default               |
+| channels        | Array of Number | _Required only for **GMSK** mode._ Demodulation baudrates, bps                         |
+| grs_file        | String          | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_name        | String          | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_norad       | Integer         | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_tlm_decode  | Boolean         | _Optional. Only for **SATS** decoder._ Save decoded telemetry. `true` by default       |
+| qpsk_baudrate   | Number          | _Required only for **(O)QPSK** mode._ (O)QPSK Baudrate, bps                            |
+| qpsk_excess_bw  | Number          | _Optional. Only for **(O)QPSK** mode._ (O)QPSK Excess bandwidth. `0.35` by default     |
+| qpsk_ntaps      | Integer         | _Optional. Only for **(O)QPSK** mode._ (O)QPSK number of taps. `33` by default         |
+| qpsk_costas_bw  | Number          | _Optional. Only for **(O)QPSK** mode._ (O)QPSK Costas bandwidth. `0.005` by default    |
+| sstv_wsr        | Number          | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default        |
+| sstv_sync       | Number          | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default                 |
 
 
 #### modulations
 * `RAW`
 * `AM`
 * `FM`
 * `WFM`
 * `WFM_STEREO`
 * `QUAD`
 * `QPSK`
+* `OQPSK`
+* `GMSK`
 
 #### decoders
 * `RAW` Saved to 2-channel float32 WAV file with `bandwidth` sample rate
-* `RSTREAM` Raw Stream - binary int8. Suitable for further processing, for example, in SatDump
-* `APT` sats-receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
+* `CSOFT` Constellation Soft Decoder - 1-channel binary int8. Suitable for further processing, for example, in SatDump
+* `APT` Sats-Receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
 * `SSTV` SSTV saved to PNG image with EXIF. Supported modes:
-  * `Robot24`
-  * `Robot36`
-  * `Robot72`
-  * `MartinM1`
-  * `MartinM2`
-  * `MartinM3`
-  * `MartinM4`
-  * `PD50`
-  * `PD90`
-  * `PD120`
-  * `PD160`
-  * `PD180`
-  * `PD240`
-  * `PD290`
+  * Robot (24, 24, 72)
+  * Martin (M1, M2, M3, M4)
+  * PD (50, 90, 120, 160, 180, 240, 290)
+  * Scottie (S1, S2, S3, S4)
+* `SATS` See [gr-satellites](#gr-satellites) for details
 * ~~`LRPT`~~ Not implemented yet
 
+##### gr-satellites
+See [gr-satellites Documentation][grs-doc]  
+**IMPORTANT:** For this decoder need to leave the `modulation` on `RAW`  
+
+This decoder need to specify one of the parameters for recognize satellite option:
+* grs_file - Path to your own [SatYAML-file][grs-satyaml]
+* grs_name - Satellite name (may different from [sats name](#sats))
+* grs_norad - Satellite NORAD ID
+
+[List of builtin supported satellites][grs-satlist]  
+Additionally supported satellites can be found in the [satyaml](satyaml) directory of this repository
+
+[grs-doc]: https://gr-satellites.readthedocs.io/en/latest/
+[grs-satyaml]: https://gr-satellites.readthedocs.io/en/latest/satyaml.html
+[grs-satlist]: https://gr-satellites.readthedocs.io/en/latest/supported_satellites.html
+
 
 ### Map Shapes
 Map shapes config file `map_shapes.json` can be found at the root of this repository.
 Shapefiles can be downloaded from [Natural Earth](https://www.naturalearthdata.com/downloads/)
 
 | Field      | Type             | Description                                                                        |
 |:-----------|:-----------------|:-----------------------------------------------------------------------------------|
```

### Comparing `sats_receiver-0.1.19/README.md` & `sats_receiver-0.1.76/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: sats_receiver
+Version: 0.1.76
+Summary: Satellites data receiver based on GNU Radio
+Home-page: https://github.com/baskiton/sats-receiver
+Author: Alexander Baskikh
+Author-email: baskiton@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: Topic :: Communications :: Ham Radio
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Sats Receiver
 [![PyPI](https://img.shields.io/pypi/v/sats-receiver?logo=python&logoColor=white)][pypi_proj]
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/sats-receiver?logo=python&logoColor=white)][pypi_proj]
 [![PyPI - License](https://img.shields.io/pypi/l/sats-receiver?logo=open-source-initiative&logoColor=white)][license]  
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/tests.yml?label=tests&logo=github)][tests]
 [![Codecov branch](https://img.shields.io/codecov/c/gh/baskiton/sats-receiver/dev?logo=codecov)][codecov]
 [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/baskiton/sats-receiver/pypi-upload.yml?label=upload&logo=github)][upload]
@@ -14,25 +31,26 @@
 
 Satellites data receiver based on GNURadio
 
 <!-- TOC -->
 * [About](#About)
 * [Requirements](#Requirements)
 * [Installation](#Installation)
-  * [Linux](#Linux)
-  * [Windows](#Windows)
+  * [From source](#From-source)
+  * [From PYPI](#From-PYPI)
 * [Usage](#Usage)
 * [Configure](#Configure)
   * [observer](#observer)
   * [tle](#tle)
   * [receivers](#receivers)
     * [sats](#sats)
       * [frequencies](#frequencies)
         * [modulations](#modulations)
         * [decoders](#decoders)
+          * [gr-satellites](#gr-satellites)
 * [Map Shapes](#Map-Shapes)
   * [shapes](#shapes)
   * [points](#points)
 <!-- TOC -->
 
 
 
@@ -52,36 +70,41 @@
 ### Requirements
 The program has only been tested on Linux. Work on Windows is not guaranteed!
 * Python>=3.10 (or lower, see below)
 * GNURadio>=3.10 (or lower if gr-soapy installed); GUI-modules is not required
 * librtlsdr (if you use RTL-SDR)
 
 ### Installation
-First [install gnuradio](https://wiki.gnuradio.org/index.php?title=InstallingGR)
+I recommended to use miniconda. So, first of all,
+[install it.](https://docs.conda.io/en/latest/miniconda.html#linux-installers)
 
-#### Linux
-  If you need a virtual environment (recommended), you need to create it
-  with the `--system-site-packages` option
-  ```
-  python3 -m venv --system-site-packages venv
-  source venv/bin/activate
-  pip install sats-receiver
-  ```
-
-#### Windows
-  After install `radioconda`, launch a terminal by running "Conda Prompt"
-  in the "radioconda" directory in the Start menu and type
-  ```
-  pip install sats-receiver
-  ```
+#### From source
+```commandline
+cd sats-receiver
+conda create -n sats-receiver-env
+conda activate sats-receiver-env
+conda config --env --add channels conda-forge
+conda config --env --set channel_priority strict
+conda env update -f environment.yml
+pip install -r requirements.txt
+```
+
+#### From PYPI
+```commandline
+conda create -n sats-receiver-env python
+conda activate sats-receiver-env
+conda config --env --add channels conda-forge
+conda config --env --set channel_priority strict
+conda install gnuradio gnuradio-satellites
+pip install sats-receiver
+```
 
 ### Usage
-* in Linux if a virtual environment has been created:  
-  `source venv/bin/activate`
-* in Windows launch "Conda Prompt" terminal
+First, activate conda environment:  
+`conda activate sats-receiver-env`
 
 `python -u -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
 * `config` Config file path. See [Configure](#Configure)
 * `-h, --help` Help message
 * `--log LOG` Logging level, INFO default
 * `--sysu SYSU` System Usages debug info timeout in seconds, 1 hour default
 
@@ -135,14 +158,15 @@
 | samp_rate        | Number          | Receiver sample rate, Hz                                                                                                                                                           |
 | output_directory | String          | Directory to save received files. You also might specify `~` symbol to specify User home directory                                                                                 |
 | sats             | Array of Object | List of Satellites configurations (see [sats](#sats))                                                                                                                              |
 | enabled          | Boolean         | _Optional._ Enable or Disable this Receiver. `true` by default                                                                                                                     |
 | serial           | String          | _Optional._ Serial number of the receiver. Empty by default                                                                                                                        |
 | biast            | Boolean         | _Optional._ Bias-T enable/disable (only for RTL-SDR at this time). `false` by default. **WARNING! Be careful when enabling this option! Use only if you know what it is and why!** |
 | gain             | Boolean         | _Optional._ Receiver gain, dB. `0` by default                                                                                                                                      |
+| freq_correction  | Number          | _Optional._ Receiver frequency correction. `0.0` by default                                                                                                                        |
 
 
 #### sats
 Each satellite object contain:
 
 | Field         | Type            | Description                                                                                                |
 |:--------------|:----------------|:-----------------------------------------------------------------------------------------------------------|
@@ -152,60 +176,75 @@
 | min_elevation | Number          | _Optional._ Elevation angle above the horizon, degrees. `0` by default. Negative number is equivalent to 0 |
 | doppler       | Boolean         | _Optional._ Enable/Disable doppler correction. `true` by default                                           |
 
 
 #### frequencies
 Each frequency object contain:
 
-| Field           | Type    | Description                                                                       |
-|:----------------|:--------|:----------------------------------------------------------------------------------|
-| freq            | Number  | Basic signal frequency, Hz                                                        |
-| bandwidth       | Number  | Received signal bandwidth, Hz                                                     |
-| enabled         | Boolean | _Optional._ Enable/Disable this frequency. `true` by default                      |
-| freq_correction | Boolean | _Optional._ Correction for basic frequency, Hz. `0` by default                    |
-| mode            | String  | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default |
-| decode          | String  | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default          |
-| qpsk_baudrate   | Number  | _Required only for **QPSK** mode._ QPSK Baudrate, bps                             |
-| qpsk_excess_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Excess bandwidth. `0.35` by default      |
-| qpsk_ntaps      | Integer | _Optional. Only for **QPSK** mode._ QPSK number of taps. `33` by default          |
-| qpsk_costas_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Costas bandwidth. `0.005` by default     |
-| sstv_wsr        | Number  | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default   |
-| sstv_sync       | Number  | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default            |
+| Field           | Type            | Description                                                                            |
+|:----------------|:----------------|:---------------------------------------------------------------------------------------|
+| freq            | Number          | Basic signal frequency, Hz                                                             |
+| bandwidth       | Number          | Received signal bandwidth, Hz                                                          |
+| enabled         | Boolean         | _Optional._ Enable/Disable this frequency. `true` by default                           |
+| subname         | String          | _Optional._ Subname added to result filename. Empty by default                         |
+| freq_correction | Boolean         | _Optional._ Correction for basic frequency, Hz. `0` by default                         |
+| mode            | String          | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default      |
+| decode          | String          | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default               |
+| channels        | Array of Number | _Required only for **GMSK** mode._ Demodulation baudrates, bps                         |
+| grs_file        | String          | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_name        | String          | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_norad       | Integer         | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_tlm_decode  | Boolean         | _Optional. Only for **SATS** decoder._ Save decoded telemetry. `true` by default       |
+| qpsk_baudrate   | Number          | _Required only for **(O)QPSK** mode._ (O)QPSK Baudrate, bps                            |
+| qpsk_excess_bw  | Number          | _Optional. Only for **(O)QPSK** mode._ (O)QPSK Excess bandwidth. `0.35` by default     |
+| qpsk_ntaps      | Integer         | _Optional. Only for **(O)QPSK** mode._ (O)QPSK number of taps. `33` by default         |
+| qpsk_costas_bw  | Number          | _Optional. Only for **(O)QPSK** mode._ (O)QPSK Costas bandwidth. `0.005` by default    |
+| sstv_wsr        | Number          | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default        |
+| sstv_sync       | Number          | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default                 |
 
 
 #### modulations
 * `RAW`
 * `AM`
 * `FM`
 * `WFM`
 * `WFM_STEREO`
 * `QUAD`
 * `QPSK`
+* `OQPSK`
+* `GMSK`
 
 #### decoders
 * `RAW` Saved to 2-channel float32 WAV file with `bandwidth` sample rate
-* `RSTREAM` Raw Stream - binary int8. Suitable for further processing, for example, in SatDump
-* `APT` sats-receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
+* `CSOFT` Constellation Soft Decoder - 1-channel binary int8. Suitable for further processing, for example, in SatDump
+* `APT` Sats-Receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
 * `SSTV` SSTV saved to PNG image with EXIF. Supported modes:
-  * `Robot24`
-  * `Robot36`
-  * `Robot72`
-  * `MartinM1`
-  * `MartinM2`
-  * `MartinM3`
-  * `MartinM4`
-  * `PD50`
-  * `PD90`
-  * `PD120`
-  * `PD160`
-  * `PD180`
-  * `PD240`
-  * `PD290`
+  * Robot (24, 24, 72)
+  * Martin (M1, M2, M3, M4)
+  * PD (50, 90, 120, 160, 180, 240, 290)
+  * Scottie (S1, S2, S3, S4)
+* `SATS` See [gr-satellites](#gr-satellites) for details
 * ~~`LRPT`~~ Not implemented yet
 
+##### gr-satellites
+See [gr-satellites Documentation][grs-doc]  
+**IMPORTANT:** For this decoder need to leave the `modulation` on `RAW`  
+
+This decoder need to specify one of the parameters for recognize satellite option:
+* grs_file - Path to your own [SatYAML-file][grs-satyaml]
+* grs_name - Satellite name (may different from [sats name](#sats))
+* grs_norad - Satellite NORAD ID
+
+[List of builtin supported satellites][grs-satlist]  
+Additionally supported satellites can be found in the [satyaml](satyaml) directory of this repository
+
+[grs-doc]: https://gr-satellites.readthedocs.io/en/latest/
+[grs-satyaml]: https://gr-satellites.readthedocs.io/en/latest/satyaml.html
+[grs-satlist]: https://gr-satellites.readthedocs.io/en/latest/supported_satellites.html
+
 
 ### Map Shapes
 Map shapes config file `map_shapes.json` can be found at the root of this repository.
 Shapefiles can be downloaded from [Natural Earth](https://www.naturalearthdata.com/downloads/)
 
 | Field      | Type             | Description                                                                        |
 |:-----------|:-----------------|:-----------------------------------------------------------------------------------|
```

### Comparing `sats_receiver-0.1.19/sats_receiver/__main__.py` & `sats_receiver-0.1.76/sats_receiver/__main__.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import argparse
 import atexit
 import logging
 import logging.handlers
 import multiprocessing as mp
 import pathlib
 
+import gnuradio as gr
+import gnuradio.gr
+
 from sats_receiver import HOMEDIR, LOGSDIR, TLEDIR, RECDIR
 from sats_receiver.async_signal import AsyncSignal
 from sats_receiver.manager import ReceiverManager
 from sats_receiver.utils import SysUsage
 
 
 def setup_logging(q: mp.Queue, log_lvl: int):
@@ -32,14 +35,17 @@
     qhl.start()
     atexit.register(qhl.stop)
 
     # PIL logging level
     pil_logger = logging.getLogger('PIL')
     pil_logger.setLevel(logging.DEBUG + 2)
 
+    gr_logger = gr.gr.logging()
+    gr_logger.set_default_level(gr.gr.log_levels.info)
+
 
 if __name__ == '__main__':
     ap = argparse.ArgumentParser()
     ap.add_argument('config', type=pathlib.Path, help='Config file path')
     ap.add_argument('--log', default='INFO', type=(lambda x: getattr(logging, x.upper(), None)),
                     help='Logging level, INFO default')
     ap.add_argument('--sysu', default=SysUsage.DEFAULT_INTV, type=int,
```

### Comparing `sats_receiver-0.1.19/sats_receiver/async_signal.py` & `sats_receiver-0.1.76/sats_receiver/async_signal.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.19/sats_receiver/gr_modules/decoders.py` & `sats_receiver-0.1.76/sats_receiver/gr_modules/decoders.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,42 +16,45 @@
 import gnuradio.gr
 
 from PIL import ExifTags
 
 from sats_receiver import utils
 from sats_receiver.gr_modules.epb import sstv as sstv_epb
 from sats_receiver.observer import Observer
-from sats_receiver.systems import apt, sstv
+from sats_receiver.systems import apt, satellites as sats, sstv
 
 
 class Decoder(gr.gr.hier_block2):
     def __init__(self,
                  name: str,
                  sat_name: str,
+                 subname: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path):
         self.prefix = f'{self.__class__.__name__}: {sat_name}'
         self.log = logging.getLogger(self.prefix)
 
         super(Decoder, self).__init__(
             name,
             gr.gr.io_signature(1, 1, gr.gr.sizeof_gr_complex),
             gr.gr.io_signature(0, 0, 0)
         )
 
         self.now = dt.datetime.fromtimestamp(0)
         self.sat_name = sat_name
+        self.subname = subname and '_' + subname
         self.samp_rate = samp_rate
         self.out_dir = out_dir
         self.tmp_file = utils.mktmp(prefix='_'.join(name.lower().split()))
-        self.base_kw = dict(log=self.log, sat_name=sat_name, out_dir=out_dir)
+        self.base_kw = dict(log=self.log, sat_name=sat_name, subname=self.subname,
+                            samp_rate=samp_rate, out_dir=out_dir)
 
     def start(self):
-        self.tmp_file = self.out_dir / ('_'.join([self.t.strftime('%Y%m%d%H%M%S'),
-                                                  *self.name().lower().split()]) + '.tmp')
+        pfx = '_'.join([*self.name().lower().split(), self.now.strftime('%Y%m%d%H%M%S')])
+        self.tmp_file = utils.mktmp(self.out_dir, pfx)
         self.base_kw.update(tmp_file=self.tmp_file)
 
     def finalize(self, executor, fin_key: str):
         pass
 
     @property
     def t(self) -> dt.datetime:
@@ -59,17 +62,18 @@
         self.now = t
         return t
 
 
 class RawDecoder(Decoder):
     def __init__(self,
                  sat_name: str,
+                 subname: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path):
-        super(RawDecoder, self).__init__('Raw Decoder', sat_name, samp_rate, out_dir)
+        super(RawDecoder, self).__init__('Raw Decoder', sat_name, subname, samp_rate, out_dir)
 
         self.ctf = gr.blocks.complex_to_float(1)
         self.wav_sink = gr.blocks.wavfile_sink(
             str(self.tmp_file),
             2,
             samp_rate,
             gr.blocks.FORMAT_WAV,
@@ -89,34 +93,43 @@
 
     def finalize(self, executor, fin_key: str):
         self.wav_sink.close()
         if self.tmp_file.exists():
             executor.execute(self._raw_finalize, **self.base_kw, fin_key=fin_key)
 
     @staticmethod
-    def _raw_finalize(log, sat_name, out_dir, tmp_file, fin_key) -> Optional[tuple[str, str, str, dt.datetime]]:
+    def _raw_finalize(log: logging.Logger,
+                      sat_name: str,
+                      subname: str,
+                      out_dir: pathlib.Path,
+                      tmp_file: pathlib.Path,
+                      fin_key: str,
+                      **kw) -> tuple[utils.Decode, str, str, pathlib.Path, dt.datetime]:
         log.debug('finalizing...')
 
         d = dt.datetime.fromtimestamp(tmp_file.stat().st_mtime, dateutil.tz.tzutc())
-        res_fn = tmp_file.rename(out_dir / d.strftime(f'{sat_name}_%Y-%m-%d_%H-%M-%S_RAW.wav'))
+        res_fn = tmp_file.rename(out_dir / d.strftime(f'{sat_name}_%Y-%m-%d_%H-%M-%S,%f{subname}_RAW.wav'))
         st = res_fn.stat()
         log.info('finish: %s (%s)', res_fn, utils.numbi_disp(st.st_size))
 
-        return sat_name, fin_key, res_fn, dt.datetime.fromtimestamp(st.st_mtime, dateutil.tz.tzutc())
+        return utils.Decode.RAW, sat_name, fin_key, res_fn, dt.datetime.fromtimestamp(st.st_mtime, dateutil.tz.tzutc())
 
 
 class AptDecoder(Decoder):
     def __init__(self,
                  sat_name: str,
+                 subname: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path,
-                 sat_ephem_tle: Optional[tuple[ephem.EarthSatellite, tuple[str, str, str]]],
+                 sat_ephem_tle: tuple[ephem.EarthSatellite, tuple[str, str, str]],
                  observer_lonlat: tuple[float, float]):
         name = 'APT Decoder'
-        super(AptDecoder, self).__init__(name, sat_name, samp_rate, out_dir)
+        super(AptDecoder, self).__init__(name, sat_name, subname, samp_rate, out_dir)
+
+        self.already_fins = 0
 
         pfx = '_'.join(name.lower().split())
         self.corr_file = utils.mktmp(dir=out_dir, prefix=pfx, suffix='.corr')
         self.peaks_file = utils.mktmp(dir=out_dir, prefix=pfx, suffix='.peaks')
         self.sat_ephem_tle = sat_ephem_tle
         self.observer_lonlat = observer_lonlat
         self.base_kw.update(sat_tle=sat_ephem_tle[1], observer_lonlat=observer_lonlat)
@@ -151,16 +164,16 @@
         self.correllator = gr.digital.corr_est_cc(
             symbols=apt.Apt.SYNC_A,
             sps=1,
             mark_delay=1,
             threshold=0.9,
             threshold_method=gr.digital.THRESHOLD_ABSOLUTE,
         )
-        self.ctf_out = gr.blocks.complex_to_float()
-        self.ctf_corr = gr.blocks.complex_to_float()
+        self.ctr_out = gr.blocks.complex_to_real()
+        self.ctr_corr = gr.blocks.complex_to_real()
 
         self.out_file_sink = gr.blocks.file_sink(gr.gr.sizeof_float, str(self.tmp_file), False)
         self.out_corr_sink = gr.blocks.file_sink(gr.gr.sizeof_float, str(self.corr_file), False)
         self.peak_detector = gr.blocks.peak_detector2_fb(
             threshold_factor_rise=7,
             look_ahead=apt.Apt.FRAME_WIDTH * apt.Apt.WORK_RATE // apt.Apt.FINAL_RATE,
             alpha=0.001,
@@ -172,144 +185,173 @@
             self.frs,
             self.rsp,
             self.lpf,
             self.ctm,
             self.ftc,
             # self.dc_rem,
             self.correllator,
-            self.ctf_out,
+            self.ctr_out,
             self.out_file_sink,
         )
         self.connect(
             (self.correllator, 1),
-            self.ctf_corr,
+            self.ctr_corr,
             self.out_corr_sink,
         )
         self.connect(
-            self.ctf_corr,
+            self.ctr_corr,
             self.peak_detector,
             self.out_peaks_sink,
         )
 
         utils.close(self.out_file_sink, self.out_corr_sink, self.out_peaks_sink)
         utils.unlink(self.tmp_file, self.corr_file, self.peaks_file)
 
     def start(self):
+        self.already_fins = 0
         super(AptDecoder, self).start()
-        self.corr_file = self.out_dir / ('_'.join([self.now.strftime('%Y%m%d%H%M%S'),
-                                                   *self.name().lower().split()]) + '.corr.tmp')
-        self.peaks_file = self.out_dir / ('_'.join([self.now.strftime('%Y%m%d%H%M%S'),
-                                                    *self.name().lower().split()]) + '.peaks.tmp')
+
+        pfx = '_'.join([*self.name().lower().split(), self.now.strftime('%Y%m%d%H%M%S')])
+        self.corr_file = utils.mktmp(self.out_dir, pfx, '.corr.tmp')
+        self.peaks_file = utils.mktmp(self.out_dir, pfx, '.peaks.tmp')
         self.base_kw.update(corr_file=self.corr_file, peaks_file=self.peaks_file)
 
         self.out_file_sink.open(str(self.tmp_file))
         self.out_file_sink.set_unbuffered(False)
 
         self.out_corr_sink.open(str(self.corr_file))
         self.out_corr_sink.set_unbuffered(False)
 
         self.out_peaks_sink.open(str(self.peaks_file))
         self.out_peaks_sink.set_unbuffered(False)
 
     def finalize(self, executor, fin_key: str):
+        if self.already_fins:
+            self.log.debug('Already finalized. Skip')
+            return
+
+        self.already_fins = 1
         self.out_file_sink.do_update()
         self.out_corr_sink.do_update()
         self.out_peaks_sink.do_update()
 
         utils.close(self.out_file_sink, self.out_corr_sink, self.out_peaks_sink)
 
         for p in self.tmp_file, self.corr_file, self.peaks_file:
             if not p.exists():
-                self.log.warning('%s: missing components `%s`', p)
+                self.log.warning('missing components `%s`', p)
                 utils.unlink(self.tmp_file, self.corr_file, self.peaks_file)
                 return
 
         executor.execute(self._apt_finalize, **self.base_kw, fin_key=fin_key)
 
     @staticmethod
     def _apt_finalize(log: logging.Logger,
                       sat_name: str,
+                      subname: str,
                       sat_tle: tuple[str, str, str],
                       observer_lonlat: tuple[float, float],
                       tmp_file: pathlib.Path,
                       corr_file: pathlib.Path,
                       peaks_file: pathlib.Path,
                       out_dir: pathlib.Path,
-                      fin_key: str) -> Optional[tuple[str, str, pathlib.Path, dt.datetime]]:
+                      fin_key: str,
+                      **kw) -> Optional[tuple[utils.Decode, str, str, pathlib.Path, dt.datetime]]:
         log.debug('finalizing...')
 
         a = apt.Apt(sat_name, tmp_file, corr_file, peaks_file, sat_tle, observer_lonlat)
         x = a.process()
 
         utils.unlink(tmp_file, corr_file, peaks_file)
 
         if x:
             log.info('finish with error')
         else:
             res_fn, sz = a.to_apt(out_dir)
+            if subname:
+                res_fn = res_fn.rename(res_fn.with_stem(res_fn.stem + subname))
             log.info('finish: %s (%s)', res_fn, utils.numbi_disp(sz))
 
-            return sat_name, fin_key, res_fn, a.end_time
+            return utils.Decode.APT, sat_name, fin_key, res_fn, a.end_time
 
 
-class RawStreamDecoder(Decoder):
+class ConstelSoftDecoder(Decoder):
+    CONSTELLS = {
+        '16QAM': gr.digital.constellation_16qam,
+        '8PSK': gr.digital.constellation_8psk,
+        '8PSK_NATURAL': gr.digital.constellation_8psk_natural,
+        'BPSK': gr.digital.constellation_bpsk,
+        'DQPSK': gr.digital.constellation_dqpsk,
+        'PSK': gr.digital.constellation_psk,
+        'QPSK': gr.digital.constellation_qpsk,
+        'OQPSK': gr.digital.constellation_qpsk,
+    }
+
     def __init__(self,
                  sat_name: str,
+                 subname: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path,
-                 name='RAW Stream Decoder'):
-        super(RawStreamDecoder, self).__init__(name, sat_name, samp_rate, out_dir)
+                 constellation,
+                 name='Constellation Soft Decoder'):
+        super(ConstelSoftDecoder, self).__init__(name, sat_name, subname, samp_rate, out_dir)
 
-        self.ctf = gr.blocks.complex_to_float(1)
+        if isinstance(constellation, str):
+            self.constellation = self.CONSTELLS[constellation.upper()]().base()
+        else:
+            raise TypeError(f'`constellation` expected str, got {type(constellation)} instead')
+
+        self.constellation.gen_soft_dec_lut(8)
+        self.constel_soft_decoder = gr.digital.constellation_soft_decoder_cf(self.constellation)
         self.rail = gr.analog.rail_ff(-1, 1)
         self.ftch = gr.blocks.float_to_char(1, 127)
-        # self.fts = gr.blocks.float_to_short(1, 32767)
-        # self.stch = gr.blocks.short_to_char(1)
 
         self.out_file_sink = gr.blocks.file_sink(gr.gr.sizeof_char, str(self.tmp_file), False)
         self.out_file_sink.close()
         utils.unlink(self.tmp_file)
 
         self.connect(
             self,
-            self.ctf,
+            self.constel_soft_decoder,
             self.rail,
             self.ftch,
             self.out_file_sink,
         )
 
     def start(self):
-        super(RawStreamDecoder, self).start()
+        super(ConstelSoftDecoder, self).start()
 
         self.out_file_sink.open(str(self.tmp_file))
         self.out_file_sink.set_unbuffered(False)
 
     def finalize(self, executor, fin_key: str):
         self.out_file_sink.do_update()
         self.out_file_sink.close()
         if self.tmp_file.exists():
-            executor.execute(self._raw_stream_finalize, **self.base_kw, fin_key=fin_key)
+            executor.execute(self._constel_soft_finalize, **self.base_kw, fin_key=fin_key)
 
     @staticmethod
-    def _raw_stream_finalize(log: logging.Logger,
-                             sat_name: str,
-                             out_dir: pathlib.Path,
-                             tmp_file: pathlib.Path,
-                             fin_key: str) -> Optional[tuple[str, str, pathlib.Path, dt.datetime]]:
+    def _constel_soft_finalize(log: logging.Logger,
+                               sat_name: str,
+                               subname: str,
+                               out_dir: pathlib.Path,
+                               tmp_file: pathlib.Path,
+                               fin_key: str,
+                               **kw) -> tuple[utils.Decode, str, str, pathlib.Path, dt.datetime]:
         log.debug('finalizing...')
 
         d = dt.datetime.fromtimestamp(tmp_file.stat().st_mtime, dateutil.tz.tzutc())
-        res_fn = tmp_file.rename(out_dir / d.strftime(f'{sat_name}_%Y-%m-%d_%H-%M-%S_RAW.s'))
+        res_fn = tmp_file.rename(out_dir / d.strftime(f'{sat_name}_%Y-%m-%d_%H-%M-%S,%f{subname}_RAW.s'))
         st = res_fn.stat()
         log.info('finish: %s (%s)', res_fn, utils.numbi_disp(st.st_size))
 
-        return sat_name, fin_key, res_fn, dt.datetime.fromtimestamp(st.st_mtime, dateutil.tz.tzutc())
+        return utils.Decode.CSOFT, sat_name, fin_key, res_fn, dt.datetime.fromtimestamp(st.st_mtime, dateutil.tz.tzutc())
 
 
-class LrptDecoder(RawStreamDecoder):
+class LrptDecoder(ConstelSoftDecoder):
     def __init__(self,
                  sat_name: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path):
         raise NotImplementedError()
         super(LrptDecoder, self).__init__(sat_name, samp_rate, out_dir, name='LRPT Decoder')
 
@@ -321,20 +363,21 @@
 
 
 class SstvDecoder(Decoder):
     _FREQ_1 = (1900 - 1200) / 2
 
     def __init__(self,
                  sat_name: str,
+                 subname: str,
                  samp_rate: Union[int, float],
                  out_dir: pathlib.Path,
                  observer: Observer = None,
                  do_sync=True,
                  wsr=16000):
-        super(SstvDecoder, self).__init__('SSTV Decoder', sat_name, samp_rate, out_dir)
+        super(SstvDecoder, self).__init__('SSTV Decoder', sat_name, subname, samp_rate, out_dir)
 
         self.observer = observer
         self.do_sync = do_sync
         self.wsr = wsr
 
         hdr_pix_width = int(wsr * sstv.Sstv.HDR_PIX_S)
         hdr = sstv.Sstv.HDR_SYNC_WORD.repeat(hdr_pix_width)
@@ -355,36 +398,36 @@
         self.rsp = gr.filter.rational_resampler_fcc(
                 interpolation=wsr // resamp_gcd,
                 decimation=samp_rate // resamp_gcd,
                 taps=[],
                 fractional_bw=0
         )
         self.correllator = gr.digital.corr_est_cc(hdr, hdr_pix_width, 1, 0.4, gr.digital.THRESHOLD_ABSOLUTE)
-        self.ctf_out = gr.blocks.complex_to_float()
+        self.ctr_out = gr.blocks.complex_to_real()
         self.out_add_const = gr.blocks.add_const_ff(450 / self._FREQ_1)
         self.out_multiply_const = gr.blocks.multiply_const_ff(self._FREQ_1 / (750 + 450))
-        self.ctf_corr = gr.blocks.complex_to_float()
+        self.ctr_corr = gr.blocks.complex_to_real()
         self.corr_peak_detector = gr.blocks.peak_detector2_fb(0.1, hdr.size, 0.001)
         self.sstv_epb = sstv_epb.SstvEpb(wsr, do_sync, self.log, sat_name, out_dir)
 
         self.connect(
             self,
             self.bpf_input,
             self.frs,
             self.quad_demod,
             self.rsp,
             self.correllator,
-            self.ctf_out,
+            self.ctr_out,
             self.out_add_const,
             self.out_multiply_const,
             (self.sstv_epb, self.sstv_epb.OUT_IN),
         )
         self.connect(
             (self.correllator, 1),
-            self.ctf_corr,
+            self.ctr_corr,
             self.corr_peak_detector,
             (self.sstv_epb, self.sstv_epb.PEAKS_IN),
         )
 
         if observer is None:
             latlonalt = None
         else:
@@ -399,46 +442,116 @@
         self.sstv_epb.stop()
         sstv_rr: list[sstv.SstvRecognizer] = self.sstv_epb.finalize()
         executor.execute(self._sstv_finalize, **self.base_kw, sstv_rr=sstv_rr, fin_key=fin_key)
 
     @staticmethod
     def _sstv_finalize(log: logging.Logger,
                        sat_name: str,
+                       subname: str,
                        out_dir: pathlib.Path,
                        observer_latlonalt: Optional[tuple[str, str, Union[int, float]]],
                        sstv_rr: list[sstv.SstvRecognizer],
-                       fin_key: str) -> tuple[str, str, list[tuple[pathlib.Path, dt.datetime]]]:
+                       fin_key: str,
+                       **kw) -> tuple[utils.Decode, str, str, list[tuple[pathlib.Path, dt.datetime]]]:
         log.debug('finalizing...')
 
         if observer_latlonalt:
             observer = ephem.Observer()
             observer.lat, observer.lon, observer.elev = observer_latlonalt
 
         fn_dt = []
         sz_sum = 0
         for i in sstv_rr:
+            if not i.sstv and i.vis_code:
+                continue
             img = i.get_image()
             if not img:
                 continue
 
             if observer_latlonalt:
                 log.debug('add GPSInfo EXIF')
                 img = utils.img_add_exif(img, observer=observer)
             exif = img.getexif()
 
             sstv_mode = exif.get_ifd(ExifTags.IFD.Exif).get(ExifTags.Base.UserComment, 'SSTV')
             end_time = exif.get(ExifTags.Base.DateTime)
             end_time = (dt.datetime.strptime(end_time, '%Y:%m:%d %H:%M:%S')
                         if end_time
                         else dt.datetime.utcnow())
-            res_fn = out_dir / end_time.strftime(f'{sat_name}_{sstv_mode}_%Y-%m-%d_%H-%M-%S,%f_{fin_key}.png')
+            res_fn = out_dir / end_time.strftime(f'{sat_name}_{sstv_mode}_%Y-%m-%d_%H-%M-%S,%f{subname}.png')
 
             img.save(res_fn, exif=exif)
 
             fn_dt.append((res_fn, end_time))
             sz = res_fn.stat().st_size
             sz_sum += sz
             log.info('finish: %s (%s)', res_fn, utils.numbi_disp(sz))
 
         log.info('finish %s images (%s)', len(fn_dt), utils.numbi_disp(sz_sum))
 
-        return sat_name, fin_key, fn_dt
+        return utils.Decode.SSTV, sat_name, fin_key, fn_dt
+
+
+class SatellitesDecoder(Decoder):
+    def __init__(self,
+                 sat_name: str,
+                 subname: str,
+                 samp_rate: Union[int, float],
+                 out_dir: pathlib.Path,
+                 config: dict,
+                 is_iq=True):
+        super(SatellitesDecoder, self).__init__('GR Satellites Decoder', sat_name, subname, samp_rate, out_dir)
+        opt_str = (
+            f' --file_output_path="{out_dir}"'
+            # f' --codec2_ip='
+            # f' --codec2_port='
+        )
+
+        x = config.copy()
+        if 'tlm_decode' in x:
+            x.pop('tlm_decode')
+        if all(map(lambda v: v is None, x.values())):
+            if sat_name.isnumeric():
+                config['norad'] = int(sat_name)
+            else:
+                config['name'] = sat_name
+
+        self.sat_fg = sats.SatFlowgraph(self.log, samp_rate, opt_str, is_iq=is_iq, **config)
+        if is_iq:
+            self.connect(self, self.sat_fg)
+        else:
+            self.ctor = gr.blocks.complex_to_real()
+            self.connect(self, self.ctor, self.sat_fg)
+
+    def start(self):
+        utils.unlink(self.tmp_file)
+
+    def finalize(self, executor, fin_key: str):
+        utils.close(f.f
+                    for d in self.sat_fg.get_files().values()
+                    for f in d.values())
+
+        d = {}
+        for dtype, v in self.sat_fg.get_files().items():
+            x = []
+            for f in v.values():
+                utils.close(f.f)
+                x.append(f.path)
+            d[dtype] = x
+        self.sat_fg.clean()
+
+        executor.execute(self._sats_finalize, **self.base_kw, files=d, fin_key=fin_key)
+
+    @staticmethod
+    def _sats_finalize(log: logging.Logger,
+                       sat_name: str,
+                       files: dict[str, list[pathlib.Path]],
+                       fin_key: str,
+                       **kw) -> tuple[utils.Decode, str, str, dict[str, list[pathlib.Path]]]:
+
+        f_cnt = 0
+        for v in files.values():
+            f_cnt += len(v)
+
+        log.info('finish %s files', f_cnt)
+
+        return utils.Decode.SATS, sat_name, fin_key, files
```

### Comparing `sats_receiver-0.1.19/sats_receiver/gr_modules/demodulators.py` & `sats_receiver-0.1.76/sats_receiver/gr_modules/demodulators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,33 @@
-import logging
 import math
 
 from typing import Union
 
 import gnuradio as gr
 import gnuradio.analog
+import gnuradio.blocks
 import gnuradio.digital
 import gnuradio.filter
 import gnuradio.gr
 
+from sats_receiver.gr_modules.epb import DelayOneImag
+
 
 class QpskDemod(gr.gr.hier_block2):
     def __init__(self,
                  samp_rate: Union[int, float],
                  baudrate: Union[int, float],
                  excess_bw: Union[int, float] = None,
                  ntaps: int = None,
-                 costas_bw: Union[int, float] = None):
+                 costas_bw: Union[int, float] = None,
+                 oqpsk=False):
         super(QpskDemod, self).__init__(
             'QPSK Demodulator',
             gr.gr.io_signature(1, 1, gr.gr.sizeof_gr_complex),
-            gr.gr.io_signature(1, 1, gr.gr.sizeof_float)
+            gr.gr.io_signature(1, 1, gr.gr.sizeof_gr_complex)
         )
 
         if excess_bw is None:
             excess_bw = 0.35
         if ntaps is None:
             ntaps = 33
         if costas_bw is None:
@@ -42,16 +45,22 @@
                 sampling_freq=samp_rate,
                 symbol_rate=baudrate,
                 alpha=excess_bw,
                 ntaps=ntaps
             )
         )
         self.agc = gr.analog.agc_cc(0.1, 1.0, 1.0)
-        self.agc.set_max_gain(10e6)
+        self.agc.set_max_gain(65536)
         self.costas = gr.digital.costas_loop_cc(costas_bw, 4, False)
+
+        if oqpsk:
+            self.after_costas = DelayOneImag()
+            self.connect(self.costas, self.after_costas)
+        else:
+            self.after_costas = self.costas
         # self.symbol_sync = gr.digital.symbol_sync_cc(
         #     detector_type=gr.digital.TED_MUELLER_AND_MULLER,
         #     sps=samp_rate / baudrate,
         #     loop_bw=(2 * math.pi) / (2 * baudrate),
         #     damping_factor=1.0,
         #     ted_gain=1.0,
         #     max_deviation=1.5,
@@ -64,19 +73,72 @@
         self.recov = gr.digital.clock_recovery_mm_cc(
             omega=samp_rate / baudrate,
             gain_omega=1e-6,
             mu=0.5,
             gain_mu=0.01,
             omega_relative_limit=0.01,
         )
-        self.constel_decoder = gr.digital.constellation_soft_decoder_cf(gr.digital.constellation_qpsk().base())
 
         self.connect(
             self,
             self.rrc,
             self.agc,
             self.costas,
+        )
+        self.connect(
+            self.after_costas,
             # self.symbol_sync,
             self.recov,
-            self.constel_decoder,
             self,
         )
+
+
+class GmskDemod(gr.gr.hier_block2):
+    def __init__(self,
+                 samp_rate: Union[int, float],
+                 channels: list[int]):
+        chan_n = len(channels)
+        super(GmskDemod, self).__init__(
+            'GMSK Demodulator',
+            gr.gr.io_signature(1, 1, gr.gr.sizeof_gr_complex),
+            gr.gr.io_signature(1, 1, gr.gr.sizeof_float)
+            if chan_n == 1
+            else gr.gr.io_signature.makev(chan_n, chan_n, [gr.gr.sizeof_float] * chan_n)
+        )
+
+        self.samp_rate = samp_rate
+        self._channels = channels
+        self.wsr = int(max(channels) * 2)
+        self.resamp_gcd = math.gcd(samp_rate, self.wsr)
+        self._chans = []
+
+        self.resamp = gr.filter.rational_resampler_ccc(
+            interpolation=(self.wsr // self.resamp_gcd),
+            decimation=(samp_rate // self.resamp_gcd),
+            taps=[],
+            fractional_bw=0,
+        )
+
+        self.connect(self, self.resamp)
+
+        for i, rate in enumerate(channels):
+            gmsk_demod = gr.digital.gmsk_demod(
+                samples_per_symbol=self.wsr // rate,
+                gain_mu=0.175,
+                mu=0.5,
+                omega_relative_limit=0.005,
+                freq_error=0.0,
+                verbose=False,
+                log=False
+            )
+            uchtf = gr.blocks.uchar_to_float()
+            self.connect(
+                self.resamp,
+                gmsk_demod,
+                uchtf,
+                (self, i),
+            )
+            self._chans.append((gmsk_demod, uchtf))
+
+    @property
+    def channels(self):
+        return self._channels
```

### Comparing `sats_receiver-0.1.19/sats_receiver/gr_modules/epb/prober.py` & `sats_receiver-0.1.76/sats_receiver/gr_modules/epb/prober.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.19/sats_receiver/gr_modules/epb/sstv.py` & `sats_receiver-0.1.76/sats_receiver/gr_modules/epb/sstv.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 class SstvEpb(gr.gr.sync_block):
     OUT_IN = 0
     PEAKS_IN = 1
 
     def __init__(self, srate=16000, do_sync=True, log=None, sat_name='unknown', out_dir=None):
         super(SstvEpb, self).__init__(
-            name='SstvProcess',
+            name='SstvEpb',
             in_sig=[np.float32, np.byte],   # [out, corr]
             out_sig=None,
         )
         self.srate = srate
         self.do_sync = do_sync
         self.log = log
         self.sat_name = sat_name
@@ -44,14 +44,19 @@
             elif status == sstv.SstvRecognizer.STATUS_DONE:
                 self.log.info('%s: Done', self.sstv[i].sstv.name)
                 self.sstv_done.append(self.sstv[i])
                 self.sstv = []
                 self.find_sstv = 1
                 break
 
+            elif status == sstv.SstvRecognizer.STATUS_VIS_UNKNOWN:
+                if self.sstv[i].vis_code:
+                    self.sstv_done.append(self.sstv[i])
+                to_delete.append(i)
+
             elif status != sstv.SstvRecognizer.STATUS_OK:
                 to_delete.append(i)
 
         for i in sorted(to_delete, reverse=True):
             self.sstv.pop(i)
 
         return input_items[self.PEAKS_IN].size
```

### Comparing `sats_receiver-0.1.19/sats_receiver/gr_modules/modules.py` & `sats_receiver-0.1.76/sats_receiver/gr_modules/modules.py`

 * *Files 16% similar despite different names*

```diff
@@ -80,16 +80,27 @@
                         # 'qpsk_baudrate',    # only in QPSK demode
                         # 'qpsk_excess_bw',   # optional
                         # 'qpsk_ntaps',       # optional
                         # 'qpsk_costas_bw',   # optional
 
                         # 'sstv_wsr',         # optional, only in SSTV decode
                         # 'sstv_sync',        # optional, only in SSTV decode
+
+                        # 'channels',         # only for GMSK
+
+                        # 'sats_file',        # optional, only for SATS decode
+                        # 'sats_name',        # optional, only for SATS decode
+                        # 'sats_norad',       # optional, only for SATS decode
+                        # 'sats_tlm_decode',  # optional, only for SATS decode
                     ]))
             and (config['mode'] != utils.Mode.QPSK or 'qpsk_baudrate' in config)
+            and (config['mode'] != utils.Mode.GMSK or 'channels' in config)
+            and (config['mode'] != utils.Mode.RAW or config['decode'] == utils.Decode.SATS)
+            # and (config['mode'] != utils.Mode.RAW or
+            #      (config['decode'] != utils.Decode.SATS or (set(config.keys()) & {'grs_file', 'grs_name', 'grs_norad'})))
         )
 
     def __init__(self,
                  up: 'Satellite',
                  config: Mapping,
                  main_tune: Union[int, float],
                  samp_rate: Union[int, float]):
@@ -142,63 +153,88 @@
             self.demodulator = gr.analog.wfm_rcv(
                 quad_rate=self.bandwidth,
                 audio_decimation=1,
             )
 
         elif self.mode == utils.Mode.WFM_STEREO:
             if self.bandwidth < 76800:
-                raise ValueError(f'{self.prefix}: param `bandwidth` for WFM Stereo must be at least 76800, got {self.bandwidth} instead')
+                raise ValueError(f'{self.prefix}: param `bandwidth` for WFM Stereo must be at least 76800, '
+                                 f'got {self.bandwidth} instead')
             self.demodulator = gr.analog.wfm_rcv_pll(
                 demod_rate=self.bandwidth,
                 audio_decimation=1,
                 deemph_tau=50e-6,
             )
             self.connect((self.demodulator, 1), (self.post_demod, 1))
 
         elif self.mode == utils.Mode.QUAD:
             self.demodulator = gr.analog.quadrature_demod_cf(1)
 
-        elif self.mode == utils.Mode.QPSK:
-            self.demodulator = demodulators.QpskDemod(self.bandwidth, self.qpsk_baudrate, self.qpsk_excess_bw, self.qpsk_ntaps, self.qpsk_costas_bw)
+        elif self.mode in (utils.Mode.QPSK, utils.Mode.OQPSK):
+            oqpsk = self.mode == utils.Mode.OQPSK
+            self.demodulator = demodulators.QpskDemod(self.bandwidth, self.qpsk_baudrate, self.qpsk_excess_bw,
+                                                      self.qpsk_ntaps, self.qpsk_costas_bw, oqpsk)
+            self.post_demod = None
 
+        elif self.mode == utils.Mode.GMSK:
+            self.demodulator = demodulators.GmskDemod(self.bandwidth, self.channels)
+
+        channels = getattr(self.demodulator, 'channels', (self.bandwidth,))
+        self.decoders = []
         if self.decode == utils.Decode.APT:
-            self.decoder = decoders.AptDecoder(up.name, self.bandwidth, up.output_directory, up.sat_ephem_tle, up.observer.lonlat)
+            self.decoders.append(decoders.AptDecoder(up.name, self.subname, self.bandwidth, up.output_directory,
+                                                     up.sat_ephem_tle, up.observer.lonlat))
 
         # elif self.decode == Decode.LRPT:
         #     # TODO
         #     # self.decoder =
 
-        elif self.decode == utils.Decode.RSTREAM:
-            self.decoder = decoders.RawStreamDecoder(up.name, self.bandwidth, up.output_directory)
+        elif self.decode == utils.Decode.CSOFT:
+            self.decoders.append(decoders.ConstelSoftDecoder(up.name, self.subname, self.bandwidth,
+                                                             up.output_directory, self.mode.value))
 
         elif self.decode == utils.Decode.RAW:
-            self.decoder = decoders.RawDecoder(up.name, self.bandwidth, up.output_directory)
+            for ch in channels:
+                self.decoders.append(decoders.RawDecoder(up.name, self.subname, ch, up.output_directory))
 
         elif self.decode == utils.Decode.SSTV:
-            self.decoder = decoders.SstvDecoder(up.name, self.bandwidth, up.output_directory, up.observer, self.sstv_sync, self.sstv_wsr)
+            self.decoders.append(decoders.SstvDecoder(up.name, self.subname, self.bandwidth, up.output_directory,
+                                                      up.observer, self.sstv_sync, self.sstv_wsr))
 
-        self.connect(
-            self,
-            self.radio,
-            *((self.demodulator, self.post_demod) if self.demodulator else tuple()),
-            self.decoder,
-        )
+        elif self.decode == utils.Decode.SATS:
+            cfg = dict(file=self.grs_file, name=self.grs_name, norad=self.grs_norad, tlm_decode=self.grs_tlm_decode)
+            self.decoders.append(decoders.SatellitesDecoder(up.name, self.subname, self.bandwidth,
+                                                            up.output_directory, cfg))
+
+        x = [self, self.radio]
+        if self.demodulator:
+            x.append(self.demodulator)
+            if self.post_demod:
+                x.append(self.post_demod)
+
+        self.connect(*x)
+        for i, decoder in enumerate(self.decoders):
+            self.connect((x[-1], i), decoder)
 
     def set_freq_offset(self, new_freq: Union[int, float]):
         self.radio.set_freq_offset(new_freq)
 
     @property
     def is_runned(self) -> bool:
         return self.radio.enabled
 
     @property
     def enabled(self) -> bool:
         return self.config.get('enabled', True)
 
     @property
+    def subname(self) -> str:
+        return self.config.get('subname', '')
+
+    @property
     def freq(self) -> Union[int, float]:
         return self.config['freq']
 
     @property
     def freq_correction(self) -> Union[int, float]:
         return self.config.get('freq_correction', 0)
 
@@ -224,28 +260,52 @@
 
     @property
     def qpsk_excess_bw(self) -> Union[int, float]:
         return self.config.get('qpsk_excess_bw', 0.35)
 
     @property
     def qpsk_ntaps(self) -> int:
-        return int(self.config.get('qpsk_ntaps'), 33)
+        return int(self.config.get('qpsk_ntaps', 33))
 
     @property
     def qpsk_costas_bw(self) -> Union[int, float]:
         return self.config.get('qpsk_costas_bw', 0.005)
 
     @property
     def sstv_wsr(self) -> Union[int, float]:
         return self.config.get('sstv_wsr', 16000)
 
     @property
     def sstv_sync(self) -> bool:
         return self.config.get('sstv_sync', True)
 
+    @property
+    def channels(self) -> list[Union[int, float]]:
+        return self.config['channels']
+
+    @property
+    def grs_file(self) -> Optional[pathlib.Path]:
+        p = self.config.get('grs_file', None)
+        if p:
+            return pathlib.Path(p).expanduser()
+
+    @property
+    def grs_name(self) -> Optional[str]:
+        return self.config.get('grs_name', None)
+
+    @property
+    def grs_norad(self) -> Optional[int]:
+        x = self.config.get('grs_norad', None)
+        if x is not None:
+            return int(x)
+
+    @property
+    def grs_tlm_decode(self) -> bool:
+        return self.config.get('grs_tlm_decode', True)
+
 
 class Satellite(gr.gr.hier_block2):
     @staticmethod
     def _validate_config(config: Mapping) -> bool:
         return (
             all(map(lambda x: x in config,
                     [
@@ -256,15 +316,15 @@
                         # 'doppler',          # optional
                     ]))
             and config['frequencies']
         )
 
     def __init__(self,
                  config: Mapping,
-                 sat_ephem_tle: Optional[tuple[ephem.EarthSatellite, tuple[str, str, str]]],
+                 sat_ephem_tle: tuple[ephem.EarthSatellite, tuple[str, str, str]],
                  observer: Observer,
                  main_tune: Union[int, float],
                  samp_rate: Union[int, float],
                  output_directory: pathlib.Path,
                  executor):
         n = config.get('name', '')
         self.prefix = f'{self.__class__.__name__}{n and f": {n}"}'
@@ -307,27 +367,29 @@
                           self.doppler,
                           [r.mode.value for r in self.recorders],
                           [r.decode.value for r in self.recorders])
             self.output_directory.mkdir(parents=True, exist_ok=True)
             self.start_event = None
 
             for r in self.recorders:
-                r.decoder.start()
+                for decoder in r.decoders:
+                    decoder.start()
                 r.radio.set_enabled(1)
 
     def stop(self):
         if self.is_runned:
             self.log.info('STOP')
             self.start_event = self.stop_event = None
             fin_key = sha256((self.name + str(dt.datetime.now())).encode()).hexdigest()
 
             for r in self.recorders:
                 if r.is_runned:
                     r.radio.set_enabled(0)
-                    r.decoder.finalize(self.executor, fin_key)
+                    for decoder in r.decoders:
+                        decoder.finalize(self.executor, fin_key)
 
     def correct_doppler(self, observer: ephem.Observer):
         if self.is_runned and self.doppler:
             self.sat_ephem_tle[0].compute(observer)
 
             for r in self.recorders:
                 if r.is_runned:
@@ -342,15 +404,15 @@
         return self.config.get('enabled', True) and self.recorders
 
     @property
     def min_elevation(self) -> Union[int, float]:
         return self.config.get('min_elevation', 0.0)
 
     @property
-    def frequencies(self) -> Mapping:
+    def frequencies(self) -> list[Mapping]:
         return self.config['frequencies']
 
     @property
     def doppler(self) -> bool:
         return self.config.get('doppler', True)
 
     @property
```

### Comparing `sats_receiver-0.1.19/sats_receiver/gr_modules/receiver.py` & `sats_receiver-0.1.76/sats_receiver/gr_modules/receiver.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,15 +125,16 @@
 
                 sat_ephem_tle = self.up.tle.get(sat_name)
                 if sat_ephem_tle is None:
                     self.log.info('Sat `%s` not found in TLE. Skip', sat_name)
                     continue
 
                 try:
-                    sat = modules.Satellite(cfg, sat_ephem_tle, self.up.observer, self.tune, self.samp_rate, self.output_directory, self.up.executor)
+                    sat = modules.Satellite(cfg, sat_ephem_tle, self.up.observer, self.tune, self.samp_rate,
+                                            self.output_directory, self.up.executor)
                 except ValueError as e:
                     self.log.warning('%s: %s. Skip', sat_name, e)
                     continue
 
                 if self.calculate_pass(sat):
                     if self.is_runned:
                         self.connect(self.blocks_correctiq, sat)
@@ -194,14 +195,22 @@
         """
         Receiver tune frequency, Hz
         """
 
         return self.config['tune']
 
     @property
+    def freq_correction(self) -> Union[int, float]:
+        """
+        Receiver frequency correction
+        """
+
+        return self.config.get('freq_correction', 0.0)
+
+    @property
     def samp_rate(self) -> Union[int, float]:
         """
         Receiver samplerate, Hz
         """
 
         return self.config['samp_rate']
 
@@ -244,15 +253,15 @@
                     if sat.enabled:
                         self.up.scheduler.plan(t, self.calculate_pass, sat)
 
                 return 1
 
             self.signal_src.set_sample_rate(0, self.samp_rate)
             self.signal_src.set_frequency(0, self.tune)
-            self.signal_src.set_frequency_correction(0, 0)
+            self.signal_src.set_frequency_correction(0, self.freq_correction)
             self.signal_src.set_gain_mode(0, False)
             self.signal_src.set_gain(0, 'TUNER', self.gain)
 
             self.connect(
                 self.signal_src,
                 self.blocks_correctiq,
                 self.src_null_sink,
@@ -326,15 +335,16 @@
                     if set_t < rise_t:
                         rise_t = t
                     sat.events = [
                         None if sat.is_runned else self.up.scheduler.plan(rise_t, sat.start),
                         self.up.scheduler.plan(set_t, sat.stop),
                         self.up.scheduler.plan(set_tt, self.calculate_pass, sat)
                     ]
-                    self.log.info('Sat `%s` planned on %s <-> %s', sat.name, rise_t.astimezone(ltz), set_t.astimezone(ltz))
+                    self.log.info('Sat `%s` planned on %s <-> %s',
+                                  sat.name, rise_t.astimezone(ltz), set_t.astimezone(ltz))
                     break
 
                 t = set_tt
 
             if t > tt:
                 self.log.info('Sat `%s`: No passes found for the next 24 hours', sat.name)
                 self.up.scheduler.plan(tt, self.calculate_pass, sat)
```

### Comparing `sats_receiver-0.1.19/sats_receiver/librtlsdr.py` & `sats_receiver-0.1.76/sats_receiver/librtlsdr.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,14 +63,15 @@
 
 
 _f = _lib.rtlsdr_get_device_count
 _f.restype = c_uint32
 def rtlsdr_get_device_count() -> int:
     return _lib.rtlsdr_get_device_count()
 
+
 _f = _lib.rtlsdr_get_device_name
 _f.argtypes = c_uint32,
 _f.restype = c_char_p
 def rtlsdr_get_device_name(idx: int) -> str:
     return _lib.rtlsdr_get_device_name(idx).decode('utf8')
```

### Comparing `sats_receiver-0.1.19/sats_receiver/manager.py` & `sats_receiver-0.1.76/sats_receiver/manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 import logging.handlers
 import multiprocessing as mp
 import pathlib
 import time
 
 from typing import Mapping
 
+from sats_receiver import utils
 from sats_receiver.gr_modules.receiver import RecUpdState, SatsReceiver
 from sats_receiver.observer import Observer
 from sats_receiver.tle import Tle
-from sats_receiver.utils import Scheduler, SysUsage
 
 
 class Executor(mp.Process):
-    def __init__(self, q: mp.Queue = None, sysu_intv=SysUsage.DEFAULT_INTV):
+    def __init__(self, q: mp.Queue = None, sysu_intv=utils.SysUsage.DEFAULT_INTV):
         super().__init__(daemon=True, name=self.__class__.__name__)
 
         self.q = q
         self.sysu_intv = sysu_intv
         self.rd, self.wr = mp.Pipe(False)
 
     def _setup_process(self):
@@ -28,15 +28,15 @@
         logger.handlers.clear()
         logger.setLevel(mp.get_logger().level)
         if self.q is not None:
             qh = logging.handlers.QueueHandler(self.q)
             logger.addHandler(qh)
             # logging.basicConfig(level=mp.get_logger().level, handlers=[qh])
         self.log = logging.getLogger(self.name)
-        self.sysu = SysUsage(self.name, self.sysu_intv)
+        self.sysu = utils.SysUsage(self.name, self.sysu_intv)
 
     def start(self) -> None:
         super(Executor, self).start()
         self.rd.close()
 
     def run(self):
         self._setup_process()
@@ -83,67 +83,96 @@
             if callable(fn):
                 try:
                     x = fn(*args, **kwargs)
                 except Exception:
                     self.log.exception('%s with args=%s kwargs=%s', fn, args, kwargs)
                     continue
 
-                if x and isinstance(x, tuple):
-                    if len(x) == 4:
-                        sat_name, fin_key, res_filename, end_time = x
-                    elif len(x) == 3:
-                        sat_name, fin_key, fn_dt = x
+                if not x:
+                    continue
+
+                decoder_type = x[0]
+                if decoder_type == utils.Decode.RAW:
+                    _, sat_name, fin_key, res_filename, end_time = x
+
+                elif decoder_type == utils.Decode.CSOFT:
+                    _, sat_name, fin_key, res_filename, end_time = x
+
+                elif decoder_type == utils.Decode.APT:
+                    _, sat_name, fin_key, res_filename, end_time = x
+
+                elif decoder_type == utils.Decode.SSTV:
+                    _, sat_name, fin_key, fn_dt = x
+
+                elif decoder_type == utils.Decode.SATS:
+                    _, sat_name, fin_key, files = x
 
     def execute(self, fn, *args, **kwargs):
         if self.wr:
             self.wr.send((fn, args, kwargs))
 
     def stop(self):
         if self.wr:
             self.wr.send('.')
-            self.wr.close()
+            utils.close(self.wr)
             self.wr = 0
 
 
 class ReceiverManager:
-    def __init__(self, q: mp.Queue, config_filename: pathlib.Path, sysu_intv=SysUsage.DEFAULT_INTV, executor_cls=Executor):
+    TD_ERR_DEF = dt.timedelta(seconds=5)
+
+    def __init__(self,
+                 q: mp.Queue,
+                 config_filename: pathlib.Path,
+                 sysu_intv=utils.SysUsage.DEFAULT_INTV,
+                 executor_cls=Executor):
         self.prefix = self.__class__.__name__
         self.log = logging.getLogger(self.prefix)
 
-        self.sysu = SysUsage(self.prefix, sysu_intv)
+        self.sysu = utils.SysUsage(self.prefix, sysu_intv)
         self.config_filename = config_filename.expanduser().absolute()
         self.config_file_stat = None
         self.config = {}
 
         self.receivers: dict[str, SatsReceiver] = {}
         self.stopped = False
         self.now = dt.datetime.now(dt.timezone.utc)
         self.file_failed_t = 0
 
+        self.t_err = self.now
+        self.td_err = self.TD_ERR_DEF
+
         if not self.update_config(True, True):
             raise ValueError(f'{self.prefix}: Invalid config!')
 
         self.observer = Observer(self.config['observer'])
         self.tle = Tle(self.config['tle'])
-        self.scheduler = Scheduler()
+        self.scheduler = utils.Scheduler()
         self.executor = executor_cls(q, sysu_intv)
         self.executor.start()
         atexit.register(lambda x: (x.stop(), x.join()), self.executor)
 
         for cfg in self.config['receivers']:
             self._add_receiver(cfg)
 
     def _add_receiver(self, cfg: Mapping):
         if cfg.get('enabled', True):
             try:
                 rec = SatsReceiver(self, cfg)
                 self.receivers[cfg['name']] = rec
+                self.td_err = self.TD_ERR_DEF
+                self.t_err = self.now
             except RuntimeError as e:
-                self.log.error('Skip receiver "%s": %s', cfg['name'], e)
-        else:
+                if self.now >= self.t_err:
+                    self.t_err = self.now + self.td_err
+                    self.td_err *= 2
+                    self.log.error('Skip receiver "%s": %s', cfg['name'], e)
+        elif self.now >= self.t_err:
+            self.t_err = self.now + self.td_err
+            self.td_err *= 2
             self.log.debug('Skip disabled receiver `%s`', cfg['name'])
 
     @property
     def t(self) -> dt.datetime:
         """
         Set and return current time
         """
@@ -258,18 +287,19 @@
     def action(self):
         self.sysu.collect()
 
         if self.stopped:
             return 1
 
         try:
+            now = self.t
             self.update_config()
             self.scheduler.action()
-            recalc = self.observer.action(self.t)
-            need_upd = self.tle.action(self.now)
+            recalc = self.observer.action(now)
+            need_upd = self.tle.action(now)
 
             for receiver in self.receivers.values():
                 if recalc:
                     receiver.recalculate_pass()
 
                 if need_upd:
                     receiver.updated = RecUpdState.UPD_NEED
```

### Comparing `sats_receiver-0.1.19/sats_receiver/observer.py` & `sats_receiver-0.1.76/sats_receiver/tle.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,155 +1,193 @@
 import datetime as dt
-import json
 import logging
+import pathlib
+import shutil
 import urllib.error
 import urllib.parse
 import urllib.request
 
 from typing import Mapping, Optional, Union
 
 import ephem
 
+from sats_receiver import TLEDIR
+
+
+class Tle:
+    TD_ERR_DEF = dt.timedelta(seconds=5)
 
-class Observer:
     def __init__(self, config: Mapping):
         self.prefix = self.__class__.__name__
         self.log = logging.getLogger(self.prefix)
 
         self.config = {}
-        self.last_weather_time = dt.datetime.fromtimestamp(0, dt.timezone.utc)
-        self.update_period = 1  # hours
-        self.t_next = self.last_weather_time + dt.timedelta(hours=self.update_period, minutes=1)
-        self._observer = ephem.Observer()
+        self.tle_file = pathlib.Path(TLEDIR / 'dummy')
+        self.last_update_tle = dt.datetime.fromtimestamp(0, dt.timezone.utc)
+        self.objects: dict[str, tuple[ephem.EarthSatellite, tuple[str, str, str]]] = {}
+        self.t_err = self.last_update_tle
+        self.td_err = self.TD_ERR_DEF
 
         if not self.update_config(config):
             raise ValueError(f'{self.prefix}: Invalid config!')
 
-    @property
-    def with_weather(self) -> bool:
-        return self.config['weather']
+        self.t_next = self.last_update_tle + dt.timedelta(days=self.update_period)
 
-    @property
-    def fetch_elev(self) -> bool:
-        return self.config['elevation'] is None
+    @staticmethod
+    def calc_checksum(full_line: str):
+        checksum = 0
+        for c in full_line[:-1]:
+            if c.isnumeric():
+                checksum += int(c)
+            elif c == '-':
+                checksum += 1
+        return str(checksum)[-1]
+
+    def fill_objects(self, tle_f: pathlib.Path, t: dt.datetime):
+        if tle_f is None:
+            if t >= self.t_err:
+                self.t_err = t + self.td_err
+                self.td_err *= 2
+                self.log.error('TLE file failed')
+            return
 
-    @property
-    def lon(self) -> Union[int, float]:
-        return self.config['longitude']
+        objects = {}
 
-    @property
-    def lat(self) -> Union[int, float]:
-        return self.config['latitude']
+        with tle_f.open() as f:
+            for line in f:
+                names = set()
+                while 0 < len(line) <= 69:
+                    names.add(line.strip())
+                    line = f.readline()
 
-    @property
-    def elev(self) -> Union[int, float]:
-        return self.config['elevation'] or 0
+                try:
+                    names.add(int(line[2:7]))
+                except ValueError:
+                    if t >= self.t_err:
+                        self.t_err = t + self.td_err
+                        self.td_err *= 2
+                        self.log.error('Not TLE. Break')
+                    return
+
+                l1 = line.rstrip()
+                l2 = f.readline().rstrip()
+                for name in names:
+                    try:
+                        objects[name] = ephem.readtle(str(name), l1, l2), (str(name), l1, l2)
+                    except ValueError as e:
+                        if str(e).startswith('incorrect TLE checksum'):
+                            self.log.warning('%s: for `%s` expect %s:%s, got %s:%s',
+                                             e, name,
+                                             self.calc_checksum(l1), l1[-1],
+                                             self.calc_checksum(l2), l2[-1])
+                        else:
+                            raise e
+
+        self.objects = objects
+        shutil.move(tle_f, self.tle_file)
+        self.td_err = self.TD_ERR_DEF
+        self.t_err = t
 
-    @property
-    def lonlat(self) -> tuple[Union[int, float], Union[int, float]]:
-        return self.lon, self.lat
+        return 1
+
+    def fetch_tle(self, t: dt.datetime):
+        try:
+            x = urllib.request.urlretrieve(self.url)
+        except urllib.error.HTTPError as e:
+            if t >= self.t_err:
+                self.t_err = t + self.td_err
+                self.td_err *= 2
+                msg = f'Tle not fetched: {e}'
+                if e.code == 400:
+                    msg = f'{msg}: "{e.url}"'
+                self.log.error('%s', msg)
+            return
+        except (urllib.error.URLError, ValueError) as e:
+            if t >= self.t_err:
+                self.t_err = t + self.td_err
+                self.td_err *= 2
+                self.log.error('Tle not fetched: %s', e)
+            return
+
+        if self.fill_objects(x and pathlib.Path(x[0]) or None, t):
+            self.last_update_tle = t
+            self.log.info('Tle updated')
 
-    def update_config(self, config: Mapping) -> Optional[int]:
+        return 1
+
+    def update_config(self, config: Mapping):
         """
         :return: True if config update success
         """
 
-        if self.config != config:
+        if config != self.config:
             if not self._validate_config(config):
                 self.log.warning('invalid new config!')
                 return
 
             self.log.debug('reconf')
             self.config = config
 
-            self._observer = ephem.Observer()
-            self._observer.lat = str(self.lat)
-            self._observer.lon = str(self.lon)
-            self._observer.elev = self.elev
-            self._observer.compute_pressure()
+            fn = pathlib.Path(urllib.parse.urlparse(self.url).path).name
+            self.tle_file = pathlib.Path(TLEDIR / fn)
+            if self.tle_file.is_file():
+                self.last_update_tle = dt.datetime.fromtimestamp(self.tle_file.stat().st_mtime, dt.timezone.utc)
+            else:
+                if self.tle_file.is_dir():
+                    shutil.rmtree(self.tle_file, True)
+                else:
+                    self.tle_file.unlink(True)
+                self.tle_file.touch()
+                self.last_update_tle = dt.datetime.fromtimestamp(0, dt.timezone.utc)
+
+            self.fill_objects(self.tle_file, dt.datetime.now(dt.timezone.utc))
 
             return 1
 
     @staticmethod
     def _validate_config(config: Mapping) -> bool:
         return all(map(lambda x: x in config, [
-            'latitude',
-            'longitude',
-            'elevation',
-            'weather',
+            'url',
+            'update_period',
         ]))
 
-    def fetch_weather(self) -> Optional[int]:
-        q = urllib.parse.urlencode({
-            'latitude': self._observer.lat / ephem.degree,
-            'longitude': self._observer.lon / ephem.degree,
-            'hourly': 'temperature_2m,surface_pressure',
-            'current_weather': 'true',
-            'windspeed_unit': 'ms',
-            'start_date': dt.datetime.utcnow().date(),
-            'end_date': dt.datetime.utcnow().date(),
-        }, safe=',')
-
-        try:
-            with urllib.request.urlopen('https://api.open-meteo.com/v1/forecast?' + q) as r:
-                j = json.loads(r.read())
-        except urllib.error.HTTPError as e:
-            msg = f'Weather not fetched!\n{e}'
-            if e.code == 400:
-                msg = f'{msg}:\n"{e.url}"'
-            self.log.error('%s', msg)
-            return
-
-        self.last_weather_time = dt.datetime.fromisoformat(j['current_weather']['time']).replace(tzinfo=dt.timezone.utc)
-        self._observer.temp = float(j['current_weather']['temperature'])
-        if self.fetch_elev:
-            self._observer.elev = j.get('elevation', self._observer.elev)
-
-        press = None
-        for i, val in enumerate(j['hourly']['time']):
-            if dt.datetime.fromisoformat(val).replace(tzinfo=dt.timezone.utc) == self.last_weather_time:
-                try:
-                    press = float(j['hourly']['surface_pressure'][i])
-                except TypeError:
-                    pass
-                break
-        if press is None:
-            self._observer.compute_pressure()
-        else:
-            self._observer.pressure = press
+    @property
+    def url(self) -> str:
+        return self.config['url']
 
-        self.log.info('weather updated: %s°C %shPa', self._observer.temp, self._observer.pressure)
+    @property
+    def update_period(self) -> Union[int, float]:
+        """
+        Period of TLE update, days
+        """
 
-        return 1
+        return self.config['update_period']
 
-    def action(self, t: dt.datetime) -> Optional[int]:
-        self.set_date(t)
-        if self.with_weather and t >= self.t_next and self.fetch_weather():
-            self.t_next = self.last_weather_time + dt.timedelta(hours=self.update_period, minutes=1)
+    def action(self, t: dt.datetime):
+        if t >= self.t_next and self.fetch_tle(t):
+            self.t_next = self.last_update_tle + dt.timedelta(days=self.update_period)
             return 1
 
-    def next_pass(self,
-                  body: ephem.EarthSatellite,
-                  start_time: dt.datetime = None) -> tuple[dt.datetime, float,
-                                                           dt.datetime, float,
-                                                           dt.datetime, float]:
+    def get(self, name: str) -> Optional[tuple[ephem.EarthSatellite, tuple[str, str, str]]]:
         """
-        Calculate next pass of the `body` from `start_time`
+        Get TLE info by satellite name or NORAD number
 
-        :return: rise_t, rise_az, culm_t, culm_alt, set_t, set_az
+        :return: Tuple of EarthSatellite object and 3 lines of TLE. Or None
         """
 
-        o = self._observer.copy()
-        if start_time is not None:
-            o.date = start_time
+        return self.objects.get(name, None)
 
-        rise_t, rise_az, culm_t, culm_alt, set_t, set_az = o.next_pass(body, False)
+    def get_ephem(self, name: str) -> Optional[ephem.EarthSatellite]:
+        """
+        Get TLE object by satellite name or NORAD number
+        """
 
-        return (ephem.to_timezone(rise_t, dt.timezone.utc), rise_az / ephem.degree,
-                ephem.to_timezone(culm_t, dt.timezone.utc), culm_alt / ephem.degree,
-                ephem.to_timezone(set_t, dt.timezone.utc), set_az / ephem.degree)
+        x = self.objects.get(name, None)
+        return x and x[0]
 
-    def set_date(self, t: dt.datetime):
-        self._observer.date = t
+    def get_tle(self, name: str) -> Optional[tuple[str, str, str]]:
+        """
+        Get raw TLE lines by satellite name or NORAD number
+        """
 
-    def get_obj(self) -> ephem.Observer:
-        return self._observer
+        x = self.objects.get(name, None)
+        return x and x[1]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sats_receiver-0.1.19/sats_receiver/systems/apt.py` & `sats_receiver-0.1.76/sats_receiver/systems/apt.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import colorsys
 import datetime as dt
 import enum
 import logging
 import math
 import os
 import pathlib
 
@@ -11,15 +12,18 @@
 import ephem
 import numpy as np
 import scipy as sp
 import scipy.signal
 
 from PIL import Image, ImageDraw
 
-from sats_receiver import utils
+from sats_receiver import utils, SYSRESDIR
+
+
+APTRESDIR = SYSRESDIR / 'NOAA-APT'
 
 
 class AptChannel(enum.Enum):
     A = enum.auto()
     B = enum.auto()
 
 
@@ -108,24 +112,31 @@
     SPACE_B_START = SYNC_B_START + SYNC_WIDTH
     IMAGE_B_START = SPACE_B_START + SPACE_WIDTH
     TLM_B_START = IMAGE_B_START + IMAGE_WIDTH
 
     BLOCK_HEIGHT = 8
     BLOCKS_NUM = 16
     FRAME_HEIGHT = BLOCK_HEIGHT * BLOCKS_NUM
+    FRAME_HEIGHT_HF = FRAME_HEIGHT // 2
 
     SYNC_A = np.array([*map(float, '000011001100110011001100110011000000000')],
                       dtype=np.float32).repeat(PIX_WIDTH) * 2 - 1
     SYNC_B = np.array([*map(float, '000011100111001110011100111001110011100')],
                       dtype=np.float32).repeat(PIX_WIDTH) * 2 - 1
-    WEDGE_SAMPLE = np.array([*np.interp([31, 63, 95, 127, 159, 191, 223, 255, 0], [0, 255], [-1, 1]),
-                             0, 0, 0, 0, 0, 0, 0], dtype=np.float32).repeat(BLOCK_HEIGHT)
+    WEDGE_SAMPLE = np.array([*np.interp([31, 63, 95, 127, 159, 191, 223, 255, 0], [0, 255], [-1, 1])], dtype=np.float32).repeat(BLOCK_HEIGHT)
 
     # TODO: anoter values???
-    NOAA_AVHRR_FOV = 110.74
+    # The AVHRR/3 scans 55.4 deg per scan line on either side of the orbital track
+    # https://en.wikipedia.org/wiki/NOAA-15#Advanced_Very_High_Resolution_Radiometer_(AVHRR/3)
+    #
+    # Scanning is cross-track with a range of ±55.37 deg about nadir.
+    # https://nwp-saf.eumetsat.int/site/software/aapp/aapp-overview/avhrr-3/
+    # https://www.eumetsat.int/avhrr#nav-two
+    NOAA_AVHRR_FOV_HALF = 55.37
+    NOAA_AVHRR_FOV = NOAA_AVHRR_FOV_HALF * 2
 
     @classmethod
     def from_apt(cls, aptf: pathlib.Path) -> 'Apt':
         """
         APT file format:
             * 3 lines of TLE data
             * observer lonlat, 2 x double, degrees
@@ -134,15 +145,15 @@
         """
 
         with aptf.open('rb') as f:
             sat_name = f.readline().decode('ascii').rstrip()
             l1 = f.readline().decode('ascii').rstrip()
             l2 = f.readline().decode('ascii').rstrip()
             sat_tle = sat_name, l1, l2
-            observer_lonlat = [*np.frombuffer(f.read(np.dtype(np.double).itemsize * 2), dtype=np.double)]
+            observer_lonlat = tuple(np.frombuffer(f.read(np.dtype(np.double).itemsize * 2), dtype=np.double))
             end_time = np.frombuffer(f.read(np.dtype(np.double).itemsize), dtype=np.double)[0]
             data = np.fromfile(f, dtype=np.float32)
 
         x = cls(sat_name, aptf, None, None, sat_tle, observer_lonlat)
         x.data = np.resize(data, (data.size // cls.FRAME_WIDTH, cls.FRAME_WIDTH))
         x.end_time = dt.datetime.fromtimestamp(end_time, dateutil.tz.tzutc())
         x.synced = True
@@ -312,38 +323,70 @@
         self.end_time -= dt.timedelta(milliseconds=(tail_cutted + result_tail_cutted) * 500)
         self.data = result[0:result_end_pos, self.PIX_WIDTH // 2::self.PIX_WIDTH]
         self.synced = True
 
     def _read_telemetry(self):
         self.log.debug('read telemetry...')
 
-        if self.data.shape[0] < self.WEDGE_SAMPLE.size:
+        if self.data.shape[0] < self.FRAME_HEIGHT:
             self.log.error('recording too short for telemetry decoding')
             return 1
-        if self.data.shape[0] < self.WEDGE_SAMPLE.size * 2:
+        if self.data.shape[0] < self.FRAME_HEIGHT * 2:
             self.log.warning('reading telemetry on short recording, expect unreliable results')
 
         tlm_a = self.data[0:, self.TLM_A_START:self.SYNC_B_START]
         tlm_b = self.data[0:, self.TLM_B_START:]
 
         # search the best template with minimum noise
-        mean_a = np.mean(tlm_a, 1, dtype=np.float32)
-        mean_b = np.mean(tlm_b, 1, dtype=np.float32)
-        variance = (np.var(tlm_a, 1, dtype=np.float32)
-                    + np.var(tlm_b, 1, dtype=np.float32)) / 2
-        corr = np.correlate(mean_a, self.WEDGE_SAMPLE) + np.correlate(mean_b, self.WEDGE_SAMPLE)
-        qual = np.array([v / np.std(variance[i:i + self.WEDGE_SAMPLE.size], dtype=np.float32)
-                         for i, v in enumerate(corr)], dtype=np.float32)
-        best = np.argmax(qual)
+        mean_a = tlm_a.mean(1)
+        mean_b = tlm_b.mean(1)
+
+        variance_a = np.var(tlm_a, 1, dtype=np.float32)
+        variance_b = np.var(tlm_b, 1, dtype=np.float32)
+
+        corr_a = np.correlate(mean_a, self.WEDGE_SAMPLE)
+        corr_b = np.correlate(mean_b, self.WEDGE_SAMPLE)
+
+        qual_a = np.array([cor / np.std(variance_a[i + 7 * self.BLOCK_HEIGHT:i + self.FRAME_HEIGHT], dtype=np.float32)
+                           for i, cor in enumerate(corr_a - np.min(corr_a))
+                           if variance_a.size > i + (9 * self.BLOCK_HEIGHT)], dtype=np.float32)
+        qual_b = np.array([cor / np.std(variance_b[i + 7 * self.BLOCK_HEIGHT:i + self.FRAME_HEIGHT], dtype=np.float32)
+                           for i, cor in enumerate(corr_b - np.min(corr_b))
+                           if variance_b.size > i + (9 * self.BLOCK_HEIGHT)], dtype=np.float32)
+
+        best_q_a = np.argmax(qual_a)
+        best_q_b = np.argmax(qual_b)
+        x_a = best_q_a - self.FRAME_HEIGHT_HF
+        if x_a < 0:
+            best_qni_a = best_q_a
+            x_a = 0
+        else:
+            best_qni_a = self.FRAME_HEIGHT_HF
+        best_cqs_a = corr_a[x_a:best_q_a + self.FRAME_HEIGHT_HF]
+        x_a = best_q_b - self.FRAME_HEIGHT_HF
+        if x_a < 0:
+            best_qni_b = best_q_a
+            x_a = 0
+        else:
+            best_qni_b = self.FRAME_HEIGHT_HF
+        best_cqs_b = corr_b[x_a:best_q_b + self.FRAME_HEIGHT_HF]
+
+        if np.max(best_cqs_a) >= np.max(best_cqs_b):
+            best = best_q_a - best_qni_a + np.argmax(best_cqs_a)
+            mean = mean_a
+        else:
+            best = best_q_b - best_qni_b + np.argmax(best_cqs_b)
+            mean = mean_b
 
         # form the best telemetry data and create combine contrast values
-        tlm_a = np.reshape(mean_a[best:best + self.FRAME_HEIGHT], (-1, self.BLOCK_HEIGHT)).mean(1, dtype=np.float32)
-        tlm_b = np.reshape(mean_b[best:best + self.FRAME_HEIGHT], (-1, self.BLOCK_HEIGHT)).mean(1, dtype=np.float32)
-        clb = (tlm_a[:9] + tlm_b[:9]) / 2
-        hi, lo = clb[7:10]
+        tlm = mean[best:best + self.FRAME_HEIGHT]
+        tlm = np.resize(tlm, (tlm.size // self.BLOCK_HEIGHT, self.BLOCK_HEIGHT)).mean(1)
+
+        clb = tlm[:9]
+        hi, lo = clb[7:]
         rng = hi - lo
 
         if rng > 0:
             # image correction by contrast values
             self.data = (self.data - lo) / rng
         else:
             self.log.warning('invalid telemetry data, perhaps is too noisy')
@@ -375,15 +418,15 @@
         self._line_width = shapes.line_width * ss_factor
 
         start_time = self.end_time - self.LINE_DUR * height
         sat_positions = np.empty((height, 2), dtype=float)
         self._x_offsets = np.empty(height, dtype=float)
         x_fovs = np.empty(height, dtype=float)
 
-        a = math.radians(self.NOAA_AVHRR_FOV / 2)
+        a = math.radians(self.NOAA_AVHRR_FOV_HALF)
         b = math.pi / 2 - a
         sa = math.sin(a)
         for i in range(height):
             t = start_time + self.LINE_DUR * i
             self.sat_ephem.compute(t)
             sat_positions[i] = self.sat_ephem.sublong, self.sat_ephem.sublat
 
@@ -406,15 +449,16 @@
             if isinstance(points, dict):
                 if points['name'] == 'observer':
                     points['lonlat'] = np.radians(self.observer_lonlat)
                 self._draw_fig(points, ss_factor)
             else:
                 self._draw_lines(points, color)
 
-        self.map_overlay = np.array(overlay_img.resize((self.IMAGE_WIDTH, height), Image.Resampling.LANCZOS), dtype=np.uint8)
+        self.map_overlay = np.array(overlay_img.resize((self.IMAGE_WIDTH, height), Image.Resampling.LANCZOS),
+                                    dtype=np.uint8)
 
         del self._height
         del self._ss_height
         del self._half_ss_height
         del self._ss_width
         del self._half_ss_width
         del self._line_width
@@ -459,7 +503,47 @@
             self._draw.line(((x, y - llen), (x, y + llen)), fill=col, width=lwidth)
 
         elif fig['type'] == 'o':
             self._draw.ellipse(((x - sz, y - sz), (x + sz, y + sz)), fill=col)
 
     def black_overlay(self):
         return self.map_overlay * np.array([0, 0, 0, 1], dtype=np.uint8)
+
+    def create_composites(self, *types):
+        composites = {
+            'HVC': APTRESDIR / f'hvc-{self.sat_name[-2:]}.png',
+            'HVCT': APTRESDIR / f'hvct-{self.sat_name[-2:]}.png',
+            'NO': APTRESDIR / f'no-{self.sat_name[-2:]}.png',
+            'MSA': APTRESDIR / f'msa-{self.sat_name[-2:]}.png',
+            'SEA': APTRESDIR / f'sea-{self.sat_name[-2:]}.png',
+            'THRM': APTRESDIR / f'thermal-{self.sat_name[-2:]}.png',
+        }
+
+        data = (self.data * 255).clip(0, 255).astype(np.uint8)
+        ch_a: np.ndarray = data[:, self.IMAGE_A_START:self.TLM_A_START]
+        ch_b: np.ndarray = data[:, self.IMAGE_B_START:self.TLM_B_START]
+
+        results = []
+        for t in types:
+            if t[:-1] in ('HVC', 'HVCT', 'MSA', 'B') and t[-1] == 'P':
+                if t[0] == 'B':
+                    img = Image.fromarray(ch_b, 'L').convert('RGB')
+                else:
+                    lut = np.array(Image.open(composites[t[:-1]]), dtype=float) / 255.0
+                    img = Image.fromarray((lut[ch_b, ch_a] * 255).clip(0, 255).astype(np.uint8), 'RGB')
+
+                lut = np.array(Image.open(composites['NO']), dtype=float) / 255.0
+
+                for y, line in enumerate(lut):
+                    if abs(155 / 360 - colorsys.rgb_to_hsv(*line[0])[0]) < (8 / 255):
+                        break
+
+                img.paste(Image.fromarray((lut[ch_b, ch_a] * 255).clip(0, 255).astype(np.uint8), 'RGB'),
+                          mask=Image.fromarray((ch_b > y).astype(np.uint8) * 255, 'L'))
+
+                results.append((t, img))
+
+            else:
+                lut = np.array(Image.open(composites[t]), dtype=float) / 255.0
+                results.append((t, Image.fromarray((lut[ch_b, ch_a] * 255).clip(0, 255).astype(np.uint8), 'RGB')))
+
+        return results
```

### Comparing `sats_receiver-0.1.19/sats_receiver/systems/sstv.py` & `sats_receiver-0.1.76/sats_receiver/systems/sstv.py`

 * *Files 21% similar despite different names*

```diff
@@ -43,16 +43,14 @@
         self.sat_name = sat_name
         self.out_dir = out_dir
         self.srate = srate
         self.do_sync = do_sync
 
         self.line_len_fp = self.LINE_S * srate
         self.line_len = int(self.LINE_S * srate)
-        self.line = np.full(self.line_len, np.nan, np.float32)
-        self.line_rest_sz = self.line_len
 
         # horizontal sync
         self.sync_pix_width = int(srate * self.SYNC_PIX_S)
 
         self.img = None
         self.img_data_max_size = int(self.line_len_fp * (self.IMG_H + 1)) * np.float32().itemsize
         self.img_data_file = utils.mktmp2(mode='wb',
@@ -110,15 +108,15 @@
 
     def _sync_process(self, data: np.ndarray) -> np.ndarray:
         self.log.debug('syncing...')
 
         hsync_len = int(self.HSYNC_MS * self.sync_pix_width)
         line_len = self.line_len - hsync_len
 
-        sync_word = np.array([-1] * int(self.HSYNC_MS * self.sync_pix_width))
+        sync_word = np.array([-1] * hsync_len)
         corrs = np.correlate(data - np.mean(data), sync_word, 'valid')
         corrs_mean = np.mean(corrs)
         corrs_up = corrs > corrs_mean
 
         k = 0
         peaks = np.empty(self.IMG_H, int)
         for i in range(peaks.size):
@@ -261,14 +259,18 @@
     IMG_H = 256
 
 
 class MartinM2(_Martin):
     VIS = 0x28
 
     C_MS = _Martin.CSYNC_MS * 128
+    LINE_S = (_Martin.HSYNC_MS + _Martin.CSYNC_MS
+              + C_MS + _Martin.CSYNC_MS
+              + C_MS + _Martin.CSYNC_MS
+              + C_MS + _Martin.CSYNC_MS) / 1000
 
     IMG_W = 160
     IMG_H = 256
 
 
 class MartinM3(_Martin):
     VIS = 0x24
@@ -277,14 +279,18 @@
     IMG_H = 128
 
 
 class MartinM4(_Martin):
     VIS = 0x20
 
     C_MS = _Martin.CSYNC_MS * 128
+    LINE_S = (_Martin.HSYNC_MS + _Martin.CSYNC_MS
+              + C_MS + _Martin.CSYNC_MS
+              + C_MS + _Martin.CSYNC_MS
+              + C_MS + _Martin.CSYNC_MS) / 1000
 
     IMG_W = 160
     IMG_H = 128
 
 
 class _PD(Sstv):
     MODE = 'YCbCr'
@@ -374,20 +380,81 @@
     C_MS = 228.8
     LINE_S = (_PD.HSYNC_MS + _PD.HSYNC_GAP_MS + C_MS * 4) / 1000
 
     IMG_W = 800
     IMG_H = 616 // 2
 
 
+class _Scottie(Sstv):
+    MODE = 'RGB'
+
+    HSYNC_MS = 9.0
+    CSYNC_MS = 1.5
+    C_MS = 138.24
+    LINE_S = (CSYNC_MS + C_MS + CSYNC_MS + C_MS + HSYNC_MS + CSYNC_MS + C_MS) / 1000
+
+    IMG_W = 320
+    IMG_H = 256
+
+    def _image_process(self, data: np.ndarray) -> np.ndarray:
+        indices = [0]
+        for i in self.CSYNC_MS, self.C_MS, self.CSYNC_MS, self.C_MS, self.CSYNC_MS:
+            indices.append(indices[-1] + i)
+
+        indices = np.array(indices[1:]) / 1000
+        _, r, _, g, _, b = np.hsplit(data, (indices * self.srate).astype(int))
+        g = np.concatenate((np.zeros((1, g.shape[1]), dtype=g.dtype), g[:-1]), axis=0)
+        b = np.concatenate((np.zeros((1, b.shape[1]), dtype=b.dtype), b[:-1]), axis=0)
+
+        return np.dstack((
+            sp.signal.resample(r, self.IMG_W, axis=1),
+            sp.signal.resample(g, self.IMG_W, axis=1),
+            sp.signal.resample(b, self.IMG_W, axis=1)
+        ))
+
+
+class ScottieS1(_Scottie):
+    VIS = 0x3c
+
+
+class ScottieS2(_Scottie):
+    VIS = 0x38
+
+    C_MS = 88.064
+    LINE_S = (_Scottie.CSYNC_MS + C_MS + _Scottie.CSYNC_MS + C_MS + _Scottie.HSYNC_MS + _Scottie.CSYNC_MS + C_MS) / 1000
+
+
+class ScottieS3(ScottieS1):
+    VIS = 0x34
+
+    IMG_W = 160
+    IMG_H = 128
+
+
+class ScottieS4(ScottieS2):
+    VIS = 0x30
+
+    IMG_W = 160
+    IMG_H = 128
+
+
+class ScottieDX(_Scottie):
+    VIS = 0x4c
+
+    C_MS = 345.6
+    LINE_S = (_Scottie.CSYNC_MS + C_MS + _Scottie.CSYNC_MS + C_MS + _Scottie.HSYNC_MS + _Scottie.CSYNC_MS + C_MS) / 1000
+
+
 class SstvRecognizer:
     STATUS_OK = 0
     STATUS_CALIB_FAIL = 1
     STATUS_VIS_FAIL = 2
-    STATUS_FOUND = 3
-    STATUS_DONE = 4
+    STATUS_VIS_UNKNOWN = 3
+    STATUS_FOUND = 4
+    STATUS_DONE = 5
 
     _STATE_0 = 0
     _STATE_GET_PEAKS = 1
     _STATE_GET_HDR = 2
     _STATE_GET_VIS = 3
     _STATE_GET_LINE = 4
 
@@ -420,14 +487,19 @@
         PD50.VIS: PD50,
         PD90.VIS: PD90,
         PD120.VIS: PD120,
         PD160.VIS: PD160,
         PD180.VIS: PD180,
         PD240.VIS: PD240,
         PD290.VIS: PD290,
+        ScottieS1.VIS: ScottieS1,
+        ScottieS2.VIS: ScottieS2,
+        ScottieS3.VIS: ScottieS3,
+        ScottieS4.VIS: ScottieS4,
+        ScottieDX.VIS: ScottieDX,
     }
 
     def __init__(self,
                  sat_name: str,
                  out_dir: pathlib.Path,
                  srate: Union[int, float],
                  start_peak: int,
@@ -443,20 +515,20 @@
         self.state = self._STATE_GET_PEAKS
 
         # calibration header setup
         self.calib_leader_len = int(self.CALIB_LEADER_S * srate)
         self.calib_break_len = int(self.CALIB_BREAK_S * srate)
         self.calib_len = self.calib_leader_len * 2 + self.calib_break_len
         self.calib_hdr = np.full(self.calib_len, np.nan, np.float32)
-        self.calib_rest_sz = self.calib_len
+        self.calib_remained_sz = self.calib_len
 
         # vis code setup
         self.vis_len = int(self.VIS_S * srate)
         self.vis = np.full(self.vis_len, np.nan, np.float32)
-        self.vis_rest_sz = self.vis_len
+        self.vis_remained_sz = self.vis_len
         self.vis_code = 0
 
         self.sstv = None
 
     def feed(self, input_data: np.ndarray) -> int:
         data = input_data
         res = self.STATUS_OK
@@ -465,30 +537,30 @@
         if not self.state:
             return self.STATUS_DONE
 
         while data.size:
             if self.state == self._STATE_GET_PEAKS:
                 data = data[self.start_peak:]
                 self.calib_hdr.fill(np.nan)
-                self.calib_rest_sz = self.calib_len
+                self.calib_remained_sz = self.calib_len
                 self.vis.fill(np.nan)
-                self.vis_rest_sz = self.vis_len
+                self.vis_remained_sz = self.vis_len
                 self.state = self._STATE_GET_HDR
 
             elif self.state == self._STATE_GET_HDR:
                 if not np.isnan(np.amin(self.calib_hdr)):
                     self.calib_hdr.fill(np.nan)
-                    self.calib_rest_sz = self.calib_len
+                    self.calib_remained_sz = self.calib_len
                 i = np.argmin(self.calib_hdr)
-                x = data[:self.calib_rest_sz]
-                data = data[self.calib_rest_sz:]
+                x = data[:self.calib_remained_sz]
+                data = data[self.calib_remained_sz:]
                 self.calib_hdr[i:i + x.size] = x
-                self.calib_rest_sz -= x.size
+                self.calib_remained_sz -= x.size
 
-                if not self.calib_rest_sz:
+                if not self.calib_remained_sz:
                     # hdr is full. check it
                     leaders = np.append(
                         self.calib_hdr[:self.calib_leader_len],
                         self.calib_hdr[self.calib_leader_len + self.calib_break_len
                                        :self.calib_len - self.calib_break_len]
                     )
                     breaker = self.calib_hdr[self.calib_leader_len:self.calib_leader_len + self.calib_break_len]
@@ -502,43 +574,45 @@
                     else:
                         self.state = self._STATE_0
                         return self.STATUS_CALIB_FAIL
 
             elif self.state == self._STATE_GET_VIS:
                 if not np.isnan(np.amin(self.vis)):
                     self.vis.fill(np.nan)
-                    self.vis_rest_sz = self.vis_len
+                    self.vis_remained_sz = self.vis_len
                 i = np.argmin(self.vis)
-                x = data[:self.vis_rest_sz]
-                data = data[self.vis_rest_sz:]
+                x = data[:self.vis_remained_sz]
+                data = data[self.vis_remained_sz:]
                 self.vis[i:i + x.size] = x
-                self.vis_rest_sz -= x.size
+                self.vis_remained_sz -= x.size
 
-                if not self.vis_rest_sz:
+                if not self.vis_remained_sz:
                     # VIS is full. check it
                     vis = np.median(np.resize(self.vis, (10, self.vis_len // 10)), axis=1)
                     vis_bits = [int(bit < self._1200) for bit in vis[8:0:-1]]
 
                     code = 0
                     for bit in vis_bits[1:]:
                         code = (code << 1) | bit
 
                     # check parity
                     if sum(vis_bits[1:]) % 2 != vis_bits[0]:
-                        # print(f'VIS<0x{code:02x}> parity check failed')
+                        if code:
+                            self.log.debug('Parity failed VIS<0x%02x>', code)
                         self.state = self._STATE_0
                         return self.STATUS_VIS_FAIL
 
+                    self.vis_code = code
                     sstv = self.CODES.get(code)
                     if not sstv:
-                        # print(f'Unknown VIS<0x{code:02x}>')
+                        if code:
+                            self.log.debug('Unknown VIS<0x%02x>', code)
                         self.state = self._STATE_0
-                        return self.STATUS_VIS_FAIL
+                        return self.STATUS_VIS_UNKNOWN
 
-                    self.vis_code = code
                     self.sstv = sstv(sat_name=self.sat_name,
                                      out_dir=self.out_dir,
                                      srate=self.srate,
                                      do_sync=self.do_sync)
                     self.state = self._STATE_GET_LINE
                     res = self.STATUS_FOUND
```

### Comparing `sats_receiver-0.1.19/sats_receiver/utils.py` & `sats_receiver-0.1.76/sats_receiver/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,22 +31,25 @@
     RAW = 'RAW'
     AM = 'AM'
     FM = 'FM'
     WFM = 'WFM'
     WFM_STEREO = 'WFM_STEREO'
     QUAD = 'QUAD'
     QPSK = 'QPSK'
+    OQPSK = 'OQPSK'
+    GMSK = 'GMSK'
 
 
 class Decode(enum.Enum):
     RAW = 'RAW'
-    RSTREAM = 'RSTREAM'
+    CSOFT = 'CSOFT'
     APT = 'APT'
     LRPT = 'LRPT'
     SSTV = 'SSTV'
+    SATS = 'SATS'
 
 
 Event = collections.namedtuple('Event', 't, prior, seq, fn, a, kw')
 
 
 class Scheduler:
     """
@@ -56,15 +59,15 @@
     """
 
     def __init__(self):
         self._queue = []
         self._lock = threading.RLock()
         self._sequence_generator = itertools.count()
 
-    def plan(self, t: dt.datetime, fn: Callable, *a: Any, prior : int = 0, **kw: Any) -> Event:
+    def plan(self, t: dt.datetime, fn: Callable, *a: Any, prior: int = 0, **kw: Any) -> Event:
         with self._lock:
             event = Event(t, prior, next(self._sequence_generator), fn, a, kw)
             heapq.heappush(self._queue, event)
         return event
 
     def cancel(self, *evt: Event):
         if not evt:
@@ -108,15 +111,15 @@
             fn(*a, **kw)
             # time.sleep(0)
 
 
 class SysUsage:
     DEFAULT_INTV = 3600
 
-    def __init__(self, ctx: str, intv : Union[int, float] = DEFAULT_INTV):
+    def __init__(self, ctx: str, intv: Union[int, float] = DEFAULT_INTV):
         self.prefix = f'{self.__class__.__name__}: {ctx}'
         self.log = logging.getLogger(self.prefix)
         self.proc = psutil.Process()
 
         gc.set_debug(gc.DEBUG_UNCOLLECTABLE)
         self.now = 0
         self.intv = intv
```

### Comparing `sats_receiver-0.1.19/sats_receiver.egg-info/PKG-INFO` & `sats_receiver-0.1.76/sats_receiver.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sats-receiver
-Version: 0.1.19
+Version: 0.1.76
 Summary: Satellites data receiver based on GNU Radio
 Home-page: https://github.com/baskiton/sats-receiver
 Author: Alexander Baskikh
 Author-email: baskiton@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/baskiton/sats-receiver/issues
 Classifier: License :: OSI Approved :: MIT License
@@ -31,25 +31,26 @@
 
 Satellites data receiver based on GNURadio
 
 <!-- TOC -->
 * [About](#About)
 * [Requirements](#Requirements)
 * [Installation](#Installation)
-  * [Linux](#Linux)
-  * [Windows](#Windows)
+  * [From source](#From-source)
+  * [From PYPI](#From-PYPI)
 * [Usage](#Usage)
 * [Configure](#Configure)
   * [observer](#observer)
   * [tle](#tle)
   * [receivers](#receivers)
     * [sats](#sats)
       * [frequencies](#frequencies)
         * [modulations](#modulations)
         * [decoders](#decoders)
+          * [gr-satellites](#gr-satellites)
 * [Map Shapes](#Map-Shapes)
   * [shapes](#shapes)
   * [points](#points)
 <!-- TOC -->
 
 
 
@@ -69,36 +70,41 @@
 ### Requirements
 The program has only been tested on Linux. Work on Windows is not guaranteed!
 * Python>=3.10 (or lower, see below)
 * GNURadio>=3.10 (or lower if gr-soapy installed); GUI-modules is not required
 * librtlsdr (if you use RTL-SDR)
 
 ### Installation
-First [install gnuradio](https://wiki.gnuradio.org/index.php?title=InstallingGR)
+I recommended to use miniconda. So, first of all,
+[install it.](https://docs.conda.io/en/latest/miniconda.html#linux-installers)
 
-#### Linux
-  If you need a virtual environment (recommended), you need to create it
-  with the `--system-site-packages` option
-  ```
-  python3 -m venv --system-site-packages venv
-  source venv/bin/activate
-  pip install sats-receiver
-  ```
-
-#### Windows
-  After install `radioconda`, launch a terminal by running "Conda Prompt"
-  in the "radioconda" directory in the Start menu and type
-  ```
-  pip install sats-receiver
-  ```
+#### From source
+```commandline
+cd sats-receiver
+conda create -n sats-receiver-env
+conda activate sats-receiver-env
+conda config --env --add channels conda-forge
+conda config --env --set channel_priority strict
+conda env update -f environment.yml
+pip install -r requirements.txt
+```
+
+#### From PYPI
+```commandline
+conda create -n sats-receiver-env python
+conda activate sats-receiver-env
+conda config --env --add channels conda-forge
+conda config --env --set channel_priority strict
+conda install gnuradio gnuradio-satellites
+pip install sats-receiver
+```
 
 ### Usage
-* in Linux if a virtual environment has been created:  
-  `source venv/bin/activate`
-* in Windows launch "Conda Prompt" terminal
+First, activate conda environment:  
+`conda activate sats-receiver-env`
 
 `python -u -m sats_receiver [-h, --help] [--log LOG] [--sysu SYSU] config`  
 * `config` Config file path. See [Configure](#Configure)
 * `-h, --help` Help message
 * `--log LOG` Logging level, INFO default
 * `--sysu SYSU` System Usages debug info timeout in seconds, 1 hour default
 
@@ -152,14 +158,15 @@
 | samp_rate        | Number          | Receiver sample rate, Hz                                                                                                                                                           |
 | output_directory | String          | Directory to save received files. You also might specify `~` symbol to specify User home directory                                                                                 |
 | sats             | Array of Object | List of Satellites configurations (see [sats](#sats))                                                                                                                              |
 | enabled          | Boolean         | _Optional._ Enable or Disable this Receiver. `true` by default                                                                                                                     |
 | serial           | String          | _Optional._ Serial number of the receiver. Empty by default                                                                                                                        |
 | biast            | Boolean         | _Optional._ Bias-T enable/disable (only for RTL-SDR at this time). `false` by default. **WARNING! Be careful when enabling this option! Use only if you know what it is and why!** |
 | gain             | Boolean         | _Optional._ Receiver gain, dB. `0` by default                                                                                                                                      |
+| freq_correction  | Number          | _Optional._ Receiver frequency correction. `0.0` by default                                                                                                                        |
 
 
 #### sats
 Each satellite object contain:
 
 | Field         | Type            | Description                                                                                                |
 |:--------------|:----------------|:-----------------------------------------------------------------------------------------------------------|
@@ -169,60 +176,75 @@
 | min_elevation | Number          | _Optional._ Elevation angle above the horizon, degrees. `0` by default. Negative number is equivalent to 0 |
 | doppler       | Boolean         | _Optional._ Enable/Disable doppler correction. `true` by default                                           |
 
 
 #### frequencies
 Each frequency object contain:
 
-| Field           | Type    | Description                                                                       |
-|:----------------|:--------|:----------------------------------------------------------------------------------|
-| freq            | Number  | Basic signal frequency, Hz                                                        |
-| bandwidth       | Number  | Received signal bandwidth, Hz                                                     |
-| enabled         | Boolean | _Optional._ Enable/Disable this frequency. `true` by default                      |
-| freq_correction | Boolean | _Optional._ Correction for basic frequency, Hz. `0` by default                    |
-| mode            | String  | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default |
-| decode          | String  | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default          |
-| qpsk_baudrate   | Number  | _Required only for **QPSK** mode._ QPSK Baudrate, bps                             |
-| qpsk_excess_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Excess bandwidth. `0.35` by default      |
-| qpsk_ntaps      | Integer | _Optional. Only for **QPSK** mode._ QPSK number of taps. `33` by default          |
-| qpsk_costas_bw  | Number  | _Optional. Only for **QPSK** mode._ QPSK Costas bandwidth. `0.005` by default     |
-| sstv_wsr        | Number  | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default   |
-| sstv_sync       | Number  | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default            |
+| Field           | Type            | Description                                                                            |
+|:----------------|:----------------|:---------------------------------------------------------------------------------------|
+| freq            | Number          | Basic signal frequency, Hz                                                             |
+| bandwidth       | Number          | Received signal bandwidth, Hz                                                          |
+| enabled         | Boolean         | _Optional._ Enable/Disable this frequency. `true` by default                           |
+| subname         | String          | _Optional._ Subname added to result filename. Empty by default                         |
+| freq_correction | Boolean         | _Optional._ Correction for basic frequency, Hz. `0` by default                         |
+| mode            | String          | _Optional._ Modulation option (see [modulations](#modulations)). `RAW` by default      |
+| decode          | String          | _Optional._ Decoder option (see [decoders](#decoders)). `RAW` by default               |
+| channels        | Array of Number | _Required only for **GMSK** mode._ Demodulation baudrates, bps                         |
+| grs_file        | String          | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_name        | String          | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_norad       | Integer         | _Optional. Only for **SATS** decoder._ See [gr-satellites](#gr-satellites) for details |
+| grs_tlm_decode  | Boolean         | _Optional. Only for **SATS** decoder._ Save decoded telemetry. `true` by default       |
+| qpsk_baudrate   | Number          | _Required only for **(O)QPSK** mode._ (O)QPSK Baudrate, bps                            |
+| qpsk_excess_bw  | Number          | _Optional. Only for **(O)QPSK** mode._ (O)QPSK Excess bandwidth. `0.35` by default     |
+| qpsk_ntaps      | Integer         | _Optional. Only for **(O)QPSK** mode._ (O)QPSK number of taps. `33` by default         |
+| qpsk_costas_bw  | Number          | _Optional. Only for **(O)QPSK** mode._ (O)QPSK Costas bandwidth. `0.005` by default    |
+| sstv_wsr        | Number          | _Optional. Only for **SSTV** decoder._ SSTV work samplerate. `16000` by default        |
+| sstv_sync       | Number          | _Optional. Only for **SSTV** decoder._ SSTV syncing. `true` by default                 |
 
 
 #### modulations
 * `RAW`
 * `AM`
 * `FM`
 * `WFM`
 * `WFM_STEREO`
 * `QUAD`
 * `QPSK`
+* `OQPSK`
+* `GMSK`
 
 #### decoders
 * `RAW` Saved to 2-channel float32 WAV file with `bandwidth` sample rate
-* `RSTREAM` Raw Stream - binary int8. Suitable for further processing, for example, in SatDump
-* `APT` sats-receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
+* `CSOFT` Constellation Soft Decoder - 1-channel binary int8. Suitable for further processing, for example, in SatDump
+* `APT` Sats-Receiver APT binary file format. See [APT](sats_receiver/systems/README.md#APT)
 * `SSTV` SSTV saved to PNG image with EXIF. Supported modes:
-  * `Robot24`
-  * `Robot36`
-  * `Robot72`
-  * `MartinM1`
-  * `MartinM2`
-  * `MartinM3`
-  * `MartinM4`
-  * `PD50`
-  * `PD90`
-  * `PD120`
-  * `PD160`
-  * `PD180`
-  * `PD240`
-  * `PD290`
+  * Robot (24, 24, 72)
+  * Martin (M1, M2, M3, M4)
+  * PD (50, 90, 120, 160, 180, 240, 290)
+  * Scottie (S1, S2, S3, S4)
+* `SATS` See [gr-satellites](#gr-satellites) for details
 * ~~`LRPT`~~ Not implemented yet
 
+##### gr-satellites
+See [gr-satellites Documentation][grs-doc]  
+**IMPORTANT:** For this decoder need to leave the `modulation` on `RAW`  
+
+This decoder need to specify one of the parameters for recognize satellite option:
+* grs_file - Path to your own [SatYAML-file][grs-satyaml]
+* grs_name - Satellite name (may different from [sats name](#sats))
+* grs_norad - Satellite NORAD ID
+
+[List of builtin supported satellites][grs-satlist]  
+Additionally supported satellites can be found in the [satyaml](satyaml) directory of this repository
+
+[grs-doc]: https://gr-satellites.readthedocs.io/en/latest/
+[grs-satyaml]: https://gr-satellites.readthedocs.io/en/latest/satyaml.html
+[grs-satlist]: https://gr-satellites.readthedocs.io/en/latest/supported_satellites.html
+
 
 ### Map Shapes
 Map shapes config file `map_shapes.json` can be found at the root of this repository.
 Shapefiles can be downloaded from [Natural Earth](https://www.naturalearthdata.com/downloads/)
 
 | Field      | Type             | Description                                                                        |
 |:-----------|:-----------------|:-----------------------------------------------------------------------------------|
```

### Comparing `sats_receiver-0.1.19/sats_receiver.egg-info/SOURCES.txt` & `sats_receiver-0.1.76/sats_receiver.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -21,11 +21,19 @@
 sats_receiver/gr_modules/receiver.py
 sats_receiver/gr_modules/epb/__init__.py
 sats_receiver/gr_modules/epb/prober.py
 sats_receiver/gr_modules/epb/sstv.py
 sats_receiver/systems/__init__.py
 sats_receiver/systems/apt.py
 sats_receiver/systems/sstv.py
+sats_receiver/systems/satellites/__init__.py
+sats_receiver/systems/satellites/demodulators/__init__.py
+sats_receiver/systems/satellites/filereceivers/__init__.py
+sats_receiver/systems/satellites/filereceivers/geoscan.py
+sats_receiver/systems/satellites/telemetry/__init__.py
+sats_receiver/systems/satellites/telemetry/geoscan_tlm.py
+sats_receiver/systems/satellites/telemetry/usp_tlm.py
 tests/__init__.py
 tests/test_async_signal.py
 tests/test_decoders.py
+tests/test_demodulators.py
 tests/test_utils.py
```

### Comparing `sats_receiver-0.1.19/tests/test_async_signal.py` & `sats_receiver-0.1.76/tests/test_async_signal.py`

 * *Files identical despite different names*

### Comparing `sats_receiver-0.1.19/tests/test_utils.py` & `sats_receiver-0.1.76/tests/test_utils.py`

 * *Files identical despite different names*

