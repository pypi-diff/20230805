# Comparing `tmp/mpcrl-1.1.5.dev1.tar.gz` & `tmp/mpcrl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpcrl-1.1.5.dev1.tar", last modified: Sat Aug  5 07:19:18 2023, max compression
+gzip compressed data, was "mpcrl-1.2.0.tar", last modified: Sat Aug  5 07:13:04 2023, max compression
```

## Comparing `mpcrl-1.1.5.dev1.tar` & `mpcrl-1.2.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.882700 mpcrl-1.1.5.dev1/
--rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.1.5.dev1/LICENSE
--rw-rw-rw-   0        0        0     5684 2023-08-05 07:19:18.882700 mpcrl-1.1.5.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     4907 2023-08-05 07:13:28.000000 mpcrl-1.1.5.dev1/README.md
--rw-rw-rw-   0        0        0     1102 2023-08-05 07:13:28.000000 mpcrl-1.1.5.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-08-05 07:19:18.882700 mpcrl-1.1.5.dev1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.780696 mpcrl-1.1.5.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.801050 mpcrl-1.1.5.dev1/src/mpcrl/
--rw-rw-rw-   0        0        0     1221 2023-06-26 12:31:21.000000 mpcrl-1.1.5.dev1/src/mpcrl/__init__.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.821656 mpcrl-1.1.5.dev1/src/mpcrl/agents/
--rw-rw-rw-   0        0        0    17981 2023-08-05 07:13:28.000000 mpcrl-1.1.5.dev1/src/mpcrl/agents/agent.py
--rw-rw-rw-   0        0        0    12653 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/agents/learning_agent.py
--rw-rw-rw-   0        0        0    18946 2023-08-04 18:21:56.000000 mpcrl-1.1.5.dev1/src/mpcrl/agents/lstd_dpg.py
--rw-rw-rw-   0        0        0    13057 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/agents/lstd_q_learning.py
--rw-rw-rw-   0        0        0     9309 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/agents/rl_learning_agent.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.839963 mpcrl-1.1.5.dev1/src/mpcrl/core/
--rw-rw-rw-   0        0        0     9093 2023-08-04 18:02:18.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/callbacks.py
--rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/errors.py
--rw-rw-rw-   0        0        0     3337 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/experience.py
--rw-rw-rw-   0        0        0    12682 2023-08-04 18:11:55.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/exploration.py
--rw-rw-rw-   0        0        0     2710 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/learning_rate.py
--rw-rw-rw-   0        0        0    12059 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/parameters.py
--rw-rw-rw-   0        0        0     4999 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/schedulers.py
--rw-rw-rw-   0        0        0     2513 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/core/update.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.841993 mpcrl-1.1.5.dev1/src/mpcrl/util/
--rw-rw-rw-   0        0        0     2785 2023-08-04 18:02:18.000000 mpcrl-1.1.5.dev1/src/mpcrl/util/control.py
--rw-rw-rw-   0        0        0      791 2023-08-04 18:06:38.000000 mpcrl-1.1.5.dev1/src/mpcrl/util/iters.py
--rw-rw-rw-   0        0        0     4918 2023-08-04 18:11:49.000000 mpcrl-1.1.5.dev1/src/mpcrl/util/math.py
--rw-rw-rw-   0        0        0      911 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/util/named.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.790760 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.852091 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/
--rw-rw-rw-   0        0        0      243 2023-01-18 07:53:19.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/__init__.py
--rw-rw-rw-   0        0        0     7572 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/log.py
--rw-rw-rw-   0        0        0     1287 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/record_updates.py
--rw-rw-rw-   0        0        0     2928 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/wrapper.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.862203 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/envs/
--rw-rw-rw-   0        0        0      175 2023-01-23 17:35:23.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/envs/__init__.py
--rw-rw-rw-   0        0        0     3810 2023-08-04 18:11:48.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/envs/monitor_episodes.py
--rw-rw-rw-   0        0        0     4911 2023-08-04 18:11:49.000000 mpcrl-1.1.5.dev1/src/mpcrl/wrappers/envs/monitor_infos.py
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.811219 mpcrl-1.1.5.dev1/src/mpcrl.egg-info/
--rw-rw-rw-   0        0        0     5684 2023-08-05 07:19:18.000000 mpcrl-1.1.5.dev1/src/mpcrl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1118 2023-08-05 07:19:18.000000 mpcrl-1.1.5.dev1/src/mpcrl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-05 07:19:18.000000 mpcrl-1.1.5.dev1/src/mpcrl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       89 2023-08-05 07:19:18.000000 mpcrl-1.1.5.dev1/src/mpcrl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-08-05 07:19:18.000000 mpcrl-1.1.5.dev1/src/mpcrl.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-08-05 07:19:18.880565 mpcrl-1.1.5.dev1/tests/
--rw-rw-rw-   0        0        0    15094 2023-08-04 18:06:43.000000 mpcrl-1.1.5.dev1/tests/test_agent.py
--rw-rw-rw-   0        0        0    21702 2023-08-04 18:11:56.000000 mpcrl-1.1.5.dev1/tests/test_core.py
--rw-rw-rw-   0        0        0    11663 2023-08-04 18:04:32.000000 mpcrl-1.1.5.dev1/tests/test_examples.py
--rw-rw-rw-   0        0        0    49977 2023-08-04 18:02:18.000000 mpcrl-1.1.5.dev1/tests/test_quadrotor_q_learning.py
--rw-rw-rw-   0        0        0     4243 2023-08-04 18:06:38.000000 mpcrl-1.1.5.dev1/tests/test_util.py
--rw-rw-rw-   0        0        0     8417 2023-08-04 18:02:18.000000 mpcrl-1.1.5.dev1/tests/test_wrappers.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.477562 mpcrl-1.2.0/
+-rw-rw-rw-   0        0        0     1093 2022-11-28 16:28:05.000000 mpcrl-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0     5687 2023-08-05 07:13:04.476606 mpcrl-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4915 2023-08-05 07:12:33.000000 mpcrl-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1091 2023-08-05 07:12:24.000000 mpcrl-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-08-05 07:13:04.479555 mpcrl-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.419658 mpcrl-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.428683 mpcrl-1.2.0/src/mpcrl/
+-rw-rw-rw-   0        0        0     1221 2023-06-26 12:31:21.000000 mpcrl-1.2.0/src/mpcrl/__init__.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.440696 mpcrl-1.2.0/src/mpcrl/agents/
+-rw-rw-rw-   0        0        0    21492 2023-08-05 07:12:24.000000 mpcrl-1.2.0/src/mpcrl/agents/agent.py
+-rw-rw-rw-   0        0        0    12653 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/agents/learning_agent.py
+-rw-rw-rw-   0        0        0    18946 2023-08-04 18:21:56.000000 mpcrl-1.2.0/src/mpcrl/agents/lstd_dpg.py
+-rw-rw-rw-   0        0        0    13057 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/agents/lstd_q_learning.py
+-rw-rw-rw-   0        0        0     9309 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/agents/rl_learning_agent.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.451650 mpcrl-1.2.0/src/mpcrl/core/
+-rw-rw-rw-   0        0        0     9093 2023-08-04 18:02:18.000000 mpcrl-1.2.0/src/mpcrl/core/callbacks.py
+-rw-rw-rw-   0        0        0     1609 2023-01-07 11:39:22.000000 mpcrl-1.2.0/src/mpcrl/core/errors.py
+-rw-rw-rw-   0        0        0     3337 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/core/experience.py
+-rw-rw-rw-   0        0        0    12682 2023-08-04 18:11:55.000000 mpcrl-1.2.0/src/mpcrl/core/exploration.py
+-rw-rw-rw-   0        0        0     2710 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/core/learning_rate.py
+-rw-rw-rw-   0        0        0    12059 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/core/parameters.py
+-rw-rw-rw-   0        0        0     4999 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/core/schedulers.py
+-rw-rw-rw-   0        0        0     2513 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/core/update.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.456633 mpcrl-1.2.0/src/mpcrl/util/
+-rw-rw-rw-   0        0        0     2785 2023-08-04 18:02:18.000000 mpcrl-1.2.0/src/mpcrl/util/control.py
+-rw-rw-rw-   0        0        0      791 2023-08-04 18:06:38.000000 mpcrl-1.2.0/src/mpcrl/util/iters.py
+-rw-rw-rw-   0        0        0     4918 2023-08-04 18:11:49.000000 mpcrl-1.2.0/src/mpcrl/util/math.py
+-rw-rw-rw-   0        0        0      911 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/util/named.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.423650 mpcrl-1.2.0/src/mpcrl/wrappers/
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.463608 mpcrl-1.2.0/src/mpcrl/wrappers/agents/
+-rw-rw-rw-   0        0        0      243 2023-01-18 07:53:19.000000 mpcrl-1.2.0/src/mpcrl/wrappers/agents/__init__.py
+-rw-rw-rw-   0        0        0     7572 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/wrappers/agents/log.py
+-rw-rw-rw-   0        0        0     1287 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/wrappers/agents/record_updates.py
+-rw-rw-rw-   0        0        0     2928 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/wrappers/agents/wrapper.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.467595 mpcrl-1.2.0/src/mpcrl/wrappers/envs/
+-rw-rw-rw-   0        0        0      175 2023-01-23 17:35:23.000000 mpcrl-1.2.0/src/mpcrl/wrappers/envs/__init__.py
+-rw-rw-rw-   0        0        0     3810 2023-08-04 18:11:48.000000 mpcrl-1.2.0/src/mpcrl/wrappers/envs/monitor_episodes.py
+-rw-rw-rw-   0        0        0     4911 2023-08-04 18:11:49.000000 mpcrl-1.2.0/src/mpcrl/wrappers/envs/monitor_infos.py
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.434705 mpcrl-1.2.0/src/mpcrl.egg-info/
+-rw-rw-rw-   0        0        0     5687 2023-08-05 07:13:04.000000 mpcrl-1.2.0/src/mpcrl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1118 2023-08-05 07:13:04.000000 mpcrl-1.2.0/src/mpcrl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-05 07:13:04.000000 mpcrl-1.2.0/src/mpcrl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-08-05 07:13:04.000000 mpcrl-1.2.0/src/mpcrl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-08-05 07:13:04.000000 mpcrl-1.2.0/src/mpcrl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-08-05 07:13:04.475569 mpcrl-1.2.0/tests/
+-rw-rw-rw-   0        0        0    15094 2023-08-04 18:06:43.000000 mpcrl-1.2.0/tests/test_agent.py
+-rw-rw-rw-   0        0        0    21702 2023-08-04 18:11:56.000000 mpcrl-1.2.0/tests/test_core.py
+-rw-rw-rw-   0        0        0    11663 2023-08-04 18:04:32.000000 mpcrl-1.2.0/tests/test_examples.py
+-rw-rw-rw-   0        0        0    49977 2023-08-04 18:02:18.000000 mpcrl-1.2.0/tests/test_quadrotor_q_learning.py
+-rw-rw-rw-   0        0        0     4243 2023-08-04 18:06:38.000000 mpcrl-1.2.0/tests/test_util.py
+-rw-rw-rw-   0        0        0     8417 2023-08-04 18:02:18.000000 mpcrl-1.2.0/tests/test_wrappers.py
```

### Comparing `mpcrl-1.1.5.dev1/LICENSE` & `mpcrl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/PKG-INFO` & `mpcrl-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.1.5.dev1
+Version: 1.2.0
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,15 +20,15 @@
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
 
 [![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
 [![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
 ![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
 
-[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml)
+[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
 [![Downloads](https://pepy.tech/badge/mpcrl)](https://pepy.tech/project/mpcrl)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
```

### Comparing `mpcrl-1.1.5.dev1/README.md` & `mpcrl-1.2.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
 
 [![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
 [![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
 ![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
 
-[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml)
+[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
 [![Downloads](https://pepy.tech/badge/mpcrl)](https://pepy.tech/project/mpcrl)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
```

### Comparing `mpcrl-1.1.5.dev1/pyproject.toml` & `mpcrl-1.2.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=67.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpcrl"
-version = "1.1.5.dev1"
+version = "1.2.0"
 authors = [
   { name="Filippo Airaldi", email="filippoairaldi@gmail.com" },
 ]
 description = "Reinforcement Learning with Model Predictive Control"
 readme = "README.md"
 requires-python = ">=3.9"
 license = { text = "MIT" }
@@ -19,17 +19,17 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering :: Mathematics"
 ]
 dependencies = [
     "typing_extensions >= 4.5.0",
     "numba >= 0.57.1",
-    "csnlp >= 1.5.7.dev1",
+    "csnlp >= 1.5.7",
     "scipy >= 1.11.0",
-    "gymnasium >= 0.28.1",
+    "gymnasium >= 0.28.1"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning"
 "Bug Tracker" = "https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues"
 
 [tool.setuptools]
```

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/__init__.py` & `mpcrl-1.2.0/src/mpcrl/__init__.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/agents/agent.py` & `mpcrl-1.2.0/src/mpcrl/agents/agent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import warnings
+from itertools import chain
 from typing import (
     Any,
     Collection,
     Generic,
     Iterable,
     Iterator,
     Literal,
@@ -11,14 +13,15 @@
     Union,
 )
 
 import casadi as cs
 import numpy as np
 import numpy.typing as npt
 from csnlp import Solution, wrappers
+from csnlp.core.cache import invalidate_caches_of
 from csnlp.util.io import SupportsDeepcopyAndPickle
 from csnlp.wrappers import Mpc
 from gymnasium import Env
 from typing_extensions import TypeAlias
 
 from mpcrl.core.callbacks import AgentCallbacks, RemovesCallbackHooksInState
 from mpcrl.core.exploration import ExplorationStrategy, NoExploration
@@ -99,14 +102,15 @@
         SupportsDeepcopyAndPickle.__init__(self)
         AgentCallbacks.__init__(self)
         RemovesCallbackHooksInState.__init__(self)
         self._V, self._Q = self._setup_V_and_Q(mpc)
         self._fixed_pars = fixed_parameters
         self._exploration: ExplorationStrategy = NoExploration()
         self._store_last_successful = warmstart == "last-successful"
+        self._post_setup_V_and_Q()
 
     @property
     def unwrapped(self) -> "Agent":
         """Gets the underlying wrapped instance of an agent."""
         return self
 
     def is_wrapped(self, *args: Any, **kwargs: Any) -> bool:
@@ -382,29 +386,98 @@
     def _setup_V_and_Q(self, mpc: Mpc[SymType]) -> tuple[Mpc[SymType], Mpc[SymType]]:
         """Internal utility to setup the function approximators for the value function
         V(s) and the quality function Q(s,a)."""
         na = mpc.na
         if na <= 0:
             raise ValueError(f"Expected Mpc with na>0; got na={na} instead.")
 
+        # create V and Q function approximations
         V, Q = mpc, mpc.copy()
         V.unwrapped.name += "_V"
         Q.unwrapped.name += "_Q"
         a0 = Q.nlp.parameter(self.init_action_parameter, (na, 1))
         perturbation = V.nlp.parameter(self.cost_perturbation_parameter, (na, 1))
 
         u0 = cs.vcat(mpc.first_actions.values())
         f = V.nlp.f
         if mpc.is_wrapped(wrappers.NlpScaling):
             f = mpc.scale(f)
 
         V.nlp.minimize(f + cs.dot(perturbation, u0))
         Q.nlp.constraint(self.init_action_constraint, u0, "==", a0)
+
+        # remove upper/lower bound on initial action in Q, since it is constrained as a0
+        for n, a in mpc.first_actions.items():
+            Q.nlp.remove_variable_bounds(n, "both", ((r, 0) for r in range(a.size1())))
+
+        # invalidate caches for V and Q since some modifications have been done
+        for nlp in (V, Q):
+            nlp_ = nlp
+            while nlp_ is not nlp_.unwrapped:
+                invalidate_caches_of(nlp_)
+                nlp_ = nlp_.nlp
+            invalidate_caches_of(nlp_.unwrapped)
         return V, Q
 
+    def _post_setup_V_and_Q(self) -> None:
+        """Internal utility that is run after the creation of V and Q, allowing for
+        further customization in inheriting classes."""
+        # warn user of any constraints that linearly includes x0 and u0 (aside from
+        # x(0)==s0 and u(0)==a0), which may thus lead to LICQ-failure
+        # - u0 in Q should only appear in the 1st dynamics constraint and a0 con
+        # - u0 in V should only appear in the 1st dynamics constraint and lbx/ubx
+        # - x0 in V, Q should only appear in the 1st dynamics constraint and s0 con
+        for mpc in (self._V, self._Q):
+            name = mpc.unwrapped.name[-1]
+            u0 = cs.vcat(self._V.first_actions.values())
+            x0 = cs.vvcat(self._V.first_states.values())
+            con = cs.vertcat(mpc.g, mpc.h, mpc.h_lbx, mpc.h_ubx)
+
+            if mpc.unwrapped.sym_type.__name__ == "SX":
+                nnz_con_u0 = len(set(cs.jacobian_sparsity(con, u0).get_triplet()[0]))
+                nnz_con_x0 = len(set(cs.jacobian_sparsity(con, x0).get_triplet()[0]))
+            else:
+                nnz_con_u0 = len(  # computes the same as above, but for MX
+                    set(
+                        chain.from_iterable(
+                            cs.jacobian(con, a)[:, : a.size1()]
+                            .sparsity()
+                            .get_triplet()[0]
+                            for a in mpc.actions.values()
+                        )
+                    )
+                )
+                nnz_con_x0 = len(
+                    set(
+                        chain.from_iterable(
+                            cs.jacobian(con, s)[:, : s.size1()]
+                            .sparsity()
+                            .get_triplet()[0]
+                            for s in mpc.states.values()
+                        )
+                    )
+                )
+
+            nnz_exp_u0 = mpc.ns + (mpc.na * 2 if name == "V" else mpc.na)
+            if nnz_con_u0 > nnz_exp_u0:
+                warnings.warn(
+                    f"detected {nnz_con_u0} (expected {nnz_exp_u0}) constraints on "
+                    f"initial actions in {name}; make sure that the initial action is "
+                    "not overconstrained (LICQ may be compromised).",
+                    RuntimeWarning,
+                )
+            nnz_exp_x0 = mpc.ns * 2
+            if nnz_con_x0 > nnz_exp_x0:
+                warnings.warn(
+                    f"detected {nnz_con_x0} (expected {nnz_exp_x0}) constraints on "
+                    f"initial states in {name}; make sure that the initial state is "
+                    "not overconstrained (LICQ may be compromised).",
+                    RuntimeWarning,
+                )
+
     def _get_parameters(
         self,
     ) -> Union[None, dict[str, npt.ArrayLike], Collection[dict[str, npt.ArrayLike]]]:
         """Internal utility to retrieve parameters of the MPC in order to solve it.
         `Agent` has no learnable parameter, so only fixed parameters are returned."""
         return self._fixed_pars
```

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/agents/learning_agent.py` & `mpcrl-1.2.0/src/mpcrl/agents/learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/agents/lstd_dpg.py` & `mpcrl-1.2.0/src/mpcrl/agents/lstd_dpg.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/agents/lstd_q_learning.py` & `mpcrl-1.2.0/src/mpcrl/agents/lstd_q_learning.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/agents/rl_learning_agent.py` & `mpcrl-1.2.0/src/mpcrl/agents/rl_learning_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/callbacks.py` & `mpcrl-1.2.0/src/mpcrl/core/callbacks.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/errors.py` & `mpcrl-1.2.0/src/mpcrl/core/errors.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/experience.py` & `mpcrl-1.2.0/src/mpcrl/core/experience.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/exploration.py` & `mpcrl-1.2.0/src/mpcrl/core/exploration.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/learning_rate.py` & `mpcrl-1.2.0/src/mpcrl/core/learning_rate.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/parameters.py` & `mpcrl-1.2.0/src/mpcrl/core/parameters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/schedulers.py` & `mpcrl-1.2.0/src/mpcrl/core/schedulers.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/core/update.py` & `mpcrl-1.2.0/src/mpcrl/core/update.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/util/control.py` & `mpcrl-1.2.0/src/mpcrl/util/control.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/util/iters.py` & `mpcrl-1.2.0/src/mpcrl/util/iters.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/util/math.py` & `mpcrl-1.2.0/src/mpcrl/util/math.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/util/named.py` & `mpcrl-1.2.0/src/mpcrl/util/named.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/log.py` & `mpcrl-1.2.0/src/mpcrl/wrappers/agents/log.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/record_updates.py` & `mpcrl-1.2.0/src/mpcrl/wrappers/agents/record_updates.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/wrappers/agents/wrapper.py` & `mpcrl-1.2.0/src/mpcrl/wrappers/agents/wrapper.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/wrappers/envs/monitor_episodes.py` & `mpcrl-1.2.0/src/mpcrl/wrappers/envs/monitor_episodes.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl/wrappers/envs/monitor_infos.py` & `mpcrl-1.2.0/src/mpcrl/wrappers/envs/monitor_infos.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl.egg-info/PKG-INFO` & `mpcrl-1.2.0/src/mpcrl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpcrl
-Version: 1.1.5.dev1
+Version: 1.2.0
 Summary: Reinforcement Learning with Model Predictive Control
 Author-email: Filippo Airaldi <filippoairaldi@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/FilippoAiraldi/mpc-reinforcement-learning
 Project-URL: Bug Tracker, https://github.com/FilippoAiraldi/mpc-reinforcement-learning/issues
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -20,15 +20,15 @@
 
 **mpcrl** is a library for training model-based Reinforcement Learning (RL) agents with Model Predictive Control (MPC) as function approximation. This framework, also known as MPC-based RL, was first proposed in [[1]](#1) and has so far been shown effective in various applications and with different learning algorithms, e.g., [[2](#2),[3](#3)].
 
 [![PyPI version](https://badge.fury.io/py/mpcrl.svg)](https://badge.fury.io/py/mpcrl)
 [![Source Code License](https://img.shields.io/badge/license-MIT-blueviolet)](https://github.com/FilippoAiraldi/casadi-nlp/blob/release/LICENSE)
 ![Python 3.9](https://img.shields.io/badge/python->=3.9-green.svg)
 
-[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml)
+[![Tests](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-main.yml/badge.svg)](https://github.com/FilippoAiraldi/mpc-reinforcement-learning/actions/workflows/test-experimental.yml)
 [![Downloads](https://pepy.tech/badge/mpcrl)](https://pepy.tech/project/mpcrl)
 [![Maintainability](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/maintainability)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/maintainability)
 [![Test Coverage](https://api.codeclimate.com/v1/badges/9a46f52603d29c684c48/test_coverage)](https://codeclimate.com/github/FilippoAiraldi/mpc-reinforcement-learning/test_coverage)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 ---
```

### Comparing `mpcrl-1.1.5.dev1/src/mpcrl.egg-info/SOURCES.txt` & `mpcrl-1.2.0/src/mpcrl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/tests/test_agent.py` & `mpcrl-1.2.0/tests/test_agent.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/tests/test_core.py` & `mpcrl-1.2.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/tests/test_examples.py` & `mpcrl-1.2.0/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/tests/test_quadrotor_q_learning.py` & `mpcrl-1.2.0/tests/test_quadrotor_q_learning.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/tests/test_util.py` & `mpcrl-1.2.0/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `mpcrl-1.1.5.dev1/tests/test_wrappers.py` & `mpcrl-1.2.0/tests/test_wrappers.py`

 * *Files identical despite different names*

