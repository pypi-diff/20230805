# Comparing `tmp/edc-lab-panel-0.1.8.tar.gz` & `tmp/edc-lab-panel-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-lab-panel-0.1.8.tar", last modified: Sat May  7 02:24:31 2022, max compression
+gzip compressed data, was "edc-lab-panel-0.1.9.tar", last modified: Wed Jul 20 12:01:09 2022, max compression
```

## Comparing `edc-lab-panel-0.1.8.tar` & `edc-lab-panel-0.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.675218 edc-lab-panel-0.1.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/.coveragrc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.669157 edc-lab-panel-0.1.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.671895 edc-lab-panel-0.1.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1745 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1837 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-27 19:26:05.000000 edc-lab-panel-0.1.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     1103 2022-05-07 02:24:31.675353 edc-lab-panel-0.1.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)      214 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.672276 edc-lab-panel-0.1.8/edc_lab_panel/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.673486 edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/
--rw-r--r--   0 erikvw     (501) staff       (20)      156 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2219 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/field_attrs.py
--rw-r--r--   0 erikvw     (501) staff       (20)      993 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/reportable_result_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)      921 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/result_model_mixin_factory.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2474 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/panels.py
--rw-r--r--   0 erikvw     (501) staff       (20)      776 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/processing_profiles.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.673710 edc-lab-panel-0.1.8/edc_lab_panel/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/__init__.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.674988 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-aes-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-aes-restricted.key
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-rsa-local-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-rsa-local-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-rsa-restricted-private.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-rsa-restricted-public.pem
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-salt-local.key
--rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-salt-restricted.key
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.675141 edc-lab-panel-0.1.8/edc_lab_panel/tests/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.8/edc_lab_panel/tests/urls.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:31.672862 edc-lab-panel-0.1.8/edc_lab_panel.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     1103 2022-05-07 02:24:31.000000 edc-lab-panel-0.1.8/edc_lab_panel.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1166 2022-05-07 02:24:31.000000 edc-lab-panel-0.1.8/edc_lab_panel.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-07 02:24:31.000000 edc-lab-panel-0.1.8/edc_lab_panel.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-06-27 19:37:02.000000 edc-lab-panel-0.1.8/edc_lab_panel.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-05-07 02:24:31.000000 edc-lab-panel-0.1.8/edc_lab_panel.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1587 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     2384 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1165 2022-05-07 02:24:31.675666 edc-lab-panel-0.1.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.525766 edc-lab-panel-0.1.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       99 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/.coveragrc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.519755 edc-lab-panel-0.1.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.522648 edc-lab-panel-0.1.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1846 2022-07-20 12:01:01.000000 edc-lab-panel-0.1.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1837 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2021-06-27 19:26:05.000000 edc-lab-panel-0.1.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     1084 2022-07-20 12:01:09.525861 edc-lab-panel-0.1.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)      214 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-07-20 12:01:01.000000 edc-lab-panel-0.1.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.522948 edc-lab-panel-0.1.9/edc_lab_panel/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.524228 edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/
+-rw-r--r--   0 erikvw     (501) staff       (20)      156 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2219 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/field_attrs.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      993 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/reportable_result_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      921 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/result_model_mixin_factory.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2487 2022-07-20 12:01:01.000000 edc-lab-panel-0.1.9/edc_lab_panel/panels.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      776 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/processing_profiles.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.524429 edc-lab-panel-0.1.9/edc_lab_panel/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/__init__.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.525568 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-aes-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-aes-restricted.key
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-rsa-local-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-rsa-local-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)     1678 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-rsa-restricted-private.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      450 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-rsa-restricted-public.pem
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-salt-local.key
+-rw-r--r--   0 erikvw     (501) staff       (20)      256 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-salt-restricted.key
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.525693 edc-lab-panel-0.1.9/edc_lab_panel/tests/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      123 2022-05-07 02:17:26.000000 edc-lab-panel-0.1.9/edc_lab_panel/tests/urls.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-07-20 12:01:09.523587 edc-lab-panel-0.1.9/edc_lab_panel.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1084 2022-07-20 12:01:09.000000 edc-lab-panel-0.1.9/edc_lab_panel.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1166 2022-07-20 12:01:09.000000 edc-lab-panel-0.1.9/edc_lab_panel.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-07-20 12:01:09.000000 edc-lab-panel-0.1.9/edc_lab_panel.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2021-06-27 19:37:02.000000 edc-lab-panel-0.1.9/edc_lab_panel.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-07-20 12:01:09.000000 edc-lab-panel-0.1.9/edc_lab_panel.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1632 2022-07-20 12:01:01.000000 edc-lab-panel-0.1.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     2384 2022-05-07 02:24:23.000000 edc-lab-panel-0.1.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1165 2022-07-20 12:01:09.526171 edc-lab-panel-0.1.9/setup.cfg
```

### Comparing `edc-lab-panel-0.1.8/.github/workflows/build.yml` & `edc-lab-panel-0.1.9/.github/workflows/build.yml`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     name: build (Python ${{ matrix.python-version }}, Django ${{ matrix.django-version }})
     runs-on: ubuntu-latest
 
     strategy:
       fail-fast: false
       matrix:
         python-version: ['3.9']
-        django-version: ['3.2']
+        django-version: ['3.2', '4.0', 'dev']
 
     services:
 
       mysql:
         image: mysql:latest
         env:
           MYSQL_DATABASE: mysql
@@ -23,14 +23,16 @@
         ports:
           - 3306:3306
         options: --health-cmd="mysqladmin ping" --health-interval=10s --health-timeout=5s --health-retries=3
 
     steps:
     - name: Install pycups and words dependency
       run: |
+        sudo sed -i 's/azure\.//' /etc/apt/sources.list
+        sudo apt-get -y update
         sudo apt-get install libcups2-dev wamerican
 
     - uses: actions/checkout@v2
 
     - name: Set up Python ${{ matrix.python-version }}
       uses: actions/setup-python@v2
       with:
```

### Comparing `edc-lab-panel-0.1.8/.gitignore` & `edc-lab-panel-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/LICENSE` & `edc-lab-panel-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/PKG-INFO` & `edc-lab-panel-0.1.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edc-lab-panel
-Version: 0.1.8
+Version: 0.1.9
 Summary: A list of panels typically used for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-panel
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django laboratory panels,clinicedc,clinical trials
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -31,8 +30,7 @@
 * RFT
 * LFT
 * LIPIDS
 * HbA1c
 * Glucose
 
 Also included are normal and graded ranges for the test results in these panels.
-
```

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/field_attrs.py` & `edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/field_attrs.py`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/reportable_result_model_mixin_factory.py` & `edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/reportable_result_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/model_mixin_factory/result_model_mixin_factory.py` & `edc-lab-panel-0.1.9/edc_lab_panel/model_mixin_factory/result_model_mixin_factory.py`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/panels.py` & `edc-lab-panel-0.1.9/edc_lab_panel/panels.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 
 
 rft_panel = RequisitionPanel(
     name="chemistry_rft",
     verbose_name="Chemistry: Renal Function Tests",
     abbreviation="RFT",
     processing_profile=rft_processing,
-    utest_ids=["urea", "creatinine", "uric_acid", "egfr"],
+    utest_ids=["urea", "creatinine", "uric_acid", "egfr", "egfr_drop"],
 )
 
 lipids_panel = RequisitionPanel(
     name="chemistry_lipids",
     verbose_name="Chemistry: Lipids",
     abbreviation="LIPIDS",
     processing_profile=lipids_processing,
```

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/processing_profiles.py` & `edc-lab-panel-0.1.9/edc_lab_panel/processing_profiles.py`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-rsa-local-private.pem` & `edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-rsa-local-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel/tests/etc/user-rsa-restricted-private.pem` & `edc-lab-panel-0.1.9/edc_lab_panel/tests/etc/user-rsa-restricted-private.pem`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel.egg-info/PKG-INFO` & `edc-lab-panel-0.1.9/edc_lab_panel.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: edc-lab-panel
-Version: 0.1.8
+Version: 0.1.9
 Summary: A list of panels typically used for clinicedc/edc projects
 Home-page: https://github.com/clinicedc/edc-lab-panel
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django laboratory panels,clinicedc,clinical trials
-Platform: UNKNOWN
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
@@ -31,8 +30,7 @@
 * RFT
 * LFT
 * LIPIDS
 * HbA1c
 * Glucose
 
 Also included are normal and graded ranges for the test results in these panels.
-
```

### Comparing `edc-lab-panel-0.1.8/edc_lab_panel.egg-info/SOURCES.txt` & `edc-lab-panel-0.1.9/edc_lab_panel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/pyproject.toml` & `edc-lab-panel-0.1.9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 [tool.isort]
 profile = "black"
 py_version = "39"
 skip = [".tox", ".eggs", "migrations"]
 
 [tool.coverage.run]
-parallel = true
+parallel = false
 branch = true
 source = ["edc_lab_panel"]
 
 [tool.coverage.paths]
 source = ["edc_lab_panel"]
 
 [tool.coverage.report]
@@ -28,34 +28,36 @@
 skip_covered = true
 omit = ["requirements.txt"]
 
 [tool.tox]
 legacy_tox_ini = """
 [tox]
 envlist =
-    py{39}-dj{32,dev},
+    py{39}-dj{32,40,dev},
     lint
 isolated_build = true
 
 [gh-actions]
 python =
     3.9: py39, lint
 
 [gh-actions:env]
 DJANGO =
     3.2: dj32, lint
+    4.0: dj40
     dev: djdev
 
 [testenv]
 deps =
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/tox.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/test_utils.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/edc.txt
     -r https://raw.githubusercontent.com/clinicedc/edc/develop/requirements.tests/third_party_dev.txt
     dj32: Django>=3.2,<3.3
+    dj40: Django>=4.0,<4.1
     djdev: https://github.com/django/django/tarball/main
 
 commands =
     pip install -U pip
     pip --version
     coverage run -a runtests.py
     coverage report
```

### Comparing `edc-lab-panel-0.1.8/runtests.py` & `edc-lab-panel-0.1.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-lab-panel-0.1.8/setup.cfg` & `edc-lab-panel-0.1.9/setup.cfg`

 * *Files identical despite different names*

